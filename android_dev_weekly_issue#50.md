layout: post
title: "Android开发技术周报 Issue#50"
date: 2015-09-29 12:38:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#50

### 新闻

1. [Android系统两大漏洞曝光：影响超10亿台设备](http://www.cnbeta.com/articles/435337.htm)

	安全研究人士周四披露了谷歌Android移动操作系统的两大严重漏洞，这些漏洞令超过10亿台Android设备面临被黑的风险。研究人士称，这意味着“几乎每台Android设备”都会受到影响，无论其所搭载的是1.0版本Android系统还是最新的5.0版本。

### 教程

1. [10行配置从Android Studio + Gradle构建体系迁移到facebook的BUCK构建体系](https://github.com/Piasy/OkBuck/blob/master/README-zh.md)

	0行配置从Android Studio + Gradle构建体系迁移到facebook的BUCK构建体系，且保持两者同时兼容使用，编码使用AS，享受安卓最强大IDE的功能，打包、安装、测试用BUCK，享受安卓最快构建系统的畅快淋漓，两者互不干扰。从此妈妈再也不用担心我在编译安卓工程时睡着了，而且真的只要10行！

1. [Android 中 View 炸裂特效的实现分析](http://blog.csdn.net/feelang/article/details/48817145)

	前几天微博上被一个很优秀的 Android 开源组件刷屏了 - ExplosionField，效果非常酷炫，有点类似 MIUI 卸载 APP 时的动画，先来感受一下。ExplosionField 不但效果很拉风，代码写得也相当好，让人忍不住要拿来好好读一下。ExplosionField 继承自 View，在 onDraw 方法中绘制动画特效，并且它提供了一个 attach2Window 方法，可以把 ExplosionField 最为一个子 View 添加到 Activity 上的 root view 中。

1. [Android应用Loaders全面详解及源码浅析](http://blog.csdn.net/yanbober/article/details/48861457)

	在Android中任何耗时的操作都不能放在UI主线程中，所以耗时的操作都需要使用异步实现。同样的，在ContentProvider中也可能存在耗时操作，这时也该使用异步操作，而3.0之后最推荐的异步操作就是Loader。

1. [使用Google官方support-annotation利器](http://mp.weixin.qq.com/s?__biz=MzA3Mjk1MjA4Nw==&mid=209000181&idx=1&sn=d1e6c748e9dd2bd70082c61f525a33db&key=2877d24f51fa5384e78d6e25b21d25936cf6f871251c631e395bef88593babe3e54a7cbac4da307ecc75a0e5bde283fd&ascene=0&uin=MTYzMjY2MTE1&version=11020201&pass_ticket=M8UsXD0Xmx42yegyV3kmzeqq1WhxItjrzlu4NxhPiEY%3D)

	support-annotations是android官方提供的support projects中的一员，提供了非常多有用的annotations来帮助我们提高我们的代码质量和api的健壮性！这个lib非常轻量级，以annotation为主，几乎所有的annotations的Retention都是CLASS,没有任何Runtime overhead，21.0.0总共方法数只有3，而22.2.0增加了Thread、CheckResult等高级支持，总方法数也只有20

1. [Android应用程序通用自动脱壳方法研](http://drops.wooyun.org/tips/9214)

	Android应用程序相比传统PC应用程序更容易被逆向，因为被逆向后能够完整的还原出Java代码或者smali中间语言，两者都具有很丰富的高层语义信息，理解起来更为容易，让程序逻辑轻易暴露给技术能力甚至并不需要很高门槛的攻击者面前。因此Android应用程序加固保护服务随之应运而生。从一开始只有甲方公司提供服务到现在大型互联网公司都有自己的加固保护服务，同时与金钱相关的Android应用程序例如银行等也越来越多开始使用加固保护自己，这个市场在不断的扩大。

1. [美团Android资源混淆保护实践](http://tech.meituan.com/mt-android-resource-obfuscation.html)

	Android应用中的APK安全性一直遭人诟病，市面上充斥着各种被破解或者汉化的应用，破解者可以非常简单的通过破解工具就能对一个APK进行反编译、破解、汉化等等，这样就可以修改原有代码的逻辑、添加新代码、添加或修改资源、或者更有甚者植入病毒等等，从而破坏原有APK的安全和用户体验，最终伤害到用户和原有的开发者。

1. [dexopt的源码跟踪](http://zongwu233.github.io/dexopt-process/)

	一般都是从AndroidStudio run出来的apk安装到手机，这里从 adb shell pm install -r xxx.apk 开始看起：找到android/frameworks/base/cmds/pm/src/com/android/commands/pm/pm.java pm命令的源码，main函数调用了new Pm().run(args);找到 runInstall（）方法
哦刚才的常用参数 "-r" 表示覆盖安装模式 INSTALL_REPLACE_EXISTING，runInstall（）方法最终会调用

1. [其实你不知道MultiDex到底有多坑](http://zongwu233.github.io/the-touble-of-multidex/?)

	遭遇MultiDex，愉快地写着Android代码的总悟君往工程里引入了一个默默无闻的jar然后Run了一下， 经过漫长的等待AndroidStudio构建失败了。

1. [基于Facebook Buck改造Android构建系统之基本概念](http://www.jianshu.com/p/b5958f5fa82f)

	使用Facebook Buck对已有的Android项目进行改造，首先需要理解Buck的一些基本概念，在这个的基础上，我们才能既快又好的进行改造工作。本文就先来介绍4个主要的概念，它们对于编写Buck构建脚本至关重要：构建规则（Build Rule）、构建目标（Build Target）、构建文件（Build File）、构建目标模式（Build Target Pattern）

### 代码&开源库
1. [Init](https://github.com/markzhai/init)

	nit帮助Android应用调度复杂的任务流（如应用初始化流程），如下一节图示的那种任务流，处理类型、优先级、多进程（像是每个进程都会执行application的onCreate），任务依赖，提高应用启动效率。

1. [Timber](https://github.com/naman14/Timber)

	一个很漂亮的Material Design风格音乐播放器。

1. [AndroidTDDBootStrap](https://github.com/Piasy/AndroidTDDBootStrap)

	一个Android TDD 实现项目，使用了一系列表新技术以及最佳实践。

1. [RxPermissions](https://github.com/tbruyelle/RxPermissions)

	一个可让你通过RxJava来操纵Android M permission模型的库。

1. [YahooNewsOnboarding](https://github.com/rahulrj/YahooNewsOnboarding)

	 一个模仿雅虎新闻功能介绍引导效果的Demo。

1. [Pancakes](https://github.com/mattlogan/Pancakes)

	一个可以让你像FragmentManager管理Fragment那样去管理View的库。

1. [smooth-app-bar-layout](https://github.com/henrytao-me/smooth-app-bar-layout)

	Smooth 版本的Google Support Design AppBarLayout。

1. [android-vts](https://github.com/nowsecure/android-vts)	
	Android 安全隐患测试套件。

1. [PianoView](https://github.com/north2014/PianoView)

	仿最美应用的琴键控件。

1. [MIUIv6-UninstallAnimation](https://github.com/kot32go/MIUIv6-UninstallAnimation)

	仿MIUI卸载动画控件 改进使用了贝塞尔曲线，过度更加自然。

1. [ChangeSkin](https://github.com/hongyangAndroid/ChangeSkin)

	基于插件式的Android换肤框架，支持app内和或者外部插件式提供资源的换肤方案，无需重启Activity。

----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)