---
layout: post
title: "Android开发技术周报 Issue#16"
date: 2015-01-19 13:48:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#16
	
### 教程

1. [Android性能优化之过渡绘制(一)](http://www.androidperformance.com/android-performance-optimization-overdraw-1.html)
	
	首先将讲解一下GPU过渡绘制，也是开发者最直接接触的部分吧，这个内容将分为两个部分来将讲，第一部分初步讲解一下gpu过渡绘制的原理，和一些优化建议，第二部分将用实际例子来讲解优化GPU过渡绘制的一般步骤。

1. [Android性能优化之过渡绘制(二)](http://www.androidperformance.com/android-performance-optimization-overdraw-2.html)

	这篇文章从实战的角度，讲解了一个过渡绘制的优化过程。当然这里用到的只是很少的一部分，毕竟每个应用差别很大，优化方式也各不一样。所以这篇文章仅供参考，想把这块做好还是要下功夫的。不过令我比较欣慰的是，在公司内推行这个优化之后，我们Flyme内部的自带应用已经做得很好了，当然还是有不少界面有优化的空间，但总体还是比较满意的。

1. [Android Studio系列教程六--Gradle多渠道打包](http://stormzhang.com/devtools/2015/01/15/android-studio-tutorial6/)
	
	由于国内Android市场众多渠道，为了统计每个渠道的下载及其它数据统计，就需要我们针对每个渠道单独打包，如果让你打几十个市场的包岂不烦死了，不过有了Gradle，这再也不是事了

<!--more-->

1. [你不可不知的10个Github功能](http://www.kuqin.com/shuoit/20141118/343265.html)

	Github深受开发者们喜爱，不过有很多Github功能还是不为大多数人熟知，有的，你可能从来没用过；有的，可能见过，却从未正真了解过。这里慧都控件网为大家收集了10个不可不知的Github功能。

1. [ListView小知识整理：滑动背景、Item间隙等](http://www.imooc.com/wenda/detail/243880)

	在Android中，ListView是最常用的一个控件，在做UI设计的时候，很多人希望能够改变一下它的背景，使他能够符合整体的UI设计，改变背景很简单只需要准备一张图片，然后指定属性 android:background="@drawable/bg"，不过不要高兴地太早，当你这么做以后，发现背景是变了，但是当你拖动，或者点击 list空白位置的时候发现ListItem都变成黑色的了，破坏了整体效果，这是为什么呢？

1. [Android性能优化课程翻译（一）：渲染性能](http://lzyblog.com/2015/01/13/Android性能优化课程翻译（一）：渲染性能/)
	
	渲染性能意味着你可以有多快的速度绘制你的activity并让它在屏幕上刷新出来。这里的性能良好指的是你的用户感觉你的应用程序是流畅的，并且是快速响应的，这意味着你必须在16ms甚至更少的时间来完成所有的逻辑和渲染操作，但实际上这可能比你想象的要困难一些。

	
1. [Android应用监听自己是否被卸载，做反馈统计](http://lzyblog.com/2015/01/09/Android应用监听自己是否被卸载，做反馈统计/)
	
	最近做项目的时候碰到这样一个需求：用户卸载应用后提供反馈信息以便更好的改进软件，并统计卸载量。Android可以监听卸载广播，得到什么应用被卸载了，但是系统并没有提供监听自己卸载的方法，于是乎，在网上找了一些方法，根据自己需求做了些修改，最后完成这个需求。
	
1. [Square开源库OkHttp的分析和使用系列教程](http://lzyblog.com/tags/OkHttp/)

	HTTP是目前很多应用的网络连接方式，通过它我们可以交换数据和媒体。有效的使用HTTP会使你的应用获得更快的加载速度，并且更节约带宽。OKHttp就是为这个目标应运而生的。
	
1. [每个程序员都应该了解的内存知识【第一部分】](http://www.oschina.net/translate/what-every-programmer-should-know-about-memory-part1?print)
	
	早期计算机比现在更为简单。系统的各种组件例如CPU，内存，大容量存储器和网口，由于被共同开发因而有非常均衡的表现。例如，内存和网口并不比CPU在提供数据的时候更（特别的）快。曾今计算机稳定的基本结构悄然改变，硬件开发人员开始致力于优化单个子系统。于是电脑一些组件的性能大大的落后因而成为了瓶颈。

### 代码&开源库

1. [Pull-to-Refresh.Rentals-Android](https://github.com/Yalantis/Pull-to-Refresh.Rentals-Android)

	一个动画效果很赞的下拉刷新的控件。
	
	![image](https://camo.githubusercontent.com/d406ac5a03a2b1fa5cf41fadc8d2408cb8709bdc/68747470733a2f2f6431337961637572716a676172612e636c6f756466726f6e742e6e65742f75736572732f3132353035362f73637265656e73686f74732f313635303331372f7265616c6573746174652d70756c6c5f312d322d332e676966)

1. [Side-Menu.Android](https://github.com/Yalantis/Side-Menu.Android)

	一个动画效果很赞的侧滑菜单库。
	
	![image](https://camo.githubusercontent.com/cb6caa7a392d01d46bca9d9485c01fc173f55fac/68747470733a2f2f6431337961637572716a676172612e636c6f756466726f6e742e6e65742f75736572732f3132353035362f73637265656e73686f74732f313638393932322f6576656e74732d6d656e755f312d312d362e676966)

1. [Context-Menu.Android](https://github.com/Yalantis/Context-Menu.Android)

	一个动画效果很赞的上下文菜单库。
	
	![image](https://camo.githubusercontent.com/46c15734b552ce3afefa7efd1518909046b4677e/68747470733a2f2f6431337961637572716a676172612e636c6f756466726f6e742e6e65742f75736572732f3132353035362f73637265656e73686f74732f313738353237342f39396d696c65732d70726f66696c652d6c696768745f312d312d342e676966)

1. [WaniKani-for-Android](https://github.com/xiprox/WaniKani-for-Android)
	
	一个做的很棒的学习日本汉字的App.

1. [KitKatEmoji](https://github.com/crossle/KitKatEmoji) (推荐人[@CrossleSong](http://www.weibo.com/songxiaoming))

	Android KitKat emoji表情库
	
	![image](https://raw.githubusercontent.com/crossle/KitKatEmoji/master/KitKatEmoji-sample/preview.gif)

1. [Slidr](https://github.com/r0adkll/Slidr)
	
	一个方便你为Activity添加滑动后关闭的库。
	
	![image](https://raw.githubusercontent.com/r0adkll/Slidr/master/images/slidr_gif.gif)
	
1. [GifImageView](https://github.com/felipecsl/GifImageView)

	Android原生的ImageView是不能显示Gif图片，而这个GifImageView对ImageView进行了扩展可以显示Gif图片。

1. [Android-RoundCornerProgressBar](https://github.com/akexorcist/Android-RoundCornerProgressBar)

	一个漂亮的圆角水平进度条。

	![image](https://raw.githubusercontent.com/akexorcist/Android-RoundCornerProgressBar/master/image/header.jpg)
	
1. [picasso-transformations](https://github.com/TannerPerrien/picasso-transformations)
	
	适用于Picasso图片加载库的图片转场动画库。
	
1. [ChipsLibrary](https://github.com/AndroidDeveloperLB/ChipsLibrary)

	在Android EditText中实现打Tag功能.

	![image](https://camo.githubusercontent.com/304547454e09fa27bcc5dea41a8572d8d96ba219/68747470733a2f2f6c68332e676f6f676c6575736572636f6e74656e742e636f6d2f2d307469445852646a4539772f55454b53526455615336492f41414141414141416f71772f746874634b4d5753574b732f773339332d683638332d6e6f2f706e672e706e67)
	
1. [glide-transformations](https://github.com/wasabeef/glide-transformations)

	适用于Glide图片加载库的图片转场动画库。
	
	![image](https://raw.githubusercontent.com/wasabeef/glide-transformations/master/art/demo.gif)
	
### 工具	 	 

1. [Android Studio 1.1 Preview 1](http://www.androiddevtools.cn)

	本次主要更新：
	
	1. 在新建项目的时候创建的launcher图标会被作为@mipmap资源代替@drawable资源。
	2. Link检查工具增加一些检查规则。
	3. 增加Android Wear的watch faces模版。
	4. 捉了许多只🐛。


### 视频

1. [Android属性动画赏析](http://www.imooc.com/view/263?from=itblog)

	动画几乎是一个好的App所不可缺少的一部分，它体现了一种更友好的交互方式，在iOS、Android L中动画的使用越来越多，特别是后者更是着重强调设计更好的动画。从3.0开始，Android就提供了一种更为强大的属性动画框架。本次课程，将向你介绍如何使用属性动画做出更好的动画

### 设计

### 工具

1. [FontPair](http://fontpair.co)

	一个帮助设计师挑选Google字体的网站。
		
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)