# Luogu Motaki

Luogu Motaki 是一个采用服务端-客户端结构的 [洛谷冬日绘板](https://www.luogu.com.cn/paintboard) 助手。

其中，服务端负责分配任务，客户端负责绘制。可以使用专门的工具将图片转为数据，调整图片的大小、绘制的位置，并进行预览。

-   方案制作: [luogu-motaki-plan-editor](https://github.com/ouuan/luogu-motaki-plan-editor)
-   方案预览: [luogu-motaki-plan-preview](https://github.com/ouuan/luogu-motaki-plan-preview) ([网页](https://ouuan.github.io/luogu-motaki-plan-preview))
-   服务端: [luogu-motaki-server](https://github.com/ouuan/luogu-motaki-server) 
-   客户端: [luogu-motaki-client](https://github.com/ouuan/luogu-motaki-client)

## 为什么使用 Luogu Motaki

### 将 token 掌握在自己手中

参与者不再需要将 token 交给领导者，可以保证 token 不被滥用，只用来画自己想画的东西。

当然，集中管理 token 也有很多优势，Luogu Motaki 在允许分布式绘制的同时，完全支持集中管理 token：客户端可以添加多个 token，并且异步进行处理。

### 让参与多个计划更加简单

如果要将 token 交予他人，就必然只能参加一个领导者的绘制计划。如果要同时参与多个计划，就需要这些计划的领导者之间进行合作。

使用 Luogu Motaki，你不仅可以同时参与多个计划，还能只参加一个计划的一部分（例如，一张图片）。

并且，Plan Preview 可以直接在 URL 的参数中加入服务端地址，点击即可预览，选择图片即可复制到客户端的配置文件并参与绘制。

### 让合作更加简单

两个计划合作时，一方面，参与者可以简单地在配置中加入一个新的服务端地址；另一方面，两个计划可以轻松地使用 Plan Editor 进行合并。

### 轻松地将图片转为数据

Luogu Motaki Plan Editor 内置了图片缩放、颜色转换、多种抖动色方式（包括不进行抖动色处理），并且可以使用 Plan Preview 快速预览。

## 我想发起绘制计划

如果只需要本地的客户端（例如，还是集中收集 token 进行绘制），直接在自己的电脑上运行服务端即可。

如果只需要内网的客户端（例如，机房一起画，或者手机热点），在一个连着内网的电脑上运行服务端即可。

如果需要其他网友一起参与，你需要一台服务器。如果没有的话，可以在 [Discussions 的 Server 板块](https://github.com/ouuan/luogu-motaki/discussions/categories/server) 发帖来让别人（例如 ouuan）帮你搭建服务端 / 在服务端中加入你要画的图。

## 我想参与他人的绘制计划

拿到别人的服务器地址后，加到客户端的配置里，运行客户端，就可以了！

## 关于封禁

为了防止领取绘制任务而不真的绘制等滥用/攻击行为，服务端有一些封禁规则，根据行为的严重程度进行一定时长的封禁。如果正常使用官方客户端，没有出现大量 token 失效/被占用等情况，一般是不会被封禁的。封禁会在封禁时长结束或重启服务端后解除。
