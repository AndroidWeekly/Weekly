layout: post
title: "Android开发技术周报 Issue#25"
date: 2015-03-18 14:13:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#25

### 教程

1. [Android ocr识别文字介绍](http://blog.csdn.net/love_xsq/article/details/44616925)

	最近在做身份证号码识别，在网上搜索的一番后发现目前开源的OCR中tesseract-ocr算是比较强大的了，它由HP于1985年到1995年间开发，后来由google直接负责，经过谷歌进一步开发后，目前的tesseract-ocr有了显著的改进。

1. [Java实现图像灰度化](http://liuyu314.github.io/java/2014/05/24/grayscale/)

	本文主要介绍了灰度化的几种方法，以及如何使用Java实现灰度化。同时分析了网上一种常见却并不妥当的Java灰度化实现，以及证明了opencv的灰度化是使用“加权灰度化”法

1. [自定义view实现水波纹效果](http://blog.csdn.net/tianjian4592/article/details/44222565)

	今天主要分享水波纹效果：1.标准正余弦水波纹；2.非标准圆形液柱水波纹；虽说都是水波纹，但两者在实现上差异是比较大的，一个通过正余弦函数模拟水波纹效果，另外一个会运用到图像的混合模式（PorterDuffXfermode）；

1. [Android自定义控件其实很简单系列](http://blog.csdn.net/column/details/androidcustomview.html)

	详解Android自定义控件的流程，在一定程度上剖析涉及控件自定义的四大类Canvas、Paint、View和ViewGroup，由浅至深，从绘制到测量到事件的处理对Android自定义控件又一个全新的认知。

1. [OKHttp源码解析](http://frodoking.github.io/2015/03/12/android-okhttp/)

	Android为我们提供了两种HTTP交互的方式：HttpURLConnection 和 Apache HTTP Client，虽然两者都支持HTTPS，流的上传和下载，配置超时，IPv6和连接池，已足够满足我们各种HTTP请求的需求。但更高效的使用HTTP可以让您的应用运行更快、更节省流量。而OkHttp库就是为此而生。

1. [Google+ 团队的 Android UI 测试](http://allenlsy.com/android-ui-tests-in-google-plus-team/)

	Android 测试主要分为3个类型：单元测试（Unit Test)、封闭UI测试 （Hermetic UI Test)、Monkey Test。区分UI代码和功能代码在Android开发中尤其困难。因为有时Activity既有Controller的功能，又有View的功能。Robolectric是一个很优秀的Android测试框架，它提供了一个Android框架的stub，这样测试运行时实际上是在JVM上运行，而不是在Android平台（比如Robotium和Instrumentation都是在Android平台运行测试），从而提高了速度。
	
1. [一个绚丽的 loading 动效分析与实现！](http://blog.csdn.net/tianjian4592/article/details/44538605)

	前两天我们这边的头儿给我说，有个 gif 动效很不错，可以考虑用来做项目里的loading，问我能不能实现，看了下效果确实不错，也还比较有新意，复杂度也不是非常高，所以就花时间给做了，我们先一起看下原gif图效果：

1. [ActivityManagerService启动流程分析](http://blog.csdn.net/wlsfling/article/details/44495589)

	ActivityManagerService (AMS) 是android系统中最核心的服务，主要负责四大组件的启动，切换，调度及应用程序的管理和调度等工作，其职责与操作系统中的进程管理和调度模块类似。

1. [深入理解Android之设备加密Device Encryption](http://blog.csdn.net/innost/article/details/44519775)

	Android从4.4开始就支持一项功能，那就是对设备进行加密。加密自然是为了安全性考虑，由于/system目录是只读的，手机里那些存储设备分区中需要保护的就剩下/data/分区和sdcard了。显然，/data/和sdcard大量存储了用户数据（比如app运行时存储的数据），对他们进行加密非常非常有必要。

1. [深入分析Java ClassLoader原理](http://www.importnew.com/15362.html)

	大家都知道，当我们写好一个Java程序之后，不是管是CS还是BS应用，都是由若干个.class文件组织而成的一个完整的Java应用程序，当程序在运行时，即会调用该程序的一个入口函数来调用系统的相关功能，而这些功能都被封装在不同的class文件当中，所以经常要从这个class文件中要调用另外一个class文件中的方法，如果另外一个文件不存在的，则会引发系统异常。而程序在启动的时候，并不会一次性加载程序所要用的所有class文件，而是根据程序的需要，通过Java的类加载机制（ClassLoader）来动态加载某个class文件到内存当中的，从而只有class文件被载入到了内存之后，才能被其它class所引用。所以ClassLoader就是用来动态加载class文件到内存当中用的。

### 代码&开源库

1. [DaVinci](https://github.com/florent37/DaVinci)

	DaVinci是一个适用于Android Wear平台的图片下载和缓存library。

	![image](https://raw.githubusercontent.com/florent37/DaVinci/master/mobile/src/main/res/drawable-hdpi/davinci_new_small.jpg)

1. [device-year-class](https://github.com/facebook/device-year-class)

	Facebook 的开源工具，让开发者快速识别用户使用的设备机型.

1. [AirMapView](https://github.com/airbnb/AirMapView)

	AirMapView是一个抽象的视图。它支持多个本地地图提供者包括谷歌地图V2和亚马逊地图V2。如果设备没有任何受支持的本地地图提供者,AirMapView会回退到基于web的地图提供者(目前谷歌地图)。

1. [BlurNavigationDrawer](https://github.com/charbgr/BlurNavigationDrawer)

	背景模糊的Navigation Drawer。

1. [materialistic](https://github.com/hidroh/materialistic)
	
	Material Desgin风格的Hacker News客户端。

1. [PopoverView](https://github.com/lupidan/PopoverView)

	一个模仿iOS UIPopoverController效果的控件。

1. [fresco](https://github.com/facebook/fresco)

	Facebook 又放出的一个新项目，一个类似 Picasso, Glide 的库，不过比他们做的更好。 强烈推荐！

1. [StatedFragment](https://github.com/nuuneoi/StatedFragment)

	如果你还在为保存Fragment的状态折麽着，那么赶紧试试StatedFragment吧。
	
1. [CreditsRoll](https://github.com/frakbot/CreditsRoll)

	实现星球大战字幕效果。
	
	![image](http://ww4.sinaimg.cn/large/005O8uRcjw1eqhykirf7og308w0dz7wk.gif)

1. [logger](https://github.com/orhanobut/logger)

	一个简单、漂亮、功能强大的Android日志程序。

		
### 工具	 

1. [Color themes for IntelliJ IDEA](http://www.ideacolorthemes.org/home/)	
	专为IDE神器InteliJ (IDEA, PhpStorm, PyCharm, RubyMine, WebStorm and AppCode)全系列打造的主题，总有一款对你的口味。

	
1. [Android SVG to VectorDrawable (Alpha)](http://inloop.github.io/svg2android/)

	一个可以将SVG图片转换为Vector Drawable xml文件的在线工具。

1. [Augmented Traffic Control](https://github.com/facebook/augmented-traffic-control)

	Facebook宣布开源移动网络测试工具ATC，该工具支持利用Wi-Fi网络模拟2G、2.5G、3G以及LTE 4G移动网络环境，让测试工程师们能够快速对智能手机和App在不同国家地区和应用环境下的性能表现进行测试。

### 视频

1. [Android Studio 系列视频 #3 Layout Editor](http://v.youku.com/v_show/id_XOTIwMjU4MDMy.html?f=23555901)
	
	Android Studio 系列视频 #3 Layout Editor ，Layout Editor 提供了可视化的界面布局编辑功能，而无需部署到手机或模拟器中，还有多种典型设备的适配功能。
	
### 新闻

1. [刚完成8000万美元融资的Cyanogen想脱离安卓 自立门户](http://www.pingwest.com/cyanogen-builds-its-own-android/)

	刚刚宣布完成8000万美元 C轮融资的 Cyanogen，即将成为智能手机软件生态里新的新搅局者。吃着 Android 开源的奶长大，Cyanogen 已经发展为世界上最大的第三方 Android 操作系统研发公司。这家公司过去开发和维护着世界上装机量最大的Android 定制 ROM之一的CyanogenMod。
			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)