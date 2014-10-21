---
layout: post
title: "Android开发周报 Issue#2"
date: 2014-1012 10:48:14 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发周报 Issue#2


### 文章

1. [Andriod Studio科普篇](http://blog.csdn.net/maosidiaoxian/article/category/2380095)

	作者记录了自己在使用Android Studio时做的一些个性化设置，踩到的一些坑等等。

1. [美团Android自动化之旅—生成渠道包](http://tech.meituan.com/mt-apk-packaging.html)
	
	文章介绍了三种打渠道包的方式。目前，Android团队打包基本使用第三种方式，完成了打包的自动化，解放了工程师的生产力，善哉善哉。打包的问题解决了，但有时候还需要为不同的渠道定制不同的APK。	
1. [美团Android自动化之旅—适配渠道包](http://tech.meituan.com/mt-apk-adaptation.html)

	文章介绍了如何使用Android构建利器Gradle的flavor特性来定制渠道包。
	
1. [如何把Android手机变成一个WIFI下载热点? — 报文转发及DNS报文拦截](http://tech.meituan.com/packet_forwarding.html)	
	
	随着wifi的普及，移动运营商的热点也越来越多了，如中国移动的CMCC、中国电信的ChinaNet、中国联通的ChinaUnicom等，一般来说，连上此类的热点，打开浏览器上网时都会自动跳转到一个验证页面，最近有个项目也有类似的需求，Android手机自建热点，别的手机wifi连接此热点，打开浏览器，输入任意内容，自动跳转到一个下载列表页面，点击相应的链接即可下载相应的文件。
	
1. 	[Android通过Wifi来调试你的应用](http://stormzhang.github.io/posts.html#Activity)

	在Android中调试我们经常要用一根USB数据线连接到手机和电脑，一方面麻烦不说，手机一直连着电脑充电时间长了对手机也是一种伤害，另一方面如果哪一天忘记带USB数据线就很悲催了。今天就来教大家一种通过wifi来连接手机调试的方法，瞬间高大上有木有？而且不需要root，以后你就可以隔空给你公司的测试妹子安装/卸载apk了。

1. [Activity生命周期详解系列](http://stormzhang.github.io/posts.html#Activity)

	文章第一部分结合官方的Activity生命周期流程图讲解了各个生命周期方法的执行顺序，第二部分结合一些特定的使用场景分析了Activity的生命周期，第三部分讲解了onSaveInstanceState和onRestoreInstanceState这两个方法的作用。

<!--more-->

### 代码&开源库

1. [android-combination-avatar](https://github.com/kongnanlive/android-combination-avatar)

	网易工程师实现的模仿QQ讨论组头像叠加效果的控件

	![image](https://github.com/kongnanlive/android-combination-avatar/raw/master/screenshots/screenshot1.jpg)

1. [RoboSpock](https://github.com/Polidea/RoboSpock) 

	RoboSpock是一个Android的测试框架，它可以让你非常快的在JVM上运行单元测试，而无需启动任何仿真器或进行任何部署。
	
1. [android-signaturepad](https://github.com/gcacace/android-signaturepad)

	一个可以平滑的绘制签名的自定义View。
	
	![image](https://github.com/gcacace/android-signaturepad/raw/master/header.png)
	
1. [android-simple-storage](https://github.com/sromku/android-simple-storage)

	这个库可以让你使用简单的Api在内部或者外部磁盘空间上创建、读取、删除、附加、加密文件等等。

1. [ZhihuPaper](https://github.com/cundong/ZhihuPaper)

	一个「知乎日报」Android 客户端
	
	![image](https://raw.githubusercontent.com/cundong/ZhihuPaper/master/screenshot/one.png)

1. [Smart App Updates](https://github.com/cundong/SmartAppUpdates)

	Android App 增量更新实例

1. [cerberus](https://github.com/chalup/cerberus)

	Android library for detecting and reporting long running SQLite queries.
	
1. [AKParallax-Android](https://github.com/ideaismobile/AKParallax-Android)

	一个可以为ScrollView或者ListView添加视差滚动效果的库。
	
1. [Android-Icon-Fonts](https://github.com/johnkil/Android-Icon-Fonts)

	Material和Holo风格的图标字体.
	
	![image](https://raw.githubusercontent.com/johnkil/Android-Icon-Fonts/master/Art/android-icon-fonts.png)

1. [SmoothProgressBar](https://github.com/castorflex/SmoothProgressBar)

	平滑的进度条。
	
	![image](https://raw.githubusercontent.com/castorflex/SmoothProgressBar/master/screenshots/SPB_sample.gif)

1. [SystemBarTint](https://github.com/jgilfelt/SystemBarTint)

	Apply background tinting to the Android system UI when using KitKat translucent modes。
	
	![image](https://camo.githubusercontent.com/fbbeaab2048f78e2d4974bb1559544c9f22eccae/68747470733a2f2f7261772e6769746875622e636f6d2f6a67696c66656c742f53797374656d42617254696e742f6d61737465722f73637265656e73686f742e706e67)	


1. [Emoticons-Keyboard](https://github.com/chiragjain/Emoticons-Keyboard)

	带表情情符号的自定义键盘。
	
	![image](https://raw.githubusercontent.com/chiragjain/Emoticons-Keyboard/master/s2.png)
	![image](https://raw.githubusercontent.com/chiragjain/Emoticons-Keyboard/master/s3.png)

### 工具

1. [Android Studio 0.8.12 Released](http://www.androiddevtools.cn)

	主要更新：
	
	* 一个全新的AVD管理器，新的AVD管理器与IDE的集成更紧密了。例如，当你试图去运行一个App时，你可以快速直接地从运行对话框中创建Nexus5或7的Nexus AVD。在这个新的AVD列表里，你可以查看和编辑AVD（你可以看到每个AVD使用多少磁盘空间），你也可以启动AVD等。你还可以很容易在现有的这些默认基础硬件上创建新的AVD，而且，在不同的类别，如手机，平板电脑，耐磨，电视。一旦你选择了硬件，你可以配置特定的架构和Android版本。最后，你可以选择一个显示名称，默认方向，GPU/快照选项 - 或者更高级的设置，例如外部存储等大小。
	* 当创建新的项目，我们现在默认使用HTTPS而不是HTTP的Gradle wrapper。我们还增加了一个lint（和的quickfix）警告如何在现有项目中使用HTTP。
	* 如果你喜欢手动编辑配置XML文件（使用XML编辑器，而不是图形化的布局编辑器），你现在可以通过点击版面编辑或布局预览窗口上方工具栏中的选项图标，并选择“首选的XML编辑器“，一旦选择了，新创建的布局将在XML编辑器中打开，而不是在布局编辑器中打开。
	* 翻译编辑器现在可以在字符串编辑器中工作了。
	* Android项目视图现在是默认选择。您可以通过右键点击上面的项目视图的下拉列表切换回普通的项目视图。
	* 现在，您可以在XML中使用的quickfix导入工具命名空间：`tools：` 前缀，然后IDE将提供插入相应的命名空间声明,同样，`Android：` 前缀它导入了Android的命名空间，而不是显示所有可用的命名空间，并要求你选择一个.
	* 一些Bug修复 

1. [Emmagee](https://github.com/NetEase/Emmagee/releases)		
	Emmagee是网易推出的一个实用的、便利的Android App性能测试工具，Emmagee推出了2.0版本，作为一次重大的升级，2.0版本主要在UI以及用户体验上做了优化，同时提供国际化的支持(感谢国际用户的反馈)，希望本次更新给各位带来更优质的用户体验。

1. [GT](http://gt.tencent.com/index.html)

	 GT（随身调）是APP的随身调测平台，它是直接运行在手机上的“集成调测环境”(IDTE, Integrated Debug&Test Environment)。利用GT，仅凭一部手机，无需连接电脑，您即可对APP进行快速的性能测试(CPU、内存、流量、电量、帧率/流畅度等等)、开发日志的查看、Crash日志查看、网络数据包的抓取、APP内部参数的调试、真机代码耗时统计等等；更重要的是，您可以在任意真实场所、任何时候做如上的系列事情，这就是“APP的场测”。如果您觉得GT提供的功能还不够满足您的需要，您还可以利用GT提供的基础API自行开发有特殊功能的GT插件（目前，仅iOS版支持），帮助您解决更加复杂的APP调试、测试问题。 

### 视频

1. [微信Android客户端架构演进及其对开发流程的影响](http://www.infoq.com/cn/presentations/android-client-architecture-evolution-and-impact-on-development-process#0-tsina-1-70270-397232819ff9a47a7b7e80a40613cfe1)

	微信ANDROID客户端的架构演进史，可以说是一个典型ANDROID应用在从小到大的成长过程中的“踩坑”与“填坑”的历史。从1.0版本安装包的354KB，到今天5.3版本的24.1MB，从最开始两三个码农的突击作业，到今天的“集团军”开发力量，微信的体量在不断增大，开发同学遇到的“成长的烦恼”也越来越多： 为什么微信收消息又延迟了？

### 书

1. [50 Android Hacks](http://www.it-ebooks.info/book/2445/)

	这本书分12部分介绍了50个Android开发中的小技巧。

### 新闻

1. [谷歌发布x86 64位Android L模拟器](http://cn.engadget.com/2014/10/09/google-android-l-64-bit/)

	【Google Android L 模拟器已经准备好了，开发者可以开发 64 位应用】Google 公布了 x86 64-bit Android L developer preview 的模拟器映像档已经开放给开发者下载，让有意的开发者可以准备着手开发新世代的应用程序。

### 设计

#### 文章

1. [图标设计之尺规作图全过程](http://www.ui.cn/project.php?id=26650)

	国外上年纪大品牌的Logo都是尺规作图做出来的，因为最开始电脑不发达的时候，制作标志都是手工做的，没有尺规制图，没法制作。后来这些品牌出名了，Logo成为了典范，尺规作图也成了一个logo规范与否的标准。
	
1. [Photoshop Actions & Workflows](http://bjango.com/articles/actions/)
	
	文章介绍了自己在过去的几年里建立了一套自己每天都在使用的Photoshop Actions以及工作流程。

1. [My app design workflow](http://bjango.com/articles/appdesignworkflow/)
	
	作者完整的介绍了自己在做iOS，Android和Mac的应用程序设计的工作流程，从你第一次打开Photoshop开始，到应用程序发布。
	
1. [Understanding Material Design](https://medium.com/android-design/latest)

	作者分Material is the metaphor、Authentic Motion和Skeuomorphism vs Flat Design这个三个主题分析讲解了自己对Material Design的理解。

1. [导航抽屉到底归属于哪个层级?](http://zhuanlan.zhihu.com/TingTalk/19865937)

	当导航抽屉成为 Google 设计规范的一部分时, Google 明确告诉我们该这么做, 而且提供了可以让开发者直接调用的工具.难道说 Google 在一开始的时候犯了个错误? 也许第一眼看上去这样做是对的, 但是从规范上看来确实是有些问题的.
	
1. [2014交互设计工具革新之年](http://www.ui.cn/project.php?id=17636)

	在这一年里，我们见到了很多新颖的交互设计工具和原型设计工具。工具旨在提高我们的工作效率，改善我们的工作流程，诸多新兴的工具造就了相关的讨论团体和设计，且这些工具，大大缩短了设计成本，现在，高保真的原型设计更简便了。

1. [如何看待 Google 让自家应用的 iOS 版与 Android 版统一使用 Material Design ？](http://www.zhihu.com/question/25812945/answer/31495421)

	国内例如 腾讯QQ 等一些 App 的 Android版 完全照搬 iOS 版的 UI ，这个一直饱受很多同学的诟病，如今 Google 刚好反过来了，把自家 App 的 iOS 版刻意做的和 Android 版一致。


#### 工具
	
1. [SubScribe](http://www.astutegraphics.com/software/subscribe/)

	一款增强绘图功能的AI插件，这个插件能轻易解决直线和圆、圆与圆的精准相切[外切内切]等问题。
	
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)