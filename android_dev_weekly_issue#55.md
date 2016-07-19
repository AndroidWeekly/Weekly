layout: post
title: "Android开发技术周报 Issue#55"
date: 2015-11-03 22:34:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#55

### 新闻

1. [Kotlin语言1.0Beta发布，JetBrain介绍其设计理念](http://www.infoq.com/cn/news/2015/11/kotlin-10beta)

	2010年，长达是十年之久的Java开发让JetBrains的工程师认为老旧的Java语言已经严重阻碍了生产力。他们认为是时候开发一款现代化的JVM语言了，这也是因为他们有足够的资源和专家。本身做各种IDEs起家的JetBrains就开始着手新工具的开发——一个编程语言。

### 教程

1. [深入理解Android之AOP](http://blog.csdn.net/innost/article/details/49387395)

	大家都知道OOP，即ObjectOriented Programming，面向对象编程。而本文要介绍的是AOP。AOP是Aspect Oriented Programming的缩写，中译文为面向切向编程。OOP和AOP是什么关系呢？首先：
l OOP和AOP都是方法论。我记得在刚学习C++的时候，最难学的并不是C++的语法，而是C++所代表的那种看问题的方法，即OOP。

1. [Android实战之你应该使用哪个网络库？](http://segmentfault.com/a/1190000003965158)

	目前基本上每个应用都会使用HTTP/HTTPS协议来作为主要的传输协议来传输数据。即使你没有直接使用HTTP协议，也会有成堆的SDK会包含这些协议，譬如分析、Crash反馈等等。当然，目前也有很多优秀的HTTP的协议库，可以很方便的帮助开发者构建应用，本篇博文中会尽可能地涵盖这些要点。

1. [Android M新特性Doze and App Standby模式详解](http://t.cn/RUov6lo)

	从Android6.0开始，Android提供了两种省电延长电池寿命的功能：Doze和App Standby；表现形式：当设备没有连接到电源，设备进入Doze模式时，系统将通过延迟最近用户没有使用的应用程序的后台CPU运作及网络活动，让应用程序处于App Standby状态，以此来减少电池消耗。谷歌表示，在Nexus5和Nexus6上测试，当屏幕处于关闭状态，平均续航时间提高30%；

1. [加速你的Android应用](http://www.devtf.cn/?p=1097)

	几周之前，我在Droidcon NYC上有过一次关于Android性能优化的演讲。.我在这个演讲中花费了大量的时间，因为我想通过真实的例子展现性能问题，以及我是通过什么样的工具去发掘这些问题的。因为时间原因，在演讲中我不得不舍弃一半的内容。在这篇文章中，我会总结在演讲中我所讨论的所有内容，并且给出实例。

1. [内存泄露从入门到精通三部曲之基础知识篇](http://t.cn/RUovc7X)

	试想这个场景，应用起来以后，转屏。转屏以后，旧MainActivity会destroy，新MainActivity会重建，导致单例ImageUtil重新getInstance。很不幸的是，由于instance已经不是空的了，所以ImageUtil不会重建，还持有之前的Context，也就是之前的那个MainActivity实例的context

1. [携程Android App插件化和动态加载实践](http://t.cn/RUigGIL)

	携程Android App的插件化和动态加载框架已上线半年，经历了初期的探索和持续的打磨优化，新框架和工程配置经受住了生产实践的考验。本文将详细介绍Android平台插件式开发和动态加载技术的原理和实现细节，回顾携程Android App的架构演化过程，期望我们的经验能帮助到更多的Android工程师。

1. [移动端图片格式调研](http://blog.ibireme.com/2015/11/02/mobile_image_benchmark/)

	图片通常是移动端流量耗费最多的部分，并且占据着重要的视觉空间。合理的图片格式选用和优化可以为你节省带宽、提升视觉效果。在这篇文章里我会分析一下目前主流和新兴的几种图片格式的特点、性能分析、参数调优，以及相关开源库的选择。

1. [关于Android Log的一些思考](http://droidyue.com/blog/2015/11/01/thinking-about-android-log/)

	在日常的Android开发中，日志打印是一项必不可少的操作，我们通过分析打印的日志可以分析程序的运行数据和情况。然而使用日志打印的正确姿势又是怎样呢，如何屏蔽日志信息输出呢，本文将逐一进行回答。

1. [Android NDK中C++运行时库介绍](http://blog.csdn.net/roland_sun/article/details/49475969)

	一般的Android应用程序都是用Java语言编写的，在Dalvik虚拟机或ART虚拟机中运行的。但是，出于对性能的考虑，Android也允许使用JNI接口，直接调用原生（Native）程序。这些程序都是直接被编译成平台支持的汇编指令，效率自然比在虚拟机中运行的要高。不过，现在ART虚拟机出现了，JNI调用在性能方面的优势被大大缩减。

1. [Android打包的那些事](http://www.jayfeng.com/2015/11/07/Android打包的那些事/)

	使用gradle打包apk已经成为当前主流趋势，我也在这个过程中经历了各种需求，并不断结合gradle新的支持，一一改进。在此，把这些相关的东西记录，做一总结。

1. [MVVM_Android-CleanArchitecture](http://segmentfault.com/a/1190000003966281)

	"Architecture is About Intent, not Frameworks" - Robert C. Martin (Uncle Bob)，Uncle Bob 的这句话套在 MVVM 上也是适用的, MVVM 也仅仅是架构模式（Architectural pattern），其有一套自己的理论概念（pattern）而不是规定的具体实现（或 Frameworks）。早之前在知乎上相关问题的回答（android UI设计MVVM设计模式讨论？）中也简单提到过 MVVM 了，M-V-X 的关系如上图，那么这一次博主把 Fernando Cejas(android10) 的 Android-CleanArchitecture 项目中的 MVP 实现重构成了用 MVVM 来实现。

1. [Android项目重构之路:架构篇](http://keeganlee.me/post/android/20150605)

	去年10月底换到了新公司，做移动研发组的负责人，刚开始接手android项目时，发现该项目真的是一团糟。首先是其架构，是按功能模块进行划分的，本来按模块划分也挺好的，可是，他却分得太细，总共分为了17个模块，而好几个模块也就只有两三个类而已。但应用本身其实比较简单，要按功能模块来分的话，最多五个模块就够了。

1. [Android项目重构之路:界面篇](http://keeganlee.me/post/android/20150619)

	在前一篇文章《Android项目重构之路:架构篇》中已经简单说明了项目的架构，将项目分为了四个层级：模型层、接口层、核心层、界面层。其中，最上层的界面，是变化最频繁的一个层面，也是最复杂最容易出问题的一个层面，如果规划不好，很容易做着做着，又乱成一团了。

1. [Android项目重构之路:实现篇](http://keeganlee.me/post/android/20150629)

	前两篇文章Android项目重构之路:架构篇和Android项目重构之路:界面篇已经讲了我的项目开始搭建时的架构设计和界面设计，这篇就讲讲具体怎么实现的，以实现最小化可用产品(MVP)的目标，用最简单的方式来搭建架构和实现代码。
IDE采用Android Studio，Demo实现的功能为用户注册、登录和展示一个券列表，数据采用我们现有项目的测试数据，接口也是我们项目中的测试接口。

### 代码&开源库

1. [Nevolution](https://github.com/oasisfeng/nevolution)

	冯森林(无锋) [@oasisfeng](http://weibo.com/oasisfeng) 大神的新项目，旨在带来更加干净的 Android 环境。

1. [DynamicAPK](https://github.com/CtripMobile/DynamicAPK)

	实现Android多apk/dex方式的apk加载，支持资源分包.

1. [AndroidChangeSkin](https://github.com/hongyangAndroid/AndroidChangeSkin)

	一种完全无侵入的换肤方式，支持插件式和应用内，无需重启Activity.

1. [InteractiveCanvas](https://github.com/elevenetc/InteractiveCanvas)

	一个可以联动交互的Canvas。
	
1. [AutoHomeRefreshListView](https://github.com/nugongshou110/AutoHomeRefreshListView)

	仿汽车之家下拉刷新效果

1. [AndroidSwipeableCardStack](https://github.com/wenchaojiang/AndroidSwipeableCardStack)

	一个可滑动的卡片View堆叠效果的控件。

1. [Search-View-Layout](https://github.com/sahildave/Search-View-Layout)	
	一个模仿5.0系统拨号器搜索联系人效果的搜索视图布局。

1. [TextViewForFullHtml](https://github.com/xuyisheng/TextViewForFullHtml)	
	TextViewForFullHtml是对原生TextView解析Html格式文本的增强。
	
### 工作机会

1. [GrowingIO 招聘 Android 工程师 (地点:北京 望京北酒厂艺术园 薪资待遇: 20-40K/月)](http://t.cn/RUNDptw)

	GrowingIO 是一家来自美国硅谷的大数据分析公司，专注于利用移动互联网数据来为企业创造商业价值，帮助我们的客户企业实现业务的高速增长。GrowingIO 拥有丰富的跨平台数据分析产品，涵盖移动 App 和传统网站，将美国最新的商业分析智能和传统的大数据分析从过去四个星期到几个月的工作压缩到几秒钟到几个小时，为互联网企业提供全面的革命性数据分析解决方案。他们的招聘要求是这样的[请戳这里](http://t.cn/RUNDptw)，他们的团队以及办公环境是这样的[请戳这里](http://t.cn/RUNDyfS)

----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)