---
layout: post
title: "Android开发周报 Issue#4"
date: 2014-10-27 15:42:14 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发周报 Issue#4


### 文章

1. [Android系统性能调优工具介绍](http://blog.csdn.net/innost/article/details/9008691)

	在软件开发过程中，想必很多读者都遇到过系统性能问题。而解决系统性能问题的几个主要步骤是：
	
	* 测评：对系统进行大量有针对性的测试，以得到合适的测试数据。
	* 分析系统瓶颈：分析测试数据，找到其中的hotspot（热点，即bottleneck）。
	* 性能优化：对hotspot相关的代码进行优化。

1. [The introduction to Reactive Programming you've been missing -- 中文版](https://github.com/jsenjoy/introrx-chinese-edition)	

	什么是FRP?在互联网上有着一大堆糟糕的解释与定义。维基百科一如既往的空泛与理论化。Stackoverflow的权威答案明显不适合初学者。Reactive Manifesto看起来是你展示给你公司的项目经理或者老板们看的东西。微软的Rx terminology "Rx = Observables + LINQ + Schedulers" 过于重量级且微软味十足，只会让大部分人困惑

1. [Android Lollipop 新特性 - Palette](http://baoyz.com/android/2014/10/21/android-palette-use/)

	Palette 可以从一张图片中提取颜色，我们可以把提取的颜色融入到App UI中，可以使UI风格更加美观融洽。比如，我们可以从图片中提取颜色设置给ActionBar做背景颜色，这样ActionBar的颜色就会随着显示图片的变化而变化。


1. [Android 使用动态加载框架DL进行插件化开发](http://blog.csdn.net/t12x3456/article/details/39958755)
	
	随着应用的不断迭代，应用的体积不断增大,项目越来越臃肿,冗余增加.项目新功能的添加，无法确定与用户匹配性，发生严重异常往往牵一发而动全身,只能紧急发布补丁版本，强制用户进行更新.结果频繁的更新，反而容易降低用户使用黏性.或者是公司业务的不断发展,同系的应用越来越多,传统方式需要通过用户量最大的主项目进行引导下载并安装.
	
<!--more-->


### 代码&开源库

1. [dex-method-counts](https://github.com/mihaip/dex-method-counts)

	一个可以统计 `.dex` 文件中方法个数的命令行工具。
	
1. [smali2java](https://github.com/demitsuri/smali2java)

	可以将smali代码转换为java代码的工具。

1. [MaterialDesignLibrary](https://github.com/navasmdc/MaterialDesignLibrary)

	可以让你在2.2系统上使用Android L系统才支持的控件效果的库。具体兼容的控件请看项目的介绍。

1. [enhanced-volley](https://github.com/vinaysshenoy/enhanced-volley)
	
	enhanced-volley是在Volley的基础上进行了扩展，添加了 `自定义Http头` 、`自定义GET请求的URL参数` 、`给ImageLoader添加了默认的BitmapLruCache实现` 、`添加了新的可以执行任意你想要的动画的AnimateImageView控件` 以及支持 `application/octet-stream MIME 类型的文件上传` 等功能。

### 小技巧

1. Android Studio / Intellij Tip of the Day：显示最近更改的文件(@[Philippe Breault](https://www.google.com/+PhilippeBreault))

	快捷键（菜单）： 
	- Mac：Cmd的+ Shift键+ E 
	- Windows / Linux：CTRL + SHIFT + E 


### 工具

1. [manifestreplace-plugin](https://github.com/castorflex/manifestreplace-plugin)

	Gradle plugin to add more placeholders to your manifest.xml.

### 设计

#### 文章

1. [IOS机Android切图标注与命名规范](http://www.ui.cn/project.php?id=28848)

	在项目迭代的过程中，会碰到很多切图替换的问题，怎么去命名？给几个分辨率合适？怎么去标注等。本文把我在版本迭代工作中的一些经验分享给大家，希望能对大家有所作用。


1. [图标设计初阶要先型](http://cdc.tencent.com/?p=8239)

	UI最重要组建之一就是图标，随着扁平化设计的发展趋势，越来越注重图标的简洁与寓意表达，平面图标已占主导地位。每位设计师所处的阶段所关注的要点是不一样的，我把图标设计分为2个阶段–初阶与高阶，这样分是为了有步骤性的学习和进阶的加强，当然，能人的话一步到位，对于新人来讲会较难，需要实际工作中辅导与自己经验总结。
	

#### 工具&资源
	
1. [Material Design UI Kit for Sketch](https://www.behance.net/gallery/20514895/Material-Design-UI-Kit)
	
	A UI Kit for Google's Material design. Essential if you're designing for Android.
	
1. [Icons8 App](http://icons8.com/app/)	

	* Quick search through the icons
	* Compatible with Photoshop, Xcode and more
	* 5000 icons for iOS 7, Windows 8 and Android
	
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)