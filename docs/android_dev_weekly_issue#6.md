---
layout: post
title: "Android开发周报 Issue#6"
date: 2014-11-10 16:45:18 +0800
comments: true
categories: AndroidDevWeekly 
---

#Android开发周报 Issue#6

### 新闻

1. [Android 5.0 Lollipop源代码发布](http://linux.cn/article-4172-1.html)

	Google将最新的Android 5.0 Lollipop系统源代码上传在公开的[Android Open Source Project(AOSP) 库](	http://source.android.com/source/index.html)。
	
1. [Android 5.0 Lollipop 安全特性详解](http://linux.cn/article-4168-1.html)

	Android 5.0 Lollipop 正式版发布在即，根据 Google 的说法，Android 5.0 是 Android 历史上最为重大的版本变更，带来了全新的设计风格，全新的软件运行环境，更好的续航能力以及大量的细节改进。可能关于 Material Design、ART 模式等等新特性你已经有所了解，但是我们今天要聊的是 5.0 的另一个重大变革，关于安全性的改进。

1. [Copresence: Google 正为 iOS 和 Android 之间数据通讯架设的桥梁](http://www.pingwest.com/copresence-is-airdrop-between-android-ios/)

	Google 最近被人发现正在开发的名为「Copresence」的功能，未来很有可能成为跨移动操作系统数据传输的最好解决方案。Copresence 的功能将允许 Android 和 iOS 操作系统设备之间互相传输文件、照片、发送导航定位、文字信息等多种类型的数据——并非通过互联网，而是更加本地化的点对点连接方式。
	
### 文章

1. [在Android上创建卡片式UI](https://github.com/AWCNTT/ArticleTranslateProject/blob/master/translated/Issue%23105/2014-11-06-Creating-a-Cards-UI-on-Android.md)

	自从卡片式UI第一次在Google+ app上亮相，这种设计模式在Android社区上开始变得越来越火。很多人都热衷于这种设计模式并在他们的开发中使用。这不只归功于其时尚的外观，还有它实用之处。每张卡片拥有其相关的内容及其内容所触发的动作。换句话来说，每张卡片有它唯一的内容管理机制。

1. [34个Android常用adb shell命令汇总](http://www.codeceo.com/article/android-adb-shell.html)

	调试Android程序有时需要adb shell 命令，adb全称Android Debug Bridge ，就是起到调试桥的作用。通过adb我们可以在Eclipse中通过DDMS来调试Android程序，说白了就是debug工具。adb通过监听Socket TCP 5554等端口让IDE和Qemu通讯。

1. [ 使用Gradle构建Android项目](http://blog.csdn.net/isming/article/details/26985317)

	Gradle是以Groovy为基础，面向java应用，基于DSL语法的自动化构建工具。是google引入，替换ant和maven的新工具，其依赖兼容maven和ivy。使用gradle的目的:更容易重用资源和代码；可以更容易创建不同的版本的程序，多个类型的apk包；更容易配置，扩展;更好的IDE集成;

1. [适配多屏幕的最佳实践](http://toughcoder.net/blog/2014/10/26/best-practices-to-support-multiple-screen/)

	对于Android应用开发来讲，比较头疼的，也是比较重要的一个工作就是要尽可能多的支持市场上的Android设备，由于Android的开放性，各种奇奇怪怪的设备都有，符合标准的，不符合标准的，行货，水货，山寨货鱼龙混杂，防不胜防。

1. [如何有效的减少重复的代码](http://toughcoder.net/blog/2014/10/25/tricks-to-remove-duplicates/)

	重复的代码一直都是可维护性的大敌，重构的重要任务之一也就是要去除掉重复的代码，有效的减少重复代码，可以大大提高软件的扩展性。

1. [在android中画圆形图片的几种办法](http://blog.csdn.net/isming/article/details/39404407)	
	在开发中经常会有一些需求,比如显示头像，显示一些特殊的需求,将图片显示成圆角或者圆形或者其他的一些形状。但是往往我们手上的图片或者从服务器获取到的图片都是方形的。这时候就需要我们自己进行处理，将图片处理成所需要的形状。

<!--more-->


### 代码&开源库

1. [MultiActionTextView](https://github.com/ajaysahani/MultiActionTextView)

	MultiActionTextView 一个textview的开源库，可以分别给TextView中的某几个字设置点击事件。

1. [UltimateAndroid](https://github.com/cymcsg/UltimateAndroid)

	快速开发Android应用的框架，框架目前主要包含的功能有View Injection,ORM,异步网络请求和图片加载，自动化脚本测试,磁盘LRU等功能.同时提供了类似于TripleDes、Webview快速设置、Md5处理、String处理,Https处理等常用工具类，还有超过100多种UI控件效果。

1. [DebugLog](https://github.com/MustafaFerhan/DebugLog)

	DebugLog可以帮你创建更简单和更容易理解的调试日志，能够友好的显示调试信息所在类和函数。

1. [MaterialEditText](https://github.com/rengwuxian/MaterialEditText)

	Material Design风格的EditText。虽然AppCompat v21中也提供了 Material Design 的控件外观支持，其中包括 EditText 。但 AppCompat 中的 EditText 实在有点难用，因为它是通过 colorAccent 来自动为控件着色的，并没有提供设置颜色的api，因此需要通过为控件定制theme的方式来实现自定义控件颜色。 另外，除了外观上的变化， AppCompat 没有提供任何 Google Material Design Spec 中提到的特性。  


### 视频

1. [GoogleFit APIs for Android](http://v.youku.com/v_show/id_XODE5NDI1MTI4.html)

	来自Google美女工程师的DevBytes系列《GoogleFit APIs for Android》视频共两集,现已搬至优酷，关注Google Fit的可以看内容，不感兴趣内容可以看美女，程序猿们我懂你们的！！！

### 工具

1. [material-design-icons-adt-template](https://github.com/intrications/material-design-icons-adt-template)

	Android Studio / Eclipse ADT template for including icon resources from [https://github.com/google/material-design-icons](https://github.com/google/material-design-icons) in your project.

1. [Android Studio 0.9.2 Released](http://tools.android.com/download/studio/canary)

	Android Studio 0.9.1 released to the canary channel! 

### 书

1. [Pro Android Apps Performance Optimization](http://it-ebooks.info/book/646/)

	Today's Android apps developers are often running into the need to refine, improve and optimize their apps performances. As more complex apps can be created, it is even more important for developers to deal with this critical issue. 

### 设计

#### 文章

1. [熊氏切图法--一键导出App icon](http://www.ui.cn/project.php?id=30796)

	做App设计的小伙伴有没有遇到这种情况呢，同一个icon要输出N种尺寸，用传统的方法批处理调整图片大小比较繁琐，不方便同时整体预览，如果后续修改了设计，又要重复一次这个批处理的过程，有没有一键输出所有尺寸的方法呢？本熊这就给大家推荐一种强大的技巧：智能对象+生成图像资源，是的，本熊不要脸的将其命名为“熊氏切图法”.

1. [UE+UI设计流程之一二三](http://www.ui.cn/project.php?id=30921)

	在做移动端app的设计过程中，经常会碰到一些二次返工或者时间的浪费，在这里分享下自己在项目中的流程经验，供遇到问题的小伙伴们参考。

1. [从Material UI得到的设计感悟](http://www.ui.cn/project.php?id=30538)

	如果你读过Google的Material设计文档，你就会发现其对细节和深度的注重。在文档中你能学到很多东西。其中最为重要的一项，就是其证明了编写复杂视觉风格指南是完全可能的。尽管可能困难重重，但还是可能的。特别是对于Google复杂多样的产品组合来说。

1. [APP规范实例(详细的UI设计方法](http://www.ui.cn/project.php?id=30540)

	设计是无限的，可作为借鉴，这一套UI设计规范，包含了界面布局、颜色、文字规范、按钮规范、图标规范、图片规范、列表规范、控件规范、弹出浮层，超级详细。大家可以借鉴下，学会自己设计一套APP设计规范，成为高级设计师。但是不要生搬硬套，毕竟不是一个产品，总之可参考的价值很高。


#### 工具&资源

1. [Size-Marks-PS](https://github.com/romashamin/Size-Marks-PS)

	Photoshop Javascript插件，可以以新建图层的方式直接在PS中标注尺寸。
	
	![image](http://ww1.sinaimg.cn/mw1024/4b4d632fgw1elyr9qvsipg20kf08jdjf.gif)
	

1. [高效神器！21款强大实用的PHOTOSHOP扩展插件](http://www.uisdc.com/21-photoshop-plugins-for-designer)
	
	21款扩展插件，特别适合网页设计师。这些神器可以让平时复杂繁琐的操作变得更加简单.
	
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)