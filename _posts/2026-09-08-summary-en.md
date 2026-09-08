---
layout: default
title: "Horizon Summary: 2026-09-08 (EN)"
date: 2026-09-08
lang: en
---

> From 10 items, 2 important content pieces were selected

---

1. [Abusive web crawlers consume more CPU than all legitimate traffic on Linux kernel&\#x27;s git server.](#item-1) ⭐️ 8.0/10
2. [Caltech hosts world&\#x27;s first research-level mathematics hackathon.](#item-2) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Abusive web crawlers consume more CPU than all legitimate traffic on Linux kernel&\#x27;s git server.](https://simonwillison.net/2026/Sep/7/creepy-crawlies/) ⭐️ 8.0/10

Konstantin Ryabitsev, from the kernel.org infrastructure team, revealed that the official Linux kernel Git repository \(git.kernel.org\) spends more CPU cycles rendering Git commits into HTML for abusive web scrapers than it does for all other legitimate access combined, including Git clones. At any given time, across five geo-distributed nodes, 14 CPU cores are dedicated solely to this task. This highlights a severe and growing infrastructure burden on critical open-source projects, where resources meant for developers are being diverted to serve automated, often malicious, data harvesting. The issue reflects a broader trend of escalating &\#x27;background radiation&\#x27; from abusive crawlers, which threatens the performance, cost, and sustainability of public-facing web services, especially those with valuable data like code repositories. The analysis specifically focuses on the CPU cost of dynamically rendering commit history as web pages, a feature that is heavily exploited by scrapers. The problem is not just about bandwidth but about intensive server-side processing, and it persists despite the servers being geo-distributed for resilience and performance.

rss · Simon Willison · Sep 7, 23:08

**Background**: git.kernel.org is the primary, official Git repository hosting the source code for the Linux kernel, a critical piece of global software infrastructure. Web crawlers \(or bots\) are automated programs that browse the web to index or scrape data; while some are legitimate \(like search engine bots\), others are abusive, aggressively harvesting content without permission, often for spam, data mining, or training AI models. Rendering Git commits as HTML allows users to view commit details in a browser, but this dynamic page generation is computationally expensive compared to serving static files or handling Git protocol traffic.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kernel.org">kernel.org - Wikipedia</a></li>
<li><a href="https://fingerprint.com/blog/web-crawler-detection/">How to Detect and Block Malicious Web Crawlers in 2025</a></li>
<li><a href="https://www.amicited.com/blog/ai-crawler-impact-server-resources/">AI Crawler Impact on Server Resources: What to Expect | Am I Cited</a></li>

</ul>
</details>

**Tags**: `#web-crawling`, `#infrastructure`, `#linux-kernel`, `#performance`, `#security`

---

<a id="item-2"></a>
## [Caltech hosts world&\#x27;s first research-level mathematics hackathon.](https://mathathonchallenge.com/index.html) ⭐️ 7.0/10

Caltech, in partnership with Anthropic and OpenAI, announced the Mathathon, the world&\#x27;s first hackathon dedicated to research-level mathematics. The 40-hour event, scheduled for October 30 to November 1, 2026, will involve around 100 selected teams solving an open math problem using AI. This event represents a significant step in democratizing access to cutting-edge mathematical research by leveraging AI and large-scale compute resources. It signals a growing trend of using competitive, collaborative formats to tackle fundamental research questions, potentially accelerating discoveries at the intersection of AI and mathematics. The hackathon is organized by Caltech undergraduates, is not officially affiliated with Caltech departments, and all funding goes towards judges and participants. A key stated goal is to promote responsible AI use, and the event is sponsored by numerous organizations including DARPA expMath, Cognition, and a16z.

hackernews · astroanax · Sep 7, 09:26 · [Discussion](https://news.ycombinator.com/item?id=49596055)

**Background**: A hackathon is typically a time-bound, collaborative event where participants intensively work on software or technology projects. Research-level mathematics involves tackling unsolved problems or making novel contributions to mathematical knowledge, a domain traditionally dominated by academic institutions and research labs. The integration of AI, particularly large language models \(LLMs\), into mathematical problem-solving is an emerging and rapidly evolving field.

<details><summary>References</summary>
<ul>
<li><a href="https://agihunt.info/en/e/1a06e401b02e2c5c041ef20ab7f">Caltech Hosts World&#x27;s First AI Math Hackathon… · AGI Hunt</a></li>
<li><a href="https://undercodetesting.com/caltech-anthropic-openai-host-worlds-first-research-level-math-hackathon-with-m-in-compute-and-ai-agents/">Caltech Anthropic OpenAI Host World&#x27;s First Research-Level Math ...</a></li>

</ul>
</details>

**Discussion**: The discussion includes an organizer clarifying the student-led, non-profit nature of the event and its goal of promoting responsible AI. A participant familiar with Caltech&\#x27;s context suggested the hackathon also serves as a way for students to gain AI recognition due to perceived weaknesses in the university&\#x27;s computer science department. Another commenter expressed skepticism about whether the hackathon format, with its intense short timespan, is suitable for LLM-based mathematical progress, which often involves long, sporadic computation runs.

**Tags**: `#hackathon`, `#mathematics`, `#artificial-intelligence`, `#research`, `#education`

---