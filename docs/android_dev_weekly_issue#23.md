3---
layout: post
title: "Android开发技术周报 Issue#23"
date: 2015-03-14 14:13:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#23

### 教程

1. [Android精选话题讨论与面试题集锦](https://github.com/android-cn/interview-questions)

	由[@Trinea](http://weibo.com/trinea?nick=Trinea)发起的，大家的共同参与和维护，目前“Android 面试题集锦及解答” 已有 63 个 Issues，近 400 Star。另外我们将一部分精彩话题移到“Android 精选话题讨论”下讨论 [http://t.cn/RwgpkQh](http://t.cn/RwgpkQh) 每天逛 GitHub 会成为更多开发的习惯。

1. [RecyclerView Bug：IndexOutOfBoundsException: Inconsistency detected. Invalid item position 解决方案](http://drakeet.me/recyclerview-bug-indexoutofboundsexception-inconsistency-detected-invalid-item-position-solution)

	使用 RecyclerView 加官方下拉刷新的时候，如果绑定的 List 对象在更新数据之前进行了 clear，而这时用户紧接着迅速上滑 RV，就会造成崩溃，而且异常不会报到你的代码上，属于RV内部错误。初次猜测是，当你 clear 了 list 之后，这时迅速上滑，而新数据还没到来，导致 RV 要更新加载下面的 Item 时候，找不到数据源了，造成 crash。

1. [使用Androguard进行Android APK逆向工程系列](http://www.technotalkative.com/part-1-reverse-engineering-using-androguard/)
	
	Androguard使用Python写的一系列逆向工具集，功能很强大哦，对逆向工程感兴趣的小伙伴可以这个系列。
	
1. [如何不重打包调试Android应用](http://appscan.360.cn/blog/?p=73)	
	安全工程师在进行Android逆向的时候常常会有动态调试的需求，由于厂商对外发布的APP都是release版，发布产品时都会将debuggable设置为 false，使第三方不能直接调试分析APP。目前流行的方法是修改APK的 AndroidManifest.xml 将 android:debuggable 设置为 true，再重新打包签名，操作较简单，但如果碰到做了自校验加固的APK包，还要去除APK的自校验才能重打包成功，对安全人员的逆向水平和技术要求又提高了不少。
		
1. [自己动手开发Drozer插件之AutoAttack](http://appscan.360.cn/blog/?p=45)

	Drozer是MWR Labs开发的一款针对Android系统的安全测试框架。Drozer可以通过与Dalivik 虚拟机,以及其它应用程序的IPC端点以及底层操作系统的交互，避免正处于开发阶段，或者部署于你的组织的android应用程序和设备暴露出不可接受的安全风险。

1. [使用Android studio分析内存泄露](http://www.jianshu.com/p/c49f778e7acf?utm_campaign=maleskine&utm_content=note&utm_medium=writer_share&utm_source=weibo)

	Android使用java作为平台开发，帮助了我们解决了很多底层问题，比如内存管理，平台依赖等等。然而，我们也经常遇到OutOfMemoey问题，垃圾回收到底去哪了？

1. [Android Proguard 详解](http://blog.csdn.net/banketree/article/details/41928175)

	Java代码是非常容易反编译的。为了很好的保护Java源代码，我们往往会对编译好的class文件进行混淆处理。ProGuard是一个混淆代码的开源项目。它的主要作用就是混淆，当然它还能对字节码进行缩减体积、优化等，但那些对于我们来说都算是次要的功能。

1. [提交library项目到 Maven Central](http://linroid.com/2015/03/13/upload-android-library-to-moven-central/)

	将FilterMenu提交到GitHub后，在README.md的Getting Started里仅仅写上 `Download the source to use it as library project` 这唯一使用途径，居然没有gradle/maven?作为Android Studio的忠实用户，自己写的库怎么能只提供这么麻烦的方法！！！于是决定把它提交到Maven Central中,并写下这篇。

1. [使用Android Studio阅读整个Android源码](http://www.cnblogs.com/qianxudetianxia/p/3721202.html)

	之前一直在windows下用source insight阅读android源码，效果非常好。后来远程异地服务器，网络限制，一直用ssh + vim，现在主要还是以这种方式。最近发现一个不错的东西（早就有了），在android源码中有这么一个目录development/tools/idegen。顾名思义，是生成ide的project文件，主要是生成intellij的project文件，当然夜可用于android studio。使用之后，发现效果超棒，所以这里专门撰文推荐。

1. [Android 开发最佳实践](https://github.com/futurice/android-best-practices/blob/master/translations/Chinese/README.cn.md)

	之前推荐过英文的，最近由[@andyiac](https://github.com/andyiac)同学翻译成了中文版，特此在推荐一下。摘要：1.使用 Gradle 和它推荐的工程结构；2.把密码和敏感数据放在gradle.properties；3.不要自己写 HTTP 客户端,使用Volley或OkHttp库；4.使用Jackson库解析JSON数据；5.避免使用Guava同时使用一些类库来避免65k method；6.limit（一个Android程序中最多能执行65536个方法）；7.使用 Fragments来呈现UI视图。

1. [使用Chrome来调试你的Android App](http://stormzhang.com/android/2015/03/05/android-debug-use-chrome/)

	个人一直对Chrome情有独钟，Chrome除了更快之外，对开发者的支持更友好。内置强大的Developer Tools，相信Web开发简直爱不释手！而且Chrome Store里提供各种各样的插件，没有你用不到，只有你想不到。现在任何事基本Chrome全部办的到，有时候就在想，如果可以用Chrome调试Android App该多方便，而如今Facebook刚刚开源了一个工具Stetho，从此Chrome调试Android不再是梦。

### 代码&开源库

1. [GridPasswordView](https://github.com/Jungerr/GridPasswordView)

	仿微信/支付宝的密码输入框效果。
	
	![image](https://camo.githubusercontent.com/2518e5bbafa0db8e9785488b80d08c7e05387a03/687474703a2f2f6a756e676572722e71696e6975646e2e636f6d2f6465766963652d323031352d30332d31342d3138333833352e676966)
	
1. [Taurus](https://github.com/Yalantis/Taurus)

	下拉刷新的动画好赞。
	
	![image](https://camo.githubusercontent.com/3a24e22eb3f8338573dba0701c089c12f6b70f11/68747470733a2f2f6431337961637572716a676172612e636c6f756466726f6e742e6e65742f75736572732f3132353035362f73637265656e73686f74732f313632333133312f746f7572732d70756c6c2d616972706c616e655f322d322d332e676966)
	
1. [android-UniversalMusicPlayer](https://github.com/googlesamples/android-UniversalMusicPlayer)

	官方Sample，一款播放器，UI和交互都超级棒，而且同时支持手机、平板和Android Wear。

	![image](https://raw.githubusercontent.com/googlesamples/android-UniversalMusicPlayer/master/screenshots/phone.png)

1. [FilterMenu](https://github.com/linroid/FilterMenu)

	效果很赞的圆形菜单。

1. [DevelopQuickSetting](https://github.com/kyze8439690/DevelopQuickSetting)

	一个快速开启关闭开发者设置的工具，提供了app界面和桌面widget，能快速打开关闭overdraw，layout border，gpu rendering，adb wifi，不保存activity实例等功能。
	
1. [UltimateRecyclerView](https://github.com/cymcsg/UltimateRecyclerView)
	
	一个多功能的RecyclerView，包括了下拉刷新、加载更多，滑动删除，拖拽排序、多种动画、视差拖动、Toolbar渐变、Toolbar和FAB随着滚动出现消失等等效果，都可以放在同一个RecyclerVIew中并自由配置。
	
	![image](https://camo.githubusercontent.com/4b0825141b2be977b93facf8879567e3e4da4ca9/68747470733a2f2f627974656275636b65742e6f72672f6d61727368616c6368656e2f696d616765732f7261772f663437393439373464386465373161623164306630656664646461353536646637653739326466322f756c74696d61746572656379636c6572766965772f756c74696d6174655f72656379636c657276696577312e676966)	
	
1. [Material-Animations](https://github.com/lgvalle/Material-Animations)

	Android Transition动画解释说明示例。
	
### 工具	 

1. [Android Sutdio 1.2 Preview 1](http://www.androiddevtools.cn/#android-studio)

	AndroidSutdio1.2新增特性列表：反编译 debugger自动显示变量值 debugger显示变量引用 evaluation expression支持lambda和操作符运算（>>>） 性能提升 注解推断（@NotNull,@Nullable，@Contract） git历史查看。

1. [Android Apk Decompiler](http://www.decompileandroid.com)

	Android Apk Decompiler 一个在线反编译 Android APK 的工具，方便手头没有开发电脑的时候临时反编译一下APK使用。

### 新闻

1. [谷歌 Android 5.1 有什么重大更新？](http://tech2ipo.com/96327?utm_source=sinaweibo&utm_medium=sinaweibo_AD&utm_campaign=weibo)

	谷歌 Android 团队通过其官方博客发布了全新的 Android 5.1 系统更新，修复一些系统错误并新增了一些特性。Android 5.1 已经率先在谷歌发布的 Android One 入门级手机进行了升级。而目前谷歌宣布 Android 5.1 将推送给 Nexus 手机和平板电脑用户。此次更新修复了一些系统错误、支持多 SIM 卡、高清语音、引入「设备安全保护」机制以及在下拉菜单新增 Wifi 和蓝牙设置。
	
### 视频

1. [Android图像处理-打造美图秀秀从它开始](http://www.imooc.com/view/302)

	本次课程将带领大家了解Android中对图像色彩的处理和分析方法，并通过实例向大家演示市面上常见的图像处理特效的实现方法。
			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)