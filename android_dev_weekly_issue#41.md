layout: post
title: "Android开发技术周报 Issue#41"
date: 2015-07-121 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#41

### 新闻

1. [谷歌确认Android M系统版本号为5.20](http://tech.sina.com.cn/notebook/pad/2015-07-21/doc-ifxfaswm0921946.shtml)

	谷歌曾经发布了Android M系统，新的系统虽然还没有应用在手机上面，但是已经有不少厂商对新系统感兴趣了。因为Android M具备很多 新功能，在内存占用等问题上也得到了优化。不过一直没有确认的是这款新系统究竟是以什么样的名字或者版本号出现。最近谷歌自己曝光了这一点。

### 教程

1. [Android DataBinding：再见Presenter，你好ViewModel！](http://www.jianshu.com/p/4e3220a580f6)

	最近一段时间MVP模式已经成为Android应用开发UI层架构设计的主流趋势。类似TED MOSBY，nucleus和mortar之类的框架都引入了Presenters来帮助我们搭建简洁的app架构。它们也（在不同的程度上）帮助我们处理Android平台上臭名昭著的设备旋转和状态持久化等问题。MVP模式也有助于隔离样板代码，虽然这并不是MVP模式的设计初衷。

1. [ORM 框架之 greenDAO 使用心得](http://itangqi.me/android/using-greendao-experience/)

	我相信，在平时的开发过程中，大家一定会或多或少地接触到 SQLite。然而在使用它时，我们往往需要做许多额外的工作，像编写 SQL 语句与解析查询结果等。所以，适用于 Android 的 ORM 框架也就孕育而生了，现在市面上主流的框架有 OrmLite、SugarORM、Active Android、Realm 与 GreenDAO。

1. [TextView预渲染研究](http://ragnraok.github.io/textview-pre-render-research.html)

	Android中的TextView是整个framework中最复杂的控件之一，负责Android中显示文本的大部分工作，framwork中的许多控件也直接或者间接的继承于TextView，例如Button，EditText等。

1. [使用Android lint发现并解决高版本API问题](http://droidyue.com/blog/2015/07/25/use-android-lint-to-find-higher-api-usage/)

	在编写代码时，为了实现一些功能，我们需要使用高版本的API，比如SharedPreference的Editor中的apply方法为API 9开始引入，在API 9 以上的机器使用没有问题，但是在API 8上，如果运行时执行了这段代码，就会崩溃，问题相当严重。尤其是该问题出现在正式版中，后果不堪设想。本文将介绍如何使用lint发现并解决这些问题。

1. [android图片处理之图像模糊](http://blog.csdn.net/crazy__chen/article/details/47027069)

	首先是对图像的模糊处理，最常见的模糊处理方式是高斯模糊，高斯模糊指定一个半径radius，对于图片上的每个像素点，以其为中心，有一个radius长的正方形(边界点除外，但是可以使用对称的方式计算)，对于这个正方形上的每一个点，和权值(权值是根据正态分布函数计算出来的)相乘以后相加，再求平均，用该平均值代替中心点的值。

1. [Android Studio使用技巧系列教程](http://blog.csdn.net/gfbgl/article/category/5609255)

	本系列教程共有6篇，在这个系列教程中，包含了在Android Studio中学习从每个开发者都应该知道的最基本的开发技巧到更多高级的技能。各种快捷键和各种小的Tips都带有操作动画图片。

1. [Android APK加固技术方案调研](http://www.jianshu.com/p/856bf5b437aa)

	软件安全领域的攻防向来是道高一尺魔高一丈，攻防双方都处于不断的演变和进化过程中，因此软件加固技术需要长期持续的研究与投入。

1. [Android 基于Message的进程间通信 Messenger完全解析](http://blog.csdn.net/lmj623565791/article/details/47017485)

	说到Android进程间通信，大家肯定能想到的是编写aidl文件，然后通过aapt生成的类方便的完成服务端，以及客户端代码的编写。如果你对这个过程不熟悉，可以查看[Android aidl Binder框架浅析](http://blog.csdn.net/lmj623565791/article/details/38461079).

1. [Android ListView工作原理完全解析，带你从源码的角度彻底理解](http://blog.csdn.net/guolin_blog/article/details/44996879)

	在Android所有常用的原生控件当中，用法最复杂的应该就是ListView了，它专门用于处理那种内容元素很多，手机屏幕无法展示出所有内容的情况。ListView可以使用列表的形式来展示内容，超出屏幕部分的内容只需要通过手指滑动就可以移动到屏幕内了。

1. [android网络操作I： OkHttp, Volley以及Gson](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2015/0720/3209.html)

	在安卓项目中有一个问题可能无法避免：网络。不管你是加载图片，请求API数据还是从因特网上获得一个字节，你都是在使用网络。鉴于网络在安卓中的重要性与基础性，当今安卓开发者面临的问题之一就是使用何种解决方案。有许多优秀的库，你可以用各种方式把一个用在另一个之上。

1. [移动端高清、多屏适配方案](http://www.html-js.com/article/3041)

	在前端开发之前，视觉MM会给我们一个psd文件，称之为视觉稿。对于移动端开发而言，为了做到页面高清的效果，视觉稿的规范往往会遵循以下两点：首先，选取一款手机的屏幕宽高作为基准(以前是iphone4的320×480，现在更多的是iphone6的375×667)。对于retina屏幕(如: dpr=2)，为了达到高清效果，视觉稿的画布大小会是基准的2倍，也就是说像素点个数是原来的4倍（对iphone6而言：原先的375×667，就会变成750×1334）。
	
### 代码&开源库

1. [MultipleTheme](https://github.com/dersoncheng/MultipleTheme)

	Android换肤／夜间模式的Android框架，配合theme和换肤控件框架可以做到无缝切换换肤（无需重启应用和当前页面）。

1. [MusicPlayerView](https://github.com/iammert/MusicPlayerView)
	
	漂亮的自定义圆形音乐播放进度条。
	
1. [MaterialDesignNavDrawer](https://github.com/Sottti/MaterialDesignNavDrawer)

1. [CustomActivityOnCrash](https://github.com/Ereza/CustomActivityOnCrash)

	一个在你的App崩溃的时候可以显示一个自定义Activity的库。

1. [EaseInterpolator](https://github.com/cimi-chen/EaseInterpolator)

	三十种动画插值器。

1. [AndroidParallax](https://github.com/florent37/AndroidParallax)

	一个用最简单的方式实现视差滚动的库。	

1. [rxnetwork-android](https://github.com/Laimiux/rxnetwork-android)

	一个可以在Android应用程序内跟踪连接的变化库。

1. [CircleRefreshLayout](https://github.com/tuesda/CircleRefreshLayout)

	一个漂亮的自定义下拉刷新布局，水滴效果的下拉刷新动画。

1. [StickerCamera](https://github.com/Skykai521/StickerCamera)	
	一个完整的开源项目.贴纸标签相机(类似nice,in),拍照,裁剪,贴贴纸打标签功能。

1. [Fontinator](https://github.com/svendvd/Fontinator)

	一个能够让你非常方便的使用自定义字体的库。

### 工具

1. [JSONExport](https://github.com/Ahmed-Ali/JSONExport)

	一款实用工具，可以将JSON转换并输出为Swift语言类模型同时也支持Java，支持简单的定制。

1. [Smalidea](https://bitbucket.org/JesusFreke/smali/downloads)

	是一款 IntelliJ IDEA/Android Studio的 smali 插件，可以无源码调试 Android 应用。
	使用教程在[这里](http://www.droidsec.cn/smalidea无源码调试-android-应用/)。

1. [File Grouping Plugin](http://www.dmytrodanylyk.com/pages/blog/android-file-grouping.html)

	一个很赞的 Android Studio 插件，它可以将你的layout文件进行分组显示而且还不用移动，如果你还在苦于从一堆layout文件中艰难的找到某一layout文件，那么赶紧试试File Grouping Plugin吧。

1. [gradle-dexinfo-plugin](https://github.com/mutualmobile/gradle-dexinfo-plugin)

	一个可以打印dex method count的Gradle插件。

### 设计资源	

1. [Icons4Android](http://www.icons4android.com/)	
	1570 Android icons in 20 icon sets.

----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)