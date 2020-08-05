layout: post
title: "Android开发技术周报 Issue#34"
date: 2015-06-2 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#34

### 教程

1. [Google Develop for Android 系列](http://www.lightskystreet.com/categories/Android最佳实践/)

	前几天在G+上看到Google Developers站点，有一个Android系列的文章，分享到个人微博，周末闲来没事就学写了下，把它们简单的翻译了下，没想到一发不可收拾，六篇文章全部都翻译完了，有些地方省略了部分示例的描述或者换了另一种表述，如果有理解的不准确的地方，还望指正。

1. [Android内核开发：图解Android系统的启动过程](http://ticktick.blog.51cto.com/823160/1659473#0-tsina-1-95166-397232819ff9a47a7b7e80a40613cfe1)

	学习任何软硬件系统，研究系统启动过程都是一种非常有效地起步手段，搞Android内核开发也不例外。网上有很多文章对Android启动相关代码进行分析和走读，大家可以先搜索阅读一下，我个人更喜欢更加直观的方式去理解未知的东西，包括图、表、系统输出的log信息等等，因此，本文准备通过一些流程图和log信息，来探索一下Android的启动过程。

1. [Android优化笔记](http://www.csdn.net/article/2015-06-06/2824884#0-tsina-1-58084-397232819ff9a47a7b7e80a40613cfe1)

	什么样的应用才能称得上是优雅的App？这是腾讯内部一直在思考的问题，优雅的App就是把简单的事情做到极致，必须对终端应用性能进行打磨。在Android应用优化方面，主要包括内存和UI流畅度的问题，比如内存占用与泄露，UI流畅度的帧数和响应时间，IO的阻塞式响应时间等。

1. [Android 系统稳定性 - ANR（一）](http://rayleeya.iteye.com/blog/1955652)

	如果你是一个Android应用程序开发人员，你的人生中不可避免的三件事情是：死亡、缴税和ANR。这么说是夸张了，但是由于Android本身的设计，以及应用程序和系统在开发过程中的缺陷，经常会在测试过程中遇到各种各样的ANR问题。在功能性的测试中还少一些，主要是在压力测试中（例如Monkey测试）会遇到非常多的ANR问题。

1. [Android 系统稳定性 - ANR（二）](http://rayleeya.iteye.com/blog/1955657)

	引起ANR问题的根本原因，总的来说可以归纳为两类：1.应用进程自身引起的，例如：主线程阻塞、挂起、死循环,应用进程的其他线程的CPU占用率高，使得主线程无法抢占到CPU时间片其他进程间接引起的，例如：当前应用进程进行进程间通信请求其他进程，其他进程的操作长时间没有反馈，其他进程的CPU占用率高，使得当前应用进程无法抢占到CPU时间片，分析ANR问题时，以上述可能的几种原因为线索，通过分析各种日志信息，大多数情况下你就可以很容易找到问题所在了。

1. [Android 系统稳定性 - ANR（三）](http://rayleeya.iteye.com/blog/1956056)

	Android应用程序的所有标准组件全部运行在一个单一的主线程中，在主线程中所做的任何耗时的操作都有可能造成ANR，因为这些耗时的操作会使得主线程没有机会处理用户输入事件或者广播事件。因此在主线程中执行的任何函数所做的工作都应该尽可能的少，特别是对于Activity的生命周期函数来说。网络和数据库操作，以及诸如位图变换的一些耗时的操作，都应该放在子线程中完成。主线程不需要等待子线程的执行，主线程应该创建一个与其绑定的Handler对象，子线程执行完毕后通过Handler通知主线程。

1. [Android Design Support Library使用详解](http://blog.csdn.net/eclipsexys/article/details/46349721)

	Google在2015的IO大会上，给我们带来了更加详细的Material Design设计规范，同时，也给我们带来了全新的Android Design Support Library，在这个support库里面，Google给我们提供了更加规范的MD设计风格的控件。最重要的是，Android Design Support Library的兼容性更广，直接可以向下兼容到Android 2.2。这不得不说是一个良心之作。

1. [程序猿必看交互设计](http://blog.csdn.net/satisfied_zx/article/details/46372035)

	本文作者 Pasquale D'Silva 是 Elepath 的一位交互设计师兼产品设计师，在本文中，他从交互的角度阐释了优秀的设计应该具有的一些品质，或者说，优秀的产品该如何实现与用户的自然沟通。不得不说，有太多程序猿或者美工(注意，是美工，真正的设计师不会这么干)误把技术当艺术、把漂亮当设计了，真正重要的交互部分反而被忽略，你可以看看，一大批的产品都是近乎静态的，许多操作诡异至极.

1. [完全掌握Android Data Binding](https://github.com/LyndonChin/MasteringAndroidDataBinding)

	本教程是跟着 Data Binding Guide 学习过程中得出的一些实践经验，同时修改了官方教程的一些错误，每一个知识点都有对应的源码，争取做到实践与理论相结合。Data Binding 解决了 Android UI 编程中的一个痛点，官方原生支持 MVVM 模型可以让我们在不改变既有代码框架的前提下，非常容易地使用这些新特性。其实在此之前，已经有些第三方的框架（RoboAndroid) 可以支持 MVVM 模型，无耐由于框架的侵入性太强，导致一直没有流行起来。

1. [防御性编程与疯狂偏执性编程](http://www.codeceo.com/article/defensive-programming-vs-crazy-programming.html)

	当程序员遇到意想不到又不能修复的bug时，，他们会“添加一些防御性的代码”，这不但可以使得代码更安全，还更容易发现问题。有时候这样的行为甚至可以直接消灭问题。开发人员还会进行数据验证——确保检查输入和输出域和返回值；审查和改进错误处理——可能会围绕一些“不可能”的条件做一些检查；添加一些有用的日志记录和诊断。换句话说，问题代码优先。

### 代码&开源库

1. [FABProgressCircle](https://github.com/JorgeCastilloPrz/FABProgressCircle)

	围绕 FloatingActionButton 的圆形进度条效果。

1. [bottomsheet](https://github.com/Flipboard/bottomsheet)

	Android component which presents a dismissible view from the bottom of the screen.

1. [AppIntro](https://github.com/PaoloRotolo/AppIntro)

	可以让你在自己的App里实现很Cool的引导页效果的库.

1. [Nammu](https://github.com/tajchert/Nammu)

	运行时权限检查助手.

1. [ColorPhrase](https://github.com/THEONE10211024/ColorPhrase)

	一个可以根据指定分隔符字符串包含的文本格式化为指定颜色的Library.

1. [colorize](https://github.com/cesarferreira/colorize)

	Android quick access to 1000+ preloaded colors!
	一个可以让你快速使用1000多个预置颜色的库。

1. [WheelIndicatorView](https://github.com/dlazaro66/WheelIndicatorView)		
	模仿 Google Fit 的活动指示进度效果.

1. [EdittextWithTag](https://github.com/pchauhan/EdittextWithTag)

	可以将输入EditText的内容自动转换为一个Tag效果。

1. [PopSeekbar](https://github.com/jiahuanyu/PopSeekbar)

	一个漂亮的自定义SeekBar。

1. [Cult](https://github.com/ppamorim/Cult)

	Cult提供一个新的工具栏布局，可以让你使用一个自定义的SearchView动画等等。

1. [WaveCompat](https://github.com/wangjiegulu/WaveCompat)

	Activity 波纹动画效果兼容库.

1. [CircleTimerView](https://github.com/jiahuanyu/CircleTimerView)

	效果很赞的圆形计时器View.

1. [PlayAnimations](https://github.com/naman14/PlayAnimations)

	PlayGames app中各种动画效果的demo。

1. [ParallaxSplash](https://github.com/leerduo/ParallaxSplash)

	视差动画的引导页.

### 工具

1. [Android Studio 1.2.2](http://www.androiddevtools.cn/#android-studio)

	

1. [ormlite-android-gradle-plugin](https://github.com/stephanenicolas/ormlite-android-gradle-plugin)

	一个可以帮助你生成 ORMLite 的配置文件的 Android Studio 插件。

### 新闻

1. [谷歌推出智能密码锁](http://www.infoq.com/cn/news/2015/06/google-smart-lock-passwords)

	谷歌在I/O 2015大会上宣布了“谷歌身份平台（Google Identity Platform）”，这是一个跨Android、iOS和Web应用程序管理身份以及处理身份验证与授权的工具和API 集合。除了大家熟悉的Sign-in，为了使用户能够使用他们的谷歌账户登录，谷歌推出了“智能密码锁（Smart Lock for Passwords）”，目前只能用在Android上，以后也可能扩展到iOS。

### 视频

1. [Android Performance Patterns系列视频](http://pan.baidu.com/s/1jGiWaVG)
	
	Google官方推出的一系列帮助你优化Android App性能视频，@hi大头鬼hi 同学把它们全部搬到了墙内，还没看的小伙伴赶紧去看看吧。

### 书

1. [Producter](http://producter.io)

	一本涵盖 设计，交互，动效，iOS开发，Swift，营销的跨界作品 — 《Producter》。一本很不错的书，推荐大家看一下。独立完成一款产品是很多人的梦想，也是我的梦想，但是单单完成一个作品并没有什么价值，真正完成一款优秀的作品的难度远超过了 “完成” 这个词语。设计上的锤炼，编程技艺的精进，营销的思考，让很多人都在起步阶段就放弃了。从来没有一本书，去讲如何完整的完成这件事情。
	
### 设计

#### 资源

1. [ TO-DO APP UI KIT ](http://www.invisionapp.com/do)

	一个TO-DO APP UI全套设计资源，可以免费下载和使用，包含Photoshop和Sketch双版本。

#### 教程

1. [免费了，切图标记外挂神器 Assistor PS 深入解读(上)](http://bigertech.com/post/assistor-ps-1/)
	
	与其他切图标记软件不同的是，Assistor PS 是完全独立于 PS 本身的，说是一个外挂更加合适，旨在提高切图标记的效率及速度。虽然不是一个插件，但是它与 PS 是连通的，当你在 PS 选择一个图层在后，即可使用它的功能。如果你肯花点时间下载是试用，相信不会让你失望，甚至能可能让你觉得相见恨晚。

1. [免费了，切图标记外挂神器 Assistor PS 深入解读(下)](http://bigertech.com/post/assistor-ps-2/)

	在 切图标记外挂 Assistor PS 深入解读（上）中，我给大家介绍了即将免费的切图标记外挂 Assistor PS 强大的标记功能，然后，这个神器的功能仅仅如此？本文将为介绍 Assistor PS 其他丧心病狂的功能：创建引导框，一键全自动切图，创建参考线，单位转换器，取色器，圆角矩形转换，按照固定间隔复制图层等。
			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)