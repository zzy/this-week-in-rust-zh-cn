# Rust 官方周报 393 期（2021-06-02）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。
> 
> 关于周报中的资源链接，已经有中文资源的，替换为中文资源链接（中文资源中，均附有原文链接）。另外，对于部分周报文章，附有阅读和简单了解后的译注，但并非全部。如果你阅读了文章，有更适合的见解，请联系、PR，或者直接参与项目 [github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)。

大家好，欢迎查阅第 393 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

# Rust 社区更新

本周无相关官方博客，研讨/论文。

### 简讯
* [RiB 简讯 #24 - Bridges](https://www.reddit.com/r/rust/comments/nqt4ul/rib_newsletter_24_bridges/)

### 项目/工具更新
* [rust-analyzer 更新日志 #79](https://rust-analyzer.github.io/thisweek/2021/05/31/changelog-79.html)
* [GCC Rust 月报 #6 2021 年 5 月](https://thephilbert.io/2021/05/31/gcc-rust-monthly-report-6-may-2021/)
* [TensorBase 周报 5 期](https://tensorbase.io/thisweek/2021-06-02-tw_5/)（译注：TensorBase 是 Rust 实现的现代化开源数据仓库）
* [tower-http 工具集库发布](https://tokio.rs/blog/2021-05-announcing-tower-http)
* [Rust 思维应用（Turning rusty tech into Rust） ~ 当你必须用 FTP，但却不想使用的时候……](https://blog.abstractinvoke.com/05-07-unftp.html)（译注：unftp 库的介绍。unftp 是一个 FTP 的云应用，是基于 Rust 实现的旧式 FTP 的改造。目前未实现 SFTP）

### 观测/思考
* [Rust 中的面向对象编程概念](https://blog.knoldus.com/object-oriented-programming-concepts-in-rust/)（译注：主要是基于与 Java 语言的对比，介绍类和对象、继承、封装、多态性，以及抽象等面向对象编程在 Rust 的编程实现。适合 Java 程序员理解 Rust）
* [我的 Rust 初体验](https://blog.frankel.ch/start-rust/1/)（译注：文章很不错，娓娓道来，易读易理解）
* [深入浅出地理解 Rust 中的可变性（Mutability）和引用（References）](https://dev.to/arunanshub/demystifying-mutability-and-references-in-rust-caf)
* [GCC-RS 的简单替代方案](https://shnatsel.medium.com/the-simpler-alternative-to-gcc-rs-90da2b3685d3)（译注：GCC-RS 项目的目标可以概括为“用 C++ 重写 Rust 编译器”，作者认为根本无此需求，`rustc_codegen_gcc` 既可以实现 GCC-RS 项目所声称的所有优点）
* [为什么我支持 GCC-rs 项目](https://chorman64.medium.com/why-i-support-gcc-rs-dc69ebfffd60)（译注：标题即可看出是上一篇文章的争鸣）
* [“试驾 ” Rust](https://ferrous-systems.com/blog/rust-test-drive/)（译注：Rust 是否适合你的项目和团队？此文作者以非常实际的方法，对项目和团队做了是否采用 Rust 的考量建议）
* [波卡（Polkadot）公链线上事故复盘 - 24.05.2021](https://polkadot.network/a-polkadot-postmortem-24-05-2021/)（译注：知名公链波卡（Polkadot)）于 2021 年 5 月 24 日，在一个节点发生了一次比较大的线上事故（Out Of Memory），事故后，复盘原因是优化 Rust 标准库 binary search 导致的。搜索优化的作者（事故与作者无关系）于 5 月 29 日发表了文章：[我的Rust binary search PR 导致 Polkadot 线上事故的缘由](https://zhuanlan.zhihu.com/p/376138344)）
* [我一定要找出那只讨厌的臭虫（Bug）](https://www.reddit.com/r/rust/comments/nqjyb7/the_most_annoying_bug_ive_had_to_track_down/)（译注：有趣的文章，由浅入深，很有帮助和启发）
* [视频] [一次又一次 - 我们的 Rust 采纳历程 [Open Source North 2021 / Luca Palmieri]](https://youtu.be/1nKC505_uTU)

### Rust 演练
* [使用同步（Sync）及异步（Async）Rust 实现 RESTful API](https://github.com/pretzelhammer/rust-blog/blob/master/posts/restful-api-in-sync-and-async-rust.md)
* [Rust 闭包（Closures）让你的开发更轻松](https://blog.knoldus.com/rust-closures-will-make-your-life-easy/)（译注：闭包使用的基础文章，可选速读）
* [开发地道的（Idiomatic）的 Rust 二分法检索（Binary Search）扩展](https://c-hirsch.de/2020-05-30-idiomatic-rust-binary-search-extended)
* [“Rust 与安全编程（Safe Programming）”之间的关系](https://blog.knoldus.com/lets-know-about-the-relation-between-rust-and-safe-programming/)
* [Rust 中的严密（Tightness）驱动开发](https://www.ecorax.net/tightness/)（译注：作者阐述了严密驱动开发的规则，可以概况理解为：紧密贴合 Rust 类型）
* [Rust 中，使用 nix 开发一个基于 Riscv 内核的 “hello world”](https://justin.restivo.me/posts/2021-05-30-nix-rust-riscv-toy-kernel.html)（译注：nix 库试图为各种 *nix 平台 api（Linux，Darwin 等）提供友好的绑定。此文是基于 riscv64 指令的示例）
* [Rust 和 F# 语法比较（Rust for Fsharpers and F# for Rustaceans）](https://github.com/Dhghomon/rust-fsharp)
* [使用 Rust 创建一个 Deno 插件](https://alexandrempsantos.com/deno/creating-a-deno-plugin/)（译注：从零开始的教程，看起来应用前景不错）
* [如何在 Rust 开发中使用 Firebird 数据库](https://itnext.io/firebird-rust-92e9043261cc)
* [Rust 中的交互/响应式（Reactive）UI 组件](https://dev.to/seanwatters/reactive-ui-components-in-rust-290b)（译注：使用 Rust 和 WebAssembly 构建反应式用户界面）
* [Redis Streams in Action（2）- 使用 Rust 处理 Twitter 数据流 API)](https://dev.to/azure/redis-streams-in-action-part-2-rust-app-to-consume-from-the-twitter-streaming-api-1ji4)
* [如何使用 Rust 和 WebAssembly 开发插件](https://devblog.arcana.rs/how-to-make-plugins-system-with-rust-and-webassembly)
* [使用 Planck ECS 库开发 ECS](https://jojolepro.com/blog/2021-06-01_getting_started_with_ecs/)（译注：ECS：Entity-Component-System。planck_ecs 是 Rust 实现的 ECS 框架）
* [为 REST APIs 设计 Rust 绑定](https://plume.benboeckel.net/~/JustAnotherBlog/designing-rust-bindings-for-rest-ap-is)
* [使用 Rust+WASM 开发基于 WebRTC 的视频聊天教程](https://charles-schleich.medium.com/webrtc-video-chat-tutorial-using-rust-wasm-fa340f7aeef9)
* [中文] [Rust 中，对网址进行异步快照，并添加水印效果的实践](https://blog.budshome.com/budshome/rust-zhong-,dui-wang-zhi-jin-xing-yi-bu-kuai-zhao-,bing-qie-tian-jia-shui-yin-xiao-guo-de-shi-jian)
* [视频] [Rust 实现的 firehose - 给工作量繁重的 C++ 开发人员](https://youtu.be/IPmRDS0OSxM)

### 其它
* [Rust 新书：Rust for Rustaceans - Jon Gjengset 著](https://www.reddit.com/r/rust/comments/nq3pxh/new_rust_book_rust_for_rustaceans_by_jon_gjengset/)
* [只想表达对你的感谢](https://www.reddit.com/r/rust/comments/nnioxj/just_to_say_thank_you/)

# 周最佳 crate

本周最佳 crate 是 [rust-codegen-gcc](https://github.com/antoyo/rustc_codegen_gcc)，用于替换以 GCC 为目标的基于 LLVM 的 Rust 编译器后端。

谢谢 [Josh Triplett](https://users.rust-lang.org/t/crate-of-the-week/2704/920) 的提议。

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

* [Backroll-rs 期待贡献者](https://www.reddit.com/r/rust/comments/npnl1p/help_wanted_with_backrollrs_new_networking_library/)（译注：backroll 是 Rust 实现的异步 GGPO，目前代码库为 C++ 代码的直接移植）

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Rust 核心更新

[255 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-05-24..2021-05-31

## Rust 编译器性能

繁忙的一周，由于性能回退，通过几个 PRs 进行了修复。但总体来说，是积极的一周。

验测工作是由 **@simulacrum**完成的。修正范围：[cdbe288..1160cf8](https://perf.rust-lang.org/?start=cdbe2888979bb8797b05f0d58a6f6e60753983d2&end=1160cf864f2a0014e3442367e1b96496bfbeadf4&absolute=false&stat=instructions%3Au)

[此处可查阅完整报告](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-06-01.md).

## 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

* [RFC: 2021 版次](https://github.com/rust-lang/rfcs/pull/3085)

## 新的 RFCs

* [切换 travis 为 github actions](https://github.com/rust-lang/rfcs/pull/3136)（译注：项目的持续集成服务方面）

# 近期活动

### 线上

* [June 8, 2021, Seattle, WA, US - Monthly meetup - Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksryccjblb/)
* [June 10, 2021, Berlin, DE - Rust Hack and Learn - Berline.rs](https://berline.rs/)
* [June 16, 2021, Vancouver, BC, US - Rust in Mozilla's Data Platform - Vancouver Rust](https://www.meetup.com/Vancouver-Rust/events/fqpkjsyccjbvb/)
* [June 17, 2021, Denver, CO, US - Learning Rust as a Python/Javascript developer by Juhis - Rust Denver](https://www.meetup.com/Rust-Boulder-Denver/events/277575285/)

### 北美

* [June 9, 2021, Atlanta, GA, US - 和 Rustaceans 一起畅饮啤酒 - Rust Atlanta](https://www.meetup.com/Rust-ATL/events/qxqdgryccjbmb/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust 招聘信息

**TrueLayer**

* [Rust Backend Engineer (London, UK)](https://apply.workable.com/truelayer/j/262DB83659/)

**Ockam**

* [Architect - Rust Library Design (Remote)](https://www.ockam.io/team/Architect-Rust-Library-Design/53838c2d-1e48-5cec-8bb4-8fa8420e6171)
* [Applied Cryptographer - Rust (Remote)](https://www.ockam.io/team/Applied-Cryptographer-Rust/61e07e82-0589-51de-b250-42dbceb31c3c)

**Tweede golf**

* [Lead Developer Embedded Rust (Nijmegen, NL)](https://tweedegolf.nl/vacatures/2/lead-developer-embedded-rust)

**Dedalus Healthcare**

* [Medical Visualization Software Engineer (Remote, EU timezone)](https://www.karriere.at/jobs/5820070)

**Yat Labs**

* [Senior Rust Developer (Remote, EU timezone)](https://www.arbeitnow.com/view/senior-rust-developer-tari-71761)

**Ubisoft**

* [Software Engineer - Machine Learning (Remote)](https://jobs.smartrecruiters.com/Ubisoft2/743999750187882-software-engineer-machine-learning-f-h-nb)

**NZXT**

* [Senior Software Engineer for CAM (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=259)
* [Senior Software Engineer for Streaming Software (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=317)

**Parity**

* [Junior/Senior Rust Solution Engineer - Substrate (Remote)](https://grnh.se/b61620583us)
* [Multiple Rust / Blockchain Engineering Positions Available](https://parity.io/jobs)

**Kraken**

* [Several Rust Engineering Positions Available](https://jobs.lever.co/kraken?team=Engineering)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

# 本周引语

好吧，如你所愿。让我们全力以赴：

> 最近，我完成了我的 Ph.D（博士学位）。在此之前的模拟器开发中，我用 4 种不同的编程语言开发了 5 个不同版本。最后一个版本，是完全用安全的 Rust 语言实现的。其之所以能够正常工作，部分原因是 Rust 对“安全”的强有力保障。因为我能够利用 Rust 将通常的运行时错误，转化为编译时错误。所以，我能够捕获错误。而之前使用的开发语言中，这些错误通常需要几天或几周的调试，才能得到相对简单的更正。\[...\] 所以，再次感谢大家！

– [Cem Karan 发表于 rust-internals](https://internals.rust-lang.org/t/ot-thank-you-to-everyone-that-has-made-rust-possible/14777)

谢谢 [Josh Triplett](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1053) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
