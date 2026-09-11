---
layout: default
title: "Horizon Summary: 2026-09-11 (ZH)"
date: 2026-09-11
lang: zh
---

> 从 13 条内容中筛选出 9 条重要资讯。

---

1. [Calif Research 展示 WeWorm：利用 AI 辅助开发的、通过微信通话传播的零点击蠕虫](#item-1) ⭐️ 9.0/10
2. [Shopify 将其移动应用从 React Native 迁移回原生 Swift 和 Kotlin。](#item-2) ⭐️ 8.0/10
3. [研究人员质疑 OpenAI 的伦理问题，担忧其可能使用合作聊天中的未发表数学成果。](#item-3) ⭐️ 8.0/10
4. [Cognition 发布 SWE-2，这是一款性能匹敌顶尖模型且成本更低的 AI 编码模型。](#item-4) ⭐️ 8.0/10
5. [微软正式将 Rust 指定为其内部开发的一级编程语言。](#item-5) ⭐️ 8.0/10
6. [索尼在诉讼中被指使用&\#x27;拥有&\#x27;字眼，挑战数字游戏许可条款](#item-6) ⭐️ 8.0/10
7. [TryNix.dev 可在浏览器虚拟机中运行过去 13 年的任何 Nix 包](#item-7) ⭐️ 8.0/10
8. [NASA 卫星图像处理技术现用于揭示褪色的古代岩画](#item-8) ⭐️ 7.0/10
9. [PlanetScale 发布 Neki，一款用于水平扩展的分片 PostgreSQL 解决方案。](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Calif Research 展示 WeWorm：利用 AI 辅助开发的、通过微信通话传播的零点击蠕虫](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 9.0/10

Calif Research 发布了一个名为 WeWorm 的概念验证演示，这是一种零点击蠕虫，可以通过微信语音通话在 iOS 和 Android 设备间传播，无需任何用户交互。该团队在 AI 的显著辅助下，在大约两天内发现了底层的内存损坏漏洞并编写了初始的远程代码执行（RCE）漏洞利用程序，完整的蠕虫构建又花了一周时间。 这次演示代表了攻击性安全领域的范式转变，表明 AI 能够极大地加速关键漏洞的发现和武器化，将过去需要大型团队数月的工作缩短至数天。它突显了威胁潜力的重大升级，因为零点击蠕虫可以大规模地静默入侵设备，对数十亿微信用户构成严重风险，并标志着 AI 驱动的网络威胁新时代的到来。 该漏洞利用针对的是微信语音通话（VoIP）堆栈中的内存损坏漏洞，受害者无需接听电话或与手机进行任何交互即可被入侵。据报道，微信的母公司腾讯已封锁了该漏洞，缓解了这一特定概念验证带来的直接风险。

rss · Simon Willison · 9月10日 00:56

**背景**: 零点击漏洞利用不需要受害者进行任何交互，例如点击链接或打开文件，因此极其隐蔽和危险。远程代码执行（RCE）是一种严重的攻击，攻击者可以通过利用软件漏洞或不安全配置，从远程位置在目标系统上运行任意代码。AI 辅助的漏洞研究涉及使用大语言模型（LLM）来自动化安全研究工作流程的某些部分，例如漏洞发现、漏洞利用程序开发和代码分析，这可能会彻底改变攻击性和防御性安全操作的速度和规模。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cyberinsider.com/zero-click-worm-spreads-on-iphones-and-android-via-wechat-calls/">Zero-click worm spreads on iPhones and Android via WeChat ...</a></li>
<li><a href="https://www.invicti.com/learn/remote-code-execution-rce">Remote Code Execution (RCE)</a></li>
<li><a href="https://cribl.io/blog/ai-assisted-vulnerability-research-at-cribl/">AI-assisted vulnerability research at Cribl</a></li>

</ul>
</details>

**标签**: `#ai-security`, `#zero-click-exploit`, `#vulnerability-research`, `#offensive-security`, `#ai-assisted-development`

---

<a id="item-2"></a>
## [Shopify 将其移动应用从 React Native 迁移回原生 Swift 和 Kotlin。](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify 宣布正在将其移动应用从跨平台的 React Native 框架迁移回使用 Swift（iOS）和 Kotlin（Android）的完全原生开发。该公司将开发者体验和性能列为主要原因，并讨论了大型语言模型（LLM）如何协助此类迁移。 这家大型科技公司的决定，验证了移动开发领域关于跨平台效率与原生性能/开发者体验之间权衡的长期争论。它预示着一个潜在的行业转变：对于复杂、高性能的应用，成本效益分析可能越来越倾向于原生技术栈，尤其是在 LLM 降低了迁移门槛的情况下。 Shopify 的评论强调，LLM 辅助工具可以显著加速迁移过程，不过一些社区成员认为，即使在高级 LLM 出现之前，大规模迁移也是可行的。此举强调，对于大规模、性能关键型应用，跨 JavaScript、C++ 和原生线程进行调试的开销，可能会超过共享代码库带来的好处。

hackernews · fnthawar2 · 9月10日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49643982)

**背景**: React Native 是 Meta 推出的一个流行的跨平台框架，允许开发者使用 JavaScript 和 React 为 iOS 和 Android 构建移动应用。其主要吸引力在于代码复用以及利用 Web 开发人员的技能进行移动开发。使用 Swift（iOS）和 Kotlin（Android）的原生开发可以直接访问平台特定的 API 和硬件，通常能带来更好的性能和更精致的用户体验，但需要维护独立的代码库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://appinventiv.com/blog/react-native-vs-native-apps/">React Native vs Native: Which is Better for App Development?</a></li>
<li><a href="https://kotlinlang.org/docs/multiplatform/kotlin-multiplatform-react-native.html">Kotlin Multiplatform vs. React Native: A cross-platform comparison | Kotlin Multiplatform Documentation</a></li>
<li><a href="https://blog.bestai.com/rewriting-the-future-how-llm-agents-are-transforming-code-migration/">Rewriting the Future: How LLM Agents Are Transforming Code ...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示，原生移动工程师对此表示强烈认同，他们长期以来一直反对为复杂应用采用跨平台的折中方案。几位评论者分享了他们自己的迁移经验，指出 LLM 可以自动化许多繁重的工作。一个关键的反驳观点是，虽然 LLM 有帮助，但大规模迁移在技术上早已可行，根本性的决策取决于长期的性能和可维护性需求，而不仅仅是迁移成本。

**标签**: `#mobile-development`, `#react-native`, `#software-architecture`, `#llm`, `#developer-tools`

---

<a id="item-3"></a>
## [研究人员质疑 OpenAI 的伦理问题，担忧其可能使用合作聊天中的未发表数学成果。](https://mathstodon.xyz/@andreasthom/117240535270608201) ⭐️ 8.0/10

由研究员 Andreas Thom 在 Mathstodon 平台上发起的一场讨论，对 OpenAI 能否妥善处理研究人员与其模型合作聊天中分享的未发表数学成果提出了严重质疑。核心指控是，OpenAI 可能利用这些新颖想法来训练其模型或发表成果，却未对贡献者进行恰当署名。 这一问题触及了研究诚信和对 AI 公司信任的核心，因为它可能导致学者因担心成果被抢先发表或原创思想得不到认可而不敢使用 AI 工具。这凸显了 AI 研究生态中一个关键且未解决的矛盾：既需要与模型进行开放式的协作探索，又需要保护知识产权和学术署名权。 讨论提及了具体事件，包括据报道 OpenAI 在得知一个重大数学证明可能在其训练数据中后，从一个仍在训练的模型中生成了 3000 亿个输出令牌，这让一些人感到可疑。此外，OpenAI 的使用政策保留了为保护其服务而使用数据的广泛权利，但这些政策如何适用于新颖、未发表的研究输入，目前仍不明确。

hackernews · pred\_ · 9月10日 06:49 · [社区讨论](https://news.ycombinator.com/item?id=49639408)

**背景**: Mathstodon 是去中心化社交媒体平台 Mastodon 上的一个服务器，深受数学家欢迎，用于专业讨论。研究人员经常使用像 OpenAI 的 ChatGPT 或 Codex 这样的 AI 模型作为协作工具，就未解决的数学问题进行头脑风暴和完善想法。大型语言模型的训练数据通常包含来自互联网的大量公开文本，但用于研究的私人合作聊天记录的状态则是一个具有重大伦理影响的灰色地带。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://terrytao.wordpress.com/2022/11/20/trying-out-mathstodon/">Trying out Mathstodon | What&#x27;s new - Terence Tao</a></li>
<li><a href="https://openai.com/policies/usage-policies/">Usage policies | OpenAI</a></li>

</ul>
</details>

**社区讨论**: 社区情绪持怀疑和担忧态度，用户将未经署名使用想法的行为类比为不道德的人类合作。关键观点包括：争论模型改进是源于记忆聊天细节还是更广泛的强化学习；怀疑 OpenAI 在开放问题上的快速进展可能得益于研究人员的输入；以及对信任公司处理敏感数据的普遍不安。

**标签**: `#AI Ethics`, `#OpenAI`, `#Research Integrity`, `#Academic Collaboration`

---

<a id="item-4"></a>
## [Cognition 发布 SWE-2，这是一款性能匹敌顶尖模型且成本更低的 AI 编码模型。](https://cognition.com/blog/swe-2) ⭐️ 8.0/10

Cognition 发布了其最新的软件工程 AI 模型 SWE-2，据报道，该模型在 FrontierCode 1.1 Main 基准测试中获得了 50.0% 的分数，与 Fable 5.1 的性能仅差一分。该公司声称，该模型在实现接近前沿性能的同时，运行成本降低了多达 70%。 这一消息之所以重要，是因为它引入了一个比当前领先的 AI 编码模型更具成本效益的潜在替代品，这可能降低高级 AI 辅助开发的门槛。如果其宣称的性能属实，将加剧编码助手市场的竞争，迫使现有参与者提升性能或降低成本。 一个关键的技术细节是，SWE-2 是基于 Kimi K3 模型进行后训练得到的，而非一个全新的架构。值得注意的是，其在较旧的 Terminal Bench 2.1（92.8%）和较新的 Terminal Bench 4（27.3%）基准测试中的得分存在巨大差距，这引发了对其处理新问题泛化能力的质疑。

hackernews · seelos · 9月10日 15:29 · [社区讨论](https://news.ycombinator.com/item?id=49645443)

**背景**: Cognition 是自主 AI 编码代理 Devin 背后的初创公司。像 Fable 5.1（来自 Anthropic）和 GPT-Astra（来自 OpenAI）这样的模型被认为是前沿模型，代表了当前 AI 在编码和推理等复杂任务上的最高水平。像 FrontierCode 这样的基准测试分数，通常用于比较这些大型语言模型（LLM）在特定任务上的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cognition.com/blog/swe-2">Introducing SWE-2: Pushing the Pareto Frontier | Cognition</a></li>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-1">Introducing Claude Fable 5 . 1 and Claude Mythos 5 . 1 \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT -6 Astra - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区情绪持怀疑和批判态度。主要观点包括：由于在新基准测试上性能大幅下降，对其模型泛化能力表示怀疑；对 Cognition 过去关于其 Devin 代理的宣称表示质疑；并批评 SWE-2 是另一个闭源模型，而市场用户正越来越倾向于像 DeepSeek 这样的开源替代品。

**标签**: `#artificial-intelligence`, `#software-engineering`, `#llm`, `#coding-assistant`, `#benchmarks`

---

<a id="item-5"></a>
## [微软正式将 Rust 指定为其内部开发的一级编程语言。](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

微软已正式授予 Rust “一级语言”地位，这意味着它现在将获得包括安全工具链构建、深度平台集成以及符合微软安全开发生命周期（SDL）要求在内的全面工程支持。这一指定为内部团队提供了从本地开发到生产环境使用 Rust 的、得到全面支持的成熟路径。 这是来自全球最大软件公司之一的重要战略背书，标志着 Rust 的成熟度及其为大规模、关键任务系统开发做好了准备。这将加速 Rust 在微软庞大产品组合中的应用，并可能通过利用 Rust 的内存安全性来减少遗留 C/C++ 代码库中的漏洞，从而提升安全性。 “一级”地位具体意味着安全工具链构建、高效的开发者工具、质量工作流以及与 Windows 平台的深度集成。此举与据报道的微软目标（即可能将数十亿行代码转换为 Rust）相一致，但此类迁移的规模和时间表在此公告中并未得到确认。

hackernews · mmastrac · 9月10日 13:39 · [社区讨论](https://news.ycombinator.com/item?id=49643546)

**背景**: Rust 是一种系统编程语言，以其无需垃圾回收器即可提供内存安全保证而闻名，这主要通过其编译时的“借用检查器”来强制执行。在像微软这样的大型公司内部，“一级语言”意味着它获得了最高级别的官方支持、工具和集成，与 C\# 和 C++ 等语言地位相当。这一地位对于推动其在新项目中的广泛内部采用至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier - 1 Language at Microsoft</a></li>
<li><a href="https://www.compilenrun.com/docs/language/rust/rust-memory-management/rust-memory-safety/">Rust Memory Safety | Compile N Run</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体积极，将此视为对 Rust 作为 C++ 和 C\# 有力竞争者的成熟度的认可。评论强调了此举对微软的战略利益，例如利用 Rust 的内存安全性来解决其产品组合中的安全漏洞（CVE）。此外，社区还讨论了微软更广泛的自动化代码转换至 Rust 的目标，并期待其与 MSVC（Microsoft Visual C++）工具链的集成得到改善。

**标签**: `#rust`, `#microsoft`, `#programming-languages`, `#systems-programming`, `#industry-trends`

---

<a id="item-6"></a>
## [索尼在诉讼中被指使用&\#x27;拥有&\#x27;字眼，挑战数字游戏许可条款](https://consumerrights.wiki/w/Sony_PlayStation_digital_game_ownership_lawsuit) ⭐️ 8.0/10

在一项针对索尼的集体诉讼的法律文件中，原告方整理了一份清单，列举了索尼官方网站和营销材料中多次使用玩家&\#x27;拥有&\#x27;数字版 PlayStation 游戏的表述。这些证据正被用来挑战索尼服务条款的可执行性，因为条款实际只授予了可撤销的许可。 此案可能为数字消费者权利开创重要的法律先例，挑战整个行业将数字商品作为许可而非自有财产出售的普遍做法。若索尼败诉，可能迫使游戏和软件行业在销售方式上更加透明，影响整个行业数百亿美元的收入模式。 该诉讼特别引用了加利福尼亚州的 AB 2426 数字商品法，该法要求当&\#x27;购买&\#x27;按钮指向的是许可而非所有权时，必须进行明确披露。索尼的辩护理由包括&\#x27;理性的消费者不会被误导&\#x27;，且其服务条款包含具有约束力的仲裁条款，并设定了 30 天的退出窗口，旨在阻止集体诉讼。

hackernews · haunter · 9月10日 12:18 · [社区讨论](https://news.ycombinator.com/item?id=49642531)

**背景**: 在版权法中，拥有作品的实体副本和许可数字副本之间存在关键区别。购买实体游戏光盘或书籍意味着你拥有那个特定的副本。然而，对于数字商品，公司通常授予的是受服务条款协议约束的、有限且可撤销的使用许可。这种&\#x27;许可而非拥有&\#x27;的模式在从游戏到软件套件的整个数字媒体领域是标准做法，但其向消费者的传达往往不清晰。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/video-games/console-gaming/playstation-store-buy-button-class-action-may-never-reach-a-courtroom">Sony argues ‘reasonable consumers would not be misled’ into believing they own digital games in class action motion — PlayStation Store ‘buy’ button lawsuit may never reach a courtroom | Tom&#x27;s Hardware</a></li>
<li><a href="https://www.nolo.com/legal-encyclopedia/digital-media-vs-physical-media-do-you-actually-own-what-you-buy.html">Digital Media vs. Physical Media: Do You Actually Own What You Buy?</a></li>

</ul>
</details>

**社区讨论**: 社区评论凸显了对具有约束力的仲裁条款的法律质疑，有用户称其为&\#x27;剥夺人们权利&\#x27;的工具。其他人则剖析了索尼的法律论点，指出用书籍所有权作类比暴露了一个缺陷：购买数字游戏不同于两人购买同一本实体书，因为数字&\#x27;副本&\#x27;并不稀缺。整体情绪对索尼过往行为及数字所有权被普遍侵蚀持批评态度。

**标签**: `#consumer-rights`, `#digital-ownership`, `#legal`, `#gaming`, `#tos`

---

<a id="item-7"></a>
## [TryNix.dev 可在浏览器虚拟机中运行过去 13 年的任何 Nix 包](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 8.0/10

开发者 Farid Zakaria 发布了 trynix.dev，这是一个基于浏览器的工具，它使用 qemu-wasm 运行一个完整的 x86\_64 Linux 虚拟机，能够通过 URL 交互式地启动过去 13 年中的任何 Nix 包。他还构建了一个名为 trynix-preview 的 GitHub Action，能自动发布链接，在浏览器中启动拉取请求的构建以供审查。 该工具极大地降低了测试和审查历史软件环境的门槛，使开发者无需本地配置即可即时运行并与任何历史版本的软件包进行交互。它展示了一种新颖的、无服务器的可重现环境方法，并具有直接的实用价值，例如通过让审查者直接在浏览器中启动拉取请求的确切构建，来简化代码审查流程。 该虚拟机由 qemu-wasm 驱动，这是一个将 QEMU 移植到 WebAssembly 的项目，使其能在浏览器内运行未经修改的 Linux 等软件。软件包可通过 URL 直接寻址（例如 https://trynix.dev/?pkg=python3@3.6.2），并且该系统利用了 Nix 的函数式包管理特性来保证精确重现历史构建。

rss · Simon Willison · 9月10日 23:44

**背景**: Nix 是一个跨平台的函数式包管理器，以其能创建可重现和声明式的软件环境而闻名。QEMU 是一个机器模拟器和虚拟化工具，而 qemu-wasm 是一个实验性的移植项目，它将 QEMU 编译为 WebAssembly，使其能在 Web 浏览器内运行并执行未经修改的操作系统或软件。WebAssembly（Wasm）是一种二进制指令格式，允许用 C++ 等语言编写的代码在 Web 浏览器中以接近原生的速度运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ktock/qemu-wasm">GitHub - ktock/qemu-wasm: QEMU on browser · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nix_%28package_manager%29">Nix (package manager) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Nix`, `#WebAssembly`, `#Virtualization`, `#Developer Tools`

---

<a id="item-8"></a>
## [NASA 卫星图像处理技术现用于揭示褪色的古代岩画](https://spinoff.nasa.gov/Manipulating_Satellite_Photos_Now_Reveals_Ancient_Images) ⭐️ 7.0/10

NASA 开发的一种名为“去相关拉伸”的图像处理技术，最初用于增强卫星和航空摄影，现正被应用于揭示已褪色至近乎不可见的古代岩画。该技术通过一个名为 DStretch 的 ImageJ 程序插件实现，使考古学家能够对图像进行数字增强，恢复肉眼无法看到的细节。 这代表了太空技术一次重要的跨学科应用，能够实现非侵入式的考古发现，并保护那些先前被认为已消失的文化遗产。它为岩画研究和记录开辟了新途径，且不会对脆弱的原始遗址造成破坏。 去相关拉伸算法在不同颜色通道的输入数据接近高斯分布时效果最佳，它能增强人类无法感知的细微颜色差异。DStretch 软件是开源平台 ImageJ 的一个免费插件，这使得研究人员和爱好者都能使用这种高级分析工具。

hackernews · gumby · 9月10日 15:29 · [社区讨论](https://news.ycombinator.com/item?id=49645437)

**背景**: 去相关拉伸是一种遥感图像增强技术，通过降低图像中不同颜色通道之间的相关性来放大细微的光谱差异。该技术最初由 NASA 喷气推进实验室开发，用于分析地球及其他行星的卫星图像，以揭示矿藏或植被健康状况等特征。在考古学中，岩画（岩石绘画）常因风化在数百年间褪色，只留下微弱的矿物颜料痕迹，这些颜料与周围岩石具有不同的光谱特征。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dstretch.com/DecorrelationStretch.pdf">Algorithm Theoretical Basis Document</a></li>
<li><a href="https://dstretch.com/">DStretch .com home page</a></li>
<li><a href="https://en.wikipedia.org/wiki/Decorrelation">Decorrelation - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区成员分享了使用类似假彩色和信号处理技术的个人经验，指出了这些技术在理解传感器如何以不同于人眼的方式感知世界方面的教育价值。几位用户提供了实用的操作建议，例如使用 GIMP 的 LAB 色彩空间分解功能，而其他用户则询问了像 ImageMagick 这样的命令行工具。一位用户讲述了在吴哥窟应用多波段成像未成功的尝试，凸显了实地考察所面临的实际挑战。

**标签**: `#image-processing`, `#remote-sensing`, `#archaeology`, `#signal-processing`, `#nasa`

---

<a id="item-9"></a>
## [PlanetScale 发布 Neki，一款用于水平扩展的分片 PostgreSQL 解决方案。](https://planetscale.com/blog/introducing-neki) ⭐️ 7.0/10

PlanetScale 宣布推出 Neki，这是一款新的分片 PostgreSQL 解决方案，旨在实现数据库工作负载的水平扩展。其发布博客详细介绍了其技术组件和部署过程。 这很重要，因为水平扩展是现代数据密集型应用面临的关键挑战，而来自 PlanetScale 这样主要厂商的托管分片解决方案可以简化复杂的架构问题。它直接满足了超越单服务器实例限制、对可扩展 PostgreSQL 部署日益增长的需求。 一个关键细节是 Neki 是一个闭源的托管服务，这与 Supabase 的 Multigres 等开源替代方案形成对比。该公告没有明确说明 Neki 针对分布式事务的一致性模型（例如，强一致性还是最终一致性），而这是分片数据库的一个核心关切点。

hackernews · simon\_weber · 9月10日 15:43 · [社区讨论](https://news.ycombinator.com/item?id=49645686)

**背景**: 分片是一种数据库扩展技术，它将数据分布在多个服务器（分片）上以处理增加的负载，从而实现水平扩展。PostgreSQL 通过 Citus 等扩展或手动分区来支持分片。PlanetScale 以其基于 Vitess 为 MySQL 构建的分布式数据库平台而闻名，而 Neki 代表了其向 PostgreSQL 生态系统的扩展，同样专注于可扩展的架构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://w3resource.com/PostgreSQL/snippets/postgresql-sharding.php">PostgreSQL Sharding Guide: Horizontal Scaling Made Simple</a></li>
<li><a href="https://planetscale.com/docs/concepts/architecture">PlanetScale database architecture — PlanetScale</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂，对技术有浓厚兴趣但也存在显著批评。关键点包括：对发布文章缺乏清晰产品定义的失望、对 CEO 针对开源替代方案的竞争性语调的批评，以及对 Neki 闭源性质的担忧。社区也提出了关于 Neki 如何在分布式系统中处理一致性的技术问题。

**标签**: `#database`, `#postgresql`, `#scalability`, `#sharding`, `#distributed-systems`

---