layout: post
title: "Android开发技术周报 Issue#15"
date: 2015-01-12 09:59:10 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#15
	
### 教程

1. [打造极致Material Design动画风格Button](http://blog.csdn.net/qiujuer/article/details/42471119)

	在我的文章中曾经有两篇关于Material Design风格的按钮实现。在第一章中只是简单的实现了动画的波纹效果，而在第二篇中对此进行了一定的扩充与优化，最后实现可以自动移动到中心位置的动画；虽然两者都可用，但是在我的使用中却发现了一定的问题，如有些位置点击会出现波纹速度的运算上的问题。

1. [Android开发-API指南-AIDL](http://www.osforce.cn/group/9/thread/1065?fr=weibo&mu=140910XRNWcD)

	Android 接口定义语言 AIDL（Android Interface Definition Language）与其他已有的 IDL 很类似。 客户端和服务端可以通过由它定义的编程接口来达成共识，以便通过进程间通讯（IPC）完成相互通讯。 在 Android 系统中，通常一个进程不允许直接访问另一个进程的内存。 因此为了能够实现对话，进程需要把对象分解为操作系统可以识别的原生数据，在跨越进程边界后再组装起来。 实现组装的代码非常枯燥无趣，因此 Android 通过 AIDL 可有助于完成这一过程。

1. [Android Proguard 详解](http://www.osforce.cn/group/9/thread/1053?fr=weibo&mu=140910XRNWcD)

	Java代码是非常容易反编译的。为了很好的保护Java源代码，我们往往会对编译好的class文件进行混淆处理。ProGuard是一个混淆代码的开源项目。它的主要作用就是混淆，当然它还能对字节码进行缩减体积、优化等，但那些对于我们来说都算是次要的功能。官网网址是：http://proguard.sourceforge.net/

1. [设计模式问答2](http://www.importnew.com/14347.html)

	这是设计模式问答1的连载。在这个系列，我们将覆盖到解释器、迭代器、调停者、备忘录和观察者模式。

1. [Java不同压缩算法的性能比较](http://www.importnew.com/14410.html)

	本文将会对常用的几个压缩算法的性能作一下比较。结果表明，某些算法在极端苛刻的CPU限制下仍能正常工作。文中进行比较的算有：JDK GZIP、JDK deflate、LZ4压缩算法的Java实现和Snappy。

1. [Android软件安全开发实践（上）](http://www.programmer.com.cn/15036/)

	Android开发是当前最火的话题之一，但很少有人讨论这个领域的安全问题。本系列将分两期，探讨Android开发中常见的安全隐患和解决方案。第一期将从数据存储、网络通信、密码和认证策略这三个角度，带你走上Android软件安全开发实践之旅。
	
1. [Android软件安全开发实践（下）](http://www.programmer.com.cn/15273/)
	
	在《Android软件安全开发实践（上）》中我们讨论了数据存储、网络通信、密码和认证策略等安全问题和解决方案，本期将继续从组件间通信、数据验证和保全保护等方面来实践Android软件安全开发之路。

<!--more-->

1. [深度：针对超强手机木马DenDroid的分析与测试](http://www.freebuf.com/tools/55392.html)

	赛门铁克的研究人员就在手机移动领域发现了一种新的名为Dendroid木马，可以轻松实现对手机远程恶意操控。而在此前赛门铁克发现了一个名为AndroidRAT的android远程管理软件被认为是第一个恶意绑定软件。然而这款最新发现的运行在http上的Dendroid具有更强功能。

1. [解析IntelliJ IDEA内部设计](http://www.importnew.com/14260.html)

	IntelliJ IDEA第一版发布于2001年1月，这是第一款集成了高级代码导航和代码重构功能的Java IDE。2009年，JetBrains开源了其社区版。从那时开始，就新出现了许多基于其社区版的IDE，如Google的Android Studio。本文使用JArchitect作为工具，深入了解Intellij IDEA社区版，探索其中使用的一些内部设计决策。

1. [Android Studio系列教程五--Gradle命令详解与导入第三方包](http://stormzhang.com/devtools/2015/01/05/android-studio-tutorial5/)

	Android Studio + Gradle的组合用起来非常方便，很多第三方开源项目也早都迁移到了Studio，为此今天就来介绍下查看、编译并导入第三方开源项目的方法。

### 代码&开源库

1. [ImageCropper](https://github.com/Jhuster/ImageCropper)

	一个Android图片剪裁库,特性:1.支持通过手势移动和缩放剪裁窗口, 2支持固定剪裁窗口大小、固定窗口的长宽比率, 3.支持设置最大的窗口长和宽, 4.支持剪裁图片的旋转。

1. [Telecine](https://github.com/JakeWharton/Telecine)

	JakeWharton大神开发的一款录屏App。

1. [DynamicRecyclerView](https://github.com/ismoli/DynamicRecyclerView)

	对RecyclerView进行了扩展，天就拖拽排序功能。

1. [BusWear](https://github.com/tajchert/BusWear)
	
	BusWear是一个简单的支持Android Wear设备的EventBus（事件总线）库。仅需要一行代码就可获得异步的事件总线（synchronized event buses）在Wear和移动平台之间。
		
	![image](https://raw.githubusercontent.com/tajchert/BusWear/master/docs/diagram_simple.png)
	
1. [SuperSLiM](https://github.com/TonicArtos/SuperSLiM)
	
	SuperSLiM为RecyclerView提供了一个布局管理器允许您创建垂直列表和每节标题和布局。 

	![image](https://camo.githubusercontent.com/3a55cfd0bbfd28e72aa875f4905cc23cc37a87f4/68747470733a2f2f342e62702e626c6f6773706f742e636f6d2f2d657034364a4b70476138342f564a685831706c575743492f4141414141414141585a592f394131417272563361336b2f73313630302f5375706572534c694d2d44656d6f2d736d616c6c2e676966)

1. [Header2ActionBar](https://github.com/AChep/Header2ActionBar)
	
	Header2ActionBar是一个实现了像Play Music and Google Newspaper应用中褪色（fading）Action Bar效果的Action Bar。
	
1. [recyclerview-animators](https://github.com/wasabeef/recyclerview-animators)

	一个方便你给RecyclerView items添加item动画的库。

1. [Singleton](https://github.com/Raizlabs/Singleton)
	
	一个非常简洁的库，可以帮助你方便将一个对象存储在磁盘。

1. [android-asyncservice](https://github.com/JoanZapata/android-asyncservice)

	AsyncService使用注释来缩短开始异步长时间运行的任务所需的代码,并返回结果。

1. [Reachability](https://github.com/sakebook/Reachability)

	类似于iPhone 6 & 6 Plus的下拉悬停从而方便你操作屏幕的顶部。
	
	![image](https://raw.githubusercontent.com/sakebook/Reachability/master/images/demo.gif)
	
1. [SectionCursorAdapter](https://github.com/twotoasters/SectionCursorAdapter)
	
	对CursorAdapter进行了扩展，添加sections和快速滚动滑块。
		
	![image](https://raw.githubusercontent.com/twotoasters/SectionCursorAdapter/master/screenshots/sections.png)![image](https://raw.githubusercontent.com/twotoasters/SectionCursorAdapter/master/screenshots/dialog.png)
	
1. [android-quick-response-code](https://github.com/phishman3579/android-quick-response-code)

	Android QR码编码解码库。
	
### 工具	 	 

1. [gradle-mdicons](https://github.com/tmiyamon/gradle-mdicons)

	一个帮助你管理google's official material design图标的插件。
	
	![image](https://raw.githubusercontent.com/tmiyamon/gradle-mdicons/master/gradle-mdicons-result.png)

### 视频

1. [ChinaGDG 视频中心](http://i.youku.com/chinagdg)

	ChinaGDG 视频中心。第一时间同步 Google Developers 的各种技术视频，如 Android、Web 等技术，方便国内开发者学习。视频已包含英文字幕，部分视频还有来自国内志愿者提供的中文翻译字幕。

1. [Android性能模式](http://t.cn/RZJaz5I)
	
	老美新年放假归来，官方更新了16集与Android性能优化相关的视频《 Android Performance Patterns》视频已运至墙内，主题为“New year, new initiative” 详细查看[G+社区](http://t.cn/RZt1F4S) 和 [Google探讨Android性能模式的16个视频总结](http://www.infoq.com/cn/news/2015/01/google-android-performance?utm_campaign=infoq_content&utm_source=infoq&utm_medium=feed&utm_term=global&utm_reader=feedly#0-tsina-1-92503-397232819ff9a47a7b7e80a40613cfe1)

1. [打造Android流式布局和热门标签](http://www.imooc.com/view/237?from=itblog)

	本课程将带大家通过自定义ViewGroup实现流式布局，课程详细介绍了自定义控件需要掌握的步骤，每个步骤相关方法的作用、调用时机的讲解以及编写。在完成自定义ViewGroup编写后，实战应用于热门标签（包括动态添加）的显示。

### 设计

### 工具

1. [SketchSquares](https://github.com/abynim/SketchSquares)

	一个将Sketch的layers自动替换为Instagram照片的插件。
		
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)