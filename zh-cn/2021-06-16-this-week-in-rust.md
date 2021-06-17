# Rust 官方周报 395 期（2021-06-16）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。
> 
> 关于周报中的资源链接，已经有中文资源的，替换为中文资源链接（中文资源中，均附有原文链接）。另外，对于部分周报文章，附有阅读和简单了解后的译注，但并非全部。如果你阅读了文章，有更适合的见解，请联系、PR，或者直接参与项目 [github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)。

大家好，欢迎查阅第 395 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

# Rust 社区更新

**高亮**
CW 电视网：自杀（Suicide）、心理健康（Mental Health）

下文中的链接，是为了悼念 Rust 社区的一个贡献者。关于真正公正地对待逝者方面，这是一个非常敏感的话题。而对于我们生者，所能做的最重要的事情，唯有提高对心理健康的认识。

如果你或你所认识的人需要自杀预防热线，请访问 <https://www.opencounseling.com/suicide-hotlines>，获取你们国家的紧急情况和自杀预防热线的电话号码。

[开源与心理健康](https://www.redox-os.org/news/open-source-mental-health/)（译注：redox-os 的贡献者，jD91mZM2，年仅 18 岁）

### 官方
* [内部] [Rust 1.53.0 预发布测试](https://blog.rust-lang.org/inside-rust/2021/06/15/1.53.0-prelease.html)（译注：Rust 1.53.0 今天发布，中文请参阅 [Rust 1.53.0 明日发布，关键新特性一瞥](https://blog.budshome.com/budshome/rust-1.53.0-ming-ri-fa-bu-,guan-jian-xin-te-xing-yi-pie)）
* [Inside] [请欢迎 Boxy、Léo Lanteri Thauvin，以及 the8472 成为编译器贡献者](https://blog.rust-lang.org/inside-rust/2021/06/15/boxyuwu-leseulartichaut-the8472-compiler-contributors.html)

### 简讯
* [Rust 游戏开发月报 #22 - 2021 年 5 月](https://gamedev.rs/news/022/)

### 项目/工具更新
* [rust-analyzer 更新日志 #81](https://rust-analyzer.github.io/thisweek/2021/06/14/changelog-81.html)
* [AWS-SDK-Rust：CloudFormation、SageMaker、EC2，以及 SES](https://github.com/awslabs/aws-sdk-rust/releases/tag/v0.0.8-alpha)
* [Aya 发布 0.10.1 版本](https://confused.ai/posts/announcing-aya)（译注：aya 是 Rust 实现的 eBPF 库）
* [TensorBase 周报 7 期](https://tensorbase.io/thisweek/2021-06-16-tw_7/)
* [cap-std 介绍，Rust 标准库基于 capability 的版本](https://blog.sunfishcode.online/introducing-cap-std/)
* [大事件，wasmer 2.0 发布！](https://wasmer.io/posts/wasmer-2.0)（译注：wasmer 提供基于 WebAssembly 的超轻量级容器。其号称可以运行于任何地方：桌面、云、IoT 设备，甚至能嵌入到任何编程语言）
* [`iterate` 库介绍](https://www.reddit.com/r/rust/comments/nwdyip/new_create_announcement_iterate/)
* [ripgrep 13.0.0 版本发布](https://github.com/BurntSushi/ripgrep/releases/tag/13.0.0)

### 观测/思考
* [关于 Fuchsia 安全的几点思考](https://blog.cr0.org/2021/06/a-few-thoughts-on-fuchsia-security.html)
* [使用 Rust 实现 shell 的历史搜索（history search）/同步（Ellie Huxtable 访谈)](https://console.dev/interviews/atuin-ellie-huxtable/)
* [Rust 中的可视化内存管理](https://deepu.tech/memory-management-in-rust/)（译注：文章精要概括，推荐）
* [视频] [Flutter 开发中使用 Rust](https://youtu.be/iQer8hUu0Es)

### Rust 演练
* [嵌入式 Rust 开发：为 STM32F3DISCOVERY 构建闪烁（Flash）二进制程序](https://blog.knoldus.com/embedded-rust-build-flash-binary-to-stm32f3discovery/)
* [使用 Rust 进行飞行学习（Learning to Fly）：模拟和进化（4）](https://pwy.io/en/posts/learning-to-fly-pt4/)（译注：系列文章，共 4 篇，开发者使用神经网络和遗传算法开发的飞行模拟游戏，从零开始，直到用户界面，内容很详实）
* [使用 Rust + WebAssembly 提速 WebCola 图形可视化库](https://cprimozic.net/blog/speeding-up-webcola-with-webassembly/)（译注：效果真的很棒，比如下图这个复杂的谱图关系，操作全面，响应极速）
![使用 Rust + WebAssembly 提速 WebCola 图形可视化库](https://blog.budshome.com/static/articles/1623905978.jpg)
* [从 NAND 到 Raytracer：Hack 计算机上的光线追踪（Raytracing）](https://blog.alexqua.ch/posts/from-nand-to-raytracer/)（译注：请注意 Hack 计算机，Hack computer 仅支持黑白二色，光线要做灰度映射）
* [Cacao：使用 Rust 构建 macOS（及 iOS）应用](https://rymc.io/blog/2021/cacao-rs-macos-ios-rust/)（译注：和以前的实践类似，还是很麻烦）
* [在 Rust 构造 API（1）](https://dev.to/naruhodo/build-an-api-in-rust-part-1-5c4g)
* [为了兴趣和利益，学习在 Rust 构建一个解析器（Parser）](https://dev.to/pancy/learn-to-build-a-parser-in-rust-for-fun-and-profit-2id5)
* [在 AWS Lambda 上运行 Rust 的初学者指南](https://dev.to/nicholaschiasson/beginner-s-guide-to-running-rust-on-aws-lambda-277n)
* [使用 Rust 实现命令行键值（k-v）数据存储](https://dev.to/sirneij/a-command-line-key-value-data-store-using-the-rust-programming-language-33b6)
* [如何在 Rust web 应用中使用 casbin 授权（3）](https://dev.to/smrpn/how-to-use-casbin-authorization-in-your-rust-web-app-part-3-4g2f)
* [从 `serde` 库切换到 `nom` 库，输入信息的解析速度提高了 3-10 倍](https://medium.com/tezedge/speeding-up-incoming-message-parsing-by-3-to-10-times-by-switching-from-serde-to-the-nom-library-a74b04391bb4)
* [中文] [系列] [Rust 和 Wasm 的融合，使用 yew 构建 web 前端（3）- 资源文件及小重构](https://blog.budshome.com/budshome/rust-he-wasm-de-rong-he-,shi-yong-yew-gou-jian-web-qian-duan-(3)--zi-yuan-wen-jian-ji-xiao-zhong-gou)
* [中文] [系列] [Rust 和 Wasm 的融合，使用 yew 构建 web 前端（4）- 获取 GraphQL 数据并解析](https://blog.budshome.com/budshome/rust-he-wasm-de-rong-he-,shi-yong-yew-gou-jian-web-qian-duan-(4)--huo-qu-graphql-shu-ju-bing-jie-xi)（注：笔者此 2 篇文章，还有个小插曲。有位国人在 Rust 周报官方提出：笔者的博客拿 Rust 搞营销，广告多等，总之不能收录。因为官方编辑不懂中文，不了解博客实际，而让其审阅中文文章的，所以笔者未做辩解。笔者借此说明下：宣传意图属实，因为笔者希望分享给更多人看。本号关注朋友很少，但这些**第一阶段**的基础文章，每天都有不少朋友联系交流调试中的问题，证明对部分朋友，是有帮助的。文章末尾以前是有 1 条广告（**已移除**），但在国内拿 Rust 搞营销？真没有那个意图，Rust 学习者和使用者才多少……但笔者接受批评，博客文章不再有任何广告。谢谢指导。）
* [视频] [使用 Rust 构建 web 应用（1） - 配置](https://youtu.be/Wmq3etdwCbM)
* [视频] [使用 Rust 构建 web 应用（2） - 数据库](https://youtu.be/c9qSGUHgE1c)
* [视频] [Rust 中实现无锁（Lock-Free）及无等待的模拟仿真（2）](https://youtu.be/tNzCj8691LE)


### 研讨/论文

无

### 其它
* [Rustaceans 座谈会：Facebook Rust 攻城狮访谈系列](https://developers.facebook.com/blog/post/2021/06/03/meet-rustaceans-neil-mitchell/)
* [Pop!_OS 使用了大量 Rust](https://www.reddit.com/r/rust/comments/nyd1qw/pop_os_uses_a_lot_of_rust/)
* [关于 Fuchsia 安全的几点思考](https://blog.cr0.org/2021/06/a-few-thoughts-on-fuchsia-security.html?m=1)
* [视频] [主题演讲：Bryan Cantrill - 软硬件协同设计（Co-design）：即将到来的黄金时代（Golden Age）](https://youtu.be/nY07zWzhyn4)

# 周最佳 crate

本周最佳 crate 是 [nativeshell](https://github.com/nativeshell/nativeshell)，使用 Rust 开发 Flutter 应用，其中 [static-rc](https://github.com/matthieu-m/static-rc) 是一个编译时（compile-time）引用计数（reference-counted）的智能指针。

谢谢 [Zicklag](https://users.rust-lang.org/t/crate-of-the-week/2704/922) 的提议。

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。



* [boa-dev/boa has some good first issues](https://github.com/boa-dev/boa/labels/good%20first%20issue)
* [softprops/shiplift - We have too many unwrap() calls in the codebase](https://github.com/softprops/shiplift/issues/301)

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Rust 核心更新

[289 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-06-07..2021-06-14

## Rust 编译器性能

一些提升，一些会退，没有大的变化。

验测工作是由 **@simulacrum**完成的。修正范围：[1160cf..a50d721](https://perf.rust-lang.org/?start=1160cf864f2a0014e3442367e1b96496bfbeadf4&end=a50d72158e08e02cfc051b863017bdbd2c45b637&absolute=false&stat=instructions%3Au)

[此处可查阅完整报告](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-06-08.md).

## 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

*无*

## 新的 RFCs

* [RFC: fallible-allocation](https://github.com/rust-lang/rfcs/pull/3140)
* [Cargo alternative registry auth](https://github.com/rust-lang/rfcs/pull/3139)

# 近期活动

### 线上

* [June 17, 2021, Denver, CO, US - Python/Javascript 开发者学习 Rust - Juhis - Rust Denver](https://www.meetup.com/Rust-Boulder-Denver/events/277575285/)
* [June 18, 2021, Online - Rust 基础学习 | Rust 101 - KubeDaily](https://www.youtube.com/watch?v=DIxjk0HTx5U)
* [June 29. 2021, Dallas, TX, US - Last Tuesday - Dallas Rust](https://www.meetup.com/Dallas-Rust/events/jqxqwryccjbmc/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust 招聘信息

**Tweede golf**

* [Lead Developer Embedded Rust (Nijmegen, NL)](https://tweedegolf.nl/vacatures/2/lead-developer-embedded-rust)

**Paige**

* [Senior Software Engineer, Visualization (Remote, Europe)](https://boards.greenhouse.io/paige/jobs/5210311002)

**ChainSafe Systems**

* [Rust Developer (Remote)](https://jobs.smartrecruiters.com/ChainSafeSystemsInc/743999739358248-rust-developer)

**Gnosis**

* [Ethereum Core Developer (Remote)](https://arbeitnow.com/view/ethereum-core-developer-mwd-gnosis-126355)

**Braiins**

* [Rust Developer (Prague, CZ)](https://braiins.com/careers/rust-developer)

**NZXT**

* [Senior Software Engineer for CAM (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=259)
* [Senior Software Engineer for Streaming Software (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=317)

**Kollider**

* [Junior Backend Engineer (Remote)](https://kollider.homerun.co/junior-backend-engineer/en)
* [Senior Backend Engineer (Remote)](https://kollider.homerun.co/senior-backend-engineer/en)
* [DevOps Engineer (Remote)](https://kollider.homerun.co/devops-engineer/en)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

# 本周引语

> 如果把手动管理内存比喻为“挥舞着一把枪”，那么，借用检查器（borrow checker）就如同一种自动安全装置，以防止你在粗心地指着自己时，不小心扣动了扳机。但它是粗粒度（coarse-grained）的，并且在警告方面有差错；它将你的“足迹”模拟为矩形，而非一个详细的全方位（3D）网格。如果你**真的**以为可以将它放在脚趾之间，同时可以避免击中自己（例如：“此函数返回的值，必须在不超过 15 次的连续调用中，保持活动状态”）；那么，`unsafe` 将允许你做尝试，但借用检查器（borrow checker）的内置规则不够精确，无法帮助到你。然而，如果你不小心把手放在了前面，但却没有声明，借用检查器（borrow checker）仍然会阻止你。

– [infogulch 发表于 Hacker News](https://news.ycombinator.com/item?id=27468885)

谢谢 [StyMaar](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1056) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
