layout: post
title: "Android开发技术周报 Issue#28"
date: 2015-04-20 12:50:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#28

### 教程

1. [Android判断APP是否在前台运行](http://www.androidcn.org/topic/55345ee18ca8a1e07687e9e8) ([@hi大头鬼hi](http://weibo.com/brucefromsdu))

	APP开发中经常会遇到这种需求，需要检查当前的APP是不是可见的，比如，如果是可见的就维持一个socket长连接，如果切到后台不可见了，就断开这个连接。Android本来并不允许APP去监听home键事件，所以我们没发像iOS那样通过监听home键事件来做对应的处理。
1. [Android Studio 入门指南](http://www.jianshu.com/p/36cfa1614d23) ([@安卓同学](http://weibo.com/lyf0306))
	
	作为一个Android 开发者，你应该很了解Android Studio，如果你现在还不了解，没关系，那么从现在开始，我们一起来了解了解Andoid Studio。

1. [Integer.valueOf(String) 方法之惑](http://www.importnew.com/9162.html) ([@陈启超_V](http://weibo.com/chenqichao2016))
	
	有个仁兄在 StackOverflow 上发起了一个问题，是这么问的：“ 我被下面的代码搞晕了，为什么它们会返回不同的值？”
	
		System.out.println(Integer.valueOf("127")==Integer.valueOf("127"));
		System.out.println(Integer.valueOf("128")==Integer.valueOf("128"));
		System.out.println(Integer.parseInt("128")==Integer.valueOf("128"));

1. [更深层次的理解Context](http://www.imooc.com/wenda/detail/255871) ([@慕课网Android学习小组](http://weibo.com/u/5321506202))	
	
	Context在开发Android应用的过程中扮演着非常重要的角色，比如启动一个Activity需要使用context.startActivity方法，将一个xml文件转换为一个View对象也需要使用Context对象，可以这么说，离开了这个类，Android开发寸步难行，对于这样一个类，我们又对他了解多少呢。
	
1. [facebook的Android调试工具Stetho介绍](http://www.androidcn.org/topic/552fabaa8ca8a1e07687e999) ([@hi大头鬼hi](http://weibo.com/brucefromsdu))
	
	Stetho是Facebook出品的一个强大的Android调试工具，使用该工具你可以在Chrome Developer Tools查看App的布局，网络请求，sqlite，preference，一切都是可视化的操作，无须自己在去使用adb，也不需要root你的设备。使用的方式很简单，配置好之后，在Chrome地址栏输入chrome://inspect （哈哈，和webview 远程调试的方式一样）。

1. [深入浅出RxJava四-在Android中使用响应式编程](http://blog.csdn.net/lzyzsd/article/details/45033611) ([@hi大头鬼hi](http://weibo.com/brucefromsdu))

	在第[1](http://blog.csdn.net/lzyzsd/article/details/41833541)，[2](http://blog.csdn.net/lzyzsd/article/details/44094895)，[3](http://blog.csdn.net/lzyzsd/article/details/44891933)篇中，我大概介绍了RxJava是怎么使用的。下面我会介绍如何在Android中使用RxJava.
RxAndroid是RxJava的一个针对Android平台的扩展。它包含了一些能够简化Android开发的工具。首先，AndroidSchedulers提供了针对Android的线程系统的调度器。需要在UI线程中运行某些代码？很简单，只需要使用AndroidSchedulers.mainThread().

1. [适用于 Google 搜索的 App Indexing(需要梯子)](https://developers.google.com/app-indexing/?hl=zh-cn) ([@北京GDG](http://www.weibo.com/gtug))

	Google 利用 App Indexing 为应用编制索引，就像为网站编制索引一样。指向您 Android 应用的深层链接显示在 Google 搜索结果中，用户可以快速体验您的本机移动应用，准确到达应用内的特定内容。

1. [Android性能优化系列](http://hukai.me/blog/categories/android-deeper/) ([@胡凯me](http://weibo.com/u/1706217303))

	Google近期在Udacity上发布了[Android性能优化的在线课程](https://www.udacity.com/course/ud825)，目前有三个篇章，分别从渲染，运算与内存，电量三个方面介绍了如何去优化性能，这些课程是Google之前在Youtube上发布的[Android性能优化典范](http://hukai.me/android-performance-patterns/)专题课程的细化与补充。

### 代码&开源库


1. [vector-compat](https://github.com/wnafee/vector-compat)

	VectorDrawable 和 AnimatedVectorDrawable 的兼容库，支持4.0以上系统。

1. [MaterialSpinner](https://github.com/ganfra/MaterialSpinner)

	一个Material Design风格的Spinner，最低支持到2.3系统。

1. [DashClock](https://github.com/romannurik/dashclock)

	[@romannurik](https://github.com/romannurik)大神开发的锁屏widget，支持4.2系统以上。

1. [Google Santa Tracker for Android](https://github.com/google/santa-tracker-android) ([@light_sky](http://www.weibo.com/lightSkyStreet))
	
	Google开源的一个带有教育和娱乐性质的App，应该是圣诞节给孩子们玩的小应用，里面有三个小游戏，另还有个Android Wear的Demo.
	
1. [spots-dialog](https://github.com/d-max/spots-dialog)

	斑点状的进度指示对话框。

1. [RxCupboard](https://github.com/erickok/RxCupboard)

	封装了RxJava 和 Cupboard ，让你流畅的从数据库中检索和存储POJOs数据流。

1. [ProgressBar](https://github.com/wly2014/ProgressBar)
	
	一个仿 github for windows 及 windows 8 的进度条。
		
### 工具	

1. [logproxy.js](https://github.com/unbug/logproxy) ([@听奏](http://www.weibo.com/unbug))
	
	logproxy.js是一个基于nodejs实现代理服务并打印http日志的小工具.给移动前端开者带来诸多便利.

### 书

1. [《软件架构模式》中文版](http://www.devtf.cn/?p=211) ([@MrSimp1e](http://weibo.com/n/MrSimp1e))
		
	书中讲解了五种流行的软件架构，非常好的资料。

1. [把时间当作朋友](http://zhibimo.com/read/xiaolai/ba-shi-jian-dang-zuo-peng-you/) [@李笑来](http://weibo.com/bylixiaolai)
	
	有些时候，有些事物，从反面描述比从正面描述更为容易。如若先仔细说清楚这本书不是什么，之后对“它究竟是什么”这个问题，可能就不言自明了。这本书不是时间管理书籍，尽管本书的内容也包括任务管理等与常见“时间管理技巧”相关的内容，但是，本书主张时间不可管理、一切都靠积累。
		
### 活动

1. [4.25日Material Design专题活动之认识与实践](http://chinagdg.com/thread-6751-1-1.html) ([@北京GDG](http://www.weibo.com/gtug))

	自2014年Google I/O发布了新的设计规范Material Design，这种设计语言旨在为手机、平板电脑、台式机和“其他平台”提供更一致、更广泛的“外观和感觉”。Material Design也已经逐渐成为了App设计的趋势，很多知名应用诸如：Evernote、Inbox等都已经采用了Material Design设计。

	北京谷歌开发者社区继续为大家奉上以Material Design为主题的活动，希望这次活动能够加深大家对Material Design的了解，解决大家在使用Material Design过程中遇到的困惑，同时也让准备使用Material Design的小伙伴通过这场活动先热个身  =。=
			
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)