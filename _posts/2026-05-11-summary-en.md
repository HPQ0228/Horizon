---
layout: default
title: "Horizon Summary: 2026-05-11 (EN)"
date: 2026-05-11
lang: en
---

> From 32 items, 23 important content pieces were selected

---

1. [EU Digital Identity Wallet Hardware Attestation Creates Monopoly Concerns](#item-1) ⭐️ 8.0/10
2. [Local AI Should Become the Standard](#item-2) ⭐️ 8.0/10
3. [AI工具如何削弱开发者的编程乐趣](#item-3) ⭐️ 8.0/10
4. [Fictional CVE Report Sparks Real Supply Chain Security Discussion](#item-4) ⭐️ 7.0/10
5. [Louis Rossmann Offers to Pay Legal Fees for OrcaSlicer Developer](#item-5) ⭐️ 7.0/10
6. [Allen Downey Releases Free Jupyter-Based Linear Algebra Textbook](#item-6) ⭐️ 7.0/10
7. [NYT Editor's Note Reveals AI-Generated False Quotation](#item-7) ⭐️ 7.0/10
8. [Study: Mainstream AI Answers Often Biased Toward Japan and US](#item-8) ⭐️ 7.0/10
9. [xAI Grok Build Tool Leaked, Targets Claude Code Competition](#item-9) ⭐️ 7.0/10
10. [Developer Returns to AWS, Shares Frustrations That Spark HN Debate](#item-10) ⭐️ 6.0/10
11. [Space Cadet Pinball Recreated on Linux via Decompilation](#item-11) ⭐️ 6.0/10
12. [Baidu Releases Wenxin 5.1 LLM with Cost-Efficient Training](#item-12) ⭐️ 6.0/10
13. [EU Research Body Calls VPNs a Loophole in Age Verification](#item-13) ⭐️ 6.0/10
14. [NASA JPL Achieves Breakthrough in Mars Rotor Technology](#item-14) ⭐️ 6.0/10
15. [Report Exposes Chinese Grey Market Claude API Scam at 90% Discount](#item-15) ⭐️ 6.0/10
16. [FCC Proposes Phone Number Identity Verification Rule](#item-16) ⭐️ 6.0/10
17. [vLLM v0.20.2 Patch Release Fixes DeepSeek V4 and Qwen3-VL Bugs](#item-17) ⭐️ 5.0/10
18. [Andrew Quinn on Reinventing Wheels to Learn](#item-18) ⭐️ 5.0/10
19. [WebRTC Packet Dropping Conflicts with LLM Voice Accuracy Needs](#item-19) ⭐️ 5.0/10
20. [ChatGPT Android APK Teardown Reveals Codex Remote Desktop Feature](#item-20) ⭐️ 5.0/10
21. [Snapseed 4.0 Major Update Released After 2 Years](#item-21) ⭐️ 5.0/10
22. [Epic Says AI Used for Efficiency, Fortnite AI Use Centralized](#item-22) ⭐️ 5.0/10
23. [Chrome 148 Removes On-Device AI Privacy Statement](#item-23) ⭐️ 5.0/10

---

<a id="item-1"></a>
## [EU Digital Identity Wallet Hardware Attestation Creates Monopoly Concerns](https://grapheneos.social/@GrapheneOS/116550899908879585) ⭐️ 8.0/10

The EU Digital Identity Wallet (EUDI Wallet) requires hardware attestation from Google or Apple, effectively tying all EU digital identities to an American tech duopoly. This requirement has raised concerns about digital sovereignty and enabling tech monopolies. This matters because it creates dependency on US tech giants for European digital identity infrastructure, potentially undermining EU digital sovereignty. The requirement could lock users into Google or Apple approved mobile devices and create privacy risks through device fingerprinting. The system does not use zero-knowledge proofs or blind signatures, meaning each attestation leaves behind a packet that can be used to link actions to a specific device. This creates a persistent tracking mechanism despite claims of privacy protection.

hackernews · ChuckMcM · May 10, 17:54 · [Discussion](https://news.ycombinator.com/item?id=48086190)

**Background**: The EU Digital Identity Wallet is a mobile identity wallet defined in EU law to let people prove their identity online and share verified attributes across the EU. Hardware attestation uses security chips like TPM (Trusted Platform Module) to verify a device's integrity. Trusted Computing is a technology that enforces expected behavior through hardware and software, and has been controversial since it can restrict users' control over their own devices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/EU_Digital_Identity_Wallet">EU Digital Identity Wallet</a></li>
<li><a href="https://en.wikipedia.org/wiki/Trusted_Computing">Trusted Computing</a></li>
<li><a href="https://en.wikipedia.org/wiki/Trusted_Platform_Module">Trusted Platform Module - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted the historical context of Intel's 1999 CPU serial number controversy, which faced massive opposition and was reversed. They criticized the lack of privacy-preserving technology like zero-knowledge proofs, with one commenter calling it 'tyranny' that makes people powerless. Another noted this continues the trend of walled garden ecosystems that lock users into approved devices.

**Tags**: `#hardware-attestation`, `#digital-identity`, `#privacy`, `#monopoly`, `#trusted-computing`, `#eu-regulation`

---

<a id="item-2"></a>
## [Local AI Should Become the Standard](https://unix.foo/posts/local-ai-needs-to-be-norm/) ⭐️ 8.0/10

An opinion piece argues that local AI running on personal devices should become the standard, similar to how open source software eventually became mainstream. This represents a potential paradigm shift in AI deployment from centralized cloud services to distributed edge devices, impacting privacy, costs, and accessibility for developers and users alike. Community comments reveal a hardware progression timeline: from large data centers with performant LLMs, to server clusters with H100 GPUs, to consumer devices like MacBook Pro with 128GB VRAM or Strix Halo. The emerging pattern is 'expensive remote LLM for planning, local fast LLM for execution'.

hackernews · cylo · May 10, 17:19 · [Discussion](https://news.ycombinator.com/item?id=48085821)

**Background**: Local AI refers to running AI models on personal devices rather than sending data to cloud servers. Edge computing processes data near the source rather than in centralized data centers. This contrasts with cloud AI services like OpenAI's GPT-4 or Anthropic's Claude, which require sending user data to remote servers for processing.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Local_AI_vs_cloud_AI">Local AI vs. cloud AI</a></li>
<li><a href="https://www.nutanix.com/info/cloud-computing/edge-computing">Edge Computing Definition : Benefits and Use Cases | Nutanix</a></li>
<li><a href="https://jakubjirak.medium.com/local-ai-vs-cloud-ai-when-does-each-make-sense-2b374f9f5e48">Local AI vs Cloud AI : When Does Each Make Sense | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters discuss hardware trajectory from data centers to consumer devices, drawing parallels to open source adoption history. One commenter distinguishes private AI from local AI, suggesting self-hosted solutions with tenant isolation. Another emphasizes that local models need to be 'good enough' rather than competing with frontier models.

**Tags**: `#local-ai`, `#edge-computing`, `#ai-infrastructure`, `#privacy`, `#hardware-trends`

---

<a id="item-3"></a>
## [AI工具如何削弱开发者的编程乐趣](https://g5t.de/articles/20260510-task-paralysis-and-ai/index.html) ⭐️ 8.0/10

开发者们报告称，AI编码助手（如Claude Code）通过用提示工程和智能体管理取代深度技术工作，降低了他们对编程的兴趣和满足感。 这揭示了软件行业中一个日益严重的现象：AI工具在提高效率的同时，可能正在侵蚀技术工作的本质乐趣，并对开发者的心理健康和工作满意度产生负面影响。 开发者描述工作模式从「自底向上」（从理解到实现，拥有完整周期）转变为「自顶向下」（管理产生输出的智能体）。有ADHD的开发者特别容易对AI上瘾，快速耗尽每月使用限额。

hackernews · MrGilbert · May 10, 06:20 · [Discussion](https://news.ycombinator.com/item?id=48081469)

**Background**: Prompt engineering is the process of structuring natural language inputs to produce specified outputs from generative AI models. AI agents are tools that automate development workflows by leveraging the context of software development infrastructure. The discussion reflects broader concerns about how these technologies are changing the nature of software engineering work.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_engineering">Prompt engineering</a></li>
<li><a href="https://github.com/resources/articles/what-are-ai-agents">What are AI agents? · GitHub</a></li>

</ul>
</details>

**Discussion**: 开发者们表达了强烈的共鸣，分享了个人经历中工作满意度下降和对AI上瘾的担忧。许多人指出最初的生产力提升但长期乐趣丧失。值得注意的是，有ADHD的开发者特别担心自己容易对AI产生依赖。

**Tags**: `#AI tools`, `#software engineering`, `#developer experience`, `#task paralysis`, `#AI addiction`

---

<a id="item-4"></a>
## [Fictional CVE Report Sparks Real Supply Chain Security Discussion](https://nesbitt.io/2026/02/03/incident-report-cve-2024-yikes.html) ⭐️ 7.0/10

A satirical fictional incident report titled 'CVE-2024-YIKES' was published, depicting a supply-chain attack on Rust dependencies. Despite being entirely fictional, it generated substantial community engagement (372 points, 90 comments) and sparked valuable discussions about real security vulnerabilities in software ecosystems. This fictional report resonated because it humorously highlighted genuine concerns about supply chain security in the Rust ecosystem, build-time attacks, and risks from agentic development. It served as both entertainment and a wake-up call for developers to consider security implications in their dependency chains. The report mentioned specific crates like vulpine-lz4 (a transitive dependency of cargo), flate2, tar, curl-sys, and libgit2-sys that could be potential targets. It also referenced build.rs files as attack vectors since they execute during build time and wouldn't stand out. The fictional scenario included a YubiKey compromise via a fake official store.

hackernews · miniBill · May 10, 17:43 · [Discussion](https://news.ycombinator.com/item?id=48086082)

**Background**: Supply chain security is a critical concern in modern software development, where applications rely on thousands of external dependencies. Rust's cargo ecosystem, while known for its safety guarantees, still depends on numerous third-party crates. Build-time attacks (via files like build.rs) represent a particularly insidious attack vector since they execute code during the build process with elevated privileges.

**Discussion**: The community appreciated the piece for its entertainment value while recognizing its underlying security message. Commenters noted it had them genuinely worried during initial reading, demonstrating its effectiveness. Some users identified real attack vectors mentioned (like crates with build.rs files), while others joked about being 'attacked and seen' by references to fish shell and the YubiKey prank. Overall sentiment was positive, with appreciation for combining humor with security awareness.

**Tags**: `#supply-chain-security`, `#rust`, `#fiction`, `#devops`, `#cybersecurity`

---

<a id="item-5"></a>
## [Louis Rossmann Offers to Pay Legal Fees for OrcaSlicer Developer](https://www.tomshardware.com/3d-printing/louis-rossmann-tells-3d-printer-maker-bambu-lab-to-go-bleep-yourself-over-its-lawsuit-against-enthusiast-right-to-repair-advocate-offers-to-pay-the-legal-fees-for-a-threatened-orcaslicer-developer) ⭐️ 7.0/10

Louis Rossmann, a prominent repair YouTuber, has offered to pay the legal fees for an OrcaSlicer developer who received a legal threat from Bambu Lab, escalating the ongoing right-to-repair conflict in the 3D printing community. This incident highlights growing tensions between 3D printer manufacturers and the open-source community over software access and user rights, potentially setting a precedent for how companies can pursue legal action against hobbyists and developers. The dispute involves an OrcaSlicer fork that allegedly interacted with Bambu Lab's private cloud APIs to impersonate Bambu Studio. Community members note that while OrcaSlicer already supports Bambu printers, this specific fork crossed into unauthorized cloud API access, though many still criticize Bambu's legal threats as excessive.

hackernews · iancmceachern · May 10, 14:47 · [Discussion](https://news.ycombinator.com/item?id=48084432)

**Background**: OrcaSlicer is an open-source 3D printing slicer software that generates G-code for various 3D printers including Bambu Lab devices. Bambu Lab has faced controversy over their cloud-dependent features and previous attempts to eliminate offline access. Louis Rossmann is a well-known YouTuber in the repair community who has been a vocal advocate for right-to-repair principles.

<details><summary>References</summary>
<ul>
<li><a href="https://www.orcaslicer.com/">OrcaSlicer — Official Website & Downloads (Orca Slicer)</a></li>
<li><a href="https://github.com/OrcaSlicer/OrcaSlicer">GitHub - OrcaSlicer/OrcaSlicer: G-code generator for 3D printers (Bambu, Prusa, Voron, VzBot, RatRig, Creality, etc.) · GitHub</a></li>
<li><a href="https://www.tomshardware.com/3d-printing/bambu-lab-lawsuit-update-its-not-over">Bambu Lab lawsuit update: It’s not over | Tom's Hardware</a></li>

</ul>
</details>

**Discussion**: The community discussion shows strong support for Louis Rossmann's offer to pay legal fees, with many users criticizing Bambu Lab's business practices. Some commenters note the distinction between direct printer connection and unauthorized cloud API access, while others express frustration that Bambu Lab is treating customers as if they're 'leasing' rather than owning their printers.

**Tags**: `#3d-printing`, `#right-to-repair`, `#open-source`, `#legal`, `#bambu-lab`, `#community`

---

<a id="item-6"></a>
## [Allen Downey Releases Free Jupyter-Based Linear Algebra Textbook](https://allendowney.github.io/ThinkLinearAlgebra/index.html) ⭐️ 7.0/10

Allen Downey released "Think Linear Algebra" in 2023, a free textbook that uses Jupyter notebooks to interleave linear algebra concepts with practical Python code examples. This textbook provides a hands-on approach to learning linear algebra, making it valuable for students and practitioners who want to apply mathematical concepts directly in Python. Its free availability and practical orientation fill a gap in open-source educational resources. The textbook is available for free online and can be run locally using Jupyter notebooks. It combines mathematical explanations with executable code, allowing readers to experiment with concepts directly.

hackernews · tamnd · May 10, 09:40 · [Discussion](https://news.ycombinator.com/item?id=48082396)

**Background**: Allen Downey is a computer science professor and author known for his "Think" series of free textbooks, which include Think Python, Think Stats, Think Bayes, and Think Complexity. His teaching approach emphasizes practical, code-based learning. The Jupyter notebook format has become increasingly popular for technical education because it allows readers to run and modify code inline with written explanations.

**Discussion**: The discussion shows genuine interest in the textbook. Commenters appreciate the practical approach and mention using other Downey books like Think Bayes. There's a suggestion to add PCA (Principal Component Analysis) and CCA (Canonical Correlation Analysis) topics. One commenter notes the unconventional ordering of topics (matrix multiplication before vector addition), which differs from some traditional linear algebra textbooks.

**Tags**: `#linear-algebra`, `#education`, `#python`, `#jupyter`, `#open-source`, `#textbook`

---

<a id="item-7"></a>
## [NYT Editor's Note Reveals AI-Generated False Quotation](https://simonwillison.net/2026/May/10/new-york-times-editors-note/#atom-everything) ⭐️ 7.0/10

The New York Times published an Editor's Note revealing that an AI-generated summary falsely attributed a quotation to Conservative leader Pierre Poilievre about Canadian politics, which the reporter should have verified. This incident highlights the critical risk of AI hallucination in journalism, demonstrating how AI tools can generate false quotations that appear credible, potentially undermining trust in major publications. The false quotation was an AI summary of Poilievre's views that the AI rendered as an actual quotation. The article has been corrected to accurately quote from a speech delivered by Poilievre in April, and he did not refer to politicians who changed allegiances as turncoats in that speech.

rss · Simon Willison · May 10, 23:58

**Background**: AI hallucination refers to when large language models generate false or fabricated information that appears plausible. Pierre Poilievre is the leader of the Conservative Party of Canada, a major federal political party. An Editor's Note is a formal correction or clarification issued by a publication to address errors in previously published content.

**Tags**: `#ai-ethics`, `#hallucinations`, `#journalism`, `#generative-ai`, `#fact-checking`

---

<a id="item-8"></a>
## [Study: Mainstream AI Answers Often Biased Toward Japan and US](https://cybernews.com/ai-news/every-ai-answer-japan/) ⭐️ 7.0/10

Researchers from the University of the Basque Country and Cardiff University studied 8 major LLMs across 24 languages answering 31,680 cultural questions, finding they often anchor answers to Japan or the US; 5 models favor Japan while 2 favor the US. This finding reveals a systematic cultural bias in AI systems that could affect billions of users worldwide, raising concerns about fairness and representation in global AI deployment. The discovery that bias forms during supervised fine-tuning provides a clear target for mitigation efforts. The study found that this cultural distribution bias primarily forms during the supervised fine-tuning (SFT) stage, while base models are relatively more balanced. Additionally, low-resource languages are more likely to output answers pointing to their own country.

telegram · zaihuapd · May 9, 10:02

**Background**: Supervised Fine-Tuning (SFT) is a common method for training large language models using labeled input-output pairs to align models with specific tasks or preferences. Low-resource languages refer to languages lacking large monolingual or parallel corpora for building NLP applications. Foundation models are large pre-trained models that can be adapted to various downstream tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.csdn.net/m0_59614665/article/details/142106952">大模型 微 调 ：SFT（ Supervised Fine - Tuning ）主要方式、SFT...</a></li>
<li><a href="https://medium.com/neuralspace/low-resource-language-what-does-it-mean-d067ec85dea5">Low-resource language: what does it mean? | by Felix Laumann, PhD | NeuralSpace | Medium</a></li>

</ul>
</details>

**Tags**: `#AI偏见`, `#大语言模型`, `#文化研究`, `#人工智能伦理`, `#监督微调`

---

<a id="item-9"></a>
## [xAI Grok Build Tool Leaked, Targets Claude Code Competition](https://tech.ifeng.com/c/8t0yrbeeuwt) ⭐️ 7.0/10

xAI's Grok Build coding tool has leaked, revealing it as a cross-platform Agent workflow application that can autonomously execute multi-step development tasks. It comes with Grok 4.3 Early Access by default, supports local file and Git permissions, and integrates MCP protocol, official skills and plugins. This represents xAI's direct entry into the AI coding assistant market, directly competing with Anthropic's Claude Code. The leaked parameter sizes (6-10 trillion) for upcoming models represent potentially major scaling if accurate, marking a significant development in the AI landscape. The leaked page shows xAI is training multiple large-scale models including 1 trillion, 1.5 trillion, 6 trillion, and 10 trillion parameter versions, plus an image/video model Imagine V2. To compete with Claude Code's Opus level requires at least 6 trillion parameters. The tool supports MCP (Model Context Protocol), an open standard introduced by Anthropic in November 2024.

telegram · zaihuapd · May 10, 13:34

**Background**: Claude Code is Anthropic's AI coding assistant, with their Opus model representing the top tier in coding capabilities. The Model Context Protocol (MCP) is an open-source standard for connecting AI applications to external systems like local files, databases, and tools. Large language models with trillions of parameters represent the cutting edge of AI scaling, though the computational and economic costs are substantial.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://udit.co/blog/xai-grok-5-6-trillion-parameters-model-scale-war">xAI's Grok 5: 6 Trillion Parameter Model Changes the AI Sca</a></li>

</ul>
</details>

**Tags**: `#xAI`, `#Grok`, `#AI coding assistant`, `#Claude Code`, `#large language models`, `#Musk`

---

<a id="item-10"></a>
## [Developer Returns to AWS, Shares Frustrations That Spark HN Debate](http://fourlightyears.blogspot.com/2026/05/i-returned-to-aws-and-was-reminded-hard.html) ⭐️ 6.0/10

A developer published a blog post about returning to AWS and recounting the reasons they originally left, sparking a Hacker News discussion with 471 comments about data transfer obstacles, AWS's treatment of open-source projects, and whether AWS is appropriate for simpler use cases. This discussion highlights persistent concerns about AWS vendor lock-in, data egress costs, and the company's approach to open-source projects—issues that continue to shape cloud computing decisions for developers and organizations. Key points include the Data Transfer Out (DTO) process requiring a month for initial response plus a multi-page questionnaire, and AWS's creation of open-source forks like OpenSearch, Valkey, and DocumentDB that sparked defensive licensing changes (SSPL, Elastic License, RSAL).

hackernews · andrewstuart · May 9, 08:37 · [Discussion](https://news.ycombinator.com/item?id=48073201)

**Background**: AWS (Amazon Web Services) is the largest cloud computing platform, offering over 200 services. The DTO (Data Transfer Out) process refers to the procedure for transferring data out of AWS to another provider. The open-source licensing debates stem from AWS creating managed services based on open-source projects (Elasticsearch→OpenSearch, Redis→Valkey, MongoDB→DocumentDB) without the original projects' consent, leading to source-available licenses designed to prevent such commercialization.

**Discussion**: The discussion revealed strong concerns about the DTO process taking up to a month with extensive questionnaires. Some commenters defended AWS, arguing it's not designed for simple CRUD apps with 100 users—comparable to using Blender for a simple task. Others noted that IAM complexity is inherent to robust security systems, not necessarily a flaw.

**Tags**: `#cloud-computing`, `#aws`, `#vendor-lock-in`, `#open-source`, `#devrel`

---

<a id="item-11"></a>
## [Space Cadet Pinball Recreated on Linux via Decompilation](https://brennan.io/2026/05/09/pinball-and-escrow/) ⭐️ 6.0/10

A developer successfully recreated Space Cadet Pinball on Linux by decompiling the original Windows exe files without access to the source code. The recreation is so accurate that it looks and feels identical to the original game. This demonstrates the power of reverse engineering for game preservation and open-source porting. The original author David St. from Cinematronics commented that it's wonderful to see their old game kept alive, highlighting the emotional and cultural value of preserving classic software. The developer used decompilation to extract information from the exe files and rebuild the game logic from scratch, essentially working 'blind' without ever seeing the original source code. The project has been ported to multiple platforms including various consoles and even runs in a web browser.

hackernews · jandeboevrie · May 10, 11:22 · [Discussion](https://news.ycombinator.com/item?id=48082968)

**Background**: Space Cadet Pinball was originally bundled with Windows 95 and later versions as a hidden easter egg. It was part of Full Tilt! Pinball, a game developed by Cinematronics. Reverse engineering is a process where one attempts to understand how software works by analyzing its compiled binary code, often to enable porting to new platforms or preserve legacy software.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Reverse_engineering_of_software">Reverse engineering of software</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reverse_engineering">Reverse engineering - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The original author davidst expressed heartfelt appreciation, saying the recreation made his day and that he would share it with his co-founders. Community members praised the impressive accuracy achieved through decompilation, with one noting it was done 'basically completely blind.' Others discussed the game ports and the interesting history of Windows 95 bundled games.

**Tags**: `#reverse-engineering`, `#gaming`, `#nostalgia`, `#open-source`, `#linux`

---

<a id="item-12"></a>
## [Baidu Releases Wenxin 5.1 LLM with Cost-Efficient Training](https://mp.weixin.qq.com/s/_I9ziafHheXiJpA-QY2F7A) ⭐️ 6.0/10

Baidu released Wenxin 5.1 (ERNIE 5.1), claiming the top Chinese ranking on LMArena with 1223 points (4th globally), with Agent capabilities surpassing DeepSeek-V4-Pro and creative writing comparable to Gemini 3.1 Pro. This release demonstrates Baidu's push to compete in the global AI race with cost-efficient training, potentially disrupting the LLM development paradigm by achieving competitive performance at just 6% of typical pretraining costs. The model uses 'multi-dimensional elastic pretraining,' a distributed training paradigm developed by Baidu. It is now available on Baidu Qianfan Model Square and Yiyan official website for enterprise users and developers.

telegram · zaihuapd · May 9, 07:45

**Background**: LMArena (Chatbot Arena) is a popular benchmark for evaluating LLMs through human preference voting. DeepSeek-V4-Pro is a Mixture-of-Experts (MoE) model supporting 1M token context windows. The multi-dimensional elastic pretraining approach represents an innovation in distributed training methodology that significantly reduces computational costs.

<details><summary>References</summary>
<ul>
<li><a href="https://llm-stats.com/benchmarks/lmarena-text">LMArena Text Leaderboard Benchmark Leaderboard</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/ DeepSeek - V 4 - Pro · Hugging Face</a></li>
<li><a href="https://finance.biggo.com/news/6G5gDJ4BNl__-4_GzYrk">Baidu Launches Ernie 5.1 AI Model, Cutting Pretraining Costs by 94%; Kunlun Chip Pursues Dual A+H Share Listing — BigGo Finance</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Large Language Models`, `#Baidu`, `#ERNIE`, `#Chinese AI`

---

<a id="item-13"></a>
## [EU Research Body Calls VPNs a Loophole in Age Verification](https://cyberinsider.com/eu-calls-vpns-a-loophole-that-needs-closing-in-age-verification-push/) ⭐️ 6.0/10

The European Parliamentary Research Service (EPRS) published a report identifying VPNs as a regulatory "loophole" in online age verification, arguing they are being used to bypass adult content age checks and calling for legislative closure. This highlights a growing tension between child protection officials pushing for stricter VPN restrictions and privacy advocates defending anonymous internet access, with implications for millions of users across the EU. Following the UK's implementation of mandatory age verification, VPN downloads surged significantly. The EU's official age verification app was recently found to have security vulnerabilities, while France is currently piloting a "double-blind" verification system as a potential solution.

telegram · zaihuapd · May 9, 11:48

**Background**: Age verification laws have gained momentum across Europe, with the UK implementing the Online Safety Act requiring platforms to deploy strict age verification mechanisms. However, studies show these systems are easily bypassed - a survey by Internet Matters found 46% of British children using simple methods like fake mustaches to circumvent age checks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ithome.com/0/946/633.htm">调查称英国 年 龄 验 证 形同虚设，46...</a></li>
<li><a href="https://www.bbc.com/zhongwen/articles/c771zmyj7m1o/simp">Pornhub等色情网站面临 欧 盟 儿童 安 全 调查 - BBC News 中文</a></li>
<li><a href="https://i.jandan.net/p/122564">英 国 社交禁令形同虚设：青少 年 用假胡子轻松骗过 年 龄 验 证 - 煎蛋</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#EU-regulation`, `#VPN`, `#age-verification`, `#policy`

---

<a id="item-14"></a>
## [NASA JPL Achieves Breakthrough in Mars Rotor Technology](https://arstechnica.com/space/2026/05/engineers-at-nasas-jet-propulsion-lab-make-a-breakthrough-in-rotor-technology/) ⭐️ 6.0/10

NASA JPL engineers have achieved a breakthrough in rotor technology designed to give Mars aircraft higher efficiency and stable lift in thin atmospheres, supporting heavier and more capable next-generation vehicles beyond Ingenuity. This advancement expands the payload and mission capabilities of Mars aircraft, enabling them to fly farther and carry more equipment, paving the way for more complex aerial exploration missions on the Red Planet. The breakthrough specifically targets next-generation Mars aircraft that are heavier and have more advanced mission capabilities than the Ingenuity helicopter. The new rotor design addresses the challenges of Mars' thin atmosphere, where atmospheric density is only about 1% of Earth's.

telegram · zaihuapd · May 9, 14:21

**Background**: Ingenuity, the first aircraft to achieve powered flight on another planet, demonstrated the feasibility of aerial exploration on Mars. However, its design was limited by the extremely thin Martian atmosphere, which makes generating lift challenging. This breakthrough aims to overcome these atmospheric limitations to enable more capable future Mars aircraft.

**Tags**: `#NASA`, `#aerospace`, `#Mars exploration`, `#rotor technology`, `#planetary aviation`

---

<a id="item-15"></a>
## [Report Exposes Chinese Grey Market Claude API Scam at 90% Discount](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinese-grey-market-sells-claude-api-access-at-90-percent-off-through-proxy-networks-that-harvest-user-data) ⭐️ 6.0/10

A security report reveals Chinese 'proxy' services selling Claude API access at just 10% of official prices, using stolen credit cards, model substitution, and harvesting user prompts for data distillation. Developers using these services risk exposing their code and business secrets while receiving inferior AI responses. This threatens Anthropic's business model and raises broader concerns about AI security and data privacy in the developer community. The grey market services use stolen credit cards, bulk airdrop account registrations, and recruit workers from low-income countries for identity verification to bypass official审查. They commonly substitute cheaper domestic models for premium Claude Opus, and harvest user prompts and outputs for data distillation.

telegram · zaihuapd · May 10, 01:48

**Background**: API proxy services (中转站) act as intermediaries that route user requests through their own infrastructure. Model distillation is a technique where a smaller model is trained to mimic a larger, more capable model's behavior using data collected from the original model. The grey market exploits pricing differences and uses fraudulent methods to obtain API access at scale.

**Tags**: `#AI security`, `#API fraud`, `#data privacy`, `#Claude`, `#grey market`, `#model distillation`

---

<a id="item-16"></a>
## [FCC Proposes Phone Number Identity Verification Rule](https://reclaimthenet.org/the-fcc-wants-your-id-before-you-get-a-phone-number) ⭐️ 6.0/10

The US FCC has unanimously passed a proposal requiring telecom operators to verify user identity before activating phone services, potentially including government-issued IDs, legal name, address, and existing phone numbers, covering traditional carriers, mobile operators, and VoIP services. This proposal could significantly impact anonymous communication methods, particularly prepaid phones and SIM cards that can currently be purchased with cash. It represents a major expansion of KYC (Know Your Customer) requirements into the telecommunications sector, potentially affecting privacy for millions of users. The proposal aims to combat illegal harassment calls and considers requiring operators to retain identity records for at least 4 years after users disconnect from the network, as well as checking law enforcement watchlists. The specific details remain open for public comment.

telegram · zaihuapd · May 10, 04:12

**Background**: The FCC (Federal Communications Commission) is the US federal agency regulating communications. VoIP (Voice over Internet Protocol) is a technology that enables voice calls over the internet. KYC (Know Your Customer) is a mandatory process in financial services requiring businesses to verify customer identity, and this proposal would extend similar requirements to telecommunications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Voice_over_IP">Voice over IP - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Know_your_customer">Know your customer - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#FCC`, `#telecom-regulation`, `#privacy`, `#identity-verification`, `#KYC`, `#US-policy`

---

<a id="item-17"></a>
## [vLLM v0.20.2 Patch Release Fixes DeepSeek V4 and Qwen3-VL Bugs](https://github.com/vllm-project/vllm/releases/tag/v0.20.2) ⭐️ 5.0/10

vLLM released v0.20.2, a patch version fixing bugs in DeepSeek V4 sparse attention and KV cache, gpt-oss MXFP4 with torch.compile, and Qwen3-VL deepstack boundary check. This patch release is significant for users of DeepSeek V4, gpt-oss, and Qwen3-VL models, as it resolves critical issues that could cause model hangs, KV cache allocation failures, and quantization problems under torch.compile. The DeepSeek V4 fix re-enables the persistent topk path on Hopper GPUs and ensures the memset kernel runs at CUDA graph capture time, fixing MTP=1 hang. The gpt-oss MXFP4 fix plumbs hidden_dim_unpadded through the moe_forward fake op to enable MXFP4 quantization under torch.compile. The Qwen3-VL fix removes an invalid deepstack boundary check that could fail under heavy load.

github · khluu · May 10, 07:37

**Background**: vLLM is a popular high-performance LLM inference engine that supports various model architectures and optimization techniques. DeepSeek V4 is a 1T parameter AI model featuring hybrid attention (CSA + HCA) and sparse attention for efficient long-context inference. MXFP4 (Microscaling Floating Point 4) is a quantization format that enables efficient inference by using 4-bit floating point representations with per-group scaling. Qwen3-VL is Alibaba's multimodal large language model in the Qwen3 series.

<details><summary>References</summary>
<ul>
<li><a href="https://deepseek.ai/deepseek-v4">DeepSeek V 4 : 1T Parameter AI Model Guide | Independent DeepSeek ...</a></li>
<li><a href="https://docs.bswen.com/blog/2026-04-25-deepseek-v4-1m-context-hybrid-attention/">How DeepSeek V 4 Handles 1M Token Context with Hybrid Attention</a></li>
<li><a href="https://rocm.blogs.amd.com/software-tools-optimization/mxfp4-online-rotation/README.html">Advanced MXFP 4 Quantization : Combining... — ROCm Blogs</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM Inference`, `#DeepSeek V4`, `#Bug Fixes`, `#Qwen3-VL`

---

<a id="item-18"></a>
## [Andrew Quinn on Reinventing Wheels to Learn](https://simonwillison.net/2026/May/10/andrew-quinn/#atom-everything) ⭐️ 5.0/10

Andrew Quinn argues that reinventing 4-5 wheels in most domains (20-30 in rigorous fields like CS) is necessary to understand wheel-making, countering the guilt of not knowing if better tools already exist. This perspective challenges the common feeling of guilt programmers have about not knowing existing tools, suggesting that building things from scratch is a valuable learning approach rather than wasted effort. Quinn emphasizes that reinventing wheels should be limited - not zero (avoiding learning) and not a thousand (becoming a wheel collector), but a targeted number that pushes you to the frontier of knowledge.

rss · Simon Willison · May 10, 14:59

**Background**: The 'reinventing the wheel' debate is a long-standing discussion in programming circles. While the conventional wisdom warns against duplicating existing solutions, an alternative view holds that building things from first principles provides deeper understanding. The quote comes from a footnote in Andrew Quinn's post about replacing a 3 GB SQLite database with a 7 MB FST (finite state transducer) binary, where he reflects on his learning journey.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Finite-state_transducer">Finite - state transducer - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/nlp/finite-state-transducer-fsts-in-nlp/">Finite State Transducer (FSTs) in NLP - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: 这一哲学反思在程序员中引发了深思熟虑的讨论。许多人同意 Quinn 的观点，指出动手实现往往能揭示被动学习无法获得的见解。有些人认为，轮子的具体数量并不那么重要，重要的是意图——为了理解而进行的刻意练习与盲目重新创造是不同的。

**Tags**: `#programming philosophy`, `#learning`, `#tool-building`, `#software engineering`, `#personal development`

---

<a id="item-19"></a>
## [WebRTC Packet Dropping Conflicts with LLM Voice Accuracy Needs](https://simonwillison.net/2026/May/9/luke-curley/#atom-everything) ⭐️ 5.0/10

Luke Curley highlights that WebRTC's aggressive packet-dropping design, optimized for real-time conference calls, creates problems for LLM voice applications where users would prefer waiting for accurate prompts rather than receiving degraded audio. This matters because it reveals a fundamental infrastructure mismatch: the protocol powering most real-time voice communication was not designed for LLM inference where accuracy trumps speed. As voice AI applications grow, developers face a choice between using WebRTC's native low-latency capabilities or building custom solutions that prioritize response quality. WebRTC prioritizes low latency by aggressively dropping packets during poor network conditions. Curley notes that even attempting to retransmit a WebRTC audio packet within a browser is impossible - the implementation is hard-coded for real-time latency. Discord tried to work around this but found the design fundamentally restrictive.

rss · Simon Willison · May 9, 01:03

**Background**: WebRTC is a real-time communication protocol built into browsers that handles audio/video transmission. It uses UDP-based RTP/RTCP protocols and includes NACK (Negative Acknowledgement) mechanisms for requesting packet retransmission. However, the browser implementation prioritizes low latency over reliability, making it unsuitable for applications where accuracy is more important than speed.

<details><summary>References</summary>
<ul>
<li><a href="https://bloggeek.me/webrtcglossary/nack/">NACK in WebRTC : What It Is & How Packet Retransmission Works</a></li>
<li><a href="https://webrtcforthecurious.com/docs/09-debugging/">Debugging | WebRTC for the Curious</a></li>

</ul>
</details>

**Tags**: `#WebRTC`, `#LLM-inference`, `#real-time-audio`, `#voice-AI`, `#systems-design`

---

<a id="item-20"></a>
## [ChatGPT Android APK Teardown Reveals Codex Remote Desktop Feature](https://www.androidauthority.com/codex-smartphone-control-3665256/) ⭐️ 5.0/10

APK teardown of ChatGPT Android v1.2026.125 revealed strings indicating OpenAI is developing Codex with mobile remote desktop control capabilities, allowing users to find and reconnect to remote sessions from their phones while requiring desktop login to the same account. This development suggests OpenAI is expanding Codex beyond a code generation tool into a comprehensive remote development environment, potentially allowing developers to control their desktop coding sessions from mobile devices. The feature is still in development with no official timeline or preview available. The discovered strings indicate capabilities for session reconnection and cross-device authentication through the same account.

telegram · zaihuapd · May 9, 02:18

**Background**: OpenAI Codex is a large language model developed by OpenAI specifically for translating natural-language prompts into source code. The recently introduced Codex-1 is a version of OpenAI o3 optimized for software engineering, and it has quickly become an industry standard tool for developers. APK teardowns are a common method used by developers and analysts to discover upcoming features by examining the code strings of mobile applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(language_model)">OpenAI Codex (language model) - Wikipedia</a></li>
<li><a href="https://openai.com/index/introducing-codex/">Introducing Codex | OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#ChatGPT`, `#Codex`, `#Android`, `#APK Teardown`, `#Mobile Development`

---

<a id="item-21"></a>
## [Snapseed 4.0 Major Update Released After 2 Years](https://play.google.com/store/apps/details?id=com.niksoftware.snapseed) ⭐️ 5.0/10

Snapseed has released version 4.0, a major update after 2 years, adding a built-in camera, redesigned UI, lossless and batch editing, smart masks, and new color tools including HSL, dehaze, lens flare, and glow effects. This update transforms Snapseed from a pure photo editor into a more complete mobile photography solution. The addition of camera functionality and batch editing addresses long-standing user requests, potentially attracting new users and retaining existing ones in the competitive mobile photo editing market. The version number jumped directly from 2.22 to 4.0, indicating significant architectural changes. HSL (Hue, Saturation, Lightness) allows precise color wheel adjustments, while the smart mask enables selective editing of specific image areas. Both iOS and Android versions were released simultaneously.

telegram · zaihuapd · May 9, 02:39

**Background**: Snapseed is a popular mobile photo editing app originally developed by Nik Software, which Google acquired in 2012. The app has been known for its powerful yet intuitive editing tools. The 4.0 update is the first major release in 2 years, marking a significant milestone in the app's development history.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HSL_and_HSV">HSL and HSV - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#mobile-apps`, `#photo-editing`, `#google`, `#software-update`, `#android`

---

<a id="item-22"></a>
## [Epic Says AI Used for Efficiency, Fortnite AI Use Centralized](https://www.ithome.com/0/948/483.htm) ⭐️ 5.0/10

Epic has clarified that the company is continuously testing various AI tools, primarily to support game development, reduce time for certain tasks, and improve operational efficiency. The company states it will not use AI to replace existing positions, and senior development manager Stephanie Arnett mentioned that AI will be used for artistic creative work in the future. This matters because it addresses growing concerns about AI replacing jobs in the gaming industry. The statement comes after Epic laid off 1,000 employees in 2026, which has made external parties skeptical about the company's claim that AI won't threaten employment. Epic maintains centralized control over AI usage for Fortnite, with partners not permitted to independently enable AI tools. The company is exploring AI applications in artistic creative workflows while maintaining that AI will not replace existing positions.

telegram · zaihuapd · May 10, 09:07

**Background**: Epic Games is the developer of Fortnite, one of the world's most popular games with hundreds of millions of players. The gaming industry has been actively exploring AI tools for various purposes, including asset creation, code assistance, and creative processes. There has been widespread concern across industries about AI's potential impact on employment, making Epic's policy announcement particularly relevant.

**Tags**: `#AI`, `#game-development`, `#Epic`, `#employment-impact`, `#corporate-policy`

---

<a id="item-23"></a>
## [Chrome 148 Removes On-Device AI Privacy Statement](https://cybernews.com/ai-news/chrome-removes-ai-privacy-wording-google-says-data-still-stays-on-device/) ⭐️ 5.0/10

Chrome 148 removed a privacy statement from the On-device AI settings that previously claimed user data would not be sent to Google servers. Google states the actual data processing behavior remains unchanged. This matters because it affects user trust and transparency around how their data is handled with on-device AI features. While Google assures the processing hasn't changed, removing explicit privacy assurance could raise concerns about what users are being told about data handling. The change appeared in Chrome 148.0.7778.97, while version 147 still displays the old wording. Additionally, in certain website integrations using Chrome's Gemini Nano, websites can access model inputs and outputs, with each site handling data according to their own privacy policies.

telegram · zaihuapd · May 10, 12:01

**Background**: Chrome's On-device AI features utilize Gemini Nano, Google's smallest AI model, to process AI tasks locally on the user's device without sending data to external servers. This approach is designed to enhance privacy by keeping sensitive data on the device. The privacy statement in question was designed to reassure users that their data would not be uploaded to Google's servers when using these on-device features.

**Tags**: `#Chrome`, `#Google`, `#privacy`, `#AI`, `#Gemini Nano`

---