> SDK Version

```
flutter --version

Flutter 2.10.5 • channel stable • https://github.com/flutter/flutter.git
Framework • revision 5464c5bac7 (1 year, 11 months ago) • 2022-04-18 09:55:37 -0700
Engine • revision 57d3bac3dd
Tools • Dart 2.16.2 • DevTools 2.9.2
```

# 使用 Flutter 开发一个豆瓣 APP

* 此项目，90%还原某瓣 APP，所有 UI 均按照某瓣来实现。
* 项目中的数据均来自豆瓣 api 真实有效数据
* 项目中用到了几乎所有的 Flutter widget
* 还有两个比较大的自定义魔改源码实现特效

> APP 中所有数据均为真实数据。但是默认，对于"书影音单个电影 tab"的数据，使用模拟数据。因为，频繁的打开关闭 APP，会频繁调用
> 这个接口。接口是有调用限制的，次数过于频繁，会被锁 IP。如果想看真实数据，则可以进入
"我的"，然后打开"书影音数据来自网络"开关后，重启 APP 即可。

#### Demo(刷不出 gif 图的，耐心等待一会，或者多刷几次。)

![](https://github.com/kaina404/FlutterDouBan/blob/master-release/0E95A04AE84EFE31104AC8E0A5808CB9.png)
![](https://github.com/kaina404/FlutterDouBan/blob/master-release/041919372752_04CCDD7BC1BDB6015935EE50DDF75C29F.png)
![](https://github.com/kaina404/FlutterDouBan/blob/master-release/041919374444_0B3C7C7E29941F75D0A7C944D4E352CB7.png)
![](https://github.com/kaina404/FlutterDouBan/blob/master-release/041919375761_05292CAB58428C7C77C544027FC899CC0.png)
![](https://github.com/kaina404/FlutterDouBan/blob/master-release/041919380838_07B17727ACF231C6D91914D71114A96CF.png)
![](https://github.com/kaina404/FlutterDouBan/blob/master-release/041919381924_01CE541B98F565C72B75567A319271CA1.png)

![demo1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/demogif/Mar-10-2019%2014-12-55.gif)

![demo1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/demogif/Mar-10-2019%2014-13-11.gif)

![demo1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/demogif/Mar-10-2019%2014-17-38.gif)

![demo1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/demogif/Mar-10-2019%2014-17-48.gif)

![demo1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/demogif/Mar-10-2019%2014-18-03.gif)

![demo1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/demogif/Mar-10-2019%2014-18-12.gif)

![demo1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/demogif/Mar-10-2019%2014-18-23.gif)

![demo1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/demogif/Mar-10-2019%2014-30-58.gif)

![demo1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/demogif/Mar-10-2019%2014-31-13.gif)

![demo1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/demogif/Mar-10-2019%2014-32-29.gif)

![demo1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/demogif/Mar-10-2019%2014-32-41.gif)

![demo1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/demogif/Mar-10-2019%2014-33-02.gif)

# dev-open

### 大家可以向这个分支根据豆瓣 UI 做设计稿，提交代码

* 这个分支供广大 Flutter 开发者来学习 Flutter
* **此分支囊括了 Flutter 90%的组件的基本与组合使用**，是初学者真正实践的不错选择
* 在此豆芽 APP 的首页实现与影片详情的 UI 特效，基于魔改 Flutter 源码。有兴趣可以看看
* 大家想实战自己的 Flutter 能力，可以将某瓣 APP 作为设计稿，完成需求，并提交
* 每位开发者提交的代码，我都会在文档中进行备注

#### 注意！！！建议使用模拟数据(mock_request.dart)

* 每个接口均有一定的调用限制
* *大家 pull 下的代码，进行测试调试时，对于特定接口，返回的特定数据。尽量不要每次求请求一次。可以请求到一次真实数据后，转成 json 保存
  到本地。然后，自己调试开发的时候，使用这个模拟数据即可。* [可参考 mock_request.dart]

# 未来版本计划(欢迎 Flutter 爱好者前来认领)

**欢迎 Flutter 爱好者共同完成**

> 涉及到 UI，可参考豆瓣。

### 萌新 TASK

* 完成任意一个未实现的按钮
* 完成任意一个未实现的页面
* 优化原有 Widget
* 爱好者想实现但是未能实现的需求
* More ...

### 进阶 TASK

* 优化代码
* 适当缓存数据
* 解决卡顿(可参考：https://flutter-io.cn/docs/testing/ui-performance)
* 优化路由（可参考咸鱼方案：https://www.yuque.com/xytech/flutter/vf1dpf）

### 老手 TASK

* [接入 rxdart](https://github.com/ReactiveX/rxdart)
* [使用 Fish Redux 重构](https://www.yuque.com/xytech/flutter/ycc9ni)

# 对魔改源码或者喜欢翻源码的童鞋可以看看下面两个

* 魔改 Flutter AppBar 源码实现豆瓣头部特效

  ![魔改 Flutter AppBar 源码实现豆瓣头部特效](https://github.com/kaina404/DouBanProject/blob/dev-0.1/%E4%BB%BF%E8%B1%86%E7%93%A3%E5%A4%B4%E9%83%A8.gif)

* 魔改源码实现电影详情抽屉特效(GIF 图如果加载不出来，多刷几次)

  ![抽屉特效1](https://github.com/kaina404/DouBanProject/blob/dev-0.1/part1.gif)

  ![抽屉特效2](https://github.com/kaina404/DouBanProject/blob/dev-0.1/part2.gif)

  ![抽屉特效3](https://github.com/kaina404/DouBanProject/blob/dev-0.1/part3.gif)

# 页面介绍

* 首页 pages/home

  * homo_app_bar.dart 首页导航头
  * home_page.dart 首页
  * my_home_tab_bar.dart 首页 tab

* 书影音 pages/movie

  * book_audio_video_page.dart 书影音页面
  * detail_page.dart 影片、电视详情页面
  * person_detail_page.dart 演员页面介绍
  * ... 页面都有注释

* 小组 pages/group

* 市集 shop_page.dart
  * 市集的数据使用两个 webview

* 我的 page/person

# 默认条约

此项目仅供大家交流沟通使用，不得用于任何商业以及利益活动。由此引起的责任，跟我无关。谢谢！