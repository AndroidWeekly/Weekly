layout: post
title: "Android开发技术周报 Issue#44"
date: 2015-08-11 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#44

### 新闻

1. [谷歌确定Android 6.0命名为Marshmallow](http://www.cnbeta.com/articles/421403.htm)

	谷歌终于确定了Android M中M所代表的甜品：Marshmallow（棉花糖）。Android 6.0五月下旬在I/O大会上亮相，将于今年秋天与用户见面。但是依照惯例，谷歌并没有宣布新Android的代号全称。新版本发布后，只能说，MM巧克力豆的粉丝对不起了。

1. [剥离安全机制：Android Auto终于还是迎来了第三方ROM](http://www.cnbeta.com/articles/420289.htm)

	移动平台的Android系统深受MOD爱好者们的喜爱，而在面向车载平台的Android Auto发布之后，我们就知道它早晚也是会迎来各种第三方ROM的。需要指出的是，尽管Android坚持着开源的理念，但是Google对于车载平台的界面却有着更加严格的控制。默认情况下，普通人是无法对其进行个性定制、甚至在Android Auto上侧载（side load）应用的。

### 教程

1. [关于Android的.so文件你所需要知道的](http://www.jianshu.com/p/cb05698a1968)

	如果项目中使用到了NDK，它将会生成.so文件，因此显然你已经在关注它了。如果只是使用Java语言进行编码，你可能在想不需要关注.so文件了吧，因为Java是跨平台的。但事实上，即使你在项目中只是使用Java语言，很多情况下，你可能并没有意识到项目中依赖的函数库或者引擎库里面已经嵌入了.so文件，并依赖于不同的ABI。

1. [安卓中的Flux架构](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2015/0816/3311.html)

	要为安卓应用找到一个好的架构不是一件容易的事情。谷歌似乎不太在乎这个事情，因此在设计模式上，除了Activity 生命周期管理之外，再也没有官方的推荐。但是，为你的应用打造一个架构师非常重要的。不管你是否喜欢，任何应用最终都会有一个架构。因此你最好是成为一个架构的奠基人，而不是等着它出现。

1. [Cool Android Apis 整理系列](http://oakzmm.com/categories/)

	本系列包含2篇文章，[Cool Android Apis 整理（一）](http://oakzmm.com/2015/08/04/cool-Android-api/)和[Cool Android Apis 整理（二）](http://oakzmm.com/2015/08/11/cool-Android-api-2/)，主要是对 `Dan Lew` 的[Android Tips Round-Up](http://blog.danlew.net/2014/03/30/android-tips-round-up-part-1/) 系列文章和知乎上问题[Android开发中，有哪些让你觉得相见恨晚的方法、类或接口？](http://www.zhihu.com/question/33636939)中涉及到的每个Tips都加入或官方文档或使用方法或效果之类的补充。

1. [Android性能优化典范（三）](http://www.csdn.net/article/2015-08-12/2825447-android-performance-patterns-season-3/3)
	
	Android性能优化典范的课程最近更新到第三季，共包含12个短视频，内容大致有：更高效的ArrayMap容器、使用Android系统提供的特殊容器来避免自动装箱、避免使用枚举类型、注意onLowMemory与onTrimMemory的回调等。

1. [Android Studio - MAC 版 - 快捷键详解](http://blog.csdn.net/shulianghan/article/details/47321177)

	在任何编程环境中, 熟练使用环境提供的快捷键会大大提高编程效率, 在 Android Studio 中也不例外, 熟练使用其快捷键是 Android 开发者必备的技能之一, 这里根据官网提供的列表, 我自己总结使用了一遍, 将快捷键使用记录以及使用后的效果都展示给大家; 

1. [MVP 在 Android 中的简单应用](https://www.v2ex.com/t/212695#reply4)

	导读：上一章我们初探了Android MVP，但是只涉及到一些概念性的东西，这一章，我们将来一起来一步步实现一个简单的MVP的Demo。

1. [Android MVP 探究与总结](http://www.v2ex.com/t/212456#reply2)

	在Android的开发过程中，Activity承担了大量地工作。如果对整个项目十分了解，并且在开发过程中有意识地抽离出了一些通用层的话，维护起来还稍微好一点，但实际上我们经常会遇到这样一些情况：维护并迭代已有地商业项目（可能前几期并不是由你开发）;UI变动极大（是不是经常Crtl+f到处查找？）

1. [MWR实验室公布Android系统0day漏洞可绕过Android沙箱](http://www.droidsec.cn/mwr实验室公布android系统0day漏洞可绕过android沙箱/)

	MWR实验室的研究人员又发现一个0day漏洞。这个漏洞存在于安卓系统中Google Admin应用程序处理一些URL的方式中，攻击者甚至可以通过这个漏洞绕过沙箱机制。MWR实验室在报告中提到了该漏洞原理：当Google Admin应用程序接收到一个URL，并且该URL是通过同一设备上任何其他应用的IPC调用接收时，Admin程序会将这个URL加载到它活动内的 Webview中。这时若攻击者使用一个file:// URL链接到他们所控制的文件，那么就可以使用符号链接绕过同源策略，并接收到Admin沙箱中的数据。

1. [安卓再爆两个短信拒绝服务/伪造状态漏洞，影响所有Android版本](安卓再爆两个短信拒绝服务/伪造状态漏洞，影响所有Android版本)	

	第一个漏洞（CVE-2015-3839）可能允许攻击者插入恶意消息到系统短信箱中导致其崩溃，造成用户无法发送和接收短信，第二个漏洞（CVE-2015-3840)可以伪造短信的发送和接收状态，可能导致用户重复发送短信增加话费。不同于之前的Android Stagefright和Mediaserver组件漏洞，新漏洞瞄准的是Android系统的短信应用。这两个漏洞影响Android系统所有版本，包获最新Android5.1.1（仅影响Android原生系统的短信应用，不包获第三方短信应用）。目前谷歌表示已经正在修复这两个漏洞，同时给出的漏洞评级均为低危。

1. [Android视频录制app解决方案汇总](https://www.zybuluo.com/lichangadd/note/148109)

	现在市面上视频App有很多，例如：蝌蚪音客、美拍、小影还有最近火起来的小咖秀。这类App的技术难点基本都是在音视频处理这一块，iOS对多媒体处理的支持还算比较丰富，但是Android就会差很多。这里总结蝌蚪音客在多媒体处理上遇到的问题，供大家参考下。

### 代码&开源库

1. [material-sheet-fab](https://github.com/gowong/material-sheet-fab)

	一个实现了 FAB 变换为 Sheet 的 Transition 动画的库。 

1. [InteractivePlayerView](https://github.com/iammert/InteractivePlayerView)

	一个漂亮的自定义音乐播放View.

1. [android-DecoView-charting](https://github.com/bmarrdev/android-DecoView-charting)

	DecoView: Android arc based animated charting library.

1. [android-HeaderFooterGridView](https://github.com/recruit-mp/android-HeaderFooterGridView)

	支持添加自定义Header和Footer View的GridView。

1. [awesome-android-testing](https://github.com/hotchemi/awesome-android-testing)

	一个收集了关于单元android testing的一系列东西，包括测试框架、集成测试工具、测试服务、文档、例子等。

1. [rx-preferences](https://github.com/f2prateek/rx-preferences)

	Reactive SharedPreferences。

1. [ArrowDownloadButton](https://github.com/fenjuly/ArrowDownloadButton)
	
	一个漂亮的下载按钮。

1. [ReactiveNetwork](https://github.com/pwittchen/ReactiveNetwork)
	
	 用RxJava Observables来检测网络连接状态和WIFI信号强弱变化的库。

1. [TagCloudView](https://github.com/kingideayou/TagCloudView)

	支持 SingleLine 模式的标签云效果.

1. [MarkdownView](https://github.com/falnatsheh/MarkdownView)

	可以显示 Markdown 格式文本的自定义WebView。

1. [Android-SpeedyViewSelector](https://github.com/devsoulwolf/Android-SpeedyViewSelector)

	一个可以方便你给控件和布局添加Color Selector的库。

1. [AndroidFillableLoaders](https://github.com/JorgeCastilloPrz/AndroidFillableLoaders)

	通过 SVG paths实现的填充进度效果的Loaders。

### 工具

1. [Jimu Mirror](http://jimulabs.com)

	与JRebel、LayoutCast也是类似的工具，只不过侧重点不同，Jimu Mirror支持Live-code（XML/Java/Kotlin/PNG files）、Hot-swapping、Accurate, interactive previews、REPL for Android UI development、Custom views, custom fonts、Great for learning Android coding、Sample data等等，Jimu Mirror是收费的Personal License每年79 USD，Commercial License每年 $149 USD，付费后第一年免费。

1. [JRebel for Android](http://zeroturnaround.com/software/jrebel-for-android/beta-quick-start/ )

	与LayoutCast类似，不需要复杂的配置只需安装JRebel for Android的Android Studio插件即可，具体使用方法可以看官网的教程，目前还处于beta阶段，不过我简单使用了下效果挺不错的，在代码中修改后Make下，新的改变就可直接在真机上查看。
	
1. [LayoutCast](https://github.com/mmin18/LayoutCast)

	一个可以把代码和资源文件的改动直接同步到手机上，应用不需要重启，省去了编译运行漫长的等待。BUCK很快，但入侵性强，项目改动大，LayoutCast对项目改动小。

1. [Sixpack-java](http://sixpack.seatgeek.com)	
	Sixpack是一个与语言无关的A/B测试框架，具有非常易用的API和内置的dashboard。Sixpack有两个主要的组件，即Sixpack server和Sixpack web。其中sixpack server负责收集experiment 数据并决定要将哪一个可选方案展现给哪些人。Sixpack web是一个基于Web的dashboard。Sixpack支持多种语言的客户端，目前包括PHP、Ruby、Python和JavaScript。

### 设计

1. [五款app原型设计工具对比](http://get.jobdeer.com/7827.get)

	我用五款“高保真”原型设计工具重新创建了IF by IFTTT user onboarding应用，目的是了解这些工具的不同之处，它们是Proto.io, Pixate, Framer, Facebook的 Origami 和 RelativeWave的Form。为什么我会选择这五款？我发现用多数原型设计工具再造这种重度动画效果的应用（图标以不同的速度向不同的方向移动）几乎不可能。大多数工具仅仅是让你连接静态“页面”，只有那些更复杂的才能让你在给定的页面里不同的对象或“层”添加动效。

1. [简约至上-交互设计四策略](http://ww2.sinaimg.cn/bmiddle/5f590940gw1ev1uo13zilj20ic7r31ky.jpg)

	简单并不意味着钱缺或低劣， 也不意味着不注重装饰或者完全赤裸裸。而是说装饰应该紧贴近设计本身，任何无关的要素都应该予以剔除。简单的特征和个性应该源自你使用的方法、所要表现的产品，以及用户执行的任务。简单的用户体验是初学者、新手的体验，或是压力一下的主流用户的体验。

1. [为什么sketch中预置的画布尺寸比真实分辨率小？](http://mp.weixin.qq.com/s?__biz=MzA4MzI0MTkxOQ==&mid=209374693&idx=1&sn=7e9e4acb85c5bc0e048aa3300541d79d#rd)

	有太多太多刚刚上手sketch的小伙伴们都有这样的问题，为什么我在Sketch中建立画布，软件预置的Artboard尺寸总是那么小呢？比如iphone6的真实分辨率是750-1334像素，但是sketch中的Artboard尺寸居然是375-667像素。同样其他机型的预置尺寸也有问题，是sketch出错了吗？

#### 设计工具

1. [ColorHunt](http://www.colorhunt.co)

	一个收集了一些漂亮的配色板网站，每天都会更新。

### Code之外

1. [我所理解的执行力](http://mp.weixin.qq.com/s?__biz=MjM5NTIyNTUyMQ==&mid=209463345&idx=1&sn=44a5fb5fdd127b69df87bf59657989f5&3rd=MzA3MDU4NTYzMw==&scene=6#rd)

	从百度说起，百度的文化里面，除了最近几年讲的「狼性」以外，还有从公司成立之初就一直讲的「简单可依赖」。这里面的「可依赖」三个字，在我看来，就是一种对执行力的理解。

1. [为什么你应该尝试全栈](http://weibo.com/p/1001593875062515164803)

	程序员看到全栈这个概念，大概会有两种反应: 1.卧槽，这个好，碉堡了 2.你懂毛，全栈就是样样稀松
以上两种反应其实都有失偏颇，即使只做一种技术，做的很菜的多的是，而全栈但是样样都做的不错的也不少，更别说这个世界还存在另外一种爆栈型的程序员，做什么什么精。

1. [怎样有超级英雄般的高效率：学会用「心流」工作](http://weibo.com/p/1001603875052117703934)

	写这篇文字的原因，是很多人都在问这样的问题，大狗熊，你每天的时间是如何分配的？又是播客，又是视频，还学英语，每天还更新订阅号文字，还组织跑步活动，还得干活儿挣钱，还得读书啥的，这样的时间，一天从早排到晚也不够啊！你一定经常夜里加班吧？

1. [时间统计法 | 善于工作的人，时间总是够](http://weibo.com/p/1001603874439224817431)

	「时间统计法」，源于一本被定义为「一部以真人真事为基础的文献性小说」：《奇特的一生》，这本书讲述了苏联昆虫学家柳比歇夫如何通过他所独创并坚持了几十年的时间管理方法，帮助他一生取得了巨大的成就。

----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)