layout: post
title: "Android开发技术周报 Issue#38"
date: 2015-06-30 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#38

### 教程

1. [Android Design Support Library 的 代码实验——几行代码，让你的 APP 变得花俏](http://www.jianshu.com/p/1078568e859f)

	目前，我相信，没有任何 Android 开发者不知道材料设计的，因为它的设计在过去的一年震惊了世界，正式的变成了一个设计理念。令人惊讶的是，在 Android 应用中材料设计是不容易实现的，因为材料设计的 UI 组件 如: Floating Action Button (FAB) 在低于 Android L 系统上是不可用的。我们只能选择使用由独立开发者公布出来的第三方库

1. [Android 增强版百分比布局库 为了适配而扩展](http://blog.csdn.net/lmj623565791/article/details/46767825)

	上周一我们发布了Android 百分比布局库(percent-support-lib) 解析与扩展中对percent-support这个库进行了解析和添加了PercentLinearLayout的支持。

1. [浅析： Android 嵌套滑动机制（ NestedScrolling）](https://www.v2ex.com/t/202534#reply0)

	谷歌在发布安卓 Lollipop版本之后，为了更好的用户体验，Google为Android的滑动机制提供了NestedScrolling特性，NestedScrolling的特性可以体现在哪里呢？比如你使用了Toolbar，下面一个ScrollView，向上滚动隐藏Toolbar，向下滚动显示Toolbar，这里在逻辑上就是一个NestedScrolling —— 因为你在滚动整个Toolbar在内的View的过程中，又嵌套滚动了里面的ScrollView。

1. [我眼中的下拉刷新](http://www.liaohuqiu.net/cn/posts/the-pull-to-refresh-in-my-eyes/#comment-2111797440)

	在APP交互中，下拉刷新是非常常见的一种交互方式。在使用APP的时候，这也成为了一种潜意识的操作了。下拉刷新最早在iOS中出现，iOS的视图渲染机制完成这种效果是非常简单的。但Android的视图呈现形式，实现这一效果就需要稍微麻烦一些了。

1. [影响数千万APP的安卓APP“寄生兽”漏洞技术分析](http://drops.wooyun.org/papers/6910)

	360手机安全研究团队vulpecker近日发现了一种新型的安卓app安全漏洞，市面上数以千万的app都受该漏洞影响。该漏洞一旦被攻击者利用，可以直接在用户手机中植入木马，盗取用户的短信、照片以及银行、支付宝等账号密码，vulpecker以“寄生兽”命名这个漏洞。

1. [虚化梦幻背景+自动来回移动动画效果](http://2.rogerbolg.sinaapp.com/?p=92)

	必须说写博客是一项非常需要毅力的事情，这两月稍微忙一点就完全忘了这茬了，罪过罪过。今天解析一个 虚化梦幻背景+自动来回移动动画 的效果，这个动画也是从Muzei中提取出来了~感谢大神！！

### 代码&开源库

1. [driveimageview](https://github.com/mrwonderman/driveimageview)

	An advanced ImageView with a nice approach to display some text inside it.

1. [Atelier](https://github.com/Musenkishi/Atelier)

	一个对Palette进行了进一步的封装，支持链式调用，帮助你简化Palette使用的库。

1. [SeekBarCompat](https://github.com/ahmedrizwan/SeekBarCompat)

	SeekBar 的一个Material Design兼容实现，支持到API 16及以上。

1. [bubbles-for-android](https://github.com/txusballesteros/bubbles-for-android)

	像QQ那样可以把联系人头像添加到桌面并显示消息个数的效果。

1. [Paper](https://github.com/pilgr/Paper)

	一个快速的NoSQL数据存储库，使用高效的 Kryo 进行对象的序列化和反序列化。

1. [MultiCardMenu](https://github.com/wujingchao/MultiCardMenu)

	 一个交互方式比较新颖的卡片菜单。

1. [Dexposed](https://github.com/alibaba/dexposed)

	阿里巴巴无线事业部的第一个重量级Android开源项目——无侵入的运行期AOP框架『Dexposed』，基于ROOT社区著名开源项目Xposed改造剥离了ROOT部分，演化为服务于所在应用自身的AOP框架。它支撑了阿里大部分App的在线分钟级客户端bugfix和线上调试能力。

1. [DeepLinkDispatch](https://github.com/airbnb/DeepLinkDispatch)

	一个简单的、基于注解的Deep Link处理库。

1. [WaterDropListView](https://github.com/THEONE10211024/WaterDropListView)	
	A powerful ListView with awesome pull-refresh and pull-on-loadmore function!

1. [card.io-Android-source](https://github.com/card-io/card.io-Android-source)	
	一个信用卡信息扫描SDK。

1. [MaterialRecents](https://github.com/ZieIony/MaterialRecents)

	像系统的最近使用应用列表那样的堆栈卡片效果。

1. [AndroidRubberIndicator](https://github.com/LyndonChin/AndroidRubberIndicator)

	效果很赞的ViewPager指示器。

1. [DownloadProgressBar](https://github.com/panwrona/DownloadProgressBar)

	效果很赞的下载进度条效果。
	
1. [barber](https://github.com/hzsweers/barber)

	通过注解获取定义控件属性值的库。

1. [BlurredGridMenu](https://github.com/gotokatsuya/BlurredGridMenu)

	毛玻璃背景效果的网格菜单。

### 工具

1. [STF](https://openstf.github.io)

	STF is Control and manage real Smartphone devices from your browser. 

1. [Mobile-Checker](https://github.com/w3c/Mobile-Checker)

	W3C发布的移动端页面检查工具，可以选择三种屏幕规格，通过工具发现网站在移动端存在的问题。

### 视频

1. [移动开发网络性能优化实践](http://www.infoq.com/cn/presentations/performance-optimization-of-mobile-development-network)

	国内大多数无线App都会使用网络服务，面对国内移动无线网络的复杂环境，加上用户多样的硬件特性，因此会在开发App时面临比传统PC互联网更具挑战性的网络性能问题。携程客户端框架团队经过半年多的摸索，在App网络性能优化方面总结了一些实践经验，分享给国内无线App的开发者和架构师。

1. [美团移动平台背后的技术](http://www.infoq.com/cn/presentations/technology-of-meituan-mobile-platform#0-tsina-1-38715-397232819ff9a47a7b7e80a40613cfe1)
	
	从千团大战胜出的美团，如今在O2O的垂直业务上阔步前进，王兴更是提出了2015年要建平台、建生态。这意味着除去主营业务，美团团购客户端还需要接入电影选座、外卖、酒店订房等垂直业务，由于业务本身的千差万别，产品设计也是各不相同，导致代码复用很苦难，而且这些业务往往还不是同一个团队维护的。那么在平台化过程中，美团的移动开发团队是如何解决技术上、团队上、业务上的困难的呢？
			
----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)