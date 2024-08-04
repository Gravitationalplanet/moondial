> 本文由 [简悦 SimpRead](http://ksria.com/simpread/) 转码， 原文地址 [sspai.com](https://sspai.com/post/70778)

> 前言我之前在 Newsletter 里分享了用 CraftXSnippets 记录晨间日记的方法，评论区收到一个关于 DailyNotes 如何归档整理的小问题，回复中也思考了一番 Craft 这个应用本身。

**编注：**

本文是少数派 [2021 年度征文](https://sspai.com/post/70693) 活动 `#效率` 标签下的入围文章。本文仅代表作者本人观点，少数派对标题和排版略作调整。

和往年不同，今年文章的数据表现将很大程度上决定征文活动的最终走向，包括「双倍稿酬（由飞书赞助）」活动奖励、最终票选名单以及征文奖品类型。如果你喜欢这篇文章，不妨通过充电或评论的方式支持作者。

前言
--

我之前在 Newsletter 里分享了用 Craft X Snippets 记录晨间日记的方法，评论区收到一个关于 Daily Notes 如何归档整理的小问题，回复中也思考了一番 Craft 这个应用本身。作为我在过去的一年中最喜爱、又带给我很大帮助的应用，想在新年伊始为它当一回「传教者」，在此展开讲讲，它有哪些特别之处，我为何喜欢它，以及一些使用上的研究和小技巧；当然，也会有它的不足。

![](https://cdnfile.sspai.com/editor/u_/c7aiuqdb34tafsdptd7g.png?imageView2/2/format/webp)

Craft 是去年 Apple 评选的 Mac App of the Year，也获得了 Apple Design Award「交互」赛道提名，足以说明它一定有值得称道之处。少数派在 [App Store Awards 2021](https://sspai.com/post/70259) 这篇文章中说它是：

> 虽然上线仅一年，Craft 的功能和体验却完全不输许多老牌笔记工具。在过去的一年多时间里，Craft 以非常高的迭代速度陆续带来了网页版本、实时协作、Daily Notes 等特性，几乎每个月都会推出新的重要功能。此次获得奖项，可谓实至名归。

是的，Craft 在 2020 年 11 月正式上线，到今天也就差不多一年的工夫。团队的精心打磨，使得它一上线就有着非常高的完成度。而过去一年中又陆续发布了 21 个大更新和 26 个小更新，也就是说，**几乎每 2-2.5 周就会有一个大更新。**我是从 iOS App Store 推荐知道它的，抱着试一试的态度，拿到手就被教学关近乎完美的动效吸引。在花了一点点时间探索，并看了帮助文档后，知道了很多令人心动的小细节，不免对这个应用心生好感，随即陆续把自己的笔记都搬了过来。

在使用 Craft 的一年里，时不时收到官方发来的「我们又更新了」的邮件，带来许多令人欣喜的 feature（很多时候刚好在想「要是有 xx 功能就好了」，结果真的更新了），并且他们的 [更新说明](https://sspai.com/link?target=https%3A%2F%2Fwww.craft.do%2Fwhats-new) 写得非常漂亮，读起来是一种享受，无处不传达着这个团队的热忱。

> 想了解 Craft，最简单的方法就是直接下载试用，也可以看看 [@红酒皇](https://sspai.com/u/Fabrina/updates) 的 [这篇文章](https://sspai.com/post/61784)，对 Craft 发布之初的功能作了非常详尽的描述。

[Craft - Docs and Notes Editor 的相关介绍](https://sspai.com/app/Craft%20-%20Docs%20and%20Notes%20Editor)[Craft - Docs and Notes Editor 的下载地址](https://sspai.com/d/JvPRoz)

它能干嘛，与大多数时兴的笔记应用大差不差，Markdown、所见即所得、块状笔记、无限层级、双向链接、分享、协作、本地存储… 等等，该有的都有。接下来，我将结合一些使用过程中的例子，介绍一些细节和常用的 usecase。

Craft 的空间与文档结构概念
----------------

![](https://cdnfile.sspai.com/editor/u_/c7aiuqlb34tae1klc9s0.png?imageView2/2/format/webp)

可以看到，Craft 是以 Space（空间）来划分工作区的。也很好理解，相当于其他应用的 Workspace，用于区分各种项目，或与不同人合作。与其他 Block-based 笔记应用相似，Craft 也是以 Block（块）为基本单位，每一个段落都是一个 Block。当一个 Block 里面包含了其他内容，它就变成了一个 Page，可以点进去，展开一个新页面。其中最顶层的 Block，也就是「新建」按钮按下去新增的那个，叫做 Document（文档），它可以被添加到文件夹中进行整理。**文件夹可以嵌套子文件夹，当一个文档不属于任何一个文件夹时，它就会被暂时放在 Inbox 中。**

> 值得注意的是，只有 Folder 和 Document 会显示在文档列表以及侧边栏中，里面的 Block 和 Page 都不会显示。

![](https://cdnfile.sspai.com/editor/u_/c7aiuqtb34tafsdptd80.png?imageView2/2/format/webp)

### 三种不同的 Space

Craft 的工作区，有以下三种类型

*   Private Space，也就是创建账号后，默认的个人空间，不能与他人协作。一般个人文档、草稿等，放在这里即可
*   Shared Space，可以邀请他人实时协作（当然，只有自己一个人也没关系）
*   External Location，外部空间，所有文档都会被保存在本地，不会备份到 Craft 的服务器。也可以把外部空间设定在 iCloud Drive 中，就会通过 iCloud 来同步。或者备份至任何网盘或磁盘，都是可以的。一些重要、隐私的文档可以考虑放在这里（不过，只有 Pro 用户才能使用这个功能）

![](https://cdnfile.sspai.com/2022/01/05/bbd8dfe1c16ddf7dbf2225ba1ae59446.png?imageView2/2/format/webp)Your Data is Yours.

Craft 支持创建多个 Space，文件夹可以嵌套文件夹，文档内部的 Block 也是无限层级的，这就给了我们极大的自由度来规划。比如，我会把自己的 Newsletter 相关内容单独开辟一个 Space，把账号整理这一类较隐私的内容放在外部空间（它们也不常被打开）。

不过，我当初看中它主要还是因为极舒适的使用体验。

完美的移动端交互
--------

Reddit 看到有网友说

> Now, after getting tired of Notion lags and Obsidian’s clunky mobile app and too much freedom, I happily landed on Craft.

他提到了 Notion 的延迟以及 Obsidian 笨拙的移动应用和过高的自由度。市面上的笔记应用我也大多用过一二，Notion 和 Obsidian 又是其中的热门选手，使用它们的过程中，能学到很多思考的方法，也曾经研究了不少。它们的共同特点是非原生，操作起来总觉得有些卡卡的。Notion 因为是在线应用，需要网络同步数据，有时候加载会转小圈圈（而且很奇怪，有些文档明明没几个字也没有图片，打开就是会加载一下；而有些文档很大，却一下就出来了）。Obsidian 版本号还在 0.xx.xx，虽然有优秀的插件、主题系统供选择，但也时不时会出现令人别扭的小问题。

不过呢，大多数笔记应用的「桌面端」都还是过得去的，因为桌面有键盘、触控板、鼠标，还有快捷键加持，有很多简化操作的方式；桌面显示区域也大，UI 也有更多的发挥空间。但「移动端」就不一样了，抛开 iPad 能外接键盘不说，手机上绝大多数时候是触屏操作，一个优秀的移动应用，交互与展示需要花很多心思去适配，又要与桌面端操作逻辑基本一致，以免切换平台的时候让人摸不着头脑。Notion 和 Obsidian 的移动应用说实话有些差强人意，每次打开前都要做一番思想工作，最后都不太想在手机上编辑文档了。

所以，发现 Craft 的时候真的是太感动了。原生应用，操作行云流水，再加上美观的渲染，每一次输入、选择、修改，或是分享、导出，都让人眼前一亮，感到一种快乐。

> No more spinners between you and your ideas. Built natively for iOS and macOS, Craft delivers the experience you’ve been waiting for.

比如以下几个我很喜欢的小细节⬇️

### 快速返回、全局搜索

Craft 支持无限层级嵌套，也就意味着当前浏览的页面可能是一个藏得很深的层级。这时，如果想返回顶层，或者想回到文档列表怎么办呢？手机上又没办法像 Mac 端能有一个侧边栏，滑动屏幕也只能一级一级返回。

![](https://cdnfile.sspai.com/editor/u_/c7aiurdb34tafo2ng37g.png?imageView2/2/format/webp)

我们都知道，iOS 14 引入了「长按返回键」展开层级列表功能，可以一次选择想返回的层级，不用再重复返回许多次了。

![](https://cdnfile.sspai.com/editor/u_/c7aiurlb34tafo2ng380.png?imageView2/2/format/webp)iOS 14 引入的长按返回键功能

Craft 当然也支持这个功能，长按返回键将会展示当前页面所在的层级，可以一次回到任何之前的层级。

![](https://cdnfile.sspai.com/editor/u_/c7aiurtb34tae1klc9sg.gif)长按返回键将会出现一个浮窗

不仅如此，它还有一个「下拉搜索」的功能，在打开的文档顶部，继续下拉屏幕，将会出现「快速搜索栏」，并有一些**快捷指令，用于回到全部文档、星标文档、当日的 Daily Note 以及创建新文档**。同时，搜索栏还会展示最近打开的文档列表。

![](https://cdnfile.sspai.com/editor/u_/c7aius5b34tafo2ng38g.gif)

> 小技巧：在任意页面，「双指轻触屏幕」也能唤起这个快速搜索栏。Mac 端这个操作的快捷键是 cmd+O。

这个功能非常实用，尤其是当我们**在 Pages 和双链中跳来跳去，不知道已经到了什么位置，**它可以让我们无论在什么地方都可以快速回到全部文档、搜索打开想要的文档，或者直接新建一个。

### 在输入状态下轻扫 Block 以改变缩进

这是一个很惊喜的小功能。我们知道键盘收起时，「选中」当前 Block 可以设置它的缩进，但也意味着我们得把键盘收起来，「取消输入状态」，才能设置格式。Craft 引入了一个功能，支持左右轻扫「当前正在输入」的 Block 来快速改变缩进，不需要等到关闭键盘，再左右划动来改变缩进了。手机上没有 Tab / Shift+Tab 快捷键，编辑中这个动作很方便。

> 注意：键盘展开和键盘收起状态的轻扫动作，效果是不一样的，建议自己体验一下。也不要用力太重了。

![](https://cdnfile.sspai.com/editor/u_/c7aiusdb34tae1klc9t0.gif)

### 流畅的 Block 选择 & 取消选择

上下划动 Block 右侧的选择框，就可以进行批量选择。响应速度非常快，**而且还有 Haptic 触屏反馈，使用起来真的很 Happy。**

![](https://cdnfile.sspai.com/editor/u_/c7aiuslb34tafrthsq4g.gif)

### 两手操作，移动端也能做到不同页面间拖拽

如果要把 Block 移动到当前页面的子页面中，除了复制粘贴，还能用两只手一起操作，「直接移过去」。一个手指先拖动所需的 Block，然后按住不放，另一只手用来导航至目标页面，到达想要的页面后，就可以松手了。

这个功能在其他应用真的很少见。不过目前只支持向下移动到子页面，不能向上移动到更高的层级中（返回按钮在拖动中是无法激活的）。

![](https://cdnfile.sspai.com/editor/u_/c7aiustb34tafo2ng390.gif)

### 最基本但也最容易忽视的一点：有收起键盘的按钮

这是我选择移动端笔记应用非常重要的要素之一，没有它，可能直接就 Pass 了（比如 Obsidian 就没有...）这个功能很重要，但也不是每家应用都会做到。有时候想收起键盘，但没有这个按钮，就得返回到上一级，再重新进入，很麻烦。

![](https://cdnfile.sspai.com/editor/u_/c7aiut5b34tafrthsq50.jpeg?imageView2/2/format/webp)

### 点击小箭头，直接将 Block 转换成 Page

在编辑当前 Block 时，直接点击键盘上方的箭头按钮进入下一层，就可以把这个 Block 的内容作为子页面的标题，直接开始输入了。这个功能使得我们不需要再多点一下来转换 Page，在快速组织内容的时候非常实用。

![](https://cdnfile.sspai.com/editor/u_/c7aiutdb34tae1klc9tg.jpeg?imageView2/2/format/webp)

### 一键 Group & Ungroup

Craft 提供了 Group & Ungroup 的智能按钮，批量选择一些 Block，点击这个按钮，就能快速创建一个「组」，也就是一个 Page。如果是以「文字 - 列表」形式批量选择，最上方的「文字」还会直接作为子页面的「标题」。

![](https://cdnfile.sspai.com/editor/u_/c7aiutlb34tafsdptd8g.gif)划动选择，点击 Group

同样，想把一个 Page「拆散」，用 Ungroup 也很方便。

![](https://cdnfile.sspai.com/editor/u_/c7aiuu5b34tafo2ng39g.gif)划动选择，点击 Ungroup

可定制的渲染样式
--------

作为一个笔记应用，颜值也是很要紧的。界面不好看，写的时候总会有些苦闷🤣。Craft 编辑器是所见即所得的，本身团队就已经为每一个 Markdown 元素打造了美观的样式，也提供了一些自定义选项，让文档更符合个人的审美需求。举几个例子。

### Task

Markdown Syntax 是 `- [ ]` 和 `- [x]`。有未完成、已完成、已删除三种 checkbox 的状态。

![](https://cdnfile.sspai.com/editor/u_/c7aiuudb34tae1klc9u0.png?imageView2/2/format/webp)

根据缩进，checkbox 会交替显示方形或圆形。

![](https://cdnfile.sspai.com/editor/u_/c7aiuudb34tafo2ng3a0.png?imageView2/2/format/webp)

也可以在 [偏好设置 - 高级设置] 中进一步设置「已完成」的 Task 如何显示。可以从 Strikethrough、Faded、None 三种样式中选择，默认 Strikethrough。

![](https://cdnfile.sspai.com/editor/u_/c7aiuulb34tafo2ng3ag.png?imageView2/2/format/webp)

### 引用

Markdown Syntax 是 `>` 。可以渲染成 Focus 也可以渲染成 Block，也可以两者结合。

可以与其他文字格式搭配使用，比如 Heading、Page、Card 等，再搭配上颜色，可以有非常丰富的展现形式。

![](https://cdnfile.sspai.com/editor/u_/c7aiuutb34tae1klc9ug.png?imageView2/2/format/webp)

### 分割线

Markdown Syntax 都是 `---` 。有四种样式，可以根据喜好来进行选择。我比较喜欢第一、二种，视觉效果更「轻」。

![](https://cdnfile.sspai.com/editor/u_/c7aiuutb34tafsdptd90.png?imageView2/2/format/webp)

### 图片

几张图片连续放置，有不同的 Layout 形式。默认情况下，Craft 会自动选择一种合理的方式。比如两张图片的方向，一个是 Portrait，一个是 Landscape，就适合并排放置。

![](https://cdnfile.sspai.com/editor/u_/c7aiuv5b34tafo2ng3b0.png?imageView2/2/format/webp)

可以设置 Image Size 和 Image Fit。其中 Image Size 指的是多张图片连续放置时，是自动并排展示，还是各自占据一行。Image Fit 指的是图片在自己的「格子」中如何填充。

![](https://cdnfile.sspai.com/editor/u_/c7aiuvdb34tae1klc9v0.png?imageView2/2/format/webp)

> 另外，当添加 Unsplash 图片时，会有一个小小的角标，点击可以前往相应的作者主页。

### Page

一个子页面的默认样式都是「Page」，即一个「代表页面的小图标」。也可以设置为 Card（卡片），或者什么都没有，就是普通的一行，页面内容会展示在该行下方。还能与 List、Task、Focus 等样式组合使用，非常方便。

![](https://cdnfile.sspai.com/editor/u_/c7aiuvdb34tae1klc9vg.png?imageView2/2/format/webp)

至于 Card，那就更多样化了，样式就有 5 种，还能设置字体、背景色、背景图等，建议可以自己玩玩看（非 Pro 用户可以用的卡片样式有限）。

![](https://cdnfile.sspai.com/editor/u_/c7aiuvlb34tafsdptd9g.png?imageView2/2/format/webp)

卡片有着丰富的自定义样式，很适合作为作品集、Gallery 的展示，分享出去就是一个美观的个人主页了。

### 链接

Craft 会自动获取链接的 icon、标题和摘要展示出来。常规模式就是每一个链接占据一行。

![](https://cdnfile.sspai.com/editor/u_/c7aiuvtb34tae1klca00.png?imageView2/2/format/webp)

也可以修改 Layout，可以从紧凑、常规、卡片三种形式当中选。

![](https://cdnfile.sspai.com/editor/u_/c7aiv05b34tae1klca0g.png?imageView2/2/format/webp)

以下是紧凑与卡片形式的示例。紧凑模式，链接的摘要就不会被显示了。卡片模式，会形成一个 Gallery，可以用来做一个自己的书签站、导航站，十分美观。

![](https://cdnfile.sspai.com/editor/u_/c7aiv0db34tafo2ng3bg.png?imageView2/2/format/webp)![](https://cdnfile.sspai.com/editor/u_/c7aiv0lb34tafsdptda0.png?imageView2/2/format/webp)

丰富的扩展支持
-------

笔记工具，只有好看还不够，还要好用。一个工具想要更好地融入我们的工作流，它必须不能局限于自己本身，而需要提供一些可以与其他应用「交流」「打通」的方式。好在 Craft 也提供了许多时兴的扩展方式。

### Share Extension

Craft 安装后，自带 Share Extension，支持 iOS Share Sheet 与 macOS Share Menu。目前支持分享文字、链接、图片、PDF 以及其他文件。

看到什么好东西，想记录到 Craft 中，**就不需要再重复「复制或保存至本地 - 打开 Craft - 找到需要的文档 - 粘贴或上传」这个笨重的过程了。**只要在需要发送的内容上，点击系统的 Share 按钮，找到 Craft 图标即可（macOS 一开始可能需要手动点亮 Craft 图标）。

可以选择添加到已有文档，也可以新建文档，但还不支持添加到 Pages。

![](https://cdnfile.sspai.com/editor/u_/c7aiv0tb34tafrthsq5g.png?imageView2/2/format/webp)iOS Share Sheet![](https://cdnfile.sspai.com/editor/u_/c7aiv15b34tafo2ng3c0.png?imageView2/2/format/webp)macOS Share Menu

### Widgets 与 Shortcuts

随着 macOS 对 Widgets 与 Shortcuts 这两个原生「快捷方式」的支持，越来越多的工具（以及非工具）应用开始加入这一阵营。Craft 当然也不示弱。

目前，有以下两类小组件，分别是打开单个文档，以及展示所选 Space 的最近文档（有两种尺寸的小组件可供选择）。

![](https://cdnfile.sspai.com/editor/u_/c7aiv1db34tae1klca10.png?imageView2/2/format/webp)

也提供了六种 Shortcuts Action，创建动作的时候，搜索 Craft 即可找到。

![](https://cdnfile.sspai.com/editor/u_/c7aiv1lb34tafsdptdag.jpeg?imageView2/2/format/webp)

至于如何使用，我会在后文的 Daily Notes Usecase 部分中详细介绍，这里先做一个简单带过。你也可以试着自行探索。

### URL Scheme

好像也是在少数派看到的，说评判一个效率应用是否优秀的标准，是看它是否对 URL Scheme 支持良好。简单来说，URL Scheme 可以让不同的应用在设备的沙盒机制下互相传递信息，实现一些自动化，大大简化我们的工作流。可以看 [@Hum](https://sspai.com/u/nfwvx7dn/updates) 的 [这篇文章](https://sspai.com/post/44591) 进一步了解。

目前 Craft 提供了以下四种 URL Scheme

*   打开文档
*   创建文档
*   添加内容至已有文档
*   在某一个 Space 执行搜索

至于具体怎么用，这篇 [官方帮助文档](https://sspai.com/link?target=https%3A%2F%2Fsupport.craft.do%2Fhc%2Fen-us%2Farticles%2F360020168838-Using-URL-Scheme) 已经很详细了，不再赘述。我在这里想展开讲讲其中的一些参数。

比如「打开文档」的 URL Scheme 是这样的：

`craftdocs://open?spaceId=<spaceId>&blockId=<blockId>`

而假如我们在分享菜单中复制一个 Craft 文档的 Deeplink，发现结果也是：

`craftdocs://open?...`

![](https://cdnfile.sspai.com/editor/u_/c7aiv1tb34tafrthsq60.png?imageView2/2/format/webp)

这也说明了 Deeplink 其实就是一个 URL Scheme，用于打开 Craft 应用的特定 Block。官方的解释是：

> Deeplinks create a URL that can directly link to a document, page, or even the selected block inside the Craft app itself - clicking on them from anywhere on your system should open the Craft app to that point.

那么，Deeplink 到底是什么？有出现在哪里过吗？

其实我们用 @ command 和传统的 [[wikilink]] 形式创建的双链，就用到了 Deeplink。

![](https://cdnfile.sspai.com/editor/u_/c7aiv1tb34tafo2ng3cg.png?imageView2/2/format/webp)这里，Getting Started 的链接，就是一个 Deeplink

再来看看 URL Scheme。其中，spaceId，顾名思义就是你加入的 Space 的 ID。**如果是你的 Private Space，那么这个 spaceId 也等同于「用户 ID」；如果是一个 Shared Space，不是成员将无法使用这个 URL Scheme。**

> 所以，虽然说 spaceId 即使被别人知道，对方没有登录我们的账号或是加入团队空间，也没办法做什么，但还是保护好比较好。

有了 URL Scheme，就可以大大扩展我们的 Workflow。可以和其他 URL Scheme 支持良好的应用配合，比如 Drafts 社区有一些很好的 [动作](https://sspai.com/link?target=https%3A%2F%2Factions.getdrafts.com%2Fsearch%3Futf8%3D%25E2%259C%2593%26q%3Dcraft)，把它们安装下来，就可以实现 Drafts -> Craft 的完美配合（当然，全部自己写也可以）。

![](https://cdnfile.sspai.com/editor/u_/c7aiv25b34tafrthsq6g.png?imageView2/2/format/webp)

我通常会使用 Drafts 做闪念笔记，因为它打开即写，写完即走，不用考虑标题，能打 tag，而且有非常好用的 Share Sheet 扩展。Drafts 还支持多个草稿合并，可以把随手记录的碎片整理起来，再一起发送出去。**把 Drafts 作为文字的起点，把 Craft 作为整理的终点，这个组合拳我很喜欢。**

与之相似的 Taio 也是优秀的文本处理与剪贴板工具，也支持自定义 Action。另外，配合简悦还能实现一直呼声很高的 [网页剪藏](https://sspai.com/link?target=https%3A%2F%2Fgithub.com%2FKenshin%2Fsimpread%2Fdiscussions%2F3144) 功能（但我好想要官方的剪藏呀🥲）。这两个应用我没有怎么使用，大家也可以多推荐一些社区力量。

Craft X —— 更多的扩展可能性
-------------------

这是 v2.0 引入的新功能，目前仍在开发者预览阶段，应该不久就会发布正式版。可以看 [@SpencerWoo](https://sspai.com/u/spencerwoo/updates) 的 [这篇文章](https://sspai.com/post/70606) 进一步了解，我这边也不再赘述。

Craft X，全称 Craft eXtension，类似于 Obsidian 的插件系统，可以为输入、编辑与发布带来不少功能上的增强。

目前官方提供了一些 [示例扩展](https://sspai.com/link?target=https%3A%2F%2Fwww.craft.do%2Fs%2FOhmDYXrBwI2wZS)，帮助开发者理解与创造。除了这些，社区也已经诞生了不少好用的扩展，比如这个 [craft-toc-maker](https://sspai.com/link?target=https%3A%2F%2Fgithub.com%2Ftimpcfan%2Fcraft-toc-maker)。Craft 是没有自己的 TOC 或是大纲功能的，文档内部我们需要手动用 @ command 或是 [[wikilink]] 的形式来创建 TOC（很麻烦）。使用这个扩展可以自动创建 TOC，并支持一些样式及插入位置的设定。

![](https://cdnfile.sspai.com/editor/u_/c7aiv2db34tae1klca1g.gif)

另外，也可以在 [Craftery](https://sspai.com/link?target=https%3A%2F%2Fcraftery.io%2F) 这个网站寻找更多的资源。

Daily Notes Usecase
-------------------

Daily Notes 是 v1.6 的一个重要更新。在侧边栏增加了日历视图，每一个日历格子都对应着一个当天的 Daily Note。它相当于一个当日的汇总，可以规划待办，记录日常会议，也可以单纯写一些日记，或是连通系统日历，把日程也放进来，非常自由。**有了 Daily Notes，就不需要手动输入日期去建立一个指向每一天的文档了。**

Daily Notes 与普通文档一样，可以分享，也可以导出，唯一的区别就是它不会出现在「全部文档列表」，只会乖乖待在日历视图，这样，就不必担心随手记录的文字会「污染」正式文档了。**当然，如果想查找，也可以用日期进行快速搜索，如「12/31」。**

![](https://cdnfile.sspai.com/editor/u_/c7aiv2lb34tafsdptdb0.png?imageView2/2/format/webp)Daily Notes

### 针对「任务」的特化设计

Daily Notes 针对任务作了一些相应的适配，它会统计当日的日记中所有 Task 类型的 Block，我们可以看到当天一共有多少任务，完成了多少 ，滞后了多少。右上角还有一个展示进度的饼图，非常直观。

![](https://cdnfile.sspai.com/editor/u_/c7aiv2tb34tafrthsq70.png?imageView2/2/format/webp)日记中的任务统计

并且在外面的列表视图中，只会显示 3 行，优先展示未完成的任务，其他文字以及已完成的任务会放在后面。**（可以上下两张图对比着看，能看到列表视图并不是按照实际文字顺序显示的。）**

![](https://cdnfile.sspai.com/editor/u_/c7aiv2tb34tafo2ng3d0.png?imageView2/2/format/webp)列表中优先显示未完成任务

因此，Daily Notes 用来追踪当日任务特别好用。

### 如何快速记录？

虽然 Craft 的搜索与查找功能很强大，但是每次想在日记中记些什么，就得打开应用，找到 Today，还是挺麻烦的。以下两招可以帮助我们快速记录日记。

#### 1⃣️ 使用 Widgets

用于打开「单个文档」的小组件，现在可以指定它来显示 Daily Notes。除了指定具体的日期，也可以选择 Yesterday、Today 和 Tomorrow 这种形式。点击设定好的小组件，Craft 会自动带你前往相应的日期。

可以按需选择，我一般只放 Today 的小组件，用于快速添加今天的所思所想。也可以放 Tomorrow 用于计划第二天，或者 Yesterday 用于回顾前一天。

![](https://cdnfile.sspai.com/editor/u_/c7aiv35b34tae1klca20.png?imageView2/2/format/webp)

#### 2⃣️ 使用 Shortcuts

在上文我提到，Craft 目前提供了 6 种动作。结合其中的 Add to Craft Doc 和 Open Document 这两个动作，可以创建一个「添加至当日日记」的捷径。

![](https://cdnfile.sspai.com/editor/u_/c7aiv3db34tafsdptdbg.png?imageView2/2/format/webp)

创建一个新的捷径，把上述两个动作添加进来，其中 Document 选择 Today，Space 选择你的个人空间或其他空间，给捷径命名并保存，就完成了。（当然，也可以选择添加至 Yesterday 或 Tomorrow。）每次运行，都会询问要添加的内容。运行完毕，会打开相应的 Daily Note。

![](https://cdnfile.sspai.com/editor/u_/c7aiv3lb34tafrthsq7g.png?imageView2/2/format/webp)![](https://cdnfile.sspai.com/editor/u_/c7aiv3tb34tafo2ng3dg.png?imageView2/2/format/webp)

以上小组件和捷径结合使用，就能快速记录当日想法。点击小组件，可以直接打开 Today；喊一声 Hey, Siri... 也可以唤起捷径直接记录。

### 如何归档与整理？

目前 Craft 还不支持对 Daily Notes 建立自动归档，也不能按年月等时间范围筛选，连查看哪些天写了哪些天没写也是不太直观的（虽然格子有颜色深浅区分）。我们需要采取其他方式自行整理。

#### Date Badges

在展开之前，先说说一个小特性：Date Badges。Craft 会把文档中的日期📅以「徽标」形式渲染出来，突出显示，方便与其他文字区分 。支持 @ command 和 / command 来输入，不过两者的呼出菜单略有不同。

当我们用 @ command 和 / command 输入以下形式的文字时，会出现日期选择

*   Today
*   Yesterday
*   Tomorrow
*   Next Sunday 这样的形式，会自动转换成日期
*   2021/11/11 这样的形式

选择日期后，就会转换成徽标。

![](https://cdnfile.sspai.com/editor/u_/c7aiv45b34tae1klca2g.png?imageView2/2/format/webp)

#### 自行创建日记归档

当我们点击一个 Date Badge，就能跳转到对应的 Daily Note。利用这一特性，可以自行建立归档文件夹来整理它们。比如，建立一个「日记」文件夹，里面按「年份」建立子文件夹，每一年里面按「月份」建立文档。之后，在每个月的文档中，用 Date Badge 链接到每一天的 Daily Note。

![](https://cdnfile.sspai.com/editor/u_/c7aiv4db34tafsdptdc0.png?imageView2/2/format/webp)

**当然，这只是一个例子，实际上这样归档也是挺麻烦的，而且比起自带的日历视图也没有什么特别大的改善。**我只是想说明，**Daily Notes 也可以引用或被引用，参与到双向链接中，**可以有许多整理的方式。不过，其实我从来不整理 Daily Notes，都是随它去的，我把它当成一个随手记录的地方，每天或每周回顾一次，截取想要保留的内容，转移到其他地方，就可以了。

至于有什么更好的归档与筛选方式，还是期待官方的更新了。

### 用 Craft X Snippets 记录晨间日记

Craft 是没有像 Notion 一样的模版功能的，也就是说，每一个文档（包括 Daily Notes）都要自己从零开始写，格式也要从头设置。我会用 Daily Notes 来写晨间日记，每次记录的形式大差不差，所以很需要模版功能。虽然手动建一个模版文档，每次复制粘贴一下也不是不行，但总归很麻烦。

好在上述的 Craft X 带来了扩展功能，官方也第一时间推出了一个叫做「Custom Snippets 自定义片段」的扩展，可以帮助「模拟」一下模版功能。（扩展的安装和使用方式看 [这里](https://sspai.com/link?target=https%3A%2F%2Fwww.craft.do%2Fs%2FOhmDYXrBwI2wZS%2Fb%2F0FD332FF-0D9E-4F09-8449-CE76B50820DB%2FCustom_Snippets)。）

先写一个模版，可以把格式也设置好。选中要作为「自定义片段」的部分，打开操作栏的扩展选项卡，选择「Save selected」并命名，就可以了。保存以后把原本的文字删除也没关系。

![](https://cdnfile.sspai.com/editor/u_/c7aiv4db34tafsdptdcg.png?imageView2/2/format/webp)创建自定义片段

使用的时候，在新建的 Daily Note 中，打开操作栏的扩展选项卡，点击之前保存过的自定义片段名称，它就会自动插入到文档中了。

![](https://cdnfile.sspai.com/editor/u_/c7aiv4lb34tae1klca30.png?imageView2/2/format/webp)使用自定义片段

使用起来还是很方便的。自定义片段也可以有很多花样，也不只是用在日记中，会议纪要、月度总结、读书笔记... 都可以这样使用。另外，Craft 团队也有提到 22 年会推出真正的「Templates 模版」功能，很期待。

分享与导出
-----

### 支持 TextBundle 大一统

TextBundle 将 Markdown 纯文本格式文件和它的图片附件打包绑定在一个文件里，让 Markdown 的图片难题不再是难题。许多支持 Markdown 的应用并没有支持 TextBundle，好在 Craft 是支持的，文档迁移、导入导出都变得非常方便，后续也不必担心想切换应用，数据该怎么办。

导入 TextBundle，只要点击 [File - Import] 即可。

![](https://cdnfile.sspai.com/editor/u_/c7aiv4tb34tafo2ng3e0.png?imageView2/2/format/webp)

TextBundle 导入后，会出现在 Imported Notes 文件夹下。打开其中的 text 文档，可以看到所有的图片也都一并导入进来了。

![](https://cdnfile.sspai.com/editor/u_/c7aiv55b34tae1klca3g.png?imageView2/2/format/webp)

至于导入 Markdown 文件，也是一样的过程。

### 导出为图片 —— 像素级复刻编辑器

Craft 还可以当作一款优秀的长图生成器。**它能做到编辑器里长什么样，导出的图片就长什么样。**文档里的图片和附件也会显示在导出的图片中。有时候发个微博或者发给联系人，用一张排版美观的图片更能说明问题。

我们可以设定图片的主题，目前有 9 种主题可供选择。

![](https://cdnfile.sspai.com/editor/u_/c7aiv5db34tafsdptdd0.png?imageView2/2/format/webp)

也可以设置图片的分割方式（一图流，或者分割成几张，选择 Fit Document 将会是一图流的形式）。也能调整文字大小，隐藏文档标题，定制项目还是挺多的。

![](https://cdnfile.sspai.com/editor/u_/c7aiv5db34tafo2ng3eg.png?imageView2/2/format/webp)

以下是我曾经导出过的舒伯特 D.960 笔记，可以作为一个参考。

![](https://cdnfile.sspai.com/editor/u_/c7aiv5lb34tae1klca40.jpeg?imageView2/2/format/webp)

### Secret Link —— 把文档变成一个好看的网页

在 Share 选项卡最上方，可以看到 Secret Link 链接分享。所有页面都可以以 Secret Link 的方式，变成一个网页，分享给其他人。这种方式也完美保留了编辑器里的样式，并且 Web 浏览可以**左右双栏**（可以参考 Craft 的 [更新说明](https://sspai.com/link?target=https%3A%2F%2Fwww.craft.do%2Fwhats-new)，都是直接用 Craft 写，并以链接形式分享的）。

> 注：如果想把该页面下的子页面和链接也分享出去，要记得开启 Share Block Links。

![](https://cdnfile.sspai.com/editor/u_/c7aiv5tb34tafo2ng3f0.png?imageView2/2/format/webp)

上文中也提到，Craft 文档可以自定义多种样式、颜色、卡片等组合，非常适合贴一些作品集、Gallery 进去，作为个人主页和博客。当然，这也离不开 Secret Link 的支持。不过，不像 Notion 有非常活跃的社区，每天都有大量的模版与页面的 idea 发布，Craft 目前能够参考的内容还是比较少的。但是呢，这两个其实不能算同一类型的笔记工具，按照自己的喜好来使用就可以了，Craft 怎么用都挺快乐的😊。

这里有一个 [博客](https://sspai.com/link?target=https%3A%2F%2Fwww.craft.do%2Fs%2FprWu9ohKSgta1T) 可以作为参考。

### 也许需要注意的：Markdown 与 Secret Link 对图片地址的不同处理

#### Share Markdown

Craft 会把文档里添加的图片上传至自家图床，因此导出的 Markdown 文件里的图片链接都是在线的地址，以 `res.craft.do/...` 开头（也就是说不用折腾图床了）。把这个 Markdown 文件分享给其他人，我们就不需要再费心打包图片，对方打开直接能看。

不过，需要注意的是，图片地址会包含文档所在的 spaceId（下图画红线 full 后面的部分）。与前面 URL Scheme 一节提到的一样，**虽然其他人得到 spaceId 也不能用来做什么，但如果不放心，还是不要随意分享出去。**

![](https://cdnfile.sspai.com/editor/u_/c7aiv65b34tae1klca4g.png?imageView2/2/format/webp)

#### Share Secret Link

如果以链接形式分享，图片地址将以 `secure-res.craft.do/...` 开头，是加密过的地址，不会包含 spaceId。类似下面这种：

`https://secure-res.craft.do/v1/y8TEuCnQ9sZvZEvPPB671BJnvQ1fDrbbb4acKPjiXUHtH9YjDdj3DkaKeScSpTxWHfSeBiZgKvhXUj63hxt512pLaPXrzxFWar4prR7GD6Cr3UB7LjkgnSySiuHxitN4v5ifuZ9f2oknNv2MzQ9wf5tWr1hexzGVnDDwszXNZuZGxW3r1at9ChXPhAYToVwwoN2yt4EN1Rskexr8povjsyYqGRTDgXJBWBae7ZXJtQyDtXvahSdoZ7RHJMAXys7Eop1ZaKeZFWj9rqzwNVTTq28PPCFi/Image.jpg`

这时，如果取消链接分享，上面的图片地址也将不可访问。

最后，几个小技巧
--------

还有一些内容不知道归类在哪里，就算作 Tips 吧。

1⃣️ 关于 Task 的小技巧

可以通过输入字母 `x` 来快速建立 Task。不需要快捷键了，在英文写作中尤其方便，中文写作由于输入法切换，其实没有那么顺畅。

![](https://cdnfile.sspai.com/editor/u_/c7aiv6db34tafsdptddg.gif)

2⃣️ 关于页面标题的小技巧

除了正文，页面标题也可以使用 emoji 和 / command。比如可以快速输入日期，调整标题颜色、字体，或是用 emoji 让文档更加个性化等等。

![](https://cdnfile.sspai.com/editor/u_/c7aiv6lb34tafo2ng3fg.gif)

Craft 的不足之处
-----------

说了这么多好的地方，Craft 当然也有它的不足。

*   价格摆在那里（当然我觉得物有所值），比 Bear 贵上不少，并且非 Pro 用户的功能十分有限，比如只能使用 1000 个 Block、只有 1GB 的存储空间、一个页面最多 3 个反链、不支持文档内部搜索等等
*   没有 Database 支持，目前的 Table 也很弱，操作起来不顺的地方很多（好在我并不太用到表格）。如果你非常需要 Notion 那样的数据库结构，Craft 不适合你
*   没有 Synced Blocks，一处修改处处生效的那种[（Notion 用户应该知道我在说什么）](https://sspai.com/link?target=https%3A%2F%2Fwww.notion.so%2Fhelp%2Fsynced-blocks)
*   没有 Tag 和 Template 系统，不过今年可能会引入
*   社区不像 Notion 和 Obsidian 那样活跃，有很多的内容和创意可以借鉴~（不借鉴也没啥）~

另外，这里是一个网友总结的 [Wishlist for Craft](https://sspai.com/link?target=https%3A%2F%2Fwww.craft.do%2Fs%2Fdxwb0SsrGtPF47)，可以看看有什么与你的想法相似的。按照过去一年的更新速度，相信 2022 年也会有不少新功能和改进面世。

结语
--

去年的大多数时候都在用 Craft 记录与整理，发现我好久没有因为一款应用那么感动了。知道 Notion 那个时候是兴奋，但是很惭愧，我用不好，一直想弄得很 fancy，看很多人的创意，自己还是用得很累（机心太重，当然也有「移动端太破」这个原因🤣）。Btw，每个人的诉求真的是不一样的，所以，当看到好的产品要大胆去尝试，觉得哪里不好，也不必硬用。

Craft 团队有一句话：

> Our mission is to create a beautiful and joyful space where you no longer feel like you are fighting the tool.

对我来说，Craft 就是目前的 THE ONE 了吧。

社区与资源
-----

*   [Discourse: Craft X Developer Forum](https://sspai.com/link?target=https%3A%2F%2Fforum.developer.craft.do%2F)
*   [Reddit: CraftDocs](https://sspai.com/link?target=https%3A%2F%2Fwww.reddit.com%2Fr%2FCraftDocs%2F)
*   [GitHub: Awesome-Craft](https://sspai.com/link?target=https%3A%2F%2Fgithub.com%2Fxvhang%2FAwesome-Craft)
*   [Craftery: 一个扩展收集站](https://sspai.com/link?target=https%3A%2F%2Fcraftery.io%2F)

供参考。也欢迎分享你的看法。

> 下载少数派 [客户端](https://sspai.com/page/client)、关注 [少数派公众号](https://sspai.com/s/J71e)，让你的工作更有效率 ⏱

> 年度回顾、好物推荐…… 更多精彩尽在 [少数派 2021 年度盘点](http://sspai.com/page/2021) 🎉