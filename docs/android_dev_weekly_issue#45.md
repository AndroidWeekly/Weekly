layout: post
title: "Android开发技术周报 Issue#45"
date: 2015-08-18 22:11:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#45

### 教程

1. [实战解析Android架构设计原则](http://www.csdn.net/article/2015-08-20/2825506?utm_source=androidweekly.cn)

	好的软件设计必须能够帮助开发者发展和扩充解决方案，保持代码清晰健壮，并且可扩展，易于维护，而不必每件事都重写代码。面对软件存在的问题，必须遵守SOLID原则，不要过度工程化，尽可能降低框架中模块的依赖性。

1. [Android 6.0 中新的新技术](http://www.race604.com/whats-new-in-android6.0/)

	最近 Google 正式发布了 Android M，并命名为“棉花糖”（Marshmallow），对于开发者来说，有哪些新的技术和变化呢？本文尝试总结一下 Android 6.0（API 23）给开发者带来新的技术和改变。权限管理是 Android M 最大的改变，权限管理更加精细，并且由以前的安装时静态授权，改为现在的运行时动态授权。大家对 Android 的权限吐槽已久，Android 应该能极大的改善这方面的问题。

1. [Android NestedScrolling 实战](http://www.race604.com/android-nested-scrolling/)

	从 Android 5.0 Lollipop 开始提供一套 API 来支持嵌入的滑动效果。同样在最新的 Support V4 包中也提供了前向的兼容。有了嵌入滑动机制，就能实现很多很复杂的滑动效果。在 Android Design Support 库中非常总要的 CoordinatorLayout 组件就是使用了这套机制，实现了 Toolbar 的收起和展开功能。
	
1. [Glide 一个专注于平滑滚动的图片加载和缓存库](http://www.jianshu.com/p/4a3177b57949?utm_campaign=maleskine&utm_content=note&utm_medium=writer_share&utm_source=weibo)

	在图片加载库烂大街的今天，选择一个适合自己使用的图片加载库已经成为了每一个Android开发者的必经之路。现在市面上知名的图片加载库有UIL,Picasso,Volley ImageLoader,Fresco以及我们今天的主角Glide。它们各有千秋，不能评定谁一定比谁好，只能说哪一个更适合你。

1. [深入讲解Android中Activity launchMode](http://droidyue.com/blog/2015/08/16/dive-into-android-activity-launchmode/)

	Android系统中的Activity可以说一件很赞的设计，它在内存管理上良好的设计，使得多任务管理在Android系统中运行游刃有余。但是Activity绝非启动展示在屏幕而已，其启动方式也大有学问，本文讲具体介绍Activity的启动模式的诸多细节，纠正一些开发中可能错误的观点，帮助大家深入理解Activity。

1. [Android实现炫酷SVG动画效果](http://blog.csdn.net/crazy__chen/article/details/47728241)

	svg是目前十分流行的图像文件格式了,svg严格来说应该是一种开放标准的矢量图形语言，使用svg格式我们可以直接用代码来描绘图像，可以用任何文字处理工具打开svg图像，通过改变部分代码来使图像具有交互功能，并可以随时插入到HTML中通过浏览器(如火狐浏览器)来观看。使用svg格式可让你设计激动人心的、高分辨率的Web图形页面。

1. [Android Hook神器：XPosed入门与登陆劫持演示](http://www.csdn.net/article/2015-08-14/2825462)

	Xposed是一款可以在不修改APK的情况下影响程序运行的框架服务，基于Xposed能够制作出许多功能强大的模块，且在功能不冲突的情况下同时运作。在本文中，作者详细介绍了Xposed的操作步骤以及登陆劫持实战演练。

### 代码&开源库

1. [SimpleCropView](https://github.com/IsseiAoki/SimpleCropView)

	一个Android的图片裁剪库，使用简单，易于定制。

1. [ColoringLoading](https://github.com/recruit-lifestyle/ColoringLoading)

	一个用纯代码实现自动绘画效果动画的项目。

1. [YouTubePlayerActivity](https://github.com/TheFinestArtist/YouTubePlayerActivity)

	一个可以播放YouTobe视频的Activity，支持屏幕旋转、声音控制、播放失败处理、可以自定义Activity关闭动画以及在横屏播放的时候自动隐藏status bar。

1. [MixtureTextView](https://github.com/hongyangAndroid/MixtureTextView)

	支持Android图文混排、文字环绕图片等效果的TextView。

1. [TransitionPlayer](https://github.com/XMFE-TEAM/TransitionPlayer)

	一个 Transition 动画控制控制库，可以让你很轻松的创建一个可交互的动画。
	
1. [android-ActionQueue](https://github.com/liaohuqiu/android-ActionQueue)
	
	Action Queue 用于执行有次序的队列操作，比如按次序弹出对话框，这在 Android 中尤其有用。

1. [SlidingCard](https://github.com/mxn21/SlidingCard)

	漂亮的卡片滑动翻页特效。

1. [WhorlView](https://github.com/Kyson/WhorlView)

	一个炫酷的漩涡加载效果自定义View。

1. [SimplifyReader](https://github.com/SkillCollege/SimplifyReader)

	一款基于Google Material Design设计开发的Android客户端，包括新闻简读，图片浏览，视频爽看 ，音乐轻听以及二维码扫描五个子模块。

### 工具

1. [lantern](https://github.com/getlantern/lantern)

	Lantern是一个免费的科学上网工具。它能帮助你随时随地快速、可靠、安全地访问互联网。

1. [GitUp](https://github.com/git-up/GitUp)

	GitUp是一个可视化的Git客户端，能够实时的进行编辑、合并、回滚等多种操作，更多功能，请下载体验。

1. [GradleDependenciesHelperPlugin](https://github.com/ligi/GradleDependenciesHelperPlugin)

	Gradle 依赖自动补全插件。

1. [android-selector-intellij-plugin](https://github.com/importre/android-selector-intellij-plugin)

	可以根据指定颜色生成Selector Drawable的插件。

### 视频

1. [Android 性能模式 第二季(中字幕)](http://www.youku.com/playlist_show/id_26016201.html)	

----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)