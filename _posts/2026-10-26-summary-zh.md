---
layout: default
title: "Horizon Summary: 2026-10-26 (ZH)"
date: 2026-10-26
lang: zh
---

> 从 7 条内容中筛选出 4 条重要资讯。

---

1. [俄勒冈州警方为一名警官的记录索要 250 万美元，为透明度设置新障碍。](#item-1) ⭐️ 8.0/10
2. [一个十年前训练的 CNN 在皮肤癌诊断上超越了前沿大语言模型。](#item-2) ⭐️ 7.0/10
3. [FOSDEM 2027 大会发出反对互联网审查的行动号召](#item-3) ⭐️ 7.0/10
4. [因学生普遍使用 AI，加州大学伯克利分校数学教授质疑家庭作业评分的意义。](#item-4) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [俄勒冈州警方为一名警官的记录索要 250 万美元，为透明度设置新障碍。](https://theintercept.com/2026/10/01/oregon-police-misconduct-public-records-cost-fee/) ⭐️ 8.0/10

俄勒冈州尤金市警察局回应一家当地新闻媒体的公共记录请求时声称，搜索和处理记录将需要超过 44,800 小时的员工时间，成本约为 250 万美元。这笔费用是针对一名警官行为的相关记录。 此案例证了一种日益增长的手段，即通过收取天价费用来有效阻止公众获取信息，这破坏了旨在确保政府问责的《信息自由法》的核心目的。这对新闻业、警察监督以及公众了解官员行为的知情权具有重大影响。 警方估计的 44,816 小时大约相当于一个人连续工作 21 年。虽然机构可以对处理复杂请求的实际成本收费，但批评者认为这一具体计算是荒谬且蓄意的阻挠，而非善意的估算。

hackernews · tdeck · 10月25日 18:04 · [社区讨论](https://news.ycombinator.com/item?id=50234232)

**背景**: 《信息自由法》（FOIA）是一项美国联邦法律，赋予公众请求获取联邦机构记录的权利。包括俄勒冈州在内的许多州，对州和地方机构也有类似的公共记录法。这些法律通常要求机构在规定时间内（例如 FOIA 通常是 20 个工作日）做出回应，并允许其对搜索、审查和复制记录收取合理费用，不过出于公共利益的请求可以申请费用减免。该流程旨在促进透明度，但可能因延迟、过度删节或高昂费用而受阻。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.epa.gov/foia/foia-request-process">The FOIA Request Process | US EPA</a></li>
<li><a href="https://www.consumerfinance.gov/foia-requests/">FOIA Requests | Consumer Financial Protection Bureau</a></li>
<li><a href="https://www.whitehouse.gov/omb/information-resources/freedom-of-information-act-foia/">Freedom of Information Act ( FOIA ) – OMB – The White House</a></li>

</ul>
</details>

**社区讨论**: 评论者对时间和成本估算的荒谬性表示愤慨，并将其与国防部 6.6 亿美元估算等其他极端案例进行比较。他们还分享了国际视角，指出英国的 FOIA 流程在 30 天内提供信息且不收费，并强调了德国类似的阻挠手段。其他人则分享了机构使用极端拖延而非高额费用来阻挠请求的个人经历。

**标签**: `#government-transparency`, `#public-records`, `#foia`, `#police-accountability`, `#journalism`

---

<a id="item-2"></a>
## [一个十年前训练的 CNN 在皮肤癌诊断上超越了前沿大语言模型。](https://lynchlab.net/llm-skin-cancer) ⭐️ 7.0/10

一项研究发现，一个基于十年前 Inception-v3 架构、针对皮肤病学图像进行微调的专用卷积神经网络模型，在皮肤癌诊断任务上显著优于前沿的大语言模型。该 CNN 在 ISIC 档案库的超过 68,000 张图像上进行了训练，并在一个包含 200 个病灶的独立测试集上进行了评估。 这一发现挑战了大型通用大语言模型在所有复杂任务上都更优越的假设，凸显了在医疗等关键领域中，专用、任务特定架构的持久价值。这表明，对于高风险应用，投资于定制化模型可能比依赖通用型 AI 产生更准确、更可靠的结果。 该 CNN 模型是从一个在普通照片上预训练的网络微调而来，测试病灶被严格排除在训练和验证数据之外，以防止数据泄露。这一比较强调，尽管大语言模型参数庞大、能力通用，但在特定、狭窄的领域，由专家优化过的更小、更旧的模型仍可能超越它们。

hackernews · sungam · 10月25日 17:15 · [社区讨论](https://news.ycombinator.com/item?id=50233779)

**背景**: 卷积神经网络是一类专门用于分析视觉图像的深度神经网络，多年来一直是医学影像分析的基石。微调是指拿一个预训练好的 CNN（通常在 ImageNet 等大型数据集上训练），再在一个更小的、特定领域的数据集（如医学图像）上进一步训练，以调整其学习到的特征。大语言模型是在海量文本语料上训练的通用模型，能执行广泛的语言任务，但它们应用于视觉任务时，通常需要通过一个独立的视觉编码器来处理图像输入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/1706.00712">Convolutional Neural Networks for Medical Image Analysis ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0925231221001314">Convolutional neural networks for medical image analysis ...</a></li>
<li><a href="https://www.linkedin.com/pulse/evolution-artificial-intelligence-from-narrow-general-enrico-vianello-szxvf">&quot;The Evolution of Artificial Intelligence: From Narrow to General ...&quot;</a></li>

</ul>
</details>

**社区讨论**: 社区情绪普遍认同研究的结论，许多人评论说专用模型胜过通用模型并不令人意外。一些用户指出，这挑战了过去关于大语言模型将彻底改变医学诊断的说法，而另一些用户则认为这种比较类似于计算器在算术上胜过 LLM，强调了为工作选择正确工具的重要性。

**标签**: `#machine-learning`, `#computer-vision`, `#llm-critique`, `#medical-ai`, `#model-evaluation`

---

<a id="item-3"></a>
## [FOSDEM 2027 大会发出反对互联网审查的行动号召](https://talkweb.eu/openweb/4558/) ⭐️ 7.0/10

一位演讲者公开发出了反对互联网审查的行动号召，并宣传即将在 FOSDEM 2027 大会上举行的一场演讲，该演讲的主题是构建一个开放、未经审查的网络。此次演讲旨在围绕这一目标凝聚技术社区的力量。 这凸显了技术社区内部在平台治理、平衡言论自由与内容审核、以及企业在控制数字基础设施方面的角色等问题上持续存在的争论。其重要性在于，它试图动员开发者和开源倡导者构建技术方案，以替代中心化、由企业控制的网络。 该演讲计划在 FOSDEM 2027 大会上举行，这是一个面向自由及开源软件开发者的重要非商业性、志愿者组织的会议。此次号召将问题定性为“拒绝接受被审查的互联网”，直接挑战了当前的内容审核实践和企业权力。

hackernews · Tomte · 10月25日 17:30 · [社区讨论](https://news.ycombinator.com/item?id=50233929)

**背景**: FOSDEM（自由及开源软件开发者欧洲会议）是一个专注于自由及开源软件的年度非商业会议，以其高质量的技术内容和缺乏商业推销而闻名。关于“互联网审查”的辩论通常集中在“内容审核”（管理在线社区所必需）与“审查”（压制言论）之间的紧张关系上，其治理模式从企业控制到像 ICANN 所使用的多利益相关方模式各不相同。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/FOSDEM">FOSDEM - Wikipedia</a></li>
<li><a href="https://www.icann.org/en/system/files/files/in-brief-multistakeholder-internet-governance-28oct25-en.pdf">In Brief: Multistakeholder Internet Governance - icann.org</a></li>

</ul>
</details>

**社区讨论**: 社区评论揭示了一场细致的辩论，质疑“未经审查的互联网”是否真的存在，以及基础设施提供商的力量。一些用户指出必要的“内容审核”与“审查”之间的界限模糊，而另一些人则指出，许多人现在接受符合其政治观点的审查。另有一条讨论称赞 FOSDEM 是一个独特、以技术为中心的会议。

**标签**: `#internet-freedom`, `#censorship`, `#open-web`, `#conference`, `#governance`

---

<a id="item-4"></a>
## [因学生普遍使用 AI，加州大学伯克利分校数学教授质疑家庭作业评分的意义。](https://www.dailycal.org/news/campus/academics/ai-use-leads-uc-berkeley-math-professor-to-see-no-point-in-grading-homework/article_bdf1eae2-c08b-491f-b9f1-81a7cea177de.html) ⭐️ 7.0/10

加州大学伯克利分校的菲尔兹奖得主、数学教授理查德·博赫兹公开质疑了为传统家庭作业评分的价值，理由是学生普遍且轻易地使用 AI 工具来完成作业。这一立场反映了生成式 AI 给高等教育带来的直接教学挑战。 这一事件凸显了学术诚信和教学法的一个关键转折点，迫使教育工作者在 AI 无处不在的环境中重新思考评估的目的与设计。它预示着传统家庭作业作为评分组成部分的地位可能发生改变，这可能会重塑各学科对学习和掌握的评估方式。 这位教授理查德·博赫兹是一位著名数学家，以证明“魔群月光猜想”而闻名。一个关键的社区观点指出了其中的讽刺性：像他这样的终身教授通常将评分工作委托给助教，这为关于家庭作业在学习中的实际作用的讨论增添了另一层维度。

hackernews · romanhn · 10月25日 16:28 · [社区讨论](https://news.ycombinator.com/item?id=50233304)

**背景**: 教学法是关于教学方法以及知识如何传授的研究。学术诚信指的是教育中的道德政策与原则，如诚实和责任，它们是可信评估的基础。传统家庭作业长期以来一直是用于练习和形成性评估的核心教学工具，但随着能够完成此类任务的 AI 工具的出现，其有效性正受到审视。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pedagogy">Pedagogy - Wikipedia</a></li>
<li><a href="https://www.macalester.edu/academic-programs/academicpolicies/academicintegrity/">Academic Integrity - Academic Programs and... - Macalester College</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了多种细致观点，包括对教授本人不亲自评分的讽刺性讨论、关于家庭作业的真实目的是为了学习还是评估的辩论，以及对 AI 消除了促使学生参与的关键“强制功能”的担忧。部分评论还建议更广泛地重新评估高等教育在技能培训与纯粹学术之间的角色。

**标签**: `#AI in Education`, `#Academic Integrity`, `#Pedagogy`, `#Higher Education`, `#Ethics`

---