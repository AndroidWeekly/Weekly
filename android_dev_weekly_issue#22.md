---
layout: post
title: "Android开发技术周报 Issue#22"
date: 2015-03-09 14:13:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#22

### 教程

1. [如何检测一个APP：从解密到批量获取他人信息](http://www.91ri.org/12472.html)

	在挖掘Android App的web端漏洞时，遇到一些看起来安全性做的比较好的应用会对http请求也会加密，这篇文章作者就提供了一个不错的基本的解决思路：反编译获取加密方式-》解密 -》添加logcat直接输出加密的内容。

1. [用Path来绘制一些图形](http://www.cnblogs.com/tianzhijiexian/p/4301113.html)

	Path是android中用来封装几何学路径的一个类，因为Path在图形绘制上占的比重还是相当大的。你可以用它来绘制各种样式的几何图形，做图表什么的都可以。

1. [用PageTransformer打造更好的动画效果](http://android.jobbole.com/80668/)

	Android的ViewPager类已经变成一个相当流行的Android应用组件了。它简单直观，并且提供了极好的功能。你可以经常在设置向导，图片画廊种看到它，它还是分开应用内容的良好方式。标准的ViewPager实现工作得非常出色，但是在Google工作的牛人创建了名为PageTransformer的类。

1. [深入理解Android之Java Security（第一部分）](http://blog.csdn.net/innost/article/details/44081147)

	从事Android工作4年以来，只有前1年不到的时间是用C++在开发东西（主要是开发DLNA组件，目前我已将它们全部开源，参考http://blog.csdn.net/innost/article/details/40216763），后面的工作几乎都在用Java。自以为Java相关的东西都见过了，可前段时间有个朋友给我花了1个多小时讲解他们某套系统的安全体系结构，其中涉及到很多专业术语，比如Message Digest（消息摘要）、Digital Signature（数字签名）、KeyStore（恕我不知道翻译成什么好，还是用英文原称吧）、CA（Certificate Authority）等。

1. [ Android最佳性能实践(三)——高性能编码优化](http://blog.csdn.net/guolin_blog/article/details/42318689)
	
	在前两篇文章当中，我们主要学习了Android内存方面的相关知识，包括如何合理地使用内存，以及当发生内存泄露时如何定位出问题的原因。那么关于内存的知识就讨论到这里，今天开始我们将学习一些性能编码优化的技巧。这里先事先提醒大家一句，本篇文章中讨论的编码优化技巧都是属于一些“微优化”，也就是说即使我们都按照本篇文章的技巧来优化代码，在性能方面也是看不出有什么显著的提升的。

1. [这些高效的Android注解，你有使用过么？](http://blog.csdn.net/icedream_hong/article/details/44103083)

	介绍几个support library 19.1中的注解:1.`Nullness annotations` 2.`Resource type annotations` 3.`IntDef and StringDef annotations`, 这几个注解在项目中非常有用，而且library本身也是用了这些注解。让我们来研究下。

1. [深入浅出RxJava(二：操作符)](http://blog.csdn.net/lzyzsd/article/details/44094895)

	在[第一篇blog](http://blog.csdn.net/lzyzsd/article/details/41833541)中，我介绍了RxJava的一些基础知识，同时也介绍了map()操作符。当然如果你并没有意愿去使用RxJava我一点都不诧异，毕竟才接触了这么点。看完这篇blog，我相信你肯定想立即在你的项目中使用RxJava了，这篇blog将介绍许多RxJava中的操作符，RxJava的强大性就来自于它所定义的操作符。

1. [Java开发者易犯错误Top10](http://www.csdn.net/article/2015-02-13/2823958)

	在Java中，有些事物如果不了解的话，很容易就会用错，如数组转换为数组列表、元素删除、Hashtable和HashMap、ArrayList和LinkedList、Super和Sub构造函数等，如果这些对你来说是陌生的，你可以在本文中了解它们。

1. [Guava 是个风火轮之基础工具(2)](http://www.jamespan.me/blog/2015/02/09/guava-basic-utilities-2/)
	
	Guava 是 Java 开发者的好朋友。虽然我在开发中使用 Guava 很长时间了，Guava API 的身影遍及我写的生产代码的每个角落，但是我用到的功能只是 Guava 的功能集中一个少的可怜的真子集，更别说我一直没有时间认真的去挖掘 Guava 的功能，没有时间去学习 Guava 的实现。

1. [配置 Android 签名的 gradle 插件](http://www.jianshu.com/p/a387269a8a43)

	使用本插件可以让所有的开发机以及持续交付设备使用完全相同的代码进行工作.
避免陷入本地配置兼容性的泥淖中, 防止私密信息泄露. 解决的问题:1.签名文件路径这样的本地信息独立配置 2.签名文件密钥与代码仓库隔离, 与开发隔离 3.便于持续交付

### 代码&开源库

1. [ZDepthShadowLayout](https://github.com/ShogoMizumoto/ZDepthShadowLayout)

	支持Z轴阴影的Layout。

	![image](https://raw.githubusercontent.com/ShogoMizumoto/ZDepthShadowLayout/master/demo.gif)

1. [Algorithms](https://github.com/pedrovgs/Algorithms)

	常见算法问题的Java实现.

1. [SpringIndicator](https://github.com/chenupt/SpringIndicator)

	模仿Morning Routine的引导页效果.
	
	![image](https://raw.githubusercontent.com/chenupt/SpringIndicator/master/img/si_1.0.0.gif)

1. [SmartProxy](https://github.com/hedaode/SmartProxy)

	安卓下的智能代理。
	
1. [GoldenGate](https://github.com/Flipboard/GoldenGate)	
	Flipboard开源一个通过注解生成类型安全的javascript bindings (Bridges)的库。

1. [palettehelper](https://github.com/hzsweers/palettehelper)

	用Kotlin实现的可以根据图片生成color palettes的android app。
	
1. [jpinyin](https://github.com/stuxuhai/jpinyin)	
	JPinyin是一个汉字转拼音的Java开源类库，在PinYin4j的功能基础上做了一些改进。
	【JPinyin主要特性】
	
	1. 准确、完善的字库；
		Unicode编码从4E00-9FA5范围及3007（〇）的20903个汉字中，JPinyin能转换除46个异体字（异体字不存	在标准拼音）之外的所有汉字；
	2. 拼音转换速度快；
		经测试，转换Unicode编码从4E00-9FA5范围的20902个汉字，JPinyin耗时约100毫秒。
	3. 多拼音格式输出支持；
		JPinyin支持多种拼音输出格式：带音标、不带音标、数字表示音标以及拼音首字母输出格式；
	4. 常见多音字识别；
		JPinyin支持常见多音字的识别，其中包括词组、成语、地名等；
	5. 简繁体中文转换
	
### 工具	 

1. [AndroidSigning](https://github.com/dodocat/AndroidSigning)

	AndroidSigning是一个可以方便你配置和管理Android签名信息的Gradle插件，使用本插件可以让所有的开发机以及持续交付设备使用完全相同的代码进行工作.避免陷入本地配置兼容性的泥淖中, 防止私密信息泄露. 

### 新闻

1. [Google 正在研发支持虚拟现实设备的安卓系统](http://www.oschina.net/news/60292/google-vr-android)

	两名熟悉谷歌虚拟现实安卓项目人士透露，在Facebook以20亿美元收购Oculus VR之后，谷歌组建了一个工程师团队来开发支持虚拟现实应用的安卓版本。他们说谷歌有“几十名工程师”及其他员工在从事这个项目。谷歌计划免费发布这个新的为虚拟现实设备定制的安卓系统。谷歌的免费策略使安卓系统成为最多人使用的智能手机系统，但谷歌为智能手表打造的安卓系统则到目前为止一直不太成功，搭载这个系统的设备销量平平
	
### 视频

1. [Analytics Academy 四套中文课程视频](http://t.cn/Rw3kQum)

	Analytics Academy 四套中文课程视频已搬到优酷 ，感兴趣的可以学习一下。Google Analytics 不仅可以做网站分析，也可以做移动分析，至少海外可用吧.教程官网:[http://t.cn/8s6kHjY](http://t.cn/8s6kHjY) 。

1. [AK(AlloyKit)—手机QQ Hybrid app 优化新思路](http://www.infoq.com/cn/presentations/alloykit-qq-hybrid-app-optimizing-ideas?utm_source=infoq&utm_medium=videos_homepage&utm_campaign=videos_row1)

	无线移动终端的兴起，引发业界 Native app 和 Web app 选型大讨论。随着终端机器性能的不断提升，结合 Web 和 Native 的 Hybrid app 在体验上逐渐得到改善和认可，并以其不可替代的快速迭代能力，在大量的场景中获得广泛的运用。如手Q 中群部落、吃喝玩乐、主题中心等核心业务。AK（AlloyKit）是一套高性能的 Hybrid Web 业务的技术架构体系，能够使 Web 项目快速拥有 Web 资源离线化、JS Api、诊断分析、自动种入登录态和续期、DNS管理、开发者工具、关键性能数据上报等特性。目前 AK 已经手机QQ、PC QQ、手机空间、手机QQ音乐 4 大平台级产品进行运用，超过 4 个 BG 的 200 个业务接入。本次分享将详细解密 AK 的核心模块实现细节。

1. [Gradle脚本的整洁之道—编写高质量的Gradle脚本](http://www.infoq.com/cn/presentations/write-high-quality-gradle-script?utm_source=infoq&utm_medium=videos_homepage&utm_campaign=videos_row1)

	本演讲介绍Gradle既可以通过Maven的约定来构建Java项目，也可以像Ant一样灵活的处理和Maven约定不一致的Java项目。虽然Gradle抛弃了冗余的XML，但是我们在使用Groovy脚本和DSL编写Gradle脚本的时候，仍然有重复代码。本演讲还介绍如何利用Gradle的特性通过Project、Task在脚本级别重用代码以及通过Plugin在项目之间重用代码，编写Clean的构建脚本。

### 设计

1. [material design学习笔记](http://colachan.com/post/3416)
	
	自从material design发布以来，可乐橙就在一直收集相关素材与资源，研究别人的作品。这套设计风格非常鲜明，带有浓郁的Google式严谨和理性哲学，深得我心。实际上，光是研究素材和别人作品，就能发现一些明显的规律，做出几分相似的设计。这样半吊子的状态一直保持到现在，最近有时间通读一遍官方的设计指南，终于有了深入的理解。在朋友的项目中实践了一番，虽然很抱歉拿朋友开刀，不过他对整体效果似乎还算满意。
			
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)