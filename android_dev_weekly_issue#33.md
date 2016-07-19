layout: post
title: "Android开发技术周报 Issue#33"
date: 2015-05-27 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#33

### 教程

1. [在 Android 中使用 data-binder 绑定布局 xml 与数据](http://undownding.me/2015/05/31/android-data-binding/)

	在前几天的 Google IO 2015 中，Google 在 support-v7 中新增了 data-binder，使用 data-binder 可以直接在布局的 xml 中绑定布局与数据，从而简化代码。因为 data-binder 是包含在 support-v7 包里面的，所以可以向下兼容到最低 Android 2.1 (API level 7+).

1. [Android的材料设计兼容库](http://jcodecraeer.com/a/anzhuokaifa/developer/2015/0531/2958.html)

	这个兼容库很容易和之前的 Android Support Library 22.1混淆，都是兼容库，区别是这个库多了个Design。 Android Support Library 22.1只是支持了一些基本控件的材料设计化，但是这个库更多的是对一些特效的实现，这个库和github上的很多开源项目是有很大关系的，material design的很多效果，同一种效果在github上有太多的实现，现在官方把部分效果标准化了。

1. [Google I/O 2015 为 Android 开发者带来了哪些福利？](http://www.jianshu.com/p/4f7f55471da2)

	先得说的便是，今年的更新有些不给力，至少显得不够 Geek。我也不打算接着盘点一些在 Keynote 中的资讯，想必很多人在各个站点已经看过不知道多少遍了，我接下来想说的一些是关于这次 Google I/O 为 Android 开发者们带来了怎样的福利。

1. [Nexus6 With Android M开启多窗口模式](http://androidperformance.com/2015/05/29/Nexus6-with-Android-M开启多窗口模式/)	

	昨天的Google IO之后，Google放出了Android M Preview for Nexus6. 固件大家可以去Google的官网去下，下好了刷完之后，就可以体验一下最新的Android M了。

1. [使用Android Accessibility实现免Root自动批量安装功能](http://www.infoq.com/cn/articles/android-accessibility-installing)

	对于国内Android设备，应用的自动批量安装/更新一直是一个痛点，在之前，第三方应用商店通常要求设备Root，然后调用系统的PackageManagerService命令行来实现后台安装。最近，豌豆荚利用Android Accessibility（辅助功能）在业内率先实现了免Root自动批量安装功能。

1. [Android 9patch 图片解析堆溢出漏洞分析](http://security.tencent.com/index.php/blog/msg/85)

	前谷歌公开了一个今年1月份更新的漏洞。这个漏洞修复了一个存在于Android 5.1版本以下图片渲染的问题，可以查看相关链接。9patch是Android上特有的一种图片格式，就是在普通的png图片的基础了增加了一些像素的边框，使之具有可随意拉伸、缩放的功能。

1. [Gradle 修改 Maven 仓库地址](http://www.yrom.net/blog/2015/05/25/the_other_way_to_package_multi_channel_apks/)

	要先说明的是本文说的“渠道”单指在AndroidManifest.xml 用<meta-data>定义的一个标识字符串（如友盟统计）。在代码或者通过其他文件定义的方式殊途同归。说起 Android 多渠道打包，真是八仙过海各显神通：有手动一个个耐心打包的，有用Ant或Maven重复跑编译任务的，有用apktool解包后再修改重打包的，有在build.gradle定义一堆flavor的，乃至有通过apk里META-INF/下的空文件来定义渠道的。

1. [谷歌推荐的技术能力提升指南](http://www.imooc.com/wenda/detail/263443)

	打好扎实的计算机科学基础对于成为一个成功的软件工程师是非常重要的。本指南主要关于如何提升自己的技术能力，非常适合学生用于制定教学课程，当然这里提供的网络资源，并不意味着就可以完全取代现有的课程，正式的课程安排还是要学的(除非你不想拿到毕业证书)。

1. [Android应用setContentView与LayoutInflater加载解析机制源码分析](http://blog.csdn.net/yanbober/article/details/45970721)

	其实之所以要说这个话题有几个原因：1.理解xml等控件是咋被显示的原理，通常大家写代码都是直接在onCreate里setContentView就完事，没怎么关注其实现原理。2.前面分析《Android触摸屏事件派发机制详解与源码分析三(Activity篇)》时提到了一些关于布局嵌套的问题，当时没有深入解释。

1. [读Android 5.X源码系列之 - 当按下电源键后，系统启动流程浅析](http://chenqichao.me/2015/05/26/118-Android-50-003/)

	对用户来说，启动手机就是按下电源键，接着看着各种品牌Logo以及Slogan轮流出现，然后系统出现启动器主界面，这样系统就算启动成功了，好的用户体验是做到最少的时间、最流畅的启动即可。然而，对开发者来说我们更关心或者会带着这样疑问：“按下系统电源键后，Android系统到底做了哪些初始化工作？”今天就来看看，Android设备启动的大致流程。

1. [Android应用程序UI硬件加速渲染的预加载资源地图集服务（Asset Atlas Service）分析](http://blog.csdn.net/luoshengyang/article/details/45831269)

	 我们知道，Android系统在启动的时候，会对一些系统资源进行预加载。这样不仅使得应用程序在需要时可以快速地访问这些资源，还使得这些资源能够在不同应用程序之间进行共享。在硬件加速渲染环境中，这些预加载资源还有进一步优化的空间。

1. [Android 不规则封闭区域填充 手指秒变油漆桶](http://blog.csdn.net/lmj623565791/article/details/45954255)

	图像的填充有2种经典算法。

	* 一种是种子填充法。种子填充法理论上能够填充任意区域和图形,但是这种算法存在大量的反复入栈和大规模的递归,降低了填充效率。
	* 另一种是扫描线填充法。

1. [Android屏幕适配全攻略(最权威的官方适配指导)](http://blog.csdn.net/zhaokaiqiang1992/article/details/45419023)

	Android的屏幕适配一直以来都在折磨着我们这些开发者，本篇文章以Google的官方文档为基础，全面而深入的讲解了Android屏幕适配的原因、重要概念、解决方案及最佳实践，我相信如果你能认真的学习本文，对于Android的屏幕适配，你将有所收获！

1. [Android系统Root与静默安装](http://blog.csdn.net/yzzst/article/details/45746853)

	静默安装，指的是安装时无需任何用户干预，直接按默认设置安装应用。因为，它的无需用户干预，很多情况下变成了用户压根不知道，应用不知不觉就安装上了。是在推广上极为流氓的手段，很类似PC上的捆绑安装。正因为静默安装时极为流氓的推广行为，所以，其推广价格也极其高。

### 代码&开源库

1. [Android-NiceTab](https://github.com/RobotAmiee/Android-NiceTab)

	支持小圆点，背景模糊，图标cross fade等效果的自定义Tab.

1. [BGARefreshLayout-Android](https://github.com/bingoogolapple/BGARefreshLayout-Android)

	多种下拉刷新效果、上拉加载更多、可配置自定义头部广告位。

1. [AnimateCheckBox](https://github.com/hanks-zyh/AnimateCheckBox)

	自定义CheckBox，选中未选中的切换动画很赞。

1. [SelectorInjection](https://github.com/tianzhijiexian/SelectorInjection)

	一个强大的selector注入器，它可以让view自动产生selector状态，免去了你写selector的麻烦。

1. [ShareLoginLib](https://github.com/lingochamp/ShareLoginLib)

	第三方分享登录组件.

1. [AndroidGradleTemplate](https://github.com/jaredsburrows/AndroidGradleTemplate)

	Gradle + Android Studio + Robolectric + Espresso + Mockito + EasyMock/PowerMock + JaCoCo

1. [Android-Task](https://github.com/vRallev/android-task)

	可以在后台执行Task的Library。

1. [FORMWatchFace](https://github.com/romannurik/FORMWatchFace)
	
	Anddroid Wear 表盘。

1. [MultiThreadDownloader](https://github.com/AigeStudio/MultiThreadDownloader)

	逻辑比较简单但实用的Android多线程断点续传下载器。

1. [DatePicker](https://github.com/AigeStudio/DatePicker)
	
	Android日历选择器。

1. [Material Calendar View](https://github.com/prolificinteractive/material-calendarview)

	Material Design风格的日历控件。		

### 工具

1. [Android Studio 1.3 Preview1](http://www.androiddevtools.cn/#android-studio)
	
	The new version contains many new features.:
	
	* New Allocation Tracker 
	* New Heap dump Viewer
	* Many new code inspections to enforce framework and support library threading annotations, range annotations, call super, check result, etc.
	* Missing permission checks and unhandled revocable permission checks
	* Android M preview data binding Support
	* Support for adding Google Services to the project in the project structure dialog (especially for Analytics)
	* SDK update notifications, and brand new integrated SDK manager UI
	* New quickfixes, such as automatic generation of a Parcelable implementation
	* Many built-in live code templates
	* Many other smaller features and bug fixes
	
	As announced at Google I/O, Android Studio 1.3 will include C/C++ support as well, but that is not included in the first couple of preview buil
	
1. [Android NDK r10e](http://www.androiddevtools.cn/#ndk)

	Release Notes: [http://developer.android.com/intl/zh-cn/ndk/downloads/index.html#rel](http://developer.android.com/intl/zh-cn/ndk/downloads/index.html#rel)

1. [GsonFormat](https://github.com/zzz40500/GsonFormat)

	根据Gson库使用的要求,将JSONObject格式的String 解析成实体的 Android Studio 插件。

### 视频	

1. [Google I/O 2015的各种视频](http://i.youku.com/u/UMjczOTc0NDkzNg==)

	墙内Google I/O 2015的各种视频，没有看的小伙伴赶紧去瞅瞅看吧。

1. [Android QQ音乐架构演进](http://www.infoq.com/cn/presentations/evolution-of-android-qq-music-architecture)
	
	随着移动互联网的不断蓬勃发展，更多用户在移动设备上使用音乐服务，QQ音乐移动客户端使用用户数也在屡创新高，QQ音乐为了达到更好的用户体验并实现用户的新需求，原有的框架已经不能优雅的实现新需求和优先。如何优雅的实现各种需求并在性能和稳定性得到提高，QQ音乐Android开发团队通过以下的篇章给大家分享QQ音乐架构演进带来的痛与乐。 
			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)