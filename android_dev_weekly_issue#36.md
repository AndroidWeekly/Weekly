layout: post
title: "Android开发技术周报 Issue#36"
date: 2015-06-16 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#36

### 教程

1. [Android Studio分模块自动化构建实战](http://www.jianshu.com/p/fec2818f2f20)

	最近在使用Android Studio＋Gradle做一个基础框架SDK项目，该框架主要实现每个app都需要的基础能力，例如网络请求，图片缓存，json解析，日志记录等等。众所周知，AndroidStudio中应该尽量使用Module来进行模块的划分，既能达到模块解耦的目的，也能在必要的时候轻松实现分模块打包，特别是在SDK项目中。

1. [一步一步教你实现Periscope点赞效果](http://www.jianshu.com/p/03fdcfd3ae9c)

	现在视频应用越来越火,Periscope火起来后,国内也出现了不少跟风者,界面几乎跟Periscope一模一样.Periscope确实不错,点赞的效果也让人眼前一亮,很漂亮,于是乎,我就想着自己实现一下.

1. [Android内核开发：学会分析系统的启动log](http://ticktick.blog.51cto.com/823160/1662911#0-tsina-1-30973-397232819ff9a47a7b7e80a40613cfe1)

	要学会分析系统的启动log信息，首先得了解Android系统的启动过程，建议先阅读《Android内核开发：图解Android系统的启动过程》这篇文章，它详细介绍了Android系统的启动过程。其次，你需要知道如何抓取系统启动log信息，建议阅读《Android内核开发：如何统计系统启动时间》这篇文章，它详细地介绍了如何抓取系统的启动log信息。

1. [用Robolectric来做Android unit testing](http://segmentfault.com/a/1190000002904944)

	我们知道安卓的app需要运行在delvik上面，我们开发Android app是在JVM上面，在开发之前我们需要下载各个API-level的SDK的，下载的每个SDK都有一个android.jar的包，这些可以在你的android_sdk_home/platforms/下面看到。当我们开发一个项目的时候，我们需要指定一个API-level，其实就是将对应的android.jar 加到这个项目的build path里面去。

1. [Android中的Low Memory Killer](http://blog.csdn.net/yujun411522/article/details/46516277)

	在现有的技术条件下，内存永远都是一个吃紧的资源，不用说是PC上会出现内存不足的可能，更不必说在移动设备上了。一旦出现内存不足就会导致系统卡顿，影响用户体验。而Android运行在Linux的基础之上，Linux的内存的使用原则就是不要浪费内存，所以在程序退出时在一段时间内还停留在内存中，这也是我们下一次打开程序时发现快一些的原因；但是这样带来的坏处就是如果驻留在内存中的程序多了，容易导致OOM的可能。

1. [Android Studio中如何打JAR包](http://www.jianshu.com/p/be4791a7abc7)

	Android Studio中对于library类型的Moudle，默认打出来的是AAR包，
但有时候我们的SDK还需要共享给一些其他eclipse的项目使用，这样我们就需要输出JAR包，
可以通过在Moudle中的build.gradle加入task来实现

1. [Android EditText的使用及值得注意的地方](http://www.jianshu.com/p/1f05bb1fde3e)

	Android上有很多输入法应用，每种输入法都有各自的特点，输入法多数时候是和EditText配合使用，结合我自己的亲身实践分享一下使用EditText过程中遇到的一些问题及解决方法。

1. [美团Android DEX自动拆包及动态加载简介](http://tech.meituan.com/mt-android-auto-split-dex.html)

	作为一个android开发者，在开发应用时，随着业务规模发展到一定程度，不断地加入新功能、添加新的类库，代码在急剧的膨胀，相应的apk包的大小也急剧增加， 那么终有一天，你会不幸遇到这个错误：生成的apk在android 2.3或之前的机器上无法安装，提示INSTALL_FAILED_DEXOPT
方法数量过多，编译时出错，提示：`Conversion to Dalvik format failed:Unable to execute dex: method ID not in [0, 0xffff]: 65536`

1. [Path相关方法讲解(一)](http://blog.csdn.net/tianjian4592/article/details/45652257)

	上一篇主要讲了Canvas的translate(平移) 、scale(缩放) 、rotate(旋转) 、skew(错切)，接下来几篇主要讲下android里的Path（封装了贝塞尔曲线）& Canvas里的drawPath(path,paint);
很多人听到贝塞尔曲线，就觉得似乎挺高端大气上档次，后面会和大家一起揭开它的面纱，一睹真容；
Path（路径）：

1. [理解AtomicBoolean](http://blog.csdn.net/yzzst/article/details/46469331)

	前些天有朋友问我，经常在代码中看到Atomic开头的类，不明白是什么意思。这里我们就从AtomicBoolean开始说吧，自己正好也复习一下。对于官方的说明是：可以用原子方式更新的 boolean 值。有关原子变量属性的描述，请参阅 java.util.concurrent.atomic 包规范。AtomicBoolean 可用在应用程序中（如以原子方式更新的标志），但不能用于替换 Boolean。

1. [Android应用安全现状与解决方案（学习资料）](http://blog.csdn.net/yzzst/article/details/46471277)

	安全对一些涉及到直接的金钱交易或个人隐私相关的应用的重要性是不言而喻的。Android系统由于其开源的属性，市场上针对开源代码定制的ROM参差不齐，在系统层面的安全防范和易损性都不一样，Android应用市场对app的审核相对iOS来说也比较宽泛，为很多漏洞提供了可乘之机。

1. [Android应用程序UI硬件加速渲染的Display List渲染过程分析](http://blog.csdn.net/luoshengyang/article/details/46281499)

	在硬件加速渲染环境中，Android应用程序窗口的UI渲染是分两步进行的。第一步是构建Display List，发生在应用程序进程的Main Thread中；第二步是渲染Display List，发生在应用程序进程的Render Thread中。Display List的渲染不是简单地执行绘制命令，而是包含了一系列优化操作，例如绘制命令的合并执行。本文就详细分析Display List的渲染过程。

### 代码&开源库

1. [RecyclerViewPager](https://github.com/lsjwzh/RecyclerViewPager)

	重写后的 RecyclerViewPager 完全继承自RecyclerView，可以自定义触发翻页的距离，可自定义翻页速度，支持VerticalViewPager，支持Fragment。

1. [rox-android](https://github.com/dan-zx/rox-android)

	一个Material Design风格的基于用户和朋友喜欢的地点给游客推荐兴趣地点的App。

1. [Notes](https://github.com/lguipeng/Notes)

	一款基于Material Design 的开源笔记本应用。

1. [SmsCodeHelper](https://github.com/drakeet/SmsCodeHelper)

	是由原「贝壳单词」团队开发的一款新的开源轻App.它可以在手机接收到验证码短信的时候，自动浮现验证码，并自动复制验证码到用户的剪切板。

1. [android-topeka](https://github.com/googlesamples/android-topeka)

	Google 放出的一个 Material Design 的演示 APP 源代码。

1. [ExpandableSelector](https://github.com/Karumi/ExpandableSelector)	
	ExpandableSelector is an Android library created to show a list of Button/ImageButton widgets inside a animated container which can be collapsed or expanded.

1. [material-animated-switch](https://github.com/glomadrian/material-animated-switch)
	
	一个material Switch 控件支持ico动画和颜色变换。

1. [GuillotineMenu-Android](https://github.com/Yalantis/GuillotineMenu-Android)

	一个铡刀效果的自定义菜单。

1. [voice-recording-visualizer](https://github.com/tyorikan/voice-recording-visualizer)

	一个可以将麦克风的音频可视化的库。

1. [IntentBuilder](https://github.com/emilsjolander/IntentBuilder)

	类型安全的Intent Builder.

1. [CreditCardView](https://github.com/vinaygaba/CreditCardView)

	自定义信用卡View。
			
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)