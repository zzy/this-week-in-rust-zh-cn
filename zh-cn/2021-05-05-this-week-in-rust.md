# Rust 官方周报 389 期（2021-05-05）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。

大家好，欢迎查阅第 389 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

# Rust 社区更新

### 官方
* [Rustup 1.24.1 已官宣发布，及其新特性详述](https://blog.budshome.com/budshome/rustup-1.24.1-yi-guan-xuan-fa-bu-,ji-qi-xin-te-xing-xiang-shu)
* [内部] [Rustup 1.24.0 发布后的 bug 事件报告（2021-04-27）](https://blog.rust-lang.org/inside-rust/2021/04/28/rustup-1.24.0-incident-report.html)（译注：指有用户升级到 rustup 1.24.0 之后，用户无法运行 `rustfmt` 和 `cargo fmt`。因此，官方将版本恢复为 1.23.1）
* [内部] [Rust 1.52.0 稳定版预发布测试中，关键新特性一瞥](https://blog.budshome.com/budshome/rust-1.52.0-wen-ding-ban-yu-fa-bu-ce-shi-zhong-,guan-jian-xin-te-xing-yi-pie)
* [内部] [核心团队 2021 年 5 月报告](https://blog.rust-lang.org/inside-rust/2021/05/04/core-team-update.html)（译注：指核心团队关于 2021 年路线图、团队章程，以及对 crate 的审核策略）
* [基金会] [Q12021 Rust 基金会成员更新](https://foundation.rust-lang.org/posts/2021-04-29-membership-update/)（译注：指 [Facebook 成为 Rust 基金会新的白金会员](https://blog.budshome.com/budshome/rust-ji-jin-hui-ying-lai-xin-de-bai-jin-hui-yuan-:facebook)；Zama、Tag1Consulting、CleverCloud 成为 Rust 基金会新的白银会员）

### 简讯
* [Rust 操作系统开发（OSDev）月报（2021 年 4 月）](https://rust-osdev.com/this-month/2021-04/)

### 项目/工具更新
* [回顾 2021 年已逝的三分之一](https://isomorphicdb.io/blog/2021/05/05/One-Third-of-2021/)（译注：IsomorphicDB 是 Rust 实现的兼容 PostgreSQL 的分布式数据库的核心，此文是作者对其 2021 年前 4 个月的开发回顾）
* [TensorBase 周报 1 期](https://tensorbase.io/thisweek/2021-05-01-tw_1/)（译注：TensorBase 是基于 Rust 的现代化开源数据仓库，详细中文介绍见页面内的链接。也可以直接在张老师整理的《[Rust语言开源杂志（2021）](https://rustmagazine.github.io/rust_magazine_2021/chapter_4/tensorbase.html)》中查阅）
* [gfx/wgpu 0.8 发布](https://gfx-rs.github.io/2021/04/30/release-0.8.html)（译注：原生（native）WebGPU）
* [Flott（Rust 中的运动控制工具包）上月回顾 - 2021 年 5 月](https://flott-motion.org/news/last-month-in-flott-may-2021/)（译注：[Rust 官方周报 385 期](https://blog.budshome.com/budshome/rust-guan-fang-zhou-bao-385-qi-(2021-04-07))中介绍过的包，前景很不错，但关注人数还不多，github 星星很少）
* [rust-analyzer 更新日志 #75](https://rust-analyzer.github.io/thisweek/2021/05/03/changelog-75.html)
* [GCC Rust 月报 #5 2021 年 4 月](https://thephilbert.io/2021/05/03/gcc-rust-monthly-report-5-april-2021/)
* [RustCrypto 发布公告（`aead`、`cipher`、`crypto`、`elliptic-curve`，以及 `ecdsa` 等等）](https://users.rust-lang.org/t/rustcrypto-release-announcements/59149)（译注：RustCrypto 是纯粹 Rust 实现加密算法的团队）

### 观测/思考
* [Rust 是如何让 Rayon 的数据并行（parallelism）变的神奇的？](https://developers.redhat.com/blog/2021/04/30/how-rust-makes-rayons-data-parallelism-magical/)（译注：Rayon 是 Rust 实现的无数据竞争（data race）的数据并行库，笔者的项目中用到此包蛮多频次。实例请参阅[来自于 rust-cookbook 的 rayon 数据并行处理](https://rust-guide.budshome.com/8-concurrency/8.2-parallel.html)）
* [使用 Rust 进行艺术创作（Making Generative Art with Rust）](https://blog.abor.dev/p/making-generative-art-with-rust)（译注：图形处理、媒体制作等，可以结合 `gfx/wgpu` 等库一起理解）
* [过程宏（Proc Macro）阐述：为我节省了大约 4000 行 Rust 代码](https://mbuffett.com/posts/incomplete-macro-walkthrough/)
* [最被低估，但非常有用的 Rust 标准库类型](https://dev.to/thepuzzlemaker/the-most-underrated-but-useful-rust-standard-library-type-59b1)
* [保持独特性；或者说，内部测试为什么让人伤脑筋](https://dev.to/ecton/guaranteed-unique-or-why-dogfooding-can-be-taxing-2gcn)
* [使用 Rust 重写伟大的软件和工具（The Great Rewriting in Rust）](https://deprogrammaticaipsum.com/the-great-rewriting-in-rust/)（译注：作者确信 Rust 会接管 `Linux` 内核开发，重写 `LaTeX`，以及蓝牙等）
* [关于 async Rust 和使用 `!Send` 类型的经历](https://procmarco.netlify.app/blog/2021-05-04-a-story-about-async-rust-and-using-send-types/)
* [以 Rust 编译器（Compilers）为师](https://ferrous-systems.com/blog/compilers-as-teachers/)
* [使用 Rust 进行艺术创作（Making Generative Art with Rust）：Alexis André 访谈](https://blog.abor.dev/p/making-generative-art-with-rust)
* [站在巨人的肩膀上：TensorFlow 和 Rust 的组合](https://www.crowdstrike.com/blog/how-crowdstrike-combines-tensorflow-and-rust-for-performance/)
* [让一切皆可迭代 - 在 Rest API 中进行迭代分页](https://0x709394.me/Let's-make%20everything%20iterable)
* [视频] [Niko Matsakis 访谈，Rust 语言团队的联席领导](https://youtu.be/alD0l_8W9Sc)

### Rust 演练
* [Rust 生态中的 gRPC 介绍](https://dev.to/rkudryashov/introduction-to-grpc-in-rust-4dgg)
* [Pinephone 中的 I2C](https://dev.to/pcvonz/i-c-on-the-pinephone-5090)（译注：Pinephone 是 Manjaro 推出的预装 Linux 的智能手机）
* [午夜忏悔（Late Night Confessions） — 使用 Rust、Rocket、Diese，以及 Askama 进行站点构建（3）](https://dev.to/pxjohnny/late-night-confessions-building-a-website-using-rust-rocket-diesel-and-askama-part-3-46i9)
* [Rust 之所有权（ownership）和借用（borrow）- 和借用检查器（borrow-checker）的战斗](https://dev.to/daaitch/rust-ownership-and-borrows-fighting-the-borrow-checker-4ea3)（译注：推荐，不论老鸟新手，都会有收获）
* [在 Android 上运行 Rust](https://blog.svgames.pl/article/running-rust-on-android)（译注：笔者去年就试过，很折腾）
* [使用 GDB 和 defmt 调试嵌入式程序](https://ferrous-systems.com/blog/gdb-and-defmt/)
* [Rust 中的数据建模](https://phazer99.blogspot.com/2021/05/data-modelling-in-rust.html)
* [Rust 中的数据建模 - 续篇](https://phazer99.blogspot.com/2021/05/data-modelling-in-rust-continued.html)
* [将 Rust 代码嵌入 Java Jar，以进行分发](https://www.fluvio.io/blog/2021/05/java-client/)（译注：github 有[完整的实例](https://github.com/drrb/java-rust-example)）
* 使用 KAS GUI 开发[计数器](https://kas-gui.github.io/tutorials/counter.html)和[计算器](https://kas-gui.github.io/tutorials/calculator.html)（译注：`kas` 是受 Qt 启发的 Rust GUI 库） 
* [中文] [系列] [基于 Async Rust 构建 GraphQL 服务，使用 tide + async-graphql + mongodb（3）- 重构](https://blog.budshome.com/budshome/gou-jian-rust-yi-bu-graphql-fu-wu-:ji-yu-tide-+-async-graphql-+-mongodb(3)--zhong-gou)
* [中文] [系列] [基于 actix-web + async-graphql + rbatis + postgresql / mysql 构建异步 Rust GraphQL 服务（2）- 查询服务](https://blog.budshome.com/budshome/ji-yu-actix-web-+-async-graphql-+-rbatis-+-postgresql---mysql-gou-jian-yi-bu-rust-graphql-fu-wu-(2)---cha-xun-fu-wu)
* [视频] [Crust of Rust：调度（Dispatch）和宽指针（Fat Pointer）](https://youtu.be/xcygqF5LVmM)
* [视频] [Ockam | 开源软件（OSS）社区对话（Community Call）| 2021 年 4 月](https://www.youtube.com/watch?v=ndujK8lTTVY)

### 论文/研究探讨
* [Rust 实现的 Buer Loader 新变体（New Variant of Buer Loader）](https://www.proofpoint.com/us/blog/threat-insight/new-variant-buer-loader-written-rust)
* [在安全、稳定的 Rust 中，编写零开销（overhead-free）循环数据结构（data-structures），是否可能？](https://www.reddit.com/r/rust/comments/n420cg/is_it_possible_to_write_overheadfree_cyclic/)

### 其它
* [Rust 生态中，最不知名的贡献者和轶事](https://blog.budshome.com/budshome/rust-sheng-tai-zhong-,na-xie-zui-bu-zhi-ming-de-gong-xian-zhe-he-yi-shi)
* [Rust 基金会迎来新的白金会员：Facebook](https://blog.budshome.com/budshome/rust-ji-jin-hui-ying-lai-xin-de-bai-jin-hui-yuan-:facebook)
* [Rust 在 Facebook 的应用简史](https://engineering.fb.com/2021/04/29/developer-tools/rust/)
* [自 Rust 1.46 到 1.51，rustc 性能提升比较](https://www.reddit.com/r/rust/comments/n2lh7z/rustc_performance_improvement_from_rust_146_to_151/)
* [微软加入字节码联盟（Bytecode Alliance），以推进 `WebAssembly` - 也就是说，在浏览器中即可运行 `C/C++/Rust` 的编译代码](https://www.theregister.com/2021/04/28/microsoft_bytecode_alliance/)（译注：字节码联盟（Bytecode Alliance）由 Mozilla 携手英特尔等公司成立于 2019 年末，以扩展 `WebAssembly`）

# 周最佳 crate

本周最佳 crate 是 [display_utils](https://docs.rs/display_utils)，具备可`展示`的结构体的库，让字符串操作更容易。

> 译注：使用蛮方便，笔者已经使用过。可以通过一个简单示例看看带来的方便，比如此官方示例 `for` 循环代码：
> ``` rust
> for (i, item) in list.iter().enumerate() {
>     if i == list.len() - 1 {
>         println!("{}", item);
>     } else {
>         print!("{} - ", item);
>     }
> }
> ```
> 使用 `display_utils` 库，可以简化为一行：
> ``` rust
> println!("{}", display_utils::join(list, " - "));
> ```

谢谢 [kangalioo](https://users.rust-lang.org/t/crate-of-the-week/2704/908) 的提议。

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

* [paru - Add -P --stats](https://github.com/Morganamilo/paru/issues/357)

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Rust 核心更新

[322 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-04-26..2021-05-03

## Rust 编译器性能

安静的一周，没有显著变化。

验测工作是由 **@simulacrum** 完成的。修正范围：[537544..7a0f178](https://perf.rust-lang.org/?start=537544b1061467ee4b74ef7f552fab3d513e5caf&end=7a0f1781d04662041db5deaef89598a8edd53717&absolute=false&stat=instructions%3Au)

[此处可查阅完整报告](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-05-04.md)。

## 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

* [Target tier 策略](https://github.com/rust-lang/rfcs/pull/2803)
* [增加 const-ub RFC](https://github.com/rust-lang/rfcs/pull/3016)

## 新的 RFCs

* [RFC: 未稳定特性（Unstable Features）预览](https://github.com/rust-lang/rfcs/pull/3120)
* [Rust-lang crate 所有权（ownership）策略](https://github.com/rust-lang/rfcs/pull/3119)

# 近期活动

### 线上
* [May 6, New York, NY, US - Rust Lightning Talks - Rust NYC](https://www.meetup.com/Rust-NYC/events/277822386)
* [May 11, Seattle, WA, US - Monthly meetup - Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksrycchbpb/)
* [May 11, Saarbücken, Saarland, DE - Meetup: 11u16 (virtual) - Rust Saar](https://www.meetup.com/de-DE/Rust-Saar/events/277607432/)
* [May 12, Online - Rust Meetup May 2021 - Rust Malaysia](https://docs.google.com/forms/d/e/1FAIpQLSf_hz-ZDwYEhVmIH0uzJ0uH41aXWZ_zRDsI0XENpfkKHvh_Jg/viewform)
* [May 15 - June 7, Online - Solana Season Hackathon - Registration open now](https://twitter.com/solana/status/1387411221717176323?s=20)
* [May 17, 2021, Cardiff, UK - Rust and Cpp Cardiff :: v2.0 - Rust and C++ Cardiff](https://secure.meetup.com/register/?referrer_n=event&referrer_i=278002832&ctx=ref)
* [May 20, 2021, Online - Go vs Rust | Round table discussion](https://rustlab.it/en/rust-vs-go/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust 招聘信息

**Fiberplane**

* **远程** - [Rust Engineer](https://fiberplane.dev/careers/rust-engineer/)

**Paige**

* **远程/欧洲** - [Senior Software Engineer, Visualization](https://boards.greenhouse.io/paige/jobs/5210311002)

**Netlify**

* **远程或旧金山** - [Senior Backend Engineer (Go/Rust)](https://boards.greenhouse.io/netlify/jobs/5054144002)

**e.ventures**

* **远程/美洲** - [Rust backend engineer](https://old.reddit.com/r/rust/comments/mfstaz/official_rrust_whos_hiring_thread_for_jobseekers/gspq9v1/)

**ConsenSys**

* [Rust Software Engineer (Protocol Engineering)](https://arbeitnow.com/view/rust-software-engineer-protocol-engineering-consensys-459183)

**Spacemesh**

* **远程** - [Rust Developer](https://spacemesh.io/rust-developer/)

**DEX Labs**

* **远程** - [Senior Software Engineer – 全栈](https://dex-labs.breezy.hr/p/49c5370a8473)

**Kollider**

* **远程** - [Junior Backend Engineer](https://kollider.homerun.co/junior-backend-engineer/en)
* **远程** - [Senior Backend Engineer](https://kollider.homerun.co/senior-backend-engineer/en)
* **远程** - [DevOps Engineer](https://kollider.homerun.co/devops-engineer/en)

**Ockam**

* [Multiple Rust Engineering Positions](https://www.ockam.io/team#open-roles)

**Kraken**

* [Several Rust Engineering Positions](https://jobs.lever.co/kraken?team=Engineering)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

# 本周引语

> 使用 R 语言或 Numpy（译注：Python 语言的一个扩展程序库，支持大量的维度数组与矩阵运算）就像开运动跑车似的：你只要转动方向盘，踩油门，然后“燃烧”轮胎。而 Rust，以及其它系统语言，就像获得了一艘宇宙飞船。你可以去梦想的地方，做一些你在开运动跑车时做梦也想不到的事情。Rust 更难驾驶，但可能性似乎是无限的！由于 Rust 生态系统仍在发展中，这种感觉好像是：你的宇宙飞船的零部件，装在标有“需要某些组件”的盒子里。

– [Erik Rose 发表在 rust-users 论坛](https://users.rust-lang.org/t/rust-for-data-first-problems/58887/16)

谢谢 [Phlopsi](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1047) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
