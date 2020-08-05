---
layout: post
title: "Android开发技术周报 Issue#21"
date: 2015-03-02 13:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#21

### 教程

1. [Android模块化编程之引用本地的aar](http://stormzhang.com/android/2015/03/01/android-reference-local-aar)

	随着项目越来越多，代码的复用就变得异常重要，这时候就要进行模块化编程，就是把一些通用的组件或者类库做成单独的模块，其他项目直接进行引用就好。针对Android开发最常见的就是Android Library，在Gradle出现之前引用Android Library的方式也很繁琐，但是有了Gradle一切变得非常简单方便。

1. [微信的jsbridge实现](http://blog.aaapei.com/article/2013/12/wei-xin-de-jsbridgeshi-xian)
	
	android的webview api中有开放过一个addJavaScriptInterface函数,这个函数的作用是在页面的Window中注入一个JS对象,如果你的应用中使用了这个api,建议先看一下国内安全领域第一人黑哥的这篇文章[android webview 漏洞背后的节操](http://hi.baidu.com/hi_heige/item/9baf99f063331d58c9f3379a).
	
1. [Android单点触控技术，对图片进行平移，缩放，旋转操作](http://blog.csdn.net/xiaanming/article/details/42833893)

	相信大家使用多点对图片进行缩放，平移的操作很熟悉了，大部分大图的浏览都具有此功能，有些app还可以对图片进行旋转操作，QQ的大图浏览就可以对图片进行旋转操作，大家都知道对图片进行缩放，平移，旋转等操作可以使用Matrix来实现，Matrix就是一个3X3的矩阵，对图片的处理可分为四个基础变换操作，Translate(平移变换)、Rotate(旋转变换）、Scale (缩放变换)、Skew（错切变换）.

1. [Android 性能优化之使用MAT分析内存泄露问题](http://blog.csdn.net/xiaanming/article/details/42396507)
	
	我们平常在开发Android应用程序的时候，稍有不慎就有可能产生OOM，虽然JAVA有垃圾回收机，但也不能杜绝内存泄露，内存溢出等问题，随着科技的进步，移动设备的内存也越来越大了，但由于Android设备的参差不齐，可能运行在这台设备好好的，运行在那台设备就报OOM，这些适配问题也是比较蛋疼的，...		
1. [Span的详细用法/演示/自定义方法](http://flavienlaurent.com/blog/2014/01/31/spans/)

	Span的详细用法/演示/自定义方法, 先介绍的各个Span之间的在Framework中的继承关系和它是如何工作的，然后又针对每种Span结合具体的示例做详细的讲解，有图有真相。

1. [Android开发贴士集合（1）](http://blog.jobbole.com/67914/)

	Android开发贴士集合共五篇文章介绍一些你可能不知道却比较有用的API。其他四篇：[Android开发贴士集合（2）](http://blog.jobbole.com/67920/)、[Android开发贴士集合（3）](http://blog.jobbole.com/67928/)、[Android开发贴士集合（4）](http://blog.jobbole.com/68006/)、[Android开发贴士集合（5）](http://blog.jobbole.com/72523/)。

1. [Android Drawable 那些不为人知的高效用法](http://blog.csdn.net/lmj623565791/article/details/43752383)

	Drawable在我们平时的开发中，基本都会用到，而且给大家非常的有用。那么什么是Drawable呢？能够在canvas上绘制的一个玩意，而且相比于View，并不需要去考虑measure、layout，仅仅只要去考虑如何draw（canavs）。

1. [深入浅出RxJava（一：基础篇）](http://blog.csdn.net/lzyzsd/article/details/41833541)
	
	[RxJava](https://github.com/ReactiveX/RxJava)正在Android开发者中变的越来越流行。唯一的问题就是上手不容易，尤其是大部分人之前都是使用命令式编程语言。但是一旦你弄明白了，你就会发现RxJava真是太棒了。这里仅仅是帮助你了解RxJava，整个系列共有四篇文章，希望你看完这四篇文章之后能够了解RxJava背后的思想，并且喜欢上RxJava。

1. [Android 开发最佳实践](https://github.com/futurice/android-best-practices)

	Best practices in Android development，整理了一些不错的Android实践。

1. [关于xml中tools属性介绍](https://medium.com/sebs-top-tips/tools-of-the-trade-part-2-b91271892d10)	

	关于xml中tools:context，tools:menu，tools:actionBarNavMode，tools:listitem/listheader/listfooter，tools:showIn，tools:layout的作用介绍，又能节省一大段Java代码了。

1. [简单几步教你不用vpn照样翻墙](http://www.jianshu.com/p/3e1fcd9e0d4b?utm_campaign=maleskine&utm_content=note&utm_medium=pc_all_hots&utm_source=recommendation)

	在这里教大家一个简单的方法，只需要修改host就可翻墙。与网上的改host方法不同，百度到的host地址基本是固定的，可能短暂时间有用，但被墙了就gg了。这里提供一个@netsh.org博客的链接，netsh大神会经常更新host地址，就算之前的host地址被墙了，去更新一下就可以继续上了。

### 代码&开源库

1. [MaterialImageView](https://github.com/zhaozhentao/MaterialImageView)

	小而美的MaterialImageView,圆角,阴影,抗锯齿。
	
1. [JsBridge](https://github.com/lzyzsd/JsBridge)
	
	模仿微信webview的JsBridge，安全方便的实现js和Java的互相调用，主要通过loadUrl和shouldOverrideUrl实现.
	
1. [search_bar.xml](https://gist.github.com/nickbutcher/b3962f0d14913e9746f2)

	![image](http://ww2.sinaimg.cn/bmiddle/7cb90679gw1epot6e8edjg20b408cjrk.gif)
	
1. [Sky31Radio](https://github.com/linroid/Sky31Radio)

	一个开源的校园电台app，一款学院风的电台节目。各色主播可供调戏。 有小清新有重口味；广播小剧专业自制；神路人档各种乱入.
	
	![image](http://ww3.sinaimg.cn/bmiddle/005ZJ8j4gw1epnzliy8bnj31221ut7g4.jpg)

1. [BooheeScrollView](https://github.com/zhaozhentao/BooheeScrollView)

	模仿薄荷食物图书馆效果.
	
	![image](https://raw.githubusercontent.com/zhaozhentao/BooheeScrollView/master/screenshot/screen.gif)

1. [RecyclerViewFastScroller](https://github.com/danoz73/RecyclerViewFastScroller)

	带Fast Scroller的RecyclerView。
	
	![image](https://camo.githubusercontent.com/8b8e323a4f7f904b6d6f5057ceaa28a81570af26/687474703a2f2f692e696d6775722e636f6d2f327a4277496c776c2e706e67)

1. [sqlbrite](https://github.com/square/sqlbrite)
	
	良心企业Square的又一开源项目，当你不想给用ContentProvider，只想简单监听SQLite表增删改的数据变更时可以试试它。
	
1. [Hawk](https://github.com/orhanobut/hawk)	
	
	安全简单的Android KV存储开源项目Hawk，使用AES加密内容，SharedPreferences存储数据、GSon序列化对象，支持存储任何类型及其List。
	
1. [LoganSquare](https://github.com/bluelinelabs/LoganSquare)
	
	一个比Gson、Jackson解析和序列化还要快的JSON解析库。

1. [CropImageView](https://github.com/cesards/CropImageView)
	
	支持9个方向进行图片裁剪的ImageView。
	
	![image](https://github.com/cesards/CropImageView/raw/master/art/cropping.png)

1. [AndroidTreeView](https://github.com/bmelnychuk/AndroidTreeView)

	Android TreeView支持第n级展开或收缩，自定义view、value、样式.

1. [Material Calendar View](https://github.com/prolificinteractive/material-calendarview)

	Material Design风格的日历控件。	
	
	![image](https://raw.githubusercontent.com/prolificinteractive/material-calendarview/master/images/screencast.gif)
		
### 工具	 

1. [Android Studio 1.1](http://www.androiddevtools.cn)

	* Improved unit testing support! This is described in much greater detail in [http://tools.android.com/tech-docs/unit-testing-support](http://tools.android.com/tech-docs/unit-testing-support). Note that this requires the new version of the Android Gradle plugin 1.1, also available (and bundled with the IDE for offline usage). Note also that while the new Gradle plugin is included and supported, version 1.0 continues to be supported as well, so you can update to the new version of the IDE without affecting your project files and builds.
	* Many new lint checks - run Analyze > Inspect Code to see if version 1.1 uncovers new issues in your projects
	* Templates for creating analog and digital Android Wear watch faces
Updated launcher icons, now packaged as mipmap resources
	* Support for BCP 47 language tags (e.g. additional 3-letter language codes when using Android 5.0); as with the improved unit testing support this requires version 1.1 of the Gradle plugin.
	* See [New Build System](http://tools.android.com/tech-docs/new-build-system) for the Gradle plugin release notes.

1. [Cow](https://github.com/cyfdecyf/cow)	
	
	COW 是一个简化穿墙的 HTTP 代理服务器。它能自动检测被墙网站，仅对这些网站使用二级代理。
	
1. [Android Material Design Icon Generator Plugin](https://github.com/konifar/android-material-design-icon-generator-plugin)
	
	自动帮你生成Material Design风格的图标的插件，还在为不会设计图标发愁吗？赶紧试试Android Material Design Icon Generator Plugin吧。
	
	<img src="https://raw.githubusercontent.com/konifar/android-material-design-icon-generator-plugin/master/docs/capture.gif" width="728" height="451"/>

### 新闻

1. [Google将在I/O大会上推出新的支付接口Android Pay](http://www.36kr.com/p/220003.html)

	有知情人士向 [Ars](http://arstechnica.com/business/2015/02/google-will-launch-android-pay-at-io-in-may/) 透露，Google 将在今年的 I/O 大会推出新的移动支付接口 Android Pay，简化用户在应用内、商店内支付流程。Android Pay 主要面向开发者，帮助后者在自己的应用内增加支付选项，用户上传信用卡或者银行卡信息后，就可以在应用内一键支付，无需经过 Google Wallet。

1. [Android 5.1新特性：单次上划关闭下拉栏、快速解锁](http://www.36kr.com/p/219941.html)

	悄然推出的 Android 5.1 在不久前于 MicroMax 的 Android One 设备上被发现，但具体更新内容并没有官方文档。然而国外爱好者 Ramit Suri 还是发现了一些新东西。

### 视频

1. [从360手机卫士的开发历程看如何实施大型移动应用开发](http://www.infoq.com/cn/presentations/from-360-development-see-big-mobile-application-development)

	视频讲解了360手机卫士在开发过程中曾经面临的许多问题，体系架构上的挑战与应对(多进程化、插件化、云化等等)、研发流程(Build流程、自动化测试等、安全审核)等。

### 设计

1. [Sketch+Keynote双剑合璧：5步快速制作移动动效](http://www.aliued.cn/2015/02/15/sketchkeynote双剑合璧：5步快速制作移动动效.html)
	
	2014年，Facebook推出了新闻阅读应用Paper，诸多交互细节与炫酷动效启动了界面设计的新时代，Google的Material Design更是将移动动效提升到了app基础体验环节的高度。盘点如今体验优秀的移动app，精彩的动效层出不穷，放眼望去，聚集UI设计大神的dribbble、behance等地，出彩的动效更好的诠释了流畅细腻的交互操作……如果说移动体验设计师还能在传统的交互视觉之上提升app的可用性，移动动效必定是最重要的方式之一。
			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)