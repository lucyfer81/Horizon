---
layout: default
title: "Horizon Summary: 2026-09-01 (ZH)"
date: 2026-09-01
lang: zh
---

> 从 11 条内容中筛选出 5 条重要资讯。

---

1. [谷歌从 Chrome 网上应用店移除 Manifest V2 扩展程序，包括 uBlock Origin。](#item-1) ⭐️ 8.0/10
2. [DIY 项目利用 BirdNET-Go 将安防摄像头音频流改造成自动鸟类识别系统。](#item-2) ⭐️ 7.0/10
3. [个人经历引发担忧：军事基地超市冰柜可能遭黑客攻击](#item-3) ⭐️ 7.0/10
4. [文章认为 NAT 是导致互联网中心化的根本原因。](#item-4) ⭐️ 7.0/10
5. [Wrapture 发布：一个用于统一追踪和模拟的 Python 库。](#item-5) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [谷歌从 Chrome 网上应用店移除 Manifest V2 扩展程序，包括 uBlock Origin。](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

谷歌已从 Chrome 网上应用店中移除了所有 Manifest V2 扩展程序，包括广泛使用的广告拦截器 uBlock Origin。此举强制用户和开发者转向更新、限制更严格的 Manifest V3 标准。 此举对广告拦截生态系统和用户隐私产生了重大影响，因为 Manifest V3 限制了内容拦截扩展的功能。它巩固了谷歌对浏览器扩展领域的控制，可能影响数百万依赖强大广告拦截器来保障安全和获得更清洁网络体验的用户。 此次移除是分阶段弃用时间表的一部分；虽然用户目前可以重新启用被禁用的 MV2 扩展，但未来的阶段将永久阻止这一操作。值得注意的是，uBlock Origin 的开发者已声明该扩展在支持功能更强大的 MV2 标准的 Firefox 上运行效果最佳。

hackernews · twapi · 8月31日 21:10 · [社区讨论](https://news.ycombinator.com/item?id=49514878)

**背景**: 浏览器扩展需要一个 manifest.json 文件来定义其功能和权限。Manifest V2 于 2012 年推出，十多年来一直是标准，它允许像 uBlock Origin 这样的扩展使用强大的 \`webRequest\` API 进行动态内容过滤。谷歌推出的 Manifest V3 用一个限制性更强的 \`declarativeNetRequest\` API 取代了它，限制了扩展检查和修改网络流量的方式，而这对于高级广告拦截器至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/mv2-deprecation-timeline">Manifest V2 support timeline | Chrome for Developers</a></li>
<li><a href="https://dev.to/notearthian/whats-the-difference-between-manifest-v2-and-v3-in-browser-extensions-3b10">What&#x27;s the Difference Between Manifest V2 and V3 in browser extensions? - DEV Community</a></li>
<li><a href="https://factually.co/fact-checks/technology/manifest-v3-ad-blockers-ublock-origin-brave-firefox-2026-4d29ee">How Manifest V 3 Changed Ad Blockers: uBlock Origin, Br...</a></li>

</ul>
</details>

**社区讨论**: 社区表达了强烈的担忧和不满，认为此举是一个安全问题，也是企业控制权的过度扩张。许多评论者主张切换到 Firefox，理由是它持续支持 Manifest V2 并且与 uBlock Origin 兼容性更好。社区普遍存在一种对 Chrome 早期岁月的怀念情绪，以及抵制谷歌单方面控制网络标准的决心。

**标签**: `#browser-extensions`, `#ad-blocking`, `#chrome`, `#web-standards`, `#privacy`

---

<a id="item-2"></a>
## [DIY 项目利用 BirdNET-Go 将安防摄像头音频流改造成自动鸟类识别系统。](https://jasontucker.blog/how-i-turned-my-security-cameras-into-an-automatic-bird-identification-system-with-birdnet-go/) ⭐️ 7.0/10

一篇博客文章详细介绍了一种方法，通过使用自托管的 BirdNET-Go 软件进行实时本地 AI 推理，将标准安防摄像头的音频流转变为持续的鸟类监测系统。该项目利用了来自 Ubiquiti 的 Unifi 门铃等摄像头的现有 RTSP 流来“监听”并分类鸟鸣声。 这展示了一种富有创意、低成本的 AI 应用，让爱好者和普通家庭也能接触到先进的生物声学监测，将常见的物联网设备变成了科学工具。它突显了将消费级硬件重新用于环境感知和公民科学项目的日益增长的趋势。 BirdNET-Go 软件执行本地 AI 推理，专为 24/7 实时声景分析而设计。提到的一个关键技术挑战是，BirdNET 期望 48kHz 的音频样本，而某些摄像头的麦克风可能仅支持较低的采样率（例如 16kHz），这会影响识别准确性或需要像使用外置麦克风这样的变通方案。

hackernews · speckx · 8月31日 16:47 · [社区讨论](https://news.ycombinator.com/item?id=49511856)

**背景**: BirdNET 是由康奈尔大学开发的最先进的 AI 系统，它使用卷积神经网络从短音频片段中识别野生动物叫声。许多现代 IP 安防摄像头支持实时流协议（RTSP），这允许第三方软件访问其视频和音频流。BirdNET-Go 是这项技术的自托管、开源实现，支持持续、本地的分析，而无需将数据发送到云端。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/tphakala/birdnet-go">GitHub - tphakala/ birdnet - go : Self-hosted realtime soundscape...</a></li>
<li><a href="https://birdnet.cornell.edu/">BirdNET – AI-Powered Sound ID</a></li>
<li><a href="https://bou.org.uk/blog-granados-birdnet/">How to use BirdNET - British Ornithologists&#x27; Union</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示出浓厚的兴趣和实际的参与，用户们分享了他们使用不同摄像头品牌（Unifi, Aqara）的实现方案，并强调了音频采样率和风噪等技术难题。几位评论者扩展了这一概念，构建了带有电子墨水屏的便携式设备用于野外使用，并分享了他们自己的设置指南和可 3D 打印外壳的链接。

**标签**: `#DIY`, `#Machine Learning`, `#IoT`, `#BirdNET`, `#Home Automation`

---

<a id="item-3"></a>
## [个人经历引发担忧：军事基地超市冰柜可能遭黑客攻击](https://signalandsilence.substack.com/p/i-think-someone-hacked-the-commissary) ⭐️ 7.0/10

一篇在网上发布的个人经历指出，美国一家军事基地超市的工业冰柜可能遭到入侵，导致了大范围的故障。这一事件引发了对工业控制系统安全和供应链漏洞的详细讨论。 这一事件凸显了关键基础设施（即使在军事环境中）也容易遭受针对运营技术的网络攻击。对此类系统的成功攻击可能破坏重要的供应链，影响当地经济，并构成重大的安全风险。 作者承认，故障也可能源于配置错误或维护问题，而不一定是蓄意攻击。社区专家指出，像关岛或夏威夷这样的海外孤立地点，由于其更大的物流影响，可能成为此类攻击的更高价值目标。

hackernews · jcurbo · 8月31日 11:45 · [社区讨论](https://news.ycombinator.com/item?id=49508506)

**背景**: 工业控制系统（ICS），包括 SCADA 和 DCS，用于监控和控制电网、水处理厂等关键基础设施中的工业过程。可编程逻辑控制器（PLC）是 ICS 中的常见组件，常因软件过时、默认安全性弱（如 admin/admin 凭证）以及缺乏加密而受到批评，使其容易受到网络攻击。供应链攻击通过入侵受信任的供应商或软件更新来渗透安全环境，从而针对这些系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tripwire.com/solutions/industrial-control-systems">ICS Security | Industrial Cybersecurity Control Systems</a></li>
<li><a href="https://plcprogramming.io/blog/plc-security-best-practices-complete-guide">PLC Security Best Practices Guide</a></li>
<li><a href="https://panorays.com/blog/cyber-security-supply-chain-attacks/">Cyber Security Supply Chain Attacks: Navigating the 2026 Threat Landscape</a></li>

</ul>
</details>

**社区讨论**: 社区观点不一，一些专家认为配置错误的可能性大于黑客攻击，而另一些人则根据对不安全 PLC 的第一手经验认为这种情况是 plausible 的。评论提供了关于供应链漏洞的历史背景，并分享了工业控制系统中常见的不良安全实践案例，例如承包商不启用 TLS 和使用默认密码。

**标签**: `#Cybersecurity`, `#Industrial Control Systems`, `#Critical Infrastructure`, `#Supply Chain`, `#PLC Security`

---

<a id="item-4"></a>
## [文章认为 NAT 是导致互联网中心化的根本原因。](https://dreamstation.systems/personal/ntppost.html) ⭐️ 7.0/10

一篇文章提出，网络地址转换（NAT）是导致互联网中心化的一个根本原因，它削弱了用户轻松托管服务器的能力，并使客户端-服务器模型成为常态。这一批评引发了讨论，包括 Linux NAT 系统的实现者 Rusty Russell 的评论，他承认了该系统在移除公共端点方面的作用。 这一观点挑战了常被视为理所当然的核心网络技术，将一项技术设计决策与深远的社会结果（如云平台的主导地位和对等网络、用户托管服务的衰落）联系起来。它重新构建了关于互联网架构的辩论，突显了在安全性、地址节约与原始的端到端开放原则之间的权衡。 文章特别批评了 NAT 的设计，该设计优先考虑在单个 IP 上复用出站连接，这本质上会阻止未经请求的入站流量，使得 NAT 后的服务器在没有显式端口转发的情况下无法被访问。讨论中的一个关键反对观点是，运营商级 NAT（CGNAT）被认为比标准 NAT 更具限制性，并且端口转发的不良用户体验（UX），而非 NAT 本身，才是主要障碍。

hackernews · robinpie · 8月31日 02:23 · [社区讨论](https://news.ycombinator.com/item?id=49504905)

**背景**: 网络地址转换（NAT）是一种技术，允许多个私有网络上的设备共享一个公共 IP 地址来访问互联网，主要是为了节约有限的 IPv4 地址池。最初的互联网架构建立在“端到端原则”之上，该原则设想智能和控制（如托管服务器）位于网络的端点（用户设备），而不是在中间。这促进了一种更加去中心化的对等网络模型，与现在占主导地位的客户端-服务器模型形成对比，在后一种模型中，用户（客户端）主要从中心化提供商（服务器）消费服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/computer-networks/network-address-translation-nat/">Network Address Translation ( NAT ) - GeeksforGeeks</a></li>
<li><a href="https://devopedia.org/end-to-end-principle">End - to - End Principle</a></li>
<li><a href="https://en.wikipedia.org/wiki/Peer-to-peer">Peer - to - peer - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了关于 NAT 影响的不同观点。Linux NAT 的实现者 Rusty Russell 对其设计消除了公共端点表示遗憾。其他人，如 elric，则认为称 NAT 为“原罪”是夸大其词，区分了常规 NAT 与限制性更强的运营商级 NAT（CGNAT），并将问题归咎于端口转发的不良用户体验。一种观点认为，NAT 为易受攻击的设备提供了一个关键（尽管不完美）的安全层，突显了在可访问性和保护之间的复杂权衡。

**标签**: `#networking`, `#internet-history`, `#decentralization`, `#nat`, `#architecture`

---

<a id="item-5"></a>
## [Wrapture 发布：一个用于统一追踪和模拟的 Python 库。](https://simonwillison.net/2026/Aug/31/introducing-wrapture/) ⭐️ 7.0/10

Graham Dumpleton 发布了 Wrapture，这是一个新的 Python 库，它扩展了其 \`wrapt\` 库中的猴子补丁概念，使得能够对函数和方法进行同时、非侵入式的追踪和模拟。这个项目仅诞生数周，包含对 OpenTelemetry 的支持以及一个基于配置的机制，用于为现有项目添加追踪功能。 这很重要，因为它解决了 Python 开发中的一个长期挑战：在不修改源代码的情况下观察和测试代码，特别是第三方或遗留代码。通过将追踪（用于可观测性）和模拟（用于测试）统一起来，Wrapture 为从事调试、性能监控和创建健壮测试套件的开发者提供了一个强大的工具。 Wrapture 提供了 Python 标准库 \`unittest.mock\` 的替代方案，并且可以通过 TOML 文件进行配置，将追踪附加到特定目标。值得注意的是，整个项目，包括其代码和文档，都是在 Graham Dumpleton 的精心指导和工程规划下由 AI 助手编写的，这使其有别于控制较少的“氛围编码”方法。

rss · Simon Willison · 8月31日 23:59

**背景**: 猴子补丁是 Python 中的一种技术，允许开发者在运行时修改或扩展函数、方法或类的行为，而无需更改原始源代码。Graham Dumpleton 的 \`wrapt\` 库是执行可靠猴子补丁的知名工具。另一方面，\`unittest.mock\` 是一个标准库模块，用于用模拟对象替换被测系统的部分组件，而 OpenTelemetry 是一个供应商中立的框架，用于收集追踪和指标等遥测数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wrapt.readthedocs.io/en/develop/monkey.html">Monkey Patching — wrapt 2.4.0 documentation</a></li>
<li><a href="https://github.com/GrahamDumpleton/wrapt">GitHub - GrahamDumpleton/wrapt: A Python module for decorators ...</a></li>
<li><a href="https://realpython.com/python-mock-library/">Understanding the Python Mock Object Library – Real Python</a></li>

</ul>
</details>

**标签**: `#python`, `#testing`, `#observability`, `#libraries`

---