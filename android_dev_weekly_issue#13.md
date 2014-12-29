---
layout: post
title: "Android开发周报 Issue#13"
date: 2014-12-29 10:18:59 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发周报 Issue#13

### 新闻
1. [Oracle开始从Java运行时中移除JAR包](http://www.infoq.com/cn/news/2014/12/oracle-java-jar-package)

	早在2012年8月，在Java平台首席架构师Mark Reinhold宣布[模块化项目Jigsaw](http://openjdk.java.net/projects/jigsaw/)之后不久，[JEP 162](http://openjdk.java.net/jeps/162)这一题为“准备模块化”的提案就指出，在Jigsaw项目中为模块化系统开发的代码不会集成到JDK 8中。那次延期直接将模块化支持推迟到JDK 9，最早也得到2016年。

1. [android5.0让位，Android 6.0曝光这是神马情况？](http://www.eoeandroid.com/thread-558758-1-1.html)
	
	　Android 5.0刚和我们见面没多久，下一代操作系统Android 6.0就曝光了。外媒报道称，谷歌另一个开发小组已经着手进行一款代号为“M”的系统的研发工作，而这个“M”很有可能就是Android 6.0的代号。据猜测，Android 6.0最主要的变化将会是优化车载表现，可直接安装在汽车当中，这样用户无需智能手机即可直接控制汽车。
	
### 教程

1. [将Eclipse代码导入到AndroidStudio的两种方式](http://www.cnblogs.com/ct2011/p/4183553.html)

	说到使用AndroidStudio，除了新建的项目，我们都会面临的问题是原先Eclipse的代码该怎么导入到AndroidStudio中使用。Google为了让我们更加方便的使用AndroidStudio，提供了两种导入Eclipse代码的方式：一种兼容Eclipse，一种是全新的Android Gradle Project.

1. [Java 注解指导手册 – 终极向导](http://www.importnew.com/14227.html)

	在这篇文章中我们将阐述什么是Java注解，它们如何工作，怎么使用它们。我们将揭开Java注解的面纱，包括内建注解或称元注解，还将讨论Java8中与之相关的的新特性。最后，我们将实现自定义的注解，编写一个使用注解的处理程序（消费器），它通过java反射使用注解。
	
1. [缓存、缓存算法和缓存框架简介](http://blog.jobbole.com/30940/)

	我们都听过 cache，当你问他们是什么是缓存的时候，他们会给你一个完美的答案，可是他们不知道缓存是怎么构建的，或者没有告诉你应该采用什么标准去选择缓存框架。在这篇文章，我们会去讨论缓存，缓存算法，缓存框架以及哪个缓存框架会更好。

<!--more-->

1. [手机QQ的移动化实践之路](http://www.infoq.com/cn/news/2014/12/qq-mobile-practice)

	手机QQ的移动化实践之路】在刚刚结束的AS北京上，腾讯即时通讯平台部技术总监范瑞彬做了题为《手机QQ的移动化实践之路》的演讲，从移动环境的特点、如何做好接入、架构设计理念三个方面分享了手Q一路走来的诸多经验。演讲PPT下载：[http://pan.baidu.com/s/1mgIDMtU](http://pan.baidu.com/s/1mgIDMtU)

1. [手机淘宝构架演化实践](http://www.infoq.com/cn/news/2014/12/taobao-app-evolution)
	
	阿里心石：手机淘宝构架演化实践】在本届ArchSummit中，来自阿里无线事业部的高级专家李敏（花名心石 @allblue_华丽地低调 ）与我们分享了《手机淘宝架构演化实践》，畅谈阿里巴巴无线从开始之初到成为日活上亿级别电商应用技术变迁和积累。演讲PPT下载：[http://pan.baidu.com/s/1kTgMfMv](http://pan.baidu.com/s/1kTgMfMv)
	
1. [Gradle 学习专辑](http://www.testerhome.com/topics/1718)
	
	该学习专辑包含：gradle 初步构建（一）、Java Project Gradle Emma、Android Project Gradle jacoco、Android Gradle Espresso tests、自由的使用 gradle 构建你的应用、Groovy 初探（一）、gradle 集成修改 Android Manifest.xml 打多个包实践和Gradle 编译交互小技巧等，并且还在持续更新中。
	
1. [代码规范和Android项目中的一些可用工具](http://tech.glowing.com/cn/dai-ma-gui-fan-he-androidxiang-mu-zhong-de-xie-ke-yong-gong-ju/)

	这里主要讲一下关于代码规范的相关问题，和在Android项目中如何利用一些工具进行规范和检查。代码规范不是一个Android项目特有的问题，所以前部分内容是不单针对Android的。

1. [Android Studio系列教程四--Gradle基础](http://stormzhang.gitcafe.com/devtools/2014/12/18/android-studio-tutorial4/)

	[googdev](http://weibo.com/zhangqi8)结合Stduio 1.0正式版与最新的Gradle语法通过自己的开源项目 [9GAG](https://github.com/stormzhang/9GAG) 讲解了Gradle相关的知识，后续会介绍一种我常用的快速方便的编译查看第三方开源项目的方法，如何导入Android Studio，Gradle常用基本命令，多渠道打包配置等。

1. [每个程序员至少阅读两次的 10 篇技术论文](http://top.jobbole.com/17733/)

	 这10篇论文包括：编程语言中的基本概念、为什么函数式编程重要、计算机编程的公理基础、分布式系统中的时间、时钟和事件顺序、理解类型、数据抽象和多态、符号表达式的递归函数，及其机器计算等。

### 代码&开源库

1. [MaterialRangeBar](https://github.com/oli107/material-range-bar)

	Android widget for selecting a range of values.
	
1. [SVG2Drawable](https://github.com/StanKocken/SVG2Drawable)
	
	Use a jar executable to create a Drawable class to display a SVG on Android.
	
1. [gradle-robojava-plugin](https://github.com/kageiit/gradle-robojava-plugin)

	Gradle plugin to integrate Robolectric tests into Android Studio。
	
1. [AndroidLocalizationer](https://github.com/westlinkin/AndroidLocalizationer)

	This is a Android Studio/ IntelliJ IDEA plugin to localize your Android app, translate your string resources automactically. [https://plugins.jetbrains.com/plugin/7629](https://plugins.jetbrains.com/plugin/7629)

1. [MrVector](https://github.com/telly/MrVector)

	AKA VectorDrawableCompat: A 14+ backport of VectorDrawable.

1. [HelloMultidex](https://github.com/frogermcs/HelloMultidex)

	Example project for multi-dex project in Android.

1. [gesture-imageview](https://github.com/jasonpolites/gesture-imageview)
	
	Implements pinch-zoom, rotate, pan as an ImageView for Android 2.1+.
	
1. [slidingtabs](https://github.com/nispok/slidingtabs)

	Gradle port of Google's SlidingTabLayout to display a custom ViewPager title strip.

1. [SuperRecyclerView](https://github.com/Malinskiy/SuperRecyclerView)

	Pumped up RecyclerView.This is an attempt to make RecyclerView easier to use.

	Features built in:

	* ProgressBar while adapter hasn't been set
	* EmptyView if adapter is empty
	* SwipeRefreshLayout (Google's one)
	* Infinite scrolling, when you reach the X last item, load more of them.
	* Swipe To Dismiss
	* Sticky headers (via [Eowise](https://github.com/eowise/recyclerview-stickyheaders), see sample)

1. [CurtainView](https://github.com/aicaprio/CurtainView)

	An android view,which can layer on any gravity for swiping.
	
### 工具	 	 

1. 国内几个Android SDK镜像
	
	大连东软信息学院镜像服务器的地址: `http://mirrors.neusoft.edu.cn` 端口：80

   	北京化工大学镜像服务器的地址: 
   	1. IPv4: `http://ubuntu.buct.edu.cn/` 端口：80
   	2. IPv4: `http://ubuntu.buct.cn/`   端口：80
   	3. IPv6: `http://ubuntu.buct6.edu.cn/`  端口：80
	
	上海GDG镜像服务器地址:`http://sdk.gdgshanghai.com `  端口：8000

	**使用方法**：
	
	1. 启动 Android SDK Manager ，打开主界面，依次选择『**Tools**』、『**Options...**』，弹出『**Android SDK Manager - Settings**』窗口；
	2. 在『**Android SDK Manager - Settings**』窗口中，在『**HTTP Proxy Server」和「HTTP Proxy Port**』输入框内填入上面镜像服务器地址和端口，并且选中『**Force https://... sources to be fetched using http://...**』复选框。设置完成后单击『**Close**』按钮关闭『**Android SDK Manager - Settings**』窗口返回到主界面；
	3. 依次选择『**Packages**』、『**Reload**』。

1. [gradle-packer-plugin Android 多渠道打包工具](https://github.com/mcxiaoke/gradle-packer-plugin)

	gradle-packer-plugin 是Android多渠道打包工具Gradle插件，可方便的于自动化构建系统集成，通过很少的配置可实现如下功能 ：

	* 支持自动替换AndroidManifest文件中的meta-data字段实现多渠道打包
	* 支持自定义多渠道打包输出的存放目录和最终APK文件名
	* 支持自动修改versionName中的build版本号，实现版本号自动增长
	
1. [Gitter.im](https://gitter.im)

	Chat, for GitHub.

	![image](http://ww4.sinaimg.cn/bmiddle/005GSHYzjw1eniqp77z75j31kw0w74ii.jpg)
	
### 视频

1. [阿里技术沙龙第十六期《android插件化及动态部署—ATLAS 》伯奎](http://v.youku.com/v_show/id_XNTMzMjYzMzM2.html)

### 设计
	
### 教程

1. [Sketch 制作扁平图标](http://zhuanlan.zhihu.com/rijing/19845226)
	
	用Sketch一步一步教你制作扁平图标，步骤很详细
	
1. [动效软件 Form 教程：概览与基础 patch 介绍](http://leonpd.lofter.com/post/20f397_4cb74d1)
	
	都说产品设计师的设计可以用 Axure + Sketch + Origami三者联动，完成原型、视觉和动效的一条龙工作，前一段时间也抽空学习了一下 Quartz Composer（以下简称 QC） + Origami，虽然有一定的上手难度，但是确实能够做出非常逼真的效果。
	
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)