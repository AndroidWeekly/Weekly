layout: post
title: "Android开发技术周报 Issue#53"
date: 2015-10-20 09:58:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#53

### 新闻

1. [谷歌公布 Android 6.0 设备要求：强制开启全磁盘加密](https://linux.cn/article-6433-1.html)

	据科技博客VentureBeat报道，谷歌在周一更新了Android 6.0的兼容性生产规格文件，向手机和平板电脑制造商详细介绍了运行Android 6.0系统的设备需要满足的要求。谷歌对于制造商生产的Android 6.0设备主要有3点要求：1.默认开启全磁盘加密(FDE) 2.配备指纹传感器 3.不得修改打盹模式(Doze mode)
	
1. [谷歌要求OEM厂家保留并不得修改安卓6.0的Doze省电模式](http://www.inexus.co/article-3756-1.html)
	
	如果说安卓6.0有什么功能是大家最感兴趣的话，那么Doze省电模式一定是大家提及最多的功能之一。多少年来安卓一直没有解决后台应用启动耗电的难题，而现在如果您安装安卓6.0的手机或者平板有段时间没有使用的话，设备就会进行Doze省电模式，应用将被休眠，所有的唤醒锁都会被忽略。

### 教程

1. [Adapter优化方案的探索](https://github.com/tianzhijiexian/Android-Best-Practices/blob/master/2015.10/adapter/adapter.md)

	故事发生在一个月黑风高的夜晚，那时候我知道了android世界中的一个恐怖的存在————adapter。看着无数的精英们随意地使用这强大的武器，造就了很多美轮美奂的应用时，我就暗自发誓，我一定要获得这个利器！

1. [Android悬浮窗TYPE_TOAST小结: 源码分析](http://www.jianshu.com/p/634cd056b90c)

	[Android无需权限显示悬浮窗, 兼谈逆向分析app](http://www.jianshu.com/p/167fd5f47d5c)这篇文章阅读量很大, 但是这篇文章是通过逆向分析UC浏览器的实现和兼容性处理来得到一个悬浮窗的实现小技巧, 但有很多问题没有弄明白, 比如为什么在API 18及以下 `TYPE_TOAST` 的悬浮窗无法接受触摸事件, 为什么使用 `TYPE_TOAST` 就不需要权限.

1. [让App像Web一样发布新版本](http://tldrify.com/c23)

	当一个App发布之后，突然发现了一个严重bug需要进行紧急修复，这时候公司各方就会忙得焦头烂额：重新打包App、测试、向各个应用市场和渠道换包、提示用户升级、用户下载、覆盖安装。有时候仅仅是为了修改了一行代码，也要付出巨大的成本进行换包和重新发布。

1. [当Field邂逅65535](http://jiajixin.cn/2015/10/21/field-65535/)

	言归正传，来聊聊为什么方法数不能超过65535？搬上Dalvik工程师在SF上的回答，因为在Dalvik指令集里，调用方法的invoke-kind指令中，method reference index只给了16bits，最多能调用65535个方法，所以在生成dex文件的过程中，当方法数超过65535就会报错。细看指令集，除了method，field和class的index也是16bits，所以也存在65535的问题。一般来说，method的数目会比field和class多，所以method数会首先遇到65535问题，你可能都没机会见到field过65535的情况。

1. [开源选型之 Android 三大图片缓存原理、特性对比](http://t.cn/RUvFbzl)

	这是我在 MDCC 上分享的内容(略微改动)，也是源码解析第一期发布时介绍的源码解析后续会慢慢做的事。从总体设计和原理上对几个图片缓存进行对比，没用到他们的朋友也可以了解他们在某些特性上的实现。

1. [Android 5.0屏幕录制漏洞（CVE-2015-3878）威胁预警](http://drops.wooyun.org/papers/9769)

	低技术门槛的漏洞利用或木马制作隐藏着极大的安全威胁，当这种安全威胁遇上手机用户的低安全意识时可能导致Android平台恶意软件的大规模爆发。360互联网安全中心最新研究发现，Android5.0屏幕录制漏洞（CVE-2015-3878）完全能够激发如上“两低”条件，漏洞威胁随时可能大规模爆发。

1. [Android动态加载技术三个关键问题详解](http://www.infoq.com/cn/articles/android-dynamic-loading)

	动态加载技术（也叫插件化技术）在技术驱动型的公司中扮演着相当重要的角色，当项目越来越庞大的时候，需要通过插件化来减轻应用的内存和CPU占用，还可以实现热插拔，即在不发布新版本的情况下更新某些模块。动态加载是一项很复杂的技术，这里主要介绍动态加载技术中的三个基础性问题，至于完整的动态加载技术的实现请参考笔者发起的[开源插件化框架DL](https://github.com/singwhatiwanna/dynamic-load-apk)：。项目期间有多位开发人员一起贡献代码。

1. [Android 高清加载巨图方案 拒绝压缩图片](http://blog.csdn.net/lmj623565791/article/details/49300989)

	对于加载图片，大家都不陌生，一般为了尽可能避免OOM都会按照如下做法：1.对于图片显示：根据需要显示图片控件的大小对图片进行压缩显示。2.如果图片数量非常多：则会使用LruCache等缓存机制，将所有图片占据的内容维持在一个范围内。其实对于图片加载还有种情况，就是单个图片非常巨大，并且还不允许压缩。比如显示：世界地图、清明上河图、微博长图等。

1. [怎样用 Android Annotations 写出高性能代码](http://blog.csdn.net/feelang/article/details/49095235)

	上一篇[博文](http://blog.csdn.net/feelang/article/details/49000203)中简单介绍了 Android Annotations 的基本用法，顺便扯了一下概念 - 契约编程，阅读量少的可怜，看来并没有多少人对此感兴趣，今天再来一篇，介绍几个稍微高级点的用法，我就不信弄不出一个大新闻。
	
1. [倍数提高工作效率的Android Studio奇技](http://zlv.me/posts/2015/07/13/14_android-studio-tips/)

	这是从Philippe Breault的系列文章《Android Studio Tips Of the Day》中提取出来的自认为精华的部分。这些技巧在实际应用中能够非常大的提高工作效率。

### 代码&开源库

1. [AVLoadingIndicatorView](https://github.com/81813780/AVLoadingIndicatorView)

	各种Loading效果。

1. [Drag-select-recyclerview](https://github.com/afollestad/drag-select-recyclerview)

	支持拖拽选择Item的Recyclerview。

1. [Lobsterpicker](https://github.com/LarsWerkman/Lobsterpicker)	
	Material Design风格的颜色选择器。

1. [AnimatorCompat](https://github.com/zzz40500/AnimatorCompat)

	一个快速创建动画帮助库.

1. [RxFlux](https://github.com/skimarxall/RxFlux)

	一个把 Flux 架构跟 RxJava 结合起来的框架
	
1. [Android-UCToast](https://github.com/liaohuqiu/android-UCToast)
	
	UC 浏览器复制，无需权限提示悬浮窗实现

1. [FlowingDrawer](https://github.com/mxn21/FlowingDrawer)

	一个弹性效果的抽屉菜单

1. [CustomSnackBar](https://github.com/TakeoffAndroid/CustomSnackBar)
	
	各种自定义的SnackBar。

1. [ProgressRoundButton](https://github.com/cctanfujun/ProgressRoundButton)

	圆角进度条，带文字进度指示。

1. [ScrollDownLayout](https://github.com/xiongwei-git/ScrollDownLayout)

	帮助你能够在ScrollView或者ListView里面使用ViewPager，支持手势下滑退出页面.

1. [RichText](https://github.com/zzhoujay/RichText)

	Android平台下的富文本显示控件，支持Html格式文本、支持图片点击事件、链接自动回调和支持设置加载中和加载错误时的图片。

1. [AnimatedRandomLayout](https://github.com/Windsander/AnimatedRandomLayout)

	本布局实现了在屏幕上随机生成可供操作的子控件控件，并完成向中心移动的随控件出现位置，
  动态设定的动画效果。

### 工具	

1. [ViewInspector](https://github.com/xfumihiro/ViewInspector)

	一个UI调试利器，支持Boundary、Layer、Event、Logging模式。Boundary模式可以显示UI控件的轮廓、margins和Padding；Layer模式可以以3D模式显示UI控件的层级；Logging模式会在Logcat下打印UI控件的生命周期事件信息等等。

1. [Android-lint-summary](https://github.com/passy/android-lint-summary)

	一个命令行工具支持将多个项目的Lint报告统一到一个输出，不再需要逐个检查每个子项目的lint错误结果以及在终端中查看格式化好的问题列表。

1. [Mobile-Security-Framework-MobSF](https://github.com/ajinabraham/Mobile-Security-Framework-MobSF)

	一个完全开源的Android/iOS应用的安全测试框架，支持静态和动态分析，并且可以输出测试报告。

1. [AndroidWiFiADB](https://github.com/pedrovgs/AndroidWiFiADB)

	一个可直接通过WiFi连接Android设备进行debug的AS插件，开发时可以摆脱USB线了.

1. [Github-Stars-Tagger](https://github.com/artisologic/github-stars-tagger)

	一个支持给GitHub第三方打标签的Chrome扩展应用.

### 书

1. [The kotlin programming language 中文翻译版](http://drakeet.me/the-kotlin-programming-language-zh)
	
	Kotlin是一门与Swift类似的静态类型JVM语言，由JetBrains设计开发并开源。与Java相比，Kotlin的语法更简洁、更具表达性，而且提供了更多的特性，比如，高阶函数、操作符重载、字符串模板。它与Java高度可互操作，可以同时用在一个项目中。

### 设计

1. [摆脱累赘的APP界面交互，回归轻生活](http://blog.jobbole.com/93116/)

	让我们一起来看看扁平化设计和Material design到底是如何起作用并渐渐引领如今这些风潮的。谷歌推出的设计语言。谷歌表示，这种设计语言旨在为手机、平板电脑和“其他平台”提供更一致、更广泛的“外观和感觉”。

----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)