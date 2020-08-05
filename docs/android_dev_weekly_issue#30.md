layout: post
title: "Android开发技术周报 Issue#30"
date: 2015-04-28 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#30

### 教程

1. [如何检查 Android 应用的内存使用情况](http://android.jobbole.com/80926/)

	Android是为移动设备而设计的，所以应该关注应用的内存使用情况。尽管Android的Dalvik虚拟机会定期执行垃圾回收操作，但这也不意味着就可以忽视应用在何时何处进行内存分配和释放。为了提供良好的用户体验，做到系统在不同应用间流畅切换，当用户和应用无交互时，避免应用不必要的内存消耗是很重要的。

1. [Android性能优化典范（二)](http://www.csdn.net/article/2015-04-29/2824583-android-performance-patterns-season-2) ([@胡凯me](http://weibo.com/kesenhoo))
	
	Google前几天刚发布了Android性能优化典范第2季的课程，一共20个短视频，包括的内容大致有：电量优化、网络优化、Android Wear上如何做优化、使用对象池来提高效率、LRU Cache、Bitmap的缩放、缓存、重用、PNG压缩、自定义View的性能、提升设置alpha之后View的渲染性能，以及Lint、StictMode等工具的使用技巧。 下面是对这些课程的总结摘要，认知有限，理解偏差的地方请多多指教！
	
1. [Android图形处理流水线：从Button到Framebuffer（1）](http://android.jobbole.com/80899/) ([@安卓开发频道](http://weibo.com/androidpd))

	为了充分理解视点是如何显示到屏幕上这一过程，我们将使用一个小的应用实例来描述Android图形流水线的每一个主要步骤，从公开的Android Java API（SDK）开始，到本地C++代码，最终观察原生的OpenGL绘制操作。

1. [在Android上实现模糊视图](http://android.jobbole.com/80895/)

	模糊效果可以生动地表现出内容的层次感，能帮助用户着重关注内容。即便在模糊表面下层发生视差效果或者动态改变，也能够保持当前专题内容。

1. [ART运行时Mark-Compact（ MC）GC执行过程分析](http://blog.csdn.net/luoshengyang/article/details/45162589)

	除了Semi-Space（SS）GC和Generational Semi-Space（GSS）GC，ART运行时还引入了第三种Compacting GC：Mark-Compact（MC）GC。这三种GC虽然都是Compacting GC，不过它们的实现方式却有很大不同。SS GC和GSS GC需两个Space来压缩内存，而MC GC只需一个Space来压缩内存。本文就详细分析MC GC的执行过程。

### 代码&开源库

1. [fab-toolbar](https://github.com/AlexKolpa/fab-toolbar)

	实现了FAB＋Toolbar效果。
	
1. [MaterialViewPager](https://github.com/florent37/MaterialViewPager)

	Material Design效果的ViewPager.

1. [DropDownMenu](https://github.com/JayFang1993/DropDownMenu) ([@方杰_Jay](http://weibo.com/ncuitstudent))
	
	类似58同城的多条件过滤筛选效果。

1. [android-intents](https://github.com/marvinlabs/android-intents)
	
	对Intent进行了2次封装，包含有EmailIntents、PhoneIntents、GeoIntents、SystemIntents、MediaIntents等。
	
1. [android-prefs](https://github.com/BoD/android-prefs)

	通过注解来生成SharedPreferences。

### 工具

1. [Appetize.io](https://appetize.io)

	Stream iOS & Android Simulators in the Browser For embedding apps in websites, development, client demos, testing and more.

1. [Android tool for mac](https://github.com/mortenjust/androidtool-mac) ([@李锦发](http://www.weibo.com/jinfali))

	一款用 Swift 写的可在 Mac 上使用的 Android 工具, 支持一键截屏, 视频录制, APK 安装等功能，同时还支持获取bug报告和自定义脚本，只支持 Mac 系统。
	
1. [fossdroid.com](https://fossdroid.com)  ([@lylekaihi](https://www.v2ex.com/member/kylekaihi))

	一个安卓 open source 网站，里面有许多不错的项目，大家可以 down 下来看看.

### 视频	

1. [Android-仿微信语音聊天](http://www.imooc.com/view/383) ([@慕课网](http://www.weibo.com/mukewang?from=feed&loc=nickname))

	本课程通过结合自定义View、媒体相关API、Dialog管理等实现仿微信语音功能。课程主要涉及自定义录音Button与用户的交互，MediaRecorder与MediaPlayer实现录音、播放功能，以及三者间的交互与协作效果。案例课程不要错过咯！
		
### 新闻

1. [Android 版 Chrome 新发布了开发版(dev)独立应用](https://play.google.com/store/apps/details?id=com.chrome.dev) ([@北京GDG](http://www.weibo.com/gtug?from=feed&loc=nickname))
 
	为了让开发者更早地测试和反馈新功能，Android 版 Chrome 新发布了开发版(dev)独立应用，O网页链接 。和桌面版类似，现在你可以在 Android 手机同时安装 stable, beta, dev 三个版本的 Chrome 。

1. [已有超过 70 个 Android app 加入 Google Now 信息卡支持行列](http://cn.engadget.com/2015/04/29/google-now-70-more-android-apps/)
		
	年初时 Google 才刚开放三方 App 与 Google Now 的协作，现在，将一次把支持的 App 数量从原本的 40 个增加到超过 70 个 ，我们也看到了 Spotify、ABC News、RunKeeper、Jawbone 与 OpenTable 都在行列当中。
			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)