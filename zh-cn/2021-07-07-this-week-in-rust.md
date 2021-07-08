# Rust 官方周报 398 期（2021-07-07）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。
> 
> 关于周报中的资源链接，已经有中文资源的，替换为中文资源链接（中文资源中，均附有原文链接）。另外，对于部分周报文章，附有阅读和简单了解后的译注，但并非全部。如果你阅读了文章，有更适合的见解，请联系、PR，或者直接参与项目 [github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)。

大家好，欢迎查阅第 398 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

## Rust 社区更新

### 官方
* [内部] [错误处理（Error Handling）项目组的工作方向](https://blog.rust-lang.org/inside-rust/2021/07/01/What-the-error-handling-project-group-is-working-towards.html)

### 项目/工具更新
* [Linux 中支持 Rust 的补丁系列](https://lore.kernel.org/lkml/20210704202756.29107-1-ojeda@kernel.org/)
* [Intellij Rust 更新日志 #150](https://intellij-rust.github.io/2021/07/05/changelog-150.html)
* [Rust Analyzer 更新日志 #84](https://rust-analyzer.github.io/thisweek/2021/07/05/changelog-84.html)
* [GCC Rust 月报 #7 - 2021 年 6 月](https://thephilbert.io/2021/07/05/gcc-rust-monthly-report-7-june-2021/)
* [Buck 前景规划](https://developers.facebook.com/blog/post/2021/07/01/future-of-buck)（译注：buck 起初是由 facebook 开发的 Android 快速构建系统，现在已经拓展为支持 15 种语言的跨平台快速构建系统）
* [ChainSafe 对 Mina spec Community Spotlight 的 Rust 实现（视频）](https://youtu.be/NaxZR-LDc_g)
* [MoonZoon 开发周报（5）：聊天实例、MoonZoon 云（Cloud）](https://dev.to/martinkavik/moonzoon-dev-news-5-chat-example-moonzoon-cloud-5de4)
* [Fluvio：可编程的数据平台](https://www.infinyon.com/blog/2021/06/introducing-fluvio/)（译注：fluvio 是一个原生云、高性能的分布式流数据平台，Rust 开发，主要应用方向为开发实时应用程序）
* [butido - Rust 中得 Linux 包（Package）构建工具](https://beyermatthias.de/butido-a-linux-package-building-tool-in-rust)（译注：使用 Docker 容器构建 Linux 包）
* [Knurling-rs 更新日志 #28](https://ferrous-systems.com/blog/knurling-changelog-28/)（译注：Knurling-rs 主要致力于嵌入式 Rust 体验）
* [`fcp` 0.2.0 发布 - 比 `cp` 命令快很多](https://github.com/Svetlitski/fcp)（译注：笔者已经使用，很棒）
* [Sycamore v0.5.0 发布 - SSR、路由](https://sycamore-rs.netlify.app/news/announcing-v0.5.0)（译注：sycamore 是无 VDOM（VDOM-less）的 Rust web 库，可在 Rust 和 WebAssembly 中提供更细的粒度）
* [TensorBase 周报 - 10](https://tensorbase.io/thisweek/2021-07-07-tw_10/)

### 观测/思考
* [以“Java 教程（The Java Tutorials）”的方式学习 Rust - 接口（Interface）的概念及其特化](https://rust-java-tutorials.netlify.app/blog/6-interfaces/)
* [Rust 和 Tinyverse](https://tinyverse.substack.com/p/rust-and-tinyverse)（译注：此处的 Tinyverse 非指游戏，而是机器学习方面的应用）
* [使用 Rust + WebAssembly 提速 WebCola 图形可视化库](https://cprimozic.net/blog/speeding-up-webcola-with-webassembly/)（译注：效果真的很棒，比如下图这个复杂的谱图关系，操作全面，响应极速）
![使用 Rust + WebAssembly 提速 WebCola 图形可视化库](https://blog.budshome.com/static/articles/1623905978.jpg)
* [Rust 闭包（closures）：闭包（closure）如何实现多个 trait](https://diaries.vercel.app/posts/closure-traits-rust/)

### Rust 演练
* [Rust 在前端（front-end）开发中的应用](https://blog.frankel.ch/start-rust/5/)
* [使用 Rocket 部署 Rust Web 应用](https://www.koyeb.com/tutorials/deploy-a-rust-web-app-with-rocket)
* [30 行 Rust 实现 TCP 代理](https://zmedley.com/tcp-proxy.html)
* [使用 Docker 工具管理 WasmEdge 中的 WebAssembly 应用](https://www.secondstate.io/articles/manage-webassembly-apps-in-wasmedge-using-docker-tools/)（译注：WasmEdge 是一个 CNCF (Cloud Native Computing Foundation云原生计算基金会)托管的官方沙盒项目。之前名为 SSVM，是为边缘计算优化的高性能 WebAssembly (Wasm) 虚拟机）
* [Rust 概念澄清：Deref vs AsRef vs Borrow vs Cow](https://dev.to/zhanghandong/rust-concept-clarification-deref-vs-asref-vs-borrow-vs-cow-13g6)
* [Rust 中的线程安全（Thread safety）](https://dev.to/onesignal/thread-safety-and-learning-in-rust-1p83)
* [使用 Rust 封装 REST API](https://dev.to/rogertorres/rest-api-wrapper-with-rust-mk4)
* [视频] [使用 Rust 构建 Web 应用（7）- Auth 中间件](https://www.youtube.com/watch?v=NEyUq5AVF2U)
* [视频] [使用 Rust 构建 Web 应用（8）- Containerization](https://www.youtube.com/watch?v=iEZAnmVX7yk)
* [视频] [Rust & Bevy 教程 - 从零开始构建游戏（1）](https://www.youtube.com/watch?v=Yb3vInxzKGE)（译注：bevy 是由 Rust 实现的数据驱动的游戏引擎）
* [视频] [使用异步（async）Rust 和 Tokio 创建一个聊天服务器](https://www.youtube.com/watch?v=4DqP57BHaXI)
* [视频] [1Password Developer Fireside：深入理解 Rust 中的 Async & Futures](https://www.youtube.com/watch?v=HrxwOUVzyDU)

### 其它

*无*

## 周最佳 crate

本周最佳 crate 是 [css-inline](https://github.com/Stranger6667/css-inline)，内联 CSS 到 `style` 标签的库。

谢谢 [Dmitry Dygalo](https://users.rust-lang.org/t/crate-of-the-week/2704/931) 的提议。

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

## 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

**Synth**

* [Feature: Scheduler / Topological sorting namespaces](https://github.com/getsynth/synth/issues/29)
* [Use parameterized Statements for Postgres export](https://github.com/getsynth/synth/issues/30)
* [Feature: Doc template generator](https://github.com/getsynth/synth/issues/31)
* [XML export / import](https://github.com/getsynth/synth/issues/32)
* [Feature: CSV import/export](https://github.com/getsynth/synth/issues/33)

**Sycamore**

* [Sycamore has some good first issues](https://github.com/sycamore-rs/sycamore/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

## Rust 核心更新

[297 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-06-28..2021-07-05

### Rust 编译器性能

本周采用新的分类流程，将为 PRs 贴上标签，并将引入性能回归标签。以供作者总结，以及问题跟踪。

希望这个改进，能够在长期范围内提高编译器性能。

验测工作是由 **@rylev** 完成的。修正范围1：
Revision range: [5a78340..9a27044](https://perf.rust-lang.org/?start=5a7834050f3a0ebcd117b4ddf0bc1e8459594309&end=9a27044f42ace9eb652781b53f598e25d4e7e918&absolute=false&stat=instructions%3Au)

[此处可查阅完整报告](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-07-06.md).

### 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

*无。*

### 新的 RFCs

*无。*

## 近期活动

### 线上

* [July 7, 2021, Denver, CO, US - End-to-end Encrypted Messaging in Rust, with Ockam by Mrinal Wadhwa - Rust Denver](https://www.meetup.com/Rust-Boulder-Denver/events/277633525/)
* [July 8, 2021, Berlin, DE - Rust Hack and Learn - Berline.rs](https://berline.rs/)
* [July 13, 2021, Seattle, WA, US - Monthly meetup - Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksrycckbrb/)
* [July 14, 2021, Malaysia - Rust Meetup July 2021 - Golang Malaysia, feat Rustlang, Erlang, Haskelllang and `.*-?(lang|script)\`](https://docs.google.com/forms/d/e/1FAIpQLSdoVbexvU3TZox1D9yLKPUggeTuih7TEDR6eaFQGTEgJtXZ5g/viewform)
* [July 14, 2021, Dublin, IE - Rust Dublin July Remote Meetup - Rust Dublin](https://www.meetup.com/Rust-Dublin/events/278698763/)
* [July 21, 2021, Vancouver, BC, CA - Rust Adoption at Huawei - Vancouver Rust](https://www.meetup.com/Vancouver-Rust/events/zkqvjsycckbcc/)

### 北美

* [July 14, 2021, Atlanta, GA, US - Grab a beer with fellow Rustaceans - Rust Atlanta](https://www.meetup.com/Rust-ATL/events/qxqdgrycckbsb/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

## Rust 招聘信息

**StructionSite**

* [Backend Engineer - AI Pipeline (Remote)](https://jobs.lever.co/structionsite/3eecbb4d-427b-4e99-87fd-89533b9e7510)

**ChainSafe Systems**

* [Rust Developer (Remote)](https://jobs.smartrecruiters.com/ChainSafeSystemsInc/743999739358248-rust-developer)

**InfinyOn**

* [Senior Rust Engineer(Remote))](https://infinyon.zohorecruit.com/jobs/Careers/619885000000428015/Senior-Rust-Software-Engineer?source=CareerSite)

**Merantix**

* [Senior Software Engineer (Data Infrastructure) (Berlin, DE)](https://arbeitnow.com/view/senior-software-engineer-data-infrastructure-merantix-125225)

**NORICS GmbH**

* [Softwareentwickler (m/w/d) (Norden, DE)](https://www.norics.de/job)

**NZXT**

* [Senior Software Engineer for CAM (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=259)
* [Senior Software Engineer for Streaming Software (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=317)

**Parity Technologies**

* [Several positions available (Berlin, DE and Remote)](https://www.parity.io/jobs/)

**Esturary**

* [Several positions available (New York, NY, US and Columbus, OH, US)](https://estuary.dev/careers)

**Kraken**

* [Several positions available (Remote)](https://jobs.lever.co/kraken?team=Engineering)

**Subspace Network**

* [Several positions available (Remote)](https://jobs.lever.co/subspacelabs)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

# 本周引语

> 对于 Rust，我喜欢其的一点是：它能过滤掉懒惰或者草率的思考者。即使我不同意其他 Rust 程序员的观点，但也本着一种尊重的态度。因为通过借用检查器（borrow checker），就可以晓得他们对问题的思考已经足够深入了。

– [Zeroexcuses 发表于 rust-users](https://users.rust-lang.org/t/what-is-you-elevator-pitch-for-rust/61713/7?u=llogiq)

谢谢 [Jonah](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1070) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
