# Rust 官方周报 385 期（2021-04-07）

大家好，欢迎查阅第 385 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一种系统语言，主要追求三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

# Rust 社区更新

本周无论文或研究探讨。

### 官方
* [内部] [Rust 核心团队人员变动](https://blog.budshome.com/budshome/-(2021-04-03)--rust-he-xin-tuan-dui-ren-yuan-bian-dong)
* [Rust 基金会] [成员介绍：侯培新](https://foundation.rust-lang.org/posts/2021-04-08-introducing-peixin-hou/)（译注：董事成员，华为开源软件与系统首席架构师）
* [Rust 基金会] [成员介绍：Florian Gilcher](https://foundation.rust-lang.org/posts/2021-04-08-introducing-florian-gilcher/)（译注：Rust 核心团队，项目主管）

### 简讯
* [Rust OSDev 2021 年 3 月简讯](https://rust-osdev.com/this-month/2021-03/)
* [RiB 简讯 #22](https://www.reddit.com/r/rust/comments/mhmfu9/rib_newsletter_22_a_few_tweaks/)

### 项目/工具 更新
* [GCC Rust 月报 #4 2021-03](https://thephilbert.io/2021/04/02/gcc-rust-monthly-report-4-march-2021/)
* [mrustc 升级：支持 rustc 1.39.0](https://www.reddit.com/r/rust/comments/mjxbaz/mrustc_upgrade_rustc_1390/)（译注：1、mrustc 是一个 Rust 编译器的替代实现；2、目前官方 rustc 版本为 1.51.0）
* [rust-analyzer 更新日志 #71](https://rust-analyzer.github.io/thisweek/2021/04/05/changelog-71.html)
* [Rust 中新的左递归 PEG 解析生成器](https://www.mess.org/2021/03/26/Left-Recursive-PEG-Parser-Generator/)
* [Flott（Rust 中的运动控制工具包）月报 - 2021-04](https://flott-motion.org/news/last-month-in-flott-april-2021/)（译注：前景不错的新包，但 github 星星仅 3 个）
* [IntelliJ Rust 更新信息](https://blog.jetbrains.com/rust/2021/04/08/intellij-rust-updates-for-2021-1/)
* [Bevy 0.5](https://bevyengine.org/news/bevy-0-5/)（译注：数据驱动的游戏引擎）

### 观测/思考
* [将低层次 actor 模型系统与 Rust async/await 结合（1）](https://uazu.github.io/blog/20210406.html)
* [Rust GC 设计中的安全追踪之旅](https://manishearth.github.io/blog/2021/04/05/a-tour-of-safe-tracing-gc-designs-in-rust/)（译注：此作者用 Rust 设计和实现了 GC 库，被集成在 Servo 浏览器，主要为 JS 层应用）
* [使用 Rust + Lunatic 构建具备 WebAssembly 的 TelNet 聊天服务器](https://www.hackernoon.com/how-i-used-rust-lunatic-to-build-a-telnet-chat-server-with-webassembly-rb3l33cg)
* [Firefox 中消除数据竞争 - 技术报告](https://hacks.mozilla.org/2021/04/eliminating-data-races-in-firefox-a-technical-report/)
* [一级（first-class）IO](https://blog.sunfishcode.online/first-class-io/)（译注：一级（first-class）IO，即执行 I/O 的函数，可作为参数或返回值在程序中传递，如 `File`。或许 first-class 不翻更好理解）
* [当前程序打包发布人的安全噩梦](https://blogs.gentoo.org/mgorny/2021/02/19/the-modern-packagers-security-nightmare/)
* [对请求排序，以加速 I/O](https://pkolaczk.github.io/disk-access-ordering/)
* [关于 Rust 中已检查异常（checked exception）的短文](https://users.rust-lang.org/t/an-essay-of-checked-exceptions-in-rust/57769)
* [离奇的架构设计，从开始就不要支持](https://blog.yossarian.net/2021/02/28/Weird-architectures-werent-supported-to-begin-with)
* [视频] [7 天内学会 Rust OpenGL](https://youtu.be/KEQIWqSq42k)

### Rust 演练
* [以 Rust 为主，构建 Python 客户端](https://www.fluvio.io/blog/2021/03/python-client/)
* [Rust 图形用户界面库 KAS 的简单实例](https://kas-gui.github.io/tutorials/hello.html)（译注：文章特短，推荐对 GUI 开发感兴趣的朋友阅读）
* [如何创建最精简的 Rust Docker 镜像](https://kerkour.com/blog/rust-small-docker-image/)
* [使用 Rust 自定义（Oxidizing）Kubernetes 算子](https://www.pavel.cool/rust/rust-kubernetes-operators/)
* [从 Node.js 向 Rust 传递元组（tuple）数据，并返回运算结果](https://www.fluvio.io/blog/2021/04/node-bindgen-tuples/)
* [用 Rust 做 Kafka 开发（1）](https://dev.to/abhirockzz/getting-started-with-kafka-and-rust-part-1-4hkb)
* [Rust 初学者的错误处理指南](https://dev.to/seanchen1991/a-beginner-s-guide-to-handling-errors-in-rust-40k2)
* [使用 Seahorn 验证 Rust 程序](https://project-oak.github.io/rust-verification-tools/using-seahorn/)
* [Rust 中的异步数据流（1）——Futures、缓冲处理（buffering），以及难解的编译错误](https://gendignoux.com/blog/2021/04/01/rust-async-streams-futures-part1.html)
* [系列] [如果 SQLite 是用 Rust 开发的，会是什么样子？（3）](https://medium.com/the-polyglot-programmer/what-would-sqlite-look-like-if-written-in-rust-part-3-edd2eefda473)
* [视频] [Rust 中的函数返回值](https://www.youtube.com/watch?v=YNSg7g46Hso)
* [视频] [Rust 中的 Crust：原子计算和内存排序](https://youtu.be/rMGWeSjctlY)（译注：crust 是 Rust 生态中的低层次网络库，用于优化对等连接和数据传输）
* [视频] [Rust 中的 Async/Await：简介](https://youtu.be/FNcXf-4CLH0)
* [视频] [OpenVehicleDiag Rust 编码直播](https://youtu.be/zjAe-uvKMJ4)
* [视频] [系列] [易学易用 Rust——用简洁的英文进行 Rust 编程](https://youtube.com/playlist?list=PLfllocyHVgsRwLkTAhG0E-2QxCf-ozBkk)

### 其它
* [best-of-ml-rust：Rust 机器学习库列表](https://github.com/e-tony/best-of-ml-rust)
* [Rust 在 Android 平台的近况： Android 团队宣布 Android 开源项目（AOSP），已支持 Rust 语言来开发 Android 系统本身](https://blog.budshome.com/budshome/android-tuan-dui-xuan-bu-android-kai-yuan-xiang-mu-(aosp),yi-zhi-chi-rust-yu-yan-lai-kai-fa-android-xi-tong-ben-shen)
* [致谢 David Tolnay](https://www.reddit.com/r/rust/comments/mify2o/david_tolnay_thank_you/)
* [我的“美好未来”](https://smallcultfollowing.com/babysteps/blog/2021/04/02/my-shiny-future/)（译注：即[【2021-04-03】Rust 核心团队人员变动](https://blog.budshome.com/budshome/-(2021-04-03)--rust-he-xin-tuan-dui-ren-yuan-bian-dong)文中所述：Niko Matsakis 正在逐步退出 Rust 核心团队，他将集中精力带领 Rust 语言团队。为此，Niko Matsakis 发表了此篇博文）

# 周最佳 crate

本周最佳 crate 是 [rs-pbrt](https://crates.io/crates/rs_pbrt)，PBRT 图书（第三版）中 C++ 部分代码的对应 Rust 实现。

谢谢 [Jan Walter](https://users.rust-lang.org/t/crate-of-the-week/2704/900) 的提议！

[关于下周最佳 crate，请您提议，并投票!][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

* [dotenv-linter 有些优先级较高的 issues](https://github.com/dotenv-linter/dotenv-linter/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Rust 核心更新

[313 PR 在上一周被合并][merged]。

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-03-29..2021-04-05

## Rust 编译器性能

对于[内存使用的改进][memory usage improvements]来说，本周颇为重要。因为默认分配器（allocator，升级到了最新的 jemalloc）的更新，发布构建（cargo build --release）的内存使用率，平均提高了约 20%；而检测构建（cargo check）则大约提升内存使用率为 5%。

验测工作是由 **@simulacrum** 完成的。修正范围：[4896450e..d32238](https://perf.rust-lang.org/?start=4896450e7e0a522486b4d3a8d360ac4e1d2072a0&end=d32238532138485c80db4f2cd596372bce214e00&absolute=false&stat=instructions%3Au)

[memory usage improvements]: https://perf.rust-lang.org/?start=4896450e7e0a522486b4d3a8d360ac4e1d2072a0&end=d32238532138485c80db4f2cd596372bce214e00&absolute=false&stat=max-rss

## 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

* [RFC：声明宏的原变量表达式（Declarative macro metavariable expressions）](https://github.com/rust-lang/rfcs/pull/3086)

## 新的 RFCs

* [RFC：预留 2021 版代号（Reserved prefixes in the 2021 edition）](https://github.com/rust-lang/rfcs/pull/3101)（译注：即 `Cargo.toml` 中的设置 `edition = "2018"`）

# 近期活动

### 线上活动
* [April 7, Johannesburg, ZA - Monthly Joburg Rust Chat! - Johannesburg Rust Meetup](https://www.meetup.com/Johannesburg-Rust-Meetup/events/277133126/)
* [April 7, Indianapolis, IN, US - Indy.rs - with Social Distancing - Indy Rust](https://www.meetup.com/indyrs/events/jhfstryccgbkb/)
* [April 12, Denver, CO, US - Building Delightful CLI Tools in Rust by Chuck Pierce - Rust Denver](https://www.meetup.com/Rust-Boulder-Denver/events/276801410/)
* [April 13, Seattle, WA, US - Monthly Meetup - Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksryccgbrb/)
* [April 13, Saarbrücken, Saarland, DE - **Rust Saar** 10u16](https://www.meetup.com/de-DE/Rust-Saar/events/276873622/)
* [April 20, Washington, DC, US - The Rust Borrow Checker—A Deep Dive - Rust DC](https://www.meetup.com/RustDC/events/ntvrgsyccgblb)

### 北美

* [April 8, Columbus, OH, US - Monthly Meetup - Columbus Rust Society](https://www.meetup.com/columbus-rs/events/dpkhgryccgblb/)
* [April 14, Atlanta, GA, US - Grab a beer with fellow Rustaceans - Rust Atlanta](https://www.meetup.com/Rust-ATL/events/qxqdgryccgbsb/)

### 亚太
* [April 19, Wellington, NZ - IGNITION: What is Rust and why should I care? Rust at work & at play - Rust Wellington](https://www.meetup.com/Rust-Wellington/events/277270667)

# Rust 招聘信息

**IOTA Foundation**

* [IOTA Identity Software Engineer - Rust (Remote)](https://iota.bamboohr.com/jobs/view.php?id=143&source=other)

**Parity Technologies**

* [Blockchain Developer - Cross Chain Messaging (Remote)](https://grnh.se/9aec49883us)
* [Numerous other Rust engineering openings](https://www.parity.io/jobs/)

**Microsoft**

* [Azure IoT Senior Software Engineer (remote possible within U.S.)](https://careers.microsoft.com/us/en/job/960784/Senior-Software-Engineer)
    * Junior developers should also apply but relocation to Redmond is necessary in that case.

**Wallaroo**

* [Software Engineer (Remote)](https://wallaroo.breezy.hr/p/30939dc4e5c7-software-engineer)

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# 本周引语

很遗憾，本周没有“引语”提议。

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman).*

谢谢您的阅读！

---
