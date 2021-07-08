# Rust 官方周报 397 期（2021-06-30）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。
> 
> 关于周报中的资源链接，已经有中文资源的，替换为中文资源链接（中文资源中，均附有原文链接）。另外，对于部分周报文章，附有阅读和简单了解后的译注，但并非全部。如果你阅读了文章，有更适合的见解，请联系、PR，或者直接参与项目 [github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)。

大家好，欢迎查阅第 397 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

## Rust 社区更新

### 官方

* [基金会] [招聘高级管理人员](https://foundation.rust-lang.org/posts/2021-06-25-announcing-executive-search/)

### 项目/工具更新

* [ChainSafe 的波卡指数网络代币（PINT，Polkadot Index Network Token）更新日志 #2](https://medium.com/chainsafe-systems/pint-community-update-2-b337ece3f031)
* [Rust Analyzer 更新日志 #83](https://rust-analyzer.github.io/thisweek/2021/06/28/changelog-83.html)
* [Fang 0.2 发布](https://www.badykov.com/rust/2021/06/27/fang/)（译注：fang 是应用 postgres 作为数据库存储的 Rust 后台处理 crate）
* [Veloren 周报 125](https://veloren.net/devblog-125/)
* [TensorBase 周报 9](https://tensorbase.io/thisweek/2021-06-30-tw_9/)

### 观测/思考

* [Rust 中，使用 wasmi 轻松托管（hosting）wasm 模块](https://blog.knoldus.com/hosting-wasm-modules-in-rust-easily-using-wasmi/)（译注：wasmi 是一个 wasm 解释器，可以做到在**浏览器之外**托管使用 wasm 模块。目前用起来还是很繁琐，但是笔者认为思路和前景都不错，对 wasm 开发感兴趣的朋友推荐阅读）
* [视频] [为什么“云”的未来将会基于 Rust](https://www.youtube.com/watch?v=BWL4889RKhU&t=5s)

### Rust 演练

* [Rust 中对二进制数据反序列化](https://adventures.michaelfbryan.com/posts/deserializing-binary-data-files/)
* [Rust 中的类型检查（type-checked）库 keypaths](http://www.cmyr.net/blog/keypaths.html)
* [Rust 中的多态（polymorphism）](https://oswalt.dev/2021/06/polymorphism-in-rust/)
* [使用 GitHub Actions 交叉编译（Cross Compiling）Rust 二进制文件](https://www.rohanjain.in/cargo-cross/)
* [Rust #2：生命周期（Lifetimes）、所有权（Owners），以及借用（Borrowers）](https://dev.to/cthutu/rust-2-lifetimes-owners-and-borrowers-oh-my-3fem)
* [系列] [Rust 中构建 API（3）](https://dev.to/naruhodo/build-an-api-in-rust-part-3-11j1)
* [系列] [视频] [使用 Rust 构建 web 应用（5）- HTTP 服务器和数据库管理](https://www.youtube.com/watch?v=TCUnZVLgNps)
* [系列] [视频] [使用 Rust 构建 web 应用（6）- 增删改查接口（CRUD API）](https://www.youtube.com/watch?v=v7y_Ngn_-AY)
* [视频] [Rust 初学者系列](https://www.youtube.com/playlist?list=PLlrxD0HtieHjbTjrchBwOVks_sr8EVW1x)
* [视频] [整合 Bloc/Cubit 和 Rid，构建多线程的 Flutter + Rust 应用](https://www.youtube.com/watch?v=PGKBdxOA6Xs&t=1s)
* [视频] [Rust 中实现风险指针（Hazard Pointers）](https://www.youtube.com/watch?v=fvcbyCYdR10)
* [视频] [Rust Linz；2021 年 6 月 - Tim McNamara - 如何学习 Rust](https://www.youtube.com/watch?v=sDtQaO5_SOw)

### 其它

* [Rust 程序设计语言（第二版）已发售](https://www.oreilly.com/library/view/programming-rust-2nd/9781492052586/)
* [Rust in Action 已发售](https://www.manning.com/books/rust-in-action)

## 周最佳 crate

本周最佳 crate 是 [hypergraph](https://github.com/yamafaktory/hypergraph)，图形数据结构实现库，可描述由任意数量顶点构成的多边图形（译注：基于 `Graphviz dot` 格式）。

谢谢 [Davy Duperron](https://users.rust-lang.org/t/crate-of-the-week/2704/929) 的提议。

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

## 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

## Rust 核心更新

[284 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-06-21..2021-06-28

### Rust 编译器性能

本周仅有部分结构（详细信息请查阅完整报告）。从收集的结果来看，由几处小的回归，以及一些改进。此外，与 11 天比较，出现了广泛的 [max-rss 回归](https://perf.rust-lang.org/compare.html?start=29cd70d40722930e66a8b726fe58a7bd1d64a22b&end=6b354a13820a444f834a33365ae4a8d97d7d27ce&stat=max-rss)。与 9 天前比较，[max-rss 回归](https://perf.rust-lang.org/compare.html?start=406d4a9cc3b9601cf98a07c6c83e0227d64f5d48&end=4573a4a879a8e1f773944a8859e4dcd136138af8&stat=max-rss)则比较狭窄。

验测工作是由 **@pnkfelix**完成的。修正范围1：[406d4a9..5a78340](https://perf.rust-lang.org/?start=406d4a9cc3b9601cf98a07c6c83e0227d64f5d48&end=5a7834050f3a0ebcd117b4ddf0bc1e8459594309&absolute=false&stat=instructions%3Au)、修正范围2：[7c3872e..7ede6e2](https://perf.rust-lang.org/?start=7c3872e6bfd555d2ad753ac1f871db3bd7f2a547&end=7ede6e2a2359c1bb9032baffa4fdafe5633749e3&absolute=false&stat=instructions%3Au)

[此处可查阅完整报告](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-06-30.md).

### 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

*无。*

### 新的 RFCs

* [Candidate Target Policy](https://github.com/rust-lang/rfcs/pull/3145)

## 近期活动

### 线上

* [July 6, 2021, Buffalo, NY, US - Buffalo Rust User Group, First Tuesdays - Buffalo Rust Meetup](https://www.meetup.com/Buffalo-Rust-Meetup/events/jxfdjsycckbjb/)
* [July 7, 2021, Denver, CO, US - End-to-end Encrypted Messaging in Rust, with Ockam by Mrinal Wadhwa - Rust Denver](https://www.meetup.com/Rust-Boulder-Denver/events/277633525/)
* [July 13, 2021, Seattle, WA, US - Monthly meetup - Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksrycckbrb/)
* [July 14, 2021, Malaysia - Rust Meetup July 2021 - Golang Malaysia, feat Rustlang, Erlang, Haskelllang and `.*-?(lang|script)\`](https://docs.google.com/forms/d/e/1FAIpQLSdoVbexvU3TZox1D9yLKPUggeTuih7TEDR6eaFQGTEgJtXZ5g/viewform)
* [July 14, 2021, Dublin, IE - Rust Dublin July Remote Meetup - Rust Dublin](https://www.meetup.com/Rust-Dublin/events/278698763/)

### 北美

* [July 14, 2021, Atlanta, GA, US - Grab a beer with fellow Rustaceans - Rust Atlanta](https://www.meetup.com/Rust-ATL/events/qxqdgrycckbsb/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

## Rust 招聘信息

**Field 33**

* [Senior Software Engineer Backend - Java/Rust (Berlin, DE)](https://arbeitnow.com/view/senior-software-engineer-backend-javarust-fxm-field-33-55295)

**Georg Fischer**

* [Software Engineer (Remote)](https://www.indeed.com/viewjob?cmp=Georg-Fischer-Signet-LLC&t=Software+Engineer&jk=c5a6c3823ac77bd4)

**Rhebo**

* [Softwareentwickler Rust - Schwerpunkt Netzwerk (Remote)](https://rhebo.com/de/unternehmen/karriere/job/senior-software-entwickler-rust-m-w/)

**ChainSafe Systems**

* [Rust Developer (Remote)](https://jobs.smartrecruiters.com/ChainSafeSystemsInc/743999739358248-rust-developer)

**Mimo**

* [Full-time senior Rust developer (Remote)](https://github.com/mimo-capital/jobs/blob/main/Full-time%20senior%20Rust%20developer.md)

**Anixe**

* [Rust Software Engineer (Wrocław, PL)]()

**NZXT**

* [Senior Software Engineer for CAM (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=259)
* [Senior Software Engineer for Streaming Software (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=317)

**Kollider**

* [Junior Backend Engineer (Remote)](https://kollider.homerun.co/junior-backend-engineer/en)
* [Senior Backend Engineer (Remote)](https://kollider.homerun.co/senior-backend-engineer/en)
* [DevOps Engineer (Remote)](https://kollider.homerun.co/devops-engineer/en)

**Ockam**

* [Multiple Rust Engineering Positions Available (Remote)](https://www.ockam.io/team#open-roles)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
