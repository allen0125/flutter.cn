---
title: Flutter Documentation
title: Flutter 开发文档
short-title: Docs
short-title: 文档
description: The landing page for Flutter documentation.
description: Flutter 开发文档页面。
---

{% for card in site.data.docs_cards -%}
  {% capture index0Modulo3 %}{{ forloop.index0 | modulo:3 }}{% endcapture %}
  {% capture indexModulo3 %}{{ forloop.index | modulo:3 }}{% endcapture %}
  {% if index0Modulo3 == '0' %}
  <div class="card-deck mb-4">
  {% endif %}
    <a class="card" href="{{card.url}}">
      <div class="card-body">
        <header class="card-title">{{card.name}}</header>
        <p class="card-text">{{card.description}}</p>
      </div>
    </a>
  {% if indexModulo3 == '0' %}
  </div>
  {% endif %}
{% endfor -%}

## What's new on the site

## 网站更新

## 网站更新

To stay on top of Flutter announcements,
including breaking changes, join the
[flutter-announce](https://groups.google.com/forum/#!forum/flutter-announce)
Google group.

加入官方的 [flutter-announce](https://groups.google.com/forum/#!forum/flutter-announce)
邮件群组，以关注 Flutter 的相关通知，包括 breaking changes 等。

**July 9, 2019**

Flutter 1.9 is live!

Flutter 1.9 正式发布！

For the 1.9 release, Flutter's web support has been
merged ("unforked") into the main repo.
**Web support hasn't reached beta, and is not ready
to be used in production.**
Web and desktop support (which is also coming), will
impact the website, which was originally written
exclusively for developing Flutter mobile apps.
Some website updates are available now (and listed below),
but more will be coming.

随着 1.9 版本的发布，在 Web 平台运行
Flutter 的代码正式被合并到主 repo，但是
**在 Web 平台的支持尚未达到 Beta 阶段，请不要用在生产环节**。
Web 和即将到来的桌面端支持将会影响本站的内容，
如下列出了一些更新，更多的更新将会在稍后时间发布：

New and updated docs on the site include:

新的文档和更新包括：

* The Flutter layout codelab has been rewritten and
  uses the updated DartPad, the browser-based tool for running
  Dart code. DartPad now supports Flutter!
  [Try it out](/docs/codelabs/layout-basics)
  and let us know what you think.

  我们重写了 Flutter 布局的 codelab，
  使用了最新的、支持了 Flutter 的 DartPad，
  可以在 [这里](/docs/codelabs/layout-basics) 
  查看并告诉我们你的想法。
  
* The Performance view tool, which allows you to record
  and profile a session from your Dart/Flutter application,
  has been enabled in DevTools. For more information,
  see the [Performance
  view](/docs/development/tools/devtools/performance)
  page.

  开发者工具（DevTools）里的性能视图工具（Performance view tool），
  可以让你录制并检查 Dart 或 Flutter 应用的某个运行时 session，
  可以在这里查看更多：
  [使用性能视图 (Performance view)](/docs/development/tools/devtools/performance)
  
* A new page on
  [building a web application](/docs/get-started/web).

  新增一个页面，关于 [如何构建一个 Web 应用](/docs/get-started/web)。
  
* A new page on [creating responsive
  apps](/docs/development/ui/layout/responsive)
  in Flutter.
  
  新增一个页面，关于在 Flutter 里
  [如何创建响应式应用](/docs/development/ui/layout/responsive)

* A new page on
  [preparing a web app for release](/docs/deployment/web).

  新增一个页面，关于如何 [打包并发布到 Web 平台](/docs/deployment/web)。

* A new [web FAQ](/docs/development/platform-integration/web).
 
  关于在 Web 平台运行 Flutter 应用，我们新增了一个 
  [Web 常见问题页面](/docs/development/platform-integration/web)。
  
* The [Flutter for web](/web) page is updated.
  
  关于 [在 Web 平台运行 Flutter](/web) 的页面已经更新。
  
Happy Fluttering!

祝你在 Flutter 应用的开发中有一个愉快的经历和体验！

[What's new archive](/docs/whats-new-archive)

[最近更新归档页面](/docs/whats-new-archive)。

## New to Flutter?

## 新接触 Flutter 吗

Once you've gone through [Get Started](/docs/get-started/install),
including [Write Your First Flutter App,](/docs/get-started/codelab)
here are some next steps.

你可以从 [安装和环境配置](/docs/get-started/install) 开始，
也可以上手试试看 [第一个 Flutter 应用的开发](/docs/get-started/codelab)。

### Docs

### 文档

Coming from another platform? Check out: 
[Android](/docs/get-started/flutter-for/android-devs),
[iOS](/docs/get-started/flutter-for/ios-devs),
[Web](/docs/get-started/flutter-for/web-devs),
[React Native](/docs/get-started/flutter-for/react-native-devs),
[Xamarin.Forms](/docs/get-started/flutter-for/xamarin-forms-devs)

看我们为各种已经有相关平台开发经验的开发者准备的文档：
[给 Android 开发者的 Flutter 指南](/docs/get-started/flutter-for/android-devs)、
[给 iOS 开发者的 Flutter 指南](/docs/get-started/flutter-for/ios-devs)、
[给 React Native 开发者的 Flutter 指南](/docs/get-started/flutter-for/web-devs)、
[给 Web 开发者的 Flutter 指南](/docs/get-started/flutter-for/react-native-devs)、
[给 Xamarin.Forms 开发者的 Flutter 指南](/docs/get-started/flutter-for/xamarin-forms-devs)。

[Building layouts in Flutter](/docs/development/ui/layout)<br>
Learn how to create layouts in Flutter, where everything is a widget.

[Flutter 中的布局](/docs/development/ui/layout)<br>
学习如何在 Flutter 中创建布局，在 Flutter 里，所有事物都是 widget。

[Adding interactivity to your Flutter app](/docs/development/ui/interactive)<br>
Learn how to add a stateful widget to your app.
  
[为你的 Flutter 应用加入交互体验](/docs/development/ui/interactive)<br>
在 app 里使用有状态的 widget。

[A tour of the Flutter widget framework](/docs/development/ui/widgets-intro)<br>
Learn more about Flutter's react-style framework.
  
[Widgets 介绍](/docs/development/ui/widgets-intro)<br>
学习 Flutter 响应式框架的核心。

[FAQ](/docs/resources/faq)<br>
Get the answers to frequently asked questions.
  
[常见问题](/docs/resources/faq)<br>
常见问题解答。

### Videos

### 视频

We also have some helpful videos on our [Flutter Youtube
channel]({{site.social.youtube}})!  In particular, check
out the Flutter in Focus series, and learn about other
series on our [videos](/docs/resources/videos) page.

我们在 YouTube 上有一个 [视频频道]({{site.social.youtube}})，欢迎订阅！
更多视频和播放列表介绍，以及社区制作的视频教程，
可以查看我们的 [Flutter 技术视频资源](/docs/resources/videos) 页面。

<iframe style="max-width: 100%" width="560" height="315" src="//player.bilibili.com/player.html?aid=55794948&cid=97538589&page=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Flutter in Focus: Learn Flutter features in 10 minutes or less.<br>
[Flutter in Focus playlist](https://www.youtube.com/playlist?list=PLjxrf2q8roU2HdJQDjJzOeO6J3FoFLWr2)

In Flutter, "everything is a widget"! If you want to better understand the
two kinds of widgets, Stateless and Stateful, see the following videos,
part of the [Flutter in
Focus](https://www.youtube.com/playlist?list=PLjxrf2q8roU2HdJQDjJzOeO6J3FoFLWr2) series.

Flutter 里 “所有的事物都是 widget”，
如果你想更好了解有状态和无状态的 widget，请关注
[Flutter in Focus 系列视频](https://www.youtube.com/playlist?list=PLjxrf2q8roU2HdJQDjJzOeO6J3FoFLWr2)。

<iframe style="max-width: 100%" width="560" height="315" src="//player.bilibili.com/player.html?aid=55794591&cid=97538062&page=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="560" height="315" src="//player.bilibili.com/player.html?aid=55832147&cid=97601562&page=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Want to skill up?

## 提升内容

If you learn best by watching engineers write code, make mistakes, and fix them,
check out the [Boring Flutter
Show](https://www.youtube.com/watch?v=vqPG1tU6-c0&list=PLjxrf2q8roU28W3pXbISJbVA5REsA41Sx&index=3&t=9s)
video series:

如果你想看工程师们在线写代码、写 bug、修 bug，请关注
[Boring Flutter Show 系列视频](https://www.youtube.com/watch?v=vqPG1tU6-c0&list=PLjxrf2q8roU28W3pXbISJbVA5REsA41Sx&index=3&t=9s)

<iframe style="max-width: 100%" width="560" height="315" src="//player.bilibili.com/player.html?aid=55815727&cid=97573460&page=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[Boring Flutter Show playlist](https://www.youtube.com/watch?v=vqPG1tU6-c0&list=PLjxrf2q8roU28W3pXbISJbVA5REsA41Sx&index=3&t=9s)

You might also find these docs useful:

这些文档也会非常有用：

* [Using packages](/docs/development/packages-and-plugins/using-packages)
  
  [在 Flutter 里使用 Packages](/docs/development/packages-and-plugins/using-packages)
  
* [Adding assets and images](/docs/development/ui/assets-and-images)
  
  [添加资源和图片](/docs/development/ui/assets-and-images)
  
* [Navigation and routing](/docs/development/ui/navigation)
  
  [路由和导航](/docs/development/ui/navigation)
  
* [State management](/docs/development/data-and-backend/state-mgmt/intro)
  
  [状态 (State) 管理介绍](/docs/development/data-and-backend/state-mgmt/intro)
  
* [Animations](/docs/development/ui/animations)
  
  [动画效果介绍](/docs/development/ui/animations)
  
