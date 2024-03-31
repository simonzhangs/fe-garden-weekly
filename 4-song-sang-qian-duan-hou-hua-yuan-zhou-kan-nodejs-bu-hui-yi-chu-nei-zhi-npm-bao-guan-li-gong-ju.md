---
description: 松桑前端后花园周刊第四期
---

# 4️⃣ #4松桑前端后花园周刊-Nodejs不会移除内置npm包管理工具

## 行业动态

1、[Nodejs 技术指导委员会证实不会移除内置的npm包管理工具](https://socket.dev/blog/node-js-tsc-confirms-no-intention-to-remove-npm-from-distribution)（英文）

npm (Node Package Manager) 是 Node.js 的官方内置的包管理器。除了 npm 外，还有 yarn、pnpm 为了解决 npm 包管理过程问题提出的。但是目前存在包管理混用的情况，不同项目代码用的包管理器不同，每次切换项目更新依赖时有可能使用错其他包管理工具，还得删除多出来的lock文件。除了上述问题，社区也在讨论 Node 内置npm，对其他包管理工具不公平，不利于社区的良性发展。

Node.js 16.9.0 提出了 Corepack 实验功能，简单来说，是包管理工具的管理器，用来管理 npm、yarn、pnpm，并计划将 Corepack 内置在 Node 发行版中，也就是说下载 Node 时，会默认下载 yarn、pnpm，但是对于是否内置 npm 有不同的意见。

目前 Node 技术指导委员会(TSC)本周召开了会议，作为关于默认启用 Corepack 的更广泛讨论的一部分。出席会议的成员证实，他们已经达成共识，没有打算删除 npm。

![Nodejs 技术指导委员会证实不会移除内置的npm包管理工具](https://s2.loli.net/2024/03/31/EeXdBoDwAx9Hnz4.png)

2、[Arc 浏览器的制造商 Browser ](https://techcrunch.com/2024/03/21/the-browser-company-raises-50-million-at-550-million-valuation/)[融资](https://techcrunch.com/2024/03/21/the-browser-company-raises-50-million-at-550-million-valuation/)[5000万美元，估值为5.5亿美元](https://techcrunch.com/2024/03/21/the-browser-company-raises-50-million-at-550-million-valuation/)

Arc 浏览器的制造商 Browser 公司在由 Pace Capital 牵头的一轮融资中筹集了5000万美元，估值为5.5亿美元。

Arc 是一款基于 Chromium 内核开发的浏览器，凭借针对日常浏览器使用痛点问题，设计了命令栏导航、临时网页概念（页面默认12h自动关闭）、工作生活分区，以及设计和交互感十足的特点，吸引了人们的注意力。Arc 浏览器在去年7月在 Mac 上开发下载服务，目前 Window 版本还在测试中，需要加入 waitlist 才能参与测试。

![Arc 浏览器](https://s2.loli.net/2024/03/31/e1xpqOiMRNkQm5v.png)

## 发布

1、[VitePress 1.0](https://vitepress.dev/) – Powerful static site generator.

VitePress 是在 Vite 和 Vue 之上构建的，是 VuePress 的“续作”和“替代”。

VitePress 是一个静态站点生成器(SSG) ，用于构建快速、以内容为中心的网站。VitePress 采用 Markdown 编写的源内容，对其应用主题，通过将 Markdown 构建为静态 HTML 页面，可轻松部署到任何地方。

![VitePress 1.0](https://s2.loli.net/2024/03/31/BGAx7MfHRm2yn9a.png)

2、[Node.js v20.12.0 (LTS)](https://javascriptweekly.com/link/153170/web)

Node 20.12.0 稳定版本引入了一个 helper `crypt.hash ()`，它一次性从输入中计算摘要。这可以比基于对象的`createHash ()`快1.2到2倍，因为对于容易获得的较小输入，并且由于不创建中间对象，所以产生的内存开销较少。

3、[Deno 1.42.0](https://javascriptweekly.com/link/153173/web)

次版本变更包括添加了多行配置文件、支持加载以CommonJS形式定义的ES模块、对TypeScript 5.4进行了更新，并修复了一些CLI、覆盖率和性能方面的问题。

Deno是一个由 Rust 语言编写的现代的 JavaScript 和 TypeScript 运行时环境，由Node.js的创建者Ryan Dahl开发。与 Nodejs 相比，Deno 设计更考虑安全性问题，通过使用沙箱机制来限制代码的访问权限，并默认禁用文件、网络和环境访问；此外 Deno 没有包管理工具，更推荐直接从远程UR导入模块；而且 Deno 使用基于Rust编写的单线程事件循环，与Node.js的事件循环机制有所不同，可以提供更好的性能和更高的并发能力。

![Deno 1.42.0](https://s2.loli.net/2024/03/31/RKQTAjEzyX8bYud.png)

## 文章

[React 中 Form 的最佳实践](https://mp.weixin.qq.com/s/JikF87PYtxnb9uxEtTtGNA)（译文）

作者在开发一个 `AI` 项目，里面有许多复杂的动态表单。在研究了许多优秀的 `React` 表单指南之后，作者意识到，大多数构建表单的资源都已经过时了，作者阐述了 `React` 中构建表单的受控和非受控概念，以及表单的现代最佳实践、如何去构建动态表单、 `RSC（React Server Components）`的表单等等。

## 开源项目

[Nodeclub](https://github.com/cnodejs/nodeclub)

Nodeclub 是使用 **Node.js** 和 **MongoDB** 开发的社区系统，已在Node.js 中文技术社区(CNode)得到应用，但你完全可以用它搭建自己的社区，可以作为学习Node的实践项目。

## 网站

1、[网易云段子](https://www.yduanzi.com/)

这个网站收集了很多网易云段子、笑话。

2、[自我销毁网站](https://www.thiswebsitewillselfdestruct.com/)

一个匿名网站，如果 24 小时内没有收到访问者的留言，将会自我销毁。在口罩时期有很多网友在这里相互留言鼓励。虽然目前这个网站已经销毁了，但是松桑还是贴在这儿了，纪念以下这个网站。

3、[项目README徽章](https://shields.io/)

生成动态或者自定义的徽章，用于开源项目的 README 页面

## CSS WEEKLY

1、[你可能不知道的 CSS 按钮样式](https://dbushell.com/2024/03/10/css-button-styles-you-might-not-know)（英文）

作者阐述了不常见但十分有用处的按钮CSS样式，包括使用`touch-action：manipulation`来禁用按钮上不小心“双击缩放”收拾，这样还有一个额外的好处，浏览器不再需要延迟点击事件等待第二次点击；`user-select:none`可以禁用按钮的复制功能，避免用户点击按钮的开启的默认复制功能；`:file-selector-button`是`type="file"`的`input`按钮组件的伪元素，`:focus-visible`是当元素匹配`:focus`伪类并且客户端 (UA) 的启发式引擎决定焦点应当可见 (指键盘tab操作时，在这种情况下很多浏览器默认显示“焦点框”) 时将生效。

![你可能不知道的 CSS 按钮样式](https://s2.loli.net/2024/03/31/wX5nDyVmlYIkG7F.png)

2、[如何使用现代 CSS 技术实现高度可配置的开关组件](https://piccalil.li/blog/a-highly-configurable-switch-component-using-modern-css)（英文）

Safari 预览版最近添加了一个版本185和186的开关组件，作者另辟蹊径，通过使用: `has ()`、容器查询、逻辑属性和自定义属性来构建一个高度可配置的开关组件，展示如何构建一个真正灵活的开关组件。

## 资源

1、[七天学会NodeJS](http://nqdeng.github.io/7-days-nodejs/#1.1)

Node 作为老牌的 JavaScript 运行时环境，正受着 Deno、Bun 新运行时环境挑战，Deno 旨在提供更安全的运行环境，Bun 在速度和性能上更优。那么现在学习 Node 还来得及吗，或者说还需要学习吗？Node 具有丰富的生态，更加成熟，仍属于必学的语言，松桑为大家搜集了阿里团队出品的 Nodejs 教程。

2、[前端开发最全设计资源合集](https://github.com/bradtraversy/design-resources-for-developers?tab=readme-ov-file#ui-graphics)

作者列出了前端开发过程设计资源，包括UI、字体、颜色、图标Icon、Logo、网页模板、CSS 框架、CSS动画、前端框架Vue、React、Angular、Svelte UI库、在线设计工具网站等等清单。
