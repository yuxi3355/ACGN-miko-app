# mikomiko 一款动漫、音乐、美图、galgame于一体的二次元app。

## 介绍
mikomiko是一款二次元手机app，里面集成了网易云api可以在线听歌。使用scrapy增量式爬虫并整合SpringBoot的完成了的动漫区、美图区、galgame区的api，并应用在app中。
实现了在线看番，壁纸欣赏、galgame分享的功能。ps：点击美图区的浮动按钮会触发隐藏美图，"绅士"们不要错过哦。

## 软件架构
1、app模块定义各种Activity和Fragment以及相应布局文件, 使用了ButterKnife进行控件绑定。<br/>
2、com模块定义项目中公用的部分，例如网络请求API、常量，自定义封装RecyclerView, Adapter, 定义实现图片圆角控件RoundImageView, 
    自定义数据回调接口DataSource.Callback<T> 以及MVP模式基本契约接口。基本Presenter抽象类等。<br/>
3、fac模块定义数据Model，封装网络请求工具类，定义Retrofit2代理接口RemoteService,以及各种Presenter的实现类。<br/>
4、res模块定义各种item布局文件，各种drawable、string、color、dimen资源。是项目主要的资源模块。<br/>
5、vitamio模块是第三方在线视频播放模块。里面封装了m3u8索引文件的解析器，可以直接播放m3u8包含的流媒体。<br/>

## 功能截图
### 主页
![avatar](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/index/5a6520b5937ee8542b1bded6bdea8754529c692d.jpg)
![avatar](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/index/Screenshot_2021-04-18-21-22-43-745_com.xana.acg.m.jpg)
![avatar](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/index/Screenshot_2021-04-18-21-23-20-921_com.xana.acg.m.jpg)
![avatar](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/index/Screenshot_2021-04-18-21-24-21-925_com.xana.acg.m.jpg)

### 搜索
![avatar](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/search/Screenshot_2021-04-18-21-25-06-562_com.xana.acg.m.jpg)
![avatar](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/search/Screenshot_2021-04-18-21-26-02-025_com.xana.acg.m.jpg)
![avatar](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/search/Screenshot_2021-04-18-21-28-05-182_com.xana.acg.m.jpg)
![avatar](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/search/Screenshot_2021-04-18-22-00-41-430_com.xana.acg.m.jpg)
![avatar](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/search/Screenshot_2021-04-18-22-00-55-530_com.xana.acg.m.jpg)
![avatar](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/search/Screenshot_2021-04-18-22-02-34-673_com.xana.acg.m.jpg)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/search/Screenshot_2021-04-18-22-02-51-161_com.xana.acg.m.jpg)

### 动漫播放 (darling in the franxx）

「比翼の鳥」というらしい<br/>
その鳥は片方の翼しかも立つ、雄と雌、つわいで寄り添わらければ、空を飛べない。不完全の生き物。<br/>
でも、なぜだろう、わたしはその命のやり方を美しいと思ってしまったのだ。<br/>
美しいと感じてしまったのだ。<br/>
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-21-59-21-999_com.xana.acg.m.jpg)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-09-51-068_com.xana.acg.m.jpg)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-09-55-744_com.xana.acg.m.jpg)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-10-04-303_com.xana.acg.m.jpg)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-12-38-239_com.xana.acg.m.jpg)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-12-40-659_com.xana.acg.m.jpg)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-13-20-535_com.xana.acg.m.jpg)

やっぱりボクと同じようだ、キミとボクを似ていてね。<br/>
人間の涙を久しぶり見た、その目を気に入ったよ、ドキドキする。<br/>
さぁおいで、キミを味あわせて、今からキミがボクのダーリンだ。<br/>
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-14-02-249_com.xana.acg.m.jpg)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-14-36-861_com.xana.acg.m.jpg)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-14-43-738_com.xana.acg.m.jpg)

なぜだが、涙が出た。傷の痛みのせいじゃない。<br/>
そうだ、わたしはたぶん嬉しかったのだ、絵本の中の世界みたいな、綺麗なものに<br/>
きっとこの人とならなれるんだと。<br/>
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-16-49-016_com.xana.acg.m.jpg)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-18-40-904_com.xana.acg.m.jpg)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-17-34-810_com.xana.acg.m.jpg)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-22-17-57-463_com.xana.acg.m.jpg)

### 音乐播放 (Re:ゼロから始める異世界生活　Memento)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-21-25-26-833_com.xana.acg.m.jpg)

### 游戏分享 (美少女万華鏡　理と迷宮の少女)
![avater](https://mikochat.oss-ap-northeast-1.aliyuncs.com/Screenshoots/mikomiko/play/Screenshot_2021-04-18-21-23-47-468_com.xana.acg.m.jpg)

## 参与贡献
1.  Fork 本仓库
2.  新建 master 分支
3.  提交代码
4.  新建 Pull Request

## 致谢


