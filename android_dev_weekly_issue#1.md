---
layout: post
title: "Android开发周报 Issue#1"
date: 2014-09-23 22:36:14 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发周报 Issue#1


### 文章

1. [HTTP2协议中英对照版](https://github.com/fex-team/http2-spec/blob/master/HTTP2中英对照版(06-29).md)

	HTTP 全称为 HyperText Transfer Protocol，中文叫做超文本传输协议。用于 Web 应用层传输，是 Web 架构的核心，它至今公布有 3 个版本：HTTP 0.9、HTTP 1.0、HTTP 1.1，作为与时俱进的我们，有必要去了解和学习 HTTP 2，它对我们未来 Web 性能优化工作起到很重要的作用，是一切优化的基础。现 Chrome 里也已使用 SPDY。
	
	由百度FEX团队的 zhangtao 等同学们，业余花费近半年时间翻译的 HTTP 2 草案发布。
	
2. [Android TouchEvent事件传递机制](http://blog.csdn.net/morgan_xww/article/details/9372285#comments)
	
	作者通过列举通俗易懂的例子和打印日志的方式讲解了Android TouchEvent事件传递机制。		
3. [Android事件分发机制完全解析，带你从源码的角度彻底理解(上)](http://blog.csdn.net/guolin_blog/article/details/9097463)	

4. [Android事件分发机制完全解析，带你从源码的角度彻底理解(下)](http://blog.csdn.net/loongggdroid/article/details/19118475)


### 代码&开源库

1. [SnappyDB](https://github.com/nhachicha/SnappyDB)

	一个Android平台的 `key-value` 数据库，在 `读/写` 操作方面可以完胜 SQLite。 下图就是它们在 `读/写` 方面的对比测试结果：

	![image](https://camo.githubusercontent.com/0f6193a1f84aa8a77d07ac18d3566b87bc89999b/687474703a2f2f736e6170707964622e636f6d2f696d672f62656e63686d61726b5f73716c6974655f776974685f7472616e73616374696f6e2e706e67)

2. [AppRate-for-Android](https://github.com/kikoso/AppRate-for-Android) 

	AppRate for Android是一个以不打扰用户的方式允许用户对您的应用程序进行评价。一个窗口中选择评价、稍后提醒还是拒绝进行评价。

	![image](https://camo.githubusercontent.com/f84466fd21066bad1ba7c47224f8f351a21d2361/68747470733a2f2f7261772e6769746875622e636f6d2f6b696b6f736f2f417070526174652d666f722d416e64726f69642f6d61737465722f6172742f73637265656e73686f742e706e67)
	
3. [BlurStickyHeaderListView](https://github.com/emmano/BlurStickyHeaderListView) 

	ListView with blur/parallax/sticky capabilities
	
4. [EasyAndroidAnimations](https://github.com/2359media/EasyAndroidAnimations) 

	Easy Android Animations is an animation library that aims to make android animations easier, with 50+ builtin animations, it allows you to introduce many complex animation effects in your application with one or two lines of code.


5. [SnackBar](https://github.com/MrEngineer13/SnackBar)

	toast-like alert pattern for Android

	![image](https://camo.githubusercontent.com/67a39af16f3d46631567c1f7bd7dcddeb3c4c9e9/687474703a2f2f6d6174657269616c2d64657369676e2e73746f726167652e676f6f676c65617069732e636f6d2f696d616765732f636f6d706f6e656e74732d746f617374732d73706563732d737065635f746f6173745f30335f315f6c617267655f6d6470692e706e67)

7. [ig-json-parser](https://github.com/Instagram/ig-json-parser)

	一个由Instagram团队实现的快速JSON解析器。
	
8. [android-floatinglabel-widgets](https://github.com/marvinlabs/android-floatinglabel-widgets)
	
	浮动标签输入组件，当输入框不为空的时候可以在其上方显示一个提示标签。
	
	![image](https://camo.githubusercontent.com/ae02c8934861e7fcc10661cfed79f7276dfe06b7/687474703a2f2f696d672e796f75747562652e636f6d2f76692f68705a4439674a635267302f302e6a7067)
	
9. [CalendarListview](https://github.com/traex/CalendarListview)

	在ListView中实现了一个日历，每行显示一个月。
	
	![image](https://github.com/traex/CalendarListview/raw/master/demo.gif)

10. [clean-status-bar](https://github.com/emmaguy/clean-status-bar)

	在你获取屏幕截图之前帮你清空Android Status bar的小工具。
	
	![image](https://raw.githubusercontent.com/emmaguy/clean-status-bar/master/images/before.png)![image](https://raw.githubusercontent.com/emmaguy/clean-status-bar/master/images/after.png)
	
11. [ResumeSample](https://github.com/geekcompany/ResumeSample)

	程序员简历模板系列。包括PHP程序员简历模板、iOS程序员简历模板、Android程序员简历模板、Web前端程序员简历模板、Java程序员简历模板、C/C++程序员简历模板、NodeJS程序员简历模板、架构师简历模板以及通用程序员简历模板 
http://get.jobdeer.com/744.get

12. [LoopingViewPager](https://github.com/imbryk/LoopingViewPager)
	
	一个Android ViewPager扩展可以无限滚动。

13. [android-beacon-library](https://github.com/AltBeacon/android-beacon-library)

	这是一个提供了与Beacons进行交互Api的库。
	
14. [BLEService](https://github.com/RatioLabs/BLEService)

	一个Android蓝牙低功耗Service库，主要实现了以下几个Feature：

	* Implements BLE as an android service
	* Requests done via AIDL with a service connection
	* Responses sent via BroadcastReceivers
	* Allows persistent device interface cross-activity.
	* Hides all the nasty stuff
	* Wraps Bluetooth classes in parcelable classes so they can be passed between activities.
	* Less than 20 calls on a single object
	* Supports connection retries

### 工具

1. [gradle-retrolambda](https://github.com/evant/gradle-retrolambda)

	一个可以在java 6，7和android中获得java lambda特性的gradle插件。

2. [Android Studio 0.8.11](http://www.androiddevtools.cn)

	Android Studio又如期的发布了更新，本次更新有如下几点：
	
	* 支持了新版的Android Gradle plugin (0.13)，新版插件支持Gradle 2.1。
	
	* Lint工具检查出的错误可以在文本扩展提示框中显示完整的错误解释说明了，以帮助你快速的解决问题。
	
	* layout editor会检查,以确保你有最新版本的“layoutlib”。
	
	* 从IntelliJ 13.1.5 RC合并了最新的改动，其中一个改动是改变了Android Studio.app bundle的目录结构。
	
	* 修复了一些Bug。
3. [chromeos-apk](https://github.com/vladikoff/chromeos-apk)
	
	一个可以让Android应用在Chrome OS, OS X, Linux 和 Windows系统上运行的小工具。
	
### 书

1. [50 Android Hacks](http://it-ebooks.info/book/2445/)

	本书讲解了50个Android开发的小技巧。

### 设计

1. [LayerCraft](http://lab.rayps.com/lc/)
	
	A Photoshop plugin to export UI assets from layers。
	
	
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)