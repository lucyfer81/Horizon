---
layout: default
title: "Horizon Summary: 2026-10-23 (EN)"
date: 2026-10-23
lang: en
---

> From 17 items, 8 important content pieces were selected

---

1. [Project Enables iOS 16.5 to Run on Android Devices via Modified XNU Kernel](#item-1) ⭐️ 8.0/10
2. [Nintendo Switch 2 Jailbreak Achieves Full Filesystem Access](#item-2) ⭐️ 8.0/10
3. [eMudhra Exits Global SSL/TLS Certificate Business After Private Key Exposure Incident](#item-3) ⭐️ 8.0/10
4. [Earstrip library achieves 3.5x speedup over Earcut, triangulating 3.7M map polygons in 489 ms.](#item-4) ⭐️ 8.0/10
5. [Quad9 DNS Resolver to Exit France Over Court-Ordered Piracy Blocks](#item-5) ⭐️ 7.0/10
6. [NVIDIA releases OpenShell, a secure runtime for autonomous AI agents.](#item-6) ⭐️ 7.0/10
7. [Woman faces six years in prison over fraudulent Cash App account opened via identity theft.](#item-7) ⭐️ 7.0/10
8. [Anthropic Donates Agent Skills Standard to Agentic AI Foundation](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Project Enables iOS 16.5 to Run on Android Devices via Modified XNU Kernel](https://github.com/oosexgang/hackios-xnu-kernel) ⭐️ 8.0/10

A GitHub project named &\#x27;hackios-xnu-kernel&\#x27; has successfully demonstrated running the full iOS 16.5 firmware on select Android devices, including specific Xiaomi phones and the QEMU emulator, by modifying Apple&\#x27;s XNU kernel. This represents a significant technical breakthrough in cross-platform mobile OS execution. This project challenges the long-standing hardware-software lock-in of Apple&\#x27;s ecosystem, demonstrating deep reverse engineering prowess. It could have implications for security research, device compatibility testing, and potentially opens discussions about the portability of closed-source operating systems. The implementation is described as a &\#x27;research bench&\#x27; rather than a full ROM, with sessions lasting a limited time before the kernel returns to a loader. It currently works on devices like the POCO X5 Pro 5G and faces technical hurdles such as adapting XNU&\#x27;s 16K memory pages to Android hardware that typically uses 4K pages.

hackernews · aghuang · Oct 22, 15:26 · [Discussion](https://news.ycombinator.com/item?id=50196718)

**Background**: Apple&\#x27;s iOS is a closed-source operating system tightly integrated with its proprietary hardware and uses the XNU kernel, which is fundamentally different from the Linux kernel used by Android. Running iOS on non-Apple hardware requires extensive reverse engineering to spoof device drivers and adapt the kernel&\#x27;s system call interface. QEMU is an open-source machine emulator and virtualizer often used by developers to test operating systems without physical hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://www.androidauthority.com/ios-on-android-phones-3726001/">Forget custom ROMs, you can now run iOS on ... - Android Authority</a></li>
<li><a href="https://github.com/MakrSas/ios-topaz">GitHub - MakrSas/ ios -topaz: iOS 16 userland + XNU on Redmi Note 12?</a></li>
<li><a href="https://blog.usro.net/2024/10/how-to-run-android-on-your-pc-using-qemu-a-step-by-step-guide/">How to Run Android on Your PC Using QEMU: A Step-by-Step Guide</a></li>

</ul>
</details>

**Discussion**: Community sentiment is a mix of technical admiration and practical skepticism. Comments praise the impressive technical feat of getting iOS to run on QEMU and specific phones, while others note its current limitations as a research tool. Some discuss broader implications, such as the potential for increased counterfeit iPhones, while a few express that modern iOS&\#x27;s perceived &\#x27;clunkiness&\#x27; reduces their personal desire for such a port.

**Tags**: `#iOS`, `#Android`, `#Kernel`, `#Reverse Engineering`, `#Mobile`

---

<a id="item-2"></a>
## [Nintendo Switch 2 Jailbreak Achieves Full Filesystem Access](https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb/) ⭐️ 8.0/10

A detailed technical blog post published in October 2026 describes a successful jailbreak of the Nintendo Switch 2, which provides read/write access to the console&\#x27;s encrypted filesystem. This breakthrough enables the potential dumping of game data and could lead to the console&\#x27;s emulation on other hardware. This jailbreak is significant as it could rapidly lead to the piracy of Switch 2 games and enable them to be played on non-Nintendo hardware, representing a major security failure for Nintendo. It also has profound implications for game preservation and the emulation community, potentially accelerating the availability of Switch 2 games on platforms like PC and mobile. The jailbreak process involved using automated tools like &\#x27;JetKVMs&\#x27; to send controller inputs and capture video output, and a physical &\#x27;SwitchBot Bot&\#x27; device to press the power button for system recovery. The blog post suggests the researchers utilized AI/LLM tools \(referred to as &\#x27;Codex&\#x27;\) to assist in the reverse-engineering and exploitation process.

hackernews · ledoge · Oct 22, 08:01 · [Discussion](https://news.ycombinator.com/item?id=50192536)

**Background**: Jailbreaking a game console involves exploiting security vulnerabilities to bypass manufacturer restrictions, allowing the installation of unofficial software and access to the system&\#x27;s underlying functions. Filesystem access is a critical step in jailbreaking, as it allows users to read and modify system files, which is necessary for actions like dumping game ROMs. Game dumping is the process of extracting the data from a physical game cartridge or disc to create a digital copy, which is a prerequisite for playing console games on emulators.

<details><summary>References</summary>
<ul>
<li><a href="https://lifehacker.com/is-it-legal-to-jailbreak-a-video-game-console-1848558154">Is It Legal to Jailbreak a Video Game Console? - Lifehacker How do jailbreaked consoles work? : r/PiratedGames - Reddit PS5 Jailbreak Explained: Benefits, Risks and Legality Which Consoles Can Be Jailbroken in 2025? - ExpertBeacon A new PS5 jailbreak works on almost every firmware version ... Game Console Jailbreaking: Benefits and Risks | MobileBurn The PS5 hacking scene just took a big leap forward</a></li>
<li><a href="https://emulation.gametechwiki.com/index.php/Ripping_games">Ripping games - Emulation General Wiki</a></li>

</ul>
</details>

**Discussion**: The community expressed excitement about the technical achievement and its immediate implications, with one user predicting Switch 2 game dumps could appear within hours. There was also notable discussion about the sophisticated, automated setup involving KVMs and a SwitchBot, and curiosity about the use of AI/LLM tools for such security research, with one user questioning how they bypassed typical usage restrictions.

**Tags**: `#hardware-hacking`, `#reverse-engineering`, `#game-console`, `#security`, `#emulation`

---

<a id="item-3"></a>
## [eMudhra Exits Global SSL/TLS Certificate Business After Private Key Exposure Incident](https://emudhra.com/en/press-release/emudhra-to-exit-global-ssl-tls-certificate-business) ⭐️ 8.0/10

eMudhra Limited announced it is exiting the global SSL/TLS certificate business following a security incident where weak private keys for eight intermediate Certificate Authority \(CA\) certificates were exposed, potentially in public code repositories. The company stated this business segment contributed only about 1% of its global revenue. This is significant because a Certificate Authority&\#x27;s core responsibility is safeguarding private keys; their exposure undermines the trust foundation of the entire web PKI. The incident has led major browser vendors like Chrome and Firefox to withdraw trust from eMudhra&\#x27;s root certificates, forcing its exit and highlighting the severe reputational and operational consequences of CA failures. The exposed keys were reportedly weak, with one example being a simple RSA private key containing the number &\#x27;4&\#x27;. Despite the exposure, eMudhra claimed no end-entity certificates were issued from the affected CAs, a statement questioned by the community given that anyone with the private key could issue certificates.

hackernews · bo0tzz · Oct 22, 13:33 · [Discussion](https://news.ycombinator.com/item?id=50195110)

**Background**: SSL/TLS certificates are digital credentials that enable secure, encrypted connections \(HTTPS\) between web browsers and servers. A Certificate Authority \(CA\) is a trusted entity that issues these certificates; its private keys must be kept secret, as anyone possessing them can create fraudulent certificates for any website, breaking the web&\#x27;s security model. The Web PKI ecosystem relies on browser and operating system vendors to maintain lists of trusted root CAs.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/emudhra-exits-global-ssl-tls-certificate/">eMudhra Exits Global SSL/TLS Certificate Business Following ...</a></li>
<li><a href="https://arstechnica.com/security/2026/10/disgraced-emudhra-drops-out-of-tls-business-following-certificate-debacle/">Disgraced eMudhra drops out of TLS business after using cert ...</a></li>
<li><a href="https://thehackernews.com/2026/10/emudhra-to-exit-global-ssltls-business.html">eMudhra to Exit Global SSL/TLS Business After 8 Intermediate ...</a></li>

</ul>
</details>

**Discussion**: The community expressed severe criticism and disbelief at the scale of the operational failure, with comments highlighting the absurdly weak exposed key \(&\#x27;4&\#x27;\) and sharing a link to a rigorous public audit by the Chrome team. There is skepticism towards eMudhra&\#x27;s claim that no end-entity certificates were issued, and the overall sentiment is that the company&\#x27;s response and security practices were inadequate.

**Tags**: `#Security`, `#PKI`, `#SSL/TLS`, `#Certificate-Authority`, `#Infrastructure`

---

<a id="item-4"></a>
## [Earstrip library achieves 3.5x speedup over Earcut, triangulating 3.7M map polygons in 489 ms.](https://globus.software/blog/2026/10/16/cutting-map-polygons/) ⭐️ 8.0/10

A new library called Earstrip was released, demonstrating a significant performance improvement by triangulating 3.7 million map polygons in 489 milliseconds using WebAssembly. This represents a 3.5x speedup compared to the widely-used JavaScript library Earcut. This matters because polygon triangulation is a fundamental operation for rendering maps, CAD models, and data visualizations in real-time web applications. A 3.5x performance gain can enable smoother interactions and the processing of more complex datasets directly in the browser, pushing the boundaries of web-based computational geometry. The performance benchmark was conducted on a specific corpus of map polygon data, and the library is implemented in WebAssembly, likely using Rust or C++. A key trade-off noted is that the optimization may produce long, thin triangles, which could be suboptimal for GPU rasterization, and the library&\#x27;s bundle size compared to Earcut&\#x27;s minimal 4.1KB gzipped size is a point of discussion.

hackernews · molind · Oct 22, 09:31 · [Discussion](https://news.ycombinator.com/item?id=50193170)

**Background**: Polygon triangulation is the process of dividing a polygon into a set of non-overlapping triangles, which is essential for rendering shapes in computer graphics and GIS. Earcut is a popular, fast, and small JavaScript library for this purpose, widely used in projects like Mapbox GL JS. WebAssembly \(WASM\) is a binary instruction format that allows code written in languages like Rust or C++ to run in the browser at near-native speed, making it suitable for computationally intensive tasks like geometry processing.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/mapbox/earcut">GitHub - mapbox/earcut: The fastest and smallest JavaScript ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Polygon_triangulation">Polygon triangulation - Wikipedia</a></li>
<li><a href="https://altersquare.io/blog/webassembly-for-cad-applications-when-javascript-isnt-fast-enough">WebAssembly for CAD Applications: When JavaScript Isn’t Fast ...</a></li>

</ul>
</details>

**Discussion**: The discussion includes praise for the performance gains and technical insights from other library authors. The author of Earcut acknowledged the achievement but highlighted the design trade-off of prioritizing minimal bundle size over peak performance for web use. Other comments raised questions about alternative algorithms like Seidel&\#x27;s method, the quality of the generated triangles for GPU rendering, and comparisons with other triangulators like Delaunay32 and the classic Triangle library.

**Tags**: `#computational-geometry`, `#performance`, `#algorithms`, `#webassembly`, `#mapping`

---

<a id="item-5"></a>
## [Quad9 DNS Resolver to Exit France Over Court-Ordered Piracy Blocks](https://quad9.net/news/blog/au-revoir-france/) ⭐️ 7.0/10

Quad9, a non-profit, privacy-focused DNS resolver, announced it will exit the French market following a Paris court order requiring it to block access to specific piracy websites. The company faced fines for non-compliance after the plaintiff used a VPN to circumvent its geo-blocking measures. This sets a significant legal precedent by holding a DNS resolver, a core internet infrastructure service, directly liable for content blocking, potentially expanding intermediary liability across the EU. It raises concerns about the effectiveness and proportionality of using DNS blocking to combat piracy and could pressure other infrastructure providers to comply with similar orders or exit markets. The initial court order in May 2025, requested by beIN Sports, required Quad9, Google, and DNS4EU to block six domains streaming WTA tennis matches in France. Quad9&\#x27;s planned exit, effective after November 24, likely involves using geoIP filtering to block French users, a method the company had previously criticized as insufficient for selective blocking.

hackernews · farrokhi · Oct 22, 14:32 · [Discussion](https://news.ycombinator.com/item?id=50195959)

**Background**: A DNS resolver translates human-readable domain names \(like quad9.net\) into machine-readable IP addresses, acting as a phone book for the internet. Quad9 is a public, non-profit resolver known for its privacy and security features, which does not log user queries. Internet intermediaries, such as DNS providers, have traditionally enjoyed liability protections under laws like the EU&\#x27;s e-commerce directive, but recent court rulings are testing these limits.

<details><summary>References</summary>
<ul>
<li><a href="https://quad9.net/news/blog/au-revoir-france/">A public and free DNS service for a better security and privacy | Quad9</a></li>
<li><a href="https://torrentfreak.com/dns-resolver-quad9-rejects-french-piracy-blocks-weighs-exit-as-bein-seeks-up-to-e580k-a-day/">DNS Resolver Quad 9 Rejects French Piracy Blocks... * TorrentFreak</a></li>
<li><a href="https://cis-india.org/internet-governance/blog/intermediary-liability-resources">Intermediary Liability Resources — Centre for Internet and Society</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely supportive of Quad9, with users criticizing the court&\#x27;s logic as akin to punishing a phone book company for listing a criminal&\#x27;s number. Comments highlight the technical futility of geo-blocking when VPNs can easily circumvent it and note that other providers like Cisco have previously made similar exits. Some suggest retaliatory measures, such as resolvers blocking the domains of the companies that sue them.

**Tags**: `#DNS`, `#Internet Governance`, `#Legal`, `#Privacy`, `#Censorship`

---

<a id="item-6"></a>
## [NVIDIA releases OpenShell, a secure runtime for autonomous AI agents.](https://github.com/NVIDIA/OpenShell) ⭐️ 7.0/10

NVIDIA has released OpenShell 0.1.0, an open-source runtime environment that allows developers to define and enforce security policies for what systems and data an AI agent can access. It provides controlled capabilities like reading files and calling APIs without granting unrestricted access to data, secrets, or the network. This addresses a critical security gap in deploying autonomous AI agents at scale, as uncontrolled agents pose risks of data exfiltration and unauthorized actions. By providing a standardized, policy-driven runtime from a major industry player, it could accelerate the safe adoption of agentic AI in enterprise and production environments. OpenShell combines sandboxed execution, controlled service access, credential management, and formal policy analysis to restrict operations. The initial release \(0.1.0\) is already being used by organizations like Cadence, Slack, and Gecko Robotics for securing their AI agent deployments.

hackernews · niemandhier · Oct 22, 17:44 · [Discussion](https://news.ycombinator.com/item?id=50198675)

**Background**: Autonomous AI agents are software programs that can perform tasks independently, such as reading files, installing packages, or calling APIs. Deploying them safely requires strict access controls to prevent security incidents like prompt injection attacks or data exfiltration, similar to the need for containerization in traditional software. Tools that provide secure, isolated runtimes with policy enforcement are becoming essential for managing fleets of such agents in production.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/NVIDIA/OpenShell">OpenShell – private runtime for autonomous AI agents</a></li>
<li><a href="https://developer.nvidia.com/blog/add-runtime-controls-to-ai-agents-with-nvidia-openshell/">Add Runtime Controls to AI Agents with NVIDIA OpenShell</a></li>
<li><a href="https://blog.aimodularity.com/how-to-implement-ai-agent-access-control">How to Implement AI Agent Access Control — AI Modularity</a></li>

</ul>
</details>

**Discussion**: Community discussion highlights practical security concerns and existing solutions. Some users note that while tools like network proxies or containers address parts of the problem, preventing data exfiltration remains a challenge. Others see OpenShell as a valuable management layer for containers, while a comment points out the inherent tension between granting an agent capability and maintaining security, suggesting the tool helps strike a balance.

**Tags**: `#ai-agents`, `#security`, `#runtime`, `#nvidia`, `#devops`

---

<a id="item-7"></a>
## [Woman faces six years in prison over fraudulent Cash App account opened via identity theft.](https://www.techspot.com/news/114296-woman-spends-three-nights-jail-faces-six-years.html) ⭐️ 7.0/10

Amanda Smith has been charged with multiple felonies and faces up to six years in prison for financial fraud conducted through a Cash App account that was opened using her stolen identity. She has refused a plea deal offered by authorities, which included a fine, restitution, and probation, maintaining her innocence. This case highlights critical flaws in financial technology platforms&\#x27; identity verification processes and exposes how prosecutorial practices can pressure innocent victims into accepting plea deals. It raises urgent questions about accountability for financial institutions and the justice system&\#x27;s handling of identity theft. The prosecution&\#x27;s case relies on linking the fraudulent account to Smith, despite her claim that it was opened without her knowledge. The offered plea deal, which would have avoided a trial, is a common tactic that places significant pressure on defendants, even innocent ones, to accept guilt.

hackernews · oidar · Oct 22, 13:11 · [Discussion](https://news.ycombinator.com/item?id=50194833)

**Background**: Cash App is a peer-to-peer payment service that requires users to verify their identity for certain transactions, typically involving providing personal information like a Social Security Number. Identity theft involves someone using another person&\#x27;s personal data without permission to commit fraud or other crimes. In the U.S. legal system, prosecutors often use plea deals to resolve cases without a trial, which can create incentives for innocent defendants to plead guilty to avoid the risk of a harsher sentence if convicted at trial.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@rufscwttet/how-to-verify-your-identity-on-cash-app-a-comprehensive-guide-33f8e9217a14">How to Verify Your Identity on Cash App : A Comprehensive... | Medium</a></li>
<li><a href="https://dutyanchor.com/prosecuting-fraud-cases/">Strategies for Effectively Prosecuting Fraud Cases in the ...</a></li>
<li><a href="https://tribunae.com/liability-in-identity-theft-cases/">Understanding Liability in Identity Theft Cases: Legal ...</a></li>

</ul>
</details>

**Discussion**: Community comments express strong criticism of prosecutorial overreach and the plea deal system, viewing the offer as a coercive tactic to avoid admitting investigative errors. Many call for holding Cash App accountable for facilitating fraud through weak verification and for making law enforcement personally liable for negligent investigations.

**Tags**: `#identity-theft`, `#financial-tech`, `#legal-system`, `#privacy`, `#social-justice`

---

<a id="item-8"></a>
## [Anthropic Donates Agent Skills Standard to Agentic AI Foundation](https://simonwillison.net/2026/Oct/22/donating-agent-skills/) ⭐️ 7.0/10

On October 22, 2026, Anthropic announced it is donating its Agent Skills specification to the vendor-neutral Agentic AI Foundation \(AAIF\) under the Linux Foundation. This follows Anthropic&\#x27;s previous donation of the Model Context Protocol \(MCP\) to the same foundation, which it co-founded with Block and OpenAI in 2025. This move promotes open, community-driven, and vendor-neutral development in the agentic AI space, preventing fragmentation and lock-in. It signals a major industry trend where leading AI companies are collaborating on foundational standards to ensure interoperability and accelerate ecosystem growth. Agent Skills is a lightweight, open format where a &\#x27;skill&\#x27; is essentially a folder containing a SKILL.md file with metadata and instructions, plus optional resources. The AAIF, launched in December 2025, already hosts the MCP standard and has major backers like AWS, Google, Microsoft, and OpenAI.

rss · Simon Willison · Oct 22, 18:09

**Background**: Agent Skills are packages that extend AI agent capabilities with specialized knowledge and workflows, allowing agents to discover and load them on demand. The Model Context Protocol \(MCP\) is an open standard for connecting AI applications to external data sources and tools. The Agentic AI Foundation \(AAIF\) is a Linux Foundation initiative focused on developing open, interoperable infrastructure for autonomous AI systems that plan and execute tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://agentskills.io/home">Agent Skills Overview - Agent Skills</a></li>
<li><a href="https://modelcontextprotocol.io/docs/2026-07-28/getting-started/intro">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>
<li><a href="https://www.linuxfoundation.org/press/linux-foundation-announces-the-formation-of-the-agentic-ai-foundation">Linux Foundation Announces the Formation of the Agentic AI ...</a></li>

</ul>
</details>

**Tags**: `#AI Agents`, `#Open Standard`, `#Industry Collaboration`, `#AI Governance`

---