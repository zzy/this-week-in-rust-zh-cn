# Rust 官方周报 388 期（2021-04-28）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。 

大家好，欢迎查阅第 388 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

# Rust 社区更新

本周无论文或研究探讨。

### 官方
* [Rustup 1.24.0 已官宣发布，及其新特性详述 ](https://blog.budshome.com/budshome/rustup-1.24.0-yi-guan-xuan-fa-bu-,ji-qi-xin-te-xing-xiang-shu)
* [内部] [Rust 编译器团队对成员 Aaron Hill 的祝贺](https://blog.budshome.com/budshome/rust-bian-yi-qi-tuan-dui-dui-cheng-yuan-aaron-hill-de-zhu-he)
* [基金会] [成员介绍：Josh Stone](https://foundation.rust-lang.org/posts/2021-04-22-introducing-josh-stone/)（译注：项目主管，质量团队）
* [Foundation] [成员介绍：Lars Bergstrom](https://foundation.rust-lang.org/posts/2021-04-22-introducing-lars-bergstrom/)（译注：董事成员，谷歌）

### 简讯

### 项目/工具更新
* [rust-analyzer 更新日志 #74](https://rust-analyzer.github.io/thisweek/2021/04/26/changelog-74.html)
* [IntelliJ Rust 更新 #146](https://intellij-rust.github.io/2021/04/26/changelog-146.html)
* [Lemmy 发布 v0.11.0 版](https://lemmy.ml/post/61856)（译注：`lemmy` 是 Rust 技术栈为主实现的，类似于 `Reddit`、`Lobste.rs`，或 `Hacker News`）
* [simdutf v0.1.1 - 语义版本的一小步，性能提升的一大步](https://www.reddit.com/r/rust/comments/mz44xi/simdutf_v011_a_small_step_for_semver_one_giant/)（译注：基于 simdjson 的实现，simd 加速和 UTF8 验证）
* [好玩有趣的 itch.io 线上益智游戏，适用于 Windows 和 Linux，界面外观精美。感谢 Rust 社区，创造了了如此棒的语言和生态工具](https://www.reddit.com/r/rust/comments/mx3enm/the_playable_demo_of_outer_wonders_our_cute/)

### 观测/思考
* [基于 evcxr 的 Rust 交互式笔记本（notebook）：David Lattimore 访谈](https://blog.abor.dev/p/evcxr)（译注：`evcxr` 是 `eval()` 的 Rust 实现，David Lattimore 是 Rust Jupyter 的核心创造者。Rust Jupyter 开源在谷歌公司仓库）
* [Rust 中的迭代器（iterator）及零成本抽象（Zero Cost Abstractions）的开销](https://github.com/mike-barber/rust-zero-cost-abstractions/blob/main/README.md)（附带视频，译注：此文和 C#、Java 语言做了比较，值得一读）
* [Rust 中移动（move）构造函数（constructor）：有可能吗？](https://mcyoung.xyz/2021/04/26/move-ctors/)（译注：要用到 `unsafe`，值得一读）
* [basedrop：Rust 生态中，适用于实时音频的垃圾收集器](https://blog.budshome.com/budshome/basedrop:rust-sheng-tai-zhong-,gua-yong-yu-shi-shi-yin-pin-de-la-ji-shou-ji-qi)
* [TurboWish 路线规划（1）：目标](http://blog.pnkfx.org/blog/2021/04/26/road-to-turbowish-part-1-goals/)（译注：嗯，名字很吸引人，但爪子？目前只是 crate 名字的占位符，大家还需期待）
* [TurboWish 路线规划（2）：功能特性](http://blog.pnkfx.org/blog/2021/04/27/road-to-turbowish-part-2-stories/)（译注：同上，作者的规划和思考）
* [Rust 中路径解析的痛点](https://www.fpcomplete.com/blog/pains-path-parsing/)（译注：篇幅不长的好文，关于网络路径及其疯狂的百分比编码，此文推荐一读）
* [若果今天你可以重新设计 Rust，你会做哪些改变？](https://www.reddit.com/r/rust/comments/my3ipa/if_you_could_redesign_rust_from_scratch_today/)（译注：讨论火热，大部分是其它语言而来的惯性）
* [实际上，“红色”函数和“蓝色”函数都是合理的](https://blainehansen.me/post/red-blue-functions-are-actually-good/)（译注：红色/蓝色函数象征同步/异步函数，函数的`颜色（colored）`源自 JavaScript，比喻 JavaScript 和其它语言中，同步函数和异步函数那些令人痛苦的不匹配难题。本文是对上期文章《[Rust 语言中，让异步函数和同步函数匹配，不是什么大问题](https://blog.budshome.com/budshome/rust-guan-fang-zhou-bao-386-qi-(2021-04-14))》的回应）

### Rust 演练
* [Rust 中，使用 BBS+ 创建隐私保护（privacy-preserving）签名](https://github.com/ockam-network/ockam/blob/develop/implementations/rust/ockam/signature_bbs_plus/GUIDE.md)
* [午夜忏悔（Late Night Confessions） — 使用 Rust、Rocket、Diese，以及 Askama 进行站点构建（2）](https://medium.com/perimeterx/late-night-confessions-building-a-website-using-rust-rocket-diesel-and-askama-part-2-fc87c463e8f3)（译注：站点名本无需翻译，但这个站名象电影名字，不由得手痒 ;-)）
* [如何在 Rust 中自定义测试套件（Test Harness）](https://www.fluvio.io/blog/2021/04/rust-custom-test-harness/)
* [Rust 生态中的 gRPC 介绍](https://romankudryashov.com/blog/2021/04/grpc-rust/)
* [Rust 中，打印格式化（Pretty Printer）的 Postgres SQL（2）](v)
* [系列] [Rust 旅程](https://dev.to/basman/series/12170)
* [中文] [系列] [基于 Async Rust 构建 GraphQL 服务，使用 tide + async-graphql + mongodb（2）](https://blog.budshome.com/budshome/gou-jian-rust-yi-bu-graphql-fu-wu-:ji-yu-tide-+-async-graphql-+-mongodb(2)--cha-xun-fu-wu)
* [中文] [系列] [基于 actix-web + async-graphql + rbatis + postgresql / mysql 构建异步 Rust GraphQL 服务（1）](https://blog.budshome.com/budshome/ji-yu-actix-web-+-async-graphql-+-rbatis-+-postgresql---mysql-gou-jian-yi-bu-rust-graphql-fu-wu---qi-bu-ji-crate-xuan-ze)
* [视频] [Rust 是什么？为什么说 Rust 很重要？](https://youtu.be/kdv1EBk6Xgc)
* [视频] [Rust 中使用 `Iterator::colect`](https://youtu.be/ECwy6s_h7T8)
* [视频] [RustConf 2020 - jam1garner 开发的更具生产力/更高效的宏（Macros）](https://youtu.be/HN6EUcnGN1s)

### 论文/研究探讨
* [嵌入 Rust 的 DSL](https://dl.acm.org/doi/10.1145/3310232.3310241)
* [跨编程语言的能效率（Energy Efficiency）](https://greenlab.di.uminho.pt/wp-content/uploads/2017/09/paperSLE.pdf)

### 其它
* [Linus Torvalds 访谈：Linux 和 Git](https://www.tag1consulting.com/blog/interview-linus-torvalds-linux-and-git)
* [编程语言现状：JavaScript 拥有最多开发人员，但 Rust 增长最快](https://www.zdnet.com/google-amp/article/programming-languages-javascript-has-most-developers-but-rust-is-the-fastest-growing/)
* [部分 tensorboard 正在使用 Rust 重写，性能提升了 100-400 倍](https://www.reddit.com/r/rust/comments/mzlg5s/parts_of_tensorboard_are_being_rewritten_in_rust/)（译注：早在 2015 年 12 月，tensorflow 即提供了 Rust API，但并不活跃）
* [我们可在 Rust 中获得有保障的尾递归（Tail Calls）么？](https://www.reddit.com/r/rust/comments/my6k5i/are_we_finally_about_to_gain_guaranteed_tail/)
* [Rust 项目的 GitHub Actions 最佳实践](https://www.fluvio.io/blog/2021/04/github-actions-best-practices/)

# 周最佳 crate

本周最佳 crate 是 [cargo-rr](https://github.com/danielzfranklin/cargo-rr)，`cargo` 子命令，“时光旅游”式的代码 `rr` 调试器。

谢谢 [Willi Kappler](https://users.rust-lang.org/t/crate-of-the-week/2704/905) 的提议。

> **译注**：非常有用，代码调试体验更好。如下示例：
>
> ``` bash
> > cargo rr test my_test
>
> thread 'main' panicked at 'assertion failed: `(left == right)`
>  left: `1`,
> right: `2`', tests/tests.rs:100
>
> test result: FAILED. 0 passed; 1 failed; 0 ignored; 0 measured; 2 filtered out; finished in 0.06s
> ```
> 还有重放功能：
> 
> ``` bash
> > cargo rr replay
> 
> (rr) continue
> 
> thread 'main' panicked at 'assertion failed: `(left == right)`
>   left: `1`,
>  right: `42`', tests/tests.rs:100
> 
> test result: FAILED. 0 passed; 1 failed; 0 ignored; 0 measured; 2 filtered out; finished in 0.06s
> ```

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

[jsonschema-rs：格式化关键字的用户定义验证](https://github.com/Stranger6667/jsonschema-rs/issues/158)（译注：jsonschema 是 JSON 模式（schema）验证器的 Rust 实现。它将模式编译为验证树，以便尽可能快地进行验证）

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Rust 核心更新

[350 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-04-19..2021-04-26

## Rust 编译器性能

本周编译器境况不错，没有任何回退，并有 2 个小进步 🎉🎉.

验测工作是由 **@rylev** 完成的。修正范围：[6df26f8..537544](https://perf.rust-lang.org/?start=6df26f897cffb2d86880544bb451c6b5f8509b2d&end=537544b1061467ee4b74ef7f552fab3d513e5caf&absolute=false&stat=instructions%3Au)

## 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

*无*

## 新的 RFCs

* [增加对 `bitfields` 的支持](https://github.com/rust-lang/rfcs/pull/3113)
* [Rust 2021 edition（trait-only edition）中的新 `prelude`](https://github.com/rust-lang/rfcs/pull/3114)

# 近期活动

### 线上活动
* [April 28, Online - Ockam Open Source Community Call - Rust 中构建端到端加密通信的实时编码演练](https://github.com/ockam-network/ockam/discussions/1303)
* [May 3, 2021, Online - Cloud Native Rust Day](https://events.linuxfoundation.org/cloud-native-rust-day/)
* [May 4, 2021, Online - Cloud Native WASM Day](https://events.linuxfoundation.org/cloud-native-wasm-day/)
* [May 4, 2021, Dublin, IE - Rust Dublin May Remote Meetup - Rust Dublin](https://www.meetup.com/Rust-Dublin/events/277860218/)
* [May 4, Buffalo, NY, US - Buffalo Rust User Group, Tues May 4th - Buffalo Rust Meetup](https://www.meetup.com/Buffalo-Rust-Meetup/events/277402612/)
* [May 11, Seattle, WA, US - Monthly meetup - Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksrycchbpb/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust 招聘信息

**Collabora**

* [**远程** - Rust developer/promoter](https://arbeitnow.com/view/rust-developerpromoter-collabora-36866)

**Paige**

* [**远程/欧洲** - Senior Software Engineer, Visualization](https://boards.greenhouse.io/paige/jobs/5210311002)

**Confio GmbH**

* [**远程** - Rust Engineer at Confio GmbH](https://jobs.gohire.io/confio-gmbh-ggtjivjy/rust-engineer-39453/)

**CoBloX**

* [**远程** - Software Engineer](https://comit.network/blog/2021/03/01/we-are-hiring/)

**Gattaca**

* [Software Engineer - Rust & Python](https://gattaca.com/jobspec.html)

**Wallaroo**

* [**远程** - Senior Client Solutions Engineer](https://wallaroo.breezy.hr/p/47862ae31c91-senior-client-solutions-engineer-remote-even-after-covid)

**Parity Technologies**

* [**远程** - Blockchain Developer - Consensus](https://grnh.se/2dd887b13us)
* [Numerous other Rust engineering openings](https://www.parity.io/jobs/)

**Kollider**

* [**远程** - Junior Backend Engineer](https://kollider.homerun.co/junior-backend-engineer/en)
* [**远程** - Senior Backend Engineer](https://kollider.homerun.co/senior-backend-engineer/en)
* [**远程** - DevOps Engineer](https://kollider.homerun.co/devops-engineer/en)

**Chainflip**

* [Rust / C++ Backend Engineer (Berlin, DE)](https://angel.co/company/chainflip/jobs/1162345-rust-c-backend-engineer)
* [Security Engineer (Berlin, DE)](https://angel.co/company/chainflip/jobs/1293957-security-engineer)
* [Junior/Mid Backend Rust/C++ Developer (Melbourne, AU)](https://angel.co/company/chainflip/jobs/1305439-junior-mid-backend-rust-c-developer)

**Kraken**

* [Several Rust Engineering Positions](https://jobs.lever.co/kraken?team=Engineering)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

# 本周引语

> 此错误消息*不真实（UNREAL）*

– [Ash 2X3 发布于 Twitter](https://twitter.com/ash2x3/status/1384986537167892483)

谢谢 [Nixon Enraght-Moony](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1046) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
