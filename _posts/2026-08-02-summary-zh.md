---
layout: default
title: "Horizon Summary: 2026-08-02 (ZH)"
date: 2026-08-02
lang: zh
---

> 从 9 条内容中筛选出 4 条重要资讯。

---

1. [Andrej Karpathy 推出新 AI 基准 &\#x27;Pelican&\#x27;，用于评估模型通过 3D 场景生成理解物理世界的能力。](#item-1) ⭐️ 8.0/10
2. [eBay 因安全团队对批评者实施骚扰活动被勒令支付 5600 万美元](#item-2) ⭐️ 8.0/10
3. [科技巨头联名倡导&\#x27;开放权重&\#x27;AI，回应美国潜在限制](#item-3) ⭐️ 8.0/10
4. [Kakehashi：一个在 Linux ARM 上运行 macOS 二进制文件的实验性用户空间项目](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Andrej Karpathy 推出新 AI 基准 &\#x27;Pelican&\#x27;，用于评估模型通过 3D 场景生成理解物理世界的能力。](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 8.0/10

AI 研究员 Andrej Karpathy 引入了一个名为 &\#x27;Pelican&\#x27; 的新基准测试，它要求 AI 模型生成一只鹈鹕骑自行车的 SVG 图像。这项任务旨在评估模型通过 3D 场景生成来理解和表征物理世界的能力。 这个基准测试很重要，因为它超越了传统的基于文本的评估，旨在探究模型的空间推理和物理常识，这对于开发能与现实世界交互的 AI 至关重要。它凸显了 AI 研究领域日益关注弥合语言模型与具身、物理智能之间的差距。 该基准测试明确要求模型生成 SVG（一种矢量图形格式），这需要理解形状、空间关系和物体交互。值得注意的是，一些社区成员认为，在此任务上的成功可能反映的是模型编写特定代码（如 three.js）的熟练度，而非真正的物理理解。

hackernews · delichon · 8月2日 04:05 · [社区讨论](https://news.ycombinator.com/item?id=49140998)

**背景**: 传统的 AI 基准测试（如 MMLU 或 GSM8K）主要测试知识记忆和基于文本的推理。相比之下，3D 场景生成涉及根据描述创建连贯的 3D 环境，这是生成式 AI 与计算机视觉交叉领域的任务。&\#x27;物理 AI&\#x27; 是一个更广泛的领域，旨在使 AI 系统能够在现实世界中感知和行动，从数字比特迈向物理原子。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark) - Grokipedia</a></li>
<li><a href="https://arxiv.org/abs/2505.05474">[2505.05474] 3D Scene Generation: A Survey - arXiv.org 3D Scene Generation: A Survey - arXiv.org GitHub - hzxie/Awesome-3D-Scene-Generation: A curated list of ... 3D Scene Generation: A Survey - NASA/ADS 3D Scene Generation GitHub - 3dlg-hcvc/SceneEval: Official implementation of the ... Paper page - 3D Scene Generation: A Survey - Hugging Face</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/generative-physical-ai/">What is Physical AI? | NVIDIA Glossary</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了不同观点：一些人认为该基准测试是衡量物理推理进展的宝贵（尽管是主观的）工具，而另一些人则持怀疑态度，认为良好的表现可能仅仅表明模型具备为特定库（如 three.js）生成代码的技能。也有人担心，这个看似简单的提示可能导致过早宣布问题已被&\#x27;解决&\#x27;。

**标签**: `#AI`, `#Benchmarks`, `#Computer-Vision`, `#3D-Graphics`, `#Machine-Learning`

---

<a id="item-2"></a>
## [eBay 因安全团队对批评者实施骚扰活动被勒令支付 5600 万美元](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 8.0/10

美国一家法院勒令 eBay 支付 5600 万美元赔偿金，因其公司安全团队对批评该公司的电商通讯 EcommerceBytes 的出版商 Ina 和 David Steiner 夫妇实施了有组织的骚扰活动。包括前警长在内的七名前 eBay 安全部门员工因参与此次网络跟踪骚扰计划而被定罪，其行为包括寄送血淋淋的猪头面具等令人不安的包裹。 此案确立了一个重要的法律和财务先例，即当企业内部安全职能被武器化以压制批评者时，企业必须承担责任，这代表了严重的公司道德和法治的破坏。它引发了关于企业安全团队监管、其他地方发生类似不当行为的可能性，以及报道大公司的记者和独立出版商安全性的紧迫问题。 这起被检察官描述为“恐怖行为”的骚扰活动，据称是由 eBay 安全团队的高级成员发起的，手段包括寄送活昆虫和进行监视。尽管前首席执行官 Devin Wenig 否认参与，但据报道该安全团队向高级副总裁 Wendy Jones 汇报，这凸显了公司治理和指挥链方面可能存在的失职。

hackernews · JumpCrisscross · 8月2日 19:19 · [社区讨论](https://news.ycombinator.com/item?id=49147435)

**背景**: 网络跟踪是指利用互联网或电子手段跟踪或骚扰个人或组织的行为，可能包括虚假指控、诽谤和威胁。Ina Steiner 运营着 EcommerceBytes，这是一份批评 eBay 商业做法的通讯。企业安全团队通常负责保护公司资产和人员，但此案表明它们可能被滥用于恐吓批评者等非法目的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://me.mashable.com/tech/74435/inside-the-ebay-harassment-campaign-that-led-to-a-557-million-settlement">Inside the eBay harassment campaign that led to a $55.7 million...</a></li>
<li><a href="https://www.abc4.com/news/tech-social-media/ap-technology/ap-member-of-ebay-security-team-sentenced-in-harassment-scheme-involving-bloody-halloween-pig-mask/">Member of eBay security team sentenced in harassment scheme...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cyberstalking">Cyberstalking - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论对此为孤立事件表示怀疑，用户质疑 eBay 是否还针对过其他批评者，并呼吁对涉案的“前警长”进行审查。有用户分享了涵盖此案的播客系列“Behind the Bastards”的链接，表明公众对此不当行为的细节和更广泛影响持续关注。

**标签**: `#corporate-governance`, `#cyber-harassment`, `#legal`, `#business-ethics`, `#security`

---

<a id="item-3"></a>
## [科技巨头联名倡导&\#x27;开放权重&\#x27;AI，回应美国潜在限制](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

7 月 24 日，由微软牵头，NVIDIA、亚马逊和 OpenAI 等 235 家公司签署了一份名为《开放权重与美国 AI 领导力》的公开信，反对美国政府可能对开放权重 AI 模型施加的限制。作为回应，Anthropic 三天后发布了其立场文件，而另一封由 1300 多名前沿 AI 公司员工签署的公开信则呼吁美国政府支持&\#x27;调控&\#x27;自动化 AI 发展的努力。 这场辩论代表了 AI 政策中的一个关键分歧，一方主张通过开放审查带来的创新、竞争和安全效益，另一方则担忧国家安全和灾难性滥用风险。其结果将决定先进的 AI 发展是继续集中在少数封闭供应商手中，还是成为一个更分布式、开放的生态系统，从而深刻影响全球技术领导地位和 AI 安全路径。 由微软主导的公开信特别为&\#x27;蒸馏&\#x27;技术辩护——即使用一个模型的输出来训练另一个模型——认为这是一种合法的开发技术，反驳了其构成盗用的论点。一个关键的争议点是 Anthropic 没有签署该信，其 CEO 强调了威权政府带来的风险，并呼吁打击工业规模的蒸馏操作，但同时声称并不主张彻底禁止开放权重模型。

rss · Simon Willison · 8月2日 04:16

**背景**: 在 AI 领域，&\#x27;模型权重&\#x27;是构成神经网络所学&\#x27;知识&\#x27;的数值参数，决定了它如何处理输入以产生输出。&\#x27;开放权重&\#x27;指的是这些权重被公开发布的模型，允许任何人运行、研究和修改模型，这与可能包含完整训练代码和数据的&\#x27;开源&\#x27;有所不同。这场辩论的背景是，美国政府可能以安全为由，限制对强大开放模型的访问，以防止对手国家获得先进能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@aruna.kolluru/exploring-the-world-of-open-source-and-open-weights-ai-aa09707b69fc">Exploring the World of Open Source and Open Weights AI | Medium</a></li>
<li><a href="https://www.ultralytics.com/glossary/model-weights">What are Model Weights in AI? | Ultralytics</a></li>
<li><a href="https://techjacksolutions.com/ai-knowledge-hub/ai-model-licensing/">AI Model Licensing (Open-Weight vs Open-Source vs Closed) | AI Knowledge Hub - Tech Jacks Solutions</a></li>

</ul>
</details>

**标签**: `#AI Policy`, `#Open Source AI`, `#Industry Analysis`, `#AI Safety`

---

<a id="item-4"></a>
## [Kakehashi：一个在 Linux ARM 上运行 macOS 二进制文件的实验性用户空间项目](https://github.com/wie-project/kakehashi) ⭐️ 7.0/10

开发者 vlad\_kalinkin 发布了 Kakehashi，这是一个实验性的用户空间兼容层，旨在让 macOS 命令行二进制文件能在 Linux ARM 机器上原生运行。该项目目前已有针对 7-Zip、curl 和 Xcode Tools Git 的工作原型，其中 7-Zip 已通过多线程压缩测试，尽管其性能比原生 Linux 执行慢约 5.2 倍。 该项目解决了一个新颖的兼容性挑战，有望为日益增长的 Linux-on-ARM 服务器和开发环境（例如由 Apple Silicon Mac 或云 ARM 实例驱动的环境）解锁庞大的 macOS 命令行工具生态。这标志着在提升软件互操作性方面迈出了重要一步，并可能减少特定工作流对特定硬件平台的依赖。 该项目目前处于早期实验阶段，性能开销是一个主要限制，例如 7-Zip 有 5.2 倍的性能下降。它特别专注于 ARM 架构和命令行二进制文件，这使其与 Darling 等更广泛的项目（旨在在 x86 Linux 上实现完整的 macOS 应用程序兼容性）有所不同。

hackernews · vlad\_kalinkin · 8月2日 16:26 · [社区讨论](https://news.ycombinator.com/item?id=49145937)

**背景**: 在不同操作系统间运行二进制文件通常需要兼容层来转换系统调用并处理应用程序二进制接口（ABI）的差异。macOS 使用 Mach-O 二进制格式和 Darwin 内核，这与 Linux 的 ELF 格式和系统调用不同。现有的项目如 Darling 提供了一个用户空间兼容层，用于在 Linux 上运行 Darwin/macOS 二进制文件，但主要针对 x86 架构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Application_binary_interface">Application binary interface - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mach-O">Mach-O - Wikipedia</a></li>
<li><a href="https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=711581">#711581 - RFP: darling -- Userspace compatibility layer for running...</a></li>

</ul>
</details>

**社区讨论**: 社区表现出浓厚的兴趣和好奇，用户将其与 WINE/Proton 的成功相提并论，并询问其与 Darling 项目的关系。评论凸显了对其长期潜力的兴奋，特别是对于未来通过桥接工具运行 macOS 音频插件的可能性，同时也指出了项目处于早期阶段以及未来面临重大技术挑战。

**标签**: `#systems-programming`, `#binary-compatibility`, `#linux`, `#macos`, `#arm`

---