---
layout: post
title: "Android开发技术周报 Issue#19"
date: 2015-02-9 15:43:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#19


### 教程

1. [Android开源项目源码解析](http://www.codekk.com/)

	由[@Trinea](https://github.com/Trinea)发起的Android开源项目源码解析项目，目前已校对发布的分析有：Volley源码解析、Android Universal Image Loader源码分析、Dagger源码解析、EventBus 源码解析、xUtils源码解析、ViewPagerindicator源码解析、HoloGraphLibrary源码解析、CircularFloatingActionMenu源码解析、PhotoView 源码解析、Android Lock Pattern源码解析以及公共技术点：Java动态代理、Java注解Annotation、View绘制流程、依赖注入和View时间传递等。

1. [Android最佳性能实践(一)——合理管理内存](http://blog.csdn.net/guolin_blog/article/details/42238627)

	有不少朋友都问过我，怎样才能写出高性能的应用程序，如何避免程序出现OOM，或者当程序内存占用过高的时候该怎么样去排查。确实，一个优秀的应用程序，不仅仅要功能完成得好，性能问题也应该处理得恰到好处。为此，我也是阅读了不少Android官方给出的高性能编程建议，那么从本篇文章开始，我就准备开始写一个全新系列的博文，来把这些建议进行整理和分析，帮助大家能够写出更加出色的应用程序。

1. [深入解析Android的自定义布局](http://android.jobbole.com/80627/)

	这篇文章是前Firefox Android工程师（现在跳槽去Facebook了） [Lucas Rocha](http://lucasr.org/about)所写，文中对Android中常用的四种自定义布局方案进行了很好地分析，并结合这四种Android自定义布局方案所写的示例项目讲解了它们各自的优劣以及四种方案之间的比较。看完这篇文章，也让我对Android 自定义布局有了进一步的了解，于是趁着兴头，我把它翻译成中文，[原文链接在此](http://lucasr.org/2014/05/12/custom-layouts-on-android/)。

1. [巧用Drawable 实现Android UI 元素间距效果](http://android.jobbole.com/80634/)

	在大部分的移动UI或者Web UI都是基于网格概念而设计的。这种网格一般都是有一些对其的方块组成，然后它们组合成为一个块。使用网格这样的设计原则可以有助于对齐UI元素，提升UI的一致性，同时还能让用户更加容易的获取UI上面包含的内容。简而言之，网格是一个相当的强大的设计工具。
		
<!--more-->

1. [模块化的乐趣](http://ifeve.com/fun-modules/)	

	模块间的紧耦合是一种很糟糕的设计，而耦合的最坏表现就是模块间的循环依赖。幸运的是，有几种方法可以用来消除循环依赖，分别是回调函数，代码上移，代码下移。 接下来，我会为大家展示一个小例子。示例中，我会分别使用上述几种技术来消除循环依赖。

1. [你的Android应用完全不需要那么多的权限](http://android.jobbole.com/80630/)	
	Android系统的权限从用户的角度来看有时候的确有点让人摸不着头脑。有时候可能你只需要做一些简单的事情（对联系人的信息进行编辑），却申请了远超你应用所需的权限（比如访问所有联系人信息的权限）。这很难不让用户对你保存戒备。
	
1. [Android App 性能优化实践](http://stackvoid.com/performance-tuning-on-android/)	
	本文从工具、布局优化、代码、View的绘制、电量、和Apk的大小等几个方面记录了Android App优化需要用到的工具和以及在实践中的Tips。
	
1. [MVC，MVP 和 MVVM 的图示](http://www.ruanyifeng.com/blog/2015/02/mvcmvp_mvvm.html)

	复杂的软件必须有清晰合理的架构，否则无法开发和维护。[MVC](http://zh.wikipedia.org/wiki/MVC)（Model-View-Controller）是最常见的软件架构之一，业界有着广泛应用。它本身[很容易理解](http://www.ruanyifeng.com/blog/2007/11/mvc.html)，但是要讲清楚，它与衍生的 MVP 和 MVVM 架构的区别就不容易了。

1. [为Nexus5编译AndroidL固件](http://www.androidperformance.com/build-rom-for-nexus5.html)

	接前一篇文章<[使用Android Studio查看Android Lollipop源码](http://www.androidperformance.com/view-android-source-code-with-androidstudio.html)> , 我们知道,仅仅看代码,提高是比较有限的,而且理解起来也比较肤浅,往往过目就忘. 而自己写过的代码,往往会印象比较深刻,在写的时候也会比较容易理解流程. 所以我们在看代码的同时, 如果能修改代码, 在手机上跑起来并看到修改的效果,这无疑会加快看代码的效率和积极性. 

1. [与Sevice实现双向通信系列](http://www.race604.com/communicate-with-remote-service-1/)
	
	经常有这样的应用场景，我们需要Client端调用Service完成一些事情，Service也可以通过回调通知客户端。
	
1. [使用Gradle发布项目到JCenter仓库](http://zhengxiaopeng.com/2015/02/02/使用Gradle发布项目到JCenter仓库/)	

	这篇文章介绍通过Gradle把开源项目发布到公共仓库JCenter中，方便你我他的事情，我们都是很懒的嘛。JCenter现在是Android Studio中repositories的默认节点了，之前是Maven的，不过JCenter是兼容Maven的，所以放心使用。

### 代码&开源库

1. [Carbon](https://github.com/ZieIony/Carbon)

	Material Design的兼容实现，支持Android 2.1+。

1. [RushOrm](https://github.com/Stuart-campbell/RushOrm)

	一个ORM框架，核心功能：

	* 自定义字段 - 轻松实现定制字段,以便任何对象都可以被序列化到数据库
	* 表关系
		* 一对一
		* 一对多
		* 保存一个父对象会自动保存与之相关关联的子对象
	* 文件 - 轻松的保存长文本, JSON and bitmaps
	* 升级 - 数据库升级支持通过注解去删除和重命名列名。

1. [android-patternview](https://github.com/geftimov/android-patternview)

	图案密码解锁库。
	
	![image](https://github.com/geftimov/android-patternview/raw/master/art/rsz_pattern_correct.png)![image](https://github.com/geftimov/android-patternview/raw/master/art/rsz_mm.png)

1. [gif-movie-view](https://github.com/sbakhtiarov/gif-movie-view)
	
	可以显示Gif动画的自定义View。
	
1. [JavaCPP](https://github.com/bytedeco/javacpp)
	
	JavaCPP provides efficient access to native C++ inside Java, not unlike the way some C/C++ compilers interact with assembly language. No need to invent new languages such as with SWIG, SIP, C++/CLI, Cython, or RPython as required by cppyy. Instead, it exploits the syntactic and semantic similarities between Java and C++. Under the hood, it uses JNI, so it works with all implementations of Java SE, in addition to Android, Avian, and RoboVM (instructions).
	
1. [Genius-Android](https://github.com/qiujuer/Genius-Android)

	Genius-Android 是 Android 中一些常用的的方法集合, Genius 提供6个基本板块：app(Ui)、animation(动画)、widget(Material控件)、command(命令行)］、net tool(Ping、Dns...)、util(常用方法,类)等。

1. [5+ Runtime](https://github.com/dcloudio)

	5+ Runtime是DCloud推出的HTML5强化引擎，性能和功能都大幅领先phoneg*p，可以使用JS调用40W原生API，可以在低端机上流畅运行。点击视频观看低端机上如何流畅运行App。http://download.dcloud.net.cn/FastAndroid-mini.m4v 也可直接下载App在手机上体验：
	
	功能演示：http://dcloud.io/helloh5/
	UI演示：http://dcloud.io/hellomui/

1. [freepager](https://github.com/alexzaitsev/freepager)

	对ViewPager进行了扩展，支持垂直切换page、垂直无限切换page、水平无线切换page和即可以垂直又可以水平无限切换page，支持ndroid 2.1.x (API 7) +系统。
	
	![image](https://raw.githubusercontent.com/alexzaitsev/freepager/master/04.gif)

1. [Android-MaterialPreference](https://github.com/jenzz/Android-MaterialPreference)
	
	一个自定义的，向后兼容的Material Design风格的Preference实现。
	
	![image](https://camo.githubusercontent.com/e7d19d635dd16b8559b1f9c1982ca47ee55ddbe1/68747470733a2f2f7261772e6769746875622e636f6d2f6a656e7a7a2f416e64726f69642d4d6174657269616c507265666572656e63652f6d61737465722f6173736574732f53637265656e73686f74312e706e67)

1. [CollapseOnScroll](https://github.com/KlassenKonstantin/CollapseOnScroll)

	模仿Android Lollipop Contacts滚动效果的容器View。

1. [AndroidEventBus](https://github.com/bboyfeiyu/AndroidEventBus)

	一个Android平台的事件总线框架, 它简化了Activity、Fragment、Service等组件之间的交互，很大程度上降低了它们之间的耦合，使得我们的代码更加简洁，耦合性更低，提升我们的代码质量。
	
	![image](https://camo.githubusercontent.com/1ba8becec515613cd83aa6b0273c67b058d0b6ab/687474703a2f2f696d672e626c6f672e6373646e2e6e65742f3230313530323033313235353038313130)
	
### 工具	 

1. [Android Studio 1.1 Beta 4](http://www.androiddevtools.cn)

	添加了对单元测试的支持以及修复了一些Bug。

1. [gradle-eclipse-aar-plugin](https://github.com/ksoichiro/gradle-eclipse-aar-plugin)	
	一个可以让你在Eclipse中使用Android AAR格式库的Gradle插件。

1. [Codota](https://www.codota.com)	

	一个代码片段搜索工具。

### 视频

1. [细说多线程之Thread VS Runnable](http://www.imooc.com/view/312?from=itblog)

	本课程带领大家更加深入地学习Java多线程机制，深入理解创建线程的两种方式之间的差异，掌握线程的生命周期和守护线程的概念。

1. [千变万化的ViewPager切换动画](http://www.imooc.com/view/226?from=itblog)

	本课程将带领大家实现个性的ViewPager切换动画，首先介绍通过PageTransformer结合ViewPager.setPageTransformer来实现动画效果，然后教大家如何让其兼容到3.0以后，其中会涉及到属性动画等知识点；最后将介绍通过自定义ViewPager的方式来实现动画切换效果。

1. [android应用卡顿优化实践-何杰](http://v.youku.com/v_show/id_XODg1NTE5MjAw.html)

	Android应用的卡顿问题非常突出，所有用户都能感觉得到却又很难做量化卡顿的严重程度，过去的做法只是零星地发现和解决一些小点。DAU超亿级的UC浏览器在卡顿优化的过程中建立了一套衡量卡顿严重性的数据指标与监控分析机制，并藉此有针对性地落实了200+个性能优化点。这里会介绍卡顿监控与分析的方法、常见的卡顿案例与原因

		
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)!