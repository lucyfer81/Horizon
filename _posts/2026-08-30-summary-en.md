---
layout: default
title: "Horizon Summary: 2026-08-30 (EN)"
date: 2026-08-30
lang: en
---

> From 6 items, 3 important content pieces were selected

---

1. [Tencent Open-Sources Hy4 Preview, a 770B-Parameter MoE Model with Self-Improving Capabilities](#item-1) ⭐️ 8.0/10
2. [DHS uses obscure customs law to secretly obtain phone records from journalists and activists.](#item-2) ⭐️ 8.0/10
3. [Samsung Unveils Processing-in-Memory \(PIM\) Architecture at Hot Chips 2026](#item-3) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Tencent Open-Sources Hy4 Preview, a 770B-Parameter MoE Model with Self-Improving Capabilities](https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/) ⭐️ 8.0/10

Tencent has released and open-sourced the Hy4 preview, a new-generation Mixture-of-Experts \(MoE\) AI model. Notably, this model participated in its own development process through an automated optimization loop, proposing approaches, running experiments, and iterating on results. This release is significant because it pushes the frontier of open-source large language models with a massive 770B-parameter architecture and a 1M-token context length. More importantly, its demonstrated ability to engage in recursive self-improvement represents a key step towards more autonomous and efficient AI development methodologies. The Hy4 preview model has 770 billion total parameters, with 49 billion activated per token, and features a 1 million token context window. It has reportedly seen massive initial adoption on platforms like OpenRouter, processing trillions of tokens within days of release.

hackernews · shenli3514 · Aug 29, 19:33 · [Discussion](https://news.ycombinator.com/item?id=49492632)

**Background**: Mixture-of-Experts \(MoE\) is a neural network architecture designed to scale model capacity efficiently. It consists of many specialized sub-networks \(experts\), but for each input, only a small subset is activated, keeping computational costs manageable. An automated optimization loop refers to a system where an AI model can propose, test, and refine its own training strategies, data selection, or evaluation methods based on feedback, creating a cycle of self-improvement.

<details><summary>References</summary>
<ul>
<li><a href="https://hy.tencent.ai/research/hy4-preview?langVersion=en">Introducing Hy4 preview - hy.tencent.ai</a></li>
<li><a href="https://github.com/Tencent-Hunyuan/Hy4-preview">GitHub - Tencent-Hunyuan/Hy4-preview</a></li>
<li><a href="https://shattered.io/tencent-hy4-preview-770b-2026/">Tencent Hy4 Preview: 770B Params, 1M-Token AI Model</a></li>

</ul>
</details>

**Discussion**: Community discussion highlights the model&\#x27;s rapid traction on inference platforms and its competitive pricing. Some users were impressed with the performance of its predecessor, Hy3, noting it was competitive with leading models. Others critiqued the presentation of benchmark data in the release materials.

**Tags**: `#AI`, `#Machine Learning`, `#Open Source`, `#Tencent`, `#Model Development`

---

<a id="item-2"></a>
## [DHS uses obscure customs law to secretly obtain phone records from journalists and activists.](https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits) ⭐️ 8.0/10

The Department of Homeland Security \(DHS\) is using a legal summons under Section 1509 of Title 19 of the U.S. Code, a provision originally for customs examinations, to secretly obtain phone and communication records from journalists, non-profits, and unions. In several cases, DHS has withdrawn the summons when challenged in court, a tactic that avoids a judicial ruling on its legality. This practice represents a significant expansion of government surveillance authority, bypassing typical judicial oversight and potentially violating Fourth Amendment protections against unreasonable searches. It directly threatens press freedom, the work of advocacy groups, and the privacy of individuals, while setting a dangerous precedent for using obscure laws for broad investigative powers. A key detail is that compliance with a Section 1509 summons is not mandatory; DHS must go to court to enforce it if challenged. Reports indicate varying corporate responses, with T-Mobile complying and providing records in one case, while Google reportedly did not. The DHS&\#x27;s own Office of Inspector General has previously warned that using these summonses in cases unrelated to customs or immigration violates policy.

hackernews · firefax · Aug 29, 18:44 · [Discussion](https://news.ycombinator.com/item?id=49492219)

**Background**: Section 1509 of Title 19 is a U.S. law that grants Customs and Border Protection \(CBP, a component of DHS\) the authority to issue summonses to examine records and witnesses as part of its customs and revenue enforcement duties. Historically, its use was tied to investigations under Title 19 \(customs\) or Title 8 \(immigration\). The Department of Homeland Security \(DHS\) is a U.S. federal agency with broad responsibilities including border security, immigration enforcement, and counterterrorism, which grants it significant surveillance and investigative authorities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.law.cornell.edu/uscode/text/19/1509">19 U.S. Code § 1509 - Examination of books and witnesses | U.S. Code | US Law | LII / Legal Information Institute</a></li>
<li><a href="https://www.oig.dhs.gov/sites/default/files/assets/Mga/2017/oig-18-18-nov17.pdf">Management Alert - CBP&#x27;s Use of Examination and Summons Authority Under</a></li>

</ul>
</details>

**Discussion**: Commenters highlight the deliberate legal strategy of withdrawing summonses to avoid a ruling, placing blame on companies that comply without challenge, and noting differing responses from service providers like T-Mobile and Google. Some suggest practical solutions for journalists, such as using decentralized communication tools, while others critique the broader political climate enabling such surveillance.

**Tags**: `#surveillance`, `#government`, `#privacy`, `#legal`, `#journalism`

---

<a id="item-3"></a>
## [Samsung Unveils Processing-in-Memory \(PIM\) Architecture at Hot Chips 2026](https://chipsandcheese.com/p/hot-chips-2026-samsungs-processing) ⭐️ 7.0/10

At the Hot Chips 2026 conference, Samsung presented its Processing-in-Memory \(PIM\) technology, which integrates compute units within memory arrays to perform calculations directly where data resides. This specific implementation aims to tackle the data movement bottleneck prevalent in modern computing systems. This matters because data movement between processors and memory has become a primary performance and energy bottleneck, especially for data-intensive workloads like AI. Samsung&\#x27;s move signals a major industry player&\#x27;s commitment to exploring non-von Neumann architectures, which could lead to significant efficiency gains for future AI accelerators and high-performance computing. Samsung&\#x27;s approach is a form of Processing-Near-Memory \(PNM\), placing compute units adjacent to memory arrays rather than fully integrating them. A key challenge noted in community discussion is that the architecture requires precise data locality, making it less flexible for general-purpose computing but potentially well-suited for specific patterns like matrix operations in AI.

hackernews · ingve · Aug 29, 06:06 · [Discussion](https://news.ycombinator.com/item?id=49487341)

**Background**: Processing-in-Memory \(PIM\) is an emerging semiconductor architecture that moves computation into or near memory arrays to reduce the costly movement of data between separate memory and processor units. The traditional von Neumann architecture, where data is shuttled back and forth, creates a &\#x27;memory wall&\#x27; or bottleneck as processors outpace memory bandwidth. Hot Chips is a leading industry symposium where major vendors like Samsung, SK Hynix, and Alibaba have recently showcased PIM prototypes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/processing-in-memory-pim-architectures-next-frontier-epbof">Processing - in - Memory ( PIM ) Architectures : The Next Frontier in...</a></li>
<li><a href="https://events.safari.ethz.ch/micro-pim-tutorial/doku.php?id=start">start [MICRO 2023 Real-World PIM Tutorial]</a></li>
<li><a href="https://semiengineering.com/data-movement-is-the-energy-bottleneck-of-todays-socs/">Data Movement Is the Energy Bottleneck of Today’s SoCs</a></li>

</ul>
</details>

**Discussion**: The community discussion reveals a mix of cautious optimism and skepticism. Some experts point out the long-standing theoretical concept and its inherent constraints, noting it&\#x27;s best suited for specific domains like AI, gaming, and crypto. Others are unconvinced by this specific implementation for matrix multiplication, arguing data movement within the memory array itself remains a challenge. There is also a sentiment that many exotic accelerator designs are pitched annually but few achieve widespread adoption.

**Tags**: `#hardware`, `#computer-architecture`, `#ai-acceleration`, `#memory`, `#samsung`

---