## ionic安装和项目的创建

说来惭愧，都说隔行如隔山，没想到自己对同行的了解都微乎其微，还成天称是程序猿，直到前几天自己才听到Ionic,上度娘一问，瞬间就泪崩了，竟然在我身边有PhoneGap、cordova、AngularJS、nodejs、npm等等这么多“赫赫有名”的专有名词我以前竟然听都没听到过，可想自己是有多无知，以下是我这几天科普来的，错误之处还望指出，谢谢！

### What is the Ionic？
Ionic 是一个强大的 HTML5 应用程序开发框架，号称Advanced Html5 Hybrid Mobile AppFramework 是 AngularJS 移动端解决方案 可以帮助您使用 Web 技术，比如 HTML、 CSS 和JavaScript 构建接近原生体验的移动应用程序。 Ionic 主要关注外观和体验，以及和你的应用程序的 UI 交互，特别适合用于基于 Hybird 模式的 HTML5 移动应用程序开发..….

### What is the PhoneGap ?
PhoneGap是一个用基于HTML，CSS和JavaScript的，创建移动跨平台移动应用程序的快速开发平台。
PhoneGap是一个跨平台的移动app开发框架，可以把html css js写的页面打包成跨平台的可以安装的移动app，并且可以调用原生的几乎所有的功能，比如摄像头，联系人，加速度等。

### What is the Cordova ?
Cordova提供了一组设备相关的API，通过这组API，移动应用能够以JavaScript访问原生的设备功能，如摄像头、麦克风等。

Cordova是PhoneGap贡献给Apache后的开源项目，是从PhoneGap中抽离出的核心代码，是驱动PhoneGap的核心引擎。有点类似Webkit和Google Chrome的关系。渊源就是：早在2011年10月，Adobe收购了Nitobi Software和它的PhoneGap产品，然后宣布这个移动Web开发框架将会继续开源，并把它提交到Apache Incubator，以便完全接受ASF的管治。当然，由于Adobe拥有了PhoneGap商标，所以开源组织的这个PhoneGap v2.0版产品就更名为Apache Cordova。

### What is the AngularJS ?
AngularJS 是一个JavaScript 框架。它是一个以JavaScript 编写的库。
AngularJS 使得开发现代的单一页面应用程序（SPAs：Single Page Applications）变得更加容易。
- AngularJS 把应用程序数据绑定到 HTML 元素。
- AngularJS 可以克隆和重复 HTML 元素。
- AngularJS 可以隐藏和显示 HTML 元素。
- AngularJS 可以在 HTML 元素"背后"添加代码。
AngularJS 支持输入验证。

### What is the NodeJs?
Node.js 是一个基于Chrome JavaScript 运行时建立的一个平台。

Node.js是一个事件驱动I/O服务端JavaScript环境，基于Google的V8引擎，V8引擎执行Javascript的速度非常快，性能非常好。

其实吧，可以认为 Node.js 就是运行在服务端的 JavaScript。
### What is the NPM ?
NPM是随同NodeJS一起安装的包管理工具，能解决NodeJS代码部署上的很多问题，常见的使用场景有以下几种：
- 允许用户从NPM服务器下载别人编写的第三方包到本地使用。
- 允许用户从NPM服务器下载并安装别人编写的命令行程序到本地使用。
- 允许用户将自己编写的包或命令行程序上传到NPM服务器供别人使用。

  新版的nodejs已经集成了npm，所以装了nodejs的话npm也一并安装好了。可以通过输入"npm -v"来测试是否成功安装。

### How to make 移动应用(App)
有三种方式可以为手机制作移动应用：

- 原生应用（Native app）

- 手机网站（Mobile website）

- 混合应用（Hybrid app）

#### 原生应用（Native app）
如上述，你可以根据不同系统平台指定SDK制作对应系统平台下的移动应用，如果你想要为iOS系统创建一款应用，你需要：

拥有一台苹果Mac电脑，当然其他方法也可以，但是我不推荐。作为初学者，一台廉价的Mac Mimi就可以了。

从App store下载Xcode

购买苹果开发者许可证（Apple Developer license）99刀￥一年（如果你想要在App store上发布应用）

你可以利用Swift语言或者它的前辈ObjectiveC语言创建App，Swift 语言在沉重的ObjectiveC语言上做出了巨大改进，如果你决定开发原生app，相比利用ObjectiveC开发原生app，Swift更容易上手，特别是当你有Web开发的背景时。    

如果你想要为Android系统创建一款原生应用，你需要：

拥有一台电脑

下载合适的SDKs（后面将会讲到）

购买谷歌开发者许可证（Google Developer license）25刀￥（如果你想要在Google Play Store上发布应用）

`利用原生开发技术开发的应用具有速度快和直接利用原生API的优势（你不需要像开发混合应用一样【Hybrid App】作任何中间封装），缺点是，你需要为不同手机系统平台开发不同版本的移动应用。（撰写多套代码）`

#### 手机网站（Mobile website）
通过手机浏览器可以访问手机网站，手机网站可以根据手机屏幕大小自适应。由于手机网站比较难以维护，一种叫做响应式网站设计（responsive website design）的方法被使用，通过这种方法你拥有一套HTML代码库，你可以通过使用媒体查询（Media queries）根据不同设备不同分辨率（resolutions）改变他们的网站外观。jQuery mobile 是一种出色的移动框架。使用它你可以制作一款移动版本的Web应用程序。移动网站一个显著的优势就是你可以根据需要实时更新他们的内容，而不用去等待苹果Apple或者谷歌Google的审核，劣势则包括低耦合，更少的特征。

#### 混合app（Hybrid app）
混合应用基本上是一款手机应用，它和撰写网站的程序语言基本相同，唯一不同的就是他们包含在一个孤立的浏览器中（WebView）， 原生应用通过WebView运行Web应用，混合应用可以调用手机摄像头、GPS等，通过利用插件，混合应用可以调用手机其它的硬件功能，你可以利用开发Web应用的技术开发混合应用。然而，WebView有速度的限制， 制作成熟的3D图像游戏可能不是最好的选择。

### 安装Ionic
1. 需要有JDK和SDK环境，这是Android开发必有的平台（JDK在技术文章003中已经详细阐述了）

  安卓SDK下载以及环境的配置：
  下载地址：（可以使用包含的 sdkmanager 下载其他 SDK 软件包 需要翻墙） [立即下载](https://dl.google.com/android/repository/tools_r25.2.3-windows.zip)

  ![](assets/002/005-ebfa888c.png)

  [安卓开发相关资源链接 包含Android Studio](https://developer.android.com/studio/index.html)

  下载后双击安装，指定Android SDK的安装目录，为了方便使用Android SDK包含的开发工具，我们在系统环境变量中的Path设置Android SDK的安装目录下的tools目录。

  
