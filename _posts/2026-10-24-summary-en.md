---
layout: default
title: "Horizon Summary: 2026-10-24 (EN)"
date: 2026-10-24
lang: en
---

> From 7 items, 4 important content pieces were selected

---

1. [Security Researchers Demonstrate Exploit Chain to Gain Root Access on Modern iPhone](#item-1) ⭐️ 9.0/10
2. [Dessa: A full-duplex speech AI model achieving low-latency, expressive conversation on local hardware.](#item-2) ⭐️ 8.0/10
3. [Moonshot AI releases Kimi K3.1 Pro and K3.1 Pro Highspeed models with deliberate limits on offensive cyber capabilities.](#item-3) ⭐️ 7.0/10
4. [Google updates privacy policy, may use Gmail and Photos data for ads under DMA.](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Security Researchers Demonstrate Exploit Chain to Gain Root Access on Modern iPhone](https://blog.calif.io/p/iphone) ⭐️ 9.0/10

A team of security researchers has successfully demonstrated a significant exploit chain that allows them to gain root access on a modern iPhone. This achievement represents a major breakthrough in iOS security research, often referred to as a &\#x27;jailbreak&\#x27;. This demonstration is significant because it highlights potential security vulnerabilities in a widely used, closed ecosystem like iOS, even on modern devices. It matters for security researchers, Apple&\#x27;s security team, and users concerned about device control, as it underscores the ongoing cat-and-mouse game between exploit discovery and platform hardening. The exploit involves chaining multiple vulnerabilities together to achieve a deep level of compromise \(root access\) that no single flaw could accomplish alone. The demonstration was shared publicly, generating substantial discussion within the technical community about its implications.

hackernews · pavel\_lishin · Oct 23, 16:21 · [Discussion](https://news.ycombinator.com/item?id=50211474)

**Background**: An &\#x27;exploit chain&\#x27; is a sequence of multiple vulnerabilities combined to compromise a system, where the full attack is greater than the sum of its parts. &\#x27;Jailbreaking&\#x27; an iPhone is the process of removing software restrictions imposed by iOS to gain root access, which can enable unauthorized software installation but also increases security risks. A &\#x27;zero-day&\#x27; vulnerability is a security flaw unknown to the vendor, making it highly valuable for attackers and defenders alike until a patch is released.

<details><summary>References</summary>
<ul>
<li><a href="https://www.csoonline.com/article/571799/exploit-chains-explained-how-and-why-attackers-target-multiple-vulnerabilities.html">Exploit chains explained: How and why attackers target ...</a></li>
<li><a href="https://www.tomsguide.com/us/pictures-story/537-jailbreaking-iphone-pros-cons.html">10 Pros and Cons of Jailbreaking Your iPhone or iPad | Tom&#x27;s Guide</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community sentiment is a mix of technical admiration and frustration with ecosystem control. Key viewpoints include sadness over the loss of early Android-like tinkering freedom due to Apple&\#x27;s integrated ecosystem \(iCloud, iMessage lockouts\), criticism of exclusive &\#x27;Red Team&\#x27; access programs in security research creating a &\#x27;moat&\#x27;, and practical questions about whether Apple&\#x27;s Lockdown Mode or future updates could mitigate such exploits.

**Tags**: `#security`, `#ios`, `#reverse-engineering`, `#jailbreak`, `#zero-day`

---

<a id="item-2"></a>
## [Dessa: A full-duplex speech AI model achieving low-latency, expressive conversation on local hardware.](https://block.xyz/dessa) ⭐️ 8.0/10

Dessa is a new full-duplex speech model that achieves low-latency, expressive conversation and runs locally on high-end consumer hardware like a MacBook Pro M4 Max. It was trained with relatively efficient compute, reportedly using only one NVIDIA GB200 NVL72 system. This matters because it pushes the boundary of realistic, real-time voice AI interactions from the cloud to personal devices, enhancing privacy and accessibility. It demonstrates that highly expressive, low-latency conversational AI can be achieved with more efficient training and on-edge deployment, potentially enabling new applications in personal assistants, gaming, and accessibility tools. The model&\#x27;s ability to run locally on a MacBook Pro M4 Max suggests significant optimization for edge computing. However, community comments indicate skepticism about the sensationalist &\#x27;most authentic ever&\#x27; marketing claim and note that the model&\#x27;s training data likely includes many podcasts.

hackernews · dsr12 · Oct 23, 19:09 · [Discussion](https://news.ycombinator.com/item?id=50213925)

**Background**: Full-duplex speech models are AI systems capable of simultaneous listening and speaking, enabling natural, overlapping dialogue and dynamic turn-taking, unlike traditional turn-based voice assistants. Edge computing for AI involves running models on local devices rather than in the cloud, which reduces latency, enhances privacy, and allows operation in bandwidth-limited environments. Training large AI models like this typically requires massive computational resources, so achieving similar results with &\#x27;relatively efficient compute&\#x27; is a notable technical challenge.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/full-duplex-speech-llms">Full - Duplex Speech LLMs</a></li>
<li><a href="https://arxiv.org/html/2609.34461">CharDuplex: Building Character-Consistent Full - Duplex Spoken...</a></li>
<li><a href="https://www.mdpi.com/2078-2489/16/8/685">Real-Time Speech-to-Text on Edge: A Prototype System for ...</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed, combining technical admiration with skepticism. Some users are impressed by the low-latency local performance and efficient training. Others criticize the sensationalist title as marketing hype, express discomfort with the &\#x27;AI girlfriend&\#x27; style of demo conversation, and question the nature of the training data, speculating it is heavily based on podcasts.

**Tags**: `#speech-synthesis`, `#ai-models`, `#edge-computing`, `#machine-learning`, `#real-time`

---

<a id="item-3"></a>
## [Moonshot AI releases Kimi K3.1 Pro and K3.1 Pro Highspeed models with deliberate limits on offensive cyber capabilities.](https://www.kimi.ai/blog/kimi-k3-1-pro) ⭐️ 7.0/10

Moonshot AI has announced the release of the Kimi K3.1 Pro and K3.1 Pro Highspeed AI models, which are updates to the K3 series. The company explicitly states that the open-weights version of K3.1 Pro has its offensive cyber capability deliberately limited below what their internal pipeline can produce and below frontier proprietary models. This release is significant as it represents a major update from a leading AI company, with performance improvements noted in benchmarks. More importantly, it highlights a growing industry debate about the responsible release of powerful AI models, specifically whether and how to limit their potential for misuse in areas like cybersecurity. The K3.1 Pro model showed a significant performance jump in a data analytics benchmark, scoring 98% compared to K3&\#x27;s 81%, though it was noted to be slower due to making many more tool calls. The model architecture is based on the K3 series, which uses Kimi Delta Attention \(KDA\) and Attention Residuals \(AttnRes\) for efficiency.

hackernews · Jowsey · Oct 23, 16:59 · [Discussion](https://news.ycombinator.com/item?id=50212065)

**Background**: Kimi K3 is a large multimodal reasoning model from Moonshot AI, featuring a 2.8 trillion parameter architecture. It employs a novel Kimi Delta Attention \(KDA\) mechanism and a sparse Mixture-of-Experts \(MoE\) design, activating only 16 out of 896 experts for computational efficiency. The term &\#x27;offensive cyber capability&\#x27; in AI models refers to their potential to assist in activities like vulnerability discovery, exploit development, or network intrusion, raising dual-use concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3">moonshotai/ Kimi -K3 · Hugging Face</a></li>
<li><a href="https://openrouter.ai/moonshotai/kimi-k3">Kimi K3 - API Pricing &amp; Benchmarks | OpenRouter</a></li>
<li><a href="https://pentesttoday.com/blog/open-weights-models-offensive-cyber">Open weights models are surprisingly aligned on offensive cyber</a></li>

</ul>
</details>

**Discussion**: Community discussion highlights several points: users note Kimi&\#x27;s distinctively blunt and argumentative personality compared to other models. Some observed inconsistencies in the model&\#x27;s self-identification during reasoning. There were complaints about restrictive subscription quotas, and significant debate was sparked by the company&\#x27;s stated policy of deliberately limiting the model&\#x27;s offensive cyber capabilities in its open release, with users questioning the rationale and implications.

**Tags**: `#ai-models`, `#llm`, `#open-source`, `#cybersecurity`, `#model-evaluation`

---

<a id="item-4"></a>
## [Google updates privacy policy, may use Gmail and Photos data for ads under DMA.](https://www.theverge.com/tech/1017600/google-personal-intelligence-privacy-policy-ads-update) ⭐️ 7.0/10

Google has updated its privacy policy to state that it might use data from services like Gmail and Google Photos for personalized advertising. This change is specifically linked to provisions in the EU&\#x27;s Digital Markets Act \(DMA\) regarding linked services. This policy shift could significantly expand the pool of personal data Google uses for ad targeting, directly impacting user privacy. It also highlights how major tech companies are adapting their data practices in response to new regulations like the DMA, which aims to regulate &\#x27;gatekeeper&\#x27; platforms. The policy clarifies that data from these services will not be used for ads unless users choose to link these services to other Google services that support personalized ads, a nuance highlighted in community discussion. The update is tied to the DMA&\#x27;s Article 5\(2\), which requires gatekeepers to offer users a choice about linking certain core platform services.

hackernews · JustSkyfall · Oct 23, 19:34 · [Discussion](https://news.ycombinator.com/item?id=50214218)

**Background**: The Digital Markets Act \(DMA\) is an EU regulation that took effect in March 2024, designed to ensure fair competition by regulating large digital &\#x27;gatekeeper&\#x27; platforms. Google, as a designated gatekeeper, must comply with rules like allowing users to choose whether to link its core services \(e.g., Search, YouTube, Chrome\). Previously, Google had stated that data from services like Google Photos was not used for advertising purposes.

<details><summary>References</summary>
<ul>
<li><a href="https://digital-markets-act.ec.europa.eu/index_en">Digital Markets Act</a></li>
<li><a href="https://blog.internxt.com/google-activity-history/">How to Monitor Your Google Activity History | Internxt Blog</a></li>
<li><a href="https://www.google.ru/photos/about/?hl=e">Google Photos : Edit, Organize, Search, and Backup Your Photos</a></li>

</ul>
</details>

**Discussion**: Community comments clarify that the change is more nuanced than a blanket data grab, noting that ad use depends on users choosing to link services under DMA rules. Some users expressed skepticism, interpreting &\#x27;might&\#x27; as &\#x27;absolutely will,&\#x27; while others shared practical advice, such as turning off personalization or migrating to alternative services like Immich for photos.

**Tags**: `#privacy`, `#google`, `#advertising`, `#policy`, `#dma`

---