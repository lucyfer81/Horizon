---
layout: default
title: "Horizon Summary: 2026-10-10 (ZH)"
date: 2026-10-10
lang: zh
---

> 从 12 条内容中筛选出 5 条重要资讯。

---

1. [Cloudflare 收购 Deno，计划一年后停止维护 Deno 运行时](#item-1) ⭐️ 9.0/10
2. [Typesafe AI 以 75 亿美元估值融资 8.7 亿美元。](#item-2) ⭐️ 8.0/10
3. [密码学家警告 AI 可能攻破公钥加密，敦促立即准备。](#item-3) ⭐️ 8.0/10
4. [Oxide Computer 宣布完成 4.45 亿美元 D 轮融资](#item-4) ⭐️ 7.0/10
5. [YouTuber 自制类似 Flock 的自动车牌识别摄像头追踪警车后遭警方上门。](#item-5) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Cloudflare 收购 Deno，计划一年后停止维护 Deno 运行时](https://simonwillison.net/2026/Oct/9/deno-is-joining-cloudflare/) ⭐️ 9.0/10

Cloudflare 已收购 Deno，其主要目标是将 Deno 的开源项目 \`celld\` 整合进来，使自托管 \`workerd\` 运行时成为 Workers 编程模型的一流选择。但 Cloudflare 仅会为独立的 Deno 运行时提供一年的月度更新支持，之后将停止其开发。 此次收购标志着无服务器和边缘计算领域的一次重大整合，Cloudflare 正在吸收关键人才和技术以强化其 Workers 平台。计划停止 Deno 作为独立运行时的开发，对 JavaScript/TypeScript 生态系统是一个重大转变，可能会将创新方向引向 Cloudflare 专有的边缘模型。 Deno 的创造者 Ryan Dahl 同意这一决定，他表示 Deno 已&\#x27;陷入 Node 兼容性的引力阱&\#x27;，他现在更感兴趣的是构建像 \`celld\` 这样的新抽象。\`celld\` 项目是一个开源守护进程，实现了 Cloudflare 的 Durable Objects 模式，允许 Workers 应用在用户控制的基础设施上运行。

rss · Simon Willison · 10月9日 22:48

**背景**: Deno 是由 Node.js 的原始创造者 Ryan Dahl 创建的一个安全的 JavaScript 和 TypeScript 运行时，旨在解决 Node.js 的设计缺陷。Cloudflare Workers 是一个用于在边缘部署代码的无服务器平台，由其 \`workerd\` 运行时驱动。Durable Objects 是 Cloudflare Workers 的一项功能，通过将计算与存储结合在一个分布式对象中，提供全局一致的有状态存储。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.everydev.ai/tools/celld">celld - Self-Hosted Durable Objects Runtime | EveryDev.ai</a></li>
<li><a href="https://confidence.sh/blog/how-to-self-host-cloudflare/">How To Self - Host Cloudflare</a></li>
<li><a href="https://developers.cloudflare.com/durable-objects/">Overview · Cloudflare Durable Objects docs</a></li>

</ul>
</details>

**社区讨论**: 社区情绪主要是失望和批评，用户对 Deno 事实上的终结表示遗憾，并将此次收购视为一次导致开发停止的&\#x27;收购式招聘&\#x27;。一些评论者指出，Deno 向 Node.js 兼容性的转变稀释了其最初的愿景，而另一些人则强调了大型科技公司整合开发者工具的广泛趋势。

**标签**: `#deno`, `#cloudflare`, `#acquisition`, `#serverless`, `#javascript`

---

<a id="item-2"></a>
## [Typesafe AI 以 75 亿美元估值融资 8.7 亿美元。](https://typesafe.ai/blog/series-ai) ⭐️ 8.0/10

AI 实验室 Typesafe AI 完成了一轮 8.7 亿美元的融资，公司估值达到 75 亿美元。此前，该公司于 2026 年 9 月脱离隐身模式，并获得了 4000 万美元的初始融资。 这笔巨额融资表明投资者对前沿 AI 领域，特别是专注于自动化决策的基础设施，抱有强烈信心。它凸显了开发能在软件系统内运行的专用 AI 模型所面临的激烈竞争和高风险。 该公司的旗舰产品是名为&\#x27;Jev&\#x27;的首个&\#x27;System One&\#x27;模型，专为在软件内进行快速、结构化的决策而设计。然而，社区讨论指出，类似的&\#x27;决策模型&\#x27;已迅速涌现，包括 OpenAI 和微软的同类产品，这引发了对其产品技术护城河的质疑。

hackernews · tosh · 10月9日 17:02 · [社区讨论](https://news.ycombinator.com/item?id=50023450)

**背景**: Typesafe AI 是一家位于旧金山的前沿 AI 实验室，致力于构建&\#x27;面向自动化的机器原生智能基础设施&\#x27;。其重点是创建旨在软件内部进行决策的 AI 模型，这与通用大语言模型（LLM）是不同的范式。该公司的首个模型 Jev 被定位为一个用于快速、结构化决策的系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://typesafe.ai/">Home - TypeSafe AI</a></li>
<li><a href="https://jevwiki.ai/wiki/entities/typesafe-ai.md">TypeSafe AI ( company ) — jevwiki. ai</a></li>
<li><a href="https://onemetrik.com/market-insights/jev-ai-typesafe-system-one-model/">Jev AI : What TypeSafe ’s System One Model Means for... - OneMetrik</a></li>

</ul>
</details>

**社区讨论**: 社区对此次估值表示怀疑，鉴于 OpenAI、微软和开源项目迅速推出了竞争性的决策模型，他们对 Typesafe 的&\#x27;Jev&\#x27;模型的技术护城河提出了质疑。一些评论者承认该公司强大的营销和工程能力，但争论仅凭品牌认知是否足以支撑 75 亿美元的估值。

**标签**: `#venture-capital`, `#artificial-intelligence`, `#funding`, `#startups`, `#business`

---

<a id="item-3"></a>
## [密码学家警告 AI 可能攻破公钥加密，敦促立即准备。](https://simonwillison.net/2026/Oct/9/matthew-green/) ⭐️ 8.0/10

密码学家 Matthew Green 公开警告，AI 的进步存在不小的可能性会从功能上攻破现有的公钥加密算法，他估计这一概率为 15%。他强调，AI 产生“意外”的速度，远超人类（即使有 AI 辅助）替换密码标准的速度，因此提前准备至关重要。 这很重要，因为公钥加密是现代互联网安全的基石，支撑着 HTTPS、数字签名和安全通信。如果 AI 驱动的突破突然攻破这些算法，将在充分的防御措施准备就绪之前，对全球数字安全、金融系统和个人隐私造成灾难性破坏。 Green 特别提到了假设性的“Minicrypt”世界，在那里公钥加密是不可能的。他的警告并非针对量子计算，而是针对 AI 不可预知的能力，并强调应对措施依赖于现在所做的准备工作，因为反应滞后期非常巨大。

rss · Simon Willison · 10月9日 15:02

**背景**: 公钥密码学（如 RSA 和 Diffie-Hellman）使用一对密钥（公钥和私钥）来保障通信安全，是互联网安全的基础。Russell Impagliazzo 提出的“Minicrypt”是计算复杂性理论中的一个理论框架，描述了一个单向函数存在但公钥加密不可能的世界。虽然量子计算是当前密码学已知的未来威胁，但 Green 的警告聚焦于 AI 可能以远超预期的速度发现新的数学弱点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.technologyreview.com/2022/09/14/1059400/explainer-quantum-resistant-algorithms/">What are quantum-resistant algorithms —and why do we need them?</a></li>
<li><a href="https://www.linkedin.com/posts/subramanian-sekar-591142318_ai-cybersecurity-cryptography-activity-7488423763966038016-52sb">AI Breaks Post-Quantum Cryptography Candidate HAWK | LinkedIn</a></li>

</ul>
</details>

**标签**: `#cryptography`, `#ai-risk`, `#security`, `#public-key-encryption`

---

<a id="item-4"></a>
## [Oxide Computer 宣布完成 4.45 亿美元 D 轮融资](https://oxide.computer/blog/our-445m-series-d) ⭐️ 7.0/10

Oxide Computer Company 宣布在其官方网站的博客文章中披露，公司已完成一轮 4.45 亿美元的 D 轮融资。 这笔巨额融资表明投资者对 Oxide 面向云基础设施的集成式软硬件平台充满信心。它为公司提供了大量资金，用于扩大运营规模、履行客户订单，并有可能在对抗现有云服务提供商时扩大其市场地位。 对于通常发生在更成熟初创公司阶段的 D 轮融资而言，这笔融资金额非常巨大。虽然提供的资料中未指明具体的领投方，但其规模暗示了主要风险投资机构或机构投资者的参与。

hackernews · ahlCVA · 10月9日 13:12 · [社区讨论](https://news.ycombinator.com/item?id=50020014)

**背景**: Oxide Computer Company 构建了一个集成平台，将计算、存储、网络和软件整合到单个机架中，旨在在本地提供与公共云基础设施一样的效率和简洁性。D 轮融资是后期风险投资轮次，通常适用于寻求大规模扩张、进军新市场或为收购或 IPO 做准备的成熟公司。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://oxide.computer/">Oxide Computer Company</a></li>
<li><a href="https://www.investopedia.com/articles/personal-finance/102015/series-b-c-funding-what-it-all-means-and-how-it-works.asp">investopedia.com/articles/personal-finance/102015/ series -b-c- funding ...</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体积极，赞扬了 Oxide 的产品和鼓舞人心的公司文化。然而，讨论中也包含了对冗长招聘流程的批评，以及对选择股权融资而非债务融资的战略性质疑。一些用户表示希望公司减少对 AI 工作负载的营销宣传，以保持其独特的品牌形象。

**标签**: `#hardware`, `#funding`, `#servers`, `#startups`, `#cloud-infrastructure`

---

<a id="item-5"></a>
## [YouTuber 自制类似 Flock 的自动车牌识别摄像头追踪警车后遭警方上门。](https://gizmodo.com/youtuber-says-cops-paid-him-a-visit-after-he-built-flock-style-camera-to-track-cops-2000824306) ⭐️ 7.0/10

一位 YouTuber 报告称，在他制造并演示了一款模仿 Flock Safety 技术的 DIY 自动车牌识别摄像头系统（用于追踪警车）后，警察上门拜访了他。此事发生在他公开演示这个开源硬件项目之后。 这一事件凸显了围绕大规模监控技术的权力动态和法律灰色地带，引发了关于谁有权使用该技术以及用于何种目的的关键问题。它加剧了执法公共监控与公民使用类似工具进行问责之间的紧张关系，引发了关于隐私、合法性和权力不对称的辩论。 这位 YouTuber 的项目专门针对警车，将一种通常由当局使用的监控工具反过来用于监控当局本身。警方的上门拜访表明，当局正在监控并可能试图阻止公众复制和使用此类监控技术来针对他们。

hackernews · gumby · 10月9日 21:06 · [社区讨论](https://news.ycombinator.com/item?id=50026555)

**背景**: Flock Safety 是一家主要的美国公司，制造和运营自动车牌识别摄像头系统，被执法部门和社区广泛用于公共安全和破案。ALPR 技术能自动捕获车牌数据和车辆特征，创建可搜索的车辆移动数据库。DIY 监控系统指的是个人可以组装的、通常是开源硬件和软件的自建监控项目，其功能与商业产品类似，但用户控制权更大。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://github.com/funnybrum/sharp_eye">GitHub - funnybrum/sharp_eye: DIY surveillance system capable of...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示出对立法解决方案（如新罕布什尔州严格的 ALPR 数据保留法）的强烈支持，以遏制大规模监控。关于“反向监控”的伦理存在激烈辩论，一些人认为这创造了必要的权力制衡，而另一些人则认为包括政府在内的任何人都不应使用此类技术。评论还表达了对于美国公众对此类监控缺乏愤怒的沮丧，并将其与其他国家的类似监控情况进行了对比。

**标签**: `#surveillance`, `#privacy`, `#police-accountability`, `#open-source-hardware`, `#ALPR`

---