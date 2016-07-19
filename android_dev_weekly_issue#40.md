layout: post
title: "Android开发技术周报 Issue#40"
date: 2015-07-13 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#40

### 教程

1. [Gradle Tips系列](http://blog.csdn.net/lzyzsd/article/details/46934187)

	由[@hi大头鬼hi](http://weibo.com/2092500601/)同学翻译的三篇很不错的Gradle文章，主要介绍了task的配置和执行，Groovy的常用语法，以及task的依赖等。另外2篇：[Gradle Tips#2-语法](http://blog.csdn.net/lzyzsd/article/details/46935063)、[Gradle tip #3-Task顺序](http://blog.csdn.net/lzyzsd/article/details/46935405)

1. [Material Design：扁而不平](http://www.jianshu.com/p/63d6011213d1)

	这篇文章本来只是篇写给同学看的短文——因为他一直认为“Android 从 4.0 开始就是扁平化设计了”....结果没想到这么想的人还不少，所以就写了这么一篇科普文，全篇偏小白，无干货，敬请放心阅读。

1. [codepath教程：浮动操作按钮详解](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2015/0718/3197.html)

	浮动操作按钮 (简称 FAB) 是: “一个特殊的promoted操作案例。因为一个浮动在UI之上的圆形图标而显得格外突出，同时它还具有特殊的手势行为”。

1. [CoordinatorLayout与滚动的处理](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2015/0717/3196.html)

	CoordinatorLayout 实现了多种Material Design中提到的滚动效果。目前这个框架提供了几种不用写动画代码就能工作的方法，这些效果包括：让浮动操作按钮上下滑动，为Snackbar留出空间。

1. [浮动操作按钮的选择](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2015/0716/3194.html)

	浮动操作按钮，现在可选的方案很多，design库中也有，目前来说在考虑实现浮动操作按钮的时候，有以下几种常用方案：官方的：`android.support.design.widget.FloatingActionButton`，优点是可以与Snackbar和 `CoordinatorLayout` 配合，在 `Snackbar` 显示的时候让出足够的空间，参见codepath的文章：[Handling Scrolls with CoordinatorLayout](https://guides.codepath.com/android/Handling-Scrolls-with-CoordinatorLayout) 。

1. [Mac OS上反编译android app的环境搭建](http://segmentfault.com/a/1190000002993196)

	很多时候，我们出于学习或者安全测试等的目的，需要对andorid app的安装文件进行反编译来查看源代码，下面我们来一起搭建Mac os 下的反编译环境。

1. [学习Android开发的二十套免费理想资源](http://mobile.51cto.com/abased-484080.htm)

	如果大家刚刚接触Android开发，那么相关教程及博客能够为各位提供具体的发展路线以及必要的编程知识，从而帮助我们顺利完成自己的首款Android应用开发项目。下面就一起来看我个人最中意的免费Android编程网站及博客。
	
1. [Android内核开发：在源码树中添加新的app应用](http://ticktick.blog.51cto.com/823160/1674206)
	
	网上也有介绍怎么在源码中添加新的app应用的博文，但大都数只介绍了不含有jni本地代码的app的添加方法，本文会更加全面地介绍三种不同类型的app应用如何添加到Android内核源码树中编译。
	
### 代码&开源库

1. [VCameraDemo](https://github.com/motianhuo/VCameraDemo)

	微信小视频+秒拍

1. [GlidePalette](https://github.com/florent37/GlidePalette)

	Android Lollipop Palette is now easy to use with Glide。

1. [ImportNewApp](https://github.com/lzjun567/ImportNewApp)

	一个专注于 Java 技术分享的博客平台的客户端。

1. [MaterialUp](https://github.com/jariz/MaterialUp)

	[MaterialUp](http://www.materialup.com)客户端。

1. [MD-BiliBili](https://github.com/Qixingchen/MD-BiliBili)

	基于 Material Design 的 BiliBili 第三方 Android 客户端.

1. [json2notification](https://github.com/8tory/json2notification)

	一个可以将JSON格式的数据转换为Android Notification的库.

1. [MaterialStatusBarCompat](https://github.com/fython/MaterialStatusBarCompat)

	完美地使 Kitkat 与 Lollipop 上的状态栏同时透明/变色。

1. [Lightweight-Stream-API](https://github.com/aNNiMON/Lightweight-Stream-API)

	Stream API from Java 8 rewrited on iterators for Java 7 and below

### 工具

1. [proxychains-ng](https://github.com/rofl0r/proxychains-ng)

	proxychains ng (new generation) - a preloader which hooks calls to sockets in dynamically linked programs and redirects it through one or more socks/http proxies.

1. [Android SDK Safari Extension](https://github.com/0legg/AndroidSDKSafariExtension)

	A Safari extension that adds view source links for the Android SDK.

### 设计资源	

1. [Icons4Android](http://www.icons4android.com/)	
	Icons4android是一套极具人气的在线资源集合，能够帮助我们为自己的Android应用程序找到理想的图标素材。这些图标皆可以单一zip压缩文件的形式下载，且提供五种不同尺寸以及十二种配色方案。

----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)