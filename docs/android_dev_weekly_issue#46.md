layout: post
title: "Android开发技术周报 Issue#46"
date: 2015-08-24 23:38:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#46

### 教程

1. [剖析Android中进程与线程调度之nice](http://droidyue.com/blog/2015/09/05/android-process-and-thread-schedule-nice/)

	在计算机操作系统中，进程是进行资源分配和调度的基本单位，同时每个进程之内也可以存在多个线程。那么在Android系统（Linux Kernel）中，进程是如何去抢占资源，线程又是如何根据优先级切换呢，本文将尝试剖析这个问题，研究nice在Linux以及Android系统中的应用。

1. [Android微信智能心跳方案](https://mp.weixin.qq.com/s?__biz=MzAwNDY1ODY2OQ==&mid=207243549&idx=1&sn=4ebe4beb8123f1b5ab58810ac8bc5994)

	本方案的主要目标是，在尽量不影响用户收消息及时性的前提下，根据网络类型自适应的找出保活信令TCP连接的尽可能大的心跳间隔，从而达到减少安卓微信因心跳引起的空中信道资源消耗，减少心跳Server的负载，以及减少部分因心跳引起的耗电。

1. [Android M 新的运行时权限开发者需要知道的一切](http://jijiaxin89.com/2015/08/30/Android-s-Runtime-Permission/)

	android在不断发展，最近的更新 M 非常不同，一些主要的变化例如运行时权限将有颠覆性影响。惊讶的是android社区鲜有谈论这事儿，尽管这事很重要或许在不远的将来会引发很严重的问题。
这是今天我写这篇博客的原因。这里有一切关于android运行时权限你需要知道的，包括如何在代码中实现。

1. [Gradle 用法总结](http://jijiaxin89.com/2015/08/29/gradle-use-note/)

	用过android studio的对gradle应该都不陌生了，gradle文件的基本配置大同小异，略做了解使用应该是没什么问题了。但是深入细致的了解一下对于理解项目还是很有帮助的，尤其是遇到一些配置复杂的github项目，不了解gradle可能会遇到跑不起来又束手无策的情形。下面对gradle相关知识、用法做一下总结。

1. [谈谈App混合开发](http://bxbxbai.gitcafe.io/2015/08/16/talk-about-bybird-app/)

	混合开发的App（Hybrid App）就是在一个App中内嵌一个轻量级的浏览器，一部分原生的功能改为Html 5来开发，这部分功能不仅能够在不升级App的情况下动态更新，而且可以在Android或iOS的App上同时运行，让用户的体验更好又可以节省开发的资源。

1. [Gradle与Makefile构建工具的对比](http://ticktick.blog.51cto.com/823160/1688586)

	随着Android Studio的普及，越来越多的Android开发者也要开始了解和学习Gradle这款强大的代码构建工具了。我们在学习和了解一项新事物的时候，最快速的方法往往是与已知的事物进行比较，对于熟悉Makefile编译机制的Linux程序员而言，认识和掌握Gradle最好的方法莫过于比较它们之间的区别了，本文不准备详细介绍Gradle的方方面面，而是希望通过与Makefile的对比帮助Gradle初学者更快速地理解Gradle的基础和原理。

1. [Drawable 着色的后向兼容方案](http://www.race604.com/tint-drawable/)

	看到 [Android Weekly]() 最新一期有一篇文章：[Tinting drawables](http://andraskindler.com/blog/2015/tinting_drawables/)，使用 ColorFilter 手动打造了一个 TintBitmapDrawable，之前也看到有些文章使用这种方式来实现 Drawable 着色或者实现类似的功能。但是，这种方案并不完善，本文将介绍一个完美的后向兼容方案。

1. [Android应用资源文件格式解析与保护对抗研究](http://www.freebuf.com/articles/terminal/75944.html)

	apktool是Android分析中会用到的一个重要的开源工具,但是apktool的使用者的增加,相应的对抗apktool的手段也开始日益增加。 anti apktool的方法有很多,不过一般都是针对.dex的反编译做处理,这次在分析某样本时遇到了比较有意思的针对.arsc文件做处理,造成apktool解包失败的手段。本着学习研究的目的,进行了本次anti apktool的研究。
	
1. [Android OkHttp完全解析 是时候来了解OkHttp了](http://blog.csdn.net/lmj623565791/article/details/47911083)

	本篇博客首先介绍okhttp的简单使用，主要包含：一般的get请求、一般的post请求、基于Http的文件上传、文件下载、加载图片、支持请求回调，直接返回对象、对象集合、支持session的保持等。

### 代码&开源库

1. [ExtendedTouchView](https://github.com/lnikkila/ExtendedTouchView)

	一个可以增加控件触摸区域的View。

1. [CustomMenu](https://github.com/flyfei/CustomMenu)

	CustomMenu是一个自定义的控件，可以帮助你快速创建Menu，支持只用左菜单，只用右菜单，左右菜单一起用，左右菜单都不用,CustomMenu相当于是一个布局
	
1. [MaterialTextField](https://github.com/florent37/MaterialTextField)

	一个漂亮的Floating Edit Text。

1. [CollapsingAvatarToolbar](https://github.com/Sloy/CollapsingAvatarToolbar)	
	一个可折叠的Toolbar。

1. [DroidPlugin](https://github.com/Qihoo360/DroidPlugin)

	DroidPlugin 是360手机助手在Android系统上实现了一种新的插件机制:它可以在无需安装、修改的情况下运行APK文件,此机制对改进大型APP的架构，实现多团队协作开发具有一定的好处。

1. [DragExpandGrid](https://github.com/wedcel/DragExpandGrid)

	一个多功能的扩展GridView，可展开，可拖动，可排序，可删除，固定更多按钮。

1. [JsonAnnotation](https://github.com/tianzhijiexian/JsonAnnotation)

	利用注解自动生成Gson‘s Model的库。

1. [HollyViewPager](https://github.com/florent37/HollyViewPager)

	一个交互效果很赞的ViewPager。

1. [tooltip-view](https://github.com/venmo/tooltip-view)

	一个工具提示view。

### 工具

1. [Hack Font](https://github.com/chrissimpkins/Hack)

	一款专门为程序员设计的字体。

1. [git-radar](https://github.com/michaeldfallen/git-radar)

	Git雷达，可以检测Git仓库中文件的变动情况，并在命令行提示符后显示文件变动情况的信息。
	
	![detailed](https://raw.githubusercontent.com/michaeldfallen/git-radar/master/images/detailed.png)

1. [Vysor](http://www.vysor.io)

	 chrome的一个插件，可以做到在电脑上操作手机，注意是实时操作，并非录屏！还是相当好用的。墙内下载地址：http://pan.baidu.com/s/1jGrjpOE

1. [Fyuneru](https://github.com/sogisha/fyuneru)

	又一个科学上网工具。

----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)