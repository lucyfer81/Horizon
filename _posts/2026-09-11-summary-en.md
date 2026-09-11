---
layout: default
title: "Horizon Summary: 2026-09-11 (EN)"
date: 2026-09-11
lang: en
---

> From 13 items, 9 important content pieces were selected

---

1. [Calif Research Demonstrates WeWorm, a Zero-Click Worm Exploiting WeChat Calls with AI Assistance](#item-1) ⭐️ 9.0/10
2. [Shopify migrates mobile apps from React Native back to native Swift and Kotlin.](#item-2) ⭐️ 8.0/10
3. [Researchers question OpenAI&\#x27;s ethics over potential use of unpublished math from collaborative chats.](#item-3) ⭐️ 8.0/10
4. [Cognition launches SWE-2, a cost-efficient AI coding model rivaling top performers.](#item-4) ⭐️ 8.0/10
5. [Microsoft designates Rust as a tier-1 programming language for internal development.](#item-5) ⭐️ 8.0/10
6. [Sony&\#x27;s &\#x27;Ownership&\#x27; References in PlayStation Lawsuit Challenge Digital License Terms](#item-6) ⭐️ 8.0/10
7. [TryNix.dev runs any Nix package from the last 13 years in a browser VM](#item-7) ⭐️ 8.0/10
8. [NASA&\#x27;s Satellite Image Technique Now Uncovers Faded Ancient Rock Art](#item-8) ⭐️ 7.0/10
9. [PlanetScale announces Neki, a sharded PostgreSQL solution for horizontal scalability.](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Calif Research Demonstrates WeWorm, a Zero-Click Worm Exploiting WeChat Calls with AI Assistance](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 9.0/10

Calif Research has released a proof-of-concept demo for WeWorm, a zero-click worm that can spread across iOS and Android devices through WeChat voice calls without any user interaction. The team, with significant AI assistance, discovered the underlying memory corruption bug and developed the initial remote code execution \(RCE\) exploit in about two days, with the full worm built in one additional week. This demonstration represents a paradigm shift in offensive security, showing that AI can dramatically accelerate the discovery and weaponization of critical vulnerabilities, turning what was once a months-long effort for a large team into a matter of days. It highlights a major escalation in threat potential, as zero-click worms can silently compromise devices at scale, posing a severe risk to billions of WeChat users and signaling a new era of AI-powered cyber threats. The exploit targets a memory corruption vulnerability in WeChat&\#x27;s Voice-over-IP \(VoIP\) stack, and the victim does not need to answer the call or interact with their phone for the compromise to succeed. According to reports, the vulnerability has since been blocked by Tencent, the parent company of WeChat, mitigating the immediate risk from this specific proof-of-concept.

rss · Simon Willison · Sep 10, 00:56

**Background**: A zero-click exploit requires no interaction from the victim, such as clicking a link or opening a file, making it extremely stealthy and dangerous. Remote Code Execution \(RCE\) is a severe attack where an attacker can run arbitrary code on a target system from a remote location, often by exploiting software bugs or insecure configurations. AI-assisted vulnerability research involves using large language models \(LLMs\) to automate parts of the security research workflow, such as bug discovery, exploit development, and code analysis, potentially revolutionizing the speed and scale of both offensive and defensive security operations.

<details><summary>References</summary>
<ul>
<li><a href="https://cyberinsider.com/zero-click-worm-spreads-on-iphones-and-android-via-wechat-calls/">Zero-click worm spreads on iPhones and Android via WeChat ...</a></li>
<li><a href="https://www.invicti.com/learn/remote-code-execution-rce">Remote Code Execution (RCE)</a></li>
<li><a href="https://cribl.io/blog/ai-assisted-vulnerability-research-at-cribl/">AI-assisted vulnerability research at Cribl</a></li>

</ul>
</details>

**Tags**: `#ai-security`, `#zero-click-exploit`, `#vulnerability-research`, `#offensive-security`, `#ai-assisted-development`

---

<a id="item-2"></a>
## [Shopify migrates mobile apps from React Native back to native Swift and Kotlin.](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify announced it is migrating its mobile applications from the cross-platform React Native framework back to fully native development using Swift for iOS and Kotlin for Android. The company cited developer experience and performance as key reasons and discussed how Large Language Models \(LLMs\) can assist in such migrations. This decision by a major tech company validates a long-standing debate in mobile development about the trade-offs between cross-platform efficiency and native performance/developer experience. It signals a potential industry shift where the cost-benefit analysis for complex, high-performance apps may increasingly favor native stacks, especially as LLMs lower the migration barrier. Shopify&\#x27;s commentary highlights that LLM-assisted tools can significantly accelerate the migration process, though some community members argue that large-scale migrations were feasible even before advanced LLMs. The move underscores that for large-scale, performance-critical applications, the overhead of debugging across JavaScript, C++, and native threads can outweigh the benefits of a shared codebase.

hackernews · fnthawar2 · Sep 10, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49643982)

**Background**: React Native is a popular cross-platform framework from Meta that allows developers to build mobile apps for iOS and Android using JavaScript and React. The primary appeal is code reuse and leveraging web developer skills for mobile development. Native development with Swift \(iOS\) and Kotlin \(Android\) provides direct access to platform-specific APIs and hardware, typically resulting in better performance and a more polished user experience but requires maintaining separate codebases.

<details><summary>References</summary>
<ul>
<li><a href="https://appinventiv.com/blog/react-native-vs-native-apps/">React Native vs Native: Which is Better for App Development?</a></li>
<li><a href="https://kotlinlang.org/docs/multiplatform/kotlin-multiplatform-react-native.html">Kotlin Multiplatform vs. React Native: A cross-platform comparison | Kotlin Multiplatform Documentation</a></li>
<li><a href="https://blog.bestai.com/rewriting-the-future-how-llm-agents-are-transforming-code-migration/">Rewriting the Future: How LLM Agents Are Transforming Code ...</a></li>

</ul>
</details>

**Discussion**: The community discussion reveals strong validation from native mobile engineers who have long argued against cross-platform compromises for complex apps. Several commenters shared their own migration experiences, noting that LLMs can automate much of the grunt work. A key counterpoint is that while LLMs help, large migrations were already technically possible, and the fundamental decision hinges on long-term performance and maintainability needs rather than just migration cost.

**Tags**: `#mobile-development`, `#react-native`, `#software-architecture`, `#llm`, `#developer-tools`

---

<a id="item-3"></a>
## [Researchers question OpenAI&\#x27;s ethics over potential use of unpublished math from collaborative chats.](https://mathstodon.xyz/@andreasthom/117240535270608201) ⭐️ 8.0/10

A discussion on Mathstodon, led by researcher Andreas Thom, raised serious concerns about whether OpenAI can be trusted with unpublished mathematical work shared in collaborative chats with its models. The core allegation is that OpenAI might use these novel ideas to train its models or publish results without proper attribution to the contributing researchers. This issue strikes at the heart of research integrity and trust in AI companies, as it could deter academics from using AI tools for fear of being scooped or losing credit for their original ideas. It highlights a critical, unresolved tension in the AI research ecosystem: the need for collaborative, open-ended exploration with models versus the protection of intellectual property and academic attribution. The discussion references specific incidents, including OpenAI reportedly generating 300 billion output tokens from a model still in training after learning a major math proof might be in its training data, which some find suspicious. Furthermore, OpenAI&\#x27;s usage policies reserve broad rights to use data to protect its services, but the application of these policies to novel, unpublished research inputs remains ambiguous.

hackernews · pred\_ · Sep 10, 06:49 · [Discussion](https://news.ycombinator.com/item?id=49639408)

**Background**: Mathstodon is a server on the Mastodon network, a decentralized social media platform popular with mathematicians for professional discussion. Researchers often use AI models like OpenAI&\#x27;s ChatGPT or Codex as collaborative tools to brainstorm and refine ideas on unsolved mathematical problems. The training data for large language models typically includes vast amounts of publicly available text from the internet, but the status of private, collaborative chat logs used for research is a gray area with significant ethical implications.

<details><summary>References</summary>
<ul>
<li><a href="https://terrytao.wordpress.com/2022/11/20/trying-out-mathstodon/">Trying out Mathstodon | What&#x27;s new - Terence Tao</a></li>
<li><a href="https://openai.com/policies/usage-policies/">Usage policies | OpenAI</a></li>

</ul>
</details>

**Discussion**: Community sentiment is skeptical and concerned, with users drawing analogies to unethical human collaboration if ideas are used without credit. Key viewpoints include debate over whether model improvements stem from memorizing chat details or from broader reinforcement learning, suspicion about OpenAI&\#x27;s rapid progress on open problems potentially fueled by researcher inputs, and broader unease about trusting companies with sensitive data.

**Tags**: `#AI Ethics`, `#OpenAI`, `#Research Integrity`, `#Academic Collaboration`

---

<a id="item-4"></a>
## [Cognition launches SWE-2, a cost-efficient AI coding model rivaling top performers.](https://cognition.com/blog/swe-2) ⭐️ 8.0/10

Cognition has introduced SWE-2, its latest AI model for software engineering tasks, which reportedly scores 50.0% on the FrontierCode 1.1 Main benchmark, coming within one point of Fable 5.1&\#x27;s performance. The company claims the model achieves this near-frontier capability while being up to 70% cheaper to run. This announcement matters because it introduces a potentially more cost-effective alternative to the current leading AI coding models, which could lower the barrier to entry for advanced AI-assisted development. If its claims hold, it could intensify competition in the coding assistant market, putting pressure on established players to improve performance or reduce costs. A key technical detail is that SWE-2 is post-trained from the Kimi K3 model, rather than being a completely new architecture. Notably, there is a significant performance gap between its score on the older Terminal Bench 2.1 \(92.8%\) and the newer Terminal Bench 4 \(27.3%\), raising questions about its generalization to new, unseen problems.

hackernews · seelos · Sep 10, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49645443)

**Background**: Cognition is the startup behind the autonomous AI coding agent Devin. Models like Fable 5.1 \(from Anthropic\) and GPT-Astra \(from OpenAI\) are considered frontier models, representing the current state-of-the-art in AI capabilities for complex tasks like coding and reasoning. Benchmark scores, such as those on FrontierCode, are commonly used to compare the performance of these large language models \(LLMs\) on specific tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://cognition.com/blog/swe-2">Introducing SWE-2: Pushing the Pareto Frontier | Cognition</a></li>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-1">Introducing Claude Fable 5 . 1 and Claude Mythos 5 . 1 \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT -6 Astra - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community sentiment is skeptical and critical. Key points include doubts about the model&\#x27;s generalization ability due to a large performance drop on a newer benchmark, skepticism about Cognition&\#x27;s past claims regarding its Devin agent, and criticism that SWE-2 is another closed-weight model in a market where users are increasingly favoring open alternatives like DeepSeek.

**Tags**: `#artificial-intelligence`, `#software-engineering`, `#llm`, `#coding-assistant`, `#benchmarks`

---

<a id="item-5"></a>
## [Microsoft designates Rust as a tier-1 programming language for internal development.](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

Microsoft has officially granted Rust &\#x27;tier-1 language&\#x27; status, meaning it now receives full engineering support including secure toolchain builds, deep platform integration, and compliance with Microsoft&\#x27;s Security Development Lifecycle \(SDL\) requirements. This designation provides internal teams with a fully supported, paved path for using Rust from local development to production. This is a major strategic endorsement from one of the world&\#x27;s largest software companies, signaling Rust&\#x27;s maturity and readiness for large-scale, mission-critical systems development. It will accelerate Rust adoption within Microsoft&\#x27;s vast product portfolio, potentially improving security by leveraging Rust&\#x27;s memory safety to reduce vulnerabilities in legacy C/C++ codebases. The &\#x27;tier-1&\#x27; status specifically entails secure toolchain builds, productive developer tooling, quality workflows, and deep integration with Windows platforms. This move aligns with reported Microsoft goals to potentially convert billions of lines of code to Rust, although the scale and timeline for such a migration are not confirmed in this announcement.

hackernews · mmastrac · Sep 10, 13:39 · [Discussion](https://news.ycombinator.com/item?id=49643546)

**Background**: Rust is a systems programming language known for providing memory safety guarantees without a garbage collector, primarily enforced by its compile-time &\#x27;borrow checker&\#x27;. A &\#x27;tier-1 language&\#x27; within a large corporation like Microsoft indicates it receives the highest level of official support, tooling, and integration, comparable to languages like C\# and C++. This status is crucial for enabling widespread internal adoption for new projects.

<details><summary>References</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier - 1 Language at Microsoft</a></li>
<li><a href="https://www.compilenrun.com/docs/language/rust/rust-memory-management/rust-memory-safety/">Rust Memory Safety | Compile N Run</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive, viewing this as validation of Rust&\#x27;s maturity as a serious competitor to C++ and C\#. Comments highlight strategic benefits for Microsoft, such as using Rust&\#x27;s memory safety to address security vulnerabilities \(CVEs\) in its portfolio. There is also discussion about Microsoft&\#x27;s broader goals for automated code conversion to Rust and anticipation for improved MSVC \(Microsoft Visual C++\) toolchain integration.

**Tags**: `#rust`, `#microsoft`, `#programming-languages`, `#systems-programming`, `#industry-trends`

---

<a id="item-6"></a>
## [Sony&\#x27;s &\#x27;Ownership&\#x27; References in PlayStation Lawsuit Challenge Digital License Terms](https://consumerrights.wiki/w/Sony_PlayStation_digital_game_ownership_lawsuit) ⭐️ 8.0/10

A legal filing in a class-action lawsuit against Sony has compiled a list of instances where Sony&\#x27;s own websites and marketing materials referred to players &\#x27;owning&\#x27; their digital PlayStation games. This evidence is being used to challenge the enforceability of Sony&\#x27;s Terms of Service, which actually grant only a revocable license. This case could set a significant legal precedent for digital consumer rights, challenging the industry-wide practice of selling digital goods as licenses rather than owned property. A ruling against Sony could force greater transparency in how games and other digital media are sold, potentially impacting billions in revenue for the entire gaming and software industry. The lawsuit specifically cites California&\#x27;s AB 2426 digital goods law, which requires clear disclosures when a &\#x27;buy&\#x27; button leads to a license, not ownership. Sony&\#x27;s defense includes an argument that &\#x27;reasonable consumers would not be misled,&\#x27; and its Terms contain a binding arbitration clause with a 30-day opt-out window that aims to prevent class actions.

hackernews · haunter · Sep 10, 12:18 · [Discussion](https://news.ycombinator.com/item?id=49642531)

**Background**: In copyright law, a key distinction exists between owning a physical copy of a work and licensing a digital copy. When you buy a physical game disc or book, you own that specific copy. However, for digital goods, companies typically grant a limited, revocable license to use the software, governed by a Terms of Service agreement. This &\#x27;license-not-ownership&\#x27; model is standard across digital media, from games to software suites, but its communication to consumers is often unclear.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/video-games/console-gaming/playstation-store-buy-button-class-action-may-never-reach-a-courtroom">Sony argues ‘reasonable consumers would not be misled’ into believing they own digital games in class action motion — PlayStation Store ‘buy’ button lawsuit may never reach a courtroom | Tom&#x27;s Hardware</a></li>
<li><a href="https://www.nolo.com/legal-encyclopedia/digital-media-vs-physical-media-do-you-actually-own-what-you-buy.html">Digital Media vs. Physical Media: Do You Actually Own What You Buy?</a></li>

</ul>
</details>

**Discussion**: Community comments highlight legal skepticism towards binding arbitration clauses, with one user calling them a tool for &\#x27;taking away people&\#x27;s rights.&\#x27; Others dissect Sony&\#x27;s legal arguments, noting the analogy to book ownership exposes a flaw: purchasing a digital game is not like two people buying the same physical book, as digital &\#x27;copies&\#x27; are not scarce. Sentiment is critical of Sony&\#x27;s past actions and the broader erosion of digital ownership.

**Tags**: `#consumer-rights`, `#digital-ownership`, `#legal`, `#gaming`, `#tos`

---

<a id="item-7"></a>
## [TryNix.dev runs any Nix package from the last 13 years in a browser VM](https://simonwillison.net/2026/Sep/10/trynix/) ⭐️ 8.0/10

Developer Farid Zakaria launched trynix.dev, a browser-based tool that uses qemu-wasm to run a full x86\_64 Linux virtual machine, enabling interactive booting of any Nix package from the past 13 years via a URL. He also built a GitHub Action called trynix-preview that automatically posts a link to boot a pull request&\#x27;s build in the browser for review. This tool significantly lowers the barrier to testing and reviewing historical software environments, enabling developers to instantly run and interact with any past version of a package without local setup. It demonstrates a novel, serverless approach to reproducible environments and has immediate practical applications, such as streamlining code review by letting reviewers boot the exact build from a pull request directly in their browser. The VM is powered by qemu-wasm, a project that ports QEMU to WebAssembly, allowing it to run unmodified software like Linux inside a browser. The packages are URL-addressable \(e.g., https://trynix.dev/?pkg=python3@3.6.2\), and the system leverages Nix&\#x27;s functional package management to guarantee the exact historical build is reproduced.

rss · Simon Willison · Sep 10, 23:44

**Background**: Nix is a cross-platform, functional package manager known for creating reproducible and declarative software environments. QEMU is a machine emulator and virtualizer, and qemu-wasm is an experimental port that compiles QEMU to WebAssembly, enabling it to run inside a web browser and execute unmodified operating systems or software. WebAssembly \(Wasm\) is a binary instruction format that allows code written in languages like C++ to run at near-native speed in web browsers.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ktock/qemu-wasm">GitHub - ktock/qemu-wasm: QEMU on browser · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nix_%28package_manager%29">Nix (package manager) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Nix`, `#WebAssembly`, `#Virtualization`, `#Developer Tools`

---

<a id="item-8"></a>
## [NASA&\#x27;s Satellite Image Technique Now Uncovers Faded Ancient Rock Art](https://spinoff.nasa.gov/Manipulating_Satellite_Photos_Now_Reveals_Ancient_Images) ⭐️ 7.0/10

A NASA-developed image processing technique called decorrelation stretch, originally used to enhance satellite and aerial photography, is now being applied to reveal ancient rock art that has faded to near-invisibility. The technique is implemented in a software plugin called DStretch for the ImageJ program, allowing archaeologists to digitally enhance images and recover details lost to the naked eye. This represents a significant cross-disciplinary application of space technology, enabling non-invasive archaeological discovery and preservation of cultural heritage that was previously considered lost. It opens new avenues for rock art research and documentation without damaging the fragile original sites. The decorrelation stretch algorithm works best when the input data from different color channels has a near-Gaussian distribution, and it enhances subtle color differences that are imperceptible to humans. The DStretch software is a free plugin for the open-source ImageJ platform, making this advanced analysis accessible to researchers and enthusiasts.

hackernews · gumby · Sep 10, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49645437)

**Background**: Decorrelation stretch is a remote sensing image enhancement technique that reduces the correlation between color channels in an image to amplify subtle spectral differences. Originally developed by NASA&\#x27;s Jet Propulsion Laboratory for analyzing satellite imagery of Earth and other planets, it helps reveal features like mineral deposits or vegetation health. In archaeology, pictographs \(rock paintings\) often fade over centuries due to weathering, leaving only faint mineral-based pigments that retain distinct spectral signatures different from the surrounding rock.

<details><summary>References</summary>
<ul>
<li><a href="https://dstretch.com/DecorrelationStretch.pdf">Algorithm Theoretical Basis Document</a></li>
<li><a href="https://dstretch.com/">DStretch .com home page</a></li>
<li><a href="https://en.wikipedia.org/wiki/Decorrelation">Decorrelation - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community members shared personal experiences with similar false-color and signal processing techniques, noting their educational value in understanding how sensors perceive the world differently than human eyes. Several users provided practical implementation tips, such as using GIMP&\#x27;s LAB color space decomposition, while others inquired about command-line tools like ImageMagick. One user recounted an unsuccessful attempt to apply multi-band imaging at Angkor Wat, highlighting the practical challenges of fieldwork.

**Tags**: `#image-processing`, `#remote-sensing`, `#archaeology`, `#signal-processing`, `#nasa`

---

<a id="item-9"></a>
## [PlanetScale announces Neki, a sharded PostgreSQL solution for horizontal scalability.](https://planetscale.com/blog/introducing-neki) ⭐️ 7.0/10

PlanetScale has announced Neki, a new sharded PostgreSQL solution designed to enable horizontal scalability for database workloads. The launch blog post details its technical components and deployment process. This matters because horizontal scaling is a critical challenge for modern, data-intensive applications, and a managed sharding solution from a major player like PlanetScale could simplify a complex architectural problem. It directly addresses the growing demand for scalable PostgreSQL deployments beyond the limitations of single-server instances. A key detail is that Neki is a closed-source, managed service, which contrasts with open-source alternatives like Supabase&\#x27;s Multigres. The announcement did not explicitly clarify Neki&\#x27;s consistency model \(e.g., strong vs. eventual\) for distributed transactions, which is a core concern for sharded databases.

hackernews · simon\_weber · Sep 10, 15:43 · [Discussion](https://news.ycombinator.com/item?id=49645686)

**Background**: Sharding is a database scaling technique that distributes data across multiple servers \(shards\) to handle increased load, enabling horizontal scalability. PostgreSQL supports sharding through extensions like Citus or manual partitioning. PlanetScale is known for its distributed database platform built on Vitess for MySQL, and Neki represents its expansion into the PostgreSQL ecosystem with a similar focus on scalable architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://w3resource.com/PostgreSQL/snippets/postgresql-sharding.php">PostgreSQL Sharding Guide: Horizontal Scaling Made Simple</a></li>
<li><a href="https://planetscale.com/docs/concepts/architecture">PlanetScale database architecture — PlanetScale</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed, with strong interest in the technology but significant criticism. Key points include frustration over the launch post&\#x27;s lack of a clear product definition, criticism of the CEO&\#x27;s competitive tone towards open-source alternatives, and concerns about Neki being closed-source. Technical questions were also raised about how Neki handles consistency in a distributed system.

**Tags**: `#database`, `#postgresql`, `#scalability`, `#sharding`, `#distributed-systems`

---