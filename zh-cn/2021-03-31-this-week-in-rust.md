# Rust 官方周报 384 期（2021-03-31）

大家好，欢迎查阅第 384 期《Rust 周报》！[Rust](http://rust-lang.budshome.com) 是一种系统语言，主要追求三个要素：安全性、并发性，以及高性能。本文是其开发进展和社区生态的每周摘要。如果您想提出意见或建议，请在推特联系我们账号 [@ThisWeekInRust](https://twitter.com/ThisWeekInRust)，或者在 github [向我们发送 PR](https://github.com/rust-lang/this-week-in-rust)。想参与吗？我们[期待您的贡献](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md)。

# Rust 社区更新

本周无资讯。

### 官方

* [Rust 1.51.0 官宣发布](https://blog.rust-lang.org/2021/03/25/Rust-1.51.0.html)，中译版本：[Rust 1.51.0 已正式发布，及其新特性详述](https://blog.budshome.com/budshome/rust-1.51.0-yi-zheng-shi-fa-bu-,ji-qi-xin-te-xing-xiang-shu)
* \\[Rust 基金会\\] [介绍 Mark Rousskov](https://foundation.rust-lang.org/posts/2021-03-25-introducing-mark-rousskov/)（Rust 核心团队，项目主管）
* \\[Rust 基金会\\] [介绍 Nell Shamrell-Harrington](https://foundation.rust-lang.org/posts/2021-03-25-introducing-nell-shamrell-harrington/)（董事会成员，微软公司）

### 项目/工具 更新

* [rust-analyzer 更新日志 #70](https://rust-analyzer.github.io/thisweek/2021/03/29/changelog-70.html)
* [IntelliJ Rust 更新日志 #144](https://intellij-rust.github.io/2021/03/29/changelog-144.html)
* [Knurling-rs 财务报告和筹资公告](https://ferrous-systems.com/blog/knurling-financial-update/)，Knurling-rs 致力于提升嵌入式 Rust 开发体验。
* [Ockam | 分布式应用程序之间的端到端加密信息传递，以及交互式身份验证](https://github.com/ockam-network/ockam)
* [Deno 公司宣布成立](https://deno.com/blog/the-deno-company)，JavaScript/TypeScript 的运行时，原 NodeJS 作者主导开发。

### 观测/思考

* [使用 Rust 极致提升 Python 性能-中文版](https://blog.budshome.com/budshome/shi-yong-rust-ji-zhi-ti-sheng-python-xing-neng-:tu-biao-he-hui-tu-ti-sheng-24-bei-,shu-ju-ji-suan-ti-sheng-10-bei)：图表和绘图提升 24 倍，数据计算提升 10 倍。
* [Rust web 框架现状-中文版](https://blog.budshome.com/budshome/rust-web-kuang-jia-xian-zhuang--(2021-nian-1-ji-du-)-)，如下图为 Rocket 框架调试工具 LogRocket 界面。

![LogRocket](https://blog.budshome.com/static/articles/1617386708.jpg)

* [GhostCell：分离权限与数据的 Rust API](http://plv.mpi-sws.org/rustbelt/ghostcell/)
* [在 slipstream 库中使用常量泛型（const generics）](https://vorner.github.io/2021/03/28/const-generic-slipstreem.html)
* [Rust 迭代器（Iterator trait ）的要诀和技巧-中文版](https://blog.budshome.com/budshome/rust-die-dai-qi-(iterator-trait-)de-yao-jue-he-ji-qiao)

### Rust 演练

* [重点和痛点](https://fasterthanli.me/articles/pin-and-suffering)，async Rust 演练，主要是 tokio。
* [使用 C-bindgen 将 Rust 嵌入 Zephyr（物联网操作系统）固件](https://www.jaredwolff.com/embedding-rust-into-zephyr-using-cbindgen/)
* [Rust 中的解析器组合因子](https://blog.budshome.com/budshome/rust-zhong-de-jie-xi-qi-zu-he-yin-zi-(parser-combinators))（中译版本），英文[原文链接](https://doma.dev/blog/parsing-stuff-in-rust/)。
* [Rust 中的网格，第二部分：常量泛型](https://blog.adamchalmers.com/grids-2/)
* [Rust 中，符合人类工程学的错误处理](https://dev.to/senyeezus/ergonomic-error-handling-with-rust-13bj)，即处理方式舒适，不生硬。
* [使用 Rust 常量泛型实现 SHA2 (256/512) 算法](https://dev.to/dandyvica/implementing-sha2-256-512-algorithm-with-rust-const-generics-5ap)
* [使用 GNU 调试器分析内存分配](https://dev.to/ignaciojvig/analisando-alocacoes-de-memoria-em-rust-utilizando-gnu-debugger-34kb)
* [测试嵌入式 Rust 应用程序](https://ferrous-systems.com/blog/test-embedded-app/)
* [使用常量泛型为电子图形建模](https://mkhan45.github.io/2021/03/28/Using-const-generics-to-model-an-electronics-graph.html)
* [Rust 的模块系统](https://aloso.github.io/2021/03/28/module-system.html)
* \\[系列\\] [使用 crate：trust-dns-resolver](https://dev.to/basman/series/11934)
* \\[视频\\] [更安全的 Rust：和 Creusot 一起检查程序](https://youtu.be/BPt987BRdDw)

### 其它

* [在 Linux 内核中，Linus Torvalds 对 Rust 语言进行评估](https://arstechnica.com/gadgets/2021/03/linus-torvalds-weighs-in-on-rust-language-in-the-linux-kernel/)
* [所有权的概念图](https://www.reddit.com/r/rust/comments/mgh9n9/ownership_concept_diagram/)

# 周最佳 crate

本周最佳 crate 是 [tide-acme](https://github.com/http-rs/tide-acme)，使用 Let's Encrypt for Tide，自动进行 HTTPS 认证。

由 [Josh Triplett](https://users.rust-lang.org/t/crate-of-the-week/2704/894) 提议，谢谢！

[关于下周最佳 crate，请您提议，并投票](https://users.rust-lang.org/t/crate-of-the-week/2704)!

# 参与邀请

您一直想为开源项目做贡献，但却不知道从哪里开始吗？每周，我们都会强调一些来自 Rust 社区的任务。您可以挑选，并开始参与！

有些任务可能还有导师，请访问具体任务页面，以了解更多信息。

* [AWS 项目：Rust lambda 运行时，以及生物信息项目 BioIT](https://umccr.org/blog/aws-bioinformatics-rust/)
* [darpi-rs/darpi 寻求用户和贡献者](https://github.com/darpi-rs/darpi)
* [RoaringBitmap/roaring-rs 请求 PR 复核](https://github.com/RoaringBitmap/roaring-rs/pull/92)

如果你是 Rust 项目所有人，正在寻求贡献人员，请提交任务到[这个页面](https://users.rust-lang.org/t/twir-call-for-participation/4821)。

# Rust 核心更新

327 PR 在\\[上一周被合并\\]\\[merged\\]

# 近期活动

### 线上活动

* [April 1, Berlin, DE - Rust Hack and Learn - Berline.rs](https://www.meetup.com/opentechschool-berlin/events/txcprryccgbcb/)
* [April 6, Buffalo, NY, US - Buffalo Rust User Group - Buffalo Rust Meetup](https://www.meetup.com/Buffalo-Rust-Meetup/events/276717867/)
* [April 7, Johannesburg, ZA - Monthly Joburg Rust Chat! - Johannesburg Rust Meetup](https://www.meetup.com/Johannesburg-Rust-Meetup/events/277133126/)
* [April 7, Indianapolis, IN, US - Indy.rs - with Social Distancing - Indy Rust](https://www.meetup.com/indyrs/events/jhfstryccgbkb/)
* [April 13, Seattle, WA, US - Monthly Meetup - Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksryccgbrb/)

### 北美

* [April 8, Columbus, OH, US - Monthly Meetup - Columbus Rust Society](https://www.meetup.com/columbus-rs/events/dpkhgryccgblb/)
* [April 14, Atlanta, GA, US - Grab a beer with fellow Rustaceans - Rust Atlanta](https://www.meetup.com/Rust-ATL/events/qxqdgryccgbsb/)

# Rust 招聘信息

**e.ventures**

* [Rust 后端工程师（远程，美国）](https://old.reddit.com/r/rust/comments/mfstaz/official_rrust_whos_hiring_thread_for_jobseekers/gspq9v1/)

**Wallaroo**

* [软件工程师（远程）](https://wallaroo.breezy.hr/p/30939dc4e5c7-software-engineer)

**Ockam**

* [招聘若干 Rust 岗位](https://www.ockam.io/team#open-roles)

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# 本周引语

> 尽管存在所有负面影响，但我必须说：我确实非常喜欢 Rust 所采用的基于民意调查的方法。遇到的大多数问题，并非错误而引起，而是因为：没有其它语言，真正将这个原则推进到如此远的地步。编程语言的设计，首要是“艺术性”，而非技术性。并且，预见所选择设计的后果，那几乎是不可能的。

– [tomaka on medium](https://tomaka.medium.com/a-look-back-at-asynchronous-rust-d54d63934a1c)

谢谢 [Michael Howell](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1028) 的提议。

[欢迎提交下周引语！](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*Rust 周报编辑人员：[nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq)、[cdmistman](https://github.com/cdmistman).*

原文链接： [This Week in Rust 384](https://this-week-in-rust.org/blog/2021/03/31/this-week-in-rust-384/)

---