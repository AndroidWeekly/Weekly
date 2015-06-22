layout: post
title: "Android开发技术周报 Issue#26"
date: 2015-04-06 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#26

### 教程
1. [FaceBook推出的Android图片加载库-Fresco](https://github.com/bboyfeiyu/android-tech-frontier/tree/master/others/FaceBook推出的Android图片加载库-Fresco)

	在Android设备上面，快速高效的显示图片是极为重要的。过去的几年里，我们在如何高效的存储图像这方面遇到了很多问题。图片太大，但是手机的内存却很小。每一个像素的R、G、B和alpha通道总共要占用4byte的空间。如果手机的屏幕是480*800,那么一张屏幕大小的图片就要占用1.5M的内存。手机的内存通常很小，特别是Android设备还要给各个应用分配内存。在某些设备上，分给Facebook App的内存仅仅有16MB。一张图片就要占据其内存的十分之一。

1. [2014年Android系统安全回顾报告](http://www.droidsec.cn/google_android_security_2014_report_final/)

	谷歌刚刚发布了2014年Android系统安全回顾报告，报告长达43页，总结了Android系统中的新的安全特性，Google Play中应用安全状况，该年度发现的Android系统漏洞及由于开发者安全意识不高，滥用各类接口导致的常见安卓应用安全漏洞。

1. [在Android 5.0中使用JobScheduler](https://github.com/bboyfeiyu/android-tech-frontier/tree/master/androidweekly/在Android%205.0中使用JobScheduler)

	在Android开发中，会存在这么些场景 : 你需要在稍后的某个时间点或者当满足某个特定的条件时执行一个任务，例如当设备接通电源适配器或者连接到WIFI。幸运的是在API 21 ( Android 5.0，即Lollipop )中，google提供了一个新叫做JobScheduler API的组件来处理这样的场景。

1. [使用RxJava.Observable取代AsyncTask和AsyncTaskLoader](https://github.com/bboyfeiyu/android-tech-frontier/tree/master/androidweekly/使用RxJava.Observable取代AsyncTask和AsyncTaskLoader)

	在网上有很多关于RxJava入门指南的帖子，其中一些是基于Android环境的。但是，我想到目前为止，很多人只是喜欢他们所看到的这些，当要解决在他们的Android项目中出现的具体问题时，他们并不知道如何或者是为什么要使用RxJava。在这一系列的文章中，我想要探索在我工作过的一些依赖于RxJava架构的Android项目中的模式。

1. [安卓字体渲染器](https://github.com/bboyfeiyu/android-tech-frontier/tree/master/androidweekly/安卓字体渲染器)

	安卓的硬件加速字体渲染最开始是由Renderscript团队的一位同事编写的，后来经过了多位工程师的修改和优化，其中就包括我以及我的朋友Chet Haase。你可以很容易的找到很多关于如何用OpenGL渲染文本的教程。但是，大部分的这些文章都把重点放在游戏开发以及如何绕过一些复杂的问题上。

1. [WebView实现离线缓存阅读](http://blog.csdn.net/wwj_748/article/details/44835865)

	本篇博客要实现的是一个离线下载和离线阅读的功能，这是很多阅读类app都常见的一个功能，典型的应用就是网易新闻。什么是离线下载？其实这个概念是比较模糊，是离线之后下载呢，还是下载之后离线，但稍微有点脑子的人都知道没有网络之后怎么下载呢？所以离线下载这个功能是”在有网络的情况下，把资源下载到本地“，离线阅读就是”在没有网络或者网络不好的时候，阅读本地好缓存的文章资源“。

1. [WebView实现白天/夜间阅读模式](http://blog.csdn.net/wwj_748/article/details/44810283)

	本篇博客给大家分享一个WebView的使用案例，实现Android调用JavaScript代码来控制白天/夜间模式。关于WebView如何使用，官网有很好的说明，[Building Web Apps in WebView](http://developer.android.com/guide/webapps/webview.html#HandlingNavigation)，小巫这里就不多赘述。

1. [Direct-Load-apk启动插件的原理](http://my.oschina.net/u/2289564/blog/393252)

	Direct-load-apk基于注入和伪装的代理机制，通过转接现有的Activity，来实现动态创建和加载插件中的资源和类，因此可以正常使用this指针，而不像Dynamic-Load-apk那样需要使用that指针来代替this。

1. [Android热编译技术——运行时动态处理和生成代码，初入殿堂！](http://my.oschina.net/u/2289564/blog/368694)

	你有没有这样的想法：想将编译时不存在的类在运行时动态创建并加载。想要使一个类动态的继承不同的父类，实现不同的接口。在不知道代码的情况下，在类中添加字段，方法。在一个方法的前后插入自己的代码。

1. [Android使用SVG矢量图打造酷炫动效！](http://blog.csdn.net/tianjian4592/article/details/44733123)

	一个真正酷炫的动效往往让人虎躯一震，话不多说，咱们先瞅瞅效果： 这个效果我们需要考虑以下几个问题： 1. 这是图片还是文字； 2. 如果是图片该如何拿到图形的边沿线坐标，如果是文字呢？ 3. 如果拿到了边沿线坐标，如何让光线沿着路径跑动； 4. 怎么处理过程的衔接； 以上四个问题似乎不是太好处理，而这几个问题也...

1. [Google推荐的图片加载库Glide介绍](http://blog.csdn.net/jianghejie123/article/details/44725649)

	在泰国举行的谷歌开发者论坛上，谷歌为我们介绍了一个名叫 Glide 的图片加载库，作者是bumptech。这个库被广泛的运用在google的开源项目中，包括2014年google I/O大会上发布的官方app。它的成功让我非常感兴趣。我花了一整晚的时间把玩，决定分享一些自己的经验。在开始之前我想说，Glide和Picasso有90%的相似度，准确的说，就是Picasso的克隆版本。但是在细节上还是有不少区别的。

1. [android apk 防止反编译技术第一篇-加壳技术](http://my.oschina.net/u/2323218/blog/393372)

	做android framework方面的工作将近三年的时间了,现在公司让做一下android apk安全方面的研究，于是最近就在网上找大量的资料来学习。现在将最近学习成果做一下整理总结。学习的这些成果我会做成一个系列慢慢写出来与大家分享，共同进步。这篇主要讲apk的加壳技术，废话不多说了直接进入正题。

### 代码&开源库

1. [PugNotification](https://github.com/halysongoncalves/pugnotification)

	一个可以帮助你高效的创建通知的Library。
	
	![image](https://raw.githubusercontent.com/halysongoncalves/pugnotification/master/art/screencshot.png)

1. [HeartProgressBar](https://github.com/Geek-1001/HeartProgressBar)

	自定义心形进度条。
	
	![image](https://camo.githubusercontent.com/e4121c187c0410c8473c52aaace6a1fb2c588e1a/68747470733a2f2f7777772e64726f70626f782e636f6d2f732f67746f766a7a68636f336430757a692f686561727450726f67726573734261722e6769663f646c3d31)

1. [ArcLayout](https://github.com/ogaclejapan/ArcLayout)

	效果很赞的弧形布局。
	
	![image](https://raw.githubusercontent.com/ogaclejapan/ArcLayout/master/art/demo1.gif)	

1. [Point-of-Android](https://github.com/FX-Max/Point-of-Android)

	Android 一些重要知识点解析整理.

1. [FloatingActionButton](https://github.com/Clans/FloatingActionButton)

	Material Design风格的Floation Action Button，并且支持Floating  Action Menu。
	
	![image](https://raw.githubusercontent.com/Clans/FloatingActionButton/master/screenshots/menu_default_opened.png)

1. [richeditor-android](https://github.com/wasabeef/richeditor-android)

	一个	漂亮的所见即所得的富文本编辑控件。
	
	![image](https://raw.githubusercontent.com/wasabeef/richeditor-android/master/art/demo2.gif)

1. [Direct-Load-apk](https://github.com/FinalLody/Direct-Load-apk)

	Direct - load - apk 是一个强大的插件化框架, 通过使用它, 你可以实现看似不可能实现的功能 ----- 直接加载一个普通apk!

	优势:

	* Direct - load - apk 能够加载插件的全部 资源.
	* 支持 插件间 Activity跳转.
	* 不像 "[dynamic load-apk](https://github.com/singwhatiwanna/dynamic-load-apk)" 这个项目, "[Direct-load-apk](https://github.com/FinalLody/Direct-Load-apk/)" 不需要对插件有任何约束，也不需要在插件中引入jar和继承自定义Activity，可以直接使用this指针。

1. [ColorTrackView](https://github.com/hongyangAndroid/ColorTrackView)

	字体或者图片可以逐渐染色和逐渐褪色的动画效果。
	
	![image](https://raw.githubusercontent.com/hongyangAndroid/ColorTrackView/master/sample_ColorTrackeView/changecolortvdemo.gif)
		
### 工具	 

1. [Android Studio 1.2 Beta](http://www.androiddevtools.cn)

	Andorid Studio 1.2 更新 Android Studio 基于 IntelliJ 14.1.1，包括了 IntelliJ 14 和 14.1 的所有特性，主要是：
	
	* 新调试器
	* distraction free mode
	* 同步 tag 编辑
	* 编辑器优化
	* 新增和改进重构操作
	* 注解推断，草稿文件，改进 Gradle 支持
	* 详情请看 https://www.jetbrains.com/idea/whatsnew/ 
	
	摘自：http://www.lupaworld.com/portal.php?mod=view&aid=251669
	
1. [apk方法统计工具](http://inloop.github.io/apk-method-count)

	一个在线的Apk方法统计工具。
	
### 视频


1. [免费的Android性能优化进阶课程](http://v.youku.com/v_show/id_XOTI2NDE1NjAw.html?f=23631701)

	Google日前联合Udacity推出了免费的Android性能优化进阶课程，内容主要涉及Android性能问题，如何使用AS各种工具分析和解决性能问题，本着方便国内小伙伴学习的目的，课程中文介绍：[http://chenqichao.me/2015/04/06/115-Android-Performance/](http://chenqichao.me/2015/04/06/115-Android-Performance/)

1. [Android Material Design Tutorial](https://www.youtube.com/watch?v=hrlGVU8z7zc&list=PLonJJ3BVjZW6CtAMbJz1XD8ELUs1KXaTD&index=2)
	
	一步步带你学习Android Material Design.
	
### 新闻

1. [Android 应用很快就能跑在 Chrome 上了](http://www.ifanr.com/507658?object_type=webpage&url_type=39&pos=1)
	
	Google 让 Chrome OS 运行 Android app 的想法早已有之，并在去年的 9 月份付诸行动，推出了 [App Runtime for Chrome](https://developer.chrome.com/apps/app_runtime)，简称 ARC，是一个运行在 Chrome OS 上的 Android 虚拟机，它本身是一个 Chrome Web 商店的应用程序，名为 [ARC Welder](https://chrome.google.com/webstore/detail/arc-welder/emfinbmielocnlhgmfkkmkngdoccbadn)。
			
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)