---
layout: post
title: "Android开发周报 Issue#11"
date: 2014-12-15 13:56:36 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发周报 Issue#11
	
### 文章

1. [Google为何这样设计OnSharedPreferenceChangeListener](http://droidyue.com/blog/2014/11/29/why-onsharedpreferencechangelistener-was-not-called/)

	之前使用OnSharedPreferenceChangeListener，遇到了点小问题，就是有些时候OnSharedPreferenceChangeListener没有被触发。最近花了点时间研究了一下，小做整理。本文将会介绍监听器不被触发的原因，解决方法，以及其中隐含的一些技术细节。

1. [导入开源库到基于Android Studio构建的项目中](http://blog.isming.me/2014/12/12/import-library-to-android-studio/)

	前两天，谷歌发布了Android Studio 1.0的正式版，也有更多的人开始迁移到Android Studio进行开发。然而，网上很多的开源库,控件等还是以前的基于Eclipse进行开发，很多人不知道怎么导入到自己的基于Android Studio项目中来，微博上也有人私信我，让我来写写，正好今天回来的比较早，就写写吧。主要介绍一下常见的一些导包的场景。

1. [Android批量打包提速 - 1分钟900个市场不是梦](http://www.cnblogs.com/ct2011/p/4152323.html)
	
	使用Ant或者Gradle来给程序进行多渠道批量打包，通常都是在manifest文件中写入一个meta标签：`<meta-data android:name="CHANNEL" android:value="xxx" />` meta的key值固定，通过循环改变meta中的value值来实现市场渠道的写入。Ant批量打包实现相对麻烦，以前写的时候多亏了[谦虚的天下-《App自动化之使用Ant编译项目多渠道打包》](http://www.cnblogs.com/qianxudetianxia/archive/2012/07/04/2573687.html) 。如果没有这篇帖子，真不知道当时Ant要折腾多少回才能写好。

1. [上传Android或Java库到Maven central repository](http://blog.csdn.net/maosidiaoxian/article/details/41692535)

	主要介绍利用Sonatype将jar或aar提交到Maven的中央仓库。是不是希望将自己的jar或是aar传到maven官方库中，在The Central Repository中可以被其他人搜索使用呢，是的话，往下看吧。

<!--more-->

1. [深入解析Android的自定义布局](http://greenrobot.me/devpost/android-custom-layout/)

	这篇文章是前Firefox Android工程师（现在跳槽去Facebook了） Lucas Rocha所写，文中对Android中常用的四种自定义布局方案进行了很好地分析，并结合这四种Android自定义布局方案所写的示例项目讲解了它们各自的优劣以及四种方案之间的比较。
	
1. [Linkedin工程师是如何优化他们的Java代码的](http://greenrobot.me/devpost/java-faster-less-jvm-garbage/)

	最近在刷各大公司的技术博客的时候，我在Linkedin的技术博客上面发现了一篇很不错博文。这篇博文介绍了Linkedin信息流中间层Feed Mixer，它为Linkedin的Web主页，大学主页，公司主页以及客户端等多个分发渠道提供支撑（如下图所示）。

	
1. [跟着ym学习Android5.0](http://blog.csdn.net/column/details/android5.html)

	跟着作者一步步学习Android 5.0开发。从创建模拟器开始，再到Material主题、Palette、AnimatedVectorDrawable、RecyclerView、CardView、Activity过渡动画、如何定义阴影等。

1. [[Material Design]使用Toolbar + DrawerLayout快速实现高大上菜单侧滑](http://qichaochen.github.io/2014/12/08/108-Android-Toolbar-DrawerLayout-01/)

	如果你有在关注一些遵循最新的Material Design设计规范的应用的话（如果没有，假设你有！），也许会发现有很多使用了看起来很舒服、很高大上的侧滑菜单动画效果。

1. [安卓中的 Cydia — Xposed 框架插件专题](http://www.dgtle.com/article-5885-1.html)

	大名鼎鼎的 Xposed，相信不少经常泡在各类安卓论坛的安卓粉们都听说过。在安卓进入 4.0 的时代后，不少“大神”也都会在自己做的 Rom 中添加这个 Xposed 软件。


### 代码&开源库

1. [AndroidFastImageProcessing](https://github.com/chrisbatt/AndroidFastImageProcessing)

	A framework for speeding up image processing on android devices by taking advantage of shaders on the GPU.	

1. [loglifecycle](https://github.com/stephanenicolas/loglifecycle)

	Logs all lifecycle methods of annotated Activities, Fragments, Services, Views, etc.

1. [ParallaxEverywhere](https://github.com/Narfss/ParallaxEverywhere)

	Parallax everywhere is a library with alternative android widgets with parallax effects.
	
1. [TimelyTextView](https://github.com/adnan-SM/TimelyTextView)
	
	Animated TextView like Timely app.
	
1. [ExpandableTextView](https://github.com/Manabu-GT/ExpandableTextView)

	ExpandableTextView是一个可以使开发人员能够轻松地创建可扩展/折叠的TextView效果，就像Google Play里用于显示App描述的TextView一样.

1. [Google Samples](https://github.com/googlesamples)
	
	Google在Github上发布了大量Demo，针对不同的特性，也包含了最新的API 21 (Lollipop).
	
### 工具

1. [Android Studio 1.0正式版发布啦](http://tools.android.com/download/studio/canary/1-0rc4)
	 
	 **墙内下载地址：**[http://www.androiddevtools.cn/#android-studio](http://www.androiddevtools.cn/#android-studio)	 	 

1. [gologcat](https://github.com/airk000/gologcat)

	一个由golang编写，可以在终端中彩色输出logcat的实用工具，支持自定义颜色。
	
1. [Android 9-patch shadow generator](http://inloop.github.io/shadow4android/)

	Android点9图片阴影生成器。
	
### 视频

1. [精通Android触摸系统(中英字幕)](http://v.youku.com/v_show/id_XODQ1MjI2MDQ0.html?f=23088492)

	[@Ocean-藏心](http://www.weibo.com/oceancx?from=feed&loc=nickname)同学历经3周的翻译,将1小时18分钟的视频,终于完成了. 简介:[的姊妹篇](http://t.cn/RzxZs6E)，详细讲解了Android自定义事件处理的方方面面。配合[guolin](http://blog.csdn.net/guolin_blog/) 大神CSDN的博客和上一个视频，让你对开发Android 自定义控件游刃有余。此外还有[@Trinea](http://)大神的[Android Touch事件传递机制](http://www.trinea.cn/android/touch-event-delivery-mechanism/)简略解读。
	
	视频中用到的PPT(PDF版)下载地址：[http://wugengxin.cn/download/pdf/android/PRE_andevcon_mastering-the-android-touch-system.pdf](http://wugengxin.cn/download/pdf/android/PRE_andevcon_mastering-the-android-touch-system.pdf)

1. [Android Studio 1.0 (稳定版)的使用](http://www.jikexueyuan.com/course/396.html)

	经过 2 年时间的研发，Google 终于在近日正式发布了面向 Android 开发者的集成开发环境 Android Studio 1.0（稳定版）。Android Studio 是 Google 开发的一款面向 Android 开发者的 IDE，支持 Windows、Mac、Linux 等操作系统，基于流行的 Java 语言集成开发环境 IntelliJ 搭建而成。该 IDE 在 2013 年 5 月的 Google I/O 开发者大会上首次露面，此间推出了若干个测试版，12 月 8 日发布的版本是 Android Studio 的首个稳定版。Google 称，相对于其他开发工具，Android Studio 更快、更具生产力，Android Studio 1.0 推出后，Google 将逐步放弃对原来主要的 Android 开发工具 Eclipse ADT 的支持。

### 设计

#### 文章

1. [关于Material Design，做到这四点便足以让用户惊喜](http://www.jianshu.com/p/a3b2422b5465?utm_campaign=hugo&utm_medium=reader_share&utm_content=note&utm_source=weibo)

	Material Design 主张将现实世界中的交互体验，应用到界面设计中来，以求用户的经验能够迁移，并更快习惯新系统。Teambition 已经根据 Material Design 重新设计了旗下所有的 Android 客户端产品。在实践过程中，设计和产品团队总结了一些值得分析的要点，与大家分享。

1. [给程序员的设计学习指南](http://www.cocoachina.com/special/design/)

	这是给 移动开发者 准备的设计学习指南。在这里你将接触到三大平台的设计规范、基础设计理论，以及设计实践，还有一些学习设计的资源。程序员为什么需要学习设计？理解设计能让程序员更上一层楼，能让TA与设计师的交流协作更高效愉快，甚至拥有独立开发面向大众的APP的能力。 [《程序员需要学习设计的5大理由》](http://www.cocoachina.com/programmer/20141113/10214.html)。

1. [[无线手册-4] dp、sp、px傻傻分不清楚[完整]](http://zhuanlan.zhihu.com/zhezhexiong/19565895)

	做移动设计的同学，不管是原生app或者web app，应该对字体字号都是很头痛的问题。根本原因是，我们用唯一分辨率的电脑，设计各个不同尺寸大小分辨率的设备，那简直要疯掉了。 [[无线手册-2]不得不说的icon-font](http://zhuanlan.zhihu.com/zhezhexiong/1956455) 	[[无线手册-3] 移动App上的动画们](http://zhuanlan.zhihu.com/zhezhexiong/1956）4893)
	
#### 资源

1. [250 free icons in 5 sizes and 14 colors](http://www.androidicons.com/)
	
	包含5种尺寸和14种颜色的250个免费icons。
	
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)