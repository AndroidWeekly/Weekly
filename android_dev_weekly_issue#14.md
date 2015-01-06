---
layout: post
title: "Android开发周报 Issue#14"
date: 2015-01-05 23:41:36 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发周报 Issue#14 

### 新闻

1. [慎用Java日期格式化](http://www.infoq.com/cn/news/2015/01/java-date-format-with-caution)
	
	这条留言实际指向了Twitter上的一个帖子，这个帖子提醒大家，如果使用了YYYY的格式符来格式化日期，那么就有可能用错格式了。Reddit的一位读者解释说，Twitter由于误用格式符，把当天的日期变成了2015年12月的某天。
	
### 教程

1. [ART运行时垃圾收集机制简要介绍和学习计划](http://blog.csdn.net/luoshengyang/article/details/42072975)

	为了学习ART运行时的垃圾收集机制，我们先把Dalvik虚拟机的垃圾收集机制研究了一遍。这是因为两者都使用到了Mark-Sweep算法，因此它们在概念上有很多一致的地方。然而在实现上，Dalvik虚拟机的垃圾收集机制要简单一些。这样我们就可以先从简单的Dalvik虚拟机垃圾收集机制入手，然后再逐步深入地学习复杂的ART运行时垃圾收集机制。

1. [Material Design in Action — 猿题库](http://www.jianshu.com/p/6c2b7d261e1a)

	猿题库很早之前就发布了 Android 版本的客户端，但猿题库的联合创始人，郭常圳 先生，并不认同 Android Design （或者现在的 Material Design），而且认为应用程序的设计规范，应当由开发商来规定。然而当我试用猿题库的时候发现，这个应用对其进行 Material Design 的适配，其实并不困难。因此就有了对其进行重新设计的念头。

1. [正确使用Android性能分析工具——TraceView](http://blog.jobbole.com/78995/)

	最近公司app中有些列表在滑动的时候会有卡顿现象，我就开始着手解决这些问题，解决问题之前首先要分析列表滑动的性能瓶颈在什么地方。因为之前不会正确使用TraceView这个工具，主要是看不懂TraceView界面下方数据指标的值代表什么意思…以前我用StopWatch类来分析性能，现在觉得弱爆了…不过有些地方StopWatch工具类还是很简单好用的~

<!--more-->

1. [Gradle 中的 task 依赖](http://testerhome.com/topics/1756)
	
	文章讲解了如何自定义Gradle的task，以及怎样定义task之间的依赖关系。
	
1. [动画系列 - ViewPger动画](http://www.lightskystreet.com/2014/12/15/viewpager-anim/)

	本篇文章介绍的ViewPager动画，可以分为两类，第一类是针对于ViewPager的界面滑动动画(这个是PageTransformer的真正用途)，分析并比较了AndroidImageSlider和JazzyViewPager两种实现，第二类是对ViewPager中的内容进行动画处理，这个是这个是PageTransformer的巧妙应用，处理好了可以达到很棒的交互效果，示例是Yahoo天气的视差效果。

1. [如何定位Android NDK开发中遇到的错误](http://www.csdn.net/article/2014-12-30/2823366-Locate-Android-NDK)

	Android NDK中的错误定位对很多开发者来说是一件头疼的事，本文通过一个Demo程序详细讲解了NDK的错误是如何产生的，以及如何通过命令行工具定位NDK的问题所在。

1. [Android 编程下 Touch 事件的分发和消费机制](http://www.cnblogs.com/sunzn/archive/2013/05/10/3064129.html)

	Android 中与 Touch 事件相关的方法包括：dispatchTouchEvent(MotionEvent ev)、onInterceptTouchEvent(MotionEvent ev)、onTouchEvent(MotionEvent ev)；能够响应这些方法的控件包括：ViewGroup、View、Activity。

1. [Android源码下载和编译总结](http://weibo.com/p/1001603793195556321741)

	前几天常用的笔记本电脑挂了，要拿去维修，于是就准备用另一台备用电脑来重新下载和编译一下Android源码，以便工作研究之用。鉴于最近一直都有人问下载和编译Android源码的问题，并且我上一次写Android源码编译的文章已经是2011年的事情，于是就趁这个机会写篇文章总结一下。

### 代码&开源库

1. [awesome-android-ui](https://github.com/wasabeef/awesome-android-ui)

	一些 Android UI/UX 库的集合列表。
	
1. [android-native-dependencies](https://github.com/nhachicha/android-native-dependencies)

	一个解析和下载Android native 依赖的Gradle插件。
	
1. [ErrorView](https://github.com/xiprox/ErrorView)

	一个用来显示错误信息的自定义View，包含图标、主标题、自标题和重试按钮。
	
	![image](https://raw.githubusercontent.com/xiprox/ErrorView/master/graphics/screenshots/ss_01.png)

1. [DraggableFlagView](https://github.com/wangjiegulu/DraggableFlagView)

	可拖拽的红点，（仿新版QQ，tab下面拖拽标记为已读的效果），拖拽一定的距离可以消失回调。
	
### 工具	 	 

1. [Hyperfox](https://hyperfox.org/)

	一个用Go 语言写的强悍的抓包工具！可以抓取https协议的！
	
	![image](https://hyperfox.org/images/hyperfox-diagram.png)

### 设计
	
### 教程

1. 	[大屏手机时代，如何重塑界面交互](http://www.tuyiyi.com/w/36011.html)

	这是一个大屏手机的时代。强调这件事情的意义在于，这已经成为事实。Medium上存在一份个人统计。在过去7年，新上市的手机屏幕尺寸越来越大。
		
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)