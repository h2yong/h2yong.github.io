# 代码构建 {docsify-ignore-all}

-   [Apache Maven](http://maven.apache.org/)：Maven使用声明进行构建并进行依赖管理，偏向于使用约定而不是配置进行构建。
-   [Gradle](http://www.gradle.org/)：Gradle采用增量构建。Gradle通过Groovy编程而不是传统的XML声明进行配置。Gradle可以很好地配合Maven进行依赖管理。

# 代码分析

-   [Checkstyle](http://checkstyle.sourceforge.net/)：对编程规范和标准进行静态分析。
-   [FindBugs](http://findbugs.sourceforge.net/)：通过字节码静态分析找出潜在Bug。
-   [PMD](http://pmd.sourceforge.net/)：对源代码中不良编程习惯进行分析。
-   [SonarQube](http://www.sonarqube.org/)：通过插件集成其它分析组件，提供评估最终结果报告

# 覆盖率统计

-   [cobertura](https://cobertura.github.io/cobertura/)
-   [jacoco](https://www.jacoco.org/jacoco/)

# 开发库

-   [AspectJ](https://eclipse.org/aspectj/)：面向切面编程扩展，与程序无缝连接。
-   [Auto](https://github.com/google/auto)：源代码生成器集合。
-   [RxJava](https://github.com/ReactiveX/RxJava)：使用JVM中可观察序列，创建异步、基于事件应用程序的函数库。
-   Spring Loaded：另一个JVM类重载代理。
-   [Apache POI](http://poi.apache.org/)：支持OOXML （XLSX、DOCX、PPTX）以及 OLE2 （XLS, DOC or PPT）格式的文档。

# 日志

-   [Apache Log4j2](http://logging.apache.org/log4j/2.x/)：对之前版本进行了完全重写。现在的版本具备一个强大的插件和配置架构。
-   [Logback](http://logback.qos.ch/)：Log4j原班人马作品。被证明是一个强健的日志函数库，通过Groovy提供了很多有意思的配置选项。
-   [SLF4J](http://www.slf4j.org/)：日志抽象层，需要与某个具体日志框架配合使用。
-   [kibana](https://www.elastic.co/products/kibana)：对日志进行分析并进行可视化。
-   [logstash](https://www.elastic.co/products/logstash)：日志文件管理工具。

# 网络编程函数库

-   [Netty](http://netty.io/)：构建高性能网络应用程序开发框架。
-   [OkHttp](http://square.github.io/okhttp/) ：一个Android和Java应用的HTTP+SPDY客户端。

# 搜索

-   [Apache Solr](http://lucene.apache.org/solr/)：一个完全的企业搜索引擎。为高吞吐量通信进行了优化。
-   [Elasticsearch](https://www.elastic.co/)：一个分布式、支持多租户（multitenant）全文本搜索引擎。提供了RESTful Web接口和无schema的JSON文档。

# 安全

-   [Apache Shiro](http://shiro.apache.org/)：执行认证、授权、加密和会话管理。
-   [Spring Security](http://projects.spring.io/spring-security/)：专注认证、授权和多维度攻击防护框架。

# 测试

-   [assertj](http://joel-costigliola.github.io/assertj/)：支持流式断言提高测试的可读性
-   [junit](http://junit.org/junit4/)：单元测试框架。
-   [testng](http://testng.org/doc/index.html)：单元测试框架。
-   [mockito](http://code.google.com/p/mockito/)：在自动化单元测试中创建测试对象，为TDD或BDD提供支持
-   [powermock](https://github.com/powermock/powermock)：PowerMock扩展了EasyMock和Mockito框架，增加了对static和final方法mock支持等功能
-   [Selenium](http://docs.seleniumhq.org/)：为Web应用程序提供可移植软件测试框架。
-   [rest-assured](http://rest-assured.io/)：rest服务测试框架
-   [karate](https://github.com/intuit/karate)：Web-Services Testing Made Simple
-   [fitnesse](http://www.fitnesse.org/FitNesseFeatures)：使用wiki的测试框架
-   [jbehave](http://jbehave.org)：行为驱动开发测试框架
-   [dbunit](http://dbunit.sourceforge.net/)：junit插件，用于数据库单元测试
-   [spring-test-dbunit](https://github.com/springtestdbunit/spring-test-dbunit)
-   [htmlunit](http://htmlunit.sourceforge.net/)：HtmlUnit是JUnit的扩展测试框架之一，用于html单元测试
-   [httpunit](http://httpunit.sourceforge.net/)：HttpUnit对网络应用程序进行自动完善和测试的JAVA类库程序
-   [unitils](http://www.unitils.org/)：单元测试整合，基础dbunit、spring test等
-   [JTester](https://code.google.com/archive/p/java-tester/)：JTester是站在众多巨人肩膀上的单元测试框架，集成了Junit4.5，dbunit2.4.3，unitils2.2，JMOCK2.5和TestNg5.1这些优秀的开源框架
-   [spock](http://spockframework.org)：Spock框架是基于Groovy语言的测试框架，Groovy与Java具备良好的互操作性，因此可以在Spring Boot项目中使用该框架写优雅、高效以及DSL化的测试用例
-   [nosql-unit](https://github.com/lordofthejars/nosql-unit)：NoSQL Unit is a JUnit extension that helps you write NoSQL unit tests
-   [assertj-db](http://joel-costigliola.github.io/assertj/assertj-db.html)：数据库流式断言
-   [JUnitParams](https://github.com/Pragmatists/JUnitParams)：java参数化测试
-   [truth](https://github.com/google/truth)：来自Google用于Java单元测试断言/命题框架
-   [test4j](https://github.com/test4j/test4j): an open source for java test

# 性能测试

-   <http://naver.github.io/ngrinder/>
-   <http://gettaurus.org/>
-   <http://grinder.sourceforge.net>
-   <http://locust.io>

# Web框架

-   [Spring](http://projects.spring.io/spring-framework/)：旨在简化Java EE的开发过程，提供依赖注入相关组件并支持面向切面编程。
-   [Spring MVC](http://projects.spring.io/spring-framework/)：Spring MVC属于SpringFrameWork的后续产品。
-   [spring-boot](http://projects.spring.io/spring-boot/)：微框架，简化了Spring新程序的开发过程。
-   [Swagger](http://swagger.io/)：Swagger是一个规范且完整的框架，提供描述、生产、消费和可视化RESTful Web Service。

# 网络爬虫

-   [Apache Nutch](http://nutch.apache.org/)：可用于生产环境的高度可扩展、可伸缩的网络爬虫。
-   [Crawler4j](https://code.google.com/p/crawler4j/)：简单的轻量级爬虫。
-   [JSoup](http://jsoup.org/)：抓取、解析、操作和清理HTML。

# 服务器

-   [Apache Tomcat](http://tomcat.apache.org/)：针对Servlet和JSP的应用服务器，健壮性好且适用性强。
-   [Jetty](http://www.eclipse.org/jetty/)：轻量级、小巧的应用服务器，通常会嵌入到项目中。
-   [undertow](https://github.com/undertow-io/undertow): 基于NIO实现的高并发轻量级的服务器

# 内存数据库

-   [H2](http://h2database.com/html/main.html)：小型SQL数据库，以内存操作著称。

# 数据库更新工具

-   <https://www.liquibase.org/>，文档：<https://www.liquibase.org/documentation/changes/create_table.html>
-   <https://flywaydb.org/>

# 数据库连接池

-   <https://github.com/alibaba/druid>
-   <https://github.com/brettwooldridge/HikariCP>

# ORM框架

-   <http://www.mybatis.org>
-   mybatis插件：<http://mp.baomidou.com/> 
-   mybatis插件：<http://www.mybatis.tk/>
-   <https://www.jooq.org/>

# 数据库读写分离框架

-   <http://shardingjdbc.io/index_zh.html>

# java定时任务开源框架

<http://www.quartz-scheduler.org/>

# 分布式定时任务开源框架

-   <http://elasticjob.io/docs/elastic-job-lite/00-overview>
-   <https://github.com/ltsopensource/light-task-scheduler>
-   <http://code.taobao.org/p/tbschedule/wiki/index>
-   <https://github.com/uncodecn/uncode-schedule>

# 内嵌式NoSQL

-   <https://github.com/mwarc/embedded-memcached-spring>
-   <https://github.com/kstyrc/embedded-redis>

# 分布式缓存

-   [Hazelcast](https://hazelcast.org/)：Highly scalable in-memory datagrid with a free open-source version.

# mock-server框架

<http://www.mock-server.com/>
<https://github.com/dreamhead/moco>

# 微服务脚手架

-   [jhipster](http://www.jhipster.tech/)，中文指南：<https://www.jhipster-cn.tech>，开发笔记：<https://jh.jiankangsn.com/>
-   [阿里出品nacos](https://qbgbook.gitbooks.io/spring-boot-reference-guide-zh/content/)
-   [阿里出品sofa](https://www.sofastack.tech/)
-   <https://github.com/thinkgem/jeesite>
-   <http://git.oschina.net/jeecg/jeecg>
-   <http://git.oschina.net/naan1993/guns>
-   <http://git.oschina.net/ixion/NUTZ-ONEKEY>
-   <http://git.oschina.net/babaio/renren-security>
-   <http://git.oschina.net/babaio/renren-security-boot>
-   <https://www.oschina.net/p/apollo-ctrip>
-   <https://gitee.com/iBase4J/iBase4J>

# jsp布局框架

<https://github.com/sitemesh/sitemesh3>

# java工具包

-   <https://gitee.com/loolly/hutool>
-   <http://feilong-core.mydoc.io>

# json工具包

-   [Jsonpath](https://github.com/json-path/JsonPath)
-   [fastjson](https://github.com/alibaba/fastjson)
-   [gson](https://github.com/google/gson)

# java内嵌nodejs

-   <https://github.com/nodyn/nodyn>
-   <https://github.com/apigee/trireme>
-   <https://github.com/eclipsesource/J2V8>

# 全栈虚拟机

<https://www.graalvm.org/>

# java优秀项目

-   [jenkins-client](https://github.com/RisingOak/jenkins-client.git)
-   [java-gitlab-api](https://github.com/timols/java-gitlab-api.git)
-   [mycat：mysql中间件](http://mycat.io/)
-   [cobar：mysql中间件](https://github.com/alibaba/cobar.git)

# spring相关文章

-   [spring-common-application-properties](https://docs.spring.io/spring-boot/docs/current/reference/html/common-application-properties.html)
-   [使用spring-boot封装j360](https://github.com/xuminwlt/j360-boot)
-   [Spring Boot集成MyBatis的基础项目](https://github.com/abel533/MyBatis-Spring-Boot)
-   [Spring Boot参考指南](https://qbgbook.gitbooks.io/spring-boot-reference-guide-zh/content/)
-   [Java通过URLClassLoader让程序支持插件扩展](http://xxgblog.com/2013/07/04/java-urlclassloader-plugin/)

# 单元测试文章

-   <https://skyao.gitbooks.io/learning-java-unit-test/content/assertj/>
-   <https://skyao.gitbooks.io/learning-java-unit-test/content/powermock/>
-   <https://skyao.gitbooks.io/learning-java-unit-test/content/mockito/>
-   <https://github.com/kkapelon/java-testing-with-spock>
-   [测试框架热门度和活跃度](https://java.ctolib.com/article/compares/2035)

# 优秀java相关资料

-   <http://www.mybatis.org/mybatis-3/zh/dynamic-sql.html>  
-   <http://git.oschina.net/free/Mybatis_Utils/blob/master/MybatisGeneator/MybatisGeneator.md> 

# awesome-java

<https://github.com/akullpp/awesome-java>

# 页面性能测试工具

**基于网页分析工具：**

1.  <https://www.webpagetest.org/>
2.  <https://www.pingdom.com/>
3.  <https://gtmetrix.com/>
4.  [showslow](https://github.com/sergeychernyshev/showslow/wiki)

**基于浏览器分析工具：**

1.  Chrome自带工具F12
2.  Firefox插件：YSlow（Yahoo工具）
3.  Page Speed（google）

# API测试工具

-   <https://www.runscope.com/docs/api-testing/scripts/post-response/>
-   [面向多端的自动化测试Macaca](https://macacajs.github.io/zh/)

# 开源git web工具

| 工具名称                                          | Language |
| --------------------------------------------- | -------- |
| [gitlab](https://about.gitlab.com/)           | ruby     |
| [gitblit](http://gitblit.com/)                | java     |
| [gitbucket](https://gitbucket.github.io/)     | java     |
| [gitiles](https://github.com/google/gitiles/) | java     |
| [gerrit](https://www.gerritcodereview.com/)   | java     |

# 云服务

-   <http://rancher.com/catalog-items/>
-   [阿里云效平台](http://yunxiao.aliyun.com)
-   [MQC-阿里移动质量中心](https://mqc.aliyun.com/)
-   [FTS-前端测试服务](http://fts.aliyun.com)
-   [百度移动云测试中心](http://mtc.baidu.com)
-   [WeTest腾讯质量开放平台](http://wetest.qq.com/)
-   [腾讯优测云测试平台](http://utest.qq.com/)
-   [OneAPM-端到端的应用性能管理软件云解决方案](https://www.oneapm.com/index.html)
-   [Heroku](https://www.heroku.com/)
-   [appfog](https://www.ctl.io/appfog/)
-   [cloudbees](https://www.cloudbees.com/)
-   [OpenShift](https://www.openshift.com/)
-   [Mendix](https://www.mendix.com/)
-   [MioSoft](https://www.miosoft.com/)
-   [Engine Yard Cloud](http://www.engineyard.com/)

# 接口测试文章收集

-   <https://www.kancloud.cn/digest/dqappinterface/120089>
-   [有赞分层自动化测试实践](http://tech.youzan.com/layers_test_automation_practice/)
-   [接口测试-分层测试重构之接口层](https://testerhome.com/topics/4284)
-   [PhoenixFramework自动化测试平台](http://www.cewan.la/)
-   [自动化测试工具 Fitnesse+RestFixture](https://testerhome.com/topics/1277)

# 移动跨平台开发

-   <https://github.com/NervJS/taro>
-   <https://github.com/Meituan-Dianping/mpvue>
-   <https://uniapp.dcloud.io/>

# PC跨平台开发

<https://electronjs.org/>

# 开发工具使用教程

-   [猴子都能懂的GIT入门](https://backlog.com/git-tutorial/cn/)
-   [IntelliJ IDEA 使用教程](http://wiki.jikexueyuan.com/project/intellij-idea-tutorial/)

# devops平台

-   [jenkins](https://jenkins.io/zh/)
-   [TFS](https://visualstudio.microsoft.com/zh-hans/tfs/)

# 学习网站

-   [w3cschool](https://www.w3cschool.cn/)

# 服务编排

-   <https://github.com/Netflix/conductor>
