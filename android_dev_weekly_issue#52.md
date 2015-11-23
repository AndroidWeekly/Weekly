layout: post
title: "Android开发技术周报 Issue#52"
date: 2015-10-07 09:10:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#52

### 新闻

1. [Google Play推出新功能，帮助开发者获取有效用户](http://blog.sina.com.cn/s/blog_9c079b040102wazz.html)

	在今年五月的Google I/O大会上，Google提前公布了一批功能强大的新开发工具，来帮助Google Play上的开发者以更敏锐的眼光扩大自身业务并提升决策水平。这些新功能已在Google Play开发者控制台正式上线。

1. [Android新掌门人确认--Hiroshi Lockheimer](http://www.cnbeta.com/articles/438269.htm)

	在成立母公司Alphabet之后，为更好的监管谷歌不断激增和庞大的业务流也为了让企业迈上新的台阶，除Google联合创始人Larry Page维持高位之外很多在公司内有影响力的高管和资深员工都得到了提拔，在Page升任Alphabet的CEO之后，此前Google的首席执行官职位已经稳妥的交由Sundar Pichai，而今天Pichai终于确认了此前职位的继任人选-- Hiroshi Lockheimer。

1. [Google Cardboard新动作，在虚拟现实世界玩起来吧！](http://blog.sina.com.cn/s/blog_9c079b040102waxu.html)

	自发布以来，Google Cardboard一直在努力将虚拟现实技术带到全世界。从今天开始，有39种不同语言版本的Google Cardboard 应用程序在100多个国家的Android和iOS设备上运行。此外，我们还公布了Cardboard 开发者说明以协助开发者创建美妙的虚拟现实体验。 Google Play目前已经有超过1500万个Cardboard 应用程序安装量，我们很兴奋能将虚拟现实技术与体验带给全世界更多的人们。

### 教程

1. [Android GC那点事](http://mp.weixin.qq.com/s?__biz=MzI1MTA1MzM2Nw==&mid=400021278&idx=1&sn=0e971807eb0e9dcc1a81853189a092f3&scene=0#rd)

	想写一篇关于Android GC的想法来源于追查一个魅族手机图片滑动卡顿问题，由于不断的GC导致的丢帧卡顿的问题让我们想了很多方案去解决，所以就打算详细的看看内存分配和GC的原理，为什么会不断的GC, GC ALLOC和GC COCURRENT有什么区别，能不能想办法扩大堆内存减少GC的频次等等。

1. [Android无需权限显示悬浮窗, 兼谈逆向分析app](http://www.jianshu.com/p/167fd5f47d5c)

	最近UC浏览器中文版出了一个快速搜索的功能, 在使用其他app的时候, 如果复制了一些内容, 屏幕顶部会弹一个窗口, 提示一些操作, 点击后跳转到UC, 显示这个悬浮窗不需要申请android.permission.SYSTEM_ALERT_WINDOW权限.

1. [如何自定义封装一个ReactNativeAndroid的NativeModule组件并在JSX中调用](http://weibo.com/p/2304184e1e357d0102yug0)

	FaceBook的 React Native Android 目前还不能加载 remoteJs的url方式，但是已经可以通过devPC-ip绑定或本地asserts编译依赖的方式进行打包了，也就是React基本可以实现了Learn Once,Run everyWhere(暂时即iOS,Andorid,webview)。

1. [iOS高性能图片架构与设计](http://t.cn/RyBJpvH)

	虽然是一篇讲解iOS高性能图片架构和设计的文章，但是讲到的一些问题拆解分析思路、架构的结构设计、缓存淘汰算法以及插件化的设计方法都很值得学习和思考。

### 代码&开源库

1. [Android 6.0源代码](http://pan.baidu.com/s/1bndnE8J)

	Android 6.0完整源代码，详情戳[这里](http://t.cn/RZgGJjj)。

1. [VerticalViewPager](https://github.com/kaelaela/VerticalViewPager)

	垂直切换的自定义ViewPager

1. [Meter](https://github.com/googlecreativelab/meter)

	一个在 Android 手机桌面上动态显示手机电量、信号强度和通知数量的动态壁纸程序.

1. [AutosizeEditText](https://github.com/txusballesteros/AutosizeEditText)

	一个对系统EditText进行了扩展，当输入的文字很多时EditText的大小变化的更加平滑。

1. [TextSurface](https://github.com/elevenetc/TextSurface)

	一个小动画框架可以帮助你漂亮地显示文本消息。

1. [android-animate-RichEditor](https://github.com/xmuSistone/android-animate-RichEditor)

	一个支持用户插入和删除图片的富文本编辑器，并且有插入和删除图片的动画效果。

1. [android-image-filter](https://github.com/ragnraok/android-image-filter)

	一些图片滤镜效果。

1. [PhotoView](https://github.com/bm-x/PhotoView)

	图片浏览缩放控件，和普通的ImageView一样的使用方法。

1. [XCL-Charts](https://github.com/xcltapestry/XCL-Charts)

	XCL-Charts基于原生的Canvas来绘制各种图表,在设计时，尽量在保证开发效率的同时，给使用者提供足够多的定制化能力。因此使用简便,同时具有相当灵活的定制能力。支持各种图表，其它特性还包括支持手势缩放、图表滑动、点击交互、多图叠加、图表批注、动画效果、多XY轴显示、轴线任意方位显示、动态图例、图表参考线、柱图刻度居中风格切换、混合图表及同数据源图表类型切换等。

1. [A-MusicView](https://github.com/north2014/A-MusicView)

	Canvas实时绘制音乐波形图，Canvas动态绘图，涉及碰撞检测，动画效果很赞，而且代码百分百全注释。

1. [pull-back-layout](https://github.com/oxoooo/pull-back-layout)

	下拉返回布局。

1. [android-vertical-slide-view](https://github.com/xmuSistone/android-vertical-slide-view)	

	仿照淘宝和聚美优品，在商品详情页，向上拖动时，可以加载下一页。使用ViewDragHelper，滑动比较流畅。ScrollView滑动到底部的时候，再行向上拖动时，添加了一些阻力。

### 工具	

1. [android-classyshark](https://github.com/googlesamples/android-classyshark)

	Android executables browser [http://www.api-solutions.com/p/classyshark.html](http://www.api-solutions.com/p/classyshark.html)

### 视频

1. [Android Performance Patterns Season 4](http://t.cn/Ry3HYnT)

	官方推出的一系列Android应用性能优化视频第四季，观看请自备“梯子”。

###设计

1. [如何成为交互设计师？](http://www.zhihu.com/question/20827149/answer/65191954)

	一个知乎上问答，可以作为自学指导，适用于完全不在相关圈子里的外行入门，可以通过这个方法找到一份初级设计师工作或申请到交互设计专业学校。但效果完全看个人天赋和水平了。

----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh3)