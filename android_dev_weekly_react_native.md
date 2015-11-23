layout: post
title: "Android开发技术周报特刊之React Native"
date: 2015-11-09 21:27:42 +0800
comments: true
categories: AndroidDevSpecialWeekly 
---

# Android开发技术周报特刊之React Native

<a href="http://t.cn/RUTw0f5" target="_blank"><img src="http://ww1.sinaimg.cn/large/8a41f469jw1ey0uhi2xobj20nm0283zf.jpg" title="卖苹果啦！一位程序员小伙伴在帮家里卖苹果，有需要的小伙伴，可以买一箱尝尝，现摘现发，还包邮哦！"></a>

### 教程	

#### 基础入门 

1. [React Native for Android 入门老虎](http://www.race604.com/react-native-for-android-start/)

	期待已久的 React Native for Android 发布了，赶紧来尝试一下，我跟着这个 Getting Started 开开始入门。发现被一些 "老虎" 堵在门口， Hello World 都跑不起来，入不了 React Native 的门，让我很懊恼，最后终于解决。可能大家也会遇到类似的问题，这篇文章希望能帮到你。
	
1. [学习 React Native for Android：环境搭建](http://hahack.com/codes/learn-react-native-for-android-01/)
	
	Facebook 于 2015 年 9 月 15 日发布了 React Native for Android 。React Native 让开发者使用 JavaScript 和 React 编写应用，利用相同的核心代码就可以创建 Web，iOS 和 Android 平台的原生应用。注意这里的 核心 两个词，它指的是那些底层的、与界面无关的逻辑。

1. [学习 React Native for Android：React 基础](http://hahack.com/codes/learn-react-native-for-android-02/)

	React Native 主张用 React 的开发思维来编写 UI 层。因此在学习 React-Native 之前，了解基本的 React 的语法和存在的坑会对今后 React Native 的开发大有裨益。本文将从一个简单的例子开始，逐步完善我们的程序。在这个过程中，我们将一步步探讨如何用 React 来开发网页应用，以及需要注意的陷阱。

1. [ReactNative Android 10个最常见问题](https://github.com/yipengmu/ReactNative_Android_QA)

	这里逐条记录下最容易遇到的React native android 相关case。

1. [Android React Native的使用细节问题](http://blog.csdn.net/sbsujjbcy/article/details/49946217)

	踩了几天React Native Android的坑。总结为一句话，目前android学习react native还为时过早，坑太多，需要你慢慢去踩。就目前来讲，能踩的坑基本上都踩了一遍，所以还是等它稳定下来再去学吧，否则会浪费掉一大堆时间。在React Native中，组件的宽度，高度都是不用写单位的，你写个100，在Android中代表的到底是100px还是100dp，就不得而知了，这时候自己实践一下就一目了然了。

#### 动手实践

1. [React Native for Android 实践 - 实现知乎日报客户端](http://www.race604.com/react-native-android-practice/)

	React Native for Android 的发布，对一个 Android 开发者来说还是有相当的吸引力的。通过前面这篇博客：React Native for Android 入门老虎好不容易入了门了，然后想找一个简单的项目，来练练手。一方面来熟悉一下 RN（React Native, 后面都做此简写），另一方面来验证使用 RN 来实现一个相对完整的项目的可行性。

1. [React Native for Android 发布独立安装包](http://www.race604.com/rn-android-standalone-apk/)

	如果要发布一个 React Native 写的 Android 应用，不可能要别人来连接这个 JS Server。可不可以不要连接这个 Server 就能运行呢？在网上找了一圈，发现资料很少，官方文档上也没有说支持。这篇文章就来讨论一种实现方案。

1. [React Native For Android の 修改React Native为本地依赖](http://www.jianshu.com/p/cca40c19faa0)

	RN的aar包托管在Bintray上面，因此，我们可以自己将其下载下来，从而将在线依赖＋下载 改为 手动下载＋本地依赖。打开bintray搜索react-native，可以查找到React Native的官方Bintray网址，在这个主页中，可以看到RN的一系列版本，最新的是0.15.1。

1. [Android React Native加载图片资源的正确姿势](http://blog.csdn.net/sbsujjbcy/article/details/49981529)

	在这篇文章中Android React Native的使用细节问题提到了 图片使用的问题，也提到了无论用哪种方法都不能加载app内部的图片资源的问题，当时的代码是这样子的 `<Image source={ require('image!icon') } />` 在官方文档中也是这么写的[Image](http://facebook.github.io/react-native/docs/image.html#content)

#### 深入理解 

1. [React Native 中组件的生命周期](http://www.race604.com/react-native-component-lifecycle/)

	就像 Android 开发中的 View 一样，React Native（RN） 中的组件也有生命周期（Lifecycle）。所谓生命周期，就是一个对象从开始生成到最后消亡所经历的状态，理解生命周期，是合理开发的关键。

1. [React Native Android版核心层js-bridge实现浅析](http://supercocoa.github.io/2015/09/26/react_native_android_js_bridge/)

	整体架构上，可以分为java层<->c++层<->js层，其中java层作为入口，主要是对整体流程的控制，模块的配置。c++层是对JavaScriptCore接口的封装（每个应用自己背一个js解释器），直接执行js脚本并获取返回值。js层则是界面的布局与事件的响应处理。
	
1. [ReactNative源码分析：Java组件如何调用JSX](http://www.jianshu.com/p/ff4e1b41c1cc)
	
	ReactNative是facebook最近推出的在Android上支持React的平台，目前看的话运行效率与社区反馈都非常不错，值得深入学习。本文主要在源码上分析了Java组件如何最终能够调用JSX的方法细节。

1. [React 源码剖析系列 － 不可思议的 react diff](http://segmentfault.com/a/1190000004003055	)

	React diff 作为 Virtual DOM 的加速器，其算法上的改进优化是 React 整个界面渲染的基础，以及性能提高的保障，同时也是 React 源码中最神秘、最不可思议的部分，本文从源码入手，深入剖析 React diff 的不可思议之处。
	
1. [你为什么应该试一试Reflux？](http://icodeit.org/2015/11/get-started-with-reflux/)	
	React在设计之初就只关注在View本身上，其余部分如数据的获取，事件处理等，全然不在考虑之内。不过构建大型的Web前端应用，这些点又实在不可避免。所以Facebook的工程师提出了前端的Flux架构，这个架构的最大特点是单向数据流（后面详述）。但是Flux本身的实现有很多不合理的地方，比如单例的Dispatcher会在系统中有多种事件时导致臃肿的switch-cases等。
	
### 文档

1. [React Native 官方文档中文版](http://wiki.jikexueyuan.com/project/react-native/)

	Facebook 在 React.js Conf 2015 大会上推出了基于 JavaScript 的开源框架 React Native，本中文教程翻译自 React Native 官方文档。React Native 结合了 Web 应用和 Native 应用的优势，可以使用 JavaScript 来开发 iOS 和 Android 原生应用。在 JavaScript 中用 React 抽象操作系统原生的 UI 组件，代替 DOM 元素来渲染等。

### 开源库

1. [DoubanMovie-React-Native](https://github.com/fengjundev/DoubanMovie-React-Native)

	

1. [react-native-desktop](https://github.com/ptmt/react-native-desktop) by GitHubDaily

	能够帮助开发者使用 React Native 快速构建自己的 Mac OS 应用, 目前各项功能还在完善中, 因此暂不建议直接用到生产环境上。

### PPT

1. [用 React Native 做 Android 开发 (by @Android笔记)](http://183.91.33.12/cache/7xo6sn.dl1.z0.glb.clouddn.com/React-Native-GDG-2015.pdf)

### 视频教程

1. [React Native 快速入门](http://www.jikexueyuan.com/course/1504.html)

	本课时介绍 React Native ，包括 React Native 的简介，主要解决的问题以及为什么我们需要关注 React Native，然后和其他同类框架做一个简单地对比。

1. [React Native 布局指南](http://www.jikexueyuan.com/course/1489.html)

	本课时讲解 React Native 的样式布局基础，包括如何添加和使用样式，以及介绍作为 Css 子集的基本盒模型布局方式。
	
1. [React Native中文视频教程](http://www.ejiakt.com/album/show/211)

	这套教程就从基础出发讲述了react native的基础概念。学些react native将会是未来的移动开发的主流。
	
### 资源合集

1. [React-Native学习指南](https://github.com/ele828/react-native-guide)

	React-Native指南汇集了react-native学习资源与各类开源app.

1. [awesome-react-native](https://github.com/jondot/awesome-react-native)

	An "awesome" type curated list of React Native components, news, tools, and learning material。
	
----
版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 3.0](http://creativecommons.org/licenses/by-nc-nd/3.0/deed.zh3)