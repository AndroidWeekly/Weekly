layout: post
title: "Android开发技术周报 Issue#29"
date: 2015-04-22 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#29

### 教程
	
1. [Android内核解读-应用的安装过程](http://www.imooc.com/wenda/detail/257590) ([慕课网android学习小组](http://www.weibo.com/u/5321506202))

	我们知道，在android手机上安装一个apk很简单，只要打开apk文件，默认就会弹出安装界面，然后点击确定，经过若干秒后，apk就安装成功了，可是你知道apk的安装过程是什么吗？你知道android系统在安装一个apk的时候都干了什么吗？在本文中，将一一解答这个问题。简单来说，apk的安装过程分两步：第一步，将apk文件复制到程序目录下（/data/app/）；第二步，为应用创建数据目录（/data/data/package name/）、提取dex文件到指定目录（/data/dalvik-cache/）、修改系统包管理信息。

1. [给半新人的app开发指南](http://hamberluo.cn/2015/04/27/fuck-new-app/) ([@hamber_罗](http://weibo.com/316289000))

	此文献给那些需要的人，不定期更新~

1. [[译]Instagram是如何提升TextView渲染性能的](http://codethink.me/2015/04/23/improving-comment-rendering-on-android/) ([@archieyang](http://www.weibo.com/archieyang))

	在IG中，feed是由图片，视频和文字组成的。对于每个图片和视频，我们需要展示对应的图片说明和5条最近的评论。由于用户通常通过图片说明来讲书图片背后的故事，这些图片说明通常是大段复杂的文字，甚至可能包含链接和emoji表情。

1. [拿到一份开源项目，快速定位感兴趣的功能代码](http://drakeet.me/quickly-locate-the-function-code) ([@drakeet](http://www.weibo.com/drak11t))

	现在越来越多的开源项目了，令人收藏不暇，有时只是觉得对方的某个 feature 特别喜欢，但很多人可能打开了其代码找了半天找不到关键所在。其实，如果运用了 Android Studio 带给我们的一些查找功能，任何一份新的开源代码摆在我们眼前，我们都可以快速定位到感兴趣的功能代码。

1. [安卓中的Model-View-Presenter模式介绍](http://jcodecraeer.com/a/anzhuokaifa/androidkaifa/2015/0425/2782.html) ([@泡在网上编代码](http://weibo.com/2711441293/))

	这是一篇安卓中MVP模式的详细教程，从最简单的例子到最佳实践。本文还介绍了一个让在安卓中使用MVP模式变得非常简单的library。它是不是很简单，我们如何才能从中获益？什么是MVP?View是指显示数据并且和用户交互的层。在安卓中，它们可以是一个Activity，一个Fragment，一个android.view.View或者是一个Dialog。
	
1. [Android加载不同DPI资源与内存消耗之间的关系](http://www.tinylab.org/android-loading-a-different-relationship-between-dpi-and-memory-consumption-of-resources/) ([@Syleee](http://www.weibo.com/1791783305/))

	Android 设备在物理尺寸和屏幕密度上都有很大的不同，为了简化多设备的设计方案，就是设定一套分级标准。屏幕密度上的分级标准就是：LDPI、MDPI、HDPI、XHDPI，也就是各种大小的 DPI(Dots per inch)。DPI 就是屏幕像素密度的衡量标准。

1. [携程App的网络性能优化实践](http://www.infoq.com/cn/articles/how-ctrip-improves-app-networking-performance) ([@InfoQ](http://www.weibo.com/infoqchina))

	在4月23日~25日举行的QCon全球软件开发大会（北京站）上，携程无线开发总监陈浩然分享了《移动开发网络性能优化实践》，总结了携程在App网络性能优化方面的一些实践经验。在2014年接手携程无线App的框架和基础研发工作之后，陈浩然面对的首要工作就是App客户端性能优化，尤其是网络服务性能，这是所有App优化工作的重中之重.

1. [常见Android Native崩溃及错误原因](http://www.droidsec.cn/常见android-native崩溃及错误原因/) ([@DroidSec安卓安全中文站](http://weibo.com/2171682081/))

	Android上的Crash可以分两种：1、Java Crash java代码导致jvm退出，弹出“程序已经崩溃”的对话框，最终用户点击关闭后进程退出。Logcat 会在“AndroidRuntime”tag下输出Java的调用栈。2、Native Crash 通过NDK，使用C/C++开发，导致进程收到错误信号，发生Crash，Android 5.0之前进程直接退出（闪退） , Android 5.0之后会弹“程序已崩溃”的对话框。

1. [Java字节码忍者禁术](http://www.infoq.com/cn/articles/Secrets-of-the-Bytecode-Ninjas) ([@InfoQ](http://www.weibo.com/infoqchina))

	ava语言本身是由Java语言规格说明（JLS）所定义的，而Java虚拟机的可执行字节码则是由一个完全独立的标准，即Java虚拟机规格说明（通常也被称为VMSpec）所定义的。JVM字节码是通过javac对Java源代码文件进行编译后生成的，生成的字节码与原本的Java语言存在着很大的不同

1. [AppCompat 22 新特性](http://www.androidcn.org/topic/5538c3158ca8a1e07687ea33) ([@makohill](https://github.com/makohill))

	构建一个可以跑在不同版本 Android 平台的软件，是非常复杂和耗时的。为了解决这个问题，Android 推出了 Android Support Library （安卓兼容包），让新的UI控件也可以跑在早期的 Android 版本。最近Android Support Library 更新到v22.1,这一版本主要AppCompat做了一些大的调整。


1. [Android 深入理解Android中的自定义属性](http://blog.csdn.net/lmj623565791/article/details/45022631) ([慕课网android学习小组](http://www.weibo.com/u/5321506202))

	对于自定义属性，大家肯定都不陌生，遵循以下几步，就可以实现：1.自定义一个CustomView(extends View )类 2.编写values/attrs.xml，在其中编写styleable和item等标签元素 3.在布局文件中CustomView使用自定义的属性（注意namespace）4.在CustomView的构造方法中通过TypedArray获取.

1. [Android.mk详解](http://blog.csdn.net/wzy_1988/article/details/39958727)

	Android.mk文件用来向编译系统描述如何编译你的源代码。更确切地说，该文件其实就是一个小型的Makefile。由于该文件会被NDK的编译工具解析多次，因此应该尽量减少源码中声明变量，因为这些变量可能会被多次定义从而影响到后面的解析。

### 代码&开源库

1. [loadtoast](https://github.com/code-mc/loadtoast) ([@泡在网上编代码](http://weibo.com/2711441293/))

	默认的toast很丑，而且也没有真正提供显示短暂消息的功能。这个库能为toast显示动画反馈，显示到选择按钮或者删除按钮的过度动画。而且toast 的生命周期是完全取决于你的。

1. [WechatLikeBottomTabUI](https://github.com/wuyexiong/WechatLikeBottomTabUI) ([@伍业雄](http://weibo.com/1174886263/))

	抄袭微信Android6.0版本底部菜单渐变效果.

1. [squidb](https://github.com/yahoo/squidb) ([@安卓同学](http://weibo.com/1751262071/))

	Yahoo 开源的 SQLite 数据库框架，它支持ORM，面向对象语句语言（类似JOOQ）和数据库管理工具，轻量级，同时具有高性能，具体介绍请看Wiki.	

1. [android-kotlin-samples](https://github.com/irontec/android-kotlin-samples)
	
	kotlin例子库。

1. [带壳截图](https://github.com/makohill/dkjt)
	
	这是一个为手机截屏而服务的图片合成工具，基于 [Device Frame Generator](https://github.com/f2prateek/device-frame-generator) 开源项目二次开发。它可以为平淡无奇的截屏图片套上等比例的手机设备外框，生成一张媲美广告的渲染图。
	
### 视频	

1. [Android Performance Patterns : Season 2](https://www.youtube.com/playlist?list=PLOU2XLYxmsIKEOXh5TwZEv89aofHzNCiu)	([@陈启超_V](http://weibo.com/chenqichao2016))

	带头大哥Colt即将带来《Android Performance Patterns : Season 2》有Bitmap的最佳实践，迭代器性能以及如何使用LINT等。
		
### 新闻

1. [谷歌准备Android Wear重大更新](http://www.cnbeta.com/articles/387181.htm)

	谷歌今天宣布将为Android Wear推出重大更新，让Android手表使用更加容易。目前大多数Android智能手表默认都采用省电模式的表盘界面，但是，有时用户需要默认获得其它信息，Android Wear更新之后，现在将允许用户选择默认始终显示信息的应用程序，比如地图位置或者购物清单等。
			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)