---
layout: default
title: "Horizon Summary: 2026-08-31 (ZH)"
date: 2026-08-31
lang: zh
---

> 从 9 条内容中筛选出 4 条重要资讯。

---

1. [QubesOS 关键漏洞 QSB-118 允许从 Dom0 执行任意代码](#item-1) ⭐️ 8.0/10
2. [欧盟委员会在 ProtectEU 战略中重提加密后门要求](#item-2) ⭐️ 8.0/10
3. [Omarchy Linux 存在严重漏洞，允许任意用户进程提权至 root](#item-3) ⭐️ 8.0/10
4. [Simon Willison 澄清 ChatGPT Work 的双重性质，区分其云端与本地桌面版本。](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [QubesOS 关键漏洞 QSB-118 允许从 Dom0 执行任意代码](https://www.qubes-os.org/news/2026/08/29/qsb-118/) ⭐️ 8.0/10

2026 年 8 月 29 日，QubesOS 披露了一个关键漏洞（QSB-118），该漏洞可通过复制到虚拟机的错误报告后门实现任意代码执行。该缺陷具体存在于从特权域 Dom0 执行 \`qvm-copy-to-vm\` 命令时。 此事至关重要，因为 QubesOS 是一个著名的以安全为中心的操作系统，其核心安全模型依赖于 Dom0 的隔离性和高完整性。一个允许从 Dom0 执行任意代码的漏洞会破坏整个系统的安全基础，可能影响所有依赖 QubesOS 进行高安全性计算用户。 该漏洞仅在使用了 Dom0 版本的 \`qvm-copy-to-vm\` 命令时才会被触发；虚拟机版本不受影响，因为其错误报告函数未使用存在漏洞的 \`system\(\)\` 调用。该漏洞利用涉及一个容易被忽视的攻击媒介——错误报告后门。

hackernews · vntok · 8月30日 08:51 · [社区讨论](https://news.ycombinator.com/item?id=49496918)

**背景**: QubesOS 是一个面向安全的操作系统，它利用虚拟化技术将应用程序和数据隔离到称为 &\#x27;qubes&\#x27; 的独立虚拟机中。Dom0（域 0）是初始的、具有特权的管理域，它控制窗口管理器并可以启动/停止其他虚拟机，但其设计初衷是保持最小的网络连接以减少攻击面。\`qvm-copy-to-vm\` 命令用于在 qubes 之间复制文件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qubes_OS">Qubes OS - Wikipedia</a></li>
<li><a href="https://www.qubes-os.org/news/2026/08/29/qsb-118/">QSB - 118 : Dom0 arbitrary code execution in... | Qubes OS</a></li>
<li><a href="https://news.ycombinator.com/item?id=49496918">Arbitrary code execution in QubesOS via copy - to - VM error reporting ...</a></li>

</ul>
</details>

**社区讨论**: 社区情绪强调了在一个以安全为中心的系统中发现此漏洞的严重性，用户指出 QubesOS 本身攻击面很小，使得这一发现更值得注意。评论澄清了漏洞利用范围仅限于该命令的 Dom0 版本，并讨论了更广泛的影响，包括引用历史上的安全批评以及对项目领导层变更的观察。

**标签**: `#security`, `#vulnerability`, `#qubesos`, `#system-security`, `#exploit`

---

<a id="item-2"></a>
## [欧盟委员会在 ProtectEU 战略中重提加密后门要求](https://reclaimthenet.org/eu-protecteu-strategy-encryption-backdoor-law-enforcement) ⭐️ 8.0/10

欧盟委员会在其于 2025 年 4 月提出的新 ProtectEU 内部安全战略中，正重新推动强制设置加密后门，以便执法部门能够访问加密数据。该举措旨在为当局打击安全威胁建立一个更强大的法律框架。 这项政策提案对全球数字安全和隐私具有重大影响，因为强制设置后门可能造成系统性漏洞，被犯罪分子和敌对行为者利用。它重新点燃了关于如何在执法需求与安全通信和数据保护这一基本权利之间取得平衡的长期辩论。 强制设置后门的具体法律文本尚未公开，一些社区成员质疑新闻稿中提到的“为执法部门提供更有效的工具”是否明确指代后门。从历史上看，类似的提案一直遭到安全专家的强烈反对，他们认为任何后门都会削弱所有人的加密安全性。

hackernews · nickslaughter02 · 8月30日 15:12 · [社区讨论](https://news.ycombinator.com/item?id=49499394)

**背景**: 加密是对数据进行编码的过程，以确保只有授权方可以读取。加密后门是一种通常隐蔽的方法，允许政府等实体在未经用户授权的情况下绕过加密。ProtectEU 战略是欧盟委员会的内部安全计划，旨在帮助成员国防范恐怖主义、有组织犯罪和混合威胁。围绕加密数据“合法访问”的争论已持续多年，一方是执法部门的调查需求，另一方是在加密系统中故意制造弱点所带来的安全和隐私风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://home-affairs.ec.europa.eu/news/commission-presents-protecteu-internal-security-strategy-2025-04-01_en">Commission presents ProtectEU Internal Security Strategy - Migration and Home Affairs</a></li>
<li><a href="https://www.securityweek.com/encryption-backdoors-the-security-practitioners-view/">Encryption Backdoors: The Security Practitioners&#x27; View</a></li>
<li><a href="https://www.congress.gov/crs-product/IF11769">Law Enforcement and Technology: The “Lawful Access” Debate | Congress.gov | Library of Congress</a></li>

</ul>
</details>

**社区讨论**: 社区讨论对该提案持压倒性的批评态度，主要关注技术风险、政治越权和历史背景。关键观点包括：批评欧盟委员会的立法权力动态；警告后门会破坏安全性，尤其是在人工智能时代；以及担忧此类工具可能被未来的威权政府滥用。还有一条评论质疑战略文本与明确要求后门之间的直接联系。

**标签**: `#encryption`, `#privacy`, `#policy`, `#security`, `#eu`

---

<a id="item-3"></a>
## [Omarchy Linux 存在严重漏洞，允许任意用户进程提权至 root](https://0xcc.io/posts/omarchy-root-creds/) ⭐️ 8.0/10

在基于 Arch Linux 的 Omarchy 发行版中发现了一个严重的本地权限提升漏洞，该漏洞允许任意用户进程获得 root 级别的系统访问权限。该漏洞及其概念验证已被公开披露，揭示了该发行版设计中存在的严重安全缺陷。 该漏洞代表了一种根本性的安全失效，因为它完全绕过了标准的 Linux 权限隔离机制，使得运行受影响 Omarchy 版本的系统极易被攻陷。这凸显了使用重度定制化或&\#x27;氛围编码&\#x27;发行版的风险，这类发行版可能将美观和便利置于稳健的安全实践之上。 据报道，该漏洞利用方法简单，无需复杂的漏洞链，这表明了系统安全模型存在根本性缺陷。在此事件之前，Omarchy 近期还出现过另一个安全问题，即 USB 描述符被不当传递给 shell，这表明其存在一系列安全疏忽。

hackernews · trap0xcc · 8月30日 15:59 · [社区讨论](https://news.ycombinator.com/item?id=49499854)

**背景**: Omarchy 是由 37signals 创建的一个基于 Arch Linux 的、固执己见的发行版，旨在通过最少的设置提供一个美观、完整的桌面工作站体验。本地权限提升漏洞允许初始权限有限的用户（如标准用户账户）获得更高的权限，例如 root 访问权限，这是在类 Unix 系统上的最高控制级别。此类漏洞尤其危险，因为它能使攻击者完全控制系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cyberpanel.net/blog/omarchy-linux-guide">Omarchy Linux : What Is It and Is It Worth Trying? 5 Min Read</a></li>
<li><a href="https://github.com/basecamp/omarchy">GitHub - basecamp/ omarchy : Beautiful, Modern &amp; Opinionated Linux</a></li>
<li><a href="https://attack.mitre.org/techniques/T1068/">Exploitation for Privilege Escalation , Technique... | MITRE ATT&amp;CK</a></li>

</ul>
</details>

**社区讨论**: 社区舆论对 Omarchy 这类&\#x27;氛围编码&\#x27;发行版持批评态度，鉴于此次及先前的漏洞，警告用户因其固有的安全风险而应避免使用。一些评论者认为，更广泛的 Linux 桌面生态系统缺乏强大的沙箱机制，使得权限提升成为一个超越 Omarchy 本身的普遍性问题。另一些人则告诫不要盲目跟风使用被过度炒作的发行版，并建议转而使用官方的 Arch Linux 安装工具。

**标签**: `#linux-security`, `#privilege-escalation`, `#vulnerability`, `#operating-systems`, `#system-administration`

---

<a id="item-4"></a>
## [Simon Willison 澄清 ChatGPT Work 的双重性质，区分其云端与本地桌面版本。](https://simonwillison.net/2026/Aug/30/understanding-chatgpt-work/) ⭐️ 7.0/10

Simon Willison 分析了新推出的 ChatGPT Work 产品，澄清它实际上是两个不同的产品：一个是通过网页和移动应用访问的云端版本，另一个是基于更名后的 Codex 应用的本地桌面版本。他详细说明，目前仅对付费订阅者开放的云端版本引入了新功能，如模型选择、具有互联网访问权限的代码执行环境以及持久化的共享文件系统。 这一澄清非常重要，因为 ChatGPT Work 的双重产品性质在发布时令人困惑，理解其区别对于用户选择适合自己需求的工具至关重要。云端版本的高级功能标志着 AI 向一个持久化、多工具工作环境迈出了重要一步，可能会重塑知识工作者将 AI 集成到复杂的、基于文件的任务和工作流中的方式。 云端版本提供在 GPT-5.6 变体（Sol、Luna、Terra）之间的模型选择，并具有不同的推理级别，还包含一个无头 Chrome 浏览器以及发布“ChatGPT Sites”的能力。一个关键限制是，目前两个版本都仅限于每月 20 美元的 ChatGPT Plus 计划或更高级别的订阅者，免费用户和每月 8 美元的 Go 用户无法使用。

rss · Simon Willison · 8月30日 23:59

**背景**: ChatGPT 是 OpenAI 的旗舰对话式 AI 助手。Codex 是 OpenAI 的桌面应用程序，最初定位为 AI 编码助手，后来演变成一个更广泛的“智能体指挥中心”，能够在用户计算机上执行任务。“ChatGPT Work”的发布代表了这些概念的融合，既提供了一个强大的云端工作空间，也提供了本地桌面集成，这导致了用户对其范围和能力的最初困惑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/codex/">Codex in ChatGPT | AI Coding Agents for Software... | OpenAI</a></li>
<li><a href="https://windowsforum.com/threads/codex-becomes-openais-desktop-work-os-chatgpt-and-agents-converge-in-2026.434874/">Codex Becomes OpenAI ’s Desktop “Work OS”... | Windows Forum</a></li>
<li><a href="https://www.bigprompthub.com/chatgpt-work-local-folder-guide/">ChatGPT Work Local Folder Guide: Desktop vs Cloud Files - Big Prompt Hub</a></li>

</ul>
</details>

**标签**: `#AI`, `#ChatGPT`, `#OpenAI`, `#Product Analysis`

---