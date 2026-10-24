---
layout: default
title: "Horizon Summary: 2026-10-24 (ZH)"
date: 2026-10-24
lang: zh
---

> 从 7 条内容中筛选出 4 条重要资讯。

---

1. [安全研究人员演示利用漏洞链获取现代 iPhone 的 Root 权限](#item-1) ⭐️ 9.0/10
2. [Dessa：一款可在本地硬件上实现低延迟、富有表现力对话的全双工语音 AI 模型。](#item-2) ⭐️ 8.0/10
3. [Moonshot AI 发布 Kimi K3.1 Pro 及 K3.1 Pro Highspeed 模型，并刻意限制其攻击性网络能力。](#item-3) ⭐️ 7.0/10
4. [谷歌更新隐私政策，可能根据《数字市场法案》使用 Gmail 和照片数据进行广告投放。](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [安全研究人员演示利用漏洞链获取现代 iPhone 的 Root 权限](https://blog.calif.io/p/iphone) ⭐️ 9.0/10

一个安全研究团队成功演示了一个重要的漏洞利用链，使他们能够在一部现代 iPhone 上获得 root 权限。这一成就代表了 iOS 安全研究领域的一个重大突破，通常被称为“越狱”。 这一演示意义重大，因为它揭示了像 iOS 这样被广泛使用的封闭生态系统，即使在现代设备上，也可能存在潜在的安全漏洞。这对于安全研究人员、苹果的安全团队以及关心设备控制权的用户来说都很重要，因为它凸显了漏洞发现与平台加固之间持续不断的攻防战。 该漏洞利用涉及将多个漏洞串联起来，以实现任何单一漏洞都无法完成的深度入侵（root 权限）。该演示被公开分享，在技术社区内引发了关于其影响的实质性讨论。

hackernews · pavel\_lishin · 10月23日 16:21 · [社区讨论](https://news.ycombinator.com/item?id=50211474)

**背景**: “漏洞利用链”是指将多个漏洞组合起来入侵一个系统的序列，其整体攻击效果大于各部分之和。对 iPhone 进行“越狱”是移除 iOS 施加的软件限制以获得 root 权限的过程，这可以安装未经授权的软件，但也会增加安全风险。“零日”漏洞是软件厂商未知的安全缺陷，在补丁发布之前，它对攻击者和防御者都具有很高的价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.csoonline.com/article/571799/exploit-chains-explained-how-and-why-attackers-target-multiple-vulnerabilities.html">Exploit chains explained: How and why attackers target ...</a></li>
<li><a href="https://www.tomsguide.com/us/pictures-story/537-jailbreaking-iphone-pros-cons.html">10 Pros and Cons of Jailbreaking Your iPhone or iPad | Tom&#x27;s Guide</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区情绪混杂着对技术成果的钦佩和对生态系统控制的沮丧。主要观点包括：对因苹果集成生态系统（iCloud、iMessage 封锁）而失去早期类似 Android 的 DIY 自由感到惋惜；批评安全研究中排他的“红队”访问计划形成了“护城河”；以及提出了关于苹果的锁定模式或未来更新是否能缓解此类漏洞利用的实际问题。

**标签**: `#security`, `#ios`, `#reverse-engineering`, `#jailbreak`, `#zero-day`

---

<a id="item-2"></a>
## [Dessa：一款可在本地硬件上实现低延迟、富有表现力对话的全双工语音 AI 模型。](https://block.xyz/dessa) ⭐️ 8.0/10

Dessa 是一款新的全双工语音模型，能够实现低延迟、富有表现力的对话，并可在 MacBook Pro M4 Max 等高端消费级硬件上本地运行。据报道，其训练计算相对高效，仅使用了一台 NVIDIA GB200 NVL72 系统。 这很重要，因为它将逼真的实时语音 AI 交互从云端推向了个人设备，增强了隐私性和可访问性。它表明，通过更高效的训练和边缘部署，可以实现高度表现力、低延迟的对话式 AI，这可能在个人助理、游戏和辅助工具中催生新的应用。 该模型能够在 MacBook Pro M4 Max 上本地运行，表明其在边缘计算方面进行了显著优化。然而，社区评论对其&\#x27;有史以来最真实&\#x27;的营销宣传表示怀疑，并指出其训练数据可能包含大量播客内容。

hackernews · dsr12 · 10月23日 19:09 · [社区讨论](https://news.ycombinator.com/item?id=50213925)

**背景**: 全双工语音模型是能够同时听和说的 AI 系统，可以实现自然、重叠的对话和动态的轮流发言，这与传统的轮流式语音助手不同。AI 的边缘计算涉及在本地设备而非云端运行模型，这可以降低延迟、增强隐私，并允许在带宽有限的环境中运行。训练此类大型 AI 模型通常需要巨大的计算资源，因此用&\#x27;相对高效的计算&\#x27;取得类似成果是一项显著的技术挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/full-duplex-speech-llms">Full - Duplex Speech LLMs</a></li>
<li><a href="https://arxiv.org/html/2609.34461">CharDuplex: Building Character-Consistent Full - Duplex Spoken...</a></li>
<li><a href="https://www.mdpi.com/2078-2489/16/8/685">Real-Time Speech-to-Text on Edge: A Prototype System for ...</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，既有技术上的钦佩，也有怀疑。一些用户对其低延迟的本地性能和高效的训练表示印象深刻。另一些用户则批评其耸人听闻的标题是营销炒作，对演示对话中&\#x27;AI 女友&\#x27;的风格感到不适，并质疑训练数据的性质，推测其大量基于播客内容。

**标签**: `#speech-synthesis`, `#ai-models`, `#edge-computing`, `#machine-learning`, `#real-time`

---

<a id="item-3"></a>
## [Moonshot AI 发布 Kimi K3.1 Pro 及 K3.1 Pro Highspeed 模型，并刻意限制其攻击性网络能力。](https://www.kimi.ai/blog/kimi-k3-1-pro) ⭐️ 7.0/10

Moonshot AI 宣布发布 Kimi K3.1 Pro 和 K3.1 Pro Highspeed AI 模型，这是 K3 系列的更新版本。该公司明确表示，K3.1 Pro 的开放权重版本，其攻击性网络能力被刻意限制在其内部流水线所能达到的水平之下，也低于前沿的专有模型。 此次发布意义重大，因为它代表了一家领先 AI 公司的一次重要更新，其性能在基准测试中有所提升。更重要的是，它突显了行业内日益激烈的关于负责任地发布强大 AI 模型的辩论，特别是是否以及如何限制这些模型在网络安全等领域的潜在滥用。 K3.1 Pro 模型在数据分析基准测试中表现出显著的性能跃升，得分达到 98%，而 K3 为 81%，不过有评测指出其速度较慢，原因是进行了更多的工具调用。该模型架构基于 K3 系列，采用了 Kimi Delta Attention \(KDA\) 和 Attention Residuals \(AttnRes\) 以提高效率。

hackernews · Jowsey · 10月23日 16:59 · [社区讨论](https://news.ycombinator.com/item?id=50212065)

**背景**: Kimi K3 是 Moonshot AI 推出的大型多模态推理模型，采用 2.8 万亿参数的架构。它采用了新颖的 Kimi Delta Attention \(KDA\) 机制和稀疏的专家混合 \(MoE\) 设计，在 896 个专家中仅激活 16 个以提高计算效率。AI 模型中的“攻击性网络能力”指的是其协助进行漏洞发现、漏洞利用开发或网络入侵等活动的潜力，这引发了双重用途的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3">moonshotai/ Kimi -K3 · Hugging Face</a></li>
<li><a href="https://openrouter.ai/moonshotai/kimi-k3">Kimi K3 - API Pricing &amp; Benchmarks | OpenRouter</a></li>
<li><a href="https://pentesttoday.com/blog/open-weights-models-offensive-cyber">Open weights models are surprisingly aligned on offensive cyber</a></li>

</ul>
</details>

**社区讨论**: 社区讨论突出了几点：用户注意到 Kimi 与其他模型相比，具有独特的直率甚至好辩的个性。一些用户观察到模型在推理过程中自我身份识别存在不一致。有用户抱怨订阅配额限制过于严格，而公司关于在开放版本中刻意限制模型攻击性网络能力的声明引发了重大辩论，用户质疑其理由和影响。

**标签**: `#ai-models`, `#llm`, `#open-source`, `#cybersecurity`, `#model-evaluation`

---

<a id="item-4"></a>
## [谷歌更新隐私政策，可能根据《数字市场法案》使用 Gmail 和照片数据进行广告投放。](https://www.theverge.com/tech/1017600/google-personal-intelligence-privacy-policy-ads-update) ⭐️ 7.0/10

谷歌更新了其隐私政策，声明其可能使用来自 Gmail 和 Google Photos 等服务的数据进行个性化广告投放。这一变化与欧盟《数字市场法案》中关于服务关联的条款有具体关联。 这一政策转变可能显著扩大谷歌用于广告定位的个人数据范围，直接影响用户隐私。它也凸显了大型科技公司如何根据《数字市场法案》等旨在监管&\#x27;守门人&\#x27;平台的新法规来调整其数据实践。 该政策澄清，除非用户选择将这些服务与支持个性化广告的其他谷歌服务关联，否则不会使用这些服务的数据进行广告投放，这是社区讨论中强调的一个细微差别。此次更新与《数字市场法案》第 5\(2\)条有关，该条款要求守门人平台为用户提供关联某些核心平台服务的选择。

hackernews · JustSkyfall · 10月23日 19:34 · [社区讨论](https://news.ycombinator.com/item?id=50214218)

**背景**: 《数字市场法案》是一项于 2024 年 3 月生效的欧盟法规，旨在通过监管大型数字&\#x27;守门人&\#x27;平台来确保公平竞争。谷歌作为被指定的守门人，必须遵守相关规则，例如允许用户选择是否关联其核心服务（如搜索、YouTube、Chrome）。此前，谷歌曾声明来自 Google Photos 等服务的数据不用于广告目的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://digital-markets-act.ec.europa.eu/index_en">Digital Markets Act</a></li>
<li><a href="https://blog.internxt.com/google-activity-history/">How to Monitor Your Google Activity History | Internxt Blog</a></li>
<li><a href="https://www.google.ru/photos/about/?hl=e">Google Photos : Edit, Organize, Search, and Backup Your Photos</a></li>

</ul>
</details>

**社区讨论**: 社区评论澄清，这一变化比笼统的数据收集更为微妙，指出广告使用取决于用户是否根据 DMA 规则选择关联服务。一些用户表示怀疑，将&\#x27;可能&\#x27;解读为&\#x27;绝对会&\#x27;，而另一些用户则分享了实用建议，例如关闭个性化设置或将照片迁移到 Immich 等替代服务。

**标签**: `#privacy`, `#google`, `#advertising`, `#policy`, `#dma`

---