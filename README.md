[![Codacy](https://api.codacy.com/project/badge/Grade/599a0a3e46f84e6bbc29e8fbe4632860)](https://www.codacy.com/app/getrebuild/rebuild)
[![codecov](https://codecov.io/gh/getrebuild/rebuild/branch/master/graph/badge.svg)](https://codecov.io/gh/getrebuild/rebuild)
[![Package](https://github.com/getrebuild/rebuild/actions/workflows/maven-publish.yml/badge.svg)](https://github.com/getrebuild?tab=packages&repo_name=rebuild)
[![Build Status](https://travis-ci.com/getrebuild/rebuild.svg?branch=master)](https://travis-ci.com/getrebuild/rebuild)
[![License GPLv3](https://img.shields.io/github/license/getrebuild/rebuild.svg)](https://getrebuild.com/legal/service-terms)
[![License 商业授权](https://img.shields.io/badge/license-%E5%95%86%E4%B8%9A%E6%8E%88%E6%9D%83-red.svg)](https://getrebuild.com/legal/service-terms)

## Project Features

**_Compared to similar products, REBUILD focuses more on business needs realization rather than basic technical framework or project startup template. _**

"Open design" is an important design concept of REBUILD! Thanks to the team's mature experience in enterprise management systems, we have achieved configurable management of various daily needs of enterprises, full graphical design and zero-code construction, what you see is what you get.

More details [https://getrebuild.com/](https://getrebuild.com/)

> **Benefits: Join REBUILD VIP user QQ exchange group 819865721 1013051587 GET Usage skills**

## V3.9 new features

This update brings you many functional enhancements and optimizations.

1. [New] Export report trigger
2. [New] Field update and field aggregation support automatic new record creation
3. [New] Custom operation (button)
4. [New] Address book function
5. [New] Chart supports selection of theme color and display unit
6. [New] View all historical approvals of records
7. [New] Multiple FrontJS functions
8. [Optimization] 20+ details/BUG/security updates
9. ...

For more update details, please see [Update log](https://getrebuild.com/docs/dev/changelog)

## Online experience

[https://nightly.getrebuild.com/](https://nightly.getrebuild.com/)

> The default super administrator username and password are `admin` `admin`

## Use

It is very simple to start using REBUILD. There is no need to configure a complex operating environment. Zero dependency and fast deployment!

#### 1. Use the released version

_This method is highly recommended for production environments!!!_

First, [download](https://getrebuild.com/download) the installation package. We provide both `standalone` and `boot` installation packages. `standalone` is an integrated installation package (recommended), and `boot` is the `jar` package of SpringBoot. There is no difference in the functions of the two installation packages.

After downloading, unzip (integrated installation package), start it through `start-rebuild.bat` or `start-rebuild.sh`, and then open the browser and enter [http://localhost:18080/](http://localhost:18080/) to start the experience.

For more details, please refer to the [installation document](https://getrebuild.com/learn/install)

#### 2. Compile from source code

_Note!!! Please use the `master` branch (default branch) for production environments. Other branches are development branches and their functions are uncertain! _

```
# 拉取
git clone --depth=1 https://github.com/getrebuild/rebuild.git

# 编译
mvn package

# 运行
java -jar target/rebuild.jar
```

运行后打开浏览器输入 [http://localhost:18080/](http://localhost:18080/) 开始体验。

## 开发

REBUILD 从 2.0 版本开始支持 `jar` 与 `war` 两种打包/运行模式，两种模式在开发与使用上没有区别。默认情况下使用 SpringBoot `jar` 模式，启动类为 [BootApplication](https://github.com/getrebuild/rebuild/blob/master/src/main/java/com/rebuild/core/BootApplication.java) 。

如你希望使用外部 Tomcat（或其他 Java Web 容器） 即 `war` 方式，请将 `pom.xml` 文件中注释为 `UNCOMMENT USE TOMCAT` 的下一行取消注释。

#### 开发环境

REBUILD 对于开发环境的要求非常简单，由于使用 Java 开发，因此可以运行在几乎所有操作系统上。请按如下清单准备：

- JDK 1.8+（兼容 OpenJDK）
- MySQL 5.6+
- Redis 3.2+（非必须，默认使用内置的 Ehcache 缓存）
- Tomcat 8.0+（非必须，默认使用 SpringBooot 内置 Tomcat）
- Apache Maven 3.6+
- IDEA 或 Eclipse (for JEE)

更多详情请参见 [开发人员文档](https://getrebuild.com/docs/dev/)

## 授权 License

REBUILD 使用 GPL-3.0 开源许可和商业授权双重授权协议，使用将被视为你自愿承诺接受 [用户服务协议](https://getrebuild.com/legal/service-terms) 之所有条款。

REBUILD uses the GPL-3.0 open source license and commercial license dual license agreement. Use will be deemed your voluntary commitment to accept all terms of the [Agreement](https://getrebuild.com/legal/service-terms).

## 购买商业授权

从 2.0 版本开始，REBUILD 将推出 [增值功能](https://getrebuild.com/docs/rbv-features) 计划。如果 REBUILD 对贵公司业务有帮助，请考虑 [购买商业授权](https://getrebuild.com/#pricing-plans) 以支持 REBUILD 可持续发展。除了永久享有全部最新功能以外，还可以得到更专业的技术支持服务。非常感谢！
