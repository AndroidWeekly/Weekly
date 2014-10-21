---
layout: post
title: "Android开发周报 Issue#3"
date: 2014-10-15 10:48:14 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发周报 Issue#3


### 文章

1. [Instagram工程师教你如何改善App的性能](http://www.csdn.net/article/2014-10-05/2821953-instagram-improved-their-apps-performance)

	扁平化设计由于其简洁的外表，更少的按钮和选项使得界面干净整齐，从而减少认知障碍的产生。扁平化设计更是功能上的简化于与重组，相比于拟物化而言，扁平风格的一个优势就在于它可以更加简单直接的将信息和事物的工作方式展示出来。本文来自Instagram一名工程师的分享。

1. [AppCompat V21：将 Materia Design 兼容到5.0之前的设备](http://blog.csdn.net/xushuaic/article/details/40212327)

	本篇文章翻译自Chris Banes(就职于Google，工作内容 Android Developer Relations team)，android 5.0今天发布。在很多很棒的更新中，包括了新的UI组件和创建 Material Design 主题的能力。为了使你能够将新的设计中更新到旧的系统中，我们同时更新了包含 AppCompat 的support libraries。在这篇文章中，我将总体说明一下appCompat的新特性并介绍一下如何应用于你的app中。

1. [Android中Activity启动过程探究](http://www.codeceo.com/article/android-activity-start.html)

	文章从源码一步步分析了Android中Activity的启动过程，步骤很详细。

1. [如何高效利用GitHub](http://www.yangzhiping.com/tech/github.html)

	正是Github，让社会化编程成为现实。本文尝试谈谈GitHub的文化、技巧与影响。

1. [跨终端Emoji](http://slides.ngot.me/emoji/index.html#0)

	由孢子社区 - 庄恒飞分享了饱子社区在跨终端Emoji表情上的一些实践经验。	
	
<!--more-->

1. [优化Android App性能？十大技巧必知！](http://blog.csdn.net/qijianke2014/article/details/40041331)
	
	无论锤子还是茄子手机的不断冒出，Android系统的手机市场占有率目前来说还是最大的，因此基于Android开发的App数量也是很庞大的。那么，如何能开发出更高性能的Android App？相信是软件开发公司以及广大程序员们头疼的一大难题。

1. [Android开发之多级下拉列表菜单实现（仿美团，淘宝等）](http://blog.csdn.net/minimicall/article/details/39484493)

	我们在常用的电商或者旅游APP中，例如美团，手机淘宝等等，都能够看的到有那种下拉式的二级列表菜单，我相信很多人都想开发一个跟它一样的功能放到自己的APP中。作者首先分析了该效果的组成结构，然后通过LinearLayout＋ToggleButton＋PopupWindow实现了类似的效果。

1. [Android 实现形态各异的双向侧滑菜单](http://blog.csdn.net/lmj623565791/article/details/39670935)

	关于自定义控件侧滑已经写了两篇了，今天决定把之前的单向改成双向，当然了，单纯的改动之前的代码也没意思，今天不仅会把之前的单向改为双向，还会多添加一种侧滑效果，给大家带来若干种形态各异的双向侧滑菜单，不过请放心，代码会很简单，然后根据这若干种，只要你喜欢，相信你可以打造任何绚（bian）丽（tai）效果的双向侧滑菜单。

### 代码&开源库


1. [ Google I/O App](https://github.com/google/iosched)

	源码已经更新到SDK5.0了，http://t.cn/RvouJFP， 对于最终的Android 5 SDK的更新，包括删除所有产品风格缺陷 使用appcompat和android.support.v7.widget.Toolbar带来更多的# material design兼容到Lollipop之前的设备 更新导航抽屉分层等

1. [FireEye](https://coding.net/u/yoojia/p/FireEye/git)

	Android校验库 - Fire Eye 简单易用的Android校验库。 这是一个简单Android校验库，按配置来验证用户输入的表单信息。 只需要几行代码，即可验证用户输入，并且将验证错误反馈给用户。 它内置了大量常用的验证类型，足以满足你的功能需求。 它还有一个可扩展的验证选项，你可以通过扩展接口添加你需要的验证方式。

1. [multi-column-list-adapter](https://github.com/twotoasters/multi-column-list-adapter)
	
	MultiColumnListAdapter是一个CursorAdapter的子类，它可以使你的ListView看起来像一个GridView，并且还可以给列表添加header和footer。
	
1. [hellocharts-android](https://github.com/lecho/hellocharts-android)

	一个兼容API 8+(Android 2.2)图表库，当硬件加速可用的时候工作状态最好，因此推荐在API 14+(Android 4.0)以上使用。
	
1. [tickplusdrawable](https://github.com/flavienlaurent/tickplusdrawable)

	通过canvas rotation + line translations实现的I/O 2014 app中对号和加号切换的效果。

### 小技巧

1.一行命令检查代码是否有addJavascriptInterface安全隐患([@杨辉__](http://weibo.com/p/1005051869137113))

	grep -r -n -i --include=*.java addJavascriptInterface *  

### 视频

1. [ From Holo to Material](http://v.youku.com/v_show/id_XODA1ODAyNzc2.html)

	介绍了如何从现有的Holo风格升级到Material风格以及在升级的过程中需要注意的地方等待。

1. [ What's new in Android 5.0 Lollipop ](http://v.youku.com/v_show/id_XODA1ODY5NTYw.html)

	介绍了Android 5.0 Lollipop的新特性。
	
### 新闻

1. [Android 5.0正式版发布，代号“棒棒糖”](http://www.infoq.com/cn/news/2014/10/android-5.0-release)

	Android L是Google在今年6月份的Google I/O开发者大会上正式推出的最新Android系统。近日，Google发布了Android L的正式版即Android 5.0，该版本延续了此前甜品命名的传统，命名为Lollipop（棒棒糖）。Android的主管 Sundar Pichai在Google官方博客中写道，Lollipop是Android迄今为止最重大的版本更新，在用户视觉、用户体验、功能等方面都有重大的改进。Lollipop最明显的改变是采用了全新的设计语言，被称之为“Material Design”。
. 

### 设计

#### 文章

1. [Creating Your First Prototype with Framer](https://medium.com/@kennycheny/creating-your-first-prototype-with-framer-c39221da7668)

	一步步教你在Framer Studio中创建自己的第一个交互原型.
	
#### 工具&资源
	
1. [Material Design的图标](https://github.com/google/material-design-icons)

	伴随着Android 5.0 Lollipop（棒棒糖）的发布，Google也在Github开源了Material Design的图标, 包含多种尺寸。主要包含了：
	
	* SVG versions of all icons in both 24px and 48px flavours
	* SVG and CSS sprites of all icons
	* 1x, 2x icons targeted at the Web (PNG)
	* 1x, 2x, 3x icons targeted at iOS (PNG)
	* Hi-dpi versions of all icons (hdpi, mdpi, xhdpi, xxhdpi, xxxhdpi) (PNG)
	
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)