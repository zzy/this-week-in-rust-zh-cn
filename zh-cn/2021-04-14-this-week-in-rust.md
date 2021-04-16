# Rust 官方周报 386 期（2021-04-14）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。 


大家好，欢迎查阅第 386 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一种系统语言，主要追求三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

# Rust 社区更新

本周无论文或研究探讨。

### 官方
* [头脑风暴进行中：Async Rust 的未来熠熠生辉 ](https://blog.budshome.com/budshome/tou-nao-feng-bao-jin-xing-zhong-:async-rust-de-wei-lai-yi-yi-sheng-hui)
* [Rust 基金会] [成员介绍：Florian Gilcher](https://foundation.rust-lang.org/posts/2021-04-08-introducing-florian-gilcher/)（译注：Rust 核心团队，项目主管）
* [Rust 基金会] [成员介绍：侯培新](https://foundation.rust-lang.org/posts/2021-04-08-introducing-peixin-hou/)（译注：董事成员，华为开源软件与系统首席架构师）

### 简讯
* [Rust 游戏开发月报 #20 - 2021 年 3 月](https://gamedev.rs/news/020/)（译注：游戏很棒，推荐大家去看看，如下笔者随意取了一张图）

![Rust veloren game](https://blog.budshome.com/static/articles/1618536523.jpg)

### 项目/工具 更新
* [基于 Cranelift 的 rustc 代码生成后端（rustc_codegen_cranelift）进展报告（2021 年 4 月）](https://bjorn3.github.io/2021/04/13/progress-report-april-2021.html)
* [IntelliJ Rust：2021.1 更新版发布](https://blog.jetbrains.com/rust/2021/04/08/intellij-rust-updates-for-2021-1/)
* [IntelliJ Rust 更新日志 #145](https://intellij-rust.github.io/2021/04/12/changelog-145.html)
* [rust-analyzer 更新日志 #72](https://rust-analyzer.github.io/thisweek/2021/04/12/changelog-72.html)
* [Ballista 项目已被捐赠给了 Apache Arrow 项目组](https://www.reddit.com/r/rust/comments/mo63t3/ballista_has_been_donated_to_the_apache_arrow/)（译注：Ballista 项目是 Rust 开发的类似 Spark 的分布式计算平台，笔者已经在使用中。其还支持  Python、C++，以及 Java 等语言，且不用为序列化付出额外开销代价）

### 观测/思考
* [Rust 用于生产环境：MeiliSearch](https://serokell.io/blog/rust-in-production-meilisearch)
* [Rust 是为专业人士准备的](https://gregoryszorc.com/blog/2021/04/13/rust-is-for-professionals/)
* [Rust 语言中，让异步函数和同步函数匹配，不是什么大问题](https://morestina.net/blog/1686/rust-async-is-colored)（译注：原标题使用了 `Rust async is colored`，这个 `colored` 源自 JavaScript，比喻 JavaScript 和其它语言中，同步函数和异步函数那些令人痛苦的不匹配难题）
* [使用 Rust 进行科学计算：从经验中学习总结](https://blog.esciencecenter.nl/using-rust-for-scientific-numerical-applications-learning-from-past-experiences-798665d9f9f0)
* [PlaintDB - 新的里程碑](https://dev.to/ecton/plaintdb-serves-another-milestone-reached-kl3)（译注：作者很有信心，计划用 PlaintDB 取代 PostgreSQL 和 Redis）
* [为什么应将 Rust 用于机器人平台？](https://dev.to/tangramvision/why-rust-for-robots-4nmd)
* [nalgebra 0.26 中整合常量泛型（const-generics）的实践](https://www.dimforge.com/blog/2021/04/12/integrating-const-generics-to-nalgebra/)（nalgebra 是 Rust 实现的线性代数库）
* [播客] [使用 Rust 进行构建：Tim McNamara 讲解《Rust in Action》](https://anchor.fm/building-with-rust/episodes/Building-with-Rust-Tim-McNamara-on-Rust-in-Action-eugoal/a-a1ptlh) [[文字实录]](https://github.com/seanchen1991/building-with-rust/blob/main/transcripts/002.md)

### Rust 演练
* [使用 `Ockam` crate，逐步构建端对端（End-to-End）的加密信息传输应用](https://github.com/ockam-network/ockam/tree/develop/documentation/guides/rust/get-started#readme)（译注：`Ockam` 是一个主要用于物联网设备间通信的库，端到端加密、相互认证通信等）
* [`easy-cast` 库介绍](https://kas-gui.github.io/blog/easy-cast.html)（译注：`easy-cast` 是一个类型转换方面的辅助库，可以用来替代 `as i32`，`u32::` 这类写法。笔者体验了，挺方便）
* [为什么 Rust 中的字符串（strings）使用体验不好（hard）](https://www.brandons.me/blog/why-rust-strings-seem-hard)
* [Rust 技巧：返回多态性类型](https://loige.co/rust-shenanigans-return-type-polymorphism/)（译注：即返回泛化类型，泛型）
* [使用 Rust 开发 Neovim 编辑器插件（plugins)](https://blog.usejournal.com/a-detailed-guide-to-writing-your-first-neovim-plugin-in-rust-a81604c606b1)
* [Rust 中的零开销（zero-overhead）链表](https://aloso.github.io/2021/04/12/linked-list.html)（译注：推荐阅读）
* [将 Rust 整合到 Python 中](https://www.vortexa.com/insight/integrating-rust-into-python)（译注：是上次使用 300 行左右 Rust 代码极致提升 Python 性能的公司，请参阅《[使用 Rust 极致提升 Python 性能：图表和绘图提升 24 倍，数据计算提升 10 倍](https://blog.budshome.com/budshome/shi-yong-rust-ji-zhi-ti-sheng-python-xing-neng-:tu-biao-he-hui-tu-ti-sheng-24-bei-,shu-ju-ji-suan-ti-sheng-10-bei)》）
* [使用 `Tonic` 建立 `gRPC Protobuf` 服务器](https://dev.to/transienterror/setting-up-a-grpc-protobuf-server-with-tonic-218e)（译注：`Tonic` 是基于 `HTTP/2` 的 gRPC 服务实现，关注高性能、互操作性和灵活性。笔者正打算项目中选择一个 gRPC 服务实现库，也看了这个项目，此项目几年没发新版本了……）
* [用 Rust 做 Kafka 开发（2）](https://dev.to/abhirockzz/getting-started-with-kafka-and-rust-part-2-354f)
* [Rust lib 错误管理，多枚举方式](http://www.tglman.com/posts/rust_lib_error_management.html)
* [Rust 中的异步数据流（2）——撤销过期请求](https://gendignoux.com/blog/2021/04/08/rust-async-streams-futures-part2.html)
* [系列] [可爱的 Warp：使用 Rust 开发 REST API](https://dev.to/rogertorres/series/12179)
* [中文] [系列] [基于 Async Rust 构建 GraphQL 服务，使用 tide + async-graphql + mongodb（1）](https://blog.budshome.com/budshome/gou-jian-rust-yi-bu-graphql-fu-wu-:ji-yu-tide-+-async-graphql-+-mongodb(1)--qi-bu-ji-crate-xuan-ze)（注：笔者的博文，官方周报同意收录，不是翻译中夹带私货哈）
* [视频] [使用 Rust 开发 Flocking Boids 游戏的实践和比较：Piston vs Tetra vs Amethyst vs Bevy](https://youtu.be/e0n9v565HR4)（译注：后面比较的都是游戏引擎，所以推断 Flocking Boids 应该是个游戏名字，如果不对请你指导）

### 其它
* [Rust，并非 Firefox，而是 Mozilla 对业界的最伟大奉献](https://www.techrepublic.com/article/rust-not-firefox-is-mozillas-greatest-industry-contribution/)
* [来自 AWS 的人员 Shane Miller将领导新的 Rust 基金会](https://www.zdnet.com/article/awss-shane-miller-to-head-the-newly-created-rust-foundation/)
* [[RFC] 将 Rust 引入 Linux 内核的讨论](https://lkml.org/lkml/2021/4/14/1023)（译注：实际是一个邮件记录，如果有朋友有兴趣翻译，希望可以也发我一份，在公众号发布）
* [LLVM 窥探 - `clamp` 实现的比较分析](https://secret.club/2021/04/09/std-clamp.html)
* [`Tokio-uring` 设计方案](https://www.reddit.com/r/rust/comments/mmz1sg/tokiouring_design_proposal/)
* [Google 使用 Rust 开发 Android 底层（low-level Android）](https://arstechnica.com/gadgets/2021/04/google-is-now-writing-low-level-android-code-in-rust/)
* [Linux 内核中的 Rust](https://security.googleblog.com/2021/04/rust-in-linux-kernel.html)

# 周最佳 crate

本周最佳 crate 是 [dipa](https://docs.rs/dipa)，Rust 数据结构中用于派生（derive）差分/增量编码（delta-encoding）的 crate。

即使缺少提名，但 llogiq（译注：周报编辑人员之一）对自己的选择非常满意。

[关于下周最佳 crate，请您提议，并投票!][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Rust 核心更新

[329 PR 在上一周被合并][merged]。

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-04-05..2021-04-12

## Rust 编译器性能

本周稍显安静。

验测工作是由 **@simulacrum** 完成的。修正范围：[d322385..5258a74](https://perf.rust-lang.org/?start=d32238532138485c80db4f2cd596372bce214e00&end=5258a74c887f8ae14717e1f98b652b470877ce4e&absolute=false&stat=instructions%3Au)

## 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

* [RFC: -C export-executable-symbols](https://github.com/rust-lang/rfcs/pull/2841)

## 新的 RFCs

* [枚举上的 `#[derive(Default)]` 具有 `#[default]` 属性（attribute） #3107](https://github.com/rust-lang/rfcs/pull/3107)
* [新增：值的宏捕获标识符（value macro capture designator）](https://github.com/rust-lang/rfcs/pull/3106)

# 近期活动

### 线上活动
* [April 20, Washington, DC, US - 深入探讨 Rust 的接用检查器 - Rust DC](https://www.meetup.com/RustDC/events/ntvrgsyccgblb)
* [April 21, Vancouver, BC, CA - Rust 的研讨/Hack/闲逛 之夜 - Vancouver Rust](https://www.meetup.com/Vancouver-Rust/events/npqfbsyccgbcc/)
* [April 27, Dallas, TX, US - Last Tuesday - Dallas Rust](https://www.meetup.com/Dallas-Rust/events/jqxqwryccgbkc/)

### 北美
* [April 14, Atlanta, GA, US - 和 Rustaceans 一起畅饮啤酒 - Rust Atlanta](https://www.meetup.com/Rust-ATL/events/qxqdgryccgbsb/)

### 亚太
* [April 19, Wellington, NZ - IGNITION: 什么是 Rust，以及我为什么要关注它？工作和游戏中的 Rust - Rust Wellington](https://www.meetup.com/Rust-Wellington/events/277270667)

### 欧洲
* [April 21, Moscow, RU -月度会议 - Rust Moscow](https://www.meetup.com/ru-RU/Rust-%D0%B2-%D0%9C%D0%BE%D1%81%D0%BA%D0%B2%D0%B5/events/277259838/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust 招聘信息

**Slight**

* [**远程** Rust 软件工程师 - 核心团队](https://www.slight.co/jobs/software-engineer-core)

**Kraken**

* [若干**远程** Rust 工程师岗位](https://jobs.lever.co/kraken?team=Engineering)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

# 本周引语

> 每天，我在 \[rust is\] 中真正看重的是：我可以放心调用其他人的代码，而不产生令人不快的“惊喜”。
> ```
> async fn verify_signature(token: &Jwt) -> Result<Claims, VerificationError>
> ```
>
> 代码段中：
>
> * 我知道我的 JWT 令牌（token）不会被更改，仅能被访问（`&`）；
> * 我晓得函数可以异步 I/O（`async`）；
> * 我明白函数失败原因（`Result`）；
> * 我了解它的故障模式（`VerificationError`）。

– [Luca Palmieri 发表于 Twitter](https://twitter.com/algo_luca/status/1380928103019597827)（译注：*Zero to Production in Rust* 一书的作者）

谢谢 [Nixon Enraght-Moony](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1031) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman).*

谢谢您的阅读！

---
