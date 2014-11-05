---
layout: post
title: "Android开发周报 Issue#5"
date: 2014-11-05 17:45:47 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发周报 Issue#5


### 文章

1. [进入Material Design时代](http://blog.csdn.net/xushuaic/article/details/40627389)

	Material Design是Android 5.0系统的重头戏，并在以后App中将成为一种设计标准，而且随着已支持Android 5.0 Lollipop的Nexus 6的开售，Google希望开发者更快的支持Material Design，连续发了3篇文章，来帮助开发者如何在自己的App 中实现Material Design。并表示：expect Winter 2014 to be a big quarter for design on Android.

1. [Android中View大小的确定过程](http://www.liaohuqiu.net/cn/posts/how-does-android-caculate-the-size-of-child-view/)

	子View有一个期望的尺寸大小，父容器有尺寸大小约束，这两方面的约束协调，用来计算View的大小状态。根据父容器的尺寸状态，以及子View的LayoutParams，可以确定子View的大小和状态：MeasureSpec，并要求子View确定自身大小。调用子View的measure()方法，子View的onMeasure()方法也会被执行。子View在onMeasure()方法中，根据父容器给出的尺寸大小和约束，根据自身情况，确定最终的大小。父容器根据子View的确定的大小，最终确定自身大小。

1. [ScheduledThreadPoolExecutor实现原理](http://www.ticmy.com/?p=329)

	自jdk1.5开始，Java开始提供ScheduledThreadPoolExecutor类来支持周期性任务的调度，在这之前，这些工作需要依靠Timer/TimerTask或者其它第三方工具来完成。但Timer有着不少缺陷，如Timer是单线程模式，调度多个周期性任务时，如果某个任务耗时较久就会影响其它任务的调度；如果某个任务出现异常而没有被catch则可能导致唯一的线程死掉而所有任务都不会再被调度。ScheduledThreadPoolExecutor解决了很多Timer存在的缺陷。

1. [Android-IM架构设计](http://mogu.io/android-im-design)

	文章介绍了蘑菇街开源的IM项目Android客户端的整体架构和消息流程。


1. [Android 命名规范（提高代码可以读性）](http://blog.csdn.net/vipzjyno1/article/details/23542617)	
	刚接触android的时候，命名都是按照拼音来，所以有的时候想看懂命名的那个控件什么是什么用的，就要读一遍甚至好几遍才知道，这样的话，在代码的审查和修改过程中就会浪费不少不必要的时间。如果就是我一个人开发，一个人维护的话还好，可是如果一个项目是团队分工合作，这样让你的同事去看你的代码就更加吃力了，因为大家之间的编程方式不一样，所以，在开发过程中，命名规范统一尤为重要，最好是团队中统一好大家命名方法，这样对于日后的工作会轻松很多。

<!--more-->


### 代码&开源库

1. [android-GridViewWithHeaderAndFooter](https://github.com/liaohuqiu/android-GridViewWithHeaderAndFooter)

	在HeaderGridView的基础上做了更改，可以addHeaderView()和addFooterView()的GridView来了。用法和ListView一样.

1. [Skycons](https://github.com/torryharris/Skycons)

	一组自定义的天气图标View库。

1. [ValueBar](https://github.com/PhilJay/ValueBar)
	
	一个漂亮的自定义View。工作原理类似于Seeker。支持API level 11+.

1. [caffeine](https://github.com/percolate/caffeine)

	一个可以加速Android开发的工具库。

1. [TeamTalk](https://github.com/mogutt)

	蘑菇街开源的 IM 项目 TeamTalk，包括 Android、iOS、Win、Mac 客户端以及 Server端、管理后台、环境自动部署，大赞！支持文字、音频、图片、表情、文件传输、屏幕振动、分组等，做聊天的同学可以看看.

1. [sweet-alert-dialog](https://github.com/pedant/sweet-alert-dialog)

	Android版的SweetAlert，清新文艺，快意灵动的甜心弹框。
	
	![image](https://github.com/pedant/sweet-alert-dialog/raw/master/change_type.gif)
	
1. [android-split-pane-layout](https://github.com/MobiDevelop/android-split-pane-layout)
	
	可以将2个子View之间的可用空间按照指定比例分割的自定义Layout。
	  

### 视频

1. [Android DevBytes and Google IO视频](https://github.com/KevinChen9117/ikevin)

	Youtube上的Google IO、跟Android相关的DevBytes、Android Design In Action和跟Android相关的DesignBytes视频，全部是720P的mp4. 包含英文字幕。


### 工具

1. [Android Studio 0.9.0 Released](http://tools.android.com/download/studio/canary)

	Android Studio 0.9.0 released to the canary channel! 
	这次发布添加了新版本的Android Gradle plugin 0.14.0，此外，修复了一些bug等。

1. [ios2android](https://github.com/matheusjardimb/ios2android)

	一个可以将iOS格式的切图转换为Android格式切图的Python脚本工具。

### 设计

#### 工具&资源
	
1. [高效神器！21款强大实用的PHOTOSHOP扩展插件](http://www.uisdc.com/21-photoshop-plugins-for-designer)
	
	21款扩展插件，特别适合网页设计师。这些神器可以让平时复杂繁琐的操作变得更加简单.
	
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh)