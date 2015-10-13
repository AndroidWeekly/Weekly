layout: post
title: "Android开发技术周报 Issue#51"
date: 2015-10-07 09:10:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#51

### 教程

1. [给 Android 开发者的 RxJava 详解](http://gank.io/post/560e15be2dca930e00da1083)

	RxJava 在 GitHub 主页上的自我介绍是 "a library for composing asynchronous and event-based programs using observable sequences for the Java VM"（一个在 Java VM 上使用可观测的序列来组成异步的、基于事件的程序的库）。这就是 RxJava ，概括得非常精准。然而，对于初学者来说，这太难看懂了。因为它是一个『总结』，而初学者更需要一个『引言』。其实， RxJava 的本质可以压缩为异步这一个词。说到根上，它就是一个实现异步操作的库，而别的定语都是基于这之上的。

1. [Android UI：机智的远程动态更新策略](http://t.cn/Ryui1ge)

	做过Android开发的人都遇到过这样的问题：随着需求的变化，某些入口界面通常会出现 UI的增加、减少、内容变化、以及跳转界面发生变化等问题。每次发生变化都要手动修改代码，而入口界面通常具有未读信息提醒这样的“小红点”逻辑；一旦UI变化，“小红点”逻辑也要重新计算。

1. [安装包立减1M--微信Android资源混淆打包工具](http://t.cn/RyuimAu)

	上一篇文章我们讲述了Android减少安装包体积的一些tips,本文主要对前文提到的资源混淆做一个简单的分析。微信中的资源混淆工具主要为了混淆资源ID长度(例如将res/drawable/welcome.png混淆为r/s/a.png)，同时利用7z深度压缩，大大减少了安装包体积，同时也增加了逼格，提升了反破解难度。

1. [React Native For Android 架构初探](http://t.cn/Ry8tFX0)

	 Facebook 在2015.9.15发布了 React Native for Android，把JavaScript 开发技术扩展到了Android平台。React Native 让开发者使用 JavaScript 和 React 编写应用，利用相同的核心代码就可以创建 基于Web，iOS 和 Android 平台的原生应用。本文将浅析Android React的架构及相关基础知识。

1. [Android 6.0 Marshmallow新特性](http://weibo.com/p/1001603895719726554010)

	语境帮助现在就点击：不必离开你正在做的就可以获得帮助，无论你是在一个应用程序或在一个网站
。只需触摸和长按home键。用你的声音做更多：现在你可以与任何支持新语音交互服务的应用程序进行对话。例如，如果一个用户说，“使用TuneIn播放一些音乐，“TuneIn就会问“什么类型的？“。
直接分享：一个快速和容易的方式分享给正确的人在正确的应用程序。

### 代码&开源库

1. [FlycoPageIndicator](https://github.com/H07000223/FlycoPageIndicator)

	PageIndicator其他的实现方式,支持圆角矩形,图片资源以及切换动画。
	
1. [AndroidGameBoyEmulator](https://github.com/pedrovgs/AndroidGameBoyEmulator)

	一个用Java写的Android游戏模拟器。

1. [spoon](https://github.com/INRIA/spoon)	
	一个高质量的 Java 源码分析和转换库。

1. [WindowView](https://github.com/justasm/WindowView)

	Android ImageView you pan by tilting your device.

1. [Android-TopScrollHelper](https://github.com/kmshack/Android-TopScrollHelper)

	一个双击状态栏自动滚动到列表最顶部的动画效果, 支持 ScrollView、NestedScrollView、WebView、ListView和RecyclerView 等多种不同类型的视图。

1. [FabricView](https://github.com/antwankakki/FabricView)

	A new canvas drawing library for Android. 

1. [BottomSheet](https://github.com/Kennyc1012/BottomSheet)	
	BottomSheet支持列表和网格样式、自定义View、Light 和 Dark主题及自定义主题、支持平板、等。

1. [UIBlock](https://github.com/tianzhijiexian/UIBlock/)
	
	代替fragment的轻量级解耦UI的类。

1. [AutoBundle](https://github.com/yatatsu/AutoBundle)	
	一个可以帮你自动生成一些模版代码的库。 

1. [solid](https://github.com/konmik/solid)

	一个支持固定大小容量集合(SolidList, SolidMap, SolidSet)和轻量级data streams的库。

### 工具	

1. [AndResGuard](https://github.com/shwenzhang/AndResGuard)

	Android资源混淆工具。

1. [lint-cleaner-plugin](https://github.com/marcoRS/lint-cleaner-plugin)

	一个可以清理项目中未使用的资源的Gradle Plugin。

1. [screenshot-tests-for-android](https://github.com/facebook/screenshot-tests-for-android)

	screenshot-tests-for-android is a library that can generate fast deterministic screenshots while running instrumentation tests in android.

1. [material-theme-jetbrains](https://github.com/ChrisRM/material-theme-jetbrains)

	JetBrains theme of Material Theme。

###书

1. [C 语言编程透视](https://www.gitbook.com/book/tinylab/cbook/details)

	本书与[《深入淺出 Hello World》](http://blog.linux.org.tw/%7Ejserv/archives/001844.html)有着类似的心路历程，旨在以实验的方式去探究类似 Hello World 这样的小程序在开发与执行过程中的微妙变化，一层层揭开 C 语言程序开发过程的神秘面纱，透视背后的秘密，不断享受醍醐灌顶的美妙。 — 泰晓科技

1. [Shell 编程范例](https://www.gitbook.com/book/tinylab/shellbook/details)

	不同于传统 Shell 书，本书未花大篇幅介绍 Shell 语法，而以面向“对象”的方式引入大量实例介绍 Shell 日常操作，“对象” 涵盖数值、逻辑值、字符串、文件、进程、文件系统等。这样有助于学以致用中加强兴趣。也可作为 Shell 编程索引，随时检索。 — 泰晓科技

----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)