<!--
 * @Author: h2yong@outlook.com
 * @Date: 2020-07-15 15:31:03
 * @LastEditTime: 2020-07-15 15:36:02
 * @LastEditors: Please set LastEditors
 * @Description: Maven打包使用代码版本号和时间戳
-->

为了显示区分部署代码版本，一般会在打包的时候带上 SVN/Git 版本号，如果是多机房部署的，还需要带上机房标签。

若代码发布在 Git 仓库，可以使用 maven 插件 [git-commit-id-plugin](https://github.com/git-commit-id/git-commit-id-maven-plugin)。该插件会产生一个 git.properties 文件，并被包含进最终的 jar 文件中。

简单配置如下：

```xml
<plugin>
   <groupId>pl.project13.maven</groupId>
   <artifactId>git-commit-id-plugin</artifactId>
   <version>2.2.6</version>
   <executions>
       <execution>
           <goals>
               <goal>revision</goal>
           </goals>
       </execution>
   </executions>
   <configuration>
       <!-- 使properties扩展到整个maven bulid 周期
       Ref: https://github.com/ktoso/maven-git-commit-id-plugin/issues/280 -->
       <injectAllReactorProjects>true</injectAllReactorProjects>
       <!--日期格式;默认值:dd.MM.yyyy '@' HH:mm:ss z;-->
       <dateFormat>yyyyMMddHHmmss</dateFormat>
       <!--,构建过程中,是否打印详细信息;默认值:false;-->
       <verbose>true</verbose>
       <!--是否生成"git.properties"文件;默认值:false;-->
       <generateGitPropertiesFile>true</generateGitPropertiesFile>
       <!-- ".git"文件路径;默认值:${project.basedir}/.git; ..表示上一级-->
       <dotGitDirectory>${project.basedir}/../.git</dotGitDirectory>
       <gitDescribe>
           <!--提交操作ID显式字符长度,最大值为:40;默认值:7;0代表特殊意义;-->
           <abbrev>7</abbrev>
           <!--构建触发时,代码有修改时(即"dirty state"),添加指定后缀;默认值:"";-->
           <dirty>-dirty</dirty>
       </gitDescribe>
   </configuration>
</plugin>
```

项目 module 可以配置打包的 finalName 如下：

```xml
<finalName>
    project-module-${dc}-${git.commit.id.abbrev}-${git.build.time}
</finalName>
```

其中 git.commit.id.abbre 是提交 Git 仓库时的版本号缩写，git.build.time 顾名思义是打包时间。

对应的 maven 打包命令如下：

```shell
mvn clean package -Dmaven.test.skip=true -Ddc=$dc -P $dc
```

若有多机房信息，为方便配置，一般会将 profile 配置成机房编码，这样上面的机房 dc 参数和项目 profile 参数即可以共享同一个参数值。

打包时间还可以通过另外一个 maven 插件 [build-helper-maven-plugin](http://www.mojohaus.org/build-helper-maven-plugin/) 读取。

```xml
<plugin>
  <groupId>org.codehaus.mojo</groupId>
  <artifactId>build-helper-maven-plugin</artifactId>
  <version>3.0.0</version>
  <executions>
      <execution>
          <id>timestamp-property</id>
          <goals>
              <goal>timestamp-property</goal>
          </goals>
      </execution>
  </executions>
  <configuration>
      <name>current.time</name>
      <pattern>yyyyMMddHHmmss</pattern>
      <timeZone>GMT+8</timeZone>
  </configuration>
</plugin>
```

上述 current.time 字段值即是打包时间，可以被 pom 文件引用。
