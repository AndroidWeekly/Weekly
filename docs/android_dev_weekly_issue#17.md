---
layout: post
title: "Android开发技术周报 Issue#17"
date: 2015-01-19 13:48:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#17
	
### 教程

1. [ART运行时垃圾收集（GC）过程分析](http://blog.csdn.net/luoshengyang/article/details/42555483)

	ART运行时与Dalvik虚拟机一样，都使用了Mark-Sweep算法进行垃圾回收，因此它们的垃圾回收流程在总体上是一致的。但是ART运行时对堆的划分更加细致，因而在此基础上实现了更多样的回收策略。不同的策略有不同的回收力度，力度越大的回收策略，每次回收的内存就越多，并且它们都有各自的使用情景。这样就可以使得每次执行GC时，可以最大限度地减少应用程序停顿。本文就详细分析ART运行时的垃圾收集过程。

1. [如何调试 Android 上 HTTP(S) 流量](http://greenrobot.me/devpost/how-to-debug-http-and-https-traffic-on-android/)

	在Android开发中我们常常会和API 打交道，可能你不想，但是这是避不开的。大部分情况下，调试发送网络请求和接收响应的过程都是十分痛苦的。有多少次我们经过调试发现API的调用失败仅仅是因为我们的编码错了或者丢失了一个HTTP头部参数？在调试的过程中，我们发现出现错误的原因千奇百怪。

1. [ART运行时为新创建对象分配内存的过程分析](http://blog.csdn.net/luoshengyang/article/details/42492621)

	 ART运行时和Dalvik虚拟机一样，在堆上为对象分配内存时都要解决内存碎片和内存不足问题。内存碎片问题可以使用dlmalloc技术解决。内存不足问题则通过垃圾回收和在允许范围内增长堆大小解决。由于垃圾回收会影响程序，因此ART运行时采用力度从小到大的进垃圾回收策略。

1. [Android性能优化典范](http://hukai.me/android-performance-patterns/)

	2015年伊始，Google发布了关于Android性能优化典范的专题，一共16个短视频，每个3-5分钟，帮助开发者创建更快更优秀的Android App。课程专题不仅仅介绍了Android系统中有关性能问题的底层工作原理，同时也介绍了如何通过工具来找出性能问题以及提升性能的建议。主要从三个方面展开，Android的渲染机制，内存与GC，电量优化。下面是对这些问题和建议的总结梳理。

<!--more-->

1. [50个Android开发技巧(20 使用MVP模式)](http://blog.csdn.net/vector_yi/article/details/24719873)

	 随着UI创建技术的功能日益增强，UI层也履行着越来越多的职责。为了更好地细分视图(View)与模型(Model)的功能，让View专注于处理数据的可视化以及与用户的交互，同时让Model只关系数据的处理，基于MVC概念的MVP(Model-View-Presenter)模式应运而生。
	
1. [Android Developer Tools(开发人员工具)](http://yanghui.name/blog/2015/01/20/android-developer-tools/)
	
	在做Android开发的过程中，不可避免地需要使用到自带的android developer tools（开发人员工具），这是一个强大的开发辅助工具，随着android版本的更新，developer tools也集成了越来越多十分方便的调试功能，这里以android 4.4.4版本为例子，说说其中一部分我常用工具的使用.

1. [GitHub秘籍](https://github.com/tiimgreen/github-cheat-sheet/blob/master/README.zh-cn.md)
	
	本秘籍收录了一些Git和Github非常酷同时又少有人知的功能。同时有英文、韩文、日文版本。

1. [Gradle自定义你的BuildConfig](http://stormzhang.com/android/2015/01/25/gradle-build-field/)

	在很早之前我发布了这篇博客[Android BuildConfig.DEBUG的妙用](http://stormzhang.com/android/2013/08/28/android-use-build-config/), 提到了Eclipse中通过BuildConfig.DEBUG字段用来调试Log非常好用，但是殊不知在Android Studio中通过Gradle这种用法更加强大。

1. [Google Guava官方教程（中文版）](http://ifeve.com/google-guava/)

	Guava工程包含了若干被Google的 Java项目广泛依赖 的核心库，例如：集合 [collections] 、缓存 [caching] 、原生类型支持 [primitives support] 、并发库 [concurrency libraries] 、通用注解 [common annotations] 、字符串处理 [string processing] 、I/O 等等。 所有这些工具每天都在被Google的工程师应用在产品服务中。

1. [Java里快如闪电的线程间通讯](http://www.infoq.com/cn/articles/High-Performance-Java-Inter-Thread-Communications)

	创建一个对开发人员友好的、简单轻量的线程间通讯框架，完全不用锁、同步器、信号量、等待和通知，在Java里开发一个轻量、无锁的线程内通讯框架；并且也没有队列、消息、事件或任何其他并发专用的术语或工具。


### 代码&开源库

1. [bitmapMesh](https://github.com/7heaven/bitmapMesh)

	一个实现窗帘效果的库。
	
	![image](https://raw.githubusercontent.com/7heaven/bitmapMesh/master/arts/arts2.gif)

1. [AndroidIndicators](https://github.com/MoshDev/AndroidIndicators)

	一个可以给Title增效动画效果的库，已实现效果有左右切换、上下切换和3D切换效果。
	
	![image](https://raw.githubusercontent.com/MoshDev/AndroidIndicators/master/snapshots/2015-01-12%2019_42_02.gif)
	
1. [Zhihu-Parallax-Animation](https://github.com/ryanhoo/Zhihu-Parallax-Animation)

	知乎 Android 客户端启动页的视差动画效果实现.
	
	![image](https://raw.githubusercontent.com/ryanhoo/Zhihu-Parallax-Animation/develop/images/zhihu-parallax-animation.gif)

1. [TutorialView](https://github.com/itzikBraun/TutorialView)

	一个方便你给Activity添加功能说明的库。

	![image](https://camo.githubusercontent.com/3ccafa15f750a95fa01b88b16077af5431e22f06/687474703a2f2f7261772e6769746875622e636f6d2f49747a696b427261756e2f5475746f7269616c566965772f6d61737465722f73637265656e5f73686f74732f6578616d706c652e676966)

1. [android-pathview](https://github.com/geftimov/android-pathview)

	
	一个可以显示路径动画的自定义View，同时也支持从SVG文件加载路径动画。
	
	![image](https://raw.githubusercontent.com/geftimov/android-pathview/master/art/settings.gif)

1. [NetworkEvents](https://github.com/pwittchen/NetworkEvents)
	
	一个监听网络连接状态并且可以改变Wifi信号强度的库。	
	
1. [RecyclerView-FlexibleDivider](https://github.com/yqritc/RecyclerView-FlexibleDivider)
	
	一个方便你控制RecyclerView中Item之间分割线样式的库。
	
	![image](https://raw.githubusercontent.com/yqritc/RecyclerView-FlexibleDivider/master/sample/sample1.gif)![image](https://raw.githubusercontent.com/yqritc/RecyclerView-FlexibleDivider/master/sample/sample2.gif)

1. [Instagram_Filter](https://github.com/yulu/Instagram_Filter)
	
	一个使用OpenGL ES Shaders模仿了Instagram滤镜效果的项目。

1. [StikkyHeader](https://github.com/carlonzo/StikkyHeader)

	This is a very simple library for Android that allows you to stick an header to a scrollable view and easly apply animation to it
	
	这是一个非常简单的库，可以让你轻松的给你一个可滚动的View添加stick Header并且可以添加动画效果。
	
	![image](https://raw.githubusercontent.com/carlonzo/StikkyHeader/develop/readme/example1.gif)![image](https://raw.githubusercontent.com/carlonzo/StikkyHeader/develop/readme/example2.gif)

1. [socket.io-android-chat](https://github.com/nkzawa/socket.io-android-chat)

 	一个Socket.io的Demo项目。	
	
### 工具	 

1. [Android Studio 1.1 Preview 2](http://www.androiddevtools.cn)

	本次主要更新：
	
	1. Lint工具新增了几条检查规则。
	1. 又修复了十几个Bug。 
	
	具体更新详情见[Android Studio 1.1 Preview 2 Release Notes](http://photo.weibo.com/5214309031/wbphotos/large/mid/3803387382973701/pid/005GSHYzjw1eona47dj7wj31kw2qe4qp)
	
1. [gradle-advanced-build-version](https://github.com/moallemi/gradle-advanced-build-version)

	可以帮你自动生成版本号和版本名称的插件。

### 视频

1. [百度地图在Android中的使用](http://www.imooc.com/view/238?from=itblog)

	课程使用百度地图SDK，由浅入深的带领大家从申请百度地图API Key开始，一步一步实现地图在APP中的常见的功能，总体包括地图的引入、基本设置、模式的切换、定位的功能、方向传感器的结合、以及添加覆盖物。

# 设计
### 教程

1. [重磅教程！帮你全面彻底搞定MATERIAL DESIGN的学习笔记](http://www.uisdc.com/comprehensive-material-design-note#368390-tsina-1-73915-ebfdadd9b239798c6a2035c828aafd11)
	
	自从Material design发布以来，可乐橙就在一直收集相关素材与资源，研究别人的作品。这套设计风格非常鲜明，带有浓郁的Google式严谨和理性哲学，深得我心。

1. [小技巧！利用PS CS6的新功能保持ICON细节饱满完美](http://www.uisdc.com/ps-icon-pixel-perfect#)

	一些本来尺寸很大，质量很不错的高清png图片，经过缩小转为icon时却变得惨不忍睹。这对于高清控与细节控来说简直没法忍，今天分享一篇关于利用Photoshop cs6网格对齐功能绘制高清icon的文章。

### 资源

1. [Awesome-Sketch](https://gitcafe.com/riku/Awesome-Sketch)
	
	这是一份为想学 Sketch 的设计师、前端工程师们准备的不完全列表，包含了 Sketch 视频、文章、手册等。
		
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)