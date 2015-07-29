这一章介绍了作者开发Ninja的动机，和目前Ninja所具有的特性，最后还列出了贡献者的名单，并简单地说明了社区的管理方式。

###动机
作者提到了一些目前主流的Java Web框架，都是我们比较熟悉的。其中特别说明了Play framework的1和2，在我看来Ninja和Play framework也是有很大的相似性的。但是这些框架都不能满足他们在当前工作场景下开箱即用的功能需求，所以在2012年的时候他们决定开发自己的框架。
他们团队对web framework需求的主要特性为：

* Restful
* 纯Java实现
* 依赖注入
* 超短开发周期
* 简单快速的测试（单元测试和集成测试）
* 构建系统
* 命令行工具
* 表单验证和解析
* 权限验证
* 方便发布到GAE

###特性
Ninja是一个全栈的集成框架，用到了大量的第三方库。
特性概括：

#### 开发
* 开发和构建支持，包括良好的IDE支持
* 无需重启的代码重加载

#### 前端
* 基于Freemarker的HTML渲染
* 基于Jackson的Json解析和渲染
* 基于Jackson的XML解析和渲染

#### 有状态的Restful
* 客户端Session
* Flash作用域

#### 核心库
* 依赖注入
* 多重环境配置
* 国际化
* 生命周期
* 邮件
* 定时器
* 基于Hibernate-validation的对象验证
* 基于Google Guava的基础类库
* 基于slf4j和logback的日志

#### 关系型数据库
* 基于Hibernate的JPA
* 基于FlyWayDB的数据库迁移

#### 缓存
* Memcached
* EhCache

#### 测试
* 基于Mockito的单元测试
* NinjaTest
* 基于DocTester的NinjaDocTester
* 基于FluentLenium的NinjaFullentLeniumTest（这个不知道是什么）

#### 发布
* WAR文件
* 包装了Jetty的可执行Jar
* 顺序编程风格（非异步）

### 贡献
目前Nanjia的开发由[FinalFrontierLabs](http://www.finalfrontierlabs.com/)团队和[Raphael](http://raphaelbauer.com/)领导。
