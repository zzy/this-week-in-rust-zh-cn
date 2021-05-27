# Rust 官方周报 392 期（2021-05-26）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。
> 
> 关于周报中的资源链接，已经有中文资源的，替换为中文资源链接（中文资源中，均附有原文链接）。另外，对于部分周报文章，附有阅读和简单了解后的译注，但并非全部。如果你阅读了文章，有更适合的见解，请联系、PR，或者直接参与项目 [github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)。

大家好，欢迎查阅第 392 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

# Rust 社区更新

本周无相关官方博客、简讯，或研讨/论文。

### 项目/工具更新
* [rust-analyzer 更新日志 #78](https://rust-analyzer.github.io/thisweek/2021/05/24/changelog-78.html)
* [TensorBase 周报 4 期](https://tensorbase.io/thisweek/2021-05-26-tw_4/)（译注：TensorBase 是 Rust 实现的现代化开源数据仓库）
* [rustc_codegen_gcc 已运行 libcore 测试，并大部分通过！](https://blog.antoyo.xyz/rustc_codegen_gcc-run-core-tests)
* [Parcel 2 beta 3 发布](https://v2.parceljs.org/blog/beta3/)（译注：Parcel 是一款极速、零配置的 web 应用打包工具，其核心、transformers，以及通用工具部分是 Rust 实现的）
* [lettre 发布版本 0.10.0-rc.1](https://lettre.rs/post/lettre-0-10-0-rc-1/)（译注：实际上，笔者已经使用到了 `0.10.0-rc.3` 候选版本。lettre 是 Rust 的邮件客户端，crates.io 即在使用。0.10.x 是 1.x 版本的前奏，主要改编是将 lettre_email 合并）
* [typed-sql 发布 beta 版本！零开销（zero-cost）的 ORM，编译速度快](https://www.reddit.com/r/rust/comments/njbt9s/announcing_typedsql_beta_zerocost_orm_with_fast/)（译注：新包，基于 sqlx）
* [valuable 开发宣言，用于对象安全检查的包](https://tokio.rs/blog/2021-05-valuable)（译注：目前只是在 crates.io 有个名称占位符，话说 Rust 社区最近好多这类标题或者宣言……）

### 观测/思考
* [为什么，以及如何开发 Rust 编译器（compiler）- 系列博客 1/X：上下文（context）](https://bnjjj.medium.com/why-and-how-we-wrote-a-compiler-in-rust-blog-post-series-1-x-the-context-e2f83b10edb9)
* [Rust 中，进行 2D web 渲染](https://medium.com/lagierandlagier/2d-web-rendering-with-rust-4401cf133f31)（译注：有趣的文章，值得一读）
* [Rust 实现快速同步/搜索和空间优化（space-optimized）的复制（replication）算法，基于 gun-db 数据复制模型](https://mateusfreira.github.io/@mateusfreira-a-fast-to-sync-search-and-space-optimized-replication-algorithm-written-in-rust-the-Nun-db-data-replication-model/)
* [rustc Forking 历险记](https://jam1.re/blog/adventures-in-rustc-forking)（译注：用于任天堂的游戏开发）
* [基准线（baseline）的实现应是可预判的](https://pvk.ca/Blog/2021/05/14/baseline-implementations-should-be-predictable/)
* [对生命周期（lifetime）进行命名](https://www.possiblerust.com/pattern/naming-your-lifetimes)（译注：推荐阅读。有效地命名生命周期，有助于提高多个场景中的代码清晰度。总是用 `'a` 不是个好习惯哈）
* [rucredstash 发布，以及来自 Haskell 语言爱好者的 Rust 体验](https://psibi.in/posts/2021-05-22-credstash.html)（译注：rucredstash 是 credstash 工具的 Rust 端口，credstash 是一个 cli 工具，用于在 AWS 云中安全地管理凭据）

### Rust 演练
* [在容器中调试 Rust 程序](https://blog.erebe.dev/blog/debug-rust-aplication-inside-container/index.html)（译注：docker 中调试 Rust 代码）
* [不用 forking Clippy，编写 Rust lints 工具](https://www.trailofbits.com/post/write-rust-lints-without-forking-clippy)（译注：cargo-dylint 的介绍，其也支持 clippy）
* [使用 Zig 语言完美执行 Rust 的交叉编译（Cross-Compilation）](https://actually.fyi/posts/zig-makes-rust-cross-compilation-just-work/)
* [Rust 中，使用 eBPF 进行流量的路由配置](https://www.infinyon.com/blog/2021/05/ebpf-routing-rust/)
* [Rust 中，如何使用 to_string](https://loige.co/how-to-to-string-in-rust/)
* [使用 Ember.js 和 Tauri 构建小型的桌面应用](https://dev.to/mitchartemis/building-small-desktop-apps-with-ember-js-and-tauri-3o28)（译注：tauri 目前支持 Windows、Linux，以及 macOS 平台，但也有支持 iOS、Android 的计划）
* [从 Django 到 Rust](https://meesha.blog/2021/coming-to-rust-from-django.html)
* [Rust 中的结构体类型](https://beachape.com/blog/2021/05/25/structural-typing-in-rust/)
* [Rust 实现二分法检索（binary search）](https://shane-o.dev/blog/binary-search-rust)
* [中文] [使用 Rust 做异步数据采集的实践](https://blog.budshome.com/budshome/shi-yong-rust-zuo-yi-bu-shu-ju-cai-ji-de-shi-jian)
* [视频] [Rust 中实现无锁（Lock-Free）及无等待的模拟仿真](https://youtu.be/Bw8-vvtA-E8)

### 其它
* [Rust Web Development - 预览版（MEAP）](https://www.manning.com/books/rust-web-development)（译注：Manning 出版的书籍）
* [Fuchsia OS 中，Rust 开发的部分功能已经整合](https://www.reddit.com/r/rust/comments/nldg5c/fuchsia_os_partially_written_in_rust_has_shipped/)

# 周最佳 crate

本周最佳 crate 是 [typed-index-collections](https://github.com/zheland/typed-index-collections)，可让动态数组（vector）使用自定义类型做为索引的 crate。

谢谢 [Tim](https://users.rust-lang.org/t/crate-of-the-week/2704/913) 的提议。

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

*本周无参与邀请*。

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Rust 核心更新

[280 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-05-17..2021-05-24

## Rust 编译器性能

较安静的一周。一些 PRs 是关于性能方面的，但更改还是被合并了。此外，我们仍然有一些问题，某些基准测试有噪音。

验测工作是由 **@rylev** 完成的。修正范围：[25a277..cdbe2](https://perf.rust-lang.org/?start=25a277f03df7e44643ddfcc240d034409cb2f505&end=cdbe2888979bb8797b05f0d58a6f6e60753983d2&absolute=false&stat=instructions%3Au)

[此处可查阅完整报告](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-05-25.md)。

## 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

* [Rust 2021 版次的新 prelude（仅是 trait 版本）](https://github.com/rust-lang/rfcs/pull/3114)

## 新的 RFCs

* [用于安全/高效且动态的数组初始化的 ArrayBuilder 结构体](https://github.com/rust-lang/rfcs/pull/3131)
* [RFC: I/O 安全性](https://github.com/rust-lang/rfcs/pull/3128)
* [Cargo profile 设置选项 trim-path，用于整理绝对路径](https://github.com/rust-lang/rfcs/pull/3127)

# 近期活动

### 线上
* [May 27, 2021, London/Remote, UK - Runtime reflection, gRPC at scale, and more](https://www.meetup.com/Rust-London-User-Group/events/278045628/)
* [May 27, 2021, Montréal, QC, CN - Rust MTL: Building a Scrabble AI with the fst crate - Rust Montréal](https://www.meetup.com/Rust-Montreal/events/278011978/)
* [June 1, 2021, Dublin, IE - June Remote Meetup - Rust Dublin](https://www.meetup.com/Rust-Dublin/events/278409501/)
* [June 1, 2021, Buffalo, NY, US - Buffalo Rust User Group, First Tuesdays - Buffalo Rust Meetup](https://www.meetup.com/Buffalo-Rust-Meetup/events/jxfdjsyccjbcb/)

### 北美
* [June 9, 2021, Atlanta, GA, US - 和 Rustaceans 一起畅饮啤酒 - Rust Atlanta](https://www.meetup.com/Rust-ATL/events/qxqdgryccjbmb/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust 招聘信息

**Ockam**

* [Architect - Rust Library Design (Remote)](https://www.ockam.io/team/Architect-Rust-Library-Design/53838c2d-1e48-5cec-8bb4-8fa8420e6171)

**Red Hat**

* [Senior Software Engineer - Virtualization & Storage (Remote Europe)](https://global-redhat.icims.com/jobs/82606/senior-software-engineer---virtualization-&-storage/job?mobile=false&width=708&height=500&bga=true&needsRedirect=false&jan1offset=60&jun1offset=120)

**Starry**

* [Rust Software Engineer (Boston, MA, US)](https://www.arbeitnow.com/view/rust-software-engineer-starry-293692)

**NZXT**

* [Senior Software Engineer for CAM (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=259)
* [Senior Software Engineer for Streaming Software (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=317)

**Kollider**

* [Junior Backend Engineer (Remote)](https://kollider.homerun.co/junior-backend-engineer/en)
* [Senior Backend Engineer (Remote)](https://kollider.homerun.co/senior-backend-engineer/en)
* [DevOps Engineer (Remote)](https://kollider.homerun.co/devops-engineer/en)

**Kraken**

* [Several Rust Engineering Postions Available](https://jobs.lever.co/kraken?team=Engineering)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

# 本周引语

好吧，如你所愿。让我们全力以赴吧：

> 这次，我们有两个 crate 和一条引语。虽然不多，但鼓舞人心。保持这个节奏，伙计们！

– [llogiq 发表于 reddit](https://www.reddit.com/r/rust/comments/ngp41e/this_week_in_rust_391/gysis5e)（译注：llogiq 即是 Rust 周报编辑人员之一）

谢谢 [Patrice Peterson](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1051) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
