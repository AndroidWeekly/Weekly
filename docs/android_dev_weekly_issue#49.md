layout: post
title: "Android开发技术周报 Issue#49"
date: 2015-09-15 20:22:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#49

### 教程

1. [TextView预渲染研究](http://ragnraok.github.io/textview-pre-render-research.html)

	Android中的TextView是整个framework中最复杂的控件之一，负责Android中显示文本的大部分工作，framwork中的许多控件也直接或者间接的继承于TextView，例如Button，EditText等。其内部实现也相当复杂，单论代码行数来说，android-22中TextView有足足9509行。

1. [UI实时预览最佳实践](https://github.com/tianzhijiexian/Android-Best-Practices/blob/master/2015.9/ui/ui.md)

	之前有读者反馈说，你搞这个所谓的最佳实践，每篇文章最后就给了一个库，感觉不是很高大上。其实，我在写这个系列之初就有想过这个问题。我的目的是：给出最实用的库来帮助我们开发，并且尽可能地说明这个库是如何编写的，希望让初创公司的程序员少写点给后人留坑的代码（想必大家对此深有体会）。

1. [Facebook:我们是如何构建第一个跨平台的React Native APP](http://ljinkai.github.io/2015/09/21/facebook-react-native-android/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

	今年早些时候，我们介绍过[iOS版的React Native](https://code.facebook.com/posts/1014532261909640/react-native-bringing-modern-web-techniques-to-mobile/). React Native带来的是用web方式的React - 自声明式的UI组件和快速的开发迭代来完成手机平台的功能，然后为了保持速度、保真性、并达到原生的体验。今天我们很高兴发布[React Native的Anroid版本](http://facebook.github.io/react-native/).

1. [React-Native for Andorid 学习路程](https://github.com/yipengmu/react-native-android-lession)

	React-Native 是Android端实现实现动态部署的另一种思路，绕过dexLoad【一些现有的Android插件框架】。是在开发效率和用户体验间做的一种权衡。React-native使用JS开发，开发效率高、发布能力强。

1. [Android内存优化之OOM](http://www.csdn.net/article/2015-09-18/2825737/1#0-tsina-1-84552-397232819ff9a47a7b7e80a40613cfe1)

	Android的内存优化是性能优化中很重要的一部分，而避免OOM又是内存优化中比较核心的一点。这是一篇关于内存优化中如何避免OOM的总结性概要文章，内容大多都是和OOM有关的实践总结概要

1. [React Native for Android 入门老虎](http://www.race604.com/react-native-for-android-start/)

	昨天期待已久的 React Native for Android 发布了，赶紧来尝试一下，我跟着这个 Getting Started 开开始入门。发现被一些 “老虎” 堵在门口， Hello World 都跑不起来，入不了 React Native 的门，让我很懊恼，最后终于解决。可能大家也会遇到类似的问题，这篇文章希望能帮到你。

1. [Handler和他的小伙伴们（上）](http://www.jianshu.com/p/e04698eaba88)

	老张已过而立之年，踌躇满志，渴望浪迹互联网的英雄豪情始终在内心澎湃，终于，他走出了这一步，成立了一家互联网公司。老张凭借着这几年在互联网领域的积累和个人魅力，很快就组建了一个技术团队，作为技术出身的老张很重视公司的技术发展，因此重金请来了一位技术总监，关于技术方面的工作，老张和CTO事必躬亲。

1. [Handler和他的小伙伴们（中）](http://www.jianshu.com/p/1d03fe0b285c)

	在上一篇文章中，老张的Handler-Looper-Message模式，在他们人数不多的创业团队里收获奇效。创业的第一年，老张和CTO致力于团队基础技术平台和基础数据平台的建设，产品线也较单一，因此，简单直接而透明的管理模式最为行之有效。然而，随着业务的扩张，技术团队的壮大，这套管理模式出现了瓶颈。

### 代码&开源库

1. [AndFix](https://github.com/alibaba/AndFix)
	
	阿里开源的在线热补丁修复框架。
	
1. [fresco-processors](https://github.com/wasabeef/fresco-processors)

	一个适用于 Fresco 的图片处理器，提供了多种多样的变换效果。

1. [ParticleLayout](https://github.com/ZhaoKaiQiang/ParticleLayout)	
	左滑粒子效果。

1. [500px-guideview](https://github.com/hanks-zyh/500px-guideview)

	500px客户端引导动画效果demo。

1. [TextViewSpanClickable](https://github.com/nimengbo/TextViewSpanClickable)

	模仿微信朋友圈、QQ说说的评论的人，点赞人可点击效果.

1. [android-vts](https://github.com/nowsecure/android-vts)

	一款简单快速检测本机是否存在常见Android系统漏洞的APP。

1. [ProgressLayout](https://github.com/iammert/ProgressLayout)

	一个自定义实现的可以显示进度的布局。

1. [MaterialDateRangePicker](https://github.com/borax12/MaterialDateRangePicker)

	Material Design 风格的日期时间范围选择器。

1. [ReactAndroid](https://github.com/facebook/react-native/tree/master/ReactAndroid)
	
	Facebook开源的 React Native for Android框架。可以用JavaScript来写Android Native应用以及iOS应用。
	
1. [MaterialSearchView](https://github.com/MiguelCatalan/MaterialSearchView)	
	Material Design风格SearchView实现。

1. [fab-toolbar](https://github.com/bowyer-app/fab-toolbar)

	Floating Action Button Toolbar。

1. [FabTransitionLayout](https://github.com/bowyer-app/FabTransitionLayout)

	Floating Action Button Transition Layout。

1. [Android-Skin-Loader](https://github.com/fengjundev/Android-Skin-Loader)
	
	一个通过动态加载本地皮肤包进行换肤的皮肤框架.
	
### 工具

1. [Total Control](http://tc.sigma-rt.com.cn/index.php)

	一个手机和电脑同步显示的工具挺强大，可以多屏控制、屏幕脚本录制、自定义热键。

1. [densinator](https://github.com/robertoestivill/densinator)

	一个可以将一张图片生成不同分辨率图片的Bash脚本，支持PNG、JPG和JPEG格式的图片。

1. [DecompileApk](https://github.com/MasonLiuChn/DecompileApk)
	
	Apk一键反编译工具，可以输出 dex,jar , smali, xml, AndroidManifest.xml, res, sign 信息, umeng channel等.

### 视频	

1. [Android 开发与最佳实践系列视频](http://chinagdg.org/2015/09/android-development-patterns-series-on/)

	Android 平台的一大优势是它提供了大量基础 API、支持库，以及 Google Play Service API ，这让 Android 开发非常灵活。然而有利也有弊，太多的 API 导致开发者需要了解东西也多，特别是面对不同选择或设计决定的时候。幸运的是，我们将推出一个新的视频系列：Android Development Patterns 。这个视频系列将关注于对应用开发影响最大的基础组件和最佳实践。我们会讨论 API 设计背后的初衷，这样你就会清楚哪种方法对你是最好的选择。我们将推出许多围绕 Android framework API、支持库以及高层应用结构与设计的视频，关注 Android 核心开发。

	附：[Youtube](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc-lJo_RGGXL2Psr8vVCTWjM) 和 [优酷](http://www.youku.com/playlist_show/id_26099421.html) 链接，这些视频的字幕稍后更新。

----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)