* [json用法](https://groovy-lang.org/json.html)

* [http-builder用法](http://javadox.com/org.codehaus.groovy.modules.http-builder/http-builder/0.6/groovyx/net/http/HTTPBuilder.RequestConfigDelegate.html)
* [HTTPBuilder：使用Groovy操作HTTP资源](https://my.oschina.net/groovyland/blog/3035)

```groovy
import groovy.json.JsonOutput
import groovy.json.StringEscapeUtils
# 将Unicode转为中文
def str= StringEscapeUtils.unescapeJava(JsonOutput.toJson(jsonParams))
# 将中文转为Unicode
# StringEscapeUtils.escapeJava(str)
```

https://chowdera.com/2021/08/20210816015935169Y.html

spock教程

https://spockframework.org/spock/docs/2.0/all_in_one.html

