layout: post
title: "Android开发技术周报 Issue#27"
date: 2015-04-12 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#27

### 教程

1. [Android开发技术前线第五期](https://github.com/bboyfeiyu/android-tech-frontier#2015412--第五期-) ([@MrSimp1e](http://weibo.com/mrsimp1e))

	深入Android图形管道、Romain Guy的性能优化案例、图片加载框架Glide、模仿iOS的模糊视图，都是些不错的文章。

1. [Android内存优化之MAT工具使用教程系列](http://androidperformance.com) ([@高建武_Gracker](http://weibo.com/270099576))

	正所谓工欲善其事，必先利其器，在对Android应用进行内存优化MAT(Memory Analyzer Tool)是一把必不可少的利剑，MAT一个基于Eclipse的内存分析工具，是一个快速、功能丰富的JAVA heap分析工具，它可以帮助我们查找内存泄漏和减少内存消耗。此系列目前有：1. [MAT使用入门](http://androidperformance.com/2015/04/11/AndroidMemory-Usage-Of-MAT/) 2. [MAT使用进阶](http://androidperformance.com/2015/04/11/AndroidMemory-Usage-Of-MAT-Pro/) 3. [打开MAT中的Bitmap原图](http://androidperformance.com/2015/04/11/AndroidMemory-Open-Bitmap-Object-In-MAT/) 三篇文章满满的干货，步骤、注释写的很详细图文并茂，一步步带你走进MAT的世界。

1. [从Fragment被销毁看replace和add的区别](http://blog.fangjie.info/从fragment被销毁看replace和add的区别/) ([@方杰_Jay](http://weibo.com/ncuitstudent))

	首先从一个bug说起 我们都知道fragment切换有两种方式： 1. replace方式transaction.replace(R.id.content, IndexFragment); 2. add－hide－show方式transaction.add(R.id.content, IndexFragment); transaction.hide

1. [使用AIDL实现进程间的通信](http://blog.csdn.net/liuhe688/article/details/6400385) ([@liuhe688](http://blog.csdn.net/liuhe688/))
	AIDL（Android Interface Definition Language）是一种接口定义语言，编译器通过*.aidl文件的描述信息生成符合通信协议的Java代码，我们无需自己去写这段繁杂的代码，只需要在需要的时候调用即可，通过这种方式我们就可以完成进程间的通信工作。

1. [Google利器Android Studio从入门到精通](http://yanbober.github.io/2015/01/28/android_studio_guide/) ([@工匠若水](http://weibo.com/yanbober))

	经过2年时间的研发，Google终于正式发布了面向Android开发者的集成开发环境Android Studio 1.0（稳定版）。Android Studio是Google开发的一款面向Android开发者的IDE， 支持Windows、Mac、Linux等操作系统，基于流行的Java语言集成开发环境IntelliJ搭建而成。该IDE在2013年5月的Google I/O开发者大会上首次露面，当时的测试版各种莫名其 妙的Bug，但是14年12月8日发布的版本是稳定版。

1. [使用Gradle构建Android程序](http://rinvay.github.io/android/2015/04/09/Build-Android-with-Gradle/) ([@Rinvay](http://weibo.com/yunfeitang))

	Android Studio正式版早已经发布了，默认使用Gradle构建，GitHub上80%的Android项目也都是使用Gradle构建的，我们还有什么理由不使用Gradle呢？

1. [Android性能优化后续](http://androidperformance.com/2015/03/31/android-performance-case-study-follow-up/) ([@高建武_Gracker](http://weibo.com/270099576))

	本文是一篇译文，原文Android Performance Case Study Follow-up的作者是大名鼎鼎的Romain Guy。本文讲述了Android性能优化的一些技巧、方法和工具。

1. [JNI/NDK开发指南](http://blog.csdn.net/column/details/blogjnindk.html) [@pleasecallone](http://weibo.com/u/2953984214)

	系统介绍JNI/NDK开发方面的知识及示例，包括各平台环境下JNI开发流程、JNI数据类型、JNI函数查找命名规则、字符串处理、本地代码访问Java的属性和方法、局部引用与全局引用、开发当中常见错误分享、NDK开发环境搭建、NDK编译系统详解和NDK开发综合案例等。

1. [符合Material Design的抽屉导航效果](https://github.com/bboyfeiyu/android-tech-frontier/tree/master/androidweekly/符合Material%20Design的抽屉导航效果) ([@MrSimp1e](http://weibo.com/mrsimp1e))

	现在看来，抽屉式导航已经成为主流导航模式之一。尽管广受批评，但我还是很喜欢该样式，因此我决定在我写的几个app上添加这个控件。这篇文章想通过介绍我觉得抽屉式导航有趣的地方，帮助阅读本文的 Android 开发者们学习到一些知识，同时从其他人的评论中学习到更多的东西。

1. [自动化截图－应用分发时的自动截图方案](https://github.com/bboyfeiyu/android-tech-frontier/tree/master/others/自动化截图－应用分发时的自动截图方案) ([@MrSimp1e](http://weibo.com/mrsimp1e))

	在发布 App 到应用商店时有一件的事情不得不做，就是上传最新的高清无码截图到应用商店上。可是如果你的 App 有许多页面，那你每次发布更新时手动截图将会变的很痛苦，因为你需要一页一页地去截图。为了解决众多 App 开发者的这个痛点，我将在这篇博文中介绍一个实现自动化截图的方法。

1. [深入浅出RxJava三--响应式的好处](http://blog.csdn.net/lzyzsd/article/details/44891933) ([@hi大头鬼hi](http://weibo.com/brucefromsdu))
	
	在第一篇中，我介绍了RxJava的基础知识。第二篇中，我向你展示了操作符的强大。但是你可能仍然没被说服。这篇里面，我讲向你展示RxJava的其他的一些好处，相信这篇足够让你去使用Rxjava.

1. [android apk 防止反编译技术第二篇-运行时修改Dalvik指令](http://my.oschina.net/u/2323218/blog/396203) [@]()

	我们知道apk生成后所有的java生成的class文件都被dx命令整合成了一个classes.dex文件，当apk运行时dalvik虚拟机加载classes.dex文件并且用dexopt命令进行进一步的优化成odex文件。我们的方法就是在这个过程中修改dalvik指令来达到我们的目的。

1. [Kotlin for Android (II)创建一个工程](https://github.com/bboyfeiyu/android-tech-frontier/tree/master/androidweekly/Kotlin%20for%20Android%20(II)创建一个工程) ([@MrSimp1e](http://weibo.com/mrsimp1e))
	当我从w[hat Kotlin is and what it can do for us](http://antonioleiva.com/kotlin-for-android-introduction/)获得一些启发之后,觉得是时候配置下 Android Studio来帮助我们使用Kotlin开发Android应用程序了. 其中有些步骤只需要在初次使用时完成一次, 但是其他一些Gradle配置需要为每一个新项目做一遍. 

1. [Google 出手尝试解决 Android WebView 的碎片化](https://typeblog.net/tech/2015/04/06/google-released-seperate-webview.html) [@颠倒的阿卡林型次元](http://weibo.com/u/1789004515)

	最近可能不少人都在 Google Play Store 上发现了一个新的App: Android System WebView 根据解释，这个是 Android 内置的 WebView 的独立版本。很多人都下载安装了这个App，评论里也有各种奇(xia)葩(bai)评论，说是这个组件非常有效果。Google甚至还建立了一个社群用于发布最新的测试版 WebView。作为一个折腾党，我肯定不能而且没有错过这个App。倒是只有一个问题：WebView 这种组件如何能够独立出来？

### 代码&开源库

1. [WaitingDots](https://github.com/tajchert/WaitingDots)

	![image](https://raw.githubusercontent.com/tajchert/WaitingDots/master/images/dotsLoadingAnimation.gif)

1. [FlipViewPager.Draco](https://github.com/Yalantis/FlipViewPager.Draco)

	Yalantis出品，必属精品啊。

1. [CircleProgress](https://github.com/Fichardu/CircleProgress)

	一个效果很赞的由圆点组成的圆形进度条。

1. [MultiImageSelector](https://github.com/lovetuzitong/MultiImageSelector)

	类似于微里的图片选择器，支持选择单张和多张图片	

1. [ListViewHelper](https://github.com/LuckyJayce/ListViewHelper)

	ListViewHelper. 实现下拉刷新，滚动底部自动加载更多，分页加载，自动切换显示网络失败布局，暂无数据布局，,真正的MVC架构.

1. [android-shapeLoadingView](https://github.com/zzz40500/android-shapeLoadingView)

	高仿新版58 加载动画。

1. [Scrollable](https://github.com/noties/Scrollable)
	
	![image](https://raw.githubusercontent.com/noties/Scrollable/master/sample.gif)

1. [Colorpicker](https://github.com/QuadFlask/colorpicker)
		
	一个漂亮的颜色选择器。
		
### 工具	

1. [Android Studio 1.2 Beta3](http://www.androiddevtools.cn/#android-studio) 

	升级狂魔又来啦，Beta3 Fixed inter-module dependencies are not configured correctly。

1. [Regulex](http://jex.im/regulex/) ([@刘哇勇](http://weibo.com/liuwayong))

	Regulex是一个在线正则表达式可视化工具。

1. [bat](https://github.com/astaxie/bat) ([@ASTA谢](http://weibo.com/533452688))

	[@ASTA谢](http://www.weibo.com/533452688)谢大出品，必属精品啊，bat是一个用Go写的命令行API测试利器，支持文件下载，文件上传，支持Linux的pipe方式，总之就是炫酷。

1. [Roboto](http://roboto.build/)

	Roboto is the easiest way to build and deploy your iOS and Android apps.

1. [ Android Killer](http://www.androiddevtools.cn/#apk-decompile-tools) ([@pwelyn-越狱](http://weibo.com/n/pwelyn-越狱?from=feed&loc=at))
	
	Android Killer 是一款可视化的安卓应用逆向工具，集Apk反编译、Apk打包、Apk签名，编码互转，ADB通信（应用安装-卸载-运行-设备文件管理）等特色功能于一 身。
	
1. [PxCook像素大厨](http://www.fancynode.com.cn)

	PxCook像素大厨,UI设计师效率提升利器，让你专注于设计本质，不再为标注切图而烦恼，从设计到实现一气呵成。支持Win & OS X系统。
	
### 视频

1. [Android性能优化进阶课程](https://www.udacity.com/course/ud825) ([@陈启超_V](http://weibo.com/chenqichao2016))

	Google日前联合Udacity推出了免费的Android性能优化进阶课程，内容主要涉及Android性能问题，如何使用AS各种工具分析和解决性能问题，本着方便国内小伙伴学习的目的，优酷地址：[Android性能优化专辑](http://www.youku.com/playlist_show/id_23631701.html) 课程中文介绍：http://chenqichao.me/2015/04/06/115-Android-Performance/

1. [Tutorial Enhancing Android UI with Custom Views](http://v.youku.com/v_show/id_XODM4NzA3ODMy.html) (@高建武_Gracker)
	
	关于Android自定义View优化的教程，[Ocean-藏心](http://)同学将视频搬到了墙内，并做了中文字幕，值得看看学习学习。同推荐姊妹篇视频[Mastering the Android Touch System](http://v.youku.com/v_show/id_XODQ1MjI2MDQ0.html?from=y1.2-1-87.3.1-2.1-1-1-0)，详细讲解了Android自定义事件处理的方方面面。配合guolin大神CSDN的博客和上一个视频，让你对开发Android自定义控件游刃有余。源码跟PDF地址: http://pan.baidu.com/s/1gd1SDqV
	
### 书

1. [The Mobile Application Hacker's Handbook ](http://www.droidsec.cn/the-mobile-application-hackers-handbook/) ([@DroidSec安卓安全中文站](http://weibo.com/androidsec))

	该书从黑客视角对iOS,Android,Windows Phone及Blackberry等平台的移动应用安全做了透彻的讲解，以让读者了解和掌握常见的移动应用评估，攻击，防御及修复等方法与技巧。感谢[@RAyH4c](http://weibo.com/n/RAyH4c?from=feed&loc=at) 分享的 EPUB 版本下载地址：http://vdisk.weibo.com/s/vGaOF84E9uXU

1. [免费的编程中文书籍索引](http://siberiawolf.com/free_programming/index.html)
	
	免费的编程中文书籍索引
	
	* 国外程序员在 stackoverflow 推荐的程序员必读书籍，[中文版](http://justjavac.com/other/2012/05/15/qualified-programmer-should-read-what-books.html)。
	* stackoverflow 上的程序员应该阅读的非编程类书籍有哪些？ [中文版](https://github.com/justjavac/free-programming-books-zh_CN/blob/master/what-non-programming-books-should-programmers-read.md)
	* github 上的一个流行的编程书籍索引 [中文版](https://github.com/vhf/free-programming-books/blob/master/free-programming-books-zh.md)
			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)