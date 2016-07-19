layout: post
title: "Android开发技术周报特刊之React Native"
date: 2015-11-09 21:27:42 +0800
comments: true
categories: AndroidDevSpecialWeekly 
---

# Android开发技术周报特刊之React Native

### 教程	

#### 基础入门 

1. [React Native入门指南](https://github.com/vczero/react-native-lession)

	一个React Native入门指南系列教程。

1. [React Native for Android 入门老虎](http://www.race604.com/react-native-for-android-start/)

	期待已久的 React Native for Android 发布了，赶紧来尝试一下，我跟着这个 Getting Started 开开始入门。发现被一些 "老虎" 堵在门口， Hello World 都跑不起来，入不了 React Native 的门，让我很懊恼，最后终于解决。可能大家也会遇到类似的问题，这篇文章希望能帮到你。
	
1. [学习 React Native for Android：环境搭建](http://hahack.com/codes/learn-react-native-for-android-01/)
	
	Facebook 于 2015 年 9 月 15 日发布了 React Native for Android 。React Native 让开发者使用 JavaScript 和 React 编写应用，利用相同的核心代码就可以创建 Web，iOS 和 Android 平台的原生应用。注意这里的 核心 两个词，它指的是那些底层的、与界面无关的逻辑。

1. [学习 React Native for Android：React 基础](http://hahack.com/codes/learn-react-native-for-android-02/)

	React Native 主张用 React 的开发思维来编写 UI 层。因此在学习 React-Native 之前，了解基本的 React 的语法和存在的坑会对今后 React Native 的开发大有裨益。本文将从一个简单的例子开始，逐步完善我们的程序。在这个过程中，我们将一步步探讨如何用 React 来开发网页应用，以及需要注意的陷阱。

1. [【入门篇】react-native](http://segmentfault.com/a/1190000004112878)

	这里以编写react-native android应用程序作为例子来讲解（为毛不用IOS？因为没有mac，也不想装黑苹果）

#### 基础进阶

1. [【布局篇】react-native](http://segmentfault.com/a/1190000004154982)	
	这里以三种经典布局来讲解react-native布局概念，主要以flexbox为主，react native中有两个基本元素< View >与< Text >，分别类似于web端div和span，用于布局和修饰。需要注意的是，react native不是所有的CSS属性都支持，这里有react native所支持的CSS属性

1. [Android React Native自定义组件的流程](http://blog.csdn.net/sbsujjbcy/article/details/49946749)

	假设我们现在有这么一个需求，就是自定义一个组件，该组件由一个小图标和图标的文字说明组成，并且带有背景色，背景色可设置，宽度高度可设置。

1. [Android React Native使用原生模块](http://blog.csdn.net/sbsujjbcy/article/details/49953041)

	有时候我们的App需要访问平台API，并且React Native可能还没有相应的模块包装；或者你需要复用一些Java代码，而不是用Javascript重新实现一遍；又或者你需要实现某些高性能的、多线程的代码，譬如图片处理、数据库、或者各种高级扩展等等。 而用React Native可以在它的基础上编写真正原生的代码，并且可以访问平台所有的能力。如果React Native还不支持某个你需要的原生特性，你应当可以自己实现该特性的封装。

1. [Android React Native在Android Studio中执行bundleReleaseJsAndAssets 打包失败的解决方法](http://blog.csdn.net/sbsujjbcy/article/details/49966909)

	这个坑在文章记一次在Windows上搭建React Native Android环境踩过的坑中我已经提到过，当时找不到解决方法，只能开一个命令提示符终端独立执行打包。

1. [Android React Native加载图片资源的正确姿势](http://blog.csdn.net/sbsujjbcy/article/details/49981529)

	在这篇文章中Android React Native的使用细节问题提到了 图片使用的问题，也提到了无论用哪种方法都不能加载app内部的图片资源的问题，当时的代码是这样子的 `<Image source={ require('image!icon') } />` 在官方文档中也是这么写的[Image](http://facebook.github.io/react-native/docs/image.html#content)

1. [Android React Native使用原生UI组件](http://blog.csdn.net/sbsujjbcy/article/details/49995407)

	Android React Native 已经将几个常用的原生组件进行了封装，比如 ScrollView 和 TextInput，但是并不是所有系统的原始组件都被封装了，因此有的时候我们不得不自己动手封装一下，从而能够使用那些React Native没有为我们封装的原生组件，比如WebView，官方并没有提供Android端的实现，那么我们现在就动手封装一下WebView。

1. [Andriod React Native 样式表中可用样式属性](http://blog.csdn.net/sbsujjbcy/article/details/50017029)

	写了这么多篇Android React Native的博文，基本上把复杂的东西都搞定了，接下来来看看一些轻松的东西，和布局有关，就是css样式，那么一个View可以设置哪些css样式呢，是和web中的css样式完全一样呢，还是有所不同呢？其实你只要在样式表中书写一个不存在的样式，就会报一大堆错，提示你该样式不存在，然后提供所有可用的样式给你。


1. [React Native For Android の 修改React Native为本地依赖](http://www.jianshu.com/p/cca40c19faa0)

	RN的aar包托管在Bintray上面，因此，我们可以自己将其下载下来，从而将在线依赖＋下载 改为 手动下载＋本地依赖。打开bintray搜索react-native，可以查找到React Native的官方Bintray网址，在这个主页中，可以看到RN的一系列版本，最新的是0.15.1。

1. [React Native  的兼容性（Android、iOS）](http://segmentfault.com/a/1190000003883126)

	刚开始学习RN的时候，写的代码只支持 iOS 版本，写起来感觉还是比较顺手的，也没有太多的疑难杂症，以及模拟器不支持一些标签的情况，今天写了支持 Android 版本的代码后，我整个人都不好了。。。

1. [React Native 操作 “DOM”](http://segmentfault.com/a/1190000003975609)

	在弄react-native的时候，突然发现它不能像js一样获取页面的dom，那如果我要修改一些dom的属性值、文本什么的，要怎么做呢？后来查谷歌，发现了一个名词：虚拟DOM。React在内存中维护一个快速响应的DOM描述。render()方法返回一个DOM的描述，React能够利用内存中的描述来快速地计算出差异，然后更新浏览器中的DOM。

1. [React Native 图片](http://www.jianshu.com/p/b7008a6ac5fc)

#### 动手实践

1. [React Native for Android 实践 - 实现知乎日报客户端](http://www.race604.com/react-native-android-practice/)

	React Native for Android 的发布，对一个 Android 开发者来说还是有相当的吸引力的。通过前面这篇博客：React Native for Android 入门老虎好不容易入了门了，然后想找一个简单的项目，来练练手。一方面来熟悉一下 RN（React Native, 后面都做此简写），另一方面来验证使用 RN 来实现一个相对完整的项目的可行性。

1. [React Native for Android 发布独立安装包](http://www.race604.com/rn-android-standalone-apk/)

	如果要发布一个 React Native 写的 Android 应用，不可能要别人来连接这个 JS Server。可不可以不要连接这个 Server 就能运行呢？在网上找了一圈，发现资料很少，官方文档上也没有说支持。这篇文章就来讨论一种实现方案。

1. [使用 BaaS 工具 与 React Native 构建原生应用](http://segmentfault.com/a/1190000004142461)

	本文将介绍：如何在 React Native 中使用 Flux 架构来组织应用的数据流，以配合我们的JavaScript SDK 向 LeanCloud 云端保存数据，重用代码和实现平台差异化。异步获取当前用户对象、文件上传、向移动端推送消息。
	
1. [React-native Android 热更新](http://richard-cao.github.io/2015/12/03/React-native-Android-热更新/)

	首先说下网上已有的方案，这是我找到的方案，并且测试确实可以热更新的：React-Native-Remote-Update。简述下这个方案实现热更新原理是反射调用了ReactInstanceManagerImpl中的如下方法：然后通过自定义JSBundleLoader将bundle指向的文件重定向，反射调用这个方法就可以实现热更新，重新加载重定向之后的bundle文件，这个bundle文件就是从服务端下载好的。

#### 深入理解 

1. [React Native 中组件的生命周期](http://www.race604.com/react-native-component-lifecycle/)

	就像 Android 开发中的 View 一样，React Native（RN） 中的组件也有生命周期（Lifecycle）。所谓生命周期，就是一个对象从开始生成到最后消亡所经历的状态，理解生命周期，是合理开发的关键。
	
1. [你为什么应该试一试Reflux？](http://icodeit.org/2015/11/get-started-with-reflux/)	
	React在设计之初就只关注在View本身上，其余部分如数据的获取，事件处理等，全然不在考虑之内。不过构建大型的Web前端应用，这些点又实在不可避免。所以Facebook的工程师提出了前端的Flux架构，这个架构的最大特点是单向数据流（后面详述）。但是Flux本身的实现有很多不合理的地方，比如单例的Dispatcher会在系统中有多种事件时导致臃肿的switch-cases等。

1. [React-Native With Redux](http://richard-cao.github.io/2016/01/12/React-Native-With-Redux/)

	那么Redux是什么呢？Redux是javascript状态容器，提供可预测化的状态管理，可以构建一致化的应用，除了和React一起用外，还支持其他界面库，体积小（只有2kb）而且没有任何依赖。Redux由Flux演变而来，但是避开了Flux的复杂性，上手快，使用简单，而且社区活跃，是目前主流的Flux数据流框架。

#### 源码分析

1. [React Native Android版核心层js-bridge实现浅析](http://supercocoa.github.io/2015/09/26/react_native_android_js_bridge/)

	整体架构上，可以分为java层<->c++层<->js层，其中java层作为入口，主要是对整体流程的控制，模块的配置。c++层是对JavaScriptCore接口的封装（每个应用自己背一个js解释器），直接执行js脚本并获取返回值。js层则是界面的布局与事件的响应处理。
	
1. [ReactNative源码分析：Java组件如何调用JSX](http://www.jianshu.com/p/ff4e1b41c1cc)
	
	ReactNative是facebook最近推出的在Android上支持React的平台，目前看的话运行效率与社区反馈都非常不错，值得深入学习。本文主要在源码上分析了Java组件如何最终能够调用JSX的方法细节。

1. [React 源码剖析系列 － 不可思议的 react diff](http://segmentfault.com/a/1190000004003055	)

	React diff 作为 Virtual DOM 的加速器，其算法上的改进优化是 React 整个界面渲染的基础，以及性能提高的保障，同时也是 React 源码中最神秘、最不可思议的部分，本文从源码入手，深入剖析 React diff 的不可思议之处。

1. [ReactNativeAndroid源码分析-Js如何调用Native的代码](http://zhuanlan.zhihu.com/program-life/20464825)

	index.android.js是ReactNative的入口文件，后缀Android表示是在Android平台使用的代码。ReactNative内置了babel，所以可以使用最新的JavaScript语法来开发（ECMAScript6简称es6），不熟悉es6的同学可以看看阮一峰写的这本[e6入门教程](ECMAScript 6入门)。

#### 架构设计

1. [ReactNative组件状态设计思考](http://segmentfault.com/a/1190000004180955)

	按照原来设计组件的方法论，一个UI组件对外应该具有属性、事件、接口，对内具有内部属性，内部接口。1.属性就像一份配置文件，描述了组件应该具有的功能、外观或者初始状态。2.事件是组件在工作工程中，当满足某种条件的时候触发的回调函数。3.接口是组件对象的方法，可以让组件去执行某个任务

1. [React Native 的架构设计](http://segmentfault.com/a/1190000004161358)

	请注意，本篇写的是react native的架构设计，如果你用react来开发web程序，本篇文章只能仅供参考，问题都没有在web上去考虑过。本篇较长，前面是目前flux开源框架的一些分析，后面是架构设计过程。您可以直奔主题。用RN最大的难题是设计思想的转变，以前的设计方法论已经不太适用了。而RN仅仅提供了view的框架，构建完整app的架构并没有直接提供。

#### 踩的那些坑

1. [ReactNative Android 10个最常见问题](https://github.com/yipengmu/ReactNative_Android_QA)

	这里逐条记录下最容易遇到的React native android 相关case。

1. [Android React Native的使用细节问题](http://blog.csdn.net/sbsujjbcy/article/details/49946217)

	踩了几天React Native Android的坑。总结为一句话，目前android学习react native还为时过早，坑太多，需要你慢慢去踩。就目前来讲，能踩的坑基本上都踩了一遍，所以还是等它稳定下来再去学吧，否则会浪费掉一大堆时间。在React Native中，组件的宽度，高度都是不用写单位的，你写个100，在Android中代表的到底是100px还是100dp，就不得而知了，这时候自己实践一下就一目了然了。

1. [React Native for Android 热部署图片解决方案](http://blog.csdn.net/kid1986513/article/details/50337083)

	热部署时，我们期望升级包中包含js代码与图片资源。bundle的热部署网上已经有两种方案了，一种是用反射，一种是利用RN自带函数，将bundle初始化时直接放到指定目录下，之后通过替换bundle文件实现代码热部署。我们希望图片也可以实现热部署，下面是一个比较简单的解决方案。
	
1. [ReactNative 开发实践](http://www.jianshu.com/p/6d4cce9d914f)

	这是一个在StuQ做分享时的讲稿。当然还有很大的改进空间，但我这会却没有什么劲头继续改进，既然这样就不如索性先发出来，先把它从脑袋清出来，把其它我更想做的事情做了，回头再看哪天想改了再回来改。


1. [多React Native项目时依赖管理的最佳实践](http://segmentfault.com/a/1190000004278414)

	在实际开发过程中，经常需要同时运行和修改多个React Native工程，比如运行github上的开源项目以观察某种控件的实际效果。那么此时，各项目下的初始化(npm install)就会非常的痛苦，因为React Native的文件非常大，以0.17.0为例，安装后达到309MB。尽管，我们可以通过阿里npm等镜像站的方式加速下载的过程，但是下载后的进一步编译也非常地耗时。

#### 系列教程

1. [React-Native入门指南](https://github.com/vczero/react-native-lession)


### 文档

1. [React Native 官方文档中文版](http://wiki.jikexueyuan.com/project/react-native/)

	Facebook 在 React.js Conf 2015 大会上推出了基于 JavaScript 的开源框架 React Native，本中文教程翻译自 React Native 官方文档。React Native 结合了 Web 应用和 Native 应用的优势，可以使用 JavaScript 来开发 iOS 和 Android 原生应用。在 JavaScript 中用 React 抽象操作系统原生的 UI 组件，代替 DOM 元素来渲染等。

### 开源库

1. [react-native-desktop](https://github.com/ptmt/react-native-desktop) By GitHubDaily

	能够帮助开发者使用 React Native 快速构建自己的 Mac OS 应用, 目前各项功能还在完善中, 因此暂不建议直接用到生产环境上。

1. [react-native-camera](https://github.com/lwansbrough/react-native-camera) By OSChina

	react-native-camera 是 React Native 的摄像头 viewport。这个模块应用于开发的早期阶段，它支持摄像头的转换和基本图片捕捉。

1. [react-native-video](https://github.com/brentvatne/react-native-video)

	是一个 `<Video>` 标签控件。

1. [react-native-carousel](https://github.com/nick/react-native-carousel)

	一个简单的 React Native 轮播控件。
	
1. [react-native-refreshable-listview](https://github.com/jsdf/react-native-refreshable-listview)

	一个下拉刷新 ListView，当数据重载的时候显示加载提示。

1. [react-native-modal](https://github.com/brentvatne/react-native-modal)

	是 React Native 的 <Modal> 组件。

1. [react-native-htmltext](https://github.com/siuying/react-native-htmltext)

	可以用 HTML 像 Markup 一样，在 ReactNative 里创建程式化的文本。ReactNative 为程式化文本提供一个文本元素，用于取代 NSAttributedString，你可以创建嵌套的文本。

1. [react-native-linear-gradient](https://github.com/brentvatne/react-native-linear-gradient)

	一个 React Native 的 LinearGradient 组件。

1. [react-native-looped-carousel](https://github.com/appintheair/react-native-looped-carousel)

	是基于 React Native 的环形传送。

1. [MRN](https://github.com/binggg/mrn)

	一个基于React Native的Material Design风格的组件库。
	
1. [React-Native-Maps](https://github.com/lelandrichardson/react-native-maps)

	React Native Mapview component for iOS + Android。

### 完整开源项目


1. [DoubanMovie-React-Native](https://github.com/fengjundev/DoubanMovie-React-Native)

	用 React Native 开发的豆瓣电影客户端

1. [HackerNews-React-Native](https://github.com/iSimar/HackerNews-React-Native)

	用 React Native 开发的 HackerNews 客户端

1. [煎蛋客户端](https://github.com/w4lle/JianDan-React-Native)

	用 React Native 开发的煎蛋客户端

1. [知乎日报Android版](https://github.com/race604/ZhiHuDaily-React-Native) 

	用 React Native 开发的知乎日报客户端

1. [ziliun-react-native](https://github.com/sonnylazuardi/ziliun-react-native
) 

	ZiLiun 这个网站上的文章阅读 App。

1. [FinanceReactNative](https://github.com/7kfpun/FinanceReactNative)

	一个股票 App，包含 iOS 和 Android 实现。

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
	
> 版权声明：欢迎自由转载-非商用-非衍生-保持署名 | [Creative Commons BY-NC-ND 4.0](http://creativecommons.org/licenses/by-nc-nd/4.0/)