###创建第一个Ninja项目

####使用Maven archetypes创建一个起步项目

首先肯定是要安装jdk与maven的，这里推荐的是jdk 1.7。
Maven archetypes只要一个命令就可以完成起步项目的创建。
```
mvn archetype:generate -DarchetypeGroupId=org.ninjaframework -DarchetypeArtifactId=ninja-servlet-archetype-simple
```
然后会搜索远程仓库并下载依赖文件和创建项目文件，在此过程中它会要求你输入groupid和artifactId。
Ninja为我们提供了一“超级开发模式(SuperDevMode)”，在完成项目的创建后只需要运行mvn ninja:run就可以启动它。在该模式下允许代码的热加载，极大地方便了开发和调试。

####导入到IDE
导入的过程和其他maven项目导入是一样的，我测试时导入的是idea。在我使用idea的Maven面板运行ninja:run的时候出了点问题。通过阅读错误提示，我发现原来是idea使用的
maven版本太低导致的。ninja项目要求Maven版本高于3.1。在手动指定了Maven安装目录后运行成功，在localhost:8080页面看到了helloworld。

####ninja项目的结构
Ninja的理念是“约定优于配置”，如果所有的文件都在它该待的位置，那么它就会自动为我们做许多工作。

Ninja的目录结构是标准mvc，感觉和RubyOnRails有许多相似之处。
