layout: post
title: "Android开发技术周报 Issue#32"
date: 2015-05-23 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#32

### 教程

1. [Android 应用启动速度优化之 Systrace 的使用](http://www.tinylab.org/android-app-launch-speed-optimization-series-part1-systrace-usage/)

	Android 应用启动速度优化方式有很多方法，不过在优化之前，需要找到应用启动速度的瓶颈，找到关键点之后，再去优化，则可以达到事半功倍的效果。 Google 提供了很多 Debug 工具来帮助我们优化应用，这其中就包括 Systrace 工具。

1. [Android View.OnTouchListener 的子类](http://zhengxiaopeng.com/2015/04/26/Android-View-OnTouchListener-的子类/)

	如下是几个实现了 OnTouchListener 接口的子类，OnTouchListener 我们是再熟悉不过了，在 Hello World 开始就接触了，但在 Support V4 中还有它的 3 个子类我们平时可能使用的较少但就其功能而言还是对我们很有帮助的。	
	* AutoScrollHelper 抽象类，用于控件边缘触发自动滚动。
	* ListViewAutoScrollHelper 用于 ListView，目前 SDK 里的唯一 AutoScrollHelper 实现类。
	* ZoomButtonsController 用于控制缩放控件。

1. [Activity启动模式图文详解](http://jcodecraeer.com/a/anzhuokaifa/androidkaifa/2015/0520/2897.html)

	Activity是安卓上最聪明的设计之一，优秀的内存管理让多任务完美运行在最流行的操作系统之上。并不是让Activity在屏幕上启动就完事了，其启动方式也是需要关注的。这个话题的内容很多，其中很重要的就是启动模式（launchMode）。这也是我们这篇博客要讨论的内容。

1. [面向对象设计六大基本原则-以Volley为例](http://www.devtf.cn/?p=502) （@开发技术前线）

	在工作初期，我们可能会经常会有这样的感觉，自己的代码接口设计混乱、代码耦合较为严重、一个类的代码过多等等，自己回头看的时候都觉得汗颜。再看那些知名的开源库，它们大多有着整洁的代码、清晰简单的接口、职责单一的类，这个时候我们通常会捶胸顿足而感叹：什么时候老夫才能写出这样的代码！

1. [Android内核开发系列](http://ticktick.blog.51cto.com/823160/d-11)

	目前网上和市面上关于Android源码的博客和书籍挺多的，其中偏向对Android源码的分析的比较多，实践性强的相对比较少，我的目标是更多的分享一些实践性强的文章，我在学习一个新的领域时，总会有很多很多的困惑，我喜欢带着这些困惑去学习和实践，我相信只有把各种疑问和困惑都解决了，才算是真正的入门了

1. [读Android 5.X源码系列之 - 再看Log日志系统模块](http://chenqichao.me/2015/05/18/117-Android-50-002/)

	Android应用开发调试离不开各种log日志信息的帮助，一般情况下log日志可以帮你快速定位问题出错的前后位置，除了掌握基本的Java层使用log api，今天来看一下Android Log框架的构成。

1. [React Native概述：背景、规划和风险](https://github.com/tmallfe/tmallfe.github.io/issues/18) （@泡在网上的日子）

	Facebook在3.26 F8大会上开源了React Native，本文是对React Native的技术背景、规划和风险的概述。看得比较仓促，问题处请直接回复。

1. [详解Dagger2](https://github.com/bboyfeiyu/android-tech-frontier/tree/master/issue-11/详解Dagger2) （@开发技术前线）
	
	为什么使用依赖注入?首先我们需要知道，人们在很长的一段时间里都是利用控制反转原则规定：应用程序的流程取决于在程序运行时对象图的建立。通过抽象定义的对象交互可以实现这样的动态流程。而使用依赖注入技术或者服务定位器便可以完成运行时绑定。


1. [android中正确保存view的状态](http://jcodecraeer.com/a/anzhuokaifa/androidkaifa/2015/0512/2870.html) 

	今天我们聊一聊安卓中保存和恢复view状态的问题。我刻意强调View状态是因为我发现这个过程要比保存 Activity 和 Fragment状态稍微复杂，还有一个原因是因为网上有太多“重复造的轮子”（有时还是奇丑无比的轮子）

1. [Material适配2 - 高级篇](http://www.cnblogs.com/ct2011/p/4493439.html)

	在使用ActionBar的时候，一堆的问题：这个文字能不能定制，位置能不能改变，图标的间距怎么控制神马的，由此暴露出了ActionBar设计的不灵活。在上一篇中，我们只是简单使用了AppCompatActivity，他使用的仍然是ActionBar
官方在21以后提供了ToolBar。Toolbar之所以灵活，是因为它其实就是一个ViewGroup，我们在使用的时候和普通的组件一样，在布局文件中声明。
	
1. [Material适配1 - 入门篇](http://www.cnblogs.com/ct2011/p/4493384.html)

	随着Material Design的普及，很多开发人员都会面临App的Material适配。如果你的App不只是针对5.0以上设备的话（多数情况也必须做兼容）， 那么下面的经验总结将会对你有所帮助。当然，有些公司的App不会改成Material Design，但如果你以前使用AppCompatV7的话，升级到21后，你必然面临和以前不一样的使用方式，了解新的方式也是必须的。

1. [Android系统上的键盘监控](http://blog.csdn.net/yzzst/article/details/45747507)

1. [Android 项目打包到 JCenter 的坑](http://www.jianshu.com/p/c721f9297b2f?utm_campaign=hugo&utm_medium=reader_share&utm_content=note)
	
	搜索下如何发布 Android 项目的信息，大部分都会找到这篇文章 [Publishing Gradle Android Library to jCenter Repository](https://www.virag.si/2015/01/publishing-gradle-android-library-to-jcenter/)，中文的指引可以看[使用Gradle发布项目到JCenter仓库](http://zhengxiaopeng.com/2015/02/02/使用Gradle发布项目到JCenter仓库/)。不过，如果按照这些文章提供的 build.gradle，可能还会遇到一些坑。
	
1. [聊聊移动端跨平台开发的各种技术](http://fex.baidu.com/blog/2015/05/cross-mobile/?utm_source=www.race604.com&utm_source=Android周报&utm_campaign=10eaa2484e-Android_3_14_2015&utm_medium=email&utm_term=0_b86664ab0c-10eaa2484e-29249049)

	最近出现的 React Native 再次让跨平台移动端开发这个话题火起来了，曾经大家以为在手机上可以像桌面那样通过 Web 技术来实现跨平台开发，却大多因为性能或功能问题而放弃，不得不针对不同平台开发多个版本。但这并没有阻止人们对跨平台开发技术的探索，毕竟谁不想降低开发成本，一次编写就处处运行呢？除了 React Native，这几年还出现过许多其它解决方案，本文我将会对这些方案进行技术分析，供感兴趣的读者参考。

### 代码&开源库

1. [ExRecyclerView](https://github.com/tianzhijiexian/ExRecyclerView)

	扩展的RecyclerView，可以设置头/底部，Item点击/长按监听的recyclerView。可利用ExStaggeredGridLayoutManager给瀑布流设置头/底，利用DividerGridItemDecoration或DividerItemDecoration来添加分割线，可利用OnRecyclerViewScrollListener监听滑动到顶部、底部的事件，还可以监听滑动的距离

1. [TwitterCover-Android](https://github.com/cyndibaby905/TwitterCover-Android)

	模仿Twitter iOS客户端的下拉封面模糊效果。

1. [PolygonImageView](https://github.com/AlbertGrobas/PolygonImageView)

	多边形的ImageView。

1. [FlippableStackView](https://github.com/blipinsk/FlippableStackView)

	有一个堆栈效果的自定义View。
	
1. [GiftCard-Android](https://github.com/MartinRGB/GiftCard-Android)

	很赞的动画交互效果。

1. [RecyclerViewHeader](https://github.com/blipinsk/RecyclerViewHeader)
	 
	 轻松为RecyclerView添加头部，调用简单的代码就可以为LinearLayoutManager，GridLayoutManager ，StaggeredGridLayoutManager布局的RecyclerView添加header。

1. [HorizontalStackView](https://github.com/binaryroot/HorizontalStackView)

	水平效果的View堆栈效果。

1. [MovingImageView](https://github.com/AlbertGrobas/MovingImageView)
	
	图片可以自动移动的ImageView。	

1. [CommonAdapter](https://github.com/tianzhijiexian/CommonAdapter)

	通过封装BaseAdapter和RecyclerView.Adapter得到的通用的，简易的Adapter对象。
	
1. [DanmakuFlameMaster](https://github.com/Bilibili/DanmakuFlameMaster)

	DanmakuFlameMaster是Android上最好的开源弹幕引擎.

### 工具

1. [Android Studio 1.2.1.1](http://www.androiddevtools.cn/#android-studio)

	This release contains only bug fixes:

	* Updated the base IDE platform from IntelliJ 14.1 to 14.1.2.
	* Fixed a few critical bugs around Gradle sync, layout rendering and the first setup wizard

1. [Droid4X](http://www.droid4x.cn)

	兼容性和操控体验方面最好的安卓模拟器。

### 视频	

1. [视频: 如何成为一名优秀的设计师](http://v.youku.com/v_show/id_XOTU4NzE4NTQ4.html?from=y1.7-1.2)

	锤子科技视觉设计总监罗子雄在重庆TEDx上的演讲视频。

1. [10分钟看透最新Android开发框架Sky](http://www.jikexueyuan.com/course/848.html?hmsr=githubcn_weibo_c848_05.07)
	
	除游戏之外的 Android 应用通常使用 Java 语言来开发，而谷歌内部的一个团队正在探索全新的应用开发方式。他们利用了谷歌自主的网页开发语言 Dart 来开发 Android 应用。在 Android 项目中使用的 Dart 并未被称作 “Android 版 Dar t”，而是有了一个新名字“ Sky ”。这帮助他们专注于速度，并可以与网页进行深度整合。

### 设计

1. [谢谷歌大神传我动画设计30年功力](http://www.zcool.com.cn/article/ZMTU5MzAw.html)
	
	谷歌上一代设计语言是卡片设计，而这一代作为卡片的延伸，Material Design 以纸片与墨水作为灵感，由纸片与墨水组成的设计隐喻贯穿整个material design 的所有细节，动画设计也不例外。
		
### 新闻

1. [例行拆包 Google Play，结果发现他们要进中国了](http://36kr.com/p/533203.html)
	
	我们曾经在去年末 Gmail 访问异常和上个月的 Google Play VP 采访中提到，Google Play Service 部分入华的计划确实存在，只剩下时间问题。Google 中国相关的工作人员也曾经告诉 36Kr，Sundar Pichai 曾经在今年的 MWC 期间表达过 Play 入华的意愿，不过需要注意的是：Google Play(Services)  此前从未正式在中国区开战业务，所以谈不上“回归”，称为“进入”中国会更合适。
			
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)