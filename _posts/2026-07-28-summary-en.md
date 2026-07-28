---
layout: default
title: "Horizon Summary: 2026-07-28 (EN)"
date: 2026-07-28
lang: en
---

> From 9 items, 8 important content pieces were selected

---

1. [vLLM v0.26.0 released with Inkling model support, DeepSeek-V4 optimizations, and accuracy improvements.](#item-1) ⭐️ 8.0/10
2. [Anthropic CEO advocates for mandatory safety testing of all capable AI models, including open-weights.](#item-2) ⭐️ 8.0/10
3. [Judge Rejects Google&\#x27;s DMCA Claims to Block Search Result Scraping](#item-3) ⭐️ 8.0/10
4. [Microsoft launches MAI-Cyber-1-Flash, its first AI cybersecurity model, integrated into the MDASH platform.](#item-4) ⭐️ 8.0/10
5. [Moonshot AI releases 2.8 trillion parameter Kimi K3 model weights with novel licensing terms.](#item-5) ⭐️ 8.0/10
6. [Case Study: Replacing React.js with HTMX for Server-Driven UI Interactivity](#item-6) ⭐️ 7.0/10
7. [Libsm64: A library that packages Super Mario 64&\#x27;s game logic for use in external engines.](#item-7) ⭐️ 7.0/10
8. [Analysis Highlights Shift in AI Guide from Chat Models to Agentic Systems](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0 released with Inkling model support, DeepSeek-V4 optimizations, and accuracy improvements.](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 introduces comprehensive support for the new Inkling multimodal MoE model family and delivers major performance optimizations for DeepSeek-V4 across NVIDIA, AMD, and Intel hardware. It also adds a new \`head\_dtype\` feature for fp32 \`lm\_head\` to improve generation accuracy and matures its KV offloading and tiered storage system. This release significantly expands vLLM&\#x27;s model ecosystem with a state-of-the-art multimodal model and pushes the performance envelope for a leading open-source model \(DeepSeek-V4\), directly benefiting developers and enterprises running high-throughput inference. The broad hardware optimizations and accuracy improvements solidify vLLM&\#x27;s position as a versatile and high-performance inference engine for production deployments. The Inkling support stack includes specialized features like piecewise CUDA graphs, Hopper FA4 relative attention, and MTP=1 speculative decoding. Performance gains for DeepSeek-V4 come from a new routing kernel \(2.94% E2E TPOT improvement\), a \`fused\_topk\_bias\` kernel \(1.5–2x speedup\), and redundant repeat/copy removal \(1.8% E2E TPOT improvement\).

github · khluu · Jul 27, 01:06

**Background**: vLLM is a high-throughput and memory-efficient inference and serving engine for large language models \(LLMs\). The Inkling model family, developed by Thinking Machines, is a multimodal mixture-of-experts \(MoE\) model with 975 billion total parameters and 41 billion active parameters, capable of reasoning over text, image, and audio inputs. FlashAttention-4 \(FA4\) is an optimized attention implementation for NVIDIA&\#x27;s Hopper architecture, offering performance improvements over previous versions, especially for long-context tasks. MTP \(Multi-Token Prediction\) is a speculative decoding technique that allows a model to predict multiple future tokens in a single forward pass, thereby increasing inference throughput.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/inkling/">Inkling - Thinking Machines Lab</a></li>
<li><a href="https://modal.com/blog/reverse-engineer-flash-attention-4">We reverse-engineered Flash Attention 4</a></li>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM</a></li>

</ul>
</details>

**Tags**: `#LLM Inference`, `#Performance Optimization`, `#vLLM`, `#Model Serving`, `#Hardware Acceleration`

---

<a id="item-2"></a>
## [Anthropic CEO advocates for mandatory safety testing of all capable AI models, including open-weights.](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic&\#x27;s CEO Dario Amodei outlined the company&\#x27;s position, advocating for mandatory safety testing for all sufficiently capable AI models, including open-weights models, while explicitly opposing outright bans on them. The position also includes support for measures like banning chip sales to China to prevent misuse. This stance is significant as it directly shapes the ongoing global debate on AI regulation, balancing safety concerns with the benefits of open-source AI. It could influence policy decisions, impacting how both open and closed AI models are developed, deployed, and governed worldwide. The proposal calls for testing by an independent third-party auditor, with the potential for governments to block deployment if a model is deemed unsafe. A key caveat is the lack of specific details on who administers the tests, their cost, and the criteria for passing, which are central to community concerns about potential regulatory capture.

hackernews · surprisetalk · Jul 27, 22:03 · [Discussion](https://news.ycombinator.com/item?id=49076057)

**Background**: Open-weight AI models are those whose trained parameters \(weights\) are publicly available for download and use, enabling customization and local deployment. Mandatory safety testing refers to a regime where models, especially frontier AI, undergo evaluation by independent auditors for risks before deployment. Anthropic is a leading AI safety and research company.

<details><summary>References</summary>
<ul>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>
<li><a href="https://aisecurityandsafety.org/en/guides/ai-model-evaluation/">AI Model Evaluation: Safety Benchmarks, Red Teaming &amp; Testing ...</a></li>
<li><a href="https://www.politico.com/news/2026/06/10/anthropic-backs-mandatory-vetting-for-frontier-ai-models-00957632">Anthropic backs mandatory testing for frontier AI models</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely critical and skeptical. Key concerns include accusations of regulatory capture, where mandatory testing could be used as a de facto ban if costs are prohibitive or access is denied. Commenters also point out perceived hypocrisy in opposing model bans while supporting hardware \(chip\) bans, and question the sincerity of the safety arguments, viewing them as a tactic to stifle competition.

**Tags**: `#AI Policy`, `#Open Source AI`, `#AI Safety`, `#Industry Debate`

---

<a id="item-3"></a>
## [Judge Rejects Google&\#x27;s DMCA Claims to Block Search Result Scraping](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

A judge has rejected Google&\#x27;s attempt to use Digital Millennium Copyright Act \(DMCA\) claims to stop a third-party service, SerpAPI, from scraping its public search results. The ruling occurred in 2026 and directly challenges the use of copyright law to restrict access to publicly available data. This ruling sets a significant legal precedent, affirming that scraping publicly accessible data is generally lawful and cannot be easily blocked by copyright claims. It impacts companies that restrict API access while trying to control data flow, potentially preserving competition and innovation in data-dependent services. The case highlights the legal distinction in the U.S., where copyright protection requires a minimum degree of creativity, unlike the EU&\#x27;s database rights which can protect substantial investment. A key factor was Google&\#x27;s deprecation of its own search API, which created the market need that services like SerpAPI filled.

hackernews · cdrnsf · Jul 27, 18:15 · [Discussion](https://news.ycombinator.com/item?id=49073513)

**Background**: The Digital Millennium Copyright Act \(DMCA\) is a 1998 U.S. law designed to protect digital copyright holders from online piracy. Web scraping involves using automated tools to extract data from websites, and its legality often hinges on whether the data is publicly accessible and the method of access. In the U.S., court rulings like hiQ Labs v. LinkedIn have established that scraping publicly available data is generally legal.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scrapingbee.com/blog/is-web-scraping-legal/">Is Web Scraping Legal? Key Insights and Guidelines You Need to Know | ScrapingBee</a></li>
<li><a href="https://cloro.dev/blog/website-scraping-legal/">Is Website Scraping Legal? 2026 Rules (US + EU) | cloro</a></li>
<li><a href="https://dmcaforce.com/what-are-dmca-claims-and-copyright-violations/">What are DMCA Claims and Copyright Violations? - DMCA Force</a></li>

</ul>
</details>

**Discussion**: Community sentiment largely criticizes Google&\#x27;s stance as hypocritical, given its own origins in web crawling. Key viewpoints include frustration over Google deprecating its official search API, which forces reliance on third-party scrapers, and observations on the legal differences between U.S. copyright and EU database rights. Some also highlight the public benefit of scraping in exposing advertising scams.

**Tags**: `#legal`, `#web-scraping`, `#copyright`, `#google`, `#api`

---

<a id="item-4"></a>
## [Microsoft launches MAI-Cyber-1-Flash, its first AI cybersecurity model, integrated into the MDASH platform.](https://microsoft.ai/news/introducing-mai-cyber-1-flash-inside-mdash/) ⭐️ 8.0/10

Microsoft introduced MAI-Cyber-1-Flash, its first AI model specifically designed for cybersecurity, and integrated it into its MDASH \(Multi-model Agentic Security Harness\) platform. The model was developed with a security-first approach and rigorously evaluated by Microsoft&\#x27;s AI Red Team. This represents a significant step in applying large language models to automate and enhance cybersecurity defense, potentially halving security model costs while improving detection accuracy for enterprises. It signals a major industry shift where AI agents could become integral to large-scale vulnerability discovery and remediation. The model is integrated with MDASH, a platform designed for automated, large-scale code auditing and vulnerability research across Microsoft software environments. Microsoft claims the model demonstrates how AI can achieve cost efficiency while boosting detection capabilities, a crucial factor given the increasing sophistication of software vulnerabilities.

hackernews · migmartri · Jul 27, 16:52 · [Discussion](https://news.ycombinator.com/item?id=49072361)

**Background**: MDASH, or Multi-model Agentic Scanning Harness, is Microsoft&\#x27;s AI-driven platform announced in mid-2026 for automating vulnerability discovery at scale. It functions as an &\#x27;agentic&\#x27; system, meaning it can deploy teams of AI agents to perform tasks like code auditing. The broader trend involves using large language models \(LLMs\) to process and analyze the vast amounts of data generated by security systems to identify threats and vulnerabilities more efficiently.

<details><summary>References</summary>
<ul>
<li><a href="https://microsoft.ai/news/introducing-mai-cyber-1-flash-inside-mdash/">Introducing MAI - Cyber - 1 - Flash inside MDASH | Microsoft AI</a></li>
<li><a href="https://runtimewire.com/article/microsoft-mai-cyber-1-flash-mdash-launch">Microsoft launches MAI - Cyber - 1 - Flash , a cost‑efficient AI security...</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/05/12/defense-at-ai-speed-microsofts-new-multi-model-agentic-security-system-tops-leading-industry-benchmark/">Defense at AI speed: Microsoft’s new multi-model agentic security system tops leading industry benchmark | Microsoft Security Blog</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed, with skepticism about practical access and Microsoft&\#x27;s execution track record. One comment questions if the model&\#x27;s advantage stems primarily from Microsoft&\#x27;s internal data on its own product vulnerabilities. Others express frustration over unclear access paths and reference past product naming inconsistencies as reasons for caution.

**Tags**: `#AI`, `#Cybersecurity`, `#Microsoft`, `#Large-Language-Models`

---

<a id="item-5"></a>
## [Moonshot AI releases 2.8 trillion parameter Kimi K3 model weights with novel licensing terms.](https://simonwillison.net/2026/Jul/27/kimi-k3/#atom-everything) ⭐️ 8.0/10

Moonshot AI has released the weights for its 2.8 trillion parameter Kimi K3 large language model on Hugging Face, with the model file size being a massive 1.56TB. The release is accompanied by a custom license that requires large &\#x27;Model as a Service&\#x27; businesses to enter a separate agreement with Moonshot AI. This release is significant as it makes one of the world&\#x27;s largest language models available for research and commercial use, potentially accelerating innovation. The novel &\#x27;open weight&\#x27; licensing approach sets a precedent for how AI companies might seek to monetize or control the commercial use of their most advanced models while still sharing the weights. The license is a modified MIT license that specifically targets large-scale commercial users, requiring a separate agreement for &\#x27;Model as a Service&\#x27; businesses with over $20 million in annual revenue. The model is already available for inference on platforms like OpenRouter, with pricing starting at $3 per million input tokens and $15 per million output tokens.

rss · Simon Willison · Jul 27, 23:39

**Background**: In machine learning, &\#x27;weights&\#x27; are the numerical parameters within a neural network that are learned during training and determine how the model processes information. Releasing model weights allows others to run the model without retraining, but it is distinct from &\#x27;open source,&\#x27; which typically includes the model&\#x27;s code and training data. Trillion-parameter models represent the cutting edge of AI scale, pushing the boundaries of what is computationally possible but requiring massive resources for training and inference.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-are-weights">What are Weights? - Stanford HAI</a></li>
<li><a href="https://developer.nvidia.com/blog/demystifying-ai-inference-deployments-for-trillion-parameter-large-language-models/">Demystifying AI Inference Deployments for Trillion Parameter Large ...</a></li>
<li><a href="https://milvus.io/ai-quick-reference/how-does-the-mit-license-work">How does the MIT license work?</a></li>

</ul>
</details>

**Tags**: `#llm`, `#open-source`, `#model-weights`, `#ai-ethics`, `#huggingface`

---

<a id="item-6"></a>
## [Case Study: Replacing React.js with HTMX for Server-Driven UI Interactivity](https://misago-project.org/t/removing-reactjs-from-the-codebase-and-adapting-htmx-for-ui-interactivity/1267/) ⭐️ 7.0/10

A project detailed the removal of the React.js client-side framework from its codebase and its replacement with HTMX to handle UI interactivity directly from the server. This migration represents a shift from a heavy JavaScript Single-Page Application \(SPA\) architecture to a server-centric, hypermedia-driven approach. This case study is significant as it highlights a growing trend of reconsidering complex frontend frameworks for simpler, server-rendered architectures, which can reduce client-side complexity, improve initial load performance, and simplify development for content-centric applications. It provides a real-world blueprint for developers evaluating similar architectural shifts, especially for applications like forums where dynamic updates are needed but full SPA complexity is unnecessary. The discussion highlights that HTMX is particularly well-suited for forum software, where content is largely static HTML, and interactivity like live updates can be achieved via server-sent events. However, a community comment notes a performance caveat where sending large HTML fragments \(e.g., complex forms with select lists\) in a single response can lead to a slow user experience.

hackernews · Ralfp · Jul 27, 09:58 · [Discussion](https://news.ycombinator.com/item?id=49067301)

**Background**: HTMX is a client-side JavaScript library that allows developers to access modern browser features like AJAX, CSS Transitions, and WebSockets directly from HTML attributes, enabling dynamic updates without writing much JavaScript. It promotes a hypermedia-driven architecture where the server responds with HTML fragments that replace parts of the page. This contrasts with frameworks like React.js, which typically manage the entire UI state and rendering logic on the client side, requiring more JavaScript and often a separate API backend.

<details><summary>References</summary>
<ul>
<li><a href="https://htmx.org/docs/">htmx ~ Documentation</a></li>
<li><a href="https://mvolkmann.github.io/blog/htmx/">htmx | Mark Volkmann&#x27;s Tech Blog</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive towards HTMX, with users praising its fit for server-rendered apps, forums, and even PWAs, often paired with utility-first CSS frameworks like Tailwind. Some share practical experiences, such as performance issues with large HTML payloads, while others suggest it for most use cases, reserving mini React/Vue apps only for highly custom interactivity. Alternative server-driven UI approaches, like those inspired by Phoenix LiveView, were also mentioned.

**Tags**: `#web-development`, `#htmx`, `#react`, `#architecture`, `#frontend`

---

<a id="item-7"></a>
## [Libsm64: A library that packages Super Mario 64&\#x27;s game logic for use in external engines.](https://github.com/libsm64/libsm64) ⭐️ 7.0/10

The libsm64 project has released a shared library that extracts the core game logic, physics, and rendering of Super Mario 64, allowing developers to import and control the Mario character within external game engines like Unity or Unreal. It requires users to provide an official Super Mario 64 ROM at runtime for texture and animation data. This represents a novel and creative approach to game character portability, enabling a beloved, complex game character to be used in entirely new contexts and fan projects. It demonstrates a practical, hype-free method for achieving character interoperability across engines, a concept often associated with &\#x27;metaverse&\#x27; or blockchain promises. The library is built upon the community-driven Super Mario 64 decompilation project and is designed to be integrated into other applications via a C API. A key limitation is that it does not distribute Nintendo&\#x27;s copyrighted assets; users must supply their own legally obtained ROM, which the library uses to extract necessary data.

hackernews · klaussilveira · Jul 27, 10:04 · [Discussion](https://news.ycombinator.com/item?id=49067352)

**Background**: Super Mario 64 is a landmark 3D platformer released for the Nintendo 64 in 1996. In recent years, a community-driven reverse engineering and decompilation project has successfully recreated the game&\#x27;s source code from the original machine code, enabling deep understanding and modification. A decompilation project like this one allows the game&\#x27;s logic to be separated from its original engine and assets, which is the foundation for tools like libsm64.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/libsm64/libsm64">GitHub - libsm64/libsm64: Mario 64 as a library for use in ...</a></li>
<li><a href="https://github.com/n64decomp/sm64">GitHub - n64decomp/sm64: A Super Mario 64 decompilation ...</a></li>
<li><a href="https://deepwiki.com/libsm64/libsm64/4.2-integration-guidelines">Integration Guidelines | libsm64/libsm64 | DeepWiki</a></li>

</ul>
</details>

**Discussion**: The community reaction is highly positive and excited, praising the library&\#x27;s creative premise and sharing demo videos of Mario in games like Half-Life 2. Commenters note it fulfills the promise of cross-game character portability without the associated hype of &\#x27;metaverse&\#x27; or crypto projects. Others humorously warn Nintendo about potential commercial misuse, while some ask about ease of setup and point to a curated list of projects using the library.

**Tags**: `#game-development`, `#reverse-engineering`, `#library`, `#emulation`, `#creative-coding`

---

<a id="item-8"></a>
## [Analysis Highlights Shift in AI Guide from Chat Models to Agentic Systems](https://simonwillison.net/2026/Jul/27/an-opinionated-guide-to-which-ai-to-use-to-do-stuff/#atom-everything) ⭐️ 7.0/10

Simon Willison analyzed the latest update to Ethan Mollick&\#x27;s &\#x27;opinionated guide&\#x27; for using AI, noting a significant evolution from a focus on chat models like ChatGPT and Claude a year ago to a current emphasis on agentic systems such as ChatGPT Work and Claude Cowork. The guide now highlights AI systems capable of performing substantial autonomous work, while Google&\#x27;s Gemini has been removed from the primary recommendations due to its lack of a proven agentic offering. This shift reflects a broader industry trend where the value of AI is moving beyond simple conversation to autonomous task execution, which could significantly enhance productivity across various professional fields. For users and developers, understanding which platforms are leading in agentic capabilities is crucial for selecting tools that can automate complex, multi-step workflows. The guide clarifies the confusing naming conventions for agent modes: &\#x27;ChatGPT Work&\#x27; and &\#x27;Codex&\#x27; for OpenAI, and &\#x27;Cowork&\#x27; and &\#x27;Code&\#x27; for Anthropic&\#x27;s Claude, which offer more capabilities when granted computer access. A notable technical detail is that switching ChatGPT mobile to &\#x27;Work&\#x27; mode removes internet access restrictions for its Code Interpreter, a feature distinction that is not intuitively obvious compared to the desktop app.

rss · Simon Willison · Jul 27, 21:55

**Background**: Agentic AI refers to artificial intelligence systems that can accomplish specific goals with limited supervision, operating semi- or fully autonomously to perceive, reason, and act. Models like Claude 4 Opus represent advanced iterations with features tailored for agentic tasks, such as long context windows and adaptive thinking. In contrast, traditional chat models are primarily designed for interactive conversation, while agentic systems like Google&\#x27;s newly launched Gemini Spark aim to work autonomously in the background on user-assigned tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained | MIT Sloan</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-8">Introducing Claude Opus 4.8 \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI Agents`, `#LLM Guide`, `#AI Tools`, `#Productivity`

---