---
layout: post
title: "Android开发周报 Issue#10"
date: 2014-12-08 11:10:12 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发周报 Issue#10
	
### 文章

1. [Android Apk 拆分机制](http://blog.csdn.net/maosidiaoxian/article/details/41692535)

	拆分机制比起使用 flavors，能让应用程序更有效地构建一些形式的多个apk。多 apk 只支持以下类型: 1.
屏幕密度 2.ABI.使用新的拆分机制，构建同一个应用程序的hdpi版本和mdpi版本，能够共享很多的任务 （如 javac，dx，proguard）。此外，它会被认为是一个单一的variant，并且同一个测试程序将会被用来测试每​​个多APK。

1. [使用manifestPlaceholders](http://relex.me/using-manifestplaceholders/)

	在项目中我需要打包不同渠道的APK，需要在AndroidManifest中定义渠道名称，以便在java中调用。以前ant或gradle打包时动态改变渠道的思路是：正则AndroidManifest的特定字符然后替换.

1. [Property Anim详解](http://blog.csdn.net/xushuaic/article/details/40424379)

	本篇文章将对PropertyAnimation进行全面深入的探讨，本篇文章可以分为两大块，从第六部分可以作为分界点。前五部分着重讲解了PropertyAnim的动画值的计算过程，ValueAnimator与ObjectAnimator以及TimeInterpolation与TypeEvaluator之间的介绍和比较，这几点是比较重要的，从第六部分开始是通过源码的角度分析了整个动画计算以及内部的处理细节，以及引出了对JakeWharton大神的NineOldAndroids 开源库的分析，如果你觉得太多，可以分开来看，有理解不准确的地方，欢迎大家指正。

<!--more-->

1. [Android Studio系列教程](http://stormzhang.com/posts.html#AndroidStudio)

	相信大家对Android Studio已经不陌生了，Android Studio是Google于2013 I/O大会针对Android开发推出的新的开发工具，目前很多开源项目都已经在采用，Google的更新速度也很快，明显能感觉到这是Android开发的未来，那么我们还有什么理由不去拥抱未来呢？虽然推出了很久，但是国内貌似普及的程度并不高，鉴于很多朋友求studio的详细教程，那么今天我就手把手教大家下载、安装、使用，Studio之路从这里开始。

1. [Dalvik虚拟机Java堆创建过程分析](http://blog.csdn.net/luoshengyang/article/details/41581063)

	 使用C/C++开发应用程序最令头痛的问题就是内存管理。慎不留神，要么内存泄漏，要么内存破坏。虚拟机要解决的问题之一就是帮助应用程序自动分配和释放内存。为了达到这个目的，虚拟机在启动的时候向操作系统申请一大块内存当作对象堆。之后当应用程序创建对象时，虚拟机就会在堆上分配合适的内存块。而当对象不再使用时，虚拟机就会将它占用的内存块归还给堆。Dalvik虚拟机也不例外，本文就分析它的Java堆创建过程。


### 代码&开源库

1. [Google Samples](https://github.com/googlesamples)
	
	Google在Github上发布了大量Demo，针对不同的特性，也包含了最新的API 21 (Lollipop),学习的好资料/

1. [MatchView](https://github.com/Rogero0o/MatchView)

	TextView中的文字由类似火柴棍分散组合的效果。
	
	![image](https://camo.githubusercontent.com/a71e9d26a7f90ea70270b3681d99785a29f83be5/687474703a2f2f7777312e73696e61696d672e636e2f6d773639302f6136393561636465677731656d79746e6b347334356732306567306d6b3439302e676966)

1. [Wally](https://github.com/Musenkishi/wally)

	Wally is a fast and efficient open source wallpaper application for Android.

1. [FolderLayout](https://github.com/kyze8439690/FolderLayout)

	A layout like a stack of files and you can choose one to open. Just imitate the UI of Tencent's QQ手机管家.

1. [android-material-icons](https://github.com/Malinskiy/android-material-icons)

	一个让你方便的在Android开发中使用Google发布出来的Material Design风格图标的库。	
1. [BabushkaText](https://github.com/quiqueqs/BabushkaText)

	A simpler way to style your TextViews
	
	![image](https://github.com/quiqueqs/BabushkaText/raw/master/images/example.png)
	
### 工具

1. [Google 技术资源离线版](http://www.chinagdg.com/thread-6053-1-1.html)

	 Google 发布了一套4张 DVD，将 Google Developers 上的在线技术文档和视频打包到离线文件中。内容很丰富，如 Android 官方文档和SDK、Google Cloud 文档和视频、Web Fundamentals 文档、I/O 大会和 Dev Bytes 视频、Google Udacity 课程视频 等等。

1. [Android Studio 1.0 Release Candidate 4](http://tools.android.com/download/studio/canary/1-0rc4)
	 
	 **墙内下载地址：**[http://www.androiddevtools.cn/#android-studio](http://www.androiddevtools.cn/#android-studio)

### 设计

#### 文章

1. [中国移动应用设计趋势解读](http://www.ui.cn/project.php?id=33849)

	铺天盖地的二维码、丧心病狂的小红点，还有繁花似锦的安卓ROMs...

	——老外对中国式App设计趋势的分析  by  Dan Grover (微信产品经理) 
	
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)