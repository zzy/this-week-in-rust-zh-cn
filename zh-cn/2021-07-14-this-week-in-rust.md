# Rust 官方周报 399 期（2021-07-14）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。
> 
> 关于周报中的资源链接，已经有中文资源的，替换为中文资源链接（中文资源中，均附有原文链接）。另外，对于部分周报文章，附有阅读和简单了解后的译注，但并非全部。如果你阅读了文章，有更适合的见解，请联系、PR，或者直接参与项目 [github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)。

大家好，欢迎查阅第 399 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

## Rust 社区更新

### 官方

*无。*

### 简讯
* [Rust 游戏开发（GameDev）月报 #23 - 2021 年 6 月](https://gamedev.rs/news/023/)
* [Rust 操作系统开发（OSDev）月报 - 2021 年 6 月](https://rust-osdev.com/this-month/2021-06/)

### 项目/工具更新
* [Arti，纯粹 Rust 实现的 Tor](https://blog.torproject.org/announcing-arti)
* [Fluvio，基于 WebAssembly 的可编程实时数据流处理平台](https://www.infinyon.com/blog/2021/06/smartstream-filters/)
* [Filecoin 项目更新 - Rust 实现的 “Forest” 项目](https://medium.com/chainsafe-systems/forest-growth-d26998a3da61)
* [Mina Rust 更新：具有 Rust x Wasm 特性的 Web 3.0](https://medium.com/chainsafe-systems/mina-wasm-benefits-for-web-3-0-3d25991c3b75)（译注；ChainSafe 的 mina-rs 是 Mina 协议的 Rust 实现，专注于 web 和 Wasm 的兼容性）
* [TensorBase 周报 - 11](https://tensorbase.io/thisweek/2021-07-14-tw_11/)
* [Rust Analyzer 更新周报 #85](https://rust-analyzer.github.io/thisweek/2021/07/12/changelog-85.html)

### 观测/思考
* [(Risp (in (Rust) (Lisp)))](https://stopachka.essay.dev/post/5/risp-in-rust-lisp)（译注：risp 项目受 Clojure 启发，使用 Rust 创建 Lisp）
* [系列] [Rust 学习 #6：理解 Rust 中的所有权（ownership）](https://hamatti.org/posts/learning-rust-6-ownership/)
* [系列] [Rust 中，为什么及如何开发编译器（compiler）： 第二部分](https://bnjjj.medium.com/why-and-how-we-wrote-a-compiler-in-rust-blog-post-series-2-x-the-stack-548dad1919d0)
* [视频] [Rust 1.52 和 1.53 差异对比](https://rustacean-station.org/episode/034-rust-1.52-1.53/)（译注：推荐观看，介绍详细，并且收集了相关资料）

### Rust 演练
* [Rust 中的 `#[inline]`](https://matklad.github.io//2021/07/09/inline-in-rust.html)
* [从 C、C++ 和 Rust 调用 WebAssembly 线程](https://web.dev/webassembly-threads/)（译注：推荐了解，wasm 应用前景广阔）
* [在树莓派（Raspberry Pi）上轻松地托管 wasm 模块（1）](https://blog.knoldus.com/host-a-wasm-module-on-raspberry-pi-easily-part-1/)
* [你好，视频编解码器（Codec）！- 通过大约 100 行 Rust 代码，解开视频编解码的神秘面纱](https://medium.com/tempus-ex/hello-video-codec-9937f64835bd)
* [通过 FizzBuzz 游戏学习地道的 Rust](https://www.fotonixx.com/posts/rust-fizzbuzz/)（译注：FizzBuzz 问题是一种英国学校学生经常玩的游戏。比如：打印数字 1 到 100。但是遇到 3 的倍数时，打印“Fizz”；5的倍数，则打印“Buzz”；既是 3 又是5 的倍数是，打印“FizzBuzz”）
* [Rust + Tauri 快速入门](https://jbarszczewski.com/rust-tauri-svelte-tutorial)（译注：tauri 是一个用于构建桌面平台的框架，但可以集成任何可编译为 html、js，以及 CSS 的前端框架，以用来构建用户界面）
* [Rust Nibbles：Gazebo 库介绍](https://developers.facebook.com/blog/post/2021/07/06/rust-nibbles-gazebo-dupe/)（译注：gazebo 是包含小的、易于测试的原语集合库，其是 facebook 的孵化项目）
* [Kubernetes 的 Rust 控制器（controller）](https://blog.frankel.ch/start-rust/6/)（译注：很棒，可跟随实践。推荐细读）
* [Docker + Rust 使用起步](https://dev.to/rogertorres/first-steps-with-docker-rust-30oi)
* [系列] [使用 rg3d 编写 RPG - #1 - 字符控制器（Character Controller）](https://rg3d.rs/tutorials/2021/07/09/rpg-tutorial1.html)（译注：rg3d 是很优秀的 3D 射击游戏引擎，此文为角色扮演类游戏教程。笔者跑了一遍游戏，挺精致、有趣。可点击下载 [rg3d-tutorials 源码](https://github.com/rg3dengine/rg3d-tutorials)，注意 rpg 要用 rg3d 0.21.0，其它使用 rg3d 0.20.0 或以下）
![rpg](https://blog.budshome.com/static/articles/1626328998.png)
![weapon](https://blog.budshome.com/static/articles/1626329470.png)
* [系列] [Rust #4: Options 和 Results（2）](https://dev.to/cthutu/rust-4-options-and-results-part-2-5aca)
* [系列] [使用 Rust web 框架 tide 实现基本的增删改查（CRUD） - 重构](https://dev.to/pepoviola/basic-crud-with-rust-using-tide-refactoring-2meb)
* [视频] [Rust 中使用 ockam 对端对端通信加密，Mrinal Wadhwa 制作](https://www.youtube.com/watch?v=jKvIeQFZKLc)（译注：ockam 是 ockam.io 开发的、用于分布式应用之间的相互身份验证，以及端到端加密消息传递的工具）
* [视频] [系列] [使用 Rust 开发 web 应用（9）- 部署于 Kubernetes](https://www.youtube.com/watch?v=bK542nqn8I0)
* [视频] [系列] [ULTIMATE Rust 语言教程 - 智能指针（Smart Pointers）- 1](https://www.youtube.com/watch?v=m76sRj2VgGo)
* [视频] [系列] [Rust 中实现风险指针（Hazard Pointers）- 2](https://www.youtube.com/watch?v=_LK7qvBWNYo)

### 论文
* [软件开发者是否在安全地使用着 Rust？](https://arxiv.org/abs/2007.00752)（译注：康奈尔大学的论文数据为：在不到 30% 的 Rust 库中，使用了关键字 `unsafe`；但由于库的调用链中隐藏着 `unsafe` Rust，因此超过一半的代码不能被 Rust 编译器完全静态检查。论文建议更改 Rust 编译器和中心存储库的接口，以帮助 Rust 软件开发人员了解自己的代码何时 `unsafe`）

### 其它
* [超函数（hyperfunctions）介绍：PostgreSQL 中新的 SQL 函数，用于简化处理时间序列（time-series）数据](https://blog.timescale.com/blog/introducing-hyperfunctions-new-sql-functions-to-simplify-working-with-time-series-data-in-postgresql/?utm_source=timescaledb&utm_medium=social&utm_campaign=hyperfunctions-1-0-release&utm_content=blog-introducing-hyperfunctions)

## 周最佳 crate

本周最佳 crate 是 [endbasic](https://www.endbasic.dev)，可运行于小型硬件设备和 web 之上的 DOS / BASIC 环境模拟器。

谢谢 [Julio Merino](https://users.rust-lang.org/t/crate-of-the-week/2704/935) 的提议。

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

## 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

**Synth**

* [Specify collections on import](https://github.com/getsynth/synth/issues/45)
* [Add tests for examples (i.e. bank_db)](https://github.com/getsynth/synth/issues/44)
* [Implemented a converter for timestamptz](https://github.com/getsynth/synth/issues/35)
* [Feature: Doc template generator](https://github.com/getsynth/synth/issues/31)

**Forest**

* [Cleanup net peers output](https://github.com/ChainSafe/forest/issues/1184)
* [FOREST_CONFIG_PATH env var](https://github.com/ChainSafe/forest/issues/1191)

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

## Rust 核心更新

[254 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-07-05..2021-07-12

### Rust 编译器性能

十分安静的一周，带来诸多改进。

验测工作是由 **@simulacrum**完成的。修正范围：[9a27044f4..5aff6dd](https://perf.rust-lang.org/?start=9a27044f42ace9eb652781b53f598e25d4e7e918&end=5aff6dd07a562a2cba3c57fc3460a72acb6bef46&absolute=false&stat=instructions%3Au)

[此处可查阅完整报告](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-07-13.md).

### 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

* [RFC: I/O 安全性](https://github.com/rust-lang/rfcs/pull/3128)

### 新的 RFCs

* [RFC: Option 和 Result 中的 map_or_default](https://github.com/rust-lang/rfcs/pull/3148)
* [Cargo 功能迁移/合并](https://github.com/rust-lang/rfcs/pull/3146)

## 近期活动

### 线上

* [July 14, 2021, Malaysia - Rust Meetup July 2021 - Golang Malaysia, feat Rustlang, Erlang, Haskelllang and `.*-?(lang|script)\`](https://docs.google.com/forms/d/e/1FAIpQLSdoVbexvU3TZox1D9yLKPUggeTuih7TEDR6eaFQGTEgJtXZ5g/viewform)
* [July 14, 2021, Dublin, IE - Rust Dublin July Remote Meetup - Rust Dublin](https://www.meetup.com/Rust-Dublin/events/278698763/)
* [July 20, 2021, Washington, DC, US - Mid-month Rustful - Rust DC](https://www.meetup.com/RustDC/events/vdhxgsycckbbc/)
* [July 21, 2021, Vancouver, BC, CA - Rust Adoption at Huawei - Vancouver Rust](https://www.meetup.com/Vancouver-Rust/events/zkqvjsycckbcc/)
* [July 22, 2021, Tokyo, JP - Rust LT Online#4 - Rust JP](https://www.youtube.com/watch?v=oK0iJz7XF3Y)
* [July 22, 2021, Berlin, DE - Rust Hack and Learn - Berline.rs](https://berline.rs/)
* [July 27, 2021, Dallas, TX, US - Last Tuesday - Dallas Rust](https://www.meetup.com/Dallas-Rust/events/jqxqwrycckbkc/)

### 北美

* [July 14, 2021, Atlanta, GA, US - Grab a beer with fellow Rustaceans - Rust Atlanta](https://www.meetup.com/Rust-ATL/events/qxqdgrycckbsb/)
* [July 27, 2021, Chicago, IL, US - Rust in production at Tempus - Chicago Rust Meetup](https://www.meetup.com/Chicago-Rust-Meetup/events/279131036)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

## Rust 招聘信息

**GraphCDN**

* [Senior Rust Engineer (Remote)](https://jobs.lever.co/GraphCDN/93b9a4fc-cf56-46c4-9fad-d7b254bd20df)

**Netlify**

* [Senior Backend Engineer (Go/Rust) (Remote or San Francisco, CA, US)](https://arbeitnow.com/view/senior-backend-engineer-gorust-netlify-181900)

**ChainSafe Systems**

* [Rust Developer (Remote)](https://jobs.smartrecruiters.com/ChainSafeSystemsInc/743999739358248-rust-developer)

**NZXT**

* [Senior Software Engineer for CAM (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=259)
* [Senior Software Engineer for Streaming Software (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=317)

**Kollider**

* [Junior Backend Engineer (Remote)](https://kollider.homerun.co/junior-backend-engineer/en)
* [Senior Backend Engineer (Remote)](https://kollider.homerun.co/senior-backend-engineer/en)
* [DevOps Engineer (Remote)](https://kollider.homerun.co/devops-engineer/en)

**Tempus Ex**

* [Several positions available (San Francisco, Atlanta, and Remote)](https://tempus-ex.com/careers)

**Estuary**

* [Several positions available (New York, NY, US or Columbus, OH, US)](https://www.estuary.dev/careers)


*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

## 本周引语

> Rust 初学者：呃，为什么编译器阻止我做这些？太讨厌了！
>
> Rust 熟练者：呃，为什么编译器不阻止我做这些！太可恶了！

– [qDot 发表于 twitter](https://twitter.com/qDot/status/1412536312150716416)

谢谢 [Nixon Enraght-Moony](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1074) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
