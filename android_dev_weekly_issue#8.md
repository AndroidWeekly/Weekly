---
layout: post
title: "Android开发周报 Issue#8"
date: 2014-11-24 10:56:01 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发周报 Issue#8
	
### 文章

1. [使用gradle构建android项目（续）](http://blog.isming.me/2014/11/21/use-gradle-new/)

	在几个月之前，我已经写过一篇使用gradle构建android项目的博客了[http://blog.isming.me/2014/05/20/android4gradle/](http://blog.isming.me/2014/05/20/android4gradle/),那篇文章已经介绍了如何使用gradle进行项目构建，以及为谷歌会推荐使用gradle。当时android的gradle插件是0.11.0,现在插件的版本已经是0.14.3了，对于一些老的方法和api，有一些已经被移除，无法使用。因此有必要再写一篇博客介绍这些被移除的部分和替代方案。同时由于个人学识原因，当时没有介绍的一些技巧，其他功能，也会在本文中进行介绍。

1. [直接拿来用！十大Material Design开源项目](http://www.csdn.net/article/2014-11-21/2822753-material-design-libs/1)

	本文详细介绍了十个Material Design开源项目，从示例、FAB、菜单、动画、Ripple到Dialog，看被誉为“Google第一次在设计语言和规范上超越了Apple”的Material Design是如何逐渐成为App的一种全新设计标准。另外推荐大家去 Github 上 Star 或者 Fork [`MaterialDesignCenter`](https://github.com/lightSky/MaterialDesignCenter)这个项目，该收集整理了

1. [放弃WebView，使用Crosswalk做富文本编辑器](http://www.cnblogs.com/ct2011/p/4100132.html)
	
	Android WebView做普通浏览还好，做富文本编辑器（`document.body.contentEditable=true;`），常常会遇到各种奇葩的bug，而且很难修复。尽管Google在版本迭代中不断修复bug，但依旧没法用它来做富文本编辑。
	
1. [在低版本android系统上实现Material设计应用](http://blog.isming.me/2014/11/17/material-design-for-pre-lollipop-android/)

	​Material Design真的很好看，动画效果真的很实用。前面也写了一些文章介绍如何编写Material风格的程序，但是很多都是一些新的api，低版本上面没有这些api，我们没办法使用。但是不用气馁，google官方，以及一些大牛，给我们提供了一些程序，让我们在低版本上面可以实现Material风格的程序，这里就给大家介绍一下。

<!--more-->

1. [使用RoundedBitmapDrawable快速生成圆角和圆形图片](http://qichaochen.github.io/2014/11/17/106-Android-RoundedBitmapDrawable/)

	在I/O大会之后，Google发布了新的Support lib，其中有一个是RoundedBitmapDrawable类，通过这个类可以很容易实现圆角和圆形图片。

1. [“黑暗潜伏者” -- 手机病毒新型攻击方式分析](http://blog.csdn.net/androidsecurity/article/details/41207959)

	近期百度安全实验室发现一款“黑暗潜伏者”新型手机病毒。该病毒附着在众多壁纸和游戏类应用中。截至目前，已经发现感染该病毒的应用超过1万多款，感染用户超过3000万。

1. [正确使用Android性能分析工具——TraceView](http://blog.jobbole.com/78995/)

	TraceView是一个非常强大的性能分析工具，因为Android 官网对这个工具的使用介绍文档很少，而且一些中文博客中写的也都是抄来抄去，没有讲到底怎么使用。


1. [移动web开发框架研究](http://blog.csdn.net/xyz_lmn/article/details/41052977#0-tsina-1-81289-397232819ff9a47a7b7e80a40613cfe1)

	 纯粹的总结一下移动web开发框架，移动web开发框架有jQuery Mobile 、Sencha Touch等等,他们都来源于web开发，是成熟的框架，jQuery Mobile出自于jQuery家族，Sencha Touch来自于ExtJS。jQuery Mobile 和Sencha Touch都是比较成熟老牌的框架，项目中也有应用。国内也有公司，像BAT巨头也在探索和实现了适合自己的移动web框架。


### 代码&开源库

1. [GitLabAndroid](https://github.com/ekx/GitLabAndroid)

	GitLab的非官方开源客户端.
	
	![image](https://github.com/ekx/GitLabAndroid/raw/master/screenshots.png)
1. [awesome-android](https://github.com/snowdream/awesome-android)

	收集整理了Gihub上Android相关的各种开源控件。

1. [Netroid](https://github.com/vince-styling/Netroid)
	
	Netroid是一个基于Volley实现的Android Http库。提供执行网络请求、缓存返回结果、批量图片加载、大文件断点下载的常见Http交互功能。致力于避免每个项目重复开发基础Http功能，实现显著地缩短开发周期的愿景。

1. [RevealLayout](https://github.com/kyze8439690/RevealLayout)

	附带一些Reveal动画效果的Layout，支持Android4.0以上系统。

1. [CircularReveal](https://github.com/03uk/CircularReveal)
	
	可以让你在2.3+系统使用Android 5.0的Reveal动画效果的库。

1. [RoundedLetterView](https://github.com/pavlospt/RoundedLetterView)

	仿Android 5.0联系人App的列表效果。

1. [UpdateHelper](http://git.oschina.net/shelwee/UpdateHelper)
	
	UpdateHelper是一个为了简化Android App的迭代升级开发的Android Library。

### 新闻

1. [不任性了！Google Play宣布开通国内开发者通道](http://www.csdn.net/article/2014-11-20/2822732-google-play-android-dev-china)

	Google今天宣布，中国的开发者现在可以通过Google Play将付费应用程序向130个国家进行发布。开发者可以利用Google Play发布免费及付费应用程序，并支持应用程序内购买和订阅，收入将汇至开发者在中国本地银行账户。

1. [安卓编年史(1)](http://linux.cn/article-4249-1.html)
	
	让我们跟着安卓从0.5版本到4.4的无尽迭代来看看它的发展历史。安卓已经以不止一种形式陪伴了我们六年以上。在这段时间内，我们已经看到了不同于任何已有开发周期的，绝对惊人的变化速度。当Google卷入智能手机的战场中时，它拿出了它的快速迭代，Web风格的更新周期，把它们应用到了开发这个操作系统之中，而结果就是突击式的持续改进。
	
### 视频

1. [Google Play 中国开发者中文入门视频](http://www.youku.com/playlist_show/id_23094862.html)

	Google Developers 最新发布的 3个 Google Play 中国开发者中文入门视频。教你怎么注册成为Google play开发者。

1. [Tutorial Enhancing Android UI with Custom Views](http://v.youku.com/v_show/id_XODMwMjg5Nzg4.html)

	Android自定义View视频教程，中文字幕，示例源码地址:http://pan.baidu.com/s/1pJp0CIn

1. [Droidcon London 2014的视频](http://www.youku.com/playlist_show/id_23078962.html)

	包含《What's New in Android》、《Material design & implementation》和《Deep Dive Into the Gradle》这个3个视频，都是来自官方工程师的干货。
	
1. [移动应用性能揭秘](http://www.infoq.com/cn/presentations/expose-mobile-application-performance)

	目前大部分移动应用都是需要与服务器进行交互的，哪么影响这些应用程序性能的主要因素有哪些？如网络请求、IO操作、多线程等都会对性能产生影响，本议题将分享基调网络在移动应用性能监控中遇到的与移动应用性能提升相关的代码问题，希望能够为程序员开发高性能的应用提供帮助。

### 工具

1. [rest2mobile](https://developer.magnet.com)

	一个可以将REST services生成Objective-C、Javascript和Java代码的开源工具，并且提供了支持Xcode、Android Studio & IntelliJ IDEA的生成代码的插件以及可以生成iOS，JS和Android跨平台代码的命令行工具。

	![image](http://ww2.sinaimg.cn/bmiddle/8a41f469jw1emk7cqynx7j21cw1660xx.jpg)

1. [树形展示 Github 项目代码的Chrome插件](https://chrome.google.com/webstore/detail/octotree/bkhaagjahfmjljalopjnoealnfndnagc) （@程序员的那些事）

	国外程序员 Buu Nguyen 做的一个 Chrome 插件，安装之后，浏览托管在Github上的项目，可看到左侧的树形结构，更方便查看代码（有点 IDE 的感觉，用着好来点个赞吧）。
	
	![image](http://ww4.sinaimg.cn/bmiddle/7cc829d3jw1egep4g1ljcj20h10ae3zy.jpg)

1. [Android Launcher图标在线生成工具](http://jgilfelt.github.io/AndroidAssetStudio/icons-launcher.html#foreground.space.trim=1&foreground.space.pad=0&foreColor=E8EAF6%2C0&crop=0&backgroundShape=square&backColor=3F51B5%2C100&effects=none&elevate=0)
	
	一个帮助你快速生成Android Launcher图标的在线生成工具，此工具是由Google 的 [`Roman Nurik`](https://github.com/romannurik)大神开发的 [`AndroidAssetStudio`](https://github.com/romannurik/AndroidAssetStudio) 系列Android资源自动生成工具（包含：）中的其中一个，支持从指定图片、文字和内置的icon生成Android Launcher图标，并且可以设置图标的前景和背景色，缩放类型、图标形状等。
	
	![image](http://ww4.sinaimg.cn/bmiddle/005GSHYzjw1emit4rrvf7j318g158tds.jpg)

1. [Astral](http://astralapp.com)（@WillYan）
	
	可以把你Github上加星的项目进行标签管理，用Github账号授权登陆即可，强迫症患者的福音啊😄。

	![image](http://ww2.sinaimg.cn/bmiddle/5fb87788tw1emils89ritj20x50g6tb2.jpg)

1. [Android Studio 1.0 Release Candidate 1](http://tools.android.com/download/studio/canary/1-0rc1)	
	这次发布的是Android Studio 1.0候选版，那么距离发布Android Studio 1.0 正式版已经不远喽😄。此次更新主要修复了一些Bug，更换了新的图标和启动界面以及包含了Android Gradle插件所需要的所有依赖，当你新建一个项目的时候就不需要联网了。
	墙内下载地址：[http://www.androiddevtools.cn/#android-studio](http://www.androiddevtools.cn/#android-studio)
	
1. [TinyJPG](https://tinyjpg.com)

	一个支持jpg和png格式的图片压缩工具，只压图片的大小而图片的质量不会损失。
	
	![image](http://ww1.sinaimg.cn/bmiddle/8a41f469jw1emhtewxnysj21kw0imagj.jpg)

1. [IOS and Android App Icon size generator](http://www.appiconsizes.com)

	一键生成iPhone, Android, IOS, Facebook, web touch icons, Blackberry, Windows Phone, Bada and WebOS 等系统App图标的在线工具.

1. [fplutil](http://google.github.io/fplutil/)
	
	一套可以用于开发Android和其他跨平台应用的库和工具。
	
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)