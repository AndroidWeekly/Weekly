layout: post
title: "Android开发技术周报 Issue#56"
date: 2015-11-10 12:34:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#56

### 新闻

1. [未来已来 Solve for X首次登陆亚洲](http://t.cn/RU89ZVy)

	你一定听说过这些项目：由泪液量测血糖值的智能隐形眼镜，针对无法上网地区提供网路服务的热气球计划，以及为手术提高效率、减低成本的纳米机器人。这些多年前听起来像是科幻小说的项目现在都已实现，而它们皆来自于Solve for X。

### 教程

1. [Android快捷方式解密](http://www.jianshu.com/p/dc3d04337d00)

	Android快捷方式作为Android设备的杀手锏技能，一直都是非常重要的一个功能，也正是如此，各种流氓App也不断通过快捷方式霸占着这样一个用户入口。同时，各大国产ROM和Luncher的崛起，让这个桌面之争变的更加激烈。毕竟大家都只想用户用自己的App资源，所以，现在各大App不仅仅是要抢占入口，同时还要和各大ROM斗智斗勇。

1. [Kotlin在Android中的应用](http://qq157755587.github.io/2015/11/14/kotlin-in-android/)
	
	最近公司新开发了一个新App，android程序员就我一个人，爱咋写咋写~~于是我尝试用Kotlin完成了这个App。开发过程中越来越感动……太好用了！！！解决了android开发中的好多痛点！

1. [Android UI：机智的远程动态更新策略](http://segmentfault.com/a/1190000003984408)

	做过Android开发的人都遇到过这样的问题：随着需求的变化，某些入口界面通常会出现 UI的增加、减少、内容变化、以及跳转界面发生变化等问题。每次发生变化都要手动修改代码，而入口界面通常具有未读信息提醒这样的“小红点”逻辑；一旦UI变化，“小红点”逻辑也要重新计算。如果不同的RD来维护这些代码，耦合性非常高，出错概率也很大。本文以自选股的个人页卡为例（界面如下图所示），并给出了一套方案来解决动态更新UI的问题以及更好的解决未读提醒的逻辑。

1. [如何准确评测Android应用的流畅度？](http://segmentfault.com/a/1190000003991467)

	怎样获取SM值？通过测量应用的帧率FPS并不能准确评价App的流畅度，FPS较低并不能代表当前App在UI上界面不流畅，而1s内VSync这个Loop运行了多少次更加能说明当前App的流畅程度。那么我们可以直接在App代码中通过Choreographer的回调FrameCallback来计算Loop被运行了几次，从而知道应用的流畅度。但在实际情况下我们不一定能修改代码（实际发布的版本不允许加入测试代码）或者根本拿不到代码（譬如和竞品进行对比）。

1. [内存泄露从入门到精通三部曲之排查方法篇](http://t.cn/RU8aIjj)

	重复多次操作关键的可疑的路径，从内存监控工具中观察内存曲线，是否存在不断上升的趋势且不会在程序返回时明显回落。这种方式可以发现最基本，也是最明显的内存泄露问题，对用户价值最大，操作难度小，性价比极高

1. [当dex分包遇上NoClassDefFoundError&ClassNotFoundException](http://t.cn/RU8acdX)

	本文记录的是：国庆节前夕，解决Crash率高达9.08%问题成功避免加班拿3倍工资的故事 PS: 除了在时间上两者相遇外，本文中提到的两个(top1&top2)crash问题与dex分包并没有关系

1. [如何实现携程动态加载插件中对aapt的改造](http://blog.csdn.net/lzyzsd/article/details/49768283)

	前几天，携程无线部门开源了他们的插件框架，使用该框架可以方便的实现app的插件化开发和热更新。 很多同学都很关心这里应该怎么修改aapt来实现为不同的插件工程指定不同的PackageID，这里我来分析一下aapt的源码，提供一个大概的思路吧

1. [ViewPager不为人知的秘密](http://www.jianshu.com/p/80891d0185f7)

	关于控制ViewPager的翻页，在网上已经有很多解决方法了，我们一个个来看看。通过控制isCanScroll变量，设置给scrollTo()方法，控制是否能滑动，看上去非常完美，实际上是最不靠谱的方法，因为你setScanScroll()调用之后状态就无法再修改这个状态了，甚至是setCurrentItem方法都不能调用了。

1. [浅谈Hybrid技术的设计与实现](http://web.jobbole.com/84121/)

	随着移动浪潮的兴起，各种APP层出不穷，极速的业务扩展提升了团队对开发效率的要求，这个时候使用IOS&Andriod开发一个APP似乎成本有点过高了，而H5的低成本、高效率、跨平台等特性马上被利用起来形成了一种新的开发模式：Hybrid APP。

1. [在Android 6.0 设备上动态获取权限](http://maoruibin.github.io/技术/2015/11/10/android_m_permission.html)

	众所周知，Android 6.0 相比之前的Android版本有一个很大的不同点，就是动态获取权限。今天自己在做拨号功能时，正巧遇到这个问题， 顺手记录下在Android 6.0 上如何动态获取权限。

1. [Android中Canvas绘图基础详解](http://blog.csdn.net/iispring/article/details/49770651)

	Android中，如果我们想绘制复杂的自定义View或游戏，我们就需要熟悉绘图API。Android通过Canvas类暴露了很多drawXXX方法，我们可以通过这些方法绘制各种各样的图形。Canvas绘图有三个基本要素：Canvas、绘图坐标系以及Paint。Canvas是画布，我们通过Canvas的各种drawXXX方法将图形绘制到Canvas上面，在drawXXX方法中我们需要传入要绘制的图形的坐标形状，还要传入一个画笔Paint。

1. [Android Design Support Library 的 代码实验——几行代码，让你的 APP 变得花俏](http://www.jianshu.com/p/1078568e859f)

	令人惊讶的是，在 Android 应用中材料设计是不容易实现的，因为材料设计的 UI 组件 如: Floating Action Button (FAB) 在低于 Android L 系统上是不可用的。我们只能选择使用由独立开发者公布出来的第三方库。

### 代码&开源库

1. [Nuwa](https://github.com/jasonross/Nuwa)

	女娲（Nuwa），可以热修复Android应用，可以加快编译。参考Qzone，纯JAVA实现，支持Dalvik和ART虚拟机，提供SDK http://t.cn/RUWLWpQ 和 Gradle Plugin http://t.cn/RUWLWpH

1. [KLog](https://github.com/ZhaoKaiQiang/KLog)

	这是一个Android专用的LogCat工具，主要功能为打印行号、函数调用、Json解析、点击跳转等。灵感来自Logger。

1. [DoubanMovie-React-Native](https://github.com/fengjundev/DoubanMovie-React-Native)

	一个用React Native写的豆瓣电影客户端。

1. [BlurImageView](https://github.com/wingjay/BlurImageView)	
	一个可以由模糊慢慢渐近显示为清晰图的控件。

1. [WheelView-Android](https://github.com/lantouzi/WheelView-Android)
	
	一个刻度滚轮控件。

1. [Highlight](https://github.com/hongyangAndroid/Highlight)

	一个用于app指向性功能高亮的库。

1. [MaterialColdStart](https://github.com/DreaminginCodeZH/MaterialColdStart)

	一个增强冷启动体验的库。

1. [CharacterPickerView](https://github.com/alafighting/CharacterPickerView)

	可实现三级联动的选择器，高仿iOS的滚轮控件。
	
### 技术之外

1. [从工程师到产品经理——转变（1）](http://www.jianshu.com/p/6fcee7aa30d1)

	从2014年以工程师身份踏入互联网行业以来，无论是平时和一线研发工程师交流抑或是面试应聘者，经常遇到工程师或者设计师朋友想转行做产品经理的情况；碰巧此时现在已接近2015年底，再过两个月便是我从一名Android研发工程师转为一名移动产品经理年满一年的日子，遂决定在这个时刻写下这个系列的文章和大家分享一名90后工程师转为移动产品经理这一年中的所思所想。

----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh3)