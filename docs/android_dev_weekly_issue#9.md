---
layout: post
title: "Android开发周报 Issue#9"
date: 2014-12-01 12:42:08 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发周报 Issue#9
	
### 文章

1. [Dalvik虚拟机Java堆创建过程分析](http://blog.csdn.net/luoshengyang/article/details/41581063)

	使用C/C++开发应用程序最令头痛的问题就是内存管理。慎不留神，要么内存泄漏，要么内存破坏。虚拟机要解决的问题之一就是帮助应用程序自动分配和释放内存。为了达到这个目的，虚拟机在启动的时候向操作系统申请一大块内存当作对象堆。之后当应用程序创建对象时，虚拟机就会在堆上分配合适的内存块。而当对象不再使用时，虚拟机就会将它占用的内存块归还给堆。Dalvik虚拟机也不例外，本文就分析它的Java堆创建过程。

1. [为什么Android的图片质量会比iPhone的差？](http://www.kuqin.com/shuoit/20140826/341828.html?url_type=39&object_type=crawler&pos=1)

	经常看到有人问：“安卓版微信发出去的图片怎么那么渣！比iPhone的差远了！”。不只是微信，很多应用安卓版的图片质量就是要比iPhone版逊色很多，这到底是怎么回事？

1. [[Material Design]使用Fackbook Rebound快速实现弹簧动画效果](http://qichaochen.github.io/2014/11/21/107-Facebook-Rebound-Demo/)

	Rebound是Facebook推出的一款Android的物理和动画库，于2013年10月在Mobile@Scale大会上正式发布，旨在解决笨重、缓慢的传统移动网络界面。Rebound不是一款通用物理库，但其弹簧模型在应用程序中引入了现实世界的物理，易于集成，创建的动画能够让人感觉到非常自然，并且可以和Material Design的设计原则呼应，可用于滚动条、切换开关、呼叫等场景下。

1. [使用curl来调试你的应用](http://stormzhang.com/devtools/2014/11/07/use-curl-debug/)

	我们在客户端开发过程中总免不了和后端进行api对接，有时候需要对返回的数据格式进行调试，有时候每次运行客户端来发送请求，这个未免效率太低，这里就来介绍一个好用的工具--curl。

1. [Android taskAffinity属性使用详解](http://www.codeceo.com/article/android-taskaffinity.html)

	Activity的归属，也就是Activity应该在哪个Task中，Activity与Task的吸附关系。我们知道，一般情况下在同一个应用中，启 动的Activity都在同一个Task中，它们在该Task中度过自己的生命周期，这些Activity是从一而终的好榜样。

1. [每个Android开发者必须知道的内存管理知识](http://www.codeceo.com/article/android-memory-manage.html)

	相信一步步走过来的Android从业者，每个人都会遇到OOM的情况。如何避免和防范OOM的出现，对于每一个程序员来说确实是一门必不可少的能力。今天我们就谈谈在Android平台下内存的管理之道，开始今天的主题之前，先再次回顾两个概念。

<!--more-->


### 代码&开源库

1. [android-Ultra-Pull-To-Refresh](https://github.com/liaohuqiu/android-Ultra-Pull-To-Refresh)

	很炫的下拉刷新效果库。
	
	
	![image](https://camo.githubusercontent.com/588a2ef2cdcfb6c71e88437df486226dd15605b3/687474703a2f2f737261696e2d6769746875622e71696e6975646e2e636f6d2f756c7472612d7074722f73746f72652d686f7573652d737472696e672d61727261792e676966)

1. [discreteSeekBar](https://github.com/AnderWeb/discreteSeekBar)

	![image](https://camo.githubusercontent.com/e717e2597779d1ddc980ace6f3943f62483d8a8c/68747470733a2f2f6c68332e676f6f676c6575736572636f6e74656e742e636f6d2f2d376e62565058785568596b2f56472d724f3634704d57492f414141414141414148734d2f614d52676c7432567a726b2f773633392d683438302f616e696d6174696f6e2e676966)

1. [InstaMaterial](https://github.com/frogermcs/InstaMaterial)

	Material Design风格的Instagram的客户端。

1. [materialish-progress](https://github.com/pnikosis/materialish-progress)

	Material Design风格的圆形进度条，最低支持到2.3的系统。
	
	![image](https://github.com/pnikosis/materialish-progress/raw/master/spinningwheel.gif)

1. [galgo](https://github.com/inaka/galgo)

	Android日志工具库，可以把log显示在屏幕上。
	
	![image](https://camo.githubusercontent.com/1e2d3b204a0898b697876817cc19ab4a2fef5de2/687474703a2f2f6936312e74696e797069632e636f6d2f327177336279302e676966)

1. [puree-android](https://github.com/cookpad/puree-android)

	一个Log日志收集框架。

1. [LoonAndroid](https://github.com/gdpancheng/LoonAndroid)

	一个ioc（依赖注入）框架，但是整个框架式不同于androidannotations，Roboguice等ioc框架，这是一个类似spring的实现方式。在整应用的生命周期中找到切入点，然后对activity的生命周期进行拦截，然后插入自己的功能。
	
### 工具

1. [Android Studio 1.0 Release Candidate 2](http://tools.android.com/download/studio/canary/1-0rc2)
	 
	 本次Release没有添加什么新的特性，只是修复了一些Bug，如果你之前已经升级到了RC1建议更新到RC2版。另外本次Release还针对Windows用户推出了包含SDK的安装包。
	 
	 **墙内下载地址：**[http://www.androiddevtools.cn/#android-studio](http://www.androiddevtools.cn/#android-studio)

### 设计

#### 文章

1. [什么才是优秀的用户界面设计](http://www.oschina.net/news/57379/what-is-good-ui-design#0-tsina-1-76379-397232819ff9a47a7b7e80a40613cfe1)

	本文分享一些 Good UI 在一些项目中获取的设计以及运营策略等方面的经验。Good UI 是一家研究用户体验的设计机构。我们知道成功的页面设计不仅有很高的转化率更便于用户使用，既能满足商业目标更能为用户带来良好的体验。

1. [Material Navigation Drawer sizing](https://medium.com/sebs-top-tips/material-navigation-drawer-sizing-558aea1ad266)

	本文分析了Material的抽屉导航的大小到底多少才最符合设计规范和美观。

#### 素材

1. [Android L GUI KIT](https://dribbble.com/shots/1683873-Android-L-GUI-KIT)
 	
	Android L GUI KIT。

#### 工具

1. [OVEN](http://oven.chrometaphore.com)

	A BETTER ASSETS WORKFLOW For Photoshop CC / 2014。
	
	![image](http://oven.chrometaphore.com/assets/oven_panel_screenshot@2x.png)
	
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)