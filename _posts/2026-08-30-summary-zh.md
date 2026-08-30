---
layout: default
title: "Horizon Summary: 2026-08-30 (ZH)"
date: 2026-08-30
lang: zh
---

> 从 6 条内容中筛选出 3 条重要资讯。

---

1. [腾讯开源 Hy4 Preview，一个具备自我改进能力的 7700 亿参数 MoE 模型](#item-1) ⭐️ 8.0/10
2. [美国国土安全部利用晦涩的海关传票法秘密获取记者及活动人士通讯记录。](#item-2) ⭐️ 8.0/10
3. [三星在 Hot Chips 2026 大会上展示其存内计算（PIM）架构](#item-3) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [腾讯开源 Hy4 Preview，一个具备自我改进能力的 7700 亿参数 MoE 模型](https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/) ⭐️ 8.0/10

腾讯发布并开源了新一代混合专家（MoE）AI 模型 Hy4 preview。值得注意的是，该模型通过一个自动化优化循环参与了自身的开发过程，提出了方法、运行了实验并根据结果进行了迭代。 此次发布意义重大，因为它以一个庞大的 7700 亿参数架构和 100 万 token 的上下文长度，推动了开源大语言模型的前沿发展。更重要的是，其展示的递归自我改进能力，代表了向更自主、更高效的 AI 开发方法迈出的关键一步。 Hy4 preview 模型总参数量为 7700 亿，每 token 激活 490 亿参数，并具备 100 万 token 的上下文窗口。据报道，该模型在 OpenRouter 等平台上获得了巨大的初期采用，在发布几天内就处理了数万亿 token。

hackernews · shenli3514 · 8月29日 19:33 · [社区讨论](https://news.ycombinator.com/item?id=49492632)

**背景**: 混合专家（MoE）是一种旨在高效扩展模型容量的神经网络架构。它由许多专门的子网络（专家）组成，但对于每个输入，只激活其中的一小部分，从而保持计算成本可控。自动化优化循环指的是一个系统，其中 AI 模型可以根据反馈提出、测试和完善其自身的训练策略、数据选择或评估方法，从而形成一个自我改进的循环。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hy.tencent.ai/research/hy4-preview?langVersion=en">Introducing Hy4 preview - hy.tencent.ai</a></li>
<li><a href="https://github.com/Tencent-Hunyuan/Hy4-preview">GitHub - Tencent-Hunyuan/Hy4-preview</a></li>
<li><a href="https://shattered.io/tencent-hy4-preview-770b-2026/">Tencent Hy4 Preview: 770B Params, 1M-Token AI Model</a></li>

</ul>
</details>

**社区讨论**: 社区讨论强调了该模型在推理平台上的快速采用及其有竞争力的定价。一些用户对其前身 Hy3 的性能印象深刻，认为其与领先模型具有竞争力。另一些人则对发布材料中基准测试数据的呈现方式提出了批评。

**标签**: `#AI`, `#Machine Learning`, `#Open Source`, `#Tencent`, `#Model Development`

---

<a id="item-2"></a>
## [美国国土安全部利用晦涩的海关传票法秘密获取记者及活动人士通讯记录。](https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits) ⭐️ 8.0/10

美国国土安全部正在利用《美国法典》第 19 编第 1509 条的法律传票（一项最初用于海关检查的规定），秘密获取记者、非营利组织和工会的电话及通讯记录。在多个案例中，当传票在法庭上受到质疑时，国土安全部会撤回传票，这种策略避免了法院对其合法性做出裁决。 这种做法意味着政府监控权力的显著扩张，绕过了典型的司法监督，并可能违反宪法第四修正案禁止无理搜查的保护条款。它直接威胁新闻自由、倡导组织的工作以及个人隐私，并为利用晦涩法律获取广泛调查权力开创了危险的先例。 一个关键细节是，遵守第 1509 条传票并非强制性的；如果受到质疑，国土安全部必须上法庭才能强制执行。报告显示企业的回应不一，例如 T-Mobile 在某个案例中配合并提供了记录，而据报道谷歌则没有。国土安全部监察长办公室此前曾警告，在与海关或移民无关的案件中使用此类传票违反了政策。

hackernews · firefax · 8月29日 18:44 · [社区讨论](https://news.ycombinator.com/item?id=49492219)

**背景**: 《美国法典》第 19 编第 1509 条是一项美国法律，授权美国海关和边境保护局（CBP，国土安全部下辖机构）签发传票以审查记录和证人，作为其海关和税收执法职责的一部分。历史上，其使用与第 19 编（海关）或第 8 编（移民）下的调查相关。美国国土安全部是一个联邦机构，职责广泛，包括边境安全、移民执法和反恐，这赋予了其重大的监控和调查权力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.law.cornell.edu/uscode/text/19/1509">19 U.S. Code § 1509 - Examination of books and witnesses | U.S. Code | US Law | LII / Legal Information Institute</a></li>
<li><a href="https://www.oig.dhs.gov/sites/default/files/assets/Mga/2017/oig-18-18-nov17.pdf">Management Alert - CBP&#x27;s Use of Examination and Summons Authority Under</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了政府为规避裁决而撤回传票的蓄意法律策略，指责那些未经质疑就配合的公司，并指出像 T-Mobile 和谷歌等服务提供商的不同回应。一些人建议记者使用去中心化的通讯工具等实用解决方案，另一些人则批评助长此类监控的更广泛政治气候。

**标签**: `#surveillance`, `#government`, `#privacy`, `#legal`, `#journalism`

---

<a id="item-3"></a>
## [三星在 Hot Chips 2026 大会上展示其存内计算（PIM）架构](https://chipsandcheese.com/p/hot-chips-2026-samsungs-processing) ⭐️ 7.0/10

在 Hot Chips 2026 大会上，三星展示了其存内计算（PIM）技术，该技术将计算单元集成到存储阵列中，以便在数据存储的位置直接执行计算。这一具体实施方案旨在解决现代计算系统中普遍存在的数据移动瓶颈。 这之所以重要，是因为处理器与内存之间的数据移动已成为主要的性能和能耗瓶颈，尤其对于 AI 等数据密集型工作负载。三星此举标志着一个主要行业参与者对探索非冯·诺依曼架构的承诺，这可能为未来的 AI 加速器和高性能计算带来显著的效率提升。 三星的方法属于近存计算（PNM）的一种形式，将计算单元放置在存储阵列附近，而非完全集成。社区讨论中指出的一个关键挑战是，该架构需要精确的数据局部性，这使得它对通用计算的灵活性较低，但可能非常适合 AI 中的矩阵运算等特定模式。

hackernews · ingve · 8月29日 06:06 · [社区讨论](https://news.ycombinator.com/item?id=49487341)

**背景**: 存内计算（PIM）是一种新兴的半导体架构，它将计算移动到存储阵列内部或附近，以减少数据在独立的内存和处理单元之间昂贵的数据移动。传统的冯·诺依曼架构中数据来回传输，随着处理器速度超过内存带宽，形成了“内存墙”或瓶颈。Hot Chips 是一个领先的行业研讨会，三星、SK 海力士和阿里巴巴等主要厂商最近都在此展示了 PIM 原型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/processing-in-memory-pim-architectures-next-frontier-epbof">Processing - in - Memory ( PIM ) Architectures : The Next Frontier in...</a></li>
<li><a href="https://events.safari.ethz.ch/micro-pim-tutorial/doku.php?id=start">start [MICRO 2023 Real-World PIM Tutorial]</a></li>
<li><a href="https://semiengineering.com/data-movement-is-the-energy-bottleneck-of-todays-socs/">Data Movement Is the Energy Bottleneck of Today’s SoCs</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了谨慎乐观与怀疑态度的混合。一些专家指出了这一长期存在的理论概念及其固有的限制，认为它最适合 AI、游戏和加密等特定领域。另一些人对这个用于矩阵乘法的具体实施方案持怀疑态度，认为存储阵列内部的数据移动仍然是一个挑战。还有一种观点认为，每年都有许多奇特的加速器设计被提出，但很少有能获得广泛采用的。

**标签**: `#hardware`, `#computer-architecture`, `#ai-acceleration`, `#memory`, `#samsung`

---