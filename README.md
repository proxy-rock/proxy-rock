# Proxy Rock
https://chromewebstore.google.com/detail/proxy-rock/dkeknkogllphlkmcfdjllhpbpnmkmgea

## 为什么做这个项目

大家对 Switchy Omega 应该都不陌生，在上古时代代理生态还比较匮乏的时候此插件是为数不多用起来还不错的项目。此外，特别是做前端开发的小伙伴，在开发过程经常会用到其提供的转发功能来保可以用域名进行请求。即使是现在仍有大批的用户在使用该插件。

但该插件又不能说毫无槽点，GitHub issue 中也有不少用户进行反馈，如在浏览器扩展栏中点击小图标会出现弹出页面加载失败的情况，配置失败导致插件崩溃继而引发浏览器崩溃，加载资源失败等等，以及 10 年前的界面风格，上次更新距今也过去 4 年了。

所以，想着能不能对插件重构一下，其实正式的重构在今年春节的时候就开始了（比较巧的是 2 月份 Google 宣布 6 月份开始不支持 manifest v2 版本的插件），由于 Switchy Omega 是用 coffeescript 构建，加之项目本身的复杂度看起来还是有点难度的，所以基本上是从头进行开发了，以至于拖拖拉拉到了现在，但核心功能已经基本可用了。

## 目前支持的功能

核心功能其实均已经支持，具体如下。

#### 模式配置

* Proxy 模式，即 so（Switchy Omega） 中的 Proxy Profile，此模式下配置好本地的代理服务，根据请求 schema 选择对应的协议。
  
<img src="https://i.imgur.com/gFqdpOF.png" width="400"></img>


* Auto 模式，即 so 中 Switch Profile，此模式下可以根据设置的 Host 规则路由到不同的 Proxy 中，也可以下载在线的 PAC 格式资源进行匹配后再转发。
  
<img src="https://i.imgur.com/Hz5xj97.png" width="400"></img>


* Pac 模式，即 so 中 Pac Profile，此模式下直接使用在线或者手动录入的 PAC 内容作为配置规则。建议熟悉 PAC 文件的同学使用。
  
<img src="https://i.imgur.com/3TdiJBp.png" width="400"></img>

#### 规则切换

* 插件栏中点击小图标，可将配置好的规则展现出来，点击即可进行切换，同样在配置页面可以选择是否在切换时进行刷新。


<img src="https://i.imgur.com/g82JG6U.png" width="150"></img>


* 另外，配置的规则会根据名字生成唯一的颜色标识，选中的配置所对应的颜色同样会在状态栏插件中体现出来

<img src="https://i.imgur.com/chWyWut.png" width="150"></img>
<img src="https://i.imgur.com/hk6aIv6.png" width="150"></img>


## 计划支持的功能

还有很多功能计划未来逐步添加，暂定每半个月一个版本的节奏。
- [ ] 导入导出
- [ ] 规则颜色可配
- [ ] 深色模式，跟随系统
- [ ] 点击小图标规则跳转配置页
- [ ] 异常配置检测
- [ ] firefox 支持
- [ ] 一键配置网站规则
- [ ] http 协议支持账号密码
- [ ] 数据同步

## 最后
由于目前还在密集开发中，使用中有什么问题的话可随时到 https://github.com/proxy-rock/proxy-rock/issues 进行反馈。

感谢 Switch Omega 的作者给我们带来如此优秀的项目 :+1: 。
