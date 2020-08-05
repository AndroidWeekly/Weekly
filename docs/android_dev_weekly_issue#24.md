3---
layout: post
title: "Android开发技术周报 Issue#24"
date: 2015-03-18 14:13:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#24

### 教程

1. [细数Android系统那些DOS漏洞](http://drops.wooyun.org/papers/5272)

	Android系统存在一些漏洞可导致系统重启，当然让系统重启只是一种现象，这些漏洞有的还可以权限提升、执行代码等。本文以重启这个现象为分类依据，牵强的把这些漏洞放在一块来看。下面对这些漏洞的成因和本质进行简单的分析，并尽量附上编译好的poc和漏洞利用演示视频。

1. [Android安全系列](http://drops.wooyun.org/author/瘦蛟舞)

	此系列包含：[Android Activtity Security](http://drops.wooyun.org/tips/3936)、[Android Content Provider Security](http://drops.wooyun.org/tips/4314)、[Android Broadcast Security](http://drops.wooyun.org/tips/4393)、[Android Service Security](http://drops.wooyun.org/tips/4907)以及[Android Logcat Security](http://drops.wooyun.org/tips/3812)等五篇文章

1. [Android内存优化总结](http://www.jianshu.com/p/d9ba8573a940?utm_campaign=haruki&utm_content=note&utm_medium=reader_share&utm_source=weibo)

	之前做过公司产品的内存优化，不过时间有一段时间了，可能记忆不全，欢迎大家添加补充，有错误之处也方便指出。1、追查内存的方法，第一步：使用lint；第二步：使用脚本每隔1s输出对应包的PSS值；第四步：使用MAT分析内存。

1. [Android Tv应用开发体验](http://blog.fangjie.info/android-tv应用开发体验/)

	这两天为公司的产品做Tv版适配，以前只是以为Tv版应用和Pad版本应用一样，只是做下简单的屏幕适配就可以，实践了下，除了屏幕适配，还有焦点的处理和手势操作，以及有些区别。

1. [Settings中显示密码选项是怎样工作的](http://2.rogerbolg.sinaapp.com/?p=54)

	最近由于工作上的需要，研究了一下framework层面的东西。收获良多，感受颇深啊。
在 设置->安全 中选择屏幕锁定，选择屏幕锁定方式为密码，然后勾选显示密码选项，此时应该在输入密码时，先显示输入的密码，过1.5S后将变为小圆点，若取消显示密码则输入直接为小圆点。
而由于“前人”对锁屏的改动造成取消显示密码后，还是先显示密码才跳为小圆点，这是我要解决的BUG。

1. [安卓调试神器andbug安装使用指南](http://appscan.360.cn/blog/?p=112)

	Andbug是基于jdwp协议的一个非常强大的安卓调试工具，该工具使用了python封装，其灵活性和可定制性堪称神器级别的安卓安全工具。由于原作者不再维护工具并未被大家熟知，但其中有很多功能仍然被很多技术大牛扩展开发了许多私有功能，如看雪的anbc大牛几年前就给andbug二次扩展了一个monitor功能。

1. [Java容器&泛型：一、认识容器](http://www.bysocket.com/?p=162#0-tsina-1-86659-397232819ff9a47a7b7e80a40613cfe1)

	容器是Java语言学习中重要的一部分。泥瓦匠我的感觉是刚开始挺难学的，但等你熟悉它，接触多了，也就“顺理成章”地知道了。Java的容器类主要由两个接口派生而出：Collection和Map。

1. [Android最佳性能实践(四)——布局优化技巧](http://blog.csdn.net/guolin_blog/article/details/43376527)

	在前面几篇文章当中，我们学习了如何通过合理管理内存，以及高性能编码技巧的方式来提升应用程序的性能。然而实际上界面布局也会对应用程序的性能产生比较大的影响，如果布局写得糟糕的话，那么程序加载UI的速度就会非常慢，从而造成不好的用户体验。那么本篇文章我们就来学习一下，如何通过优化布局来提供应用程序的性能。还没有看过前面前面一篇文章的朋友建议可以先去阅读 [Android最佳性能实践(三)——高性能编码优化](http://blog.csdn.net/guolin_blog/article/details/42318689) 。

1. [手机淘宝性能优化](http://mp.weixin.qq.com/s?__biz=MzAxNDEwNjk5OQ%3D%3D&from=groupmessage&idx=1&isappinstalled=0&mid=203394618&scene=1&sn=58b05aaf205b20c361935a02282392d9)

	为了满足不同用户的多样性购物需求，过去两年里手机淘宝的业务不断膨胀，已经从单一的购物工具成为了购物内容平台。在业务快速增长的同时，也带来一些副作用，很多操作环节和页面因为承载功能太多，展示速度变慢，用户等待时间变长，性能优化势在必行。

1. [Android开发实践：实战演练隐式Intent的用法](http://ticktick.blog.51cto.com/823160/1621957#0-tsina-1-31485-397232819ff9a47a7b7e80a40613cfe1)
	
	本文通过完成一个实战任务，来掌握Android开发中隐式Intent的用法。任务：假设我们已经实现了一个视频播放器（PlayerActivity），我们希望能把它注册到系统中，当用户点击本地视频或者在线视频时，能启动这个视频播放器。
	
1. [加速Android Studio/Gradle构建](http://blog.isming.me/2015/03/18/android-build-speed-up/#0-tsina-1-65794-397232819ff9a47a7b7e80a40613cfe1)

	已经使用Android Studio进行开发超过一年，随着项目的增大，依赖库的增多，构建速度越来越慢，现在最慢要6分钟才能build一个release的安装包，在网上查找资料，发现可以通过一些配置可以加快速度，这里跟大家分享一下。

1. [Android兼容性测试的一些坑](http://qa.blog.163.com/blog/static/1901470022014817936189/)

	还记得上次我们网易云音乐做大改版时，最后播放器界面适配每一款机型实在是个大工程，不同的系统，不同的分辨率，不同的尺寸都会有不一样的表现，为了达到完美的结果，需要花费很大的精力。

### 代码&开源库

1. [MaterialSettings](https://github.com/kenumir/MaterialSettings)	
	可以让你轻松创建Material Design风格的Settings Activity的库。
	
	![image](https://raw.githubusercontent.com/kenumir/MaterialSettings/master/screens/theme_default2.png)

1. [V2EX-Daily-Hot-Widget-Kotlin](https://github.com/kyze8439690/V2EX-Daily-Hot-Widget-Kotlin)

	一个用kotlin写的V2EX Daily Hot的Widget项目，对kotlin感兴趣的同学可以参考学习学习，至于kotlin是啥，可以参考以下资料：[kotlin](http://kotlinlang.org)，[kotlin源码](https://github.com/JetBrains/kotlin)，[JetBrains推出新JVM语言Kotlin](http://www.infoq.com/cn/news/2011/07/kotlin), [@JakeWharton](https://github.com/JakeWharton)大神写的一个关于在Android开发中使用Kotlin的文档Using Project Kotlin for Android[墙内地址](http://pan.baidu.com/s/1gdIQEdl)，[墙外地址](https://docs.google.com/document/d/1ReS3ep-hjxWA8kZi0YqDbEhCqTt29hG8P44aA9W0DM8/edit?forcehl=1&hl=zh-CN)，还有我在22期周报中推荐过的另外一个项目[palettehelper](https://github.com/hzsweers/palettehelper)

1. [Android源码设计模式分析项目](https://github.com/simple-android-framework-exchange/android_design_patterns_analysis)

	满满的干货，强烈推荐，该项目通过分析Android系统中的设计模式来提升大家对设计模式的理解，从源码的角度来剖析既增加了对Android系统本身的了解，也从优秀的设计中领悟模式的实际运用以及它适用的场景，避免在实际开发中的生搬硬套。

1. [android-testing](https://github.com/googlesamples/android-testing)

	Goolge官方发布的Android单元测试以、自动化测试的Sample，

1. [500px-android-blur](https://github.com/500px/500px-android-blur)

	500px公司开园的可以实现毛玻璃模糊效果的库。

1. [SimpleTagImageView](https://github.com/wujingchao/SimpleTagImageView)	
	一个可以在图片四个角显示一个小标签的ImageView，并且可以控制标签的宽度和背景颜色。
	
	![image](https://raw.githubusercontent.com/wujingchao/SimpleTagImageView/master/demo2.gif)

1. [MiClockView](https://github.com/AvatarQing/MiClockView)

	仿MIUI v6时钟效果。
	
	![image](https://raw.githubusercontent.com/AvatarQing/MiClockView/master/art/duplication.gif)
		
### 工具	 

1. [Android Sutdio 1.2 Preview 3](http://www.androiddevtools.cn/#android-studio)

	
### 新闻

1. [Android 5.1 SDK正式发布](http://www.infoq.com/cn/news/2015/03/android-5-1-sdk-release)

	3月9日，谷歌正式发布了Android 5.1版本，这一版本在稳定性和性能方面有所提升，此外在通知的控制方面也有所增强。在Android 5.1发布的第二天，作为这次Lollipop版本升级的一部分，谷歌发布了Android 5.1 SDK（API level 22）。从开发者的角度来说，Android 5.1 SDK引入了小部分新的API。其中最关键的新增API就是对多SIM卡的支持，这对许多采用Android One手机的地区来说很有意义。Android One手机的用户将可以更加灵活的在运营商之间切换，并且可以更加合适的方式管理他们的网络活动。作为开发者来说，则可以利用这一新的特性创造全新的应用体验。

1. [Android Wear 新技能：变身失物寻找器](http://tech2ipo.com/96498?utm_source=sinaweibo&utm_medium=sinaweibo_AD&utm_campaign=weibo)

	Google 昨日更新了其安卓设备管理服务 Android Device Manager，增加对 Android Wear 的支持，意味着今后用户可以用智能手表寻找丢失的手机。Google 表示更新是在后端进行，用户无需做进行操作。所有 Android Wear 设备都将在未来数周内获得更新。

1. [Google Play将引入年龄分级和人工审核机制](http://www.36kr.com/p/220715.html)
	
	Google Play 商店和苹果 App Store 最大的区别就是前者的应用不用审核。不过现在，Google 方面决定结束 Play 商店放养的状态。周二针对开发者的一篇博客显示，Google 将针对年龄组对游戏和应用进行评级，主要是为了适应不同年龄段人群的需求和不同地区的监管政策。
			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)