layout: post
title: "Android开发技术周报 Issue#43"
date: 2015-08-04 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#43

### 教程

1. [Android项目中如何用好构建神器Gradle？](http://www.csdn.net/article/2015-08-10/2825420/2)

	Gradle虽为构建神器，但感觉学习曲线比较陡峭。Gradle User Guide内容很多，但有点太多了，多的你看不完，Gradle Plugin User Guide一篇文章主要讲了Android相关的配置，看完可能感觉马马虎虎会用，但到了修改一些构建流程的时候还是不知所措。

1. [Android Context 是什么？](http://blog.csdn.net/feiduclear_up/article/details/47356289)

	Context对于Android开发人员来说并不陌生，项目中我们会经常使用Context来获取APP资源，创建UI，获取系统Service服务，启动Activity，绑定Service，发送广播，获取APP信息等等。那么Context到底是什么？Context又是怎么来实现以上功能的？在什么场景下使用不同的Context？一个APP中总共有多少个Context？这篇博客将从源码角度带你分析Android Context到底是个啥。

1. [Android应用开发之所有动画使用详解](http://blog.csdn.net/yanbober/article/details/46481171)

	Android系统提供了很多丰富的API去实现UI的2D与3D动画，最主要的划分可以分为如下几类：View Animation： 视图动画在古老的Android版本系统中就已经提供了，只能被用来设置View的动画。Drawable Animation： 这种动画（也叫Frame动画、帧动画）其实可以划分到视图动画的类别，专门用来一个一个的显示Drawable的resources，就像放幻灯片一样。

1. [Activity Testing](http://www.devtf.cn/?p=979)

	Activity测试依赖于Android Instrumentation测试框架。有其他组件不同的是Activity有更复杂的生命周期，这些生命周期函数不能直接地被调用，而只能通过Instrumentation发送事件来触发它们。

1. [Android 中的 AOP 编程](http://www.devtf.cn/?p=981)

	面向切面编程（AOP，Aspect-oriented programming）需要把程序逻辑分解成『关注点』（concerns，功能的内聚区域）。这意味着，在 AOP 中，我们不需要显式的修改就可以向代码中添加可执行的代码块。这种编程范式假定『横切关注点』（cross-cutting concerns，多处代码中需要的逻辑，但没有一个单独的类来实现）应该只被实现一次，且能够多次注入到需要该逻辑的地方。
	
1. [APK 在32bit/64bit平台 动态库问题](http://blog.csdn.net/jscese/article/details/47101815)

	目前64bit android系统也慢慢的多了，看到也有apk声称支持64bit system，然后就往里面打包搞了个arm64-v8a 目录，放了个64bit的so，但是apk代码里面却不按规范去load so ，导致一系列 file not found 异常~

1. [ApplicationId 与 PackageName](http://chaosleong.github.io/blog/2015/06/04/applicationid-yu-packagename/)

	Android 应用都有自己的包名。包名是设备上每个应用程序的唯一标识，同样也是 Google Play 商店里的唯一标识。就是说，假如你已经使用某个包名来发布应用，就不能再去改变应用的包名，因为这样做会导致你的应用被视为一个全新的应用，你现有的用户也不会收到应用的更新通知。

1. [Android Studio 使用 Gradle 打包 Jar](http://chaosleong.github.io/blog/2015/08/02/android-studio-shi-yong-gradle-da-bao-jar/)

	Android Studio 打 Jar 包一直是一个麻烦的事，按照网上现有的教程，打包一个混淆的 jar 需要完成下列步骤：1.将 plugin 修改为 library 后 build 出 aar，再提取 aar 里面的 classes.jar
2.使用 jarjar 等工具剔除多余的 class 3.对第二步得到的 jar 进行混淆

1. [Android平台免Root无侵入AOP框架Dexposed使用详解](http://www.jianshu.com/p/14edcb444c51)
	
	Dexposed是基于久负盛名的开源Xposed框架实现的一个Android平台上功能强大的无侵入式运行时AOP框架。Dexposed的AOP实现是完全非侵入式的，没有使用任何注解处理器，编织器或者字节码重写器。集成Dexposed框架很简单，只需要在应用初始化阶段加载一个很小的JNI库就可以，这个加载操作已经封装在DexposedBridge函数库里面的canDexposed函数中。

1. [Android.Hook框架Xposed篇](http://www.droidsec.cn/android-hook框架xposed篇/)
	
	模块基本开发流程：1.创建工程android4.0.3(api15,测试发现其他版本也可以),可以不用activity 2.修改AndroidManifest.xml 3.在工程目录下新建一个lib文件夹,将下载好的XposedBridgeApi-54.jar包放入其中.eclipse 在工程里 选中XposedBridgeApi-54.jar 右键–Build Path–Add to Build Path.IDEA 鼠标右键点击工程,选择Open Module Settings,在弹出的窗口中打开Dependencies选项卡.把XposedBridgeApi这个jar包后面的Scope属性改成provided.
	
### 代码&开源库

1. [SuperSwipeRefreshLayout](https://github.com/nuptboyzhb/SuperSwipeRefreshLayout)

	可定制的SwipeRefreshLayout，一举解决产品经理提出的各种下拉刷新问题！非侵入式、可定制、支持RecyclerView，ListView，ScrollView等。

1. [AndroidSweetSheet](https://github.com/zzz40500/AndroidSweetSheet)

	一个富有动感的Sheet(选择器)。

1. [Android-RatioLayout](https://github.com/devsoulwolf/Android-RatioLayout)

	比例布局。

1. [FingerTransparentView](https://github.com/drakeet/FingerTransparentView)

	手指区域羽化透明，显示出底部图片布局区域。

1. [AndroidScrollingImageView](https://github.com/Q42/AndroidScrollingImageView)

	可以实现视差滚动动画的ImageView。

1. [FoldingTabBar.Android](https://github.com/tosslife/FoldingTabBar.Android)

	一个可折叠的Tabbar菜单。

1. [easyfonts](https://github.com/vsvankhede/easyfonts)
	
	一个方便你在App里使用自定义字体的库。

1. [WaveSwipeRefreshLayout](https://github.com/recruit-lifestyle/WaveSwipeRefreshLayout)

	水滴动画效果的下拉刷新效果。	

1. [BeerSwipeRefresh](https://github.com/recruit-lifestyle/BeerSwipeRefresh)

	一个倒啤酒效果的下拉刷新效果。

1. [android-testing-templates](https://github.com/googlesamples/android-testing-templates)

	Google官方推出的Android单元测试模版项目。

1. [fab-transformation](https://github.com/konifar/fab-transformation)

	一个可以给Floating Action Button 添加 Transformation 动画的库。

1. [nice-spinner](https://github.com/arcadefire/nice-spinner)

	一个带有展开和折叠动画的Spinner。
	
1. [MetaballLoading](https://github.com/dodola/MetaballLoading)

	一个贝塞尔曲线实现的利用圆球拖拽粘连动画效果的加载进度条。

### 工具

1. [Android Studio 1.3.1](http://www.androiddevtools.cn/#android-studio)

	![](http://ww1.sinaimg.cn/mw690/8a41f469jw1euvelv8hfyj210a0con46.jpg)

1. [bintray-release](https://github.com/novoda/bintray-release)

	一个方便你将 Android Library 上传至bintray中央仓库的Gradle插件。

1. [AWebDB](https://lusfold.github.io/android/2015/07/29/使用AWebDB通过浏览器操作Android数据库.html)

	一个可以帮助你在浏览器查看Android Sqlite Database的库。

1. [ShakaApktool](https://github.com/rover12421/ShakaApktool)

	一个基于ApkTools的Android Apk 反编译工具。

### 视频

1. [Android 性能模式 第三季(英字幕)](http://www.youku.com/playlist_show/id_25972284.html)

### 设计资源	

1. [NOW UI KIT](http://www.invisionapp.com/now)

	A beautiful cross-platform UI kit. Yours free.Download all 52 templates, 35 custom icons, and 180+ UI elements free for Photoshop and Sketch.

----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)