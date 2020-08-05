---
layout: post
title: "Android开发周报 Issue#7"
date: 2014-11-17 16:31:09 +0800
comments: true
categories: AndroidDevWeekly 
---

#Android开发周报 Issue#7

### 新闻

1. [盘点最受开发者喜爱的Android 5.0 Lollipop API](http://www.csdn.net/article/2014-11-14/2822647-12-great-lollipop-apis/1)

	作为Android系统的一次重大升级，Android 5.0 Lollipop突出采用全新的Material Design设计语言，不但在视觉和操作上更胜一筹，还包含扩展UI工具包供开发者使用，为应用添加3D实时阴影，可缩放矢量“drawbles”以及流畅的动画效果。本文着重介绍了其中值得开发者深爱的12款API，赶紧一睹为快吧！

1. [.NET开源了，VS开始支持Android和iOS编程并自带Android模拟器](http://news.cnblogs.com/n/508431/)

	北京时间今天凌晨的 Connect (); 大会上，多少程序员的假想成为现实。.NET 开源，集成 Clang 和 LLVM 并且自带 Android 模拟器，这意味着 Visual Studio 这个当下最好没有之一的 IDE 正式支持编写 Android 和 iOS 程序。

1. [Android 5.0正式开启：Nexus系列最早更新](http://digi.it.sohu.com/20141113/n405991228.shtml)	
	从谷歌给出的公告来看，今天就将会有用户收到Android 5.0的更新提示，而首批设备包含了Nexus 4、Nexus 5、Nexus 7以及Nexus 10。值得一提的是，今天早些时候，摩托罗拉也开始向Moto G的用户提供5.0系统的升级，随后到来的是Moto X，很快LG的G3也将得到系统的升级。
	
### 文章

1. [Android 那些你所不知道的Bitmap对象详解](http://blog.csdn.net/xiaanming/article/details/41084843#0-tsina-1-26268-397232819ff9a47a7b7e80a40613cfe1)

	我们知道Android系统分配给每个应用程序的内存是有限的，Bitmap作为消耗内存大户，我们对Bitmap的管理稍有不当就可能引发OutOfMemoryError，而Bitmap对象在不同的Android版本中存在一些差异，今天就给大家介绍下这些差异，并提供一些在使用Bitmap的需要注意的地方。

1. [如何给你的Android 安装文件（APK）瘦身](http://greenrobot.me/category/devpost/)

	Android的apk文件越来越大了这已经是一个不争的事实。在Android 还是最初版本的时候，一个app的apk文件大小也还只有2 MB左右，到了现在，一个app的apk文件大小已经升级到10MB到20MB这个范围了。apk文件大小的爆炸式增长主要是因为用户对app质量的期待越来越高以及开发者的开发经验增长。

1. [创建Material Design风格的Android应用系列文章](http://blog.isming.me/tags/material-design/)

	随着Android 5.0的发布，Android Developer网站也更新了，增加了创建Material Design风格的Android应用指南,也更新了Support Library，在support library增加了一些Material Design风格的控件和动画等，这里给大家简单介绍一下怎样开发aterial Design风格的Android应用。

1. [从Java代码到字节码（1）](http://www.importnew.com/13107.html)

	理解Java代码是如何被编译为字节码并在Java虚拟机（JVM）上执行是非常重要的，这将帮助理解你的程序是如何执行的。这样的理解不仅仅能够让你在逻辑上更好的掌握语言特性，而且能够有机会理解在做出重要决定时所需的权衡以及相应的副作用。

1. [在WebView中如何让JS与Java安全地互相调用](http://www.pedant.cn/2014/07/04/webview-js-java-interface-research/)

	在现在安卓应用原生开发中，为了追求开发的效率以及移植的便利性，使用WebView作为业务内容展示与交互的主要载体是个不错的折中方案。那么在这种Hybrid(混合式) App中，难免就会遇到页面JS需要与Java相互调用，调用Java方法去做那部分网页JS不能完成的功能。

1. [译文：理解Android中垃圾回收日志信息](http://droidyue.com/blog/2014/11/08/understanding-garbage-collection-output-messages-in-android/)

	如果你是一名Android开发者并且常常看程序日志的话，你会经常在logcat的调试日志窗口看到像 `GC_CONCURRENT freed 178K, 41% free 3673K/6151K, external 0K/0K, paused 2ms+2ms` 这样的日志信息，这就是Android系统垃圾回收的部分输出信息，本文将具体介绍这些日志信息的每一部分的含义来帮助帮助大家更好地了解垃圾回收的运行情况。

1. [Android 使用android-support-multidex解决Dex超出方法数的限制问题,让你的应用不再爆棚](http://blog.csdn.net/t12x3456/article/details/40837287)

	 随着应用不断迭代，业务线的扩展,应用越来越大(比如集成了各种第三方sdk或者公共支持的jar包,项目耦合性高，重复作用的类越来越多)，相信很多人都遇到过如下的错误: `java.lang.IllegalArgumentException: method ID not in [0, 0xffff]: 65536 ` 没错，你的应用中的Dex 文件方法数超过了最大值65536的上限,简单来说，应用爆棚了.

<!--more-->


### 代码&开源库

1. [MaterialDesignCenter](https://github.com/lightSky/MaterialDesignCenter)

	收集整理了Android Material Design相关的设计资源、视频教程、译文教程和开源库等。

1. [Android-PullLayout](https://github.com/BlueMor/Android-PullLayout)

	仿UC天气下拉和微信下拉眼睛
	
	![image](https://raw.githubusercontent.com/BlueMor/Android-PullLayout/master/screenshoot/123.gif)

1. [safe-java-js-webview-bridge](https://github.com/pedant/safe-java-js-webview-bridge)

	抛弃使用高风险的WebView addJavascriptInterface方法，利用onJsPrompt解析纯JSON字符串，来实现网页JS层反射调用Java方法，同时通过对js层调用函数及回调函数的包装，支持方法参数传入所有已知的类型，包括number、string、boolean、object、function。

1. [CircleProgress](https://github.com/lzyzsd/CircleProgress)

	各种样式的自定义圆形进度条。
	
	![image](https://raw.githubusercontent.com/lzyzsd/CircleProgress/master/demos/circle_progress.gif)

1. [SwitchButton](https://github.com/kyleduo/SwitchButton)

	同时支持Material Design和iOS7风格的SwitchButton。
	
	![image](https://raw.githubusercontent.com/kyleduo/SwitchButton/master/preview/easy_to_style.png)


### 视频

1. [使用Visual Studio 2015开发Android应用](http://www.jikexueyuan.com/course/364.html?hmsr=sina_weibo_VisualStudio)

	2014年的微软Connect();在线开发者大会在11月12日和11月13日举行。在大会上，微软公布了很多新的特性和功能。其中最吸引人的是.Net开源和Android模拟器。显示了微软更开放的战略思想。并突出了微软CEO移动优先和云优先的理念。

### 工具

1. [icon-version](https://github.com/akonior/icon-version)

	可以给Android的App图标添加版本号和变种名字的Android gradle插件。
	
	![image](https://github.com/akonior/icon-version/raw/master/doc/icon-version-screenshot.png)

### 书

1. [GitHub秘籍](http://snowdream86.gitbooks.io/github-cheat-sheet/content/zh/index.html)

	本秘籍收录了一些Git和Github非常酷同时又少有人知的功能。灵感来自于Zach Holman在2012年Aloha Ruby Conference和2013年WDCNZ上所做的演讲：Git and GitHub Secrets(slides)和More Git and GitHub Secrets(slides)。

### 设计

#### 文章

1. [切图小贴士](http://mux.baidu.com/?p=3367)

	用户手中看到的产品界面，并非设计师呕心沥血创作的效果图，而是一个个单独的切图经由开发同学技术实现。切图作为设计师与开发者之间的桥梁，它的作用很关键，合适的切图、精准的位置可以最大限度的还原效果图的设计，精妙的切图更会有事半功倍的效果哦！	
	
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)