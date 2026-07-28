---
layout: default
title: "Horizon Summary: 2026-07-28 (ZH)"
date: 2026-07-28
lang: zh
---

> 从 9 条内容中筛选出 8 条重要资讯。

---

1. [vLLM v0.26.0 发布，支持 Inkling 模型家族、深度优化 DeepSeek-V4 并提升生成准确性。](#item-1) ⭐️ 8.0/10
2. [Anthropic CEO 主张对所有能力强大的 AI 模型（包括开源权重模型）进行强制性安全测试。](#item-2) ⭐️ 8.0/10
3. [法官驳回谷歌利用 DMCA 阻止搜索结果抓取的企图](#item-3) ⭐️ 8.0/10
4. [微软发布其首个 AI 网络安全模型 MAI-Cyber-1-Flash，并集成至 MDASH 平台。](#item-4) ⭐️ 8.0/10
5. [月之暗面发布 2.8 万亿参数 Kimi K3 模型权重，附带新颖的许可条款。](#item-5) ⭐️ 8.0/10
6. [案例研究：用 HTMX 替换 React.js 以实现服务器驱动的 UI 交互性](#item-6) ⭐️ 7.0/10
7. [Libsm64：将《超级马里奥 64》游戏逻辑打包成库，供外部游戏引擎使用。](#item-7) ⭐️ 7.0/10
8. [分析指出 AI 使用指南已从聊天模型转向智能体系统](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0 发布，支持 Inkling 模型家族、深度优化 DeepSeek-V4 并提升生成准确性。](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 全面支持新的 Inkling 多模态 MoE 模型家族，并为 DeepSeek-V4 在 NVIDIA、AMD 和 Intel 硬件上提供了重大性能优化。该版本还新增了 \`head\_dtype\` 功能以支持 fp32 \`lm\_head\` 来提升生成准确性，并使其 KV 卸载与分层存储系统更加成熟。 此次发布通过支持一个先进的多模态模型显著扩展了 vLLM 的模型生态，并对领先的开源模型 DeepSeek-V4 进行了性能极限优化，直接惠及运行高吞吐量推理的开发者与企业。广泛的硬件优化和准确性提升巩固了 vLLM 作为生产部署中多功能、高性能推理引擎的地位。 对 Inkling 的支持栈包含多项专门功能，例如分段 CUDA 图、Hopper FA4 相对注意力以及 MTP=1 推测解码。DeepSeek-V4 的性能提升源自新的路由内核（端到端 TPOT 提升 2.94%）、\`fused\_topk\_bias\` 内核（1.5–2 倍加速）以及冗余重复/复制移除（端到端 TPOT 提升 1.8%）。

github · khluu · 7月27日 01:06

**背景**: vLLM 是一个用于大语言模型的高吞吐量、内存高效的推理和服务引擎。Inkling 模型家族由 Thinking Machines 开发，是一个多模态混合专家模型，总参数量达 9750 亿，激活参数量为 410 亿，能够对文本、图像和音频输入进行推理。FlashAttention-4 是针对 NVIDIA Hopper 架构的优化注意力实现，相比前代版本提供了性能提升，尤其对于长上下文任务。MTP 是一种推测解码技术，允许模型在单次前向传播中预测多个未来 token，从而提高推理吞吐量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/inkling/">Inkling - Thinking Machines Lab</a></li>
<li><a href="https://modal.com/blog/reverse-engineer-flash-attention-4">We reverse-engineered Flash Attention 4</a></li>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM</a></li>

</ul>
</details>

**标签**: `#LLM Inference`, `#Performance Optimization`, `#vLLM`, `#Model Serving`, `#Hardware Acceleration`

---

<a id="item-2"></a>
## [Anthropic CEO 主张对所有能力强大的 AI 模型（包括开源权重模型）进行强制性安全测试。](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic 的 CEO Dario Amodei 阐述了公司立场，主张对所有能力足够强大的 AI 模型（包括开源权重模型）进行强制性安全测试，同时明确反对彻底禁止这类模型。该立场还包括支持禁止向中国销售芯片等措施以防止滥用。 这一立场意义重大，因为它直接影响了正在进行的全球 AI 监管辩论，在安全关切与开源 AI 的好处之间寻求平衡。它可能影响政策决策，从而改变全球范围内开源和闭源 AI 模型的开发、部署和治理方式。 该提案要求由独立的第三方审计机构进行测试，如果模型被认为不安全，政府有权阻止其部署。一个关键的注意事项是，提案没有具体说明由谁来管理测试、测试成本以及通过标准，这些正是社区担忧可能产生监管俘获的核心问题。

hackernews · surprisetalk · 7月27日 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开源权重 AI 模型是指其训练好的参数（权重）可公开下载和使用，从而支持定制化和本地部署的模型。强制性安全测试指的是一种制度，要求模型（尤其是前沿 AI）在部署前需由独立审计机构进行风险评估。Anthropic 是一家领先的 AI 安全和研究公司。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>
<li><a href="https://aisecurityandsafety.org/en/guides/ai-model-evaluation/">AI Model Evaluation: Safety Benchmarks, Red Teaming &amp; Testing ...</a></li>
<li><a href="https://www.politico.com/news/2026/06/10/anthropic-backs-mandatory-vetting-for-frontier-ai-models-00957632">Anthropic backs mandatory testing for frontier AI models</a></li>

</ul>
</details>

**社区讨论**: 社区情绪主要是批评和怀疑。关键担忧包括指责这是监管俘获，即如果测试成本过高或访问被拒绝，强制性测试可能被用作事实上的禁令。评论者还指出，在反对模型禁令的同时支持硬件（芯片）禁令是虚伪的，并质疑安全论点的诚意，认为这是一种扼杀竞争的策略。

**标签**: `#AI Policy`, `#Open Source AI`, `#AI Safety`, `#Industry Debate`

---

<a id="item-3"></a>
## [法官驳回谷歌利用 DMCA 阻止搜索结果抓取的企图](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

一名法官驳回了谷歌试图利用《数字千年版权法案》\(DMCA\) 来阻止第三方服务 SerpAPI 抓取其公开搜索结果的行为。这项于 2026 年作出的裁决，直接挑战了利用版权法限制访问公开数据的做法。 这项裁决确立了一个重要的法律先例，确认抓取公开可访问的数据通常是合法的，不能轻易被版权主张所阻止。它影响了那些在限制 API 访问的同时又试图控制数据流的公司，可能有助于维护数据依赖型服务领域的竞争与创新。 此案凸显了美国法律中的区别：版权保护要求最低限度的创造性，这与欧盟保护实质性投资的数据库权利不同。一个关键因素是谷歌自己废弃了其搜索 API，这恰恰催生了 SerpAPI 等服务所填补的市场需求。

hackernews · cdrnsf · 7月27日 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49073513)

**背景**: 《数字千年版权法案》\(DMCA\) 是 1998 年颁布的美国法律，旨在保护数字版权持有者免受在线盗版侵害。网络抓取涉及使用自动化工具从网站提取数据，其合法性通常取决于数据是否公开可访问以及访问方法。在美国，像 hiQ Labs 诉 LinkedIn 这样的法院裁决已经确立，抓取公开可用的数据通常是合法的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.scrapingbee.com/blog/is-web-scraping-legal/">Is Web Scraping Legal? Key Insights and Guidelines You Need to Know | ScrapingBee</a></li>
<li><a href="https://cloro.dev/blog/website-scraping-legal/">Is Website Scraping Legal? 2026 Rules (US + EU) | cloro</a></li>
<li><a href="https://dmcaforce.com/what-are-dmca-claims-and-copyright-violations/">What are DMCA Claims and Copyright Violations? - DMCA Force</a></li>

</ul>
</details>

**社区讨论**: 社区情绪大多批评谷歌的立场是虚伪的，考虑到其自身就起源于网络爬虫。关键观点包括对谷歌废弃其官方搜索 API 的失望（这迫使人们依赖第三方抓取工具），以及对美国版权法与欧盟数据库权利之间法律差异的观察。还有人强调了抓取在揭露广告骗局方面的公共利益。

**标签**: `#legal`, `#web-scraping`, `#copyright`, `#google`, `#api`

---

<a id="item-4"></a>
## [微软发布其首个 AI 网络安全模型 MAI-Cyber-1-Flash，并集成至 MDASH 平台。](https://microsoft.ai/news/introducing-mai-cyber-1-flash-inside-mdash/) ⭐️ 8.0/10

微软推出了其首个专为网络安全设计的 AI 模型 MAI-Cyber-1-Flash，并将其集成到其 MDASH（多模型智能体安全平台）中。该模型采用安全优先的方法开发，并经过了微软 AI 红队的严格评估。 这标志着将大语言模型应用于自动化和增强网络安全防御的重要一步，有望为企业将安全模型成本减半的同时提高检测准确性。它预示着行业的一个重大转变，即 AI 智能体可能成为大规模漏洞发现和修复不可或缺的一部分。 该模型与 MDASH 平台集成，该平台专为跨微软软件环境的自动化、大规模代码审计和漏洞研究而设计。微软声称该模型展示了 AI 如何在提升检测能力的同时实现成本效益，鉴于软件漏洞日益复杂，这是一个关键因素。

hackernews · migmartri · 7月27日 16:52 · [社区讨论](https://news.ycombinator.com/item?id=49072361)

**背景**: MDASH，即多模型智能体扫描平台，是微软于 2026 年中宣布的 AI 驱动平台，用于大规模自动化漏洞发现。它是一个“智能体”系统，意味着可以部署 AI 智能体团队来执行代码审计等任务。更广泛的趋势涉及使用大语言模型（LLM）来处理和分析安全系统生成的海量数据，以更高效地识别威胁和漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://microsoft.ai/news/introducing-mai-cyber-1-flash-inside-mdash/">Introducing MAI - Cyber - 1 - Flash inside MDASH | Microsoft AI</a></li>
<li><a href="https://runtimewire.com/article/microsoft-mai-cyber-1-flash-mdash-launch">Microsoft launches MAI - Cyber - 1 - Flash , a cost‑efficient AI security...</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/05/12/defense-at-ai-speed-microsofts-new-multi-model-agentic-security-system-tops-leading-industry-benchmark/">Defense at AI speed: Microsoft’s new multi-model agentic security system tops leading industry benchmark | Microsoft Security Blog</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，对实际可访问性和微软的执行记录持怀疑态度。一条评论质疑该模型的优势是否主要源于微软自身产品漏洞的内部数据。其他人则对访问路径不明确表示失望，并以过去产品命名不一致为由主张保持谨慎。

**标签**: `#AI`, `#Cybersecurity`, `#Microsoft`, `#Large-Language-Models`

---

<a id="item-5"></a>
## [月之暗面发布 2.8 万亿参数 Kimi K3 模型权重，附带新颖的许可条款。](https://simonwillison.net/2026/Jul/27/kimi-k3/#atom-everything) ⭐️ 8.0/10

月之暗面（Moonshot AI）已在 Hugging Face 上发布了其 2.8 万亿参数的 Kimi K3 大语言模型的权重，模型文件大小高达 1.56TB。此次发布附带了一份自定义许可证，要求大型 &\#x27;模型即服务&\#x27; 企业必须与月之暗面签订单独的协议。 此次发布意义重大，因为它让全球最大的语言模型之一可供研究和商业使用，可能加速相关领域的创新。这种新颖的 &\#x27;开放权重&\#x27; 许可方式开创了一个先例，展示了 AI 公司如何在共享模型权重的同时，寻求对其最先进模型的商业使用进行货币化或控制。 该许可证是一个修改版的 MIT 许可证，专门针对大规模商业用户，要求年收入超过 2000 万美元的 &\#x27;模型即服务&\#x27; 企业签订单独协议。该模型现已在 OpenRouter 等平台上提供推理服务，定价为每百万输入 token 3 美元，每百万输出 token 15 美元。

rss · Simon Willison · 7月27日 23:39

**背景**: 在机器学习中，&\#x27;权重&\#x27; 是神经网络中在训练过程中学习到的数值参数，决定了模型如何处理信息。发布模型权重允许他人在无需重新训练的情况下运行模型，但这与 &\#x27;开源&\#x27; 不同，后者通常包括模型的代码和训练数据。万亿参数模型代表了 AI 规模的尖端水平，突破了计算能力的边界，但需要巨大的资源进行训练和推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-are-weights">What are Weights? - Stanford HAI</a></li>
<li><a href="https://developer.nvidia.com/blog/demystifying-ai-inference-deployments-for-trillion-parameter-large-language-models/">Demystifying AI Inference Deployments for Trillion Parameter Large ...</a></li>
<li><a href="https://milvus.io/ai-quick-reference/how-does-the-mit-license-work">How does the MIT license work?</a></li>

</ul>
</details>

**标签**: `#llm`, `#open-source`, `#model-weights`, `#ai-ethics`, `#huggingface`

---

<a id="item-6"></a>
## [案例研究：用 HTMX 替换 React.js 以实现服务器驱动的 UI 交互性](https://misago-project.org/t/removing-reactjs-from-the-codebase-and-adapting-htmx-for-ui-interactivity/1267/) ⭐️ 7.0/10

一个项目详细介绍了从其代码库中移除 React.js 客户端框架，并用 HTMX 取而代之，以直接从服务器处理 UI 交互性。这次迁移代表了从繁重的 JavaScript 单页应用架构向以服务器为中心、超媒体驱动的方法转变。 这个案例研究很重要，因为它突显了一个日益增长的趋势：重新考虑使用复杂的前端框架，转而采用更简单的服务器渲染架构，这可以减少客户端复杂性、改善初始加载性能，并简化以内容为中心的应用开发。它为评估类似架构转变的开发者提供了一个现实世界的蓝图，特别是对于像论坛这样需要动态更新但不需要完整 SPA 复杂性的应用。 讨论强调，HTMX 特别适合论坛软件，因为其内容主要是静态 HTML，而实时更新等交互性可以通过服务器发送事件实现。然而，一条社区评论指出一个性能上的注意事项：在单个响应中发送大型 HTML 片段（例如，带有选择列表的复杂表单）可能导致用户体验变慢。

hackernews · Ralfp · 7月27日 09:58 · [社区讨论](https://news.ycombinator.com/item?id=49067301)

**背景**: HTMX 是一个客户端 JavaScript 库，允许开发者直接从 HTML 属性访问 AJAX、CSS 过渡和 WebSockets 等现代浏览器功能，从而实现动态更新而无需编写大量 JavaScript。它提倡一种超媒体驱动的架构，服务器用 HTML 片段进行响应，以替换页面的部分内容。这与 React.js 等框架形成对比，后者通常在客户端管理整个 UI 状态和渲染逻辑，需要更多 JavaScript 并且通常需要一个单独的 API 后端。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://htmx.org/docs/">htmx ~ Documentation</a></li>
<li><a href="https://mvolkmann.github.io/blog/htmx/">htmx | Mark Volkmann&#x27;s Tech Blog</a></li>

</ul>
</details>

**社区讨论**: 社区对 HTMX 的情绪基本是积极的，用户称赞它适合服务器渲染的应用、论坛，甚至渐进式网络应用，并且常与 Tailwind 等实用优先的 CSS 框架搭配使用。一些人分享了实践经验，例如大型 HTML 负载导致的性能问题，而另一些人则建议将其用于大多数用例，仅将迷你 React/Vue 应用保留用于高度自定义的交互性。讨论中还提到了其他服务器驱动的 UI 方法，例如受 Phoenix LiveView 启发的方法。

**标签**: `#web-development`, `#htmx`, `#react`, `#architecture`, `#frontend`

---

<a id="item-7"></a>
## [Libsm64：将《超级马里奥 64》游戏逻辑打包成库，供外部游戏引擎使用。](https://github.com/libsm64/libsm64) ⭐️ 7.0/10

libsm64 项目发布了一个共享库，它提取了《超级马里奥 64》的核心游戏逻辑、物理和渲染功能，使开发者能够在 Unity 或 Unreal 等外部游戏引擎中导入并控制马里奥角色。该库在运行时需要用户提供一个官方的《超级马里奥 64》ROM 文件来获取纹理和动画数据。 这代表了一种新颖且富有创意的游戏角色可移植性方案，使得一个备受喜爱且机制复杂的游戏角色能够被用于全新的场景和粉丝项目中。它展示了一种无需炒作、切实可行的方法，实现了跨引擎的角色互操作性，这一概念通常与“元宇宙”或区块链的承诺相关。 该库建立在社区驱动的《超级马里奥 64》反编译项目之上，旨在通过 C API 集成到其他应用程序中。一个关键的限制是它不分发任天堂的受版权保护的资产；用户必须提供自己合法获得的 ROM 文件，库会使用该文件提取必要的数据。

hackernews · klaussilveira · 7月27日 10:04 · [社区讨论](https://news.ycombinator.com/item?id=49067352)

**背景**: 《超级马里奥 64》是 1996 年为任天堂 64 主机发布的具有里程碑意义的 3D 平台游戏。近年来，一个社区驱动的逆向工程和反编译项目成功地从原始机器代码中重建了游戏的源代码，使得深入理解和修改成为可能。此类反编译项目使得游戏的逻辑能够与其原始引擎和资产分离，这正是 libsm64 等工具的基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/libsm64/libsm64">GitHub - libsm64/libsm64: Mario 64 as a library for use in ...</a></li>
<li><a href="https://github.com/n64decomp/sm64">GitHub - n64decomp/sm64: A Super Mario 64 decompilation ...</a></li>
<li><a href="https://deepwiki.com/libsm64/libsm64/4.2-integration-guidelines">Integration Guidelines | libsm64/libsm64 | DeepWiki</a></li>

</ul>
</details>

**社区讨论**: 社区反响非常积极和兴奋，赞扬了该库的创意前提，并分享了马里奥在《半条命 2》等游戏中的演示视频。评论者指出，它实现了跨游戏角色可移植性的承诺，却没有“元宇宙”或加密项目相关的炒作。其他人则幽默地警告任天堂注意潜在的商业滥用，还有一些人询问设置的简易性，并指向了使用该库的精选项目列表。

**标签**: `#game-development`, `#reverse-engineering`, `#library`, `#emulation`, `#creative-coding`

---

<a id="item-8"></a>
## [分析指出 AI 使用指南已从聊天模型转向智能体系统](https://simonwillison.net/2026/Jul/27/an-opinionated-guide-to-which-ai-to-use-to-do-stuff/#atom-everything) ⭐️ 7.0/10

Simon Willison 分析了 Ethan Mollick 关于 AI 使用的“观点性指南”的最新更新，指出其重点已从一年前关注 ChatGPT、Claude 等聊天模型，显著演变为当前强调 ChatGPT Work、Claude Cowork 等智能体系统。该指南现在着重介绍能够执行大量自主工作的 AI 系统，而谷歌的 Gemini 因其缺乏成熟的智能体产品，已从主要推荐列表中移除。 这一转变反映了更广泛的行业趋势，即 AI 的价值正从简单的对话转向自主任务执行，这可能会显著提升各专业领域的生产力。对于用户和开发者而言，了解哪些平台在智能体能力上领先，对于选择能够自动化复杂、多步骤工作流程的工具至关重要。 该指南澄清了智能体模式令人困惑的命名规则：OpenAI 的“ChatGPT Work”和“Codex”，以及 Anthropic Claude 的“Cowork”和“Code”，这些模式在获得计算机访问权限后能提供更多功能。一个值得注意的技术细节是，将移动版 ChatGPT 切换到“Work”模式会解除其代码解释器的互联网访问限制，这一功能与桌面应用的区别并不直观。

rss · Simon Willison · 7月27日 21:55

**背景**: 智能体 AI 指的是能够在有限监督下完成特定目标、半自主或全自主运行以感知、推理和行动的人工智能系统。像 Claude 4 Opus 这样的模型代表了为智能体任务优化的高级迭代，具备长上下文窗口和自适应思维等特性。相比之下，传统的聊天模型主要为交互式对话设计，而像谷歌新推出的 Gemini Spark 这样的智能体系统，则旨在后台自主处理用户分配的任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained | MIT Sloan</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-8">Introducing Claude Opus 4.8 \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#LLM Guide`, `#AI Tools`, `#Productivity`

---