---
layout: default
title: "Horizon Summary: 2026-05-15 (EN)"
date: 2026-05-15
lang: en
---

> From 38 items, 28 important content pieces were selected

---

1. [First Public macOS M5 Kernel Memory Corruption Exploit](#item-1) ⭐️ 9.0/10
2. [RTX 5090 eGPU with M4 MacBook Air: Gaming & LLM Benchmarks](#item-2) ⭐️ 8.0/10
3. [Bun Merges Major Rewrite from Zig to Rust](#item-3) ⭐️ 8.0/10
4. [Mullvad Exit IPs Enable User Fingerprinting](#item-4) ⭐️ 7.0/10
5. [Removing Toyota RAV4 Modem and GPS for Privacy](#item-5) ⭐️ 7.0/10
6. [DS4: Local DeepSeek 4 Runtime Released](#item-6) ⭐️ 7.0/10
7. [Nginx-Rift: 18-Year-Old Vulnerability Enables Remote Code Execution](#item-7) ⭐️ 7.0/10
8. [Codex Now Available in ChatGPT Mobile App](#item-8) ⭐️ 7.0/10
9. [arXiv Implements 1-Year Ban for Hallucinated References](#item-9) ⭐️ 7.0/10
10. [Ontario Auditors Find Doctors' AI Note Takers Make Basic Factual Errors](#item-10) ⭐️ 7.0/10
11. [MIT President Kornbluth on Funding and Talent Pipeline Crisis](#item-11) ⭐️ 7.0/10
12. [Anthropic Launches Claude for Small Business](#item-12) ⭐️ 7.0/10
13. [OpenAI Sued for Sharing User Data with Meta and Google](#item-13) ⭐️ 7.0/10
14. [HDD Firmware Hacking Technical Exploration](#item-14) ⭐️ 6.0/10
15. [US Approves NVIDIA H200 Sales to 10 Chinese Firms](#item-15) ⭐️ 6.0/10
16. [Obesity Rates Stabilize in Rich Nations, Rise in Low-Income Countries](#item-16) ⭐️ 6.0/10
17. [Huawei, JAC, Stellantis in Talks for Maserati EV Partnership](#item-17) ⭐️ 6.0/10
18. [DeepSeek Chat Session Isolation Vulnerability Leaks User Conversations](#item-18) ⭐️ 6.0/10
19. [Technology Lock-in Decreases as Cross-Platform Tools Improve](#item-19) ⭐️ 5.0/10
20. [Mitchell Hashimoto: Languages Are Increasingly Expendable in AI Era](#item-20) ⭐️ 5.0/10
21. [Datasette IP Rate Limiting Plugin Released](#item-21) ⭐️ 5.0/10
22. [Boris Mann Critiques '11 AI Agents' as Meaningless Metric](#item-22) ⭐️ 5.0/10
23. [Tencent CEO Pony Ma Admits AI Was Initially Uncompetitive](#item-23) ⭐️ 5.0/10
24. [Google Tests 5GB Free Storage for New Gmail Accounts](#item-24) ⭐️ 5.0/10
25. [JD.com Launches AI Hardware Zone Selling NVIDIA RTX 5090 and Sanctioned H100](#item-25) ⭐️ 5.0/10
26. [ChatGPT Android APK Reveals Codex Mobile Remote Control Features](#item-26) ⭐️ 5.0/10
27. [AMD FSR 4.1 Coming to RX 7000 in July, RX 6000 in 2027](#item-27) ⭐️ 5.0/10
28. [Surge Declines VLESS Support Due to Non-Standard TLS Design](#item-28) ⭐️ 5.0/10

---

<a id="item-1"></a>
## [First Public macOS M5 Kernel Memory Corruption Exploit](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 9.0/10

The Calif team with AI system Mythos Preview achieved the first public macOS M5 kernel memory corruption exploit, bypassing Apple's MTE (Memory Tagging Extension) hardware protection in just 5 days (April 25 to May 1) to achieve root privileges from an unprivileged user. This represents the first public demonstration that AI + human collaboration can bypass Apple's 5-year MTE defense, potentially reshaping bug bounty valuations ($100K-$1.5M) and raising urgent questions about the future of hardware security in the AI era. The exploit chain involves two vulnerabilities and multiple techniques. A full 55-page technical report will be published after Apple releases a fix. The attack uses normal system calls and achieves local privilege escalation from an unprivileged user to root.

hackernews · quadrige · May 14, 18:25 · [Discussion](https://news.ycombinator.com/item?id=48139219)

**Background**: MTE (Memory Tagging Extension) is an ARMv9 hardware security feature that adds 4-bit allocation tags to 16-byte memory granules, allowing detection of use-after-free and buffer-overflow bugs. Apple implemented MTE (called MTE in their documentation) as a major defense mechanism starting with M1 chips, spending five years building this protection. Anthropic's Mythos Preview is an AI system designed for security research, previously found vulnerabilities in every major OS and browser.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.android.com/ndk/guides/arm-mte">Arm Memory Tagging Extension (MTE) | Android NDK | Android Developers</a></li>
<li><a href="https://www.npr.org/2026/04/11/nx-s1-5778508/anthropic-project-glasswing-ai-cybersecurity-mythos-preview">How AI is getting better at finding security holes : NPR</a></li>
<li><a href="https://simonwillison.net/2026/Apr/7/project-glasswing/">Anthropic’s Project Glasswing—restricting Claude Mythos to security ...</a></li>

</ul>
</details>

**Discussion**: Comments show a mix of excitement and concern: some praised the achievement as groundbreaking while noting the world is unprepared for LLM's impact on security. Others criticized the lack of technical details, with one asking how the bug survived MTE. There's discussion about bug bounty values ($100K-$1.5M depending on how it's packaged) and speculation about whether Apple should use more Swift in their own code.

**Tags**: `#security-research`, `#apple-m5`, `#kernel-exploit`, `#memory-corruption`, `#mte-bypass`, `#ai-security`, `#zero-day`

---

<a id="item-2"></a>
## [RTX 5090 eGPU with M4 MacBook Air: Gaming & LLM Benchmarks](https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/) ⭐️ 8.0/10

A technical deep-dive benchmarks gaming and local LLM performance when connecting an RTX 5090 eGPU to an M4 MacBook Air, showing significant AI inference improvements but revealing Mac gaming limitations due to OpenGL issues. This matters because it demonstrates the potential of external GPU solutions for Apple Silicon Macs, particularly for local AI inference, while also highlighting the ongoing challenges of gaming on macOS due to graphics API limitations. 该设置揭示了关键限制：1.5 GB内存窗口约束、macOS上OpenGL支持不佳（导致某些游戏无法游玩），以及需要通过MoltenVK支持Vulkan。LLM基准测试显示，与原生Apple Silicon相比，推理速度有显著提升。

hackernews · allenleee · May 14, 15:47 · [Discussion](https://news.ycombinator.com/item?id=48137145)

**Background**: eGPU (external Graphics Processing Unit) is a type of graphics card meant to be used outside the computer case, expanding built-in graphics processing capabilities through Thunderbolt connections. Local LLM inference means running large language models on personal hardware rather than remote servers, offering privacy and customization benefits. Apple officially states that eGPUs require Intel-based Macs and recommends AMD graphics cards, not NVIDIA.

<details><summary>References</summary>
<ul>
<li><a href="https://support.apple.com/en-us/102363">Use an external graphics processor with your Mac - Apple Support</a></li>
<li><a href="https://www.computerhope.com/jargon/e/egpu.htm">What Is an eGPU ( External Graphics Processing Unit)?</a></li>
<li><a href="https://prajnaaiwisdom.medium.com/what-is-local-llm-inference-a-beginners-guide-b31043768d4f">What Is Local LLM Inference? A Beginner’s Guide</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights mixed perspectives: some celebrate the technical achievement of getting RTX 5090 working with Apple Silicon, while others note this is a workaround since Apple officially states eGPUs don't work with Apple Silicon. Commenters particularly noted the LLM inference improvements as practically significant, while also discussing VM GPU passthrough limitations and the challenges of prompt processing speed on Macs.

**Tags**: `#eGPU`, `#Apple Silicon`, `#RTX 5090`, `#LLM Inference`, `#Mac Gaming`

---

<a id="item-3"></a>
## [Bun Merges Major Rewrite from Zig to Rust](https://github.com/oven-sh/bun/pull/30412) ⭐️ 8.0/10

Bun has merged a major rewrite of their JavaScript runtime from Zig to Rust, representing a significant architectural pivot. The rewrite addresses 10,428 unsafe code blocks across 736 files, aiming to eliminate use-after-free, double-free, and memory leak bugs through Rust's ownership system. This represents a major vote of confidence in Rust's memory safety guarantees for systems programming. The shift could set a new standard for runtime safety and reliability in the JavaScript ecosystem, as Bun becomes one of the largest Rust codebases with over 1 million lines of code. The rewrite includes detailed instructions for mapping Zig idioms to Rust equivalents, and the codebase already had internal smart pointer types that map 1-to-1 to Rust equivalents. However, maintainer Jarred noted that Rust won't catch all memory issues—leaks from holding references too long and anything that re-enters across the JS boundary remain the team's responsibility.

hackernews · Chaoses · May 14, 08:15 · [Discussion](https://news.ycombinator.com/item?id=48132488)

**Background**: Bun is a fast JavaScript runtime that was originally built using Zig, a systems programming language designed as a general-purpose improvement to C. Zig requires manual memory management, while Rust provides memory safety through its ownership system at compile time without garbage collection. This rewrite leverages Rust's ownership model to prevent common memory bugs that have historically plagued systems software.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Discussion**: Community members noted that the rewrite required extensive preparation, with detailed instructions mapping Zig to Rust idioms already in place. The statistics showing 10,428 unsafe blocks and over 1 million lines of Rust code drew both admiration and skepticism—some developers compared Bun's scale to the Rust compiler itself, questioning whether such a large codebase can be effectively maintained. Maintainer Jarred acknowledged that while Rust eliminates many memory bugs, some issues like reference lifetime problems across the JS boundary remain unresolved.

**Tags**: `#bun`, `#rust`, `#javascript-runtime`, `#zig`, `#memory-safety`, `#systems-programming`

---

<a id="item-4"></a>
## [Mullvad Exit IPs Enable User Fingerprinting](https://tmctmt.com/posts/mullvad-exit-ips-as-a-fingerprinting-vector/) ⭐️ 7.0/10

Security researchers discovered that Mullvad VPN exit IPs are deterministically assigned based on WireGuard keys rather than randomized, allowing user fingerprinting across different connections and servers. This undermines user privacy expectations as the same user can be identified across different Mullvad server connections, potentially linking their activities across websites and enabling deanonymization attacks. The exit IP is determined by the WireGuard key, which rotates every 1-30 days for official app users but never rotates for third-party clients. This creates a persistent fingerprint that can be used to link sessions with over 99% confidence when IP ranges overlap.

hackernews · RGBCube · May 15, 02:35 · [Discussion](https://news.ycombinator.com/item?id=48143880)

**Background**: VPN exit nodes are the final gateway between a user's device and the internet, masking the user's real IP address. WireGuard is a modern, fast VPN protocol that uses cryptographic keys for authentication. Deterministic IP assignment means the same input (WireGuard key) always produces the same output (exit IP), unlike randomized assignment which provides better anonymity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WireGuard">WireGuard - Wikipedia</a></li>
<li><a href="https://fastercapital.com/content/Exit-Node--Securing-Your-Online-Privacy--The-Role-of-Exit-Nodes-in-VPNs.html">Exit Node: Securing Your Online Privacy: The Role of Exit ...</a></li>

</ul>
</details>

**Discussion**: Comments reveal debate about the statistical claims and VPN vs Tor anonymity expectations. Some users argue VPNs were never designed to provide anonymity comparable to Tor, while others criticize the >99% confidence claim as unsupported. A notable viewpoint compares the design to 'how I'd design a VPN if I were an intelligence agency.'

**Tags**: `#vpn-security`, `#privacy`, `#mullvad`, `#fingerprinting`, `#wireguard`

---

<a id="item-5"></a>
## [Removing Toyota RAV4 Modem and GPS for Privacy](https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/) ⭐️ 7.0/10

A privacy researcher documented physically removing the cellular modem and GPS unit from their 2024 Toyota RAV4 Hybrid to prevent Toyota from collecting telemetry and location data. This highlights growing concerns about automotive data collection and demonstrates that some car owners are taking extreme physical measures to protect their privacy. The high engagement (744 points, 407 comments) indicates this is a significant concern for privacy-conscious vehicle owners. The researcher physically removed the hardware components from the vehicle. Community comments reveal that while Bluetooth connections allow the car to use the phone's internet for telemetry, wired USB connections with CarPlay do not. However, both CarPlay and Android Auto capture their own vehicle telemetry independently, meaning the privacy battle continues even after hardware removal.

hackernews · arkadiyt · May 14, 17:08 · [Discussion](https://news.ycombinator.com/item?id=48138136)

**Background**: Modern cars like the 2024 RAV4 come equipped with embedded cellular modems (telematics units) that continuously transmit vehicle data back to the manufacturer. This data can include location, driving behavior, speed, acceleration patterns, and diagnostic information. Privacy researchers have raised concerns about the extent of data collection and who has access to it, including potential sharing with insurance companies.

**Discussion**: The discussion reveals important nuances: commenters note that Bluetooth connections can still route telemetry through the phone even after the modem is removed, while USB/CarPlay avoids this. However, one commenter points out that CarPlay and Android Auto themselves capture vehicle telemetry. Some users have different motivations, like fixing GPS/compass issues. Others mention Ford vehicles have a removable telematics fuse as an easier alternative.

**Tags**: `#privacy`, `#hardware`, `#automotive`, `#security`, `#IoT`

---

<a id="item-6"></a>
## [DS4: Local DeepSeek 4 Runtime Released](https://antirez.com/news/165) ⭐️ 7.0/10

Antirez released DS4 (DwarfStar4), a specialized LLM inference runtime for running DeepSeek 4 locally with support for Metal, CUDA, and ROCm backends. This enables developers to run DeepSeek 4 locally on consumer hardware, potentially matching premium AI coding assistants at a fraction of the cost, challenging the business model of services like Anthropic. The runtime requires 96GB of VRAM, with Metal as the primary target for MacBooks. CUDA support focuses on NVIDIA DGX Spark, while ROCm support is maintained in a separate community branch. It builds on llama.cpp and GGML.

hackernews · caust1c · May 14, 22:29 · [Discussion](https://news.ycombinator.com/item?id=48142108)

**Background**: DeepSeek V4 is an AI coding assistant model that matches GPT-5.5 and Opus on agentic coding benchmarks at lower cost. ROCm is AMD's GPU computing platform for high-performance computing and AI. Metal is Apple's GPU framework for graphics and compute tasks on Apple devices.

<details><summary>References</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/news/news260424">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>
<li><a href="https://github.com/ROCm/ROCm">GitHub - ROCm / ROCm : AMD ROCm ™ Software - GitHub Home</a></li>
<li><a href="https://developer.apple.com/technologies/">Technologies - Apple Developer</a></li>

</ul>
</details>

**Discussion**: Users are excited about the possibility of running high-quality AI coding assistants locally, with one noting it's 'shockingly close to Claude' albeit slower. There's discussion about whether slower/cheaper models can match premium services, and questions about whether this will work on consumer hardware like 16GB RAM in the future. The imatrix quantization was praised as better than OpenRouter backends.

**Tags**: `#llm-inference`, `#deepseek`, `#open-source`, `#local-ai`, `#hardware-acceleration`

---

<a id="item-7"></a>
## [Nginx-Rift: 18-Year-Old Vulnerability Enables Remote Code Execution](https://github.com/DepthFirstDisclosures/Nginx-Rift) ⭐️ 7.0/10

Security researchers disclosed Nginx-Rift (CVE-2026-42945), a critical heap buffer overflow vulnerability in the NGINX rewrite module that has existed since 2008, affecting versions 0.6.27 through 1.30.0. F5 has released patches 1.31.0 and 1.30.1, along with a proof-of-concept exploit called Nginx-Rift. This vulnerability allows unauthenticated remote code execution in a widely-deployed web server, potentially affecting millions of production systems. The 18-year undetected period and the availability of a working exploit make this a critical concern for security teams. The exploit requires specific preconditions: a rewrite directive with a question mark in the replacement string, followed by a set directive that references an unnamed regex capture group (e.g., $1, $2). The published POC assumes ASLR is disabled, though researchers claim ASLR bypass is possible. Mitigation includes using named captures instead of unnamed captures.

hackernews · hetsaraiya · May 14, 17:17 · [Discussion](https://news.ycombinator.com/item?id=48138268)

**Background**: NGINX is one of the world's most popular web servers, powering a large percentage of websites and applications. The vulnerability exists in the rewrite module, which is commonly used for URL manipulation and redirection. ASLR (Address Space Layout Randomization) is a memory protection technique that randomizes memory addresses to make exploitation harder. Named captures in regex allow referencing matched groups by name rather than position.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/05/18-year-old-nginx-rewrite-module-flaw.html">18-Year-Old NGINX Rewrite Module Flaw Enables Unauthenticated...</a></li>
<li><a href="https://www.picussecurity.com/resource/blog/nginx-rift-cve-2026-42945-critical-heap-buffer-overflow-vulnerability-explained">NGINX Rift: CVE-2026-42945 Critical Heap Buffer Overflow Vulnerability Explained - Picus Security</a></li>
<li><a href="https://logicity.in/en/blog/18-year-old-nginx-bug-allows-dos-and-remote-code-execution">18-Year-Old NGINX Bug Allows DoS and Remote Code... | Logicity</a></li>

</ul>
</details>

**Discussion**: Security experts are debating the severity, with some noting the exploit requires specific configuration conditions. However, researchers emphasize that ASLR bypass is likely possible, and the vulnerability should not be dismissed. One commenter asked about memory-safe alternatives like Caddy (Go) or Jetty (Java), noting these have their own vulnerability histories.

**Tags**: `#security`, `#nginx`, `#vulnerability`, `#exploit`, `#f5`

---

<a id="item-8"></a>
## [Codex Now Available in ChatGPT Mobile App](https://openai.com/index/work-with-codex-from-anywhere/) ⭐️ 7.0/10

OpenAI's Codex coding agent is now available in the ChatGPT mobile app, making AI-assisted coding accessible on the go with a free tier option. This expands access to AI coding tools beyond desktop, potentially benefiting developers in regions with limited PC access and enabling quick code reviews or redirects on the go. Codex is available for free on both the desktop app and CLI - users just need to sign in to their ChatGPT account. The caveat is that interactions may be used for training. Some users report that mobile usage leads to less effective direction of the agent compared to keyboard use, potentially creating more tech debt.

hackernews · mikeevans · May 14, 20:06 · [Discussion](https://news.ycombinator.com/item?id=48140529)

**Background**: OpenAI Codex is an AI-driven coding agent that automates software engineering tasks, enabling developers to delegate activities such as feature development, code refactoring, debugging, and test generation. It represents a significant step in making AI-assisted coding more accessible to developers worldwide.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/OpenAI_Codex">OpenAI Codex</a></li>
<li><a href="https://www.reddit.com/r/OpenAI/comments/1n5iqqj/openai_nailed_it_with_codex_for_devs/">openAI nailed it with Codex for devs - Reddit</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed. Some find the free tier surprising and valuable, noting it could particularly benefit developers in regions like Nigeria with limited PC access. Others are more skeptical, with users reporting that mobile coding produces less optimal results compared to desktop use due to reduced screen size and lack of keyboard, potentially leading to more code churn. The ability to unblock or redirect longer-running work from a phone is seen as potentially underrated.

**Tags**: `#OpenAI`, `#Codex`, `#AI coding`, `#mobile development`, `#developer tools`

---

<a id="item-9"></a>
## [arXiv Implements 1-Year Ban for Hallucinated References](https://twitter.com/tdietterich/status/2055000956144935055) ⭐️ 7.0/10

arXiv has announced a new policy imposing a 1-year submission ban on authors whose papers contain hallucinated references—citations that do not exist but were generated by LLMs and not verified by authors. This policy addresses a growing crisis in academic publishing: the proliferation of non-existent citations in LLM-generated papers. Studies estimate over 146,000 hallucinated citations appeared in 2025 alone, threatening the integrity of scientific literature. The ban applies to hallucinated citations, LLM meta-comments left in text (like 'replace with real data'), and other unverified AI-generated content. After the 1-year ban expires, authors must have subsequent submissions accepted by a peer-reviewed venue before posting to arXiv. Authors bear full responsibility for all content regardless of how it was generated.

hackernews · gjuggler · May 14, 20:39 · [Discussion](https://news.ycombinator.com/item?id=48140922)

**Background**: Hallucinated references are fabricated citations that appear real but point to non-existent papers. Following widespread LLM adoption, studies have documented a sharp rise in these invalid citations across major scientific repositories including arXiv, bioRxiv, SSRN, and PubMed Central. A Nature analysis suggests tens of thousands of 2025 publications may contain AI-generated invalid references.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nature.com/articles/d41586-026-00969-z">Hallucinated citations are polluting the scientific ... - Nature</a></li>
<li><a href="https://arxiv.org/abs/2605.07723">[2605.07723] LLM hallucinations in the wild: Large-scale ...</a></li>

</ul>
</details>

**Discussion**: The community response is largely supportive, with commenters viewing the ban as appropriate for maintaining science integrity—arXiv is a privilege, not a right. Some raised concerns about citation management tools making it difficult to generate correct BibTeX entries. Others noted that LLM critics are facing backlash from AI proponents, with some dismissing any hindrance to rapid LLM adoption.

**Tags**: `#arXiv`, `#academic-publishing`, `#research-integrity`, `#LLM`, `#policy`

---

<a id="item-10"></a>
## [Ontario Auditors Find Doctors' AI Note Takers Make Basic Factual Errors](https://www.theregister.com/ai-ml/2026/05/14/ontario-auditors-find-doctors-ai-note-takers-routinely-blow-basic-facts/5240771) ⭐️ 7.0/10

Ontario's auditors found that AI-powered note-taking systems used by doctors routinely make basic factual errors, raising serious patient safety concerns. The audit revealed systematic accuracy problems with AI medical transcription tools deployed in clinical settings. This is significant because AI medical scribes are increasingly being adopted across healthcare systems, and factual errors in medical documentation could lead to misdiagnoses, inappropriate treatments, and compromised patient safety. The findings highlight a critical gap between AI capabilities and the precision required in medical contexts. The audit specifically identified problems with AI systems that convert patient-doctor conversations into clinical notes. These AI scribes use ambient listening technology to generate documentation, but they frequently hallucinate or misinterpret information, potentially including incorrect diagnoses or symptoms that were never discussed.

hackernews · sohkamyung · May 14, 22:37 · [Discussion](https://news.ycombinator.com/item?id=48142188)

**Background**: AI medical scribe technology (such as DeepScribe, Sunoh.ai, and MarianaAI) uses ambient listening to convert clinical conversations into documentation in real-time. Research has identified three types of AI hallucinations: input-conflicting, context-conflicting, and fact-conflicting, all of which can undermine trust and efficacy in healthcare settings. Studies have shown that AI hallucinations in healthcare can lead to misdiagnoses and inappropriate treatments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.deepscribe.ai/">DeepScribe AI Medical Scribe | Built for Specialty Care</a></li>
<li><a href="https://www.eclinicalworks.com/sunoh-ai-medical-scribe-technology-for-clinical-documentation/">Sunoh. ai - Medical AI Scribe Technology for Clinical Documentation</a></li>
<li><a href="https://www.medscape.com/viewarticle/ai-hallucinations-are-changing-medicine-should-we-worry-2025a1000647">AI ‘Hallucinations’ Are Changing Medicine — Should We Worry?</a></li>

</ul>
</details>

**Discussion**: Commenters shared personal anecdotes validating the concerns about AI accuracy. One commenter described how an AI summary incorrectly stated they were diagnosed with osteoporosis when they actually had Runner's Knee. Another noted that LLM note-takers at work promised things that were never actually said in meetings. Overall, the discussion highlighted widespread agreement that AI outputs require careful verification, especially in sensitive domains like healthcare.

**Tags**: `#ai-limitations`, `#healthcare`, `#hallucination`, `#medical-technology`, `#audit-findings`

---

<a id="item-11"></a>
## [MIT President Kornbluth on Funding and Talent Pipeline Crisis](https://president.mit.edu/writing-speeches/video-transcript-message-president-kornbluth-about-funding-and-talent-pipeline) ⭐️ 7.0/10

MIT President Kornbluth addressed funding challenges and talent pipeline issues in academia, sparking widespread debate about PhD prospects, research funding declines, and the future of higher education. This matters because it highlights a systemic crisis in academia affecting the tech talent pipeline, with 80% of recent PhD graduates considering leaving academia despite entering to pursue academic careers. The discussion reflects broader concerns about research funding declines and university sustainability. The median science PhD now takes 6 years with grueling work for relatively low pay, and job prospects are difficult given the current market. Unfunded students are less likely to accept admissions, creating a cycle of declining talent pipeline.

hackernews · dmayo · May 14, 14:51 · [Discussion](https://news.ycombinator.com/item?id=48136262)

**Background**: MIT President Kornbluth's message addresses the intersection of research funding and talent pipeline in higher education. The discussion touches on the challenges facing academia, including declining grant success rates, the financial burden on PhD students, and the sustainability of the traditional academic model. This comes at a time when universities face increasing pressure to demonstrate workforce readiness and ROI for students.

**Discussion**: Comments reveal deep disillusionment with academia, with many noting that 80% of recent PhD grads are looking to leave. Some view this as a generational reset for broken systems, while others argue that PhDs going to industry isn't wasted - particularly in fields like nanofabrication and semiconductors. International perspectives from India and China add nuance, with China's rising position in higher education noted.

**Tags**: `#academia`, `#higher-education`, `#funding`, `#talent-pipeline`, `#research`

---

<a id="item-12"></a>
## [Anthropic Launches Claude for Small Business](https://www.anthropic.com/news/claude-for-small-business) ⭐️ 7.0/10

Anthropic has launched Claude for Small Business, integrating Claude with QuickBooks, PayPal, HubSpot, Canva, DocuSign, Google Workspace, and Microsoft 365. The service offers 15 ready-to-run workflows and 15 skills covering finance, sales, marketing, HR, and customer service tasks. This launch represents Anthropic's strategic push into the small business market, competing with other AI assistants targeting enterprise customers. The integration with major business tools and focus on practical workflows could make AI more accessible to smaller companies with limited technical resources. The service runs on Claude Cowork, Anthropic's agentic AI system that executes multi-step knowledge work including research synthesis, document preparation, and file management. It requires user approval before sending, publishing, or making payments. Team and Enterprise tiers do not use customer data for model training by default.

telegram · zaihuapd · May 14, 12:41

**Background**: Claude Cowork is Anthropic's product for knowledge work that brings Claude Code's agentic capabilities to desktop applications. It can execute multi-step tasks on behalf of users, such as drafting reports by pulling from meeting notes and project documents. This launch expands Anthropic's strategy to target different market segments beyond enterprise customers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/product/claude-cowork">Claude Cowork | Anthropic ’s agentic AI for knowledge work</a></li>
<li><a href="https://claude.com/product/cowork">Cowork : Claude Code power for knowledge... | Claude by Anthropic</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#Claude AI`, `#Small Business`, `#AI Products`, `#Business Automation`

---

<a id="item-13"></a>
## [OpenAI Sued for Sharing User Data with Meta and Google](https://futurism.com/artificial-intelligence/openai-personal-information-meta-google) ⭐️ 7.0/10

A class action lawsuit filed in California alleges that OpenAI shared user data including chat queries, email addresses, and user IDs with Meta and Google without proper consent, using Meta Pixel and Google Analytics tracking tools. This lawsuit represents a significant legal challenge to AI companies' data practices, potentially setting a precedent for how user data must be protected in the AI era. If successful, it could force major changes across the industry regarding consent and data sharing with third parties. The lawsuit claims the data transfers occurred via Meta Pixel and Google Analytics tracking pixels installed on OpenAI's platforms, allegedly violating California's Privacy Invasion Law and Electronic Communications Privacy Act. OpenAI has not yet responded to requests for comment.

telegram · zaihuapd · May 15, 03:45

**Background**: Meta Pixel (formerly Facebook Pixel) is a JavaScript tracking code that collects user activity data on websites and shares it with Meta's advertising platform for ad optimization. Google Analytics performs similar tracking functions for Google. Both tools can collect personal identifiers and behavioral data. California has some of the strongest privacy laws in the US, including the California Consumer Privacy Act (CCPA), which requires companies to disclose data collection and obtain consent.

<details><summary>References</summary>
<ul>
<li><a href="https://www.facebook.com/business/tools/meta-pixel/">Meta Pixel: Measure, Optimize & Retarget Ads on Facebook ...</a></li>
<li><a href="https://support.google.com/analytics/answer/9213390?hl=en">Measure activity across platforms with User-ID - Analytics Help</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#privacy`, `#legal`, `#Meta`, `#Google`, `#AI regulation`

---

<a id="item-14"></a>
## [HDD Firmware Hacking Technical Exploration](https://icode4.coffee/?p=1465) ⭐️ 6.0/10

A technical blog post explores HDD firmware hacking techniques, demonstrating reverse engineering and modification of hard drive firmware. This research highlights critical security vulnerabilities in storage devices, demonstrating how attackers could potentially modify HDD firmware for persistent malware or data exfiltration. The article provides a deep-dive into firmware reverse engineering techniques specific to HDDs, with community comments adding related examples including Samsung 840 EVO firmware decompilation and SSD obfuscation bypass methods.

hackernews · jsploit · May 14, 16:19 · [Discussion](https://news.ycombinator.com/item?id=48137553)

**Background**: HDD firmware is low-level software that controls hard drive operations including data reading/writing, error correction, and hardware management. Firmware modification can give attackers deep system access that survives OS reinstalls. This research comes amid growing concerns about supply chain security and hardware-level threats.

**Discussion**: Comments highlight related security issues: one user describes bypassing SSD firmware encryption using seccomp to intercept decrypted firmware during updates, while another mentions Samsung 840 EVO firmware being decompiled before Samsung encrypted subsequent versions. Users also discuss Red Balloon's interview CTF involving a physical hard drive and firmware patching of cheap disk controllers.

**Tags**: `#hardware-security`, `#firmware`, `#reverse-engineering`, `#storage`, `#security-research`

---

<a id="item-15"></a>
## [US Approves NVIDIA H200 Sales to 10 Chinese Firms](https://www.reuters.com/business/retail-consumer/us-clears-h200-chip-sales-10-china-firms-nvidia-ceo-looks-breakthrough-2026-05-14/) ⭐️ 6.0/10

The US Commerce Department has approved NVIDIA H200 chip sales to approximately 10 Chinese companies, including Alibaba, Tencent, ByteDance, and JD.com. Distributors like Lenovo and Foxconn also received licenses, with single customers permitted to purchase up to 75,000 chips. This approval marks a significant development in US-China tech relations, as the H200 is one of the most advanced AI accelerators currently available. The decision reflects the ongoing balancing act between geopolitical tensions and commercial interests in the semiconductor industry. Despite the approval, no deliveries have been completed yet, with some Chinese companies becoming more cautious under Beijing's guidance. Jensen Huang's visit to China is viewed as a critical effort to facilitate deal implementation.

telegram · zaihuapd · May 14, 08:57

**Background**: The NVIDIA H200 is based on the Hopper architecture and represents a significant upgrade over the H100. It is the first GPU to offer 141 GB of HBM3e memory at 4.8 TB/s, nearly double the capacity of the H100 with 1.4X more memory bandwidth. This makes it particularly powerful for generative AI and large language model workloads. The US has maintained export controls on advanced chips to China amid ongoing tech competition, creating complex challenges for NVIDIA in one of its largest markets.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">NVIDIA H200 GPU</a></li>
<li><a href="https://www.trgdatacenters.com/resource/nvidia-h200-vs-h100/">NVIDIA GPUs H200 vs. H100 - A detailed comparison guide | TRG Datacenters</a></li>
<li><a href="https://vast.ai/article/nvidia-h100-vs-h200-two-hopper-based-heavyweights">NVIDIA H100 vs. H200: Two Hopper-based Heavyweights</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#US-China Tech Relations`, `#AI Chips`, `#Geopolitics`, `#Export Controls`

---

<a id="item-16"></a>
## [Obesity Rates Stabilize in Rich Nations, Rise in Low-Income Countries](https://www.nature.com/articles/s41586-026-10383-0) ⭐️ 6.0/10

A Nature study covering 200 countries and 232 million people over 44 years (1980-2024) found that obesity rates have stabilized in high-income countries since the 2000s, while continuing to rise steadily or accelerate in low- and middle-income countries, with some already surpassing developed nations. This represents a significant global health trend reversal with major implications for public health policy worldwide. The findings suggest that social, economic, and technological factors affecting food availability and affordability may have helped high-income countries curb obesity growth, while low- and middle-income countries still require policy interventions. The study shows that childhood and adolescent obesity rate increases in high-income countries began slowing in the 1990s, with countries like Italy, Portugal, and France even experiencing slight declines after the 2000s. Adult obesity rates followed a similar plateau pattern, occurring about a decade later than the youth trend.

telegram · zaihuapd · May 14, 09:45

**Background**: Obesity is a major global health concern linked to increased risks of diabetes, cardiovascular disease, and certain cancers. The World Health Organization has classified obesity as a growing epidemic worldwide. This study provides comprehensive epidemiological data spanning nearly five decades across nearly all countries, making it one of the most extensive analyses of global obesity trends to date.

**Tags**: `#public-health`, `#epidemiology`, `#global-health`, `#obesity`, `#research`

---

<a id="item-17"></a>
## [Huawei, JAC, Stellantis in Talks for Maserati EV Partnership](https://eu.36kr.com/zh/p/3807764479680774) ⭐️ 6.0/10

Huawei, JAC Motors, and Stellantis Group are in negotiations to jointly develop Maserati-branded electric vehicles, with Huawei providing core technology, JAC handling R&D and manufacturing, and Maserati offering design and brand endorsement. This partnership represents a significant trend of foreign heritage brands partnering with Chinese EV technology providers to accelerate electrification, as traditional luxury automakers struggle with the transition to electric vehicles. The first model is currently in the design phase with planned production in the second half of next year. Domestic versions will be sold under Huawei's 'Zunjie' (尊界) brand while overseas versions will bear the Maserati logo. No formal agreement has been signed yet despite R&D work already underway since early last year.

telegram · zaihuapd · May 14, 11:15

**Background**: Stellantis is one of the world's largest automotive groups formed by the merger of Fiat Chrysler Automobiles and PSA Group, owning brands including Maserati, Jeep, and Ferrari. Huawei's HarmonyOS Intelligent Mobility (鸿蒙智行) has been rapidly expanding its EV partnerships, with the 'Zunjie' brand representing its ultra-luxury positioning. Maserati has been facing sales pressures and needs to accelerate its EV transition to meet stricter emission regulations.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/斯泰蘭蒂斯">斯 特 兰 蒂 斯 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.stellantis.com/">Official Global Website | Stellantis</a></li>
<li><a href="https://auto.news18a.com/news/storys_255822.html">所有人都在吹 尊 界 200...</a></li>

</ul>
</details>

**Tags**: `#新能源汽车`, `#华为`, `#玛莎拉蒂`, `#电动汽车`, `#汽车合作`, `#江淮汽车`

---

<a id="item-18"></a>
## [DeepSeek Chat Session Isolation Vulnerability Leaks User Conversations](https://github.com/deepseek-ai/DeepSeek-R1/issues/840) ⭐️ 6.0/10

A session isolation vulnerability in DeepSeek's chat system allows attackers to leak other users' conversation history by sending an unclosed <think> tag in empty conversations, potentially exposing sensitive information like code, keys, and privacy data. This represents a serious privacy breach in a widely-used AI platform, as it exposes confidential user data to unauthorized parties and undermines the fundamental trust in session isolation that users expect from chat systems. The vulnerability affects both DeepSeek Web and API interfaces. The reporter (cancat2024) disclosed the issue responsibly on May 11, 2026 without exploiting it to obtain or spread others' privacy data.

telegram · zaihuapd · May 14, 13:15

**Background**: Session isolation is a fundamental security principle in multi-user systems that ensures one user's data remains inaccessible to other users. The <think> tag is used by DeepSeek's reasoning models to display the model's internal thinking process. Prompt injection is a well-known security vulnerability that manipulates AI models through adversarial prompt engineering.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://github.com/vllm-project/vllm/discussions/12708">Nested `` and `` tag in deepseek-r1 reasoning parser · vllm-project/vllm · Discussion #12708</a></li>

</ul>
</details>

**Discussion**: Some community members expressed skepticism about the vulnerability, with one commenter suggesting it might be a hallucination since third-party deployments also exhibit similar behavior.

**Tags**: `#security vulnerability`, `#DeepSeek`, `#privacy`, `#session isolation`, `#AI safety`

---

<a id="item-19"></a>
## [Technology Lock-in Decreases as Cross-Platform Tools Improve](https://simonwillison.net/2026/May/14/not-so-locked-in/#atom-everything) ⭐️ 5.0/10

Simon Willison shares an anecdote about a company using coding agents to rewrite their legacy iPhone and Android apps to React Native, noting that React Native has improved significantly and they can port back to native if needed. This reflects a broader trend where technology lock-in is decreasing because cross-platform tools have matured and coding agents make it easier to switch platforms. Developers no longer need to fear getting locked into a single technology stack. The company chose React Native despite coding agents making separate iOS/Android development cheaper, because React Native now covers all their needs. Mitchell Hashimoto's example of Bun migrating from Zig to Rust illustrates that even programming languages themselves are no longer a form of lock-in.

rss · Simon Willison · May 14, 22:53

**Background**: React Native is a framework for building cross-platform mobile apps using JavaScript and React. Coding agents are AI-powered tools that can autonomously write and modify code. The concept of technology lock-in refers to the situation where a developer becomes dependent on a specific technology and switching to alternatives would be costly or time-consuming. Previously, choosing a programming language or platform often meant being permanently locked into that ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#software-development`, `#react-native`, `#technology-lock-in`, `#coding-agents`, `#cross-platform-development`

---

<a id="item-20"></a>
## [Mitchell Hashimoto: Languages Are Increasingly Expendable in AI Era](https://simonwillison.net/2026/May/14/mitchell-hashimoto/#atom-everything) ⭐️ 5.0/10

Mitchell Hashimoto commented that programming languages have become increasingly fungible, using Bun's recent rewrite from Zig to Rust as evidence. He suggested that Bun could port to "any language they want in roughly a week or two." This observation challenges the traditional view of programming languages as strategic lock-in assets. If AI tools can make language switching trivial, it could reshape how developers choose technologies and how companies invest in language-specific ecosystems. Hashimoto specifically mentioned Bun's ability to rewrite in any language within a week or two as evidence of language expendability. He framed this as interesting rather than positive or negative, noting that Rust is "useful until its not then it can be thrown out."

rss · Simon Willison · May 14, 22:31

**Background**: Mitchell Hashimoto is the creator of widely-used developer tools including Terraform and Vagrant, co-founder of HashiCorp. Bun is a JavaScript runtime that was originally written in Zig and recently announced a port to Rust. The observation connects to the broader trend of AI-powered code generation making it easier to work across multiple programming languages.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>

</ul>
</details>

**Tags**: `#programming-languages`, `#rust`, `#zig`, `#developer-tools`, `#ai-impact`

---

<a id="item-21"></a>
## [Datasette IP Rate Limiting Plugin Released](https://simonwillison.net/2026/May/14/datasette-ip-rate-limit/#atom-everything) ⭐️ 5.0/10

Simon Willison released datasette-ip-rate-limit 0.1a0, a configurable IP-based rate limiting plugin for Datasette built with assistance from Codex AI (GPT-5.5 xhigh), now deployed on datasette.io to block abusive crawlers. This addresses a practical need for Datasette users dealing with abusive crawlers, demonstrating how AI tools can accelerate plugin development. The production configuration provides a template for others facing similar issues. The plugin supports configurable rules per path, with a window_seconds setting of 60 and max_requests of 60 for demo-databases, blocking for 20 seconds. It uses the Fly-Client-IP header for IP detection, which is provided by the Fly.io platform where datasette.io is hosted.

rss · Simon Willison · May 14, 04:10

**Background**: Datasette is an open source multi-tool for exploring and publishing data, built with Python. It supports a plugin system that extends its functionality. The Fly-Client-IP header is added by Fly.io's proxy to identify the original client IP address, though it must be used carefully to avoid spoofing issues.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>
<li><a href="https://fly.io/docs/networking/request-headers/">Request headers · Fly Docs</a></li>

</ul>
</details>

**Tags**: `#Datasette`, `#Rate Limiting`, `#Python`, `#Plugins`, `#AI-Assisted Development`

---

<a id="item-22"></a>
## [Boris Mann Critiques '11 AI Agents' as Meaningless Metric](https://simonwillison.net/2026/May/13/boris-mann/#atom-everything) ⭐️ 5.0/10

Boris Mann critiques the phrase '11 AI agents' as meaningless, comparing it to saying 'I have 11 spreadsheets' or '11 browser tabs' - where the number itself conveys little about the actual work or capability. This critique highlights the vague terminology problem in AI discourse, where 'agent' has become a buzzword without clear definition. It matters because precise terminology is crucial for meaningful discussions about AI capabilities, limitations, and market claims. Mann's comparison points out that simply counting 'AI agents' provides no meaningful information - much like counting spreadsheets or browser tabs says nothing about what work is actually being done or the complexity of the tasks.

rss · Simon Willison · May 13, 16:15

**Background**: AI agents are software systems that use AI to pursue goals and complete tasks on behalf of users. The term 'AI agent' has been traced back to research from the 1990s, and researcher Andrew Ng is credited with popularizing 'agentic' to wider audiences in 2024. The lack of clear definition has made 'AI agent' a vague marketing term that different companies use to describe various types of autonomous AI systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://cloud.google.com/discover/what-are-ai-agents">What are AI agents? Definition, examples, and types</a></li>
<li><a href="https://github.com/resources/articles/what-are-ai-agents">What are AI agents ? · GitHub</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#ai`, `#agent-definitions`, `#terminology`, `#discourse`

---

<a id="item-23"></a>
## [Tencent CEO Pony Ma Admits AI Was Initially Uncompetitive](https://t.me/zaihuapd/41377) ⭐️ 5.0/10

At Tencent's shareholders' meeting, CEO Pony Ma responded to questions about whether Tencent's AI is lagging behind, acknowledging that the company's early AI capabilities were not competitive. He used a metaphor: last year they thought they were on the boat, then discovered it was leaking, and now they've stabilized but cannot yet sit comfortably. This admission provides rare insight into Tencent's self-assessment of its AI position compared to competitors like ByteDance and Alibaba. It signals a more cautious, steady approach to AI development rather than aggressive expansion, which could shape Tencent's competitive strategy in the coming years. Ma specifically mentioned that Tencent has been addressing its weaknesses through talent building, team management, and internal training. He emphasized that Tencent will not blindly rush into areas simply because competitors are布局ing there, but will advance steadily based on its own advantages.

telegram · zaihuapd · May 14, 06:52

**Background**: This shareholders' meeting comment reflects Tencent's broader AI strategy as the company seeks to catch up in the generative AI race. Unlike some competitors who have made aggressive AI announcements, Tencent has taken a more measured approach, focusing on building foundational capabilities rather than racing to release consumer-facing AI products.

**Tags**: `#Tencent`, `#AI Strategy`, `#Corporate News`, `#Pony Ma`, `#Chinese Tech`

---

<a id="item-24"></a>
## [Google Tests 5GB Free Storage for New Gmail Accounts](https://www.androidauthority.com/google-gmail-5gb-free-storage-test-3667002/) ⭐️ 5.0/10

Google is testing a reduced 5GB free storage limit for newly created Gmail accounts, down from the standard 15GB. Users can unlock the full 15GB capacity by adding a phone number to their account. This change could affect millions of new users who rely on Gmail's free storage for email and Google Drive files. If implemented permanently, it would represent a significant shift in Google's free service offerings and could drive more users toward paid storage plans. The test appears to be an A/B test rather than a confirmed permanent change. Google has not officially announced the policy shift, and the support pages still list 15GB as the standard free storage limit. It remains unclear whether this is a regional test or a global policy change.

telegram · zaihuapd · May 14, 14:07

**Background**: Since 2014, Google has offered 15GB of free storage shared across Gmail, Google Drive, and Google Photos. This storage pool has been the standard for all Google account users. The current test reduces new account storage to 5GB unless users verify their identity with a phone number, potentially serving anti-spam or data collection purposes.

**Tags**: `#Google`, `#Gmail`, `#Cloud Storage`, `#Policy Change`, `#A/B Testing`

---

<a id="item-25"></a>
## [JD.com Launches AI Hardware Zone Selling NVIDIA RTX 5090 and Sanctioned H100](https://u.jd.com/HaDkFMa) ⭐️ 5.0/10

JD.com has opened an 'AI Hardware JD Self-operated Zone' selling NVIDIA products including GeForce RTX 5090 32G Turbo, RTX PRO 6000 Blackwell server edition, and previously sanctioned H100 chips. This is significant because H100 chips were previously restricted from export to China due to US sanctions. The availability of these products suggests potential workarounds to US export controls, which could have major implications for the AI chip market and US-China tech relations. The RTX 5090 Turbo is described as an uncut global standard version. The RTX PRO 6000 targets professional rendering and data center applications. The source is a Telegram deals channel rather than an authoritative tech news outlet, making independent verification difficult.

telegram · zaihuapd · May 14, 15:15

**Background**: The US imposed export restrictions on advanced AI chips like NVIDIA's H100 to China starting in 2022, requiring special licenses for export. The H100 was specifically targeted due to its high compute capabilities useful for AI training. In 2025, there were reports of smuggling rings attempting to export $160 million worth of H100 and H200 GPUs to China. NVIDIA's Blackwell architecture succeeds Hopper and Ada Lovelace, with the RTX PRO 6000 featuring 96GB GDDR7 memory.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2025/12/31/160-million-export-controlled-nvidia-gpus-allegedly-smuggled-to-china.html">$160 million export-controlled Nvidia GPUs allegedly ... - CNBC</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/">The Engine Behind AI Factories | NVIDIA Blackwell Architecture</a></li>
<li><a href="https://www.pny.com/en-eu/nvidia-rtx-pro-6000-blackwell-ws">NVIDIA RTX PRO 6000 Blackwell Workstation Edition | Professional GPUs | pny.com</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#AI hardware`, `#China tech`, `#export controls`, `#JD.com`

---

<a id="item-26"></a>
## [ChatGPT Android APK Reveals Codex Mobile Remote Control Features](https://t.me/zaihuapd/41388) ⭐️ 5.0/10

The ChatGPT Android APK version 1.2026.125 was reverse engineered, revealing strings that indicate OpenAI is developing phone-based remote control capabilities for Codex desktop sessions, allowing users to find and reconnect to remote sessions from their mobile device. This discovery suggests OpenAI is expanding Codex beyond a CLI tool to a cross-device experience, potentially enabling developers to control their coding sessions remotely from mobile devices, which could significantly change how developers work on code. The feature requires the desktop client to be logged into the same account as the mobile device for session reconnection. It is still in early development with no preview available and no officially announced release timeline.

telegram · zaihuapd · May 14, 21:48

**Background**: OpenAI Codex is an AI-driven coding agent designed to automate software engineering tasks. The Codex CLI runs locally on computers, while the mobile remote control feature would extend its functionality to mobile devices. APK reverse engineering is a common technique where security researchers and developers decompile Android apps to discover hidden features, strings, and potential future functionalities.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI</a></li>
<li><a href="https://github.com/openai/codex">GitHub - openai/codex: Lightweight coding agent that runs in ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#ChatGPT`, `#Codex`, `#reverse-engineering`, `#mobile-remote-control`

---

<a id="item-27"></a>
## [AMD FSR 4.1 Coming to RX 7000 in July, RX 6000 in 2027](https://videocardz.com/newz/amd-fsr-upscaling-4-1-officially-coming-to-radeon-rx-7000-gpus-in-july-rx-6000-in-2027) ⭐️ 5.0/10

AMD has confirmed that FSR 4.1, its machine learning-based upscaling technology, will launch for the Radeon RX 7000 series (RDNA 3) in July 2025 with support for over 300 games at launch. The RX 6000 series (RDNA 2) will receive FSR 4.1 support in early 2027. This announcement matters because it brings AMD's latest AI upscaling improvements to previous-generation RDNA 3 GPUs, though the extended timeline for RDNA 2 support (until 2027) highlights the technical challenges of porting ML models to older hardware with different AI accelerator architectures. FSR 4.1 was specifically developed for first-generation AI accelerators using INT8 instructions, which differs from RDNA 4's FP8 approach used in RX 9000 series. The update improves sharpness and reduces smearing and blur compared to FSR 4.0, while also optimizing Ultra Performance and dynamic resolution scaling modes.

telegram · zaihuapd · May 15, 04:57

**Background**: FSR (FidelityFX Super Resolution) is AMD's answer to Nvidia's DLSS, using machine learning to upscale lower-resolution images to higher resolutions for better performance in games. RDNA 3 is AMD's RDNA 3 architecture used in RX 7000 series GPUs, while RDNA 2 powers the RX 6000 series. The key difference is that RDNA 4 (RX 9000) has newer FP8 AI acceleration, while RDNA 3 and older use INT8 integer-based AI acceleration that requires more optimization.

<details><summary>References</summary>
<ul>
<li><a href="https://videocardz.com/newz/amd-fsr-upscaling-4-1-officially-coming-to-radeon-rx-7000-gpus-in-july-rx-6000-in-2027">AMD FSR Upscaling 4.1 officially coming to Radeon RX 7000 ...</a></li>
<li><a href="https://linustechtips.com/topic/1637457-amd-confirms-fsr-41-upscaling-for-radeon-rx-7000-series/">AMD confirms FSR 4.1 Upscaling for Radeon RX 7000 series</a></li>
<li><a href="https://www.techspot.com/article/3102-amd-fsr-41-tested/">Testing AMD FSR 4.1: Sharper Images, But DLSS Still Leads</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#FSR`, `#GPU`, `#graphics`, `#upscaling`

---

<a id="item-28"></a>
## [Surge Declines VLESS Support Due to Non-Standard TLS Design](https://t.me/zaihuapd/41396) ⭐️ 5.0/10

Surge developer has officially responded to long-standing user requests for VLESS protocol support, stating they will not merge it into the official version. Despite completing an experimental implementation, the non-standard TLS layering design requires custom modifications to upstream TLS libraries like OpenSSL or BoringSSL. This decision affects the network proxy tool community, as VLESS is a popular protocol for bypassing censorship. The technical reasoning highlights the trade-off between protocol compatibility and maintenance burden, especially for commercial products that need stable upstream TLS library updates. VLESS and its variants (like XTLS/Vision) deviate from traditional TLS layering boundaries, requiring non-standard modifications to TLS libraries. This cross-layer design increases TLS subsystem complexity, security assessment costs, and makes it difficult to follow upstream library updates.

telegram · zaihuapd · May 15, 05:36

**Background**: Surge is a well-known network proxy tool for advanced users. VLESS is a lightweight proxy protocol designed to bypass censorship, often used with XTLS which optimizes TLS performance by removing redundant encryption layers. XTLS is part of the Xray-core project, a popular implementation for censorship circumvention.

<details><summary>References</summary>
<ul>
<li><a href="https://vless.dev/">Quick guide to setting up a Vless Reality Proxy server</a></li>
<li><a href="https://github.com/XTLS/Xray-core">GitHub - XTLS /Xray-core: Xray, Penetrates Everything. Also the best...</a></li>

</ul>
</details>

**Discussion**: Users in the community acknowledge the technical validity of Surge's explanation but express disappointment that VLESS support will not be officially available. Some understand the maintenance concerns while others continue to seek alternative solutions.

**Tags**: `#Surge`, `#VLESS`, `#network-proxy`, `#TLS`, `#XTLS`

---