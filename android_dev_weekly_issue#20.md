---
layout: post
title: "Android开发技术周报 Issue#20"
date: 2015-02-18 09:03:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#20

### 新闻

1. [Xposed Framework for Android Lollipop is Here!](http://www.xda-developers.com/xposed-framework-for-android-lollipop-is-here/)

	Xposed框架是一款可以在不修改APK的情况下影响程序运行（修改系统）的框架服务，基于它可以制作出许多功能强大的模块，且在功能不冲突的情况下同时运作。

### 教程

1. [用 RecyclerView 实现『贝壳单词』英语角的 Quick Return 效果](http://drakeet.me/quick-return-like-as-seashell)

	今天把『贝壳单词』中英语角的 quick return 效果剥离出来写了个 Demo，讲解使用 RecyclerView 和 nineoldandroids 自己动手写快速返回菜单。通过这篇文章你将了解到的知识有：1.RecyclerView 和其适配器的基本使用
RV、2.适配多种 Item View 类型写法、3.mRecyclerView.setOnScrollListener()、4.nineoldandroids 这个强大 View 操作库的使用等。

1. [开源项目Philm的MVP架构分析](http://www.lightskystreet.com/2015/02/10/philm_mvp/)

	最近一直在研究ChrisBannes的开源项目[Philm](https://github.com/chrisbanes/philm)，其整体架构是一套MVP的实现，因为自己也确实没有遇到过整个项目利用MVP搭建的架构，看到的更多是一些代码片段，这里就探讨Philm是如何结合Android实际问题来实现一种MVP架构，如有分析不准确的地方，欢迎指出，大家一起探讨。

1. [Gradle 修改 Maven 仓库地址](http://www.yrom.net/blog/2015/02/07/change-gradle-maven-repo-url/)

	近来迁移了一些项目到Android Studio，采用Gradle构建确实比原来的Ant方便许多。但是编译时下载依赖的网速又着实令人蛋疼不已。如果能切换到国内的Maven镜像仓库，如开源中国的Maven库，又或者是换成自建的Maven私服，那想必是极好的。

1. [为什么我们可以在非UI线程中更新UI](http://blog.csdn.net/aigestudio/article/details/43449123)

	看到这样的标题...估计N多人会说我是逗比…因为很多盆友在学习Android（特别是从4.0之后开始入门的）的时候都会常看见或听到别人说我们更新UI呢要在UI线程（或者说主线程）中去更新UI，不要在子线程中更新UI，而Android官方呢也建议我们不要在非UI线程直接更新UI，为什么呢?

1. [Guava 是个风火轮之基础工具(1)](http://ifeve.com/guava-base-1/)

	Guava 是 Java 开发者的好朋友。虽然我在开发中使用 Guava 很长时间了，Guava API 的身影遍及我写的生产代码的每个角落，但是我用到的功能只是 Guava 的功能集中一个少的可怜的真子集，更别说我一直没有时间认真的去挖掘 Guava 的功能，没有时间去学习 Guava 的实现。

1. [Android最佳性能实践(二)—分析内存的使用情况](http://blog.csdn.net/guolin_blog/article/details/42238633)

	由于Android是为移动设备开发的操作系统，我们在开发应用程序的时候应当始终把内存问题充分考虑在内。虽然Android系统拥有垃圾自动回收机制，但这并不意味着我们就可以完全忽略何时去分配或释放内存。即使我们全部按照上一篇文章中给出的编程建议来去编写程序，还是会很有可能出现内存泄露或其它类型的内存问题。所以，唯一能够解决问题的办法，就是尝试去分析应用程序的内存使用情况，那么本篇文章就会教大家如何进行分析。

1. [Android 主线程之旅—PSVM](http://android.jobbole.com/80636/)

	当碰到与Android主线程交互相关的Bug时，我决定好好去看看Android的主线程究竟是怎么一回事。这篇文章就是描述我的Android主线程之旅的第一部分。

1. [Java注解处理器](http://www.race604.com/annotation-processing/)
	
	Java中的注解(Annotation)是一个很神奇的东西，特别现在有很多Android库都是使用注解的方式来实现的。在这篇文章中，我将阐述怎样写一个注解处理器(Annotation Porcessor)。在这篇教程中，首先，我将向您解释什么是注解器，你可以利用这个强大的工具做什么以及不能做什么；然后，我将一步一步实现一个简单的注解器。
		
<!--more-->

1. [在 x86 上优化 Android 应用的方法和技巧](http://www.eoeandroid.com/thread-557380-1-1.html)

	英特尔致力于帮助开发人员提供能够在英特尔架构上正常运行（甚至出色运行）的 Android 应用。 虽然英特尔主要致力于社区层面：优化 Dalvik Java、V8 引擎和 Bionic C；丰富代码库；为 IA 提供采用 32 位和 64 位内核的版本，他们同样提供了多种类型的新工具为 Android 开发人员提供帮助。 这些工具主要用于提高性能，使其超过面向 x86 的默认 ARM 转换层：libhoudini 所提供的性能。 

### 代码&开源库

1. [KugouLayout](https://github.com/zhaozhentao/KugouLayout)

	一个模仿酷狗播放器滑动返回的layout，可以让你的app有更丰富便捷的手势操作，支持activity滑动返回和普通layout的滑动显示/隐藏两种模式。
	
	![image](https://raw.githubusercontent.com/zhaozhentao/KugouLayout/master/screenshot/screen2.gif)

1. [labelview](https://github.com/linger1216/labelview)

	贴纸效果。
	
	![image](https://raw.githubusercontent.com/linger1216/labelview/master/img/img2.png)	
<!--	![image](https://github.com/linger1216/labelview/raw/master/img/img1.png)-->

1. [AndroidTagGroup](https://github.com/2dxgujun/AndroidTagGroup/)

	一个漂亮的标签组控件。
	
	![image](https://camo.githubusercontent.com/6a4ce346d402597d71f3e523c4a404311a4cd25b/68747470733a2f2f7261772e6769746875622e636f6d2f32647867756a756e2f416e64726f696454616747726f75702f6d61737465722f6173736574732f64656d6f5f73637265656e73686f742e706e67)
	

1. [drozer](https://github.com/mwrlabs/drozer)

	一个Android安全测试框架。

1. [Lynx](https://github.com/pedrovgs/Lynx)

	一个可以创建一个自定义View并显示所有日志信息的库。
	
	![image](https://raw.githubusercontent.com/pedrovgs/Lynx/master/art/screenshot_demo_1.gif)

1. [Android-Ultra-Photo-Selector](https://github.com/AizazAZ/Android-Ultra-Photo-Selector)

	一个图片选择器控件，支持选择多张图片、浏览设备上所有包含图片的文件夹、预览选择的图片并且支持缩放。
	
	![image](https://raw.githubusercontent.com/AizazAZ/Android-Ultra-Photo-Selector/master/media/image1.png)
	
1. [fab](https://github.com/shell-software/fab)

	一个支持很多自定义属性的Floating Action Button控件。
	
	![image](https://github.com/shell-software/fab/raw/master/demo/button_type_default.png)

1. [EasyMVP](https://github.com/JorgeCastilloPrz/EasyMVP)

	Linkedin工程师做的一个mvp示例demo.
	
	![image](https://raw.githubusercontent.com/JorgeCastilloPrz/EasyMVP/master/art/screenshot_1.png)
	
1. [IconButton](https://github.com/pnc/IconButton)

	一个Button的子类，支持更好控制over drawable位置的功能。
	
	<!--![image](https://raw.githubusercontent.com/pnc/IconButton/master/images/demo.png)-->

1. [MaterialLoadingProgressBar](https://github.com/lsjwzh/MaterialLoadingProgressBar)

	抽取的support-v4 v21 中的loading圈效果。

	![image](https://raw.githubusercontent.com/lsjwzh/MaterialLoadingProgressBar/master/screen.gif)

1. [ElasticScrollView](https://github.com/Kitdroid/ElasticScrollView)

	带回弹效果的ScrollView。
	
	![image](https://raw.githubusercontent.com/Kitdroid/ElasticScrollView/master/image/elastic_sample.gif)

1. [android-resources](https://github.com/Tikitoo/android-resources)

	Android 开发资料收集汇总。

1. [dashed-circular-progress](https://github.com/glomadrian/dashed-circular-progress)

	圆形轨迹进度条控件。
	
	![image](https://raw.githubusercontent.com/glomadrian/dashed-circular-progress/master/art/sample.gif)

1. [AutoCompleteBubbleText](https://github.com/FrederickRider/AutoCompleteBubbleText)	
	
	 
	![image](https://raw.githubusercontent.com/FrederickRider/AutoCompleteBubbleText/master/images/Screenshot_1.png)

1. [DrawableView](https://github.com/PaNaVTEC/DrawableView)

	支持手写绘画的自定View，并且可以将绘画的结果保存为图片。
	
	![image](https://raw.githubusercontent.com/PaNaVTEC/DrawableView/master/art/DrawableView.gif)
	
1. [anytextview](https://github.com/hanspeide/anytextview)
	
	对TextView、EditText和Button进行了扩展，可以支持非系统字体。
	
### 工具	 

1. [Android Studio 1.1 RC1](http://www.androiddevtools.cn)

	修复了一些Bug。

1. [JitPack.io](https://jitpacio)

　　JitPack根据需要构建GitHub项目并提供现成的软件包，方便你在Gradle,Maven和Sbt项目中使用包库。

1. [GerritHub](http://gerrithub.io)

	Github仓库代码Review工具。

### 视频

1. [Android面试常客Handler详解](http://www.imooc.com/view/267?from=itblog)

	本课程将深入理解Android的Handler机制，并结合源码实例，讲解Looper、MessageqQueue、Handler之间的关系，同时介绍HandlerThread的原理和使用，并分析Handler在开发中遇到的异常的原因，最后从源码的角度分析一下Handler更新UI的流程。

1. [Android自定义任意层级树形控件](http://www.imooc.com/view/303)

	本课程将带领大家通过ListView打造一个任意层级的树形控件，大家可以学到巧妙的设计思想以及数据结构的知识。课程中也包含如何巧妙的利用反射加注解将设计通用化，同时可以进一步加深对ListView适配器的理解.

### 设计

1. [Twitter视频功能设计流程全程剖析](http://www.ui.cn/project.php?id=41420)
	
	在这7000字文章中，Twitter设计师展示了严谨的设计流程 以及 设计开发协作心得。Twitter设计流程值得学习的几点：1.原型设计驱动设计方向，可交互、便于测试、确定开发可行性。2.注重设计与开发的沟通，将很多设计师来做更好的开发工作转移给设计师，项目跟进扎实，与其在AE中死抠“设计”细节，不如简单制作大致原型，尽早协助开发调节效果，制作“产品”3.精雕细琢，750+静态设计变种，54份原型可见细心程度。4.问题汇总，bug发现，用户测试并非与设计师无关。5.任何棘手的实现问题，多揪着开发问，很多小发现影响却很大。

1. [四个不为人知的PHOTOSHOP高效操作秘籍（二）](http://www.uisdc.com/photoshop-efficient-operation-skills-2)
	
	首先花一小段文字来重申下 mac 和 win 的快捷键问题。两个操作系统下的 PS 是一样的，只不过 mac 下的快捷键 Command 在 win 下换成了 Ctrl，Option 换成了 Alt ，其他是没有区别的。本文所提的技巧对两个平台都是通用的！
			
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)