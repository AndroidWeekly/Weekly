layout: post
title: "Android开发技术周报 Issue#37"
date: 2015-06-16 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#37

### 教程

1. [探索在Android中使用Emoji Font的方法](http://ragnraok.github.io/android-emoji-font-method.html)

	先说结论，在android4.4以前，无法使用像苹果那样的emoji字体样式，最简单的解决方案是使用ImageSpan配合SpannableString，而在4.4及之后的版本，则可以直接采用类似iOS/OSX的方案进行快速渲染。

1. [使用Kotlin进行Android开发](http://ragnraok.github.io/using-kotlin-to-write-android-app.html)

	Kotlin，原意是在俄罗斯的一个小岛，JetBrain在2011年推出了以这个来命名的一个运行在JVM上的语言， 看上去有点类似C#和Scala的结合，并且同为静态类型，作为一门JVM上的语言，可以轻松兼容Java，并且整个语言设计的非常轻量。目前的版本为0.12.200，尚未发布正式版。

1. [提高Android Studio中Gradle执行效率](http://blog.csdn.net/growth58/article/details/46648333)

	Android Studio使用Gradle来构建工程。目前Gradle的版本为2.2。最近的版本为2.4，性能比之前的版本有很大的提升。这有两种方式，一种是手动编辑构建文件，另一种是通过Android Studio改变配置。

1. [浅谈 MVP in Android](http://blog.csdn.net/lmj623565791/article/details/46596109)

	对于MVP（Model View Presenter），大多数人都能说出一二：“MVC的演化版本”，“让Model和View完全解耦”等等。本篇博文仅是为了做下记录，提出一些自己的看法，和帮助大家如何针对一个Activity页面去编写针对MVP风格的代码。

1. [Android应用程序UI硬件加速渲染的动画执行过程分析](http://blog.csdn.net/luoshengyang/article/details/46449677)

	 通常我们说一个系统不如另一个系统流畅，说的就是前者动画显示不如后者流畅，因此动画显示流畅程度是衡量一个系统流畅性的关键指标。为什么这样说呢？这是因为流畅的动画显示需要60fps的UI刷新速度，然而这却不是一个容易达到的速度。Android 5.0通过引入Render Thread尽最大努力提升动画显示流畅性。本文就分析Render Thread显示动画的过程，以便了解它是如何提高动画显示流畅性的。

1. [如何使用Android Studio把自己的Android library分享到jCenter和Maven Central](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2015/0623/3097.html)

	理解jcenter和Maven Central,为何有两个标准的仓库？事实上两个仓库都具有相同的使命：提供Java或者Android library服务。上传到哪个（或者都上传）取决于开发者。起初，Android Studio 选择Maven Central作为默认仓库。如果你使用老版本的Android Studio创建一个新项目，mavenCentral()会自动的定义在build.gradle中。

1. [移动Web之触摸和指针事件详解](http://www.infoq.com/cn/articles/touch-pointer-event)

	在大多数方面，触摸事件和指针事件是普通的JavaScript事件。当触摸动作发生时，触摸事件和指针事件被触发。你可以为它们指定事件处理函数，它们的事件对象也提供了有用的触摸相关的信息。触控事件和传统的鼠标、键盘事件之间有一些技术上的差异。

1. [Android4.4的init进程](http://my.oschina.net/youranhongcha/blog/469028)

	我们先概述一下Android的init进程。init是Linux系统中，用户空间的第一个进程。它负责创建系统中最关键的几个子进程，尤其是zygote。另外，init还提供了property service（属性服务），类似于windows系统的注册表服务。有关属性服务的细节，大家可参考我写的《Android Property机制》一文，本文就不多说了。

### 代码&开源库

1. [Leonids](https://github.com/plattysoft/Leonids)

	一个非常轻量的粒子效果系统库。

1. [secure-preferences](https://github.com/ophio/secure-preferences)

	安全的 SharedPreferences，可以将要存储在 SharedPreferences 的内容进行加密，而加密用的key 会通过库里自定义的 KeyGenerator 生成并存储在 [Android Keystore System](https://developer.android.com/training/articles/keystore.html#UsingAndroidKeyStore) 中。

1. [FABtransitions](https://github.com/Adirockzz95/FABtransitions)

	Floating Action Button 动画库。

1. [ApkAutoInstaller](https://github.com/bunnyblue/ApkAutoInstaller)

	Android apk自动安装sdk 基于AccessibilityService。

1. [Folder-ResideMenu](https://github.com/dkmeteor/Folder-ResideMenu)

	An extension of ResideMenu。

1. [Android-ScalableVideoView](https://github.com/yqritc/Android-ScalableVideoView)
	
	拥有像ImageView那样的多种缩放类型的VideoView。

1. [FrescoDemo](https://github.com/06peng/FrescoDemo)

	一个基于Android Design library使用Fresco来加载图片的Demo项目。

1. [Android-ItemTouchHelper-Demo](https://github.com/iPaulPro/Android-ItemTouchHelper-Demo)

	Basic example of using ItemTouchHelper to add drag & drop and swipe-to-dismiss to RecyclerView.

1. [RearrangeableLayout](https://github.com/rajasharan/RearrangeableLayout)
	
	一个可以通过拖动重新排列内部子View的布局。

1. [pocketknife](https://github.com/hansenji/pocketknife)

	Intent and Bundle "injection" library。

1. [Android-TextView-LinkBuilder](https://github.com/klinker24/Android-TextView-LinkBuilder)
	
	一个可以让你给TextView的指定文字添加点击Link的库，支持用户点击的时候可以高亮被点击的文字，支持修改高亮文字的透明度，支持通过正则表达式去匹配要添加Link的文字，支持改变Link文字的颜色等。

1. [TreeRecyclerView](https://github.com/nuptboyzhb/TreeRecyclerView)

	一个使用RecyclerView写的树结构效果。

1. [Android-StepsView](https://github.com/anton46/Android-StepsView)

	Step By Step的进度指示View，可以定义进度的颜色。

1. [AndroidEagleEye](https://github.com/MindMac/AndroidEagleEye)
	
	一个基于Xposed的Hook工具，可以对系统API和应用程序方法进行Hook，支持对需Hook API或方法的定制。

### 工具

1. [DexExtractor](https://github.com/bunnyblue/DexExtractor)

	android dex extractor ，anti-shell，android 脱壳。
			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)