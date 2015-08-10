layout: post
title: "Android开发技术周报 Issue#42"
date: 2015-07-27 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#42

### 新闻

1. [Android Broadcast组件权限绕过漏洞](http://www.freebuf.com/articles/terminal/73885.html)

	Lolipop源码已经放出有些日子了，我发现google在Android 5.0上修复了一个高危漏洞，利用该漏洞可以发送任意广播：不仅可以发送系统保护级别的广播、还可以无视receiver的android:exported=false、android:permisson=XXX 属性的限制。

1. [安卓再曝新漏洞：可远程致使用户无法接打电话](http://www.freebuf.com/news/73755.html)

	本周堪称是安卓设备的“黑色周”，几天前刚被爆出[Stagefight媒体库上存在胜似“心脏滴血”的高危漏洞](http://www.freebuf.com/news/73411.html)，这两天安全研究人员再曝可远程致使安卓设备无法正常接打电话的最新漏洞。

### 教程

1. [如何在Android Gradle中添加原生so文件依赖](http://www.jianshu.com/p/20cee429d1c3)

	通过Maven仓库发布我们的函数库没有什么问题（只要你通过繁琐的发布流程），maven-android-plugin可以帮助我们包含共享库。Maven依赖规则使得我们可以指定想要获取的ABI（不同的CPU架构）的类型以及函数库的格式（我们的是.so格式）。

1. [Android开发中，有哪些让你觉得相见恨晚的方法、类或接口？](http://www.zhihu.com/question/33636939)

	1、Throwable接口中的getStackTrace()方法，根据这个方法可以得到函数的逐层调用地址，其返回值为StackTraceElement[]；2、StackTraceElement类，其中四个方法getClassName()，getFileName()，getLineNumber()，getMethodName()在调试程序打印Log时非常有用；3、UncaughtExceptionHandler接口，再好的代码异常难免，利用此接口可以处理未捕获的异常；

1. [关于安卓libStagefright系列漏洞分析](http://www.freebuf.com/vuls/73618.html)

	libStagefright默认会被mediaserver使用，也就是说，如果恶意的视频文件有机会被mediaserver处理到，该漏洞就有机会触发，举例：如文件管理app，如果视频被存放在sdcard，那么打开文件管理app，下拉列表到露出视频，就会触发缩略图解析，漏洞触发图库app，点击本地图片会出现缩略图，如果视频在sdcard，或者download目录，这时候也会触发。

1. [使用O-LLVM和NDK对Android应用进行混淆](http://www.jianshu.com/p/0c23e0a886f4)
	
	Android开发中经常需要对敏感信息进行加密，避免不了要将密钥存放在终端设备上，那么如何防止密钥被逆向出来呢？这是一个先有鸡还是先有蛋的悖论。相比较将密钥写在Java层，将其下移到NDK层是个更好的选择，本文就来介绍如何对NDK层代码进行混淆，以更好的保护我们的密钥。

1. [Android中读取图片EXIF元数据之metadata-extractor的使用](http://blog.csdn.net/gao_chun/article/details/46854323)

	首先介绍一下什么是EXIF，EXIF是 Exchangeable Image File 的缩写，这是一种专门为数码相机照片设定的格式。这种格式可以用来记录数字照片的属性信息，如相机的品牌及型号、相片的拍摄时间、拍摄时所设置的光圈大小、快门速度、ISO等信息。除此之外它还能够记录拍摄数据，以及图片格式化方式，这样就可以输出到兼容EXIF格式的外设上，如照片打印机等。

1. [Android调试命令总结](http://blog.csdn.net/yzzst/article/details/47128581)	
	主要介绍了 am、pm、input、ime、netcfg、ndc、vdc、service、getprop、dumpstate、dumpsys、bugreport等一系例命令行调试调试工具以及Android中的Linux命令的使用方法。

1. [ Android Camera 实时滤镜系列](http://blog.csdn.net/wyhuan1030/article/category/3113937)
	
	Android系统将内置滤镜功能,滤镜功能有二十余种不同效果，不逊色于极受欢迎的智能手机应用Instagram所产生的效果。android中可以通过颜色矩阵（ColorMatrix类）方面的操作颜色，颜色矩阵是一个5x4 的矩阵。可以用来方面的修改图片中RGBA各分量的值，颜色矩阵以一维数组的方式存储如下：
 [ a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t ]
他通过RGBA四个通道来直接操作对应颜色，如果会使用Photoshop就会知道有时处理图片通过控制RGBA各颜色通道来做出特殊的效果。
	
### 代码&开源库

1. [Once](https://github.com/jonfinerty/Once)

	一个方便你管理一次性操作设置的库。

1. [LandscapeVideoCamera](https://github.com/JeroenMols/LandscapeVideoCamera)

	强大的自定义 Android Camera，并且支持细粒度的控制视频质量和文件大小。

1. [material-code-input](https://github.com/glomadrian/material-code-input)

	一个 Material 风格的 Code 输入框。

1. [FastGCM](https://github.com/iammert/FastGCM)
	
	一个可以让你快速集成Google Cloud Messaging(GCM)的库。
	
1. [dotted-progress-bar](https://github.com/igortrncic/dotted-progress-bar)
	
	圆点进度条。

1. [Carpaccio](https://github.com/florent37/Carpaccio)

	一个第三方的Android DataBinding库.

1. [RecyclerTabLayout](https://github.com/nshmura/RecyclerTabLayout)

	一个用 RecyclerView 实现的滑动TabLayout。

1. [ParkedTextView](https://github.com/gotokatsuya/ParkedTextView)

	一个支持占位符的EditText。

1. [SortableTableView](https://github.com/ISchwarz23/SortableTableView)

	支持按列排序的TableView。

1. [material-icon-lib](https://github.com/code-mc/material-icon-lib)

	一个包含1000多个 Material 风格图标的库，可以很容易的通过 Drawable 或者 单独的View来使用这些图标。

### 工具

1. [Google 镜像站搜集](https://github.com/sxyx2008/DevArticles/issues/99)

	一个Google国内镜像站点列表，镜像站分原版和非原版，非原版界面有些改变，搜索结果依然是相同的。

### 视频

1. [手机百度Android平台平台化解决方案](http://www.infoq.com/cn/presentations/mobile-baidu-android-platform-solutions)

	通过此演讲，将向大家介绍百度APS (Advance Plugin System) 平台的由来、技术方案以及第三方开发者、使用者们比较关注的相关问题，包括如何快速开发、如何合作接入等等，同时也将通过案例数据分析更加全面具体的解析百度APS (Advance Plugin System)，并着重讲解基于Android的平台插件解决方案！

### 设计工具	

1. [Magic Mirror for Sketch 3](http://magicmirror.design)

	这是一款 Sketch 插件，可以在 Sketch 中快速创建透视图.

----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)