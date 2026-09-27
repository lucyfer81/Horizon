---
layout: default
title: "Horizon Summary: 2026-09-27 (ZH)"
date: 2026-09-27
lang: zh
---

> 从 5 条内容中筛选出 3 条重要资讯。

---

1. [Reladraw：一种融合可编程性与手动布局控制的图表语言](#item-1) ⭐️ 7.0/10
2. [Haskell 社区讨论在 LLM 主导的时代如何保持编程的乐趣。](#item-2) ⭐️ 7.0/10
3. [Conversations 应用退出 Google Play 后转为免费，开发者控诉平台支持不力](#item-3) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Reladraw：一种融合可编程性与手动布局控制的图表语言](https://github.com/reladraw/reladraw) ⭐️ 7.0/10

Reladraw 是一种新的开源图表语言和工具，它允许用户以编程方式定义图表，同时保留对元素布局的手动控制权。该项目包含一个网页游乐场、一个 npm 包，以及一个可供 Claude 等 AI 智能体安装的技能。 该工具填补了全自动布局工具（如 Mermaid）与手动绘图软件之间的重要空白，提供了一种混合方法，既便于程序化生成，又能满足人类设计师的表达需求。其同时为人类和 AI 智能体设计的特点，使其在 AI 辅助开发和文档工作流中具有特殊的相关性。 该语言的语法允许指定相对位置（例如“left of”、“right of”）来指导布局，而无需绝对坐标。早期用户反馈指出存在一些缺陷，例如渲染器并不总是能正确解释边的方向注释来创建曲线箭头。

hackernews · jpwalsh234 · 9月26日 17:10 · [社区讨论](https://news.ycombinator.com/item?id=49858513)

**背景**: Mermaid 和 Graphviz 等工具是流行的文本转图表解决方案，它们自动计算布局，但用户对最终视觉排列的控制通常有限，这可能导致复杂图表的效果不佳。相反，像 Draw.io 这样的手动工具提供了完全的控制，但非常耗时，且不易于自动化或与 AI 智能体集成——AI 智能体可以使用预定义的“技能”来执行特定任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mermaid_%28software%29">Mermaid (software) - Wikipedia</a></li>
<li><a href="https://graphviz.org/doc/info/attrs.html">Attributes - Graphviz</a></li>
<li><a href="https://claude-plugins.dev/skills">Discover Agent Skills</a></li>

</ul>
</details>

**社区讨论**: 社区反应非常积极，强调 Reladraw 在自动化和控制之间找到了“最佳平衡点”，特别是在 AI 辅助开发中，图表有助于对齐思维模型。建议包括将其用作 C4 模型的布局层，以及将拓扑定义与布局关注点解耦。一位用户指出了一个关于边渲染的小缺陷。

**标签**: `#diagramming`, `#developer-tools`, `#ai-agents`, `#visualization`, `#open-source`

---

<a id="item-2"></a>
## [Haskell 社区讨论在 LLM 主导的时代如何保持编程的乐趣。](https://discourse.haskell.org/t/how-to-keep-enjoying-programming-in-a-world-of-llms/14705) ⭐️ 7.0/10

Haskell Discourse 论坛上发起了一场题为“在 LLM 的世界里如何继续享受编程”的讨论，已收到超过 200 条评论，探讨了 AI 编程助手对个人和职业的影响。对话呈现了从技能退化、工作满意度下降到利用 AI 提高繁琐任务效率等多种不同的体验。 这场讨论意义重大，因为它触及了在一个快速采用 AI 工具的行业中，开发者长期职业满意度和技能相关性的核心关切。这种自我反思的结果可能会影响个人和团队如何构建工作流程，以在生产力与个人成长、工作乐趣之间取得平衡。 社区成员分享了具体策略，例如使用更快、自主性较低的 LLM 以保持动手控制权，并用汽车修理工从手工工具转向软件调校来类比这一转变。讨论是细致入微的，承认对于一些开发者来说，对编程的不满在 LLM 出现之前就已存在。

hackernews · signa11 · 9月26日 09:41 · [社区讨论](https://news.ycombinator.com/item?id=49854875)

**背景**: 像 GPT-4 和 Claude Code 这样的大型语言模型（LLM）是在海量文本和代码上训练的 AI 系统，能够根据自然语言提示生成、解释和调试代码。集成这些模型的 AI 编程助手已成为开发者工作流程中的变革者，为许多人显著提高了生产力，但也引发了关于过度依赖的担忧。“技能退化”指的是由于过度依赖 AI 工具而导致的基本开发者技能（如阅读文档、架构规划和调试）的下降。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://addyosmani.com/blog/ai-coding-workflow/">My LLM coding workflow going into 2026 | AddyOsmani.com</a></li>
<li><a href="https://addyo.substack.com/p/avoiding-skill-atrophy-in-the-age">Avoiding Skill Atrophy in the Age of AI - Elevate | Addy Osmani</a></li>
<li><a href="https://medium.com/@iamalvisng/the-skills-youre-losing-while-ai-handles-the-boring-parts-380266adcf0c">The Skills You&#x27;re Losing While AI Handles the Boring Parts | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，反映了个人层面的焦虑与适应。一些人表达了对技能退化和动手技艺丧失的担忧，将其比作现在使用微波炉的厨师。另一些人则认为 LLM 是一种解放，让他们能够卸下繁琐的“垃圾”工作，专注于更有趣的问题。几位评论者分享了减轻负面影响的个人策略，例如选择更快的模型以保持交互式的工作流程。

**标签**: `#programming`, `#llms`, `#career`, `#productivity`, `#ethics`

---

<a id="item-3"></a>
## [Conversations 应用退出 Google Play 后转为免费，开发者控诉平台支持不力](https://gultsch.de/posts/breaking-up-with-google-play/) ⭐️ 7.0/10

XMPP 客户端 Conversations 的开发者 Daniel Gultsch 已将应用从 Google Play 商店下架，并使其转为免费下载。这一决定源于他对 Google Play 糟糕的开发者支持、不透明的政策执行以及对 Android 应用生态垄断控制的不满。 此举凸显了独立开发者与主导性应用商店平台之间日益紧张的关系，挑战了标准的收入模式，并对公平支持和透明政策提出了质疑。它揭示了平台垄断如何对开发者体验和用户的应用可用性产生负面影响。 开发者指出了具体问题，例如版本审核缓慢以及 Google Play 支持缺乏有意义的反馈。该应用在 F-Droid 等替代平台上仍可免费获取，这与其开源性质和对 XMPP 协议的依赖相符。

hackernews · ezst · 9月26日 10:55 · [社区讨论](https://news.ycombinator.com/item?id=49855315)

**背景**: Conversations 是一款流行的 Android 开源即时通讯客户端，使用 XMPP（可扩展消息与存在协议）标准，是 WhatsApp 等中心化服务的替代品。Google Play 是 Android 主要的官方应用分发平台，开发者通常需要支付费用并分享收入，但必须遵守 Google 的政策和审核流程。此处的“垄断”指的是 Google Play 在 Android 设备上占据的主导市场地位，这限制了开发者的分发渠道选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://conversations.im/">Conversations : the very last word in instant messaging</a></li>
<li><a href="https://play.google/developer-content-policy/">Developer Policy Center - Google Play</a></li>

</ul>
</details>

**社区讨论**: 社区讨论强烈支持开发者的不满，许多评论者同意 Google 糟糕的支持是核心问题，而不仅仅是收入分成。几位开发者分享了他们在不透明的政策和验证流程方面的挫败经历，突显了系统性问题。大家普遍担心 Google 正让业余爱好者和小型项目在 Play 商店中越来越难以生存，同时也在加强对侧载安装的控制。

**标签**: `#app-stores`, `#android`, `#developer-experience`, `#google-play`, `#monopoly`

---