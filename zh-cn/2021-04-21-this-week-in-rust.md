# Rust 官方周报 387 期（2021-04-21）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。 

大家好，欢迎查阅第 387 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

# Rust 社区更新

本周无论文或研究探讨。

### 官方
* [内部] [Rust 编译器（Compiler）团队 4 月份计划 - Rust Compiler April Steering Cycle](https://blog.budshome.com/budshome/rust-bian-yi-qi-(compiler)tuan-dui-4-yue-fen-ji-hua---rust-compiler-april-steering-cycle)
* [内部] [Rust 语言团队 4 月份更新简报](https://blog.rust-lang.org/inside-rust/2021/04/17/lang-team-apr-update.html)
* [内部] [Jacob Hoffman-Andrews 加入 Rustdoc 团队](https://blog.budshome.com/budshome/jacob-hoffman-andrews-jia-ru-rustdoc-tuan-dui)
* [基金会] [成员介绍：Jane Lusby](https://foundation.rust-lang.org/posts/2021-04-15-introducing-jane-lusby/)（译注：项目主管，协作团队）
* [基金会] [成员介绍：Shane Miller](https://foundation.rust-lang.org/posts/2021-04-15-introducing-shane-miller/)（译注：董事成员，亚马逊）

### 简讯

### 项目/工具更新
* [rust-analyzer 更新日志 #73](https://rust-analyzer.github.io/thisweek/2021/04/19/changelog-73.html)
* [Knurling-rs 更新日志 #23](https://ferrous-systems.com/blog/knurling-changelog-23/)（译注：Knurling-rs 主要致力于嵌入式 Rust 体验）
* [Ballista 周报 #11](https://ballistacompute.org/thisweek/2021/04/18/this-week-in-ballista-11/)（译注：Ballista 项目是 Rust 开发的类似 Spark 的分布式计算平台，目前已被捐赠给了 Apache Arrow 项目组。笔者已经在使用中。其还支持  Python、C++，以及 Java 等语言，且不用为序列化付出额外开销代价）
* [欢迎 Alice Ryhl 成为第一个受薪的 Tokio 项目贡献者](https://tokio.rs/blog/2021-04-welcome-alice)（译注：通过 github 赞助）
* [Zellij：Rust 实现的终端复用器，已经发布 beta 版本](https://zellij.dev/news/beta/)（译注：类似 `tmux` 或者 `gnu screen`）
* [faux：结构体模拟（mocking）库 - v0.1 发布](https://nrxus.github.io/faux/blog/landing-v-0-1.html)（译注：允许模拟结构体的方法进行测试，而不会使代码复杂化或污染代码）
* [Otter - 棋盘类游戏服务器](https://diziet.dreamwidth.org/8121.html)，主要使用 [Rust 开发](https://www.chiark.greenend.org.uk/~ianmdlvl/otter/docs/build.html)
* [音频] [Rust 1.50 和 1.51 的新特性](https://rustacean-station.org/episode/033-rust-1.50-1.51/)

### 观测/思考
* [实际上，“红色”函数和“蓝色”函数都是合理的](https://blainehansen.me/post/red-blue-functions-are-actually-good/)（译注：红色/蓝色函数象征同步/异步函数，函数的`颜色（colored）`源自 JavaScript，比喻 JavaScript 和其它语言中，同步函数和异步函数那些令人痛苦的不匹配难题。本文是对上期文章《[Rust 语言中，让异步函数和同步函数匹配，不是什么大问题](https://blog.budshome.com/budshome/rust-guan-fang-zhou-bao-386-qi-(2021-04-14))》的回应）
* [Rust 赋能 Temporal 的新核心 SDK](https://docs.temporal.io/blog/why-rust-powers-core-sdk/)
* [Rust 中的数独（sudoku）求解优化](https://www.simonclark.dev/2020/08/10/optimizing-sudoku-solver.html)（译注：文章不长，值得一读）
* [我的 Rust 语言理解之旅](https://daveshawley.medium.com/my-journey-to-understand-rust-lang-28e4cf808b12)
* [如何在 Rust 中实现 `/dev/printerfact`](https://christine.website/blog/dev-printerfact-2021-04-17)
* [为什么使用 Rust 重新实现 fnm](https://gal.hagever.com/posts/why-fnm-was-rewritten-in-rust/)（译注：fnm 是系统应用，包括文件系统、网络，以及用户输入等）
* [在 AWS Lambda 之上，使用 Rust 运行 GraphQL 服务](https://dev.to/dbanty/running-graphql-on-lambda-with-rust-1lak)
* [运行时（Runtime）类型别名检测](https://myrrlyn.net/blog/bitvec/alias-detection)（译注：指针值（pointer-value）的类型别名分析）
* [`box` 里面隐藏着什么？](https://fasterthanli.me/articles/whats-in-the-box)（译注：指 `Box<dyn Error>` 或 `Box<T>` 的 `box`）
* [视频] [嵌入式 Rust 生态概览](https://youtu.be/vLYit_HHPaY)（译注：值得一看）

### Rust 演练
* [午夜忏悔（Late Night Confessions） — 使用 Rust、Rocket、Diese，以及 Askama 进行站点构建（1）](https://medium.com/perimeterx/late-night-confessions-building-a-website-using-rust-rocket-diesel-and-askama-part-1-aeccade43252)（译注：站点名本无需翻译，但这个站名象电影名字，不由得手痒 ;-)）
* [Rust 之标准库 `trait` 之旅](https://github.com/pretzelhammer/rust-blog/blob/master/posts/tour-of-rusts-standard-library-traits.md)（译注：好文章，适合精读）
* [Rust 学习 #3：crates.io 及发布新包](https://hamatti.org/posts/learning-rust-3-crates-io-publishing-your-package/)
* [Rust 技术栈中，使用 Nakama 制作多人在线游戏](https://heroiclabs.com/blog/tutorials/rust-fishgame/)
* [使用 React 和 WebAssembly 创建明亮的砌砖画廊（Sleek Masonry Gallery）](https://dev.to/rvanderlaan/creating-a-sleek-masonry-gallery-with-react-and-webassembly-17p2)
* [GPIO 之战：类型状态骤升后的宏保护（2）](https://www.ecorax.net/macro-bunker-2/)
* [在嵌入式 Rust 中使用 `std`](https://timmmm.github.io/std-embedded-rust/index.html)
* [Rust 和 TUI：在 Rust 中 构建命令行（command-line）界面](https://blog.logrocket.com/rust-and-tui-building-a-command-line-interface-in-rust/)（译注：`tui` 类似 JavaScript 的界面库 `blessed-contrib` 或 Go 的界面库 `termui`）
* [Rust：Serde：处理无类型的 JSON 数据](https://youtu.be/NwYY00paiH0)
* [系列] [Rust 中编写 NES 模拟器](https://bugzmanov.github.io/nes_ebook/index.html)

### 其它
* [rustc、iOS，以及 M1](https://fnordig.de/2021/04/16/rustc-ios-and-an-m1/)
* [微软预发布 Rust For Windows](https://www.tectalk.co/microsoft-previews-rust-for-windows/)（译注：简单说，支持 Rust 象 C 一样通过元数据访问 Windows API）
* [Rustls 已为广泛使用做好准备](https://www.abetterinternet.org/post/preparing-rustls-for-wider-adoption/)
* [错误还在吗（Are We Yeet Yet）？](https://areweyeetyet.rs/)（译注：以**有些“火气”的语气**说出：错误还在吗？此站点是错误追踪类）
* [使用 BL602 IoT SDK 运行 Rust RISC-V 固件](https://lupyuen.github.io/articles/rust)
* [视频] [斯坦福大学研讨会 - 新机器的灵魂：重新思考计算机](https://youtu.be/vvZA9n3e5pc)

# 周最佳 crate

本周最佳 crate 是 [deltoid](https://github.com/jjpe/deltoid)，用于增量压缩 Rust 数据结构的 crate。

谢谢 [Joey Ezechiëls](https://users.rust-lang.org/t/crate-of-the-week/2704/904) 的提议。

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Rust 核心更新

[292 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-04-12..2021-04-19

## Rust 编译器性能

又是一个安静的一周，编译器的性能变化很小。 

验测工作是由 **@rylev** 完成的。修正范围：[5258a74..6df26f](https://perf.rust-lang.org/?start=5258a74c887f8ae14717e1f98b652b470877ce4e&end=6df26f897cffb2d86880544bb451c6b5f8509b2d&absolute=false&stat=instructions%3Au)

## 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

* [try_trait_v2：`?` 脱糖（desugaring）语法的新设计](https://github.com/rust-lang/rfcs/pull/3058)

## 新的 RFCs

*无。*

# 近期活动

### 线上活动
* [April 21, 温哥华, BC, CA - Rust 的研讨/Hack/闲逛 之夜 - Vancouver Rust](https://www.meetup.com/Vancouver-Rust/events/npqfbsyccgbcc/)
* [April 27, 柏林, DE - Rust 和 Tell - Rust Berlin](https://www.meetup.com/Rust-Berlin/events/277590271)
* [April 27, 伦敦, UK - LDN Virtual Talks Apr 2021 - Red Badger Takeover - Rust London User Group](https://www.meetup.com/Rust-London-User-Group/events/277520645/)
* [April 27, Dallas, TX, US - Last Tuesday - Dallas Rust](https://www.meetup.com/Dallas-Rust/events/jqxqwryccgbkc/)
* [April 28, Online - Ockam Open Source Community Call - Live coding walkthrough of building end-to-end encrypted communication in Rust](https://github.com/ockam-network/ockam/discussions/1303)
* [May 4, Buffalo, NY, US - Buffalo Rust User Group, Tues May 4th - Buffalo Rust Meetup](https://www.meetup.com/Buffalo-Rust-Meetup/events/277402612/)

### 欧洲
* [April 21, Moscow, RU - Monthly Meetup - Rust Moscow](https://www.meetup.com/ru-RU/Rust-%D0%B2-%D0%9C%D0%BE%D1%81%D0%BA%D0%B2%D0%B5/events/277259838/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust 招聘信息

**Grover GmbH**

* [**柏林或者远程** - Software Engineer - Risk & Data, Rust & Python](https://grnh.se/15fcbda73us)

**Massa Labs**

* [**远程** - Rust Blockchain Developer](https://massa.network/#jobs)

**Instaclustr**

* [Software Engineer (Canberra, AU)](https://www.seek.com.au/job/52021829)

**Subspace Labs**

* [**远程** - Core Protocol Engineer](https://jobs.lever.co/subspacelabs/7f6a654b-60a8-4740-aa19-36b9f7a9e624?lever-origin=applied&lever-source%5B%5D=Twitter)

**Paige**

* [**远程/欧洲** - Senior Software Engineer, Visualization](https://boards.greenhouse.io/paige/jobs/5217029002)

**Luminovo**

* [**远程，中欧夏令时区** - (Senior) Software Engineer - Rust](https://luminovo.jobs.personio.de/job/357453)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

# 本周引语

> 我们认为：Rust 现在已经为加入 C 做好了准备，成为实现 \[Linux\] 内核的实用语言。Rust 可以帮助我们减少特权代码中潜在的 bug，减少安全漏洞的数量。同时，Rust 可以很好地处理核心内核，并保持其性能特色。

– [Wedson Almeida Filho 发表于 Google 安全博客](https://security.googleblog.com/2021/04/rust-in-linux-kernel.html)

谢谢 [Jacob Pratt](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1040) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
