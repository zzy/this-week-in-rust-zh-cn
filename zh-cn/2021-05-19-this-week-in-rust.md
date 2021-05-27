# Rust 官方周报 391 期（2021-05-19）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。
> 
> 关于周报中的资源链接，已经有中文资源的，替换为中文资源链接（中文资源中，均附有原文链接）。另外，对于部分周报文章，附有阅读和简单了解后的译注，但并非全部。如果你阅读了文章，有更适合的见解，请联系、PR，或者直接参与项目 [github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)。

大家好，欢迎查阅第 391 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

# Rust 社区更新

本周无相关简讯或研讨/论文。

### 官方
* [Rustup 发布版本 1.24.2](https://blog.rust-lang.org/2021/05/17/Rustup-1.24.2.html)
* [Rust，风雨六载，砥砺奋进](https://blog.budshome.com/budshome/rust,feng-yu-liu-zai-,di-li-fen-jin)

### 项目/工具更新
* [rust-analyzer 更新日志 #77](https://rust-analyzer.github.io/thisweek/2021/05/17/changelog-77.html)
* [IntelliJ Rust 更新日志 #147](https://intellij-rust.github.io/2021/05/18/changelog-147.html)
* [GCC Rust 每周状态报告 15](https://thephilbert.io/2021/05/14/gcc-rust-weekly-status-report-15/)（译注：gcc 的 Rust 实现，还处于早期的阶段，并不能实际编译）
* [MoonZoon 开发简报（3）：Signals，类 React 的钩子（Hooks），及其优化](https://dev.to/martinkavik/moonzoon-dev-news-3-signals-react-like-hooks-optimizations-39lp)（译注：MoonZoon 演示看起来还不错，作者说其是 `NO Javascript、NO CSS、NO HTML、NO REST、NO GraphQL、NO SQL、NO Analysis Paralysis、NO Wheel Reinventing、NO Passwords*` 的 Rust 全栈开发框架）
* [Alacritty 发布版本 0.8.0](https://github.com/alacritty/alacritty/releases/tag/v0.8.0)（译注：Alacritty 是 Rust 实现的、快速的、跨平台的 OpenGL 终端模拟器）
* [Micromath 2.0.0：基于近似值的（approximation-based）嵌入式算法，2D/3D 动态数组（vector），四分位数（quarternion），及其统计库](https://www.reddit.com/r/rust/comments/nekdbc/ann_micromath_200_approximationbased_embedded/)（译注：Micromath 是适用于嵌入式 Rust 的科学计算库）
* [TensorBase 周报 3 期](https://tensorbase.io/thisweek/2021-05-19-tw_3/)（译注：TensorBase 是基于 Rust 的现代化开源数据仓库）

### 观测/思考
* [Rust web 应用中的认证/授权（authorization）机制](https://ddtkey.com/blog/authz-mechanisms-in-Rust/)
* [Scylla 开发者会议和黑客马拉松（Hackathon）：Rust Driver](https://www.scylladb.com/2021/02/17/scylla-developer-hackathon-rust-driver/)（译注：ScyllaDB 是用 C++ 重写的 Cassandra，官方称其拥有比 Cassandra 高达 10x 倍的吞吐量，并降低了延迟，是性能优异的 NoSQL 列存储数据库，主要应用于实时数据方面。目前，ScyllaDB 已经在向 Rust 迁移）
* [Rust 中的插件开发技术](https://nullderef.com/blog/plugin-tech/)（译注：讲述如何在 Rust 中实现 PDK，即插件开发工具包，Plugin Development Kit。此文很值得读，从 6 个方面讲解了跨平台、安全、移植，以及兼容性等）
* [Rust 中实现 gRPC 的负载均衡](https://truelayer.com/blog/grpc-load-balancing-in-rust)
* [重新审视 Rust 编译中的矢量化（Verifying vectorized Rust revisited）](https://project-oak.github.io/rust-verification-tools/2021/05/15/verifying-vectorized-code2.html)（译注：讲述可以通过设定 Rust 编译器，不自动对代码进行矢量化。以及 SIMD 指令和模拟库的使用）
* [Rust 探索之旅](https://blog.abor.dev/p/timclicks)（译注：Tim McNamara 访谈，讨论如何通过学习 Rust，以进行系统编程）
* [运用模糊化（fuzzing）来提高 TezEdge 节点（node）的安全性，并创建 Rust 代码模糊化的开源 CI 工具](https://medium.com/tezedge/how-we-utilized-fuzzing-to-improve-security-in-the-tezedge-node-and-created-an-open-source-ci-tool-92ffbd804db1)
* [使用 Rust 提高生产率（boost productivity）](https://dev.to/pancy/boost-productivity-with-rust-anf)
* [为 Linux 构建 Outer Wonders 游戏](https://utopixel.games/en/blog/building-outer-wonders-for-linux/)（译注：Outer Wonders 是一款益智游戏，具有开放性，以及丰富的视觉。如下截图所示）
![outer wonders](https://blog.budshome.com/static/articles/1621498886.gif)
* [1Password for Linux 的开发幕后](https://dteare.medium.com/behind-the-scenes-of-1password-for-linux-d59b19143a23)（译注：1Password 的生产环境中，使用 Rust 已有几年。详细参见文章 [Rust 用在生产环境的 42 家公司](https://blog.budshome.com/budshome/rust-yong-zai-sheng-chan-huan-jing-de-42-jia-gong-si)。1Password 公司的 Windows 团队，是这项工作的领跑者，Windows 中所用的 1Password 7，大约 70% 都是用 Rust 开发的。在 2019 年底，1Password 还将 1Password Brain（驱动浏览器填充逻辑的引擎）从 Go 移植到了 Rust，以在浏览器扩展中，发挥将 Rust 程序部署到 WebAssembly 应用的性能优势）
* [编写 Python 风格（Pythonic）的 Rust 代码](http://www.cmyr.net/blog/rust-python-learnings.html)（译注：文章很有趣，建议一读）
* [parking_lot::RwLock 的运作，或许并非你所期望](https://morestina.net/blog/1739/upgradable-parking_lotrwlock-might-not-be-what-you-expect)（译注：parking_lot 是 Rust 中紧凑高效的同步原语 crate，提供了用于创建自定义同步原语的 API）
* [为什么我们应当将 Rust 用于嵌入式开发？](https://blog.budshome.com/budshome/wei-shi-yao-wo-men-ying-dang-jiang-rust-yong-yu-qian-ru-shi-kai-fa--)

### Rust 演练
* [理解 Rust 的私有性（Privacy）和可见性（Visibility）模型](https://iximiuz.com/en/posts/rust-privacy-and-visibility/)（译注：夯实基础的好文，包括子模块访问父模块，提升父模块的私有性，以及 `use` 关键词的深入介绍等）
* [Rust 中不能做和应该做的事](https://blog.logrocket.com/what-you-cant-do-in-rust-and-what-to-do-instead/)
* [Rust 及其 WebAssembly 开发中的状态管理](https://dev.to/seanwatters/state-management-with-webassembly-rust-5a1g)
* [Rust 中实现链表（Linked List）](https://dev.to/felixfaisal/implementing-linked-list-in-rust-3and)
* [在 Rust Tonic 和 Postgres 数据库中使用 gRPC 的实例](https://dev.to/steadylearner/how-to-use-grpc-with-rust-tonic-and-postgres-database-with-examples-3dl7)
* [Rust 中生成预签名的（pre-signed）S3 URLs](https://dev.to/rtyler/generating-pre-signed-s3-urls-in-rust-27gd)（译注：AWS S3，通过签名的 URL 来完成访问控制）
* [介绍一个简单的用户输入、验证，以及转换的 Rust 库](https://dev.to/jahwi/a-simple-user-input-collection-validation-and-conversion-library-in-rust-34cj)
* [使用 Rust 和 Teloxide 创建加密货币（cryptocurrency）的电报机器人](https://dev.to/steadylearner/how-to-make-a-telegram-bot-with-rust-teloxide-m60)（译注：teloxide 是电报机器人框架）
* [Rust 中，使用 RV 0.12 实现无限混淆（Infinite Mixture）模型](https://redpoll.ai/blog/imm-with-rv-12/)
* [逐步优化 HashMaps](https://blog.yoshuawuyts.com/optimizing-hashmaps-even-more/)
* [`Service` trait 的创建尝试](https://tokio.rs/blog/2021-05-14-inventing-the-service-trait)（译注：`Service` trait 是 Tower 框架的核心）
* [warp 框架中，`route` 宏的应用“干货”](https://shivjm.blog/rust-macros-rule-dry-warp-routes/)
* [深入理解 Rust 中的错误处理](https://www.lpalmieri.com/posts/error-handling-rust/)
* [德文] [Rust 中的存储管理（Speicherverwaltung in Rust）](https://jo-so.de/2021-01/Speicher-Rust.html)
* [西班牙文] [Cómo utilizar Rust web framework Warp](https://dev.to/steadylearner/como-utilizar-rust-web-framework-warp-n3c)
* [葡萄牙文] [O que é dyn no Rust?](https://dev.to/henrybarreto/o-que-e-dyn-no-rust-4ol9)
* [中文] [Rust web 开发中，将 markdown 渲染为 HTML 的实践](https://blog.budshome.com/budshome/rust-zhong-jiang-markdown-xuan-ran-wei-html)
* [中文] [系列] [基于 actix-web + async-graphql + rbatis + postgresql / mysql 构建异步 Rust GraphQL 服务（4）](https://blog.budshome.com/budshome/ji-yu-actix-web-+-async-graphql-+-rbatis-+-postgresql---mysql-gou-jian-yi-bu-rust-graphql-fu-wu-(4)---bian-geng-fu-wu-,yi-ji-xiao-zhong-gou)
* [视频] [Rust 借用检查器（Borrow Checker） - 深入理解 @ Rust DC，2021 年 4 月 20 日 w/ Nell Shamrell-Harrington](https://youtu.be/Ys7ma3au5m0)

### 其它
* [James Munns 谈论嵌入式和专注安全性的 Rust 的现状和未来 | Emergence 博客](https://www.youtube.com/watch?v=SNUklwUi_M4)
* [Rust 2021 版次将在今年 10 月发布，具有“更持久的 panic”特性，以及其它新功能](https://www.theregister.com/2021/05/13/rust_2021_edition/)
* [SpaceX 公司中，关于 Rust 语言的应用](https://www.reddit.com/r/rust/comments/ndm4ne/spacex_about_the_rust_programming_language/)

# 周最佳 crate

本周最佳 crate 是 [arraygen](https://docs.rs/arraygen)，派生（derive）过程宏（proc macro），用于从结构体（structs）生成数组。

谢谢 [José Manuel Barroso Galindo](https://users.rust-lang.org/t/crate-of-the-week/2704/911) 的提议。

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

*本周无参与邀请*。

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Rust 核心更新

[333 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-05-10..2021-05-17

## Rust 编译器性能

本周的基准测试结果，有许多噪音。我们正在讨论（[zulip archive](https://zulip-archive.rust-lang.org/247081tcompilerperformance/06104coercionsdebugnoise.html)、[live zulip](https://rust-lang.zulipchat.com/#narrow/stream/247081-t-compiler.2Fperformance/topic/coercions-debug.20noise)）如何最恰当地跟新基准测试集，以消除噪音对测试的干扰。除此之外，还有一些独立的基准测试，对其进行了较大改进。

内存使用率（[max-rss](https://perf.rust-lang.org/?start=2021-05-11&end=2021-05-18&absolute=true&stat=max-rss)）似乎基本持平。除过 `tuple-stess`，其内存使用比上周增加了 4%。

验测工作是由 **@pnkfelix**完成的。修正范围：[382f..25a2](https://perf.rust-lang.org/?start=382f748f23979e37e3e012b090e5a0313463f182&end=25a277f03df7e44643ddfcc240d034409cb2f505&absolute=false&stat=instructions%3Au)

[此处可查阅完整报告](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-05-18.md)。

## 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

*本周无已核准的 RFCs*。

## 新的 RFCs

* [Pinned synchronization primitives](https://github.com/rust-lang/rfcs/pull/3124)

# 近期活动

### 线上
* [May 19, 2021, Vancouver, BC - Rust Study/Hack/Hang-out night - Vancouver Rust](https://www.meetup.com/Vancouver-Rust/events/zppkjsycchbzb/)
* [May 20, 2021, Online - Go vs Rust | Round table discussion](https://rustlab.it/en/rust-vs-go/)
* [May 20, 2021, Dallas, TX, US - Last Tuesday - Dallas Rust](https://www.meetup.com/Dallas-Rust/events/jqxqwrycchbhc/)
* [May 25, 2021, Berlin, DE - Rust and Tell - Berline.rs](https://berline.rs/)
* [May 27, 2021, Montréal, QC, CN - Rust MTL: Building a Scrabble AI with the fst crate - Rust Montréal](https://www.meetup.com/Rust-Montreal/events/278011978/)
* [June 1, 2021, Buffalo, NY, US - Buffalo Rust User Group, First Tuesdays - Buffalo Rust Meetup](https://www.meetup.com/Buffalo-Rust-Meetup/events/jxfdjsyccjbcb/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust 招聘信息

**Protocol Labs**

* [Research Engineer, CryptoCompute Lab (Remote)](https://www.arbeitnow.com/view/research-engineer-cryptocompute-lab-protocol-labs-444987)

**Amazon Web Services**

* [Applied Scientist (Boston/Cambridge Area, MA, US)](https://www.amazon.jobs/en/jobs/1555897/applied-scientist)

**Techno Creatives**

* [Senior Rust Full Stack Developer (Gothenburg, Sweden)](https://technocreatives.homerun.co/senior-rust-full-stack-developer/en)

**Paige**

* [Senior Software Engineer, Visualization (Remote, Europe)](https://boards.greenhouse.io/paige/jobs/5210311002)

**ANIXE**

* [Rust Software Engineer (Wrocław, PL)](https://anixe.bamboohr.com/jobs/view.php?id=72)

**NZXT**

* [Senior Software Engineer for CAM (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=259)
* [Senior Software Engineer for Streaming Software (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=317)

**Zondax**

* [Embedded Systems Engineer (C/C++ & Rust)(Remote)](https://zondax.ch/news/embedded-systems-engineer)
* [Software Engineer (Golang / Rust) (Remote)](https://zondax.ch/news/engineers-golang-rust)

**Ockam**

* [Several Rust related positions available](https://www.ockam.io/team#open-roles)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

# 本周引语

> 我常常将 Rust 视为开发编程语言的工艺流程和社区，而非编程语言自身。

– [throwaway894345 发表于 hacker news](https://news.ycombinator.com/item?id=27120691)

谢谢 [Krishna Sundarram](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1050) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
