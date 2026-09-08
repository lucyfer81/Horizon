---
layout: default
title: "Horizon Summary: 2026-09-08 (ZH)"
date: 2026-09-08
lang: zh
---

> 从 10 条内容中筛选出 2 条重要资讯。

---

1. [恶意网络爬虫消耗的 CPU 资源超过 Linux 内核 Git 服务器所有合法流量总和。](#item-1) ⭐️ 8.0/10
2. [加州理工学院举办全球首个研究级数学黑客松。](#item-2) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [恶意网络爬虫消耗的 CPU 资源超过 Linux 内核 Git 服务器所有合法流量总和。](https://simonwillison.net/2026/Sep/7/creepy-crawlies/) ⭐️ 8.0/10

内核.org 基础设施团队的 Konstantin Ryabitsev 透露，Linux 内核的官方 Git 仓库（git.kernel.org）为恶意网络爬虫将 Git 提交记录渲染成 HTML 所消耗的 CPU 周期，超过了包括 Git 克隆在内的所有其他合法访问的总和。在五个地理分布式节点上，随时都有 14 个 CPU 核心专门处理这项任务。 这突显了关键开源项目正面临日益严重的、不断增长的基础设施负担，原本用于开发者的资源被转移用于服务自动化、通常是恶意的数据抓取。这个问题反映了恶意爬虫造成的&\#x27;背景辐射&\#x27;不断升级的广泛趋势，威胁着面向公众的 Web 服务（尤其是像代码仓库这样拥有高价值数据的服务）的性能、成本和可持续性。 该分析特别关注了将提交历史动态渲染为网页所带来的 CPU 成本，这一功能被爬虫大量利用。问题不仅在于带宽消耗，更在于密集的服务器端处理。尽管服务器已采用地理分布式部署以提高弹性和性能，但问题依然存在。

rss · Simon Willison · 9月7日 23:08

**背景**: git.kernel.org 是托管 Linux 内核源代码的主要官方 Git 仓库，Linux 内核是全球软件基础设施的关键组成部分。网络爬虫（或机器人）是自动浏览网页以索引或抓取数据的程序；其中一些是合法的（如搜索引擎机器人），但另一些则是恶意的，未经许可就大量抓取内容，通常用于垃圾邮件、数据挖掘或训练 AI 模型。将 Git 提交记录渲染为 HTML 允许用户在浏览器中查看提交详情，但与提供静态文件或处理 Git 协议流量相比，这种动态页面生成的计算成本要高得多。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kernel.org">kernel.org - Wikipedia</a></li>
<li><a href="https://fingerprint.com/blog/web-crawler-detection/">How to Detect and Block Malicious Web Crawlers in 2025</a></li>
<li><a href="https://www.amicited.com/blog/ai-crawler-impact-server-resources/">AI Crawler Impact on Server Resources: What to Expect | Am I Cited</a></li>

</ul>
</details>

**标签**: `#web-crawling`, `#infrastructure`, `#linux-kernel`, `#performance`, `#security`

---

<a id="item-2"></a>
## [加州理工学院举办全球首个研究级数学黑客松。](https://mathathonchallenge.com/index.html) ⭐️ 7.0/10

加州理工学院与 Anthropic 和 OpenAI 合作，宣布举办全球首个专注于研究级数学的黑客松——Mathathon。这项为期 40 小时的活动定于 2026 年 10 月 30 日至 11 月 1 日举行，将有约 100 支入选团队使用人工智能解决一个开放的数学问题。 该活动通过利用人工智能和大规模计算资源，在使前沿数学研究大众化方面迈出了重要一步。它标志着一个日益增长的趋势，即使用竞争性、协作性的形式来解决基础研究问题，这可能会加速人工智能与数学交叉领域的发现。 该黑客松由加州理工学院的本科生组织，并非加州理工学院院系的官方活动，所有资金都用于支付评委和参与者的费用。一个明确的关键目标是促进负责任的人工智能使用，该活动由包括 DARPA expMath、Cognition 和 a16z 在内的众多组织赞助。

hackernews · astroanax · 9月7日 09:26 · [社区讨论](https://news.ycombinator.com/item?id=49596055)

**背景**: 黑客松通常是一种有时限的协作活动，参与者集中精力进行软件或技术项目开发。研究级数学涉及解决未解问题或对数学知识做出新颖贡献，这一领域传统上由学术机构和研究实验室主导。将人工智能，特别是大语言模型（LLM），整合到数学问题解决中，是一个新兴且快速发展的领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://agihunt.info/en/e/1a06e401b02e2c5c041ef20ab7f">Caltech Hosts World&#x27;s First AI Math Hackathon… · AGI Hunt</a></li>
<li><a href="https://undercodetesting.com/caltech-anthropic-openai-host-worlds-first-research-level-math-hackathon-with-m-in-compute-and-ai-agents/">Caltech Anthropic OpenAI Host World&#x27;s First Research-Level Math ...</a></li>

</ul>
</details>

**社区讨论**: 讨论中，一位组织者澄清了该活动由学生主导、非营利的性质及其促进负责任人工智能的目标。一位熟悉加州理工学院背景的参与者表示，由于认为该校计算机科学系实力较弱，该黑客松也是学生获得人工智能领域认可的一种方式。另一位评论者则对黑客松这种高强度、短时间的模式是否适合基于大语言模型的数学研究表示怀疑，因为后者通常涉及长时间、间歇性的计算运行。

**标签**: `#hackathon`, `#mathematics`, `#artificial-intelligence`, `#research`, `#education`

---