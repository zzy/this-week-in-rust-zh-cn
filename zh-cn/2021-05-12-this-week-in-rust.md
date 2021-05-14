# Rust 官方周报 390 期（2021-05-12）

> [Rust 官方周报（中文版）仓库为 github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)，欢迎您的参与，一起丰富中文网络的 Rust 资源。
> 
> 关于周报中的资源链接，已经有中文资源的，替换为中文资源链接（中文资源中，均附有原文链接）。另外，对于部分周报文章，附有阅读和简单了解后的译注，但并非全部。如果你阅读了文章，有更适合的见解，请联系、PR，或者直接参与项目 [github.com/zzy/this-week-in-rust-zh-cn](https://github.com/zzy/this-week-in-rust-zh-cn)。

大家好，欢迎查阅第 390 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一门系统编程语言，专注于三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github 向我们[发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

# Rust 社区更新

### 官方
* [Rust 2021 版次工作计划](https://blog.rust-lang.org/2021/05/11/edition-2021.html)（译注：每月计划，2021 年 4 月计划请参阅文章 [Rust 2021 版本特性预览，以及工作计划](https://blog.budshome.com/budshome/rust-2021-ban-ben-te-xing-yu-lan-,yi-ji-gong-zuo-ji-hua)）
* [Rust 1.52.1 已正式发布，及其新特性详述](https://blog.budshome.com/budshome/rust-1.52.1-yi-zheng-shi-fa-bu-,ji-qi-xin-te-xing-xiang-shu)
* [Rust 1.52.0 已正式发布，及其新特性详述](https://blog.budshome.com/budshome/rust-1.52.0-yi-zheng-shi-fa-bu-,ji-qi-xin-te-xing-xiang-shu)

### 简讯
* [Rust 游戏开发（GameDev）月报 #21 - 2021 年 4 月](https://gamedev.rs/news/021/)（译注：游戏非常精美，随意截图如下）
![Rust GameDev](https://blog.budshome.com/static/articles/1620899678.jpg)
* [RiB 简讯 #23 - 使用 Rust 重写？](https://www.reddit.com/r/rust/comments/n5xhku/rib_newsletter_23_rewriting_in_rust/)

### 项目/工具更新
* [rust-analyzer 更新日志 #76](https://rust-analyzer.github.io/thisweek/2021/05/10/changelog-76.html)
* [Knurling-rs 更新日志 #24：3 次发布，`defmt-test` 支持更多项目，以及解决了一个让人生厌的问题](https://ferrous-systems.com/blog/knurling-changelog-24/)（译注：Knurling-rs 主要致力于嵌入式 Rust 体验）
* [TensorBase 周报 2 期](https://tensorbase.io/thisweek/2021-05-10-tw_2/)（译注：TensorBase 是基于 Rust 的现代化开源数据仓库，详细中文介绍见页面内的链接）
* [Naga 着色器（shader）转换的基准测试](https://gfx-rs.github.io/2021/05/09/dota2-msl-compilation.html)（译注：naga 是一个实验性的着色器转换库，用于 WebGPU，以及 gfx-rs 项目，一个高性能、无绑定的图形 API）
* [egui 发布版本 0.12 - 一个简单的 GUI 库](https://www.reddit.com/r/rust/comments/n9f6vt/announcing_egui_012_the_simple_gui_library/)（译注：支持多种样式主题，蛮漂亮）
* [GCC Rust 每周状态报告 14](https://thephilbert.io/2021/05/10/gcc-rust-weekly-status-report-14/)（译注：gcc 的 Rust 实现，还处于早期的阶段，并不能实际编译）
* [Rust + Android 的集成开发设计](https://blog.budshome.com/budshome/rust-+-android-de-ji-cheng-kai-fa-she-ji)（译注：Rust 和 Android 集成开发的官方设计，包括：无需嵌套的（nested）构建系统、用过程宏（proc_macro）而无需构建脚本（build.rs）、以 crate 形式生成源码，以及动态链接 crate 等）
* [Alpha Launch - 亚马逊公司新开发的 Rust SDK](https://aws.amazon.com/blogs/developer/a-new-aws-sdk-for-rust-alpha-launch/)
* [Gleam v0.15 发布](https://gleam.run/news/gleam-v0.15-released/)（译注：Servo 的 OpenGL 绑定和封装）
* [IsomorphicDB 未来之路](https://isomorphicdb.io/blog/2021/05/11/IsomorphicDB-The-Road-ahead/)（译注：IsomorphicDB 是 Rust 实现的，兼容 PostgreSQL 的分布式数据库的核心）
* [我的第一个 Rust crate，pretend](https://sfietkonstantin.github.io/2021/05/10/First-Crate-Pretend.html)（译注：pretend 是基于宏的 HTTP 客户端）

### 观测/思考
* [将 Rust 用在前端和后端](https://blog.abor.dev/p/moonzoon)（译注：MoonZoon 作者 Martin Kavík 的访谈，MoonZoon 演示看起来还不错，作者说其是 `NO Javascript、NO CSS、NO HTML、NO REST、NO GraphQL、NO SQL、NO Analysis Paralysis、NO Wheel Reinventing、NO Passwords*` 的 Rust 全栈开发框架）
* [为什么我们应当将 Rust 用于嵌入式开发？](https://blog.budshome.com/budshome/wei-shi-yao-wo-men-ying-dang-jiang-rust-yong-yu-qian-ru-shi-kai-fa--)
* [编写地道的（idiomatic）Rust 代码](https://shane-o.dev/blog/aiming-for-idiomatic-rust)
* [使用 Rust 优化 7000 个 CPUs](https://medium.com/tenable-techblog/optimizing-700-cpus-away-with-rust-dc7a000dbdb2)
* [通过 Bors 提升我们开发时的信心和效率](https://www.fluvio.io/blog/2021/05/bors-confident-merges/)（译注：此处说的 Bors 是一个 github 的应用/bot，用于将 PR 整合到 master 分支）
* [提高 DataFusion 4.0 中的数据并行层次](https://medium.com/@danilheres/increasing-the-level-of-parallelism-in-datafusion-4-0-d2a15b5a2093)（译注：DataFusion 是以 Apache Arrow 作为内存模型的内存查询引擎）
* [我对 Rust 的第二印象，以及为什么我认为 Rust 是最佳通用语言](https://deepu.tech/my-second-impression-of-rust/)
* [渐进地将一个小型 Python 项目迁移到 Rust](https://blog.waleedkhan.name/port-python-to-rust/)
* [视频] [Rust 验证（Verification）研讨会 2021 - Ferrite：用于消息传递协议验证的 Rust EDSL](https://youtu.be/6dcf3tOPOwo)
* [视频] [Rust 验证（Verification）研讨会 2021 - RustBelt：快速潜入深渊](https://youtu.be/iAs0gZ8o0oQ)
* [视频] [Rust 验证（Verification）研讨会 - Polonius](https://youtu.be/H54VDCuT0J0)
* [视频] [Rust 验证（Verification）研讨会 - Rust 对安全和关键环境的兴趣](https://youtu.be/_DM36e2A9dg)
* [视频] [Rust 验证（Verification）研讨会 - 利用编译器中介（Intermediate）表征进行多/跨语言验证](https://youtu.be/0DcIn7kiNxM)

### Rust 演练
* [BABE – 共识算法及其实现](https://blog.knoldus.com/babe-consensus-algorithm-and-how-to-implement-it-in-our-runtime/)（译注：BABE 全称是 Blind Assignment for Blockchain Extension，指在验证节点之间运行，并确定新块生产者的区块生成机制）
* [Substrate 中的“托盘”，以及在运行时（runtime）中使用它们](https://blog.knoldus.com/pallets-in-substrate-and-using-them-in-runtime/)（译注：Substrate 框架允许节点运行时（runtime）开发者在模块中声明特定于领域的逻辑，称之为“托盘”）
* [如何在 DigitalOcean 部署 Rust web 应用？](https://dev.to/steadylearner/how-to-deploy-rust-web-app-with-digitalocean-h2o)
* [学习 Rust #4: 使用强类型（strong types）解析 JSON](https://dev.to/hamatti/learning-rust-4-parsing-json-with-strong-types-575m)
* [如何使用 Rust web 框架 Warp？](https://dev.to/steadylearner/how-to-use-rust-warp-web-framework-2b4e)
* [Ray Tracing in One Weekend](https://misterdanb.github.io/raytracinginrust/)（译注：一个 CC0 协议的周末系列丛书，源码可下载）
* [过程宏之错误处理](https://blog.turbo.fish/proc-macro-error-handling/)
* [使用 arena 分配器（allocators）加速算法](https://mnwa.medium.com/speeding-up-algorithms-with-arena-allocators-d72d06f23607)
* [使用 Rust 和 Actix 构建 REST 及 Web Socket API](https://agmprojects.com/blog/building-a-rest-and-web-socket-api-with-actix.html)
* [在 CI 中构建与老版本 GLIBC 一起工作的 Rust 二进制程序](https://kobzol.github.io/rust/ci/2021/05/07/building-rust-binaries-in-ci-that-work-with-older-glibc.html)
* [中文] [系列] [基于 Async Rust 构建 GraphQL 服务，使用 tide + async-graphql + mongodb（4）](https://blog.budshome.com/budshome/gou-jian-rust-yi-bu-graphql-fu-wu-:ji-yu-tide-+-async-graphql-+-mongodb(4)--bian-geng-fu-wu-,yi-ji-di-er-ci-zhong-gou)
* [中文] [系列] [基于 actix-web + async-graphql + rbatis + postgresql / mysql 构建异步 Rust GraphQL 服务（3）](https://blog.budshome.com/budshome/ji-yu-actix-web-+-async-graphql-+-rbatis-+-postgresql---mysql-gou-jian-yi-bu-rust-graphql-fu-wu-(3)---zhong-gou)
* [视频] [Rust 中的 Graphs：什么是 Graph？Rust 中如何表述它们？](https://youtu.be/3DLrUNbKhjQ)
* [视频] [Rust 验证（Verification）研讨会 2021 - 窥视编译器内部数据（基于乐趣和裨益）](https://youtu.be/SKmd5A-1cSE)
* [视频] [Rust 验证（Verification）研讨会 2021 - 确保 Rust 不会崩溃（crash）](https://youtu.be/vMGilPbIotw)
* [视频] [Rust 验证（Verification）研讨会 2021 - crux-mir：Rust 中的符号（Symbolic）测试](https://youtu.be/0mocaSR9f_M)
* [视频] [Rust 验证（Verification）研讨会 2021 - Rustv：不安全（Unsafe）Rust 的半自动（semi-automatic）验证](https://youtu.be/bikmlNlwAYo)
* [视频] [Rust 验证（Verification）研讨会 2021 - 使用受约束的（constrained）Horn 解算器实现不安全（Unsafe）Rust 的自动验证](https://youtu.be/yJQZ7sG8xSM)
* [视频] [Rust 验证（Verification）研讨会 2021 - Prusti - Rust 的演绎式验证](https://youtu.be/C9TTioH5JUg)
* [视频] [Rust 验证（Verification）研讨会 2021 - Creusot：Rust 验证软件的原型工具](https://youtu.be/b8sBtmzq0FM)
* [视频] [Rust 验证（Verification）研讨会 2021 - hacspec：简洁、可执行、可验证的高可靠性密码学规范](https://youtu.be/k7_BcWwvz7k)

### 其它
* [使用 Rust 进行创新](https://aws.amazon.com/blogs/opensource/innovating-with-rust/)
* [那些事情是 C++ 能做到的，而 Rust 却做不到？（2021 版）](https://www.reddit.com/r/rust/comments/n7rjfk/what_can_c_do_that_rust_cant_2021_edition/)
* [视频] [Rust 借用检查器（borrow checker）— 深入研究 @ Rust DC, April 20, 2021 w/ Nell Shamrell-Harrington](https://youtu.be/Ys7ma3au5m0)

# 周最佳 crate

本周最佳 crate 是 [tokio-console](https://github.com/tokio-rs/console)，类似 “top” 的实用工具（译注：Linux top 命令），用于查看任务的运行情况。

谢谢 [Simon Farnsworth](https://users.rust-lang.org/t/crate-of-the-week/2704/910) 的提议。

[关于下周最佳 crate，请您提议，并投票][submit_crate]！

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

* [advent_of_code_traits - 提升默认的 `run` 方法的效率](https://github.com/drmason13/advent_of_code_traits/issues/3)
* [compress-tools-rs - 由于连接失败，无法在Windows上静态编译，退出代码（exit code）1120](https://github.com/OSSystems/compress-tools-rs/issues/57)

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面][guidelines]。

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Rust 核心更新

[324 PRs 在上周被合并][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-05-03..2021-05-10

## Rust 编译器性能

总体上，没有太大的变化——回归和改进都很少。除了对 PR [#83278](https://github.com/rust-lang/rust/issues/83278) 中 libcore 的编译时进行了 2 倍改进之外。

验测工作是由 **@pnkfelix** 完成的。修正范围：[7a0f..382f](https://perf.rust-lang.org/?start=7a0f1781d04662041db5deaef89598a8edd53717&end=382f748f23979e37e3e012b090e5a0313463f182&absolute=false&stat=instructions%3Au)

[此处可查阅完整报告](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-05-11.md).

## 已核准的 RFCs

Rust 的改进遵循 [RFC（request for comments）流程](https://github.com/rust-lang/rfcs#rust-rfcs)。如下是本周核准实现的 RFCs：

* [RFC：Rust 2021 版的保留性前缀](https://github.com/rust-lang/rfcs/pull/3101)

## 新的 RFCs

* [从 examples/ directory 为 Rustdoc 提示示例代码](https://github.com/rust-lang/rfcs/pull/3123)

# 近期活动

### 线上
* [May 12, Online - Rust Meetup May 2021 - Rust Malaysia](https://docs.google.com/forms/d/e/1FAIpQLSf_hz-ZDwYEhVmIH0uzJ0uH41aXWZ_zRDsI0XENpfkKHvh_Jg/viewform)
* [May 13, Berlin, DE - Rust Hack and Learn - Berline.rs](https://berline.rs/2021/05/13/rust-hack-and-learn.html)
* [May 15 - June 7, Online - Solana Season Hackathon - Registration open now](https://twitter.com/solana/status/1387411221717176323?s=20)
* [May 17, 2021, Cardiff, UK - Rust and Cpp Cardiff :: v2.0 - Rust and C++ Cardiff](https://secure.meetup.com/register/?referrer_n=event&referrer_i=278002832&ctx=ref)
* [May 18, 2021, Washington, DC, US - Mid-month Rustful: rust4ml - Rust DC](https://www.meetup.com/RustDC/events/ntvrgsycchbxb)
* [May 19, 2021, Vancouver, BC - Rust Study/Hack/Hang-out night - Vancouver Rust](https://www.meetup.com/Vancouver-Rust/events/zppkjsycchbzb/)
* [May 20, 2021, Online - Go vs Rust | Round table discussion](https://rustlab.it/en/rust-vs-go/)
* [May 20, 2021, Dallas, TX, US - Last Tuesday - Dallas Rust](https://www.meetup.com/Dallas-Rust/events/jqxqwrycchbhc/)

如果你正在运作一次 Rust 活动，请将其[添加到日历][calendar]中，以便在此处提及。请向 [Rust 社区团队][community]发送电子邮件，以获取访问日历权限。

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust 招聘信息

**Paige**

* [Senior Software Engineer, Visualization (Remote, Europe)](https://boards.greenhouse.io/paige/jobs/5210311002)

**Impero**

* [Full Stack Developer (Denmark + Remote)](https://www.linkedin.com/jobs/view/2493233249/)

**Zimpler**

* [Rust Developer (Gothenburg, SE)](https://careers.zimpler.com/jobs/1170476-rust-developer-to-zimpler)

**Yat Labs**

* [Senior Rust Developer (Remote)](https://www.arbeitnow.com/view/senior-rust-developer-tari-71761)

**Kollider**

* [Junior Backend Engineer (Remote)](https://kollider.homerun.co/junior-backend-engineer/en)
* [Senior Backend Engineer (Remote)](https://kollider.homerun.co/senior-backend-engineer/en)
* [DevOps Engineer (Remote)](https://kollider.homerun.co/devops-engineer/en)

**TrueLayer**

* [Rust Backend Engineer (London, UK)](https://apply.workable.com/truelayer/j/D07759DAF6/)
* [Rust Backend Engineer (Milan, Italy)](https://apply.workable.com/truelayer/j/F13E839E3B/)
* [Rust Engineering Lead (London, UK)](https://apply.workable.com/truelayer/j/3B78A6F6F4/)
* [Rust Engineering Lead (Milan, Italy)](https://apply.workable.com/truelayer/j/8D8D56C09E/)

**Aleph Alpha**

* [Several Rust Engineering Positions (Heidelberg, DE)](https://aleph-alpha.de/career)

**Kraken**

* [Several Rust Engineering Positions (Remote)](https://jobs.lever.co/kraken?team=Engineering)

**ChainSafe**

* [Several Rust Engineering Positions (Remote)](https://chainsafe.io/careers)

*通过 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，tweet 信息给我们，以便于我们在此处列出你的招聘信息！*

# 本周引语

> 除非你愿意花上几个星期的时间，使用 Rust 构建一些应用。否则，你不会喜欢 Rust。最初阶段，陡峭的学习曲线充满挑战，可能会让人沮丧——不过这取决于你对它的看法。但这个阶段一旦过去，你很难做到不喜欢 Rust。毕竟，Rust 是个有超能力的孩童 💗

– [Deepu K Sasidharan 发表于个人博客](https://deepu.tech/my-second-impression-of-rust)

谢谢 [Phlopsi](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1047) 的提议！

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman)。*

谢谢您的阅读！

---
