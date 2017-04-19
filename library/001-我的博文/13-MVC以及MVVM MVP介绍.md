## 前端框架MVC、MVVM、MVP介绍
`by winter`

### 1. MVC
Model-View-Controller(模型-视图-控制器)是最常见的软件架构之一，业界有着广泛应用。

- 视图（View）：用户界面
- 控制器（Controller）：业务逻辑
- 模型（Model）：数据保存

各部分之间的通信如下：

![](assets/001/13-c871edca.png)

1. View传送指令到Controller
2. Controller完成业务之后要求Model改变状态
3. Model将新的数据发送到View，用户得到反馈

#### 接受用户指令时，MVC的两种方式：（互动模式）
![](assets/001/13-807024f4.png)

*另一种是直接通过Controller接受指令*

![](assets/001/13-f18acc87.png)

### 2. MVP
**MVP模式将Controller改名为Presenter，同时改变了通信方向**

![](assets/001/13-355c3d4d.png)

1. 各部分之间的通信，都是双向的
2. View与Model不发生联系，都是通过Presenter传递
3. View非常薄，不部署任何业务逻辑，称为“被动视图”（Passive View）,即没有任何主动性，而Presenter非常厚，所有逻辑都部署在那里

### 3. MVVM
**MVVM模式将Presenter改名为ViewModel，基本上与MVP模式完全一致**

![](assets/001/13-64e9b98a.png)

唯一的区别是，它采用**双向数据绑定**（data-binding）:View的变动自动反映在ViewModel，反之亦然。Angular和Ember都采用这种模式
