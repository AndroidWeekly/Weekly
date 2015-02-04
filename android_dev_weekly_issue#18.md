---
layout: post
title: "Android开发技术周报 Issue#18"
date: 2015-01-19 13:48:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#18

### 新闻

1. [Groovy 2.4发布，支持Android开发](http://www.infoq.com/cn/news/2015/01/groovy-2-4-released)

	近日，Groovy编程语言的管理者Guillaume Laforge在博客上宣布了Groovy 2.4发布的消息。就在不久前，Pivotal宣布不再资助Groovy/Grails项目，Groovy 2.4将成为Pivotal资助下的最后一个主要的Groovy版本。Groovy 2.4最大的亮点就是对Android的支持，现在开发者可以完全使用Groovy编写Android应用了，而且与Java相比，可以省去很多样板代码。

### 教程

1. [Android应用性能优化实践](http://yanghui.name/blog/2015/02/01/2015-1-31-ali-technical-salon/)

	周末跑去深圳参加了一场阿里主持的技术沙龙，主题是《如何构建高可用的APP》，沙龙中相关的ppt和视频可以在他们的微博中找到。沙龙中收获比较大的是有关UC的何杰分享的Android应用性能优化实践，和手Q web业务优化的解析。

1. [android动画-View Animation](http://blog.isming.me/2015/02/01/android-view-animation/)

	视图动画（View Animation）,又称补间动画（Tween Animation）,即给出两个关键帧，通过一些算法将给定属性值在给定的时间内在两个关键帧间渐变。本文首先讲解各种基本动画的使用，其实介绍View动画的工作过程。

1. [用开源项目ActivityOptionsICS让ActivityOptions的动画实现兼容](http://www.cnblogs.com/tianzhijiexian/p/4128045.html)

	我之前写过一篇文章是讲解ActivityOption的api方法的（http://www.cnblogs.com/tianzhijiexian/p/4087917.html），当时吐槽各种动画不兼容，完全无视我们4.x或者2.x用户嘛，好在有开源库来帮助我们实现动画。

1. [android:clipToPadding属性的分析](http://www.imooc.com/wenda/detail/245687)

	ListView或GridView中android:clipToPadding属性的使用说明示例该属性的解释:Defines whether the ViewGroup will clip its drawing surface so as to exclude the padding area. 什么意思呢?就是说:clipToPadding属性定义了是否允许ViewGroup在padding中绘制,该值默认为true,即不允许.

<!--more-->

1. [JNI/NDK开发指南](http://blog.csdn.net/xyang81/article/category/2759987)

	相信很多做过Java或Android开发的朋友经常会接触到JNI方面的技术，由其做过Android的朋友，为了应用的安全性，会将一些复杂的逻辑和算法通过本地代码（C或C++）来实现，然后打包成so动态库文件，并提供Java接口供应用层调用，这么做的目的主要就是为了提供应用的安全性，防止被反编译后被不法分子分析应用的逻辑。

1. [Android NDK开发Crash错误定位](http://blog.csdn.net/xyang81/article/details/42319789)

	在Android开发中，程序Crash分三种情况：未捕获的异常、ANR（Application Not Responding）和闪退（NDK引发错误）。其中未捕获的异常根据logcat打印的堆栈信息很容易定位错误。ANR错误也好查，Android规定，应用与用户进行交互时，如果5秒内没有响应用户的操作，则会引发ANR错误，并弹出一个系统提示框，让用户选择继续等待或立即关闭程序。

1. [Android APP安全测试入门](https://sobug.com/article/detail/7)

	最近这两年移动端真是非常火，每个单位或多或少都会有那么几款App，对于我们Web安全攻城师来说，App安全也需要或多或少的了解一些。年初单位来了一位对App安全略有研究的小伙伴，某日闲来无事教了笔者几招，分享给大家。有句古语:”工欲善其事，必先利其器”，我们要研究App安全，没有几款高大上的神器是会非常麻烦的，因此本文主要给大家分享一下笔者学到的一些基础知识，主要是一些移动端测试辅助工具的使用。

1. [Java多线程编程模式实战指南](http://www.infoq.com/cn/author/黄文海)

	Active Object模式是一种异步编程模式。它通过对方法的调用与方法的执行进行解耦来提高并发性。若以任务的概念来说，Active Object模式的核心则是它允许任务的提交（相当于对异步方法的调用）和任务的执行（相当于异步方法的真正执行）分离。

### 代码&开源库

1. [TuentiTV](https://github.com/pedrovgs/TuentiTV)

	一个Android TV应用。

1. [Android-CircleMenu](https://github.com/hongyangAndroid/Android-CircleMenu)

	自定义ViewGroup实现的圆形旋转菜单，支持跟随手指旋转以及快速旋转。
	
	![image](https://raw.githubusercontent.com/hongyangAndroid/Android-CircleMenu/master/sample_zhy_CircleMenu/screen_shot.gif)

1. [VolleyPlus](https://github.com/DWorkS/VolleyPlus)

	Volley的加强版，在Volley的基础上进行了扩展：

1. [VerticalSeekBar](https://github.com/h6ah4i/android-verticalseekbar)
	
	垂直的SeekBar，支持2.3～5.0系统。
	
	<img src="https://github.com/h6ah4i/android-verticalseekbar/raw/master/pic/gb.png?raw=true" alt="Example on Android 2.3" width="200" />
	<img src="https://github.com/h6ah4i/android-verticalseekbar/raw/master/pic/ics.png?raw=true" alt="Example on Android 4.0" width="200" />
	<img src="https://github.com/h6ah4i/android-verticalseekbar/raw/master/pic/lollipop.png?raw=true" alt="Example on Android 5.0" width="200" />

1. [ChromeOverflowMenu](https://github.com/rahulrj/ChromeOverflowMenu)

	模仿实现了Chrome的Overflow Menu的动画效果。

1. [json2view](https://github.com/Avocarrot/json2view)
	
	json2view是一个非常简单的库，它可以将JSON文件转换为Android View，从而实现无需升级Apk就可以动态的更新View的样式。

1. [/KJFrameForAndroid](https://github.com/kymjs/KJFrameForAndroid)

	KJFrameForAndroid 又叫KJLibrary，是一个帮助快速开发的框架。使用KJFrameForAndroid，你可以轻松完成http请求、网络图片加载、数据库数据保存或读取。

1. [CJFrameForAndroid](https://github.com/kymjs/CJFrameForAndroid)

	CJFrameForAndroid 是一个实现android插件化开发的框架。使用CJFrameForAndroid，apk动态加载不再是难题，更重要的是可以轻松实现插件与APP项目之间的解耦。

1. [android-pluginmgr](https://github.com/houkx/android-pluginmgr/)

	android插件化开发的框架,实现apk动态加载。
	
1. [ActivityOptionsICS](https://github.com/tianzhijiexian/ActivityOptionsICS)

	ActivityOptions Animations的兼容库，支持Android api3.1+。

1. [DragTopLayout](https://github.com/chenupt/DragTopLayout)

	一个在ViewPager头部添加一个TopView用以显示头部菜单的控件，类型豌豆荚的应用详情页实现。
	
	![image](https://raw.githubusercontent.com/chenupt/DragTopLayout/master/imgs/dragtop_1.1.0.gif)

1. [InboxLayout](https://github.com/zhaozhentao/InboxLayout)

	模仿Google Inbox邮箱的上下拉返回效果，让你的app加入真正方便的手势操作。目前已支持底部为scrollview 顶部为listview和scrollview的情况,适用于大部分场景，正在做底部为listview的情况。
	
	![image](https://raw.githubusercontent.com/zhaozhentao/InboxLayout/master/screenshot/pic.gif)

1. [icepick](https://github.com/frankiesardo/icepick)

	一个通过注解来方便我们保存和恢复Android Instance状态的Library。
	
### 工具	 

1. [Android Studio 1.1 Beta 2](http://www.androiddevtools.cn)

	

### 视频

1. [React.js Conf 2015 Keynote](http://www.tudou.com/programs/view/A-1wE18UWeA/)
	
	React是Facebook开源的一个方便开发大型WebApp的框架。 

1. [Android图案解锁](http://www.imooc.com/view/308)
	
	本课程将带领大家通过自定义控件实现一个图案解锁的功能，包括自定义控件的使用、常见绘图操作、控件事件处理、监听器使用、以及综合案例的应用。
	
1. [多种多样的App主界面Tab实现方法](http://www.imooc.com/view/264)	
	Tab选项卡几乎成为了App必备的一个功能，它的实现方法也是多种多样，本课程就将讲解迄今为止最主流的4种实现Tab的方法，包括ViewPager、Fragment、FragmentPagerAdapter和ViewPagerIndicator。

1. [安卓APP漏洞的静态检测方法](http://www.infoq.com/cn/presentations/static-detection-method-for-android-app-vulnerabilities)

	安卓系统凭借其灵活和开放的特性获得了市场的青睐，但开放性也意味着APP开发者需要为安全负更大的责任。一方面在安卓APP这个快速发展的领域有大量新手开发者的加入，另一方面即使经验丰富的开发者也难免犯错误，安卓应用的漏洞层出不穷，值得我们深入研究。由于安卓APP的功能越来越多，代码逻辑越来越复杂，漏洞常常隐藏在深处，只有触发到一系列特定条件后才会被触发。

### 小技巧

1. 查看task stack中当前正在运行的activity([@hi大头鬼hi](http://weibo.com/brucefromsdu))

		adb shell dumpsys activity activities | sed -En -e '/Running activities/,/Run #0/p'

2. Android使用Chrome远程调试Webview([@hi大头鬼hi](http://weibo.com/brucefromsdu))
	
	1. chrome中输入`chrome://inspect/#devices`
	2. 代码中需要开启webview debug 
	
			if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.KITKAT) { 
				WebView.setWebContentsDebuggingEnabled(true); 
			}
		
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)