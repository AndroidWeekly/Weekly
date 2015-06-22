layout: post
title: "Android开发技术周报 Issue#31"
date: 2015-05-12 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#31

### 教程

1. [LeakCanary: 让内存泄露无所遁形](http://www.liaohuqiu.net/cn/posts/leak-canary/)	
	一些对象有着有限的生命周期。当这些对象所要做的事情完成了，我们希望他们会被回收掉。但是如果有一系列对这个对象的引用，那么在我们期待这个对象生命周期结束的时候被收回的时候，它是不会被回收的。它还会占用内存，这就造成了内存泄露。持续累加，内存很快被耗尽。

1. [移动端尺寸基础知识](http://www.imooc.com/wenda/detail/261436) (@慕课网)

	初涉移动端设计和开发的同学们，基本都会在尺寸问题上纠结好一阵子才能摸到头绪。我也花了很长时间才弄明白，感觉有必要写一篇足够通俗易懂的教程来帮助大家。从原理说起，理清关于尺寸的所有细节。由于是写给初学者的，所以不要嫌我啰嗦。

1. [NotRxJava懒人专用指南](http://www.devtf.cn/?p=323) (@开发技术前线)

	如果你是一位 Android 开发者，那么这些天你可能已经听到或看到一些关于 RxJava 满天飞的宣传了。RxJava 是一个能让你摆脱编写一些复杂繁琐的代码去处理异步事件的库。一旦开始在你的项目中使用，你会对它爱不释手的。

1. [模仿ButterKnife的ViewBinder机制](http://www.cnblogs.com/wenjiang/p/4298143.html) (@慕课网Android学习小组)

	ButterKnife的使用极大方便了Android程序员的开发，实际上，我们可以自己模仿一下实现。首先就是要了解Java注解的使用。我们首先要声明一个@interface，也就是注解类：@interface是用于自定义注解的，它里面定义的方法的声明不能有参数，也不能抛出异常，并且方法的返回值被限制为简单类型、String、Class、emnus、@interface，和这些类型的数组。

1. [安卓APP动态调试技术](http://www.droidsec.cn/安卓app动态调试技术/) (@DroidSec安卓安全中文站)

	随着智能手机的普及，移动APP已经贯穿到人们生活的各个领域。越来越多的人甚至已经对这些APP应用产生了依赖，包括手机QQ、游戏、导航地图、微博、微信、手机支付等等，尤其2015年春节期间各大厂商推出的抢红包活动，一时让移动支付应用变得异常火热。然后移动安全问题接憧而至，主要分为移动断网络安全和客户端应用安全。

### 代码&开源库

1. [LeakCanary](https://github.com/square/leakcanary)

	Android 和 Java 内存泄露检测工具库。[LeakCanary 中文使用说明](http://www.liaohuqiu.net/cn/posts/leak-canary-read-me/)
	
1. [Bookends](https://github.com/tumblr/Bookends)

	可以给 RecyclerView 添加 headers 和 footers 的库。

1. [android_gradle_script](https://github.com/lihei12345/android_gradle_script)

	android批量打包脚本，持续适配最新Android studio版本.

1. [Trigger](https://github.com/airk000/Trigger) （@打杂的机器猫）

	事件触发器，类JobScheduler。

1. [ElasticDownload](https://github.com/Tibolte/ElasticDownload)

	一个效果炫酷的下载进度条。

### 工具

1. [androidtool-mac](https://github.com/mortenjust/androidtool-mac/releases/) (@李锦发)

	 一款用 Swift 写的可在 Mac 上使用的 Android 工具, 支持一键截屏, 视频录制, APK 安装等功能。

### Tips

1. Android Webview在4.4的坑 (@hi大头鬼hi)

	4.4以下的webview会将url中的反斜杠\强制转换成斜杠/，也是醉了，解决方案就是先escape以下，Java中再用URI.decode获取原来的url。可以参考[@hi大头鬼hi](http://stackoverflow.com/questions/19911226/android-webview-4-4-converts-custom-url/30057785#30057785)在StackOverFlow的回答。
			
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)