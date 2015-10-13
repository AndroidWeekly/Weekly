layout: post
title: "Android开发技术周报 Issue#48"
date: 2015-09-07 21:11:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#48

### 教程

1. [深入理解Android之Gradle](http://blog.csdn.net/innost/article/details/48228651)

	Gradle是当前非常“劲爆”得构建工具。本篇文章就是专为讲解Gradle而来。介绍Gradle之前，先说点题外话。说实话，我在大法工作的时候，就见过Gradle。但是当时我一直不知道这是什么东西。而且大法工具组的工程师还将其和Android Studio大法版一起推送，偶一看就更没兴趣了。为什么那个时候如此不待见Gradle呢？因为我此前一直是做ROM开发。

1. [Java反射最佳实践](https://github.com/tianzhijiexian/Android-Best-Practices/blob/master/2015.9/reflect/reflect.md)

	最简单优雅的使用反射。因为反射在开发中很少用（做普通的业务开发的话），仅仅在自己写一些框架和注解框架时会用到，所以对api总是不熟悉。每次用到api都要去网上查，查了后又得自己实验下，很不爽。更差劲的是这样写法可读性十分低下。

1. [Android Studio中Gradle使用详解](http://www.jianshu.com/p/02cb9a0eb2a0)

	文章介绍的Gradle构建Android应用各种常用配置脚本和技巧。
	
1. [Android应用Preference相关及源码浅析(Preference组件家族篇)](http://blog.csdn.net/yanbober/article/details/47954653)

	前一篇（点我阅读前一篇《Android应用Preference相关及源码浅析(SharePreferences篇)》）我们讨论分析使用了Android的SharePreferences，相信看过的朋友都有了自己的感悟与理解，这一篇我们继续乘热打铁来说说SharePreferences的衍生品—-Preference组件。其实Preference组件大家一定不陌生，因为Android系统的Setting应用及我们市面上一些符合Android设计思想的应用的设置界面一般都会用它来实现，而且Google原生Android代码中大量的使用了Preference组件。

1. [Android应用Preference相关及源码浅析(SharePreferences篇)](http://blog.csdn.net/yanbober/article/details/47866369)

	在我们开发Android过程中数据的存储会有很多种解决方案，譬如常见的文件存储、数据库存储、网络云存储等，但是Android系统为咱们提供了更加方便的一种数据存储方式，那就是SharePreference数据存储。其实质也就是文件存储，只不过是符合XML标准的文件存储而已，而且其也是Android中比较常用的简易型数据存储解决方案。

1. [Android分包MultiDex原理详解](http://blog.csdn.net/yzzst/article/details/48290701)

	当Android系统安装一个应用的时候，有一步是对Dex进行优化，这个过程有一个专门的工具来处理，叫DexOpt。DexOpt的执行过程是在第一次加载Dex文件的时候执行的。这个过程会生成一个ODEX文件，即Optimised Dex。执行ODex的效率会比直接执行Dex文件的效率要高很多。

### 代码&开源库

1. [telescope](https://github.com/mattprecious/telescope)

	一个方便你在项目中进行Bug报告和捕获的工具库。

1. [Dividers](https://github.com/Karumi/Dividers)

	一个方便你给RecyclerView创建分割线的库。

1. [jOOR](https://github.com/jOOQ/jOOR)

	一个帮你摆脱反射的繁琐代码的库，链式调用，一行代码就可以反射。

1. [DraggableView](https://github.com/elevenetc/DraggableView)

	这是一个可拖拽的，并在拖拽的时候有旋转、倾斜和缩放的效果的自定义View。

1. [Bugtags-Android](https://github.com/bugtags/Bugtags-Android)

	一个简单和高效的Bug报告工具，可在当前界面上添加带有Bug信息的Tag来标记Bug问题。

1. [PickerUI](https://github.com/DavidPizarro/PickerUI)

	防iOS的滚轮选择器效果的自定义View，并且支持背景模糊效果。

1. [ExpandableLayout](https://github.com/AAkira/ExpandableLayout)
	
	一个可展开的Layout。

1. [CountryCodePicker](https://github.com/chathudan/CountryCodePicker)

	一个国家码选择器，支持选择和搜索，并且可以获取到已经选择的国家的名称，编码，货币和拨号代码。

1. [Search](https://github.com/lurbas/Search)

	VIPER架构的实战项目。

1. [frenchtoast](https://github.com/pyricau/frenchtoast)

	Toast的一种新的实现，摒弃了原生Toas的诸多缺点，例如不能很好的控制它的出现以及持续时间、打乱上下文以及API设计的不合理，容易出错等缺点，它通过为每一个Toast创建一个新的Window来实现真正的Toast。

### 工具

1. [Snapdrago Profiler](https://developer.qualcomm.com/software/snapdragon-profiler)

	Snapdrago Profiler是一款Android App分析调试工具，能够在单一用户界面中同时显示功耗、温度曲线、网络使用和CPU、GPU及内存性能，它还支持Android跟踪数据的分析调节。

1. [Bugtags](http://bugtags.com)

	新一代的、专为移动测试而生的缺陷发现及管理工具。

1. [qark](https://github.com/linkedin/qark)

	LinkedIn开源的静态分析工具QARK，该工具用于分析那些用Java语言开发的Android应用中的潜在安全缺陷。

### 书

1. Android开发艺术探索
	
	《Android开发艺术探索》由[@任玉刚Coder](http://weibo.com/uc83018062)所著，是一本Android进阶类书籍，采用理论、源码和实践相结合的方式来阐述高水准的Android应用开发要点。《Android开发艺术探索》从三个方面来组织内容。第一，介绍Android开发者不容易掌握的一些知识点；第二，结合Android源代码和应用层开发过程，融会贯通，介绍一些比较深入的知识点；第三，介绍一些核心技术和Android的性能优化思想。全书基于Android 5.0，采用理论、源码和实践相结合的方式来阐述高水准的Android开发技术，让你深入理解Android开发艺术。
		
	购买地址：[目录和样章](http://pan.baidu.com/s/1pJL1WCj) [京东](http://item.jd.com/1709011859.html) [China-pub](http://product.china-pub.com/4806147) 

1. Android群英传 

	购买地址：[京东](http://item.jd.com/11758334.html) [亚马逊](http://www.amazon.cn/Android群英传-徐宜生/dp/B01481RAA4/ref=sr_1_1?m=A1AJ19PSB66TGU&s=books&ie=UTF8&qid=1442198757&sr=1-1&keywords=android群英传) [天猫](https://detail.tmall.com/item.htm?spm=a1z10.3-b.w4011-10017777404.30.jLLTe3&id=521663212917&rn=f1a753af2af55796f958950f8074f229&abbucket=17)

	本书作者[@Tomcat的猫](http://weibo.com/u/1904977584)，曾就职于上海TCL通讯，从事Alcatel（阿尔卡特）Android手机系统的定制工作，目前就职于上海沪江网Android开发部RD项目组，负责沪江App的功能预研。《Android群英传》对具有一定Android开发基础的读者，以通俗易懂的语言介绍了Android开发的进阶技巧。《Android群英传》共分为13章，讲解了Android体系与系统架构、Android开发工具新接触、Android控件架构与自定义控件详解、ListView使用技巧、Android Scroll分析、Android绘图机制与处理技巧、Android动画机制与使用技巧、Activity与Activity调用栈分析、Android系统信息与安全机制、Android性能优化、搭建云端服务器、Android 5.X新特性详解、Android实例提高。《Android群英传》最后通过实例来展示如何实际实践这些技巧，让读者更好地体会如何提高Android开发。

	购买地址：[京东](http://item.jd.com/11758334.html) [亚马逊](http://www.amazon.cn/Android群英传-徐宜生/dp/B01481RAA4/ref=sr_1_1?m=A1AJ19PSB66TGU&s=books&ie=UTF8&qid=1442198757&sr=1-1&keywords=android群英传) [天猫](https://detail.tmall.com/item.htm?spm=a1z10.3-b.w4011-10017777404.30.jLLTe3&id=521663212917&rn=f1a753af2af55796f958950f8074f229&abbucket=17)

### 视频	

1. [GDG 字幕组的成品列表](https://www.gitbook.com/book/gfansub/pub/details)

	目前 GDG 字幕组有来自国内外的翻译志愿者 30 余位，翻译了 Udacity 以及 GDS 频道等众多英文技术视频，目前我们也在[招募更多翻译志愿者](http://www.gfansub.com/join_translator)，如果您与我们一样，希望为 Google 的技术，开放开源的技术贡献一份力量的话，请加入我们，我们已经等了很久了

----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)