layout: post
title: "Android开发技术周报 Issue#47"
date: 2015-08-31 22:06:42 +0800
comments: true
categories: AndroidDevWeekly
---

#Android开发技术周报 Issue#47

### 教程

1. [Android内存泄露案例分析](http://www.csdn.net/article/2015-09-07/2825631)

	一款优秀的Android应用，不仅要有完善的功能，也要有良好的体验，而性能是影响体验的一个重要因素。内存泄露是Android开发中常见的性能问题。这篇文章，通过我们曾经遇到的一个真实的案例，来讲述一个内存泄露问题，从发现到分析定位，再到最终解决的全过程。

1. [Android微信上的SVG](https://mp.weixin.qq.com/s?__biz=MzAwNDY1ODY2OQ==&mid=207863967&idx=1&sn=3d7b07d528f38e9f812e8df7df1e3322)

	面对android的各种dpi某事，想要所有设备上的图片都能有最清晰的效果，就意味着每种dpi模式都必须提供一份对应尺寸的资源，除非你不在乎安装包的体积有多大，所以这显然是不可能去做的。在过去的几年里andorid从mdpi发展到xxxhdpi，每当微信想让相同的图片在更清晰的屏幕上显示我们想要的效果时，我们总要重新提供一份体积更大的高清png并且删掉可能不太多使用的小分辨率图片。

1. [MAT - Memory Analyzer Tool 使用进阶](http://www.lightskystreet.com/2015/09/01/mat_usage/)

	尽管Java虚拟机可以帮我们对内存进行回收，但是其回收的是Java虚拟机不再引用的对象。很多时候我们使用系统的IO流，Cursor，Receiver如果不及时释放，就会导致内存泄漏，这些场景是常见的，一般开发人员也都能够避免。但是，很多时候内存泄漏的现象不是很明显，比如内部类，Handler相关的使用导致的内存泄漏，或者你使用了第三方library的一些引用，比较消耗资源，但又不是像系统资源那样会引起你足够的注意去手动释放它们。

1. [微信ANDROID客户端-会话速度提升70%的背后](https://mp.weixin.qq.com/s?__biz=MzAwNDY1ODY2OQ==&mid=207548094&idx=1&sn=1a277620bc28349368b68ed98fbefebe)

	背景：打开会话速度慢，在同一个会话有较多的历史消息下，各种查询，更新,删除等操作，速度明显下降。在会话内有较大量历史消息情况下，进入速度/刷新速度明显降低。分析阶段：整个优化我们分2个阶段进行：第一阶段,针对历史记录较小的会话，通过Android自带的trace工具分析，我们发现较大的耗时分布在进入会话的几个关键点：在打开会话过程中涉及的磁盘读写操作，加载会话UI所执行的inflate操作（inflate指的是创建View对象）

1. [BDD在移动开发中的应用](http://insights.thoughtworkers.org/bdd-testing-in-mobile/)

	移动应用程序现在已经非常普及，大多数的应用可以支持3种主流平台:iOS、Android和Windows phones。此外Firefox OS平台的市场占有率也在不断提升中。应用程序的功能是与平台无关的。但是不同的平台还是会有差异，例如处理消息事件的方式等。测试移动应用程序，并保证它们能在所有的平台上正常工作，是一项很有挑战的工作。

1. [Tools 命名空间的使用与 Support Library Annotations 介绍](http://yanghui.name/blog/2015/08/31/tools-namespace-and-support-library-annotations/)	
	tools 命名空间是在 Android Studio 中引入的 编辑预览特性，可以生成一些只在 IDE 预览界面生效的特性。

1. [Android关于Theme.AppCompat相关问题的深入分析](http://www.jianshu.com/p/6ad7864e005e)

	Android的SDK版本很多，新的SDK版本包含了很多新的特性，为此Google官方提供Android Support Library package来保证高版本SDK的向下兼容。通过使用此包，可以让拥有最新SDK特性的应用运行在API lever 4(即Android 1.6) 及更高版本的设备之上。

1. [Java8 lambda表达式10个示例](http://www.importnew.com/16436.html)

	我个人对Java 8发布非常激动，尤其是lambda表达式和流API。越来越多的了解它们，我能写出更干净的代码。虽然一开始并不是这样。第一次看到用lambda表达式写出来的Java代码时，我对这种神秘的语法感到非常失望，认为它们把Java搞得不可读，但我错了。

### 代码&开源库

1. [ListViewWithSofPpanel](https://github.com/nimengbo/ListViewWithSofPpanel)

	模仿微信朋友圈列表中嵌套列表，点某个评论弹出键盘效果。

1. [Tabby](https://github.com/hitherejoe/Tabby)

	 Android Custom Tabs 支持库的Demo项目。

1. [Android-PickerView](https://github.com/saiwu-bigkoo/Android-PickerView)

	仿iOS的PickerView控件，有时间选择和选项选择并支持一二三级联动效果.

1. [WashingMachineView](https://github.com/naman14/WashingMachineView)

	一个洗衣机洗衣服动画效果的自定义的View。

1. [Pixelate](https://github.com/DanielMartinus/Pixelate)

	一个可以将图片像素化显示的自定义ImgeView

1. [FAB-Loading](https://github.com/smasoumi/FAB-Loading)

	在Floating Action Button上实现了loading动画效果。

### 工具

1. [PP鸭](http://ppduck.com)

	PP鸭使用优秀的算法，自动完成图片压缩任务。在保证图片品质的前提下，使图片体积得到压缩。PP鸭支持图片批量导入导出、压缩前后视觉比较，显示压缩比，手动微调参数等。

1. [vectalign](http://www.jcodecraeer.com/a/opensource/2015/0905/3421.html)

	我们知道4.4以后AnimatedVectorDrawable可以让两个SVG图像无缝过渡（称为变形动画），但是这两个svg图像的path必须参数个数要相等，同时这些参数的类型要匹配（也就是说格式要对齐）。这个工具就是通过命令行的方式将任意两个svg资源转换成匹配的模式。

### 视频	

1. [Android内存泄漏案例分析](http://edu.csdn.net/course/detail/1377)

	一款优秀的Android应用，不仅要有完善的功能，也要有良好的体验，而性能是影响体验的一个重要因素。内存泄露是Android开发中常见的性能问题。这次公开课，通过我们曾经遇到的一个真实的案例，来演示一个内存泄露问题，从发现到分析定位，再到最终解决的全过程。

1. [Android Design for Developers](https://www.udacity.com/course/android-design-for-developers--ud862)

	Google 在 Udacity 上新推出的 5 课时 Android 设计课程。

----
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)