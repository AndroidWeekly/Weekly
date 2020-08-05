layout: post
title: "Android开发技术周报 Issue#39"
date: 2015-07-08 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#39

### 新闻

1. [Google 收购 Android 十周年，多图看 Android 十年间的变迁](http://www.pingwest.com/ten-years-after-google-acquired-android/)

	往事一回首，十年就过去了。由于 Google 当年是悄悄地做了这笔收购交易，所以外界其实没有多数人知道 Google 收购 Android 的具体时间点。按照维基百科上“Google 公司收购列表”这个词条上给出的信息，Google 是在 2005 年 8 月 17 日收购了 Android；现在看上去，维基百科上的这个日期恐怕要修改了一下了。

1. [谷歌黑莓联手开发企业版安卓系统](http://tech.163.com/15/0710/08/AU5BJ0OF000915BE.html)

	近日谷歌和黑莓走得更近了，两家公司宣布将会联手创造一款更符合企业需求的安卓操作系统。该系统将会注重黑莓BES12企业设备部署服务与安卓5.0 Lollipop和Google Play的整合。

1. [Android M 开发者预览版 2 漏洞曝光](http://www.oschina.net/news/64138/android-m-2-vulnerability)

	谷歌公布了Android M开发者预览版2，在第一个版本基础上修复了不少BUG，同时也带来了一些新特性，这些我们早上已经有报道。尽管如此，到现在有不少网友发现了该版本并不稳定，依然存在一些漏洞。

### 教程

1. [Android Data Binding初探和代码实战](http://www.aswifter.com/tags/Data-Binding/)

	今年的Google IO大会，给Andorid开发者带来了很多新东西，比如新的Material Design支持库，还有Data Binding技术，使用Data Binding，我们可以很方便的实现 MVVM设计模式。

1. [Android ViewDragHelper完全解析 自定义ViewGroup神器](http://blog.csdn.net/lmj623565791/article/details/46858663)

	在自定义ViewGroup中，很多效果都包含用户手指去拖动其内部的某个View(eg:侧滑菜单等)，针对具体的需要去写好onInterceptTouchEvent和onTouchEvent这两个方法是一件很不容易的事，需要自己去处理：多手指的处理、加速度检测等等。

1. [Android安全输入设计与思考](http://blog.csdn.net/yzzst/article/details/46741681)

	本文对市面上的Android安全键盘进行了总结，详细分析了为什么采用安全键盘，怎么样实现安全键盘等问题。以及各个产品线使用的安全键盘有何优劣点。以方便开发者对自我开发安全项目键盘进行总结与学习。

1. [给初学者的 Android 加密工具](http://www.oschina.net/translate/android-cryptography-tools-for-beginners)

	越来越多的黑客盯上了移动应用，每天都会增加，因为移动应用中有黑客感兴趣的东西，如用户数据。硬编码（Hard-coded，注，固定写死，不能修改的）安全秘钥，SD 卡中以明文存放的个人信息，数据库中未加密存储的用户名和密码，收集的分析（analytics）并以明文方式发到远程服务器，这些情况都使得攻击更容易（得手）。

1. [浅谈Android开放网络端口的安全风险](http://drops.wooyun.org/mobile/6973)

	Android应用通常使用PF_UNIX、PF_INET、PF_NETLINK等不同domain的socket来进行本地IPC或者远程网络通信，这些暴露的socket代表了潜在的本地或远程攻击面，历史上也出现过不少利用socket进行拒绝服务、root提权或者远程命令执行的案例。特别是PF_INET类型的网络socket，可以通过网络与Android应用通信，其原本用于linux环境下开放网络服务，由于缺乏对网络调用者身份或者本地调用者pid、permission等细粒度的安全检查机制，在实现不当的情况下，可以突破Android的沙箱限制，以被攻击应用的权限执行命令，通常出现比较严重的漏洞。
	
1. [Android内核开发：从源码树中删除出厂的app应用](http://ticktick.blog.51cto.com/823160/1671438)
	
	上一篇文章中提到过，系统出厂的app应用，其实就是被安装到/system分区的app，这些app在Android源码树中被编译后打包到了system.img镜像中，系统启动时，以只读的方式挂载/system目录，因此，非root手机用户是无法删除这些app的。
	
### 代码&开源库

1. [letterpress](https://github.com/Pixplicity/letterpress)

	一个方便你在App中应用自定义字体的库。

1. [TourGuide](https://github.com/worker8/TourGuide)

	一个可以让你很方便的给App添加操作提示导航的库。

1. [ParallaxSwipeBack](https://github.com/bushijie/ParallaxSwipeBack)

	带视觉差的侧滑返回，类似于新版微信和lofter的侧滑返回效果。

1. [Android-Download-Manager-Pro](https://github.com/majidgolshadi/Android-Download-Manager-Pro)

	一个可以并行执行下载任务的管理器。

1. [ListItemFold](https://github.com/dodola/ListItemFold)

	很赞的LsitView折叠效果。

1. [AnimatedCircleLoadingView](https://github.com/jlmd/AnimatedCircleLoadingView)

	加载动画效果很赞的加载控件。

1. [fit-chart](https://github.com/txusballesteros/fit-chart)

	Fit Chart is an Android view similar to Google Fit wheel chart.
	一个类似Google Fit里环形图表控件。

1. [storio](https://github.com/pushtorefresh/storio)

	一个流式接口的Sqlite库。

1. [android-percent-support-extend](https://github.com/hongyangAndroid/android-percent-support-extend)

	对于android-percent-support的扩展库。

1. [android_dbinspector](https://github.com/infinum/android_dbinspector)

	一个可以让你在App内查看应用的自己数据库内容的库。

1. [ThreeTenABP](https://github.com/JakeWharton/ThreeTenABP) ([@hi大头鬼hi](http://weibo.com/2092500601))	
	
	Jake 大神开源的一个把Java8 的Date包移植到Android中来的库，主要就是替换joda。Java 8 date api的主要设计者就是joda的创建者，新的API对joda做了不少改进。另外移植过来的包大小比joda小，api数目也少，值得试试。

### 工具

1. [Android Studio with Android NDK Preview Support Available](http://tools.android.com/tech-docs/android-ndk-preview)

	We've just release Android Studio 1.3 RC 1 to the canary channel, which includes the preview of Android NDK C/C++ support!（不能翻墙可以点[这里](http://photo.weibo.com/2319578217/wbphotos/large/mid/3863147439838716/pid/8a41f469jw1etxxge1t6yj21kw4a8e81))

1. [Android Library Finder](https://github.com/cesarferreira/alfi)

	ALFI（Android Library Finder）——最快的方式获取依赖库。

1. [Android-DPI-Calculator](https://github.com/JerzyPuchalski/Android-DPI-Calculator)

	Android Studio plugin allowing to calculate sizes in different densities like xxxhdpi, xxhdpi, xhdpi, hdpi, mdpi, ldpi and tvdpi.

1. [兰贝壳儿](http://www.orchidshell.com/)	
	兰贝壳儿是一个辅助安卓开发的 eclipse 插件工具。主要提供三个功能：自动打包多渠道包的apk、项目工程文件或文件夹在资源管理器中打开、工程依赖的其他jar包管理（使用maven的dependency格式）。
			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)