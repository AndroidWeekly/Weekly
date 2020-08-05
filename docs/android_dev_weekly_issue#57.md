layout: post
title: "Android开发技术周报 Issue#57"
date: 2015-11-17 12:34:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#57

### 新闻

1. [传谷歌明年在中国大陆上线Google Play](http://tech.qq.com/a/20151120/060130.htm)

	据悉，谷歌将为中国大陆市场专门制作Google Play应用商店，该应用商店将不能连接海外版Google Play。消息人士称，谷歌打算遵守中国法律对Google Play的内容进行过滤，且Google Play的数据都将存储在中国。截至目前，谷歌新加坡发言人对此报道未予置评。

### 教程

1. [Android App 线上热修复方案](http://t.cn/RU1q22P)

	热修复一词恐怕最早应用在微软。为了巩固其windows系统和office的市场占有率，微软开发并维护了一套线上修复方案，用于修复漏洞及特定问题（LDR），避免延续到发版解决（GDR），详见HotFix维基词条

1. [通往全栈工程师的捷径 —— React](http://t.cn/RUuzmLI)

	React 起源于 Facebook 的内部项目，因为 FB 对市场上所有 JavaScript MVC 框架，都不满意，就决定自己写一套，用来架设 Instagram 的网站。做出来以后，发现这套东西很好用，就在2013年5月开源了。

1. [Android应用启动优化:一种DelayLoad的实现和原理](http://androidperformance.com/2015/11/18/Android-app-lunch-optimize-delay-load.html)

	一提到DelayLoad,大家可能第一时间想到的就是在 onCreate 里面调用 Handler.postDelayed方法, 将需要 Delay 加载的东西放到这里面去初始化, 这个也是一个比较方便的方法. Delay一段时间再去执行,这时候应用已经加载完成,界面已经显示出来了, 不过这个方法有一个致命的问题: 延迟多久?

1. [Andriod性能优化之列表卡顿——以“简书”APP为例](http://blog.csdn.net/zhaokaiqiang1992/article/details/49951095)

	这几天闲得无聊，就打开手机上的开发者模式里面的“GPU过度绘制”功能，看看别家的App做的咋样，然后很偶然的打开了“简书”，然后就被它的过度绘制惊呆了，于是写了这篇性能分析的文章，从一个只有APK文件的角度，说下如何寻找布局中可能存在的性能问题，以及解决方案。本文章以简书Android最新版本1.9.1进行分析。

1. [浅析Android开源渗透测试框架Drozer中的反射交互机制](http://www.freebuf.com/tools/86180.html)

	Drozer是MWR Labs开发的一款开源Android渗透测试框架。它能够通过自身实现的协议，与Android虚拟机进行交互。良好的框架，也使得我们能够根据自身的需求，进行定制化的拓展模块开发，打造更为强大的Drozer。

1. [安卓通知栏消息点击启动Activity时“Intent flag残留”问题](http://blog.piasy.com/Android-Notification-Pending-Intent-Bug/)

	今天开发的过程中偶遇一个系统的bug：响应通知栏消息，启动一个新的Activity，之前代码写得有问题，为intent设置了Intent.FLAG_ACTIVITY_CLEAR_TASK这个flag，删除这行代码重新安装之后，竟然发现修改不起作用，启动Activity的行为依然是清除了之前所有的Activity，疑惑之余，对这个问题进行了进一步的测试，总结成此文。

1. [Java Synchronized详解](http://www.cnblogs.com/GnagWang/archive/2011/02/27/1966606.html)

	Java语言的关键字，当它用来修饰一个方法或者一个代码块的时候，能够保证在同一时刻最多只有一个线程执行该段代码。一、当两个并发线程访问同一个对象object中的这个synchronized(this)同步代码块时，一个时间内只能有一个线程得到执行。另一个线程必须等待当前线程执行完这个代码块以后才能执行该代码块。二、然而，当一个线程访问object的一个synchronized(this)同步代码块时，另一个线程仍然可以访问该object中的非synchronized(this)同步代码块。

1. [竞品技术三瞥安装包的大小](http://t.cn/RUuySYD)

	安装包为什么那么大？是什么让App安装包的体积变得如此之大？我们在前面的章节看到了iOS和Android安装包的内部结构，对于可执行文件，我们无能为力；对于xml文件，这些文件在App打包压缩后会极大减小体积，所以也不用管它们；那么就只能在图片和音频文件上做文章了。

### 代码&开源库

1. [BadgedImageview](https://github.com/yesidlazaro/BadgedImageview)

	一个支持在图片上显示一个徽章的ImageView。

1. [animate](https://github.com/hitherejoe/animate)

	一个提供了很多 Android 动画效果的实例的Demo项目。

1. [Dexter](https://github.com/Karumi/Dexter)

	一个简化Runtime Permissions请求的库。

1. [PermissionHelper](https://github.com/k0shk0sh/PermissionHelper)

	一个runtime Permissions的Help库，而且可以有不同Style的提示。

1. [Paginate](https://github.com/MarkoMilos/Paginate)

	可以结合 RecyclerView 或者 AbsListView 创建带页号的功能。

1. [AgendaCalendarView](https://github.com/Tibolte/AgendaCalendarView)

	一款在日历和议事日程间添加简易导航效果的 Android 控件。

1. [AudioWaves](https://github.com/FireZenk/AudioWaves)	
	一个可以显示声音波形的控件。

1. [GithubContributorsLib](https://github.com/alorma/GithubContributorsLib)
	
	一个可以让你很容易的显示Github上开源项目贡献者的库。

1. [CropperNoCropper](https://github.com/jayrambhia/CropperNoCropper)

	一个实现 Instagram 图片裁切风格的Demo。

### 视频

1. [Matering RecyclerView Layouts](http://pan.baidu.com/s/1dDHNPT3)

	深入剖析了RecyclerView中最核心的布局管理器部分,也捎带讲解了RecyclerView的其他机制,看完之后,你会真正明白为何ListView要被废弃。 视频中文字幕：https://github.com/oceancx/android-subtitles

1. [Droidcon 2015的视频](https://skillsmatter.com/conferences/6712-droidcon-2015#skillscasts)

	其它内容包括Gradle，Rxjava，Gradle，Infer，MaterialDesign等等，内容还是挺丰富的，质量就不用说了。


### 工具

1. [GitHub-Dark](https://github.com/StylishThemes/GitHub-Dark)

	是一款以暗黑色调为主的 GitHub 主题。	

1. [lolcat](https://github.com/busyloop/lolcat)

	一款可以将命令行终端打印日志变成彩虹色的小工具。

----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)