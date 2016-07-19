layout: post
title: "Android开发技术周报 Issue#35"
date: 2015-06-9 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#35

### 教程

1. [Google Developing for Android 九 － Tools](http://www.lightskystreet.com/2015/06/13/google-for-android-9-tools/)

	Andorid提供了很多可以帮助我们debug和分析问题的工具，它们可以让你的app拥有更好的性能。这些检测工具涵盖了内存分析，比如Allocation Tracker(在DDMS和Android Studio中都有)和设备性能。知道这些工具很重要，但更重要的是要真正的使用这些工具，保证你的应用拥有期望的表现（60帧限制，避免垃圾回收器搅动）。通过尽可能的优化和提高整体体验可以帮助Android更好的整体平台性。

1. [Google Developing for Android 八 － User Interface](http://www.lightskystreet.com/2015/06/13/google-for-android-8-user-interface/)

	正如在第一篇Context介绍种关于GPU讨论的部分所说，很多手机的性能有限，如果应用中有严重的过度绘制可能会导致比较糟糕的渲染性能。不透明的View会完全遮盖其它的View的情况下会导致渲染引擎进行多次绘制。你可以通过开启设置中的开发者选项的GPU overdraw来修复相应的问题。

1. [Android图片编码机制深度解析（Bitmap，Skia，libJpeg）](http://www.cnblogs.com/hrlnw/p/4403334.html)

	工作中遇到了Android中有关图片压缩保存的问题，发现这个问题还挺深，而且网上资料比较有限，因此自己深入研究了一下，算是把这个问题自顶至下全部搞懂了，在此记录。相关的几个问题如下：1.Android系统是如何编码压缩保存图片的？2.Skia库起到的作用？3.libJpeg库起到的作用？4.能不能自己调用Skia或libJpeg？

1. [戏（细）说Executor框架线程池任务执行全过程（上）](http://www.infoq.com/cn/articles/executor-framework-thread-pool-task-execution-part-01)

	1.5后引入的Executor框架的最大优点是把任务的提交和执行解耦。要执行任务的人只需把Task描述清楚，然后提交即可。这个Task是怎么被执行的，被谁执行的，什么时候执行的，提交的人就不用关心了。具体点讲，提交一个Callable对象给ExecutorService（如最常用的线程池ThreadPoolExecutor），将得到一个Future对象，调用Future对象的get方法等待执行结果就好了。

1. [戏（细）说Executor框架线程池任务执行全过程（下）](http://www.infoq.com/cn/articles/executor-framework-thread-pool-task-execution-part-02)

	上一篇文章中通过引入的一个例子介绍了在Executor框架下，提交一个任务的过程，这个过程就像我们老大的老大要找个老大来执行一个任务那样简单。并通过剖析ExecutorService的一种经典实现ThreadPoolExecutor来分析接收任务的主要逻辑，发现ThreadPoolExecutor的工作思路和我们带项目的老大的工作思路完全一致。
	
1. [Android Studio新手完全指引](http://www.jianshu.com/p/f7de559b9752)

	Android Studio的基本用法就比较琐碎了，篇幅也比较大，已经有很多文章进行过介绍，这里就不展开讲解了，想了解的可以参考@StormZhang的系列教程，教程中基于Android Studio 1.0 版本进行介绍，跟最新的有些许差别，但并不影响我们学习。

1. [[AndroidUITestRunner]面向UI的单元测试框架](http://www.jianshu.com/p/3453b641e594)

	通常我们使用的单元测试框架都是用来测试一些非UI的逻辑的，如JUnit,CPPUnit。我希望团队中的成员都要养成写单元测试的习惯，一方面单元测试本身就是一份非常好的文档，另一方面单元测试有助于强迫使你的代码耦合更加松散(模块可以独立测试), 在移动应用开发中我遇到一些这样的问题。

1. [Android应用Activity、Dialog、PopWindow、Toast窗口添加机制及源码分析](http://blog.csdn.net/yanbober/article/details/46361191)

	在那篇文章里我们当时重点是Activity的View加载解析xml机制分析，当时说到了Window的东西，但只是皮毛的分析了Activity相关的一些逻辑。（PS：看到这不清楚上面啥意思的建议先移步到《Android应用setContentView与LayoutInflater加载解析机制源码分析》，完事再回头继续看这篇文章。）当时给大家承诺过我们要从应用控件一点一点往下慢慢深入分析，所以现在开始深入，但是本篇的深入也只是仅限Window相关的东东，之后文章还会继续慢慢深入。

### 代码&开源库

1. [android-ui-test-runner](https://github.com/examplecode/android-ui-test-runner)

	一个非常简单的用于测试 UI 的单元测试框架.

1. [ProductTour](https://github.com/matrixxun/ProductTour)

	Google Drive的视差滚动引导页效果实现.

1. [SilkCal](https://github.com/NLMartian/SilkCal)

	一个效果很赞的自定义日历View.

1. [velocimeter-view](https://github.com/glomadrian/velocimeter-view)

	一个速度指示盘效果的自定义View.

1. [SublimePicker](https://github.com/vikramkakkar/SublimePicker)

	一个Material Design风格的日期、时间选择器.

1. [Spanny](https://github.com/binaryfork/Spanny)

	一个继承自 SpannableStringBuilder 的工具类，添加了一些可以方便你给文本添加多种Span的方法.

1. [MaterialProgressBar](https://github.com/DreaminginCodeZH/MaterialProgressBar)

	在4.0系统以上提供统一风格 Material Design 风格的 ProgressBar.

### 工具

1. [infer](https://github.com/facebook/infer)

	Facebook 开源的静态代码分析工具，用于在发布移动应用之前对代码进行分析，找出潜在的问题。目前 Facebook 使用该工具来分析 Facebook 的 App，包括 Android 、iOS、Facebook Messenger 和 Instagram 等等。

1. [eventbus-intellij-plugin](https://github.com/kgmyshin/eventbus-intellij-plugin)

	Plugin to navigate between events posted by EventBus.

1. [SQLScout](http://www.idescout.com)

	在 Android studio 内连接并操作 Android 设备上 sqlite 数据库。Android 工程师杀人越货居家旅行必备插件！

1. [android-dip-ruler](https://github.com/BoD/android-dip-ruler)

	Print it, cut it, give it to your designer!

			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)