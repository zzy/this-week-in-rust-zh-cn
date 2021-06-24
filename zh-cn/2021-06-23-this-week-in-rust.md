# Rust 官方周报 396 期（2021-06-23）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。
> 
> 关于周报中的资源链接，已经有中文资源的，替换为中文资源链接（中文资源中，均附有原文链接）。另外，对于部分周报文章，附有阅读和简单了解后的译注，但并非全部。如果你阅读了文章，有更适合的见解，请联系、PR，或者直接参与项目 [github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)。

大家好，欢迎查阅第 396 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

## Rust 社区更新

本周无相关官方博客，研讨/论文。

### 官方
* [Rust 1.53.0 发布](https://blog.rust-lang.org/2021/06/17/Rust-1.53.0.html)
* [内部] [Rust 编译器（Compiler）团队 6 月份计划](https://blog.rust-lang.org/inside-rust/2021/06/23/compiler-team-june-steering-cycle.html)

### 项目/工具更新
* [rust-analyzer 更新日志 #82](https://rust-analyzer.github.io/thisweek/2021/06/21/changelog-82.html)
* [IntelliJ Rust 更新日志 #149](https://intellij-rust.github.io/2021/06/21/changelog-149.html)
* [rustymind - 使用 Rust 对脑电波（brainwaves）进行解析和可视化](https://github.com/junjunjd/rustymind)（译注：rustymind 是 Rust 在医疗硬件方向应用的一个库，主要适用于头戴式脑电仪 NeuroSky MindWave EEG）
* [TensorBase 周报 8 期](https://tensorbase.io/thisweek/2021-06-23-tw_8/)
* [支持 Miguel Ojeda 使用 Rust 开发 Linux 内核的工作](https://www.memorysafety.org/blog/supporting-miguel-ojeda-rust-in-linux/)（译注：Miguel Ojeda 曾编写过大型强子对撞机粒子加速器所使用的软件，并从事过编程语言安全方面的工作。2021 年 6 月中旬，Google 与 Miguel 签订了一年的合约，希望他来提高 Linux 内核的内存安全。Miguel Ojeda 将使用 Rust 来进行 Linux 内核的开发，这也是 Linux 内核中将首次出现 Rust 代码）
* [rustc_codegen_gcc：进展报告 #1](https://blog.antoyo.xyz/rustc_codegen_gcc-progress-report-1)

### 观测/思考
* [以“Java 教程（The Java Tutorials）”的方式学习 Rust - 封装的 trait 对象和继承（inheritance）](https://rust-java-tutorials.netlify.app/blog/5-trait-objects-2/)（译注：主要是 `dyn`、`Box<T>`，以及 trait 的实现 `impl` 方面的内容。这是一个系列，参考 6 月 9 日 394 期周报）
* [WABT：wasm 开发中好用的 CLI 工具包](https://blog.knoldus.com/wabt-a-wonderful-cli-for-manipulating-wasm/)（译注：C++ 语言开发，功能很全，包括对 `simd` 和多线程的支持。目前已有 Rust 的绑定库。但此文与 Rust 没关系，或许是 wasm-binden 与之关联紧密的原因吧）
* [wasm-bindgen 使得 Rust 和 JavaScript 的交互变得容易](https://blog.knoldus.com/wasm-bindgen-making-rust-and-javascript-interoperability-easy/)（译注：使用 Rust 构建 wasm 应用必不可少的库，可参阅[《Rust 和 Wasm 的融合，使用 yew 构建 web 前端》](https://blog.budshome.com/budshome/rust-he-wasm-de-rong-he-,shi-yong-yew-gou-jian-webassembly-biao-zhun-de-web-qian-duan-(1)--qi-bu-ji-crate-xuan-ze)）
* [Rust 中的类型检查（type-checked）库 keypaths](https://www.cmyr.net/blog/keypaths.html)（译注：swift 风格的 keypaths 库）
* [使异步（async）Rust 更易于使用的方法探讨](https://carllerche.com/2021/06/17/six-ways-to-make-async-rust-easier/)
* [重读你所编写的 Rust 代码](https://www.morsecodist.io/blog/rust-writer-ownership)
* [Rust 项目初体验：一个国际象棋引擎](https://www.reddit.com/r/rust/comments/o3k6yu/first_rust_project_a_chess_engine/)
* [游戏发开中，比较 Rust 和 C++](https://blog.logrocket.com/rust-vs-c-for-game-development/)
* [Rust 中的 Skipping Tests](https://plume.benboeckel.net/~/JustAnotherBlog/skipping-tests-in-rust)
* [中文] [使用 Rust 开发 Gameboy 模拟器](https://yodalee.me/2020/12/2020_rust_gameboy/)（译注：繁体中文）
* [视频] [为什么“云”的未来将会基于 Rust - Oliver Gould, Buoyant](https://youtu.be/BWL4889RKhU)

### Rust 演练
* [Rust 和 AWS Lambda](https://mitchgollub.com/rust-and-aws-lambda/)
* [Rust 中对二进制数据反序列化](https://adventures.michaelfbryan.com/posts/deserializing-binary-data-files/)
* [又一个新潮的（snazzy) Rust CLI](https://dev.to/jeikabu/yet-another-snazzy-rust-cli-k4i)
* [Rust 中构建 API（2）](https://dev.to/naruhodo/build-an-api-in-rust-part-2-f11)
* [Rust 中的多态（polymorphism）](https://oswalt.dev/2021/06/polymorphism-in-rust/)
* [Rust 中使用 MongoDB 和 Redis 的入门教程](https://romankudryashov.com/blog/2021/06/mongodb-redis-rust/)
* [网站开发（1）：树莓派上的监控应用](https://www.rotoclone.zone/blog/posts/raspberry-pi-monitoring)
* [中文] [使用 Rust 开发 WebAssembly 程序](https://yodalee.me/2021/05/1helloworld/)（译注：繁体中文）
* [视频] [Rust 模糊测试（fuzzing）#3：如何编写（更好的）Rust fuzz 测试目标？](https://youtu.be/MiDFvrqjM2E)
* [视频] [使用 Rust 构建 web 应用（3）- 数据库管理](https://youtu.be/u-bjMHQ22TI)
* [视频] [使用 Rust 构建 web 应用（4）- HTTP 服务器](https://youtu.be/rJB0PLwipRI)

### 其它
* [Rust 组织不是一个公司](https://blog.m-ou.se/rust-is-not-a-company/)
* [Google 希望在 Linux 内核中出现 Rust 代码，已与开发人员签订合同](https://www.phoronix.com/scan.php?page=news_item&px=Google-Wants-Rust-In-Kernel)（译注：开发人员即 Miguel Ojeda，参阅上文[支持 Miguel Ojeda 使用 Rust 开发 Linux 内核的工作](https://www.memorysafety.org/blog/supporting-miguel-ojeda-rust-in-linux/)）
* [Rust 是 Godot 游戏引擎开发者最想要的语言](https://www.reddit.com/r/rust/comments/o5p267/rust_is_the_most_wanted_language_by_godot_engine/)（译注：Godot 是由社区开发的一款二维和三维跨平台、开源的游戏引擎）

## 周最佳 crate

本周最佳 crate 是 [serde-encrypt](https://github.com/laysakura/serde-encrypt)，用于向所有 `Serialize` 实现添加加密（encryption）特性的库。

谢谢 [Sho Nakatani](https://users.rust-lang.org/t/crate-of-the-week/2704/926) 的提议。

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

## 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

* [cargo - SearchIndexer takes time indexing \target on windows](https://github.com/rust-lang/cargo/issues/8694)
* [cargo - Ability to specify the output name for a bin target different from the crate name](https://github.com/rust-lang/cargo/issues/1706)
* [cargo - Using alternative registries names in text output](https://github.com/rust-lang/cargo/issues/6691)
* [cargo - A dependency on path = "." should have a good error message](https://github.com/rust-lang/cargo/issues/9518)

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Rust 核心更新

[301 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-06-07..2021-06-14

## Rust 编译器性能

在一些较小的基准测试（如 helloworld）上有一些小回归，或许在少数情况下会出现较多的 IR。

验测工作是由 **@simulacrum**完成的。修正范围：[d192c80..3912083](https://perf.rust-lang.org/?start=d192c80d2284ba6b5146bb3da586354c3762c72b&end=3912083821c5072f700a75589c8af6a9d3e20a21&absolute=false&stat=instructions%3Au)

[此处可查阅完整报告](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-06-22.md).

### 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

* [Type-changing struct update syntax](https://github.com/rust-lang/rfcs/pull/2528)

### 新的 RFCs

* [Stabilize Cargo's weak-dep-features and namespaced-features.](https://github.com/rust-lang/rfcs/pull/3143)

## 近期活动

### 线上

* [June 24, 2021, Berlin, DE - Rust Hack and Learn - Berline.rs](https://berline.rs/)
* [June 29, 2021, Dallas, TX, US - Last Tuesday - Dallas Rust](https://www.meetup.com/Dallas-Rust/events/jqxqwryccjbmc/)
* [July 6, 2021, Buffalo, NY, US - Buffalo Rust User Group, First Tuesdays - Buffalo Rust Meetup](https://www.meetup.com/Buffalo-Rust-Meetup/events/jxfdjsycckbjb/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

## Rust 招聘信息

**ChainSafe Systems**

* [Rust Developer (Remote)](https://jobs.smartrecruiters.com/ChainSafeSystemsInc/743999739358248-rust-developer)

**Kollider**

* [Junior Backend Engineer (Remote)](https://kollider.homerun.co/junior-backend-engineer/en)
* [Senior Backend Engineer (Remote)](https://kollider.homerun.co/senior-backend-engineer/en)
* [DevOps Engineer (Remote)](https://kollider.homerun.co/devops-engineer/en)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

# 本周引语

> 终于，我可以恰当地命名我的不安全（unsafe）函数了。
>
> `unsafe fn e͙̤͎̪͒x̲͓̞̤͍̻̺̂͗͛͆͡t̜̣͊̓ͩ̍̑e̩͖͙͎̼̖͉ͮṇ̨͖̎̓ͅd̗̼͕ͫ̅_̲̦̥̙̙͍͂́l͙͙̦̞̠̃͌͒i̹̘͍̳̊ͪͦͤ͒̊͋f̨ͥ̄̌ḛ̜͗̉̃̎̂̔̐t̩̲̘͕͉̺̫̓͗́i̹̤̭ͭ͆̔ͪͤ͢m̹̤̜̗̫̩͍ͨe̝͒ͣ<'b>(r: R<'b>) -> R<'static>`

– [Freeky 发表于 r/rust](https://www.reddit.com/r/rust/comments/o1yy1p/announcing_rust_1530/h2488f5)

谢谢 [Vincent de Phily](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1063) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
