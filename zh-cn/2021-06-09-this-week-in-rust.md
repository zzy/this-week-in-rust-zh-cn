# Rust 官方周报 394 期（2021-06-09）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。
> 
> 关于周报中的资源链接，已经有中文资源的，替换为中文资源链接（中文资源中，均附有原文链接）。另外，对于部分周报文章，附有阅读和简单了解后的译注，但并非全部。如果你阅读了文章，有更适合的见解，请联系、PR，或者直接参与项目 [github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)。

大家好，欢迎查阅第 394 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

# Rust 社区更新

### 官方
* [Rustup 发布版本 1.24.3](https://blog.rust-lang.org/2021/06/08/Rustup-1.24.3.html)

### 简讯
* [Rust OS 开发月报（2021 年 5 月）](https://rust-osdev.com/this-month/2021-05/)

### 项目/工具更新
* [Filecoin Forest 更新信息](https://medium.com/chainsafe-systems/back-into-the-forest-983a4344ffe9)（译注：Filecoin 是一个开源的云存储市场、协议和加密货币。Forest 是用 Rust 编写的 Filecoin 的实现，采用模块化方法来分两部分构建完整的 Filecoin 节点）
* [Mina Protocol 更新信息](https://medium.com/chainsafe-systems/realizing-the-mina-vision-in-rust-453f6f522205)（译注：Mina Protocol 主打轻量级的协议，前身为 Coda Protocol，是基于零知识证明 zkSNARKs 的轻量级区块链证明协议。其可以将区块链封装在一个单一的、可验证的、轻量级的协议中，大幅压缩区块链大小）
* [rust-analyzer 更新日志 #80](https://rust-analyzer.github.io/thisweek/2021/06/07/changelog-80.html)
* [IntelliJ Rust 更新日志 #148](https://intellij-rust.github.io/2021/06/07/changelog-148.html)
* [Android 平台中的 Rust/C++ 交互](https://security.googleblog.com/2021/06/rustc-interop-in-android-platform.html)
* [Rocket v0.5 发布候选版本（Candidate）](https://rocket.rs/v0.5-rc/news/2021-06-09-version-0.5-rc.1/)
* [TensorBase 周报 6 期](https://tensorbase.io/thisweek/2021-06-09-tw_6/)
* [Dotenv-linter v3.1.0：关键升级概览](https://dotenv-linter.github.io/#/whats_new/v310)
* [AWS SDK Rust：增加了 9 个新的服务](https://github.com/awslabs/aws-sdk-rust/releases/tag/v0.0.7-alpha)

### 观测/思考
* [Rust 类型系统中未开发的潜能（untapped potential）](https://www.jakobmeier.ch/blogging/Untapped-Rust.html)
* [地道的（idiomatic）Rust？实现二分法检索（Binary Search）- 第二部分](https://shane-o.dev/blog/binary-search-rust-part-2)
* [为 REST APIs 设计 Rust 绑定](https://plume.benboeckel.net/~/JustAnotherBlog/designing-rust-bindings-for-rest-ap-is)（译注：上期周报已经发过）
* [Rust 中实现零开销（zero-cost）抽象](https://medium.com/ingeniouslysimple/rust-zero-cost-abstraction-in-action-9e4e2f8bf5a)
* [将雷神之锤（Quake）3 迁移到 Rust](https://immunant.com/blog/2020/01/quake3/)（译注：迁移 Rust 后，游戏效果图如下所示：）
![Rust 雷神之锤 3](https://blog.budshome.com/static/articles/1623396158.gif)
* [基于 Solana 进行 Rust 编程第一印象](https://brson.github.io/2021/06/08/rust-on-solana)（译注：Solana 是全新的区块链架构。高性能、无须许可。该体系结构在千兆网络上，支持每秒 71 万个事务处理）
* [基于配对的加密优化：Rust 中的 Montgomery 算法](https://research.nccgroup.com/2021/06/09/optimizing-pairing-based-cryptography-montgomery-arithmetic-in-rust/)
* [我的“第二杯” Rust](https://blog.frankel.ch/start-rust/2/)
* [云中之鹅（A Goose In The Clouds）：大规模负载测试](https://www.tag1consulting.com/blog/goose-clouds-load-testing-scale)（译注：莎翁笔下的鹅，多表示蠢笨。非宙斯变成的那个天鹅（swan））
* [以“Java 教程（The Java Tutorials）”的方式学习 Rust](https://rust-java-tutorials.netlify.app/blog/)（译注：主要是关于 2 个语言的 OOP、继承、多态，以及 trait 的类比学习）
* [Rust 中的行为继承（behavior inheritance）](https://abadcafe.wordpress.com/2021/01/08/behavior-inheritance-in-rust/)（译注：Rust 中的 trait，可以提供默认的实现，但不能提供其实现可以处理的数据。本文即是以类 P-Impl 模式的处理方式）
* [音频] [Rust 中的构建：Ralf Jung on GhostCell and working as a PL researcher](https://anchor.fm/building-with-rust/episodes/Building-with-Rust-Ralf-Jung-on-GhostCell-and-Working-as-a-PL-Researcher-e12auje)

### Rust 演练
* [Rust 派生宏（derive macro）开发指南](https://github.com/imbolc/rust-derive-macro-guide)
* [从零开始，使用 Rust 开发镜头校准模块：1/3](https://www.tangramvision.com/blog/calibration-from-scratch-using-rust-part-1-of-3)（译注：校准理论）
* [从零开始，使用 Rust 开发镜头校准模块：2/3](https://www.tangramvision.com/blog/calibration-from-scratch-using-rust-part-2-of-3)（译注：算法、原理，以及路线图）
* [从零开始，使用 Rust 开发镜头校准模块：3/3](https://www.tangramvision.com/blog/calibration-from-scratch-using-rust-part-3-of-3)（译注：编码实现，以及结果测试）
* [从 JavaScript 的视觉看待 Rust](https://blogs.harvard.edu/kapolos/rust-from-a-javascript-perspective/)
* [WASI 的 !#[no_std]，其复杂超出我的想象](https://dev.to/thepuzzlemaker/nostd-with-wasi-is-more-complicated-than-i-thought-it-would-be-14j7)
* [我对 Rust 中的所有权和内存模型豁然开朗](https://deavid.wordpress.com/2021/06/06/rust-what-made-it-click-for-me-ownership-memory-internals/)
* [使用 Rust 编写一个 NPM 包](https://popcornpaws.medium.com/creating-an-npm-package-written-in-rust-ce02f7c55458)
* [起床时间到：让 nRF52840 进入休眠状态，以及定时唤醒](https://tweedegolf.nl/blog/57/rise-and-shine-putting-the-nrf52840-to-sleep-and-waking-back-up)（译注：Rust 的嵌入式开发）
* [Rust 中的迭代器（iterator）真的很有用](https://blog.knoldus.com/iterator-producing-iterator-in-rust-is-really-helpful/)
* [使用图像缓存和 Buildkit 加速 Rust CI](https://blog.erebe.dev/blog/speed-up-your-ci-with-buildkit/)
* [中文] [系列] [Rust 和 Wasm 的融合，使用 yew 构建 WebAssembly 标准的 web 前端（1）- 起步及 crate 选择](https://blog.budshome.com/budshome/rust-he-wasm-de-rong-he-,shi-yong-yew-gou-jian-webassembly-biao-zhun-de-web-qian-duan-(1)--qi-bu-ji-crate-xuan-ze)
* [中文] [系列] [Rust 和 Wasm 的融合，使用 yew 构建 WebAssembly 标准的 web 前端（2）- 组件和路由](https://blog.budshome.com/budshome/rust-he-wasm-de-rong-he-,shi-yong-yew-gou-jian-webassembly-biao-zhun-de-web-qian-duan-(2)--zu-jian-he-lu-you)
* [视频] [Rust 初学者 5 - 元组（Tuples）](https://youtu.be/gZMet9Vi7_A)

### 研讨/论文
* [文集] [Rust 自动验证工具（2021）](https://alastairreid.github.io/automatic-rust-verification-tools-2021/)（译注：2021 年 5 月召开的 Rust 验证工具研讨会的成果集，详见 [Rust 官方周报 390 期（2021-05-12）](https://blog.budshome.com/budshome/rust-guan-fang-zhou-bao-390-qi-(2021-05-12))研讨会部分）

### 其它
* [QUIC v1 版本已在 Cloudflare 提供](https://blog.cloudflare.com/quic-version-1-is-live-on-cloudflare/)
* [最“专业”的 crate 有哪些？](https://www.reddit.com/r/rust/comments/nsvyxq/what_are_the_most_professional_crates/)
* [被低估的（under-rated），但你特别喜欢的 Rust crate 有哪些？为什么？](https://www.reddit.com/r/rust/comments/nuq1ix/whats_your_favourite_underrated_rust_crate_and_why/)
* [今天我高中毕业，选择 Rust 作为我的编程语言](https://www.reddit.com/r/rust/comments/nrin1u/its_not_much_but_i_graduated_from_middleschool/)
* [从 Julia 到 Rust](https://miguelraz.github.io/blog/juliatorust/) 
* [如何使用 fastText 和 Rust 进行即时翻译](https://instantdomainsearch.com/engineering/how-to-use-fasttext-for-instant-translations)

# 周最佳 crate

本周最佳 crate 是 [cargo-sort](https://github.com/DevinR528/cargo-sort)，cargo 子命令，用于对 `Cargo.toml` 的依赖项和工作空间（workspace）的包成员进行排序。

谢谢 [jplatte](https://users.rust-lang.org/t/crate-of-the-week/2704/921) 的提议。

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

* [Ruma 有几个问题“需要帮忙”](https://github.com/ruma/ruma/labels/help%20wanted)
* [Cargo 有几个问题“需要帮忙”](https://github.com/rust-lang/cargo/labels/E-help-wanted)

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Rust 核心更新

[267 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-05-31..2021-06-07

## Rust 编译器性能

一些改进，以及一些回归。本周没有大的变化。

验测工作是由 **@simulacrum**完成的。修正范围：[1160cf..a50d721](https://perf.rust-lang.org/?start=1160cf864f2a0014e3442367e1b96496bfbeadf4&end=a50d72158e08e02cfc051b863017bdbd2c45b637&absolute=false&stat=instructions%3Au)

[此处可查阅完整报告](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-06-08.md).

## 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

*无*

## 新的 RFCs

* [RFC：let-else 语句](https://github.com/rust-lang/rfcs/pull/3137)

# 近期活动

### 线上

* [June 15, 2021, Washington, DC, US - In-kernel, fast-path packet processing with AF_XDP - Rust DC](https://www.meetup.com/RustDC/events/vdhxgsyccjbtb)
* [June 16, 2021, Vancouver, BC, CA - Rust in Mozilla's Data Platform - Vancouver Rust](https://www.meetup.com/Vancouver-Rust/events/fqpkjsyccjbvb/)
* [June 17, 2021, Denver, CO, US - Learning Rust as a Python/Javascript developer by Juhis - Rust Denver](https://www.meetup.com/Rust-Boulder-Denver/events/277575285/)
* [June 18, 2021, Online - Learn Rust Fundamentals | Rust 101 - KubeDaily](https://www.youtube.com/watch?v=DIxjk0HTx5U)
* [June 29. 2021, Dallas, TX, US - Last Tuesday - Dallas Rust](https://www.meetup.com/Dallas-Rust/events/jqxqwryccjbmc/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust 招聘信息

**Tweede golf**

* [Lead Developer Embedded Rust (Nijmegen, NL)](https://tweedegolf.nl/vacatures/2/lead-developer-embedded-rust)

**Eniride**

* [Rust Developer Tech, Autonomous Transport(Stockholm/Gothenburg, SE)](https://www.einride.tech/careers/1186875-rust-developer)

**Field33**

* [Senior Software Engineer - Backend (Java/Rust)(Berlin, DE)](https://arbeitnow.com/view/senior-software-engineer-backend-javarust-fxm-atlanticlabs-154911)

**Snapview**

* [(Senior) Rust Backend Engineer (Remote)](https://snapview.jobs.personio.de/job/381815)

**Apollo**

* [Infrastructure Systems Engineer - Rust (Remote)](https://jobs.lever.co/apollographql/d7c1d4f1-f2ad-41b0-a43b-b9f70d934ec3)

**NZXT**

* [Senior Software Engineer for CAM (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=259)
* [Senior Software Engineer for Streaming Software (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=317)

**Kollider**

* [Junior Backend Engineer (Remote)](https://kollider.homerun.co/junior-backend-engineer/en)
* [Senior Backend Engineer (Remote)](https://kollider.homerun.co/senior-backend-engineer/en)
* [DevOps Engineer (Remote)](https://kollider.homerun.co/devops-engineer/en)

**Estuary**

* [Multiple Rust Positions Available](https://estuary.dev/careers)

**Kraken**

* [Several Rust Engineering Positions Available](https://jobs.lever.co/kraken?team=Engineering)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

# 本周引语

> 软件工程中技术的权衡取舍，随着时间的推移而改变，理想的解决方案同样如此。大约 40 年前，当第一个 C 语言标准被研究人员核定的时候，他们的能力，并不比今天这些研究 Rust 的人员逊色。C 语言的设计及其未定义的特性，在当时的背景下，可能比现在看起来更有意义。同样，Rust 目前做出的选择，在未来的数年后，或许不会像今天这般有意义。

– [Simonas 发表于 rust-internals](https://users.rust-lang.org/t/why-deference-maybeuninit-unint-as-mut-ptr-is-safe/60344/19)

谢谢 [Kill The Mule](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1055) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
