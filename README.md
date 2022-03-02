---
description: 为英雄小屋客户端和APP创建WEB小程序吧！
---

# 英雄小屋DVA SDK

## DVA SDK

DVA SDK为开发者提供了一系列方法的调用。这些方法不仅包含了英雄小屋WEB小程序（以下简称小程序，注意区分WEB小程序和Node小程序的区别。DVA SDK仅为WEB小程序提供支持。）的设计规范，也使得小程序可以调用PC客户端或APP的底层方法。因此小程序不仅可以通过DVA SDK和应用底层交换信息，也可以和其他小程序交换信息。

> DVA SDK作者：千岛秋（[![千岛秋的微博](https://app.heroxw.com/assets/weibo.png)](https://weibo.com/u/6902161510)[![千岛秋的github](https://app.heroxw.com/assets/github.png)](https://github.com/xkevas24/)）、sz（）
>
> Sombra协议作者：黄融（[![黄融的github](https://app.heroxw.com/assets/github.png)](https://github.com/hr567/)）、王云飞、千岛秋（[![千岛秋的github](https://app.heroxw.com/assets/github.png)](https://github.com/xkevas24/)）



## 官方支持的开发框架

DVA SDK 仅对 Quasar Framework（[https://quasar.dev/](https://quasar.dev)）和 uni-app（[https://uniapp.dcloud.io/](https://uniapp.dcloud.io)）提供官方适配和Demo代码。

### Quasar Framework

官方文档：[https://quasar.dev/](https://quasar.dev) ，热心网友翻译的中文文档：[http://www.quasarchs.com/](http://www.quasarchs.com)

Quasar（发音为/kweɪ.zɑɹ/)是MIT许可的基于Vue.js的开源框架，允许作为Web开发人员的您快速创建多种类型的responsive++网站/应用：

* SPAs (单页应用)
* SSR (服务器端渲染的应用) (+可选的PWA客户端接管)
* PWA（渐进式网页应用）
* BEX (浏览器扩展)
* 通过Cordova或Capacitor构建移动APP（Android、iOS…）
* 多平台桌面应用（使用Electron）

Quasar的座右铭是：**编写代码一次并同时将其部署**为网站、移动应用和/或Electron应用。 是的，所有这些应用都用一个代码库，通过使用最先进的CLI并辅以精心编写的、性能导向的Quasar Web组件，帮助您以最短时间开发应用。

当使用Quasar时，你不需要像Hammer.js，Moment.js或Bootstrap这样的额外重型库。它内部覆盖了这些需求，而且占用空间小！

### uni-app

官方文档：[https://uniapp.dcloud.io/](https://uniapp.dcloud.io)

`uni-app` 是一个使用 [Vue.js](https://vuejs.org) 开发所有前端应用的框架，开发者编写一套代码，可发布到iOS、Android、Web（响应式）、以及各种小程序（微信/支付宝/百度/头条/飞书/QQ/快手/钉钉/淘宝）、快应用等多个平台。

## Sombra通信协议

Sombra 协议用于英雄小屋平台中小程序与底层内核、小程序与小程序之间进行通信。该协议在小程序与内核之间建立双向通信，支持内核对小程序进行身份验证。该协议设计符合 [WebSocket协议](https://datatracker.ietf.org/doc/html/rfc6455) 规范与 [JSON-RPC规范](https://www.jsonrpc.org/specification) 。Sombra 协议使用 WebSocket 建立小程序和底层内核之间的连接，将小程序身份验证过程集成在 WebsSocket 握手过程中。WebSocket 连接建立后，Sombra 协议通过 JSON-RPC 协议所定义的方式传递指令。

Sombra通信协议的开发者文档可以参见：[https://sombra.docs.heroxw.com/](https://sombra.docs.heroxw.com)

