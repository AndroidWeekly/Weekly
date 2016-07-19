---
layout: post
title: "Android开发周报 Issue#12"
date: 2014-12-22 09:54:44 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发周报 Issue#12
	
### 文章

1. [Dalvik虚拟机垃圾收集（GC）过程分析](http://blog.csdn.net/luoshengyang/article/details/41822747)

	 前面我们分析了Dalvivk虚拟机堆的创建过程，以及Java对象在堆上的分配过程。这些知识是理解Dalvik虚拟机垃圾收集过程的基础。垃圾收集是一个复杂的过程，它要将那些不再被引用的对象进行回收。一方面要求Dalvik虚拟机能够标记出哪些对象是不再被引用的。另一方面要求Dalvik虚拟机尽快地回收内存，避免应用程序长时间停顿。本文就将详细分析Dalvik虚拟机是如何解决上述问题完成垃圾收集过程的。

1. [使用Android Studio查看Android Lollipop源码](http://www.jianshu.com/p/c85984cf99e2?utm_campaign=maleskine&utm_content=note&utm_medium=writer_share&utm_source=weibo)

	作为Google的亲儿子,Nexus手机系列所收到的待遇大家有目共睹.Android5.0出来之后,Nexus5第一时间就升级到了最新的系统.那么作为Google亲儿子的Android Studio同样备受Google的重视,我也是第一时间从Eclipse转投到了Android Studio的怀抱中,从最初的测试版本一路升级到现在的1.0正式版本(今天发布了1.0.2,果断已经升级了),关于Android Studio的好处我就不用说了...

1. [Facebook工程师是如何改进他们Android客户端的](http://greenrobot.me/devnews/facebook-engineer-improve-android-app/)

	作为世界上最大的社交网络，Facebook的Android客户端面临着各种各样的使用环境（地理环境、Android设备以及移动网络等环境的差异）。也正是这个原因，为了检测自家Android客户端在发展中国家的性能表现，Android的产品经理、工程师在2013年的时候去了一趟非洲。当时我看到这个新闻的时候觉得有点怪异，后来看到他们这篇博客才有点理解他们这样做的原因了。

1. [你的Android应用完全不需要那么多的权限](http://greenrobot.me/devpost/i-dont-need-your-permission/)
	
	Android系统的权限从用户的角度来看有时候的确有点让人摸不着头脑。有时候可能你只需要做一些简单的事情（对联系人的信息进行编辑），却申请了远超你应用所需的权限（比如访问所有联系人信息的权限）。

<!--more-->

1. [关于 Android Dex 方法限制的一些总结](http://greenrobot.me/devpost/about-android-dex-method-number-limit/)
	
	在了解这个问题之前我们先要来看看Android 应用编译的过程:1. IDE中的资源打包工具 (Android Asset Packaging Tool ，即图中的aapt) 会将应用中的资源文件进行编译，这些资源文件包括 AndroidManifest.xml文件，为Activity定义的 XML 文件等等。在这个编译过程中也会产生一个 R.java 文件，这样你就可以在你的Java代码中引用这些资源了。

1. [安卓Hacking科普系列](http://bobao.360.cn/learning/detail/122.html)

	本系列科普文章包含：[Part 1: 应用组件攻防](http://bobao.360.cn/learning/detail/122.html)、[Part 2: Content Provider攻防](http://bobao.360.cn/learning/detail/127.html)、[Part 3：Broadcast Receivers攻防](http://bobao.360.cn/learning/detail/126.html)、[Part 4:非预期的信息泄露（边信道信息泄露）](http://bobao.360.cn/learning/detail/133.html)、[Part 5:使用JDB调试Java应用](http://bobao.360.cn/learning/detail/138.html)、[Part 6：调试Android应用](http://bobao.360.cn/learning/detail/140.html)、[Part 7:攻击WebView](http://bobao.360.cn/learning/detail/142.html)、[Part 8:Root的检测和绕过](http://bobao.360.cn/learning/detail/144.html)、[Part9: 不安全的本地存储：Shared Preferences](http://bobao.360.cn/learning/detail/150.html)、[Part 10:不安全的本地存储](http://bobao.360.cn/learning/detail/152.html)等，还在更新中。

### 代码&开源库

1. [Go on Android](https://github.com/golang/mobile)

	The Go mobile repository holds packages and build tools for using Go on Android.

1. [AccountAutoCompleteEditText](https://github.com/KeithYokoma/AccountAutoCompleteEditText)
	
	Just a simple implementation for use of auto complete text view with device account suggestion.
	
1. [SelectableRoundedImageView](https://github.com/pungrue26/SelectableRoundedImageView)
	
	Android ImageView that supports different radiuses on each corner. It also supports oval(and circle) shape and border. This would be especially useful for using inside CardView which should be rounded only top left and top right corners(Don't forget to call setPreventCornerOverlap(false) on your cardview).
	
1. [ObjectLayout](https://github.com/ObjectLayout/ObjectLayout)

	Java classes designed with optimizable object layout in mind 
[http://objectlayout.github.com/ObjectLayout/](http://objectlayout.github.com/ObjectLayout/)。

1. [MvpCleanArchitecture](https://github.com/glomadrian/MvpCleanArchitecture)
	
	A sample project using Clean architecture and MVP in Android。

1. [ViewStateSaveDemo](https://github.com/paveldudka/ViewStateSaveDemo)
	
	Simple Demo of how do you save View's state in Android。

1. [LandscapeVideoCamera](https://github.com/jmolsmobile/LandscapeVideoCamera)

	Powerful custom Android Camera with granular control over the video quality and filesize, restricting recordings to landscape only.

1. [transitions-everywhere](https://github.com/andkulikov/transitions-everywhere)

	Backport of Transitions API from Android KitKat and Lollipop. Compatible with Android 2.2+。

1. [android-proguard-snippets](https://github.com/krschultz/android-proguard-snippets)

	Example Proguard configurations for common Android libraries。
	
### 工具

1. [Android Studio 1.0.2](http://tools.android.com/download/studio/canary/1-0rc4)
	 
	 **墙内下载地址：**[http://www.androiddevtools.cn/#android-studio](http://www.androiddevtools.cn/#android-studio)	 	 

	
### 视频

1. [Android DevBytes](http://v.youku.com/v_show/id_XODUxODEzMDQ4.html?f=23217955)
	
	墙内DevBytes视频更新啦！包括最新的《Android Vector Graphics》（难得有个华裔面孔！）、《Introducing Route 85》（Google面向iOS开发即将推出一系列视频）以及Auto和Wear（有车有表！）

### 设计
	
#### 工具

1. [Material Design Color Palette Generator - Material Palette](http://www.materialpalette.com)

	一个可以快速搭配Material Design主题颜色的并且提供下载的在线网站.

1. [material-design-color-palette-sketch-plugin](https://github.com/t32k/material-design-color-palette-sketch-plugin)
	
	Sketch app plugin for displaying Google material design color palette.
	
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)