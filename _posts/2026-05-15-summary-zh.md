---
layout: default
title: "Horizon Summary: 2026-05-15 (ZH)"
date: 2026-05-15
lang: zh
---

> From 38 items, 28 important content pieces were selected

---

1. [首个公开的 Apple M5 macOS 内核内存破坏漏洞利用](#item-1) ⭐️ 9.0/10
2. [RTX 5090 外接显卡搭配 M4 MacBook Air：游戏与 LLM 基准测试](#item-2) ⭐️ 8.0/10
3. [Bun 完成从 Zig 到 Rust 的大规模重写](#item-3) ⭐️ 8.0/10
4. [Mullvad 出口 IP 可被用于用户指纹识别](#item-4) ⭐️ 7.0/10
5. [为保护隐私移除丰田 RAV4 的调制解调器和 GPS](#item-5) ⭐️ 7.0/10
6. [DS4：本地运行 DeepSeek 4 的专用运行时发布](#item-6) ⭐️ 7.0/10
7. [Nginx-Rift：发现可导致远程代码执行的 18 年历史漏洞](#item-7) ⭐️ 7.0/10
8. [Codex 现已在 ChatGPT 移动应用中可用](#item-8) ⭐️ 7.0/10
9. [arXiv 实施幻觉引用一年禁令](#item-9) ⭐️ 7.0/10
10. [安大略省审计员发现医生使用的 AI 笔记工具经常出现基本事实错误](#item-10) ⭐️ 7.0/10
11. [MIT 校长科恩布鲁斯谈资金与人才输送危机](#item-11) ⭐️ 7.0/10
12. [Anthropic 推出面向小企业的 Claude 套餐](#item-12) ⭐️ 7.0/10
13. [OpenAI 因未经同意向 Meta 和 Google 分享用户数据被起诉](#item-13) ⭐️ 7.0/10
14. [硬盘固件黑客技术深度探索](#item-14) ⭐️ 6.0/10
15. [美国批准英伟达 H200 芯片对约 10 家中国企业销售](#item-15) ⭐️ 6.0/10
16. [发达国家肥胖率上升趋稳，中低收入国家仍在加速](#item-16) ⭐️ 6.0/10
17. [华为、江淮与斯特兰蒂斯洽谈玛莎拉蒂新能源车合作](#item-17) ⭐️ 6.0/10
18. [DeepSeek 对话系统会话隔离漏洞可泄露用户对话](#item-18) ⭐️ 6.0/10
19. [随着跨平台工具改进，技术锁定效应减弱](#item-19) ⭐️ 5.0/10
20. [Mitchell Hashimoto：AI 时代编程语言日益变得可替代](#item-20) ⭐️ 5.0/10
21. [Datasette IP 限流插件发布](#item-21) ⭐️ 5.0/10
22. [Boris Mann 批评「11 个 AI 智能体」说法毫无意义](#item-22) ⭐️ 5.0/10
23. [马化腾承认腾讯 AI 初期缺乏竞争力](#item-23) ⭐️ 5.0/10
24. [谷歌测试新 Gmail 账户 5GB 免费存储](#item-24) ⭐️ 5.0/10
25. [京东上线 AI 硬件自营专区 销售 RTX 5090 及受制裁 H100 芯片](#item-25) ⭐️ 5.0/10
26. [ChatGPT Android 版拆解发现 Codex 手机远控功能](#item-26) ⭐️ 5.0/10
27. [AMD FSR 4.1 将于 7 月支持 RX 7000，2027 年初支持 RX 6000](#item-27) ⭐️ 5.0/10
28. [Surge 因非标准 TLS 设计拒绝支持 VLESS 协议](#item-28) ⭐️ 5.0/10

---

<a id="item-1"></a>
## [首个公开的 Apple M5 macOS 内核内存破坏漏洞利用](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 9.0/10

这代表了 AI 与人类协作首次公开突破 Apple 耗时五年构建的 MTE 防御，可能重塑漏洞赏金估值（10 万至 150 万美元），并引发关于 AI 时代硬件安全未来的紧迫问题。 该利用链涉及两个漏洞及多项技术。完整 55 页技术报告将在 Apple 发布修复补丁后公布。攻击使用普通系统调用，实现从非特权用户到 root 的本地权限提升。

hackernews · quadrige · May 14, 18:25 · [社区讨论](https://news.ycombinator.com/item?id=48139219)

**背景**: MTE（内存标签扩展）是 ARMv9 硬件安全功能，为 16 字节内存粒添加 4 位分配标签，可检测 use-after-free 和缓冲区溢出漏洞。Apple 从 M1 芯片开始将 MTE 作为主要防御机制，耗时五年构建此保护。Anthropic 的 Mythos Preview 是专为安全研究设计的 AI 系统，此前已在所有主流操作系统和浏览器中发现漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.android.com/ndk/guides/arm-mte">Arm Memory Tagging Extension (MTE) | Android NDK | Android Developers</a></li>
<li><a href="https://www.npr.org/2026/04/11/nx-s1-5778508/anthropic-project-glasswing-ai-cybersecurity-mythos-preview">How AI is getting better at finding security holes : NPR</a></li>
<li><a href="https://simonwillison.net/2026/Apr/7/project-glasswing/">Anthropic’s Project Glasswing—restricting Claude Mythos to security ...</a></li>

</ul>
</details>

**社区讨论**: 评论显示兴奋与担忧并存：一些人称赞这一成就具有开创性，同时指出世界对 LLM 在安全领域的影响准备不足。其他人批评缺乏技术细节，有人询问漏洞如何绕过 MTE。还讨论了漏洞赏金价值（10 万至 150 万美元，取决于如何包装）以及关于 Apple 是否应在自己的代码中使用更多 Swift 的猜测。

**标签**: `#security-research`, `#apple-m5`, `#kernel-exploit`, `#memory-corruption`, `#mte-bypass`, `#ai-security`, `#zero-day`

---

<a id="item-2"></a>
## [RTX 5090 外接显卡搭配 M4 MacBook Air：游戏与 LLM 基准测试](https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/) ⭐️ 8.0/10

一项技术深入研究测试了在 M4 MacBook Air 上连接 RTX 5090 外接显卡时的游戏和本地 LLM 性能，显示出 AI 推理能力显著提升，但由于 OpenGL 问题也暴露了 Mac 游戏功能的局限性。 这很重要，因为它展示了 Apple Silicon Mac 外接显卡解决方案的潜力，特别是对于本地 AI 推理，同时也突出了由于图形 API 限制导致在 macOS 上游戏面临的持续挑战。

hackernews · allenleee · May 14, 15:47 · [社区讨论](https://news.ycombinator.com/item?id=48137145)

**背景**: eGPU（外接图形处理器）是一种用于计算机外部的显卡，通过 Thunderbolt 连接扩展内置图形处理能力。本地 LLM 推理是指在个人硬件上运行大型语言模型，而非远程服务器，提供隐私和定制化优势。Apple 官方表示 eGPU 需要基于 Intel 的 Mac，并推荐 AMD 显卡而非 NVIDIA。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/en-us/102363">Use an external graphics processor with your Mac - Apple Support</a></li>
<li><a href="https://www.computerhope.com/jargon/e/egpu.htm">What Is an eGPU ( External Graphics Processing Unit)?</a></li>
<li><a href="https://prajnaaiwisdom.medium.com/what-is-local-llm-inference-a-beginners-guide-b31043768d4f">What Is Local LLM Inference? A Beginner’s Guide</a></li>

</ul>
</details>

**社区讨论**: The community discussion highlights mixed perspectives: some celebrate the technical achievement of getting RTX 5090 working with Apple Silicon, while others note this is a workaround since Apple officially states eGPUs don't work with Apple Silicon. Commenters particularly noted the LLM inference improvements as practically significant, while also discussing VM GPU passthrough limitations and the challenges of prompt processing speed on Macs.

**标签**: `#eGPU`, `#Apple Silicon`, `#RTX 5090`, `#LLM Inference`, `#Mac Gaming`

---

<a id="item-3"></a>
## [Bun 完成从 Zig 到 Rust 的大规模重写](https://github.com/oven-sh/bun/pull/30412) ⭐️ 8.0/10

重写包含了将 Zig 惯用法映射到 Rust 惯用法的详细说明，而且代码库已经使用了内部智能指针类型，可以与 Rust 等效类型一一对应。然而，维护者 Jarred 指出，Rust 无法捕获所有内存问题——持有引用时间过长导致的泄漏以及跨 JS 边界重新进入的情况仍然需要团队自行处理。 这表明对 Rust 在系统编程中的内存安全保证投下了信任票。这一转变可能会为 JavaScript 生态系统中的运行时安全性和可靠性树立新的标准，因为 Bun 现在已成为最大的 Rust 代码库之一，拥有超过 100 万行代码。

hackernews · Chaoses · May 14, 08:15 · [社区讨论](https://news.ycombinator.com/item?id=48132488)

**背景**: Bun 是一个快速的 JavaScript 运行时，最初使用 Zig 构建。Zig 是一种系统编程语言，设计作为 C 语言的通用改进版本。Zig 需要手动内存管理，而 Rust 则通过其所有权系统在编译时提供内存安全性，无需垃圾回收。此次重写利用了 Rust 的所有权模型来防止历来困扰系统软件的常见内存错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**社区讨论**: 社区成员注意到，此次重写需要大量准备工作，实际上已经准备了将 Zig 惯用法映射到 Rust 惯用法的详细说明。显示 10,428 个不安全代码块和超过 100 万行 Rust 代码的统计数据引发了赞赏和怀疑——一些开发者将 Bun 的规模与 Rust 编译器本身进行比较，质疑如此大的代码库是否能得到有效维护。维护者 Jarred 承认，虽然 Rust 消除了许多内存错误，但一些问题（如跨 JS 边界的引用生命周期问题）仍未解决。

**标签**: `#bun`, `#rust`, `#javascript-runtime`, `#zig`, `#memory-safety`, `#systems-programming`

---

<a id="item-4"></a>
## [Mullvad 出口 IP 可被用于用户指纹识别](https://tmctmt.com/posts/mullvad-exit-ips-as-a-fingerprinting-vector/) ⭐️ 7.0/10

安全研究人员发现，Mullvad VPN 的出口 IP 是根据 WireGuard 密钥确定性分配的，而不是随机分配的，这使得可以跨不同连接和服务器对用户进行指纹识别。 这破坏了用户的隐私预期，因为同一用户可以在不同的 Mullvad 服务器连接中被识别，从而可能将他们在不同网站上的活动关联起来，并 enable 去匿名化攻击。 出口 IP 由 WireGuard 密钥决定，官方应用用户的密钥每 1-30 天轮换一次，但第三方客户端的密钥永远不会轮换。这创造了一个持久的指纹，当 IP 范围重叠时，可以以超过 99%的置信度关联会话。

hackernews · RGBCube · May 15, 02:35 · [社区讨论](https://news.ycombinator.com/item?id=48143880)

**背景**: VPN 出口节点是用户设备与互联网之间的最终网关，掩盖用户的真实 IP 地址。WireGuard 是一种现代的快速 VPN 协议，使用加密密钥进行身份验证。确定性 IP 分配意味着相同的输入（WireGuard 密钥）总是产生相同的输出（出口 IP），而随机分配则提供更好的匿名性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WireGuard">WireGuard - Wikipedia</a></li>
<li><a href="https://fastercapital.com/content/Exit-Node--Securing-Your-Online-Privacy--The-Role-of-Exit-Nodes-in-VPNs.html">Exit Node: Securing Your Online Privacy: The Role of Exit ...</a></li>

</ul>
</details>

**社区讨论**: 评论显示了对统计声明和 VPN 与 Tor 匿名性预期的争论。一些用户认为 VPN 从未被设计为提供与 Tor 相当的匿名性，而其他人则批评 99%置信度的说法缺乏支持。一个值得注意的观点将其比作「如果我是情报机构，我会如何设计 VPN」。

**标签**: `#vpn-security`, `#privacy`, `#mullvad`, `#fingerprinting`, `#wireguard`

---

<a id="item-5"></a>
## [为保护隐私移除丰田 RAV4 的调制解调器和 GPS](https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/) ⭐️ 7.0/10

这凸显了人们对汽车数据收集日益增长的担忧，并表明一些车主正在采取极端的物理措施来保护他们的隐私。高参与度（744 分，407 条评论）表明，这对注重隐私的车主来说是一个重要的关注点。 研究人员从车辆中物理移除了硬件组件。社区评论显示，虽然蓝牙连接允许汽车使用手机的流量进行数据传输，但使用有线 USB 连接的 CarPlay 不会这样做。然而，CarPlay 和 Android Auto 都会独立采集自己的车辆遥测数据，这意味着即使移除硬件后，隐私保护斗争仍在继续。

hackernews · arkadiyt · May 14, 17:08 · [社区讨论](https://news.ycombinator.com/item?id=48138136)

**背景**: 像 2024 款 RAV4 这样的现代汽车配备了嵌入式蜂窝调制解调器（远程信息处理单元），可以持续将车辆数据传回制造商。这些数据可能包括位置、驾驶行为、速度、加速度模式以及诊断信息。隐私研究人员对数据收集的范围以及谁可以访问这些数据（包括可能与保险公司共享）表示担忧。

**社区讨论**: 讨论揭示了重要的细微差别：评论者指出，即使移除调制解调器后，蓝牙连接仍然可以通过手机传输遥测数据，而 USB/CarPlay 可以避免这个问题。然而，一位评论者指出，CarPlay 和 Android Auto 本身也会采集车辆遥测数据。一些用户有不同的动机，比如修复 GPS/指南针问题。其他人提到福特汽车的远程信息处理保险丝可以更容易地拆卸作为替代方案。

**标签**: `#privacy`, `#hardware`, `#automotive`, `#security`, `#IoT`

---

<a id="item-6"></a>
## [DS4：本地运行 DeepSeek 4 的专用运行时发布](https://antirez.com/news/165) ⭐️ 7.0/10

Antirez 发布了 DS4（DwarfStar4），这是一个专用的 LLM 推理运行时，支持 Metal、CUDA 和 ROCm 后端，可在本地运行 DeepSeek 4。 这使得开发者能够在消费级硬件上本地运行 DeepSeek 4，可能会以更低的价格匹配高端 AI 编程助手，挑战 Anthropic 等服务的商业模式。 该运行时需要 96GB 显存，Metal 是 MacBooks 的主要目标。CUDA 支持聚焦于 NVIDIA DGX Spark，而 ROCm 支持则在单独的社区分支中维护。它基于 llama.cpp 和 GGML 构建。

hackernews · caust1c · May 14, 22:29 · [社区讨论](https://news.ycombinator.com/item?id=48142108)

**背景**: DeepSeek V4 是一款 AI 编程助手模型，在代理编码基准测试中以更低成本匹配 GPT-5.5 和 Opus。ROCm 是 AMD 用于高性能计算和 AI 的 GPU 计算平台。Metal 是 Apple 设备上用于图形和计算任务的 GPU 框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/news/news260424">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>
<li><a href="https://github.com/ROCm/ROCm">GitHub - ROCm / ROCm : AMD ROCm ™ Software - GitHub Home</a></li>
<li><a href="https://developer.apple.com/technologies/">Technologies - Apple Developer</a></li>

</ul>
</details>

**社区讨论**: 用户对在本地运行高质量 AI 编程助手的可能性感到兴奋，有人指出它"令人惊讶地接近 Claude"，尽管速度较慢。有人讨论较慢/较便宜的模型是否能匹配高端服务，以及未来是否可以在 16GB RAM 等消费级硬件上运行。imatrix 量化被称赞为优于 OpenRouter 后端。

**标签**: `#llm-inference`, `#deepseek`, `#open-source`, `#local-ai`, `#hardware-acceleration`

---

<a id="item-7"></a>
## [Nginx-Rift：发现可导致远程代码执行的 18 年历史漏洞](https://github.com/DepthFirstDisclosures/Nginx-Rift) ⭐️ 7.0/10

此漏洞允许在广泛部署的 Web 服务器中进行未经身份验证的远程代码执行，可能影响数百万生产系统。18 年未被发现的潜伏期以及可用的工作漏洞利用程序使这成为安全团队的严重关切。 该漏洞利用需要特定的前提条件：重写指令的替换字符串中包含问号，随后是指向未命名正则表达式捕获组（例如$1、$2）的 set 指令。已发布的 POC 假设 ASLR 被禁用，但研究人员声称可以绕过 ASLR。缓解措施包括使用命名捕获代替未命名捕获。

hackernews · hetsaraiya · May 14, 17:17 · [社区讨论](https://news.ycombinator.com/item?id=48138268)

**背景**: NGINX 是全球最受欢迎的 Web 服务器之一，为大量网站和应用程序提供支持。该漏洞存在于重写模块中，该模块常用于 URL 操作和重定向。ASLR（地址空间布局随机化）是一种内存保护技术，通过随机化内存地址来增加漏洞利用的难度。正则表达式中的命名捕获允许按名称而非位置引用匹配的组。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/05/18-year-old-nginx-rewrite-module-flaw.html">18-Year-Old NGINX Rewrite Module Flaw Enables Unauthenticated...</a></li>
<li><a href="https://www.picussecurity.com/resource/blog/nginx-rift-cve-2026-42945-critical-heap-buffer-overflow-vulnerability-explained">NGINX Rift: CVE-2026-42945 Critical Heap Buffer Overflow Vulnerability Explained - Picus Security</a></li>
<li><a href="https://logicity.in/en/blog/18-year-old-nginx-bug-allows-dos-and-remote-code-execution">18-Year-Old NGINX Bug Allows DoS and Remote Code... | Logicity</a></li>

</ul>
</details>

**社区讨论**: 安全专家正在就严重性展开辩论，一些人指出该漏洞利用需要特定的配置条件。然而，研究人员强调，ASLR 绕过很可能实现，不应忽视该漏洞。一位评论者询问了关于 Caddy（Go 语言编写）或 Jetty（Java 编写）等内存安全替代方案的问题，指出这些方案也有自己的漏洞历史。

**标签**: `#security`, `#nginx`, `#vulnerability`, `#exploit`, `#f5`

---

<a id="item-8"></a>
## [Codex 现已在 ChatGPT 移动应用中可用](https://openai.com/index/work-with-codex-from-anywhere/) ⭐️ 7.0/10

OpenAI 的 Codex 编码智能体现已在 ChatGPT 移动应用中可用，让用户可以随时随地进行 AI 辅助编程，并提供免费套餐选项。 这将 AI 编码工具的访问范围扩展到桌面以外，可能使 PC 访问受限地区的开发者受益，并能在移动中快速进行代码审查或调整工作方向。 Codex 在桌面应用和 CLI 上都可以免费使用——用户只需登录 ChatGPT 账户即可。需要注意的警告是用户的互动可能会被用于训练。一些用户报告称，与使用键盘相比，移动端使用会导致对智能体的引导效果较差，可能会产生更多技术债务。

hackernews · mikeevans · May 14, 20:06 · [社区讨论](https://news.ycombinator.com/item?id=48140529)

**背景**: OpenAI Codex 是一个 AI 驱动的编码智能体，可自动化软件工程任务，使开发者能够将功能开发、代码重构、调试和测试生成等活动委托给它。这代表了让全球开发者更便捷地使用 AI 辅助编程的重要一步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/OpenAI_Codex">OpenAI Codex</a></li>
<li><a href="https://www.reddit.com/r/OpenAI/comments/1n5iqqj/openai_nailed_it_with_codex_for_devs/">openAI nailed it with Codex for devs - Reddit</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一。一些人认为免费套餐令人惊喜且有价值，特别指出它可能使 PC 访问受限地区（如尼日利亚）的开发者受益。其他人则更为谨慎，有用户报告称由于屏幕较小且缺乏键盘，移动端编码的效果不如桌面端，可能导致更多代码变动。从手机上解除或重定向长时间运行的工作被认为可能被低估了。

**标签**: `#OpenAI`, `#Codex`, `#AI coding`, `#mobile development`, `#developer tools`

---

<a id="item-9"></a>
## [arXiv 实施幻觉引用一年禁令](https://twitter.com/tdietterich/status/2055000956144935055) ⭐️ 7.0/10

arXiv 宣布了一项新政策，对含有幻觉引用的论文作者实施一年禁投处罚。幻觉引用是指由 LLM 生成但作者未核实的不存在引用。 禁投适用于幻觉引用、留在文本中的 LLM 元注释（如"请替换为真实数据"）以及其他未核实的 AI 生成内容。一年期禁投结束后，作者的后续投稿必须先被同行评审的期刊接收，才能在 arXiv 上发布。无论内容如何生成，作者都承担全部责任。

hackernews · gjuggler · May 14, 20:39 · [社区讨论](https://news.ycombinator.com/item?id=48140922)

**背景**: 幻觉引用是指看起来真实但指向不存在论文的伪造引用。随着 LLM 的广泛采用，研究记录显示在 arXiv、bioRxiv、SSRN 和 PubMed Central 等主要科学数据库中这类无效引用急剧增加。《自然》的一项分析表明，2025 年可能有数万篇出版物包含 AI 生成的无效引用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nature.com/articles/d41586-026-00969-z">Hallucinated citations are polluting the scientific ... - Nature</a></li>
<li><a href="https://arxiv.org/abs/2605.07723">[2605.07723] LLM hallucinations in the wild: Large-scale ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体上表示支持，评论者认为这一禁令对于维护科学诚信是恰当的——arXiv 是一种特权而非权利。有些人担心引用管理工具难以生成正确的 BibTeX 条目。其他人指出，LLM 批评者正面临 AI 支持者的反对，一些人反对任何阻碍 LLM 快速采用的措施。

**标签**: `#arXiv`, `#academic-publishing`, `#research-integrity`, `#LLM`, `#policy`

---

<a id="item-10"></a>
## [安大略省审计员发现医生使用的 AI 笔记工具经常出现基本事实错误](https://www.theregister.com/ai-ml/2026/05/14/ontario-auditors-find-doctors-ai-note-takers-routinely-blow-basic-facts/5240771) ⭐️ 7.0/10

这一点非常重要，因为 AI 医疗记录员正在被医疗系统广泛采用，医疗文档中的事实错误可能导致误诊、不当治疗和患者安全受损。这些发现突显了 AI 能力与医疗环境所需精度之间的关键差距。 审计特别指出了将医患对话转换为临床笔记的 AI 系统存在问题。这些 AI 记录员使用环境监听技术生成文档，但它们经常产生幻觉或误解信息，可能包含从未讨论过的错误诊断或症状。

hackernews · sohkamyung · May 14, 22:37 · [社区讨论](https://news.ycombinator.com/item?id=48142188)

**背景**: AI 医疗记录技术（如 DeepScribe、Sunoh.ai 和 MarianaAI）使用环境监听将临床对话实时转换为文档。研究已识别出三种类型的 AI 幻觉：输入冲突、上下文冲突和事实冲突，所有这些都可能破坏医疗环境的信任和效能。研究表明，医疗领域的 AI 幻觉可能导致误诊和不当治疗。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.deepscribe.ai/">DeepScribe AI Medical Scribe | Built for Specialty Care</a></li>
<li><a href="https://www.eclinicalworks.com/sunoh-ai-medical-scribe-technology-for-clinical-documentation/">Sunoh. ai - Medical AI Scribe Technology for Clinical Documentation</a></li>
<li><a href="https://www.medscape.com/viewarticle/ai-hallucinations-are-changing-medicine-should-we-worry-2025a1000647">AI ‘Hallucinations’ Are Changing Medicine — Should We Worry?</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了个人经历，证实了人们对 AI 准确性的担忧。一位评论者描述了 AI 摘要错误地声称他们被诊断为骨质疏松症，而实际上他们患有跑步者膝。另一位指出，工作中的 LLM 笔记记录员承诺了一些会议上从未实际说过的话。总体而言，讨论强调人们普遍认为 AI 输出需要仔细验证，特别是在医疗等敏感领域。

**标签**: `#ai-limitations`, `#healthcare`, `#hallucination`, `#medical-technology`, `#audit-findings`

---

<a id="item-11"></a>
## [MIT 校长科恩布鲁斯谈资金与人才输送危机](https://president.mit.edu/writing-speeches/video-transcript-message-president-kornbluth-about-funding-and-talent-pipeline) ⭐️ 7.0/10

MIT 校长科恩布鲁斯就学术界的资金挑战和人才输送问题发表了讲话，引发了关于博士前景、研究经费下降和高等教育未来的广泛讨论。 这很重要，因为它突出了影响科技人才输送的学术系统性危机，尽管 80%的近期博士毕业生进入学术界是为了追求学术生涯，但许多人正在考虑离开。该讨论反映了人们对研究经费下降和大学可持续性的更广泛担忧。 目前科学博士的中位学习时间为 6 年，工作繁重但薪酬相对较低，考虑到当前市场，就业前景也很困难。未获得资助的学生接受录取的可能性较低，从而形成了人才输送的恶性循环。

hackernews · dmayo · May 14, 14:51 · [社区讨论](https://news.ycombinator.com/item?id=48136262)

**背景**: MIT 校长科恩布鲁斯的讲话涉及高等教育中研究资金与人才输送的交叉点。讨论涵盖了学术界面临的挑战，包括资助成功率下降、博士生的经济负担以及传统学术模式的可持续性。这正值大学面临越来越大的压力，需要证明学生的就业能力和投资回报率。

**社区讨论**: 评论显示人们对学术界深感失望，许多人指出 80%的近期博士毕业生正在考虑离开。一些人将这视为破碎系统的代际重置，而另一些人则认为博士进入工业界并非浪费——特别是在纳米制造和半导体等领域。印度和中国的国际视角增加了细微差别，中国在高等教育中的崛起地位也值得关注。

**标签**: `#academia`, `#higher-education`, `#funding`, `#talent-pipeline`, `#research`

---

<a id="item-12"></a>
## [Anthropic 推出面向小企业的 Claude 套餐](https://www.anthropic.com/news/claude-for-small-business) ⭐️ 7.0/10

Anthropic 推出了 Claude for Small Business，将 Claude 接入 Intuit QuickBooks、PayPal、HubSpot、Canva、Docusign、Google Workspace 和 Microsoft 365，提供 15 个可直接运行的工作流和 15 项技能，覆盖财务、销售、营销、人力资源和客服等任务。 这次发布代表了 Anthropic 向小企业市场的战略进军，与其他面向企业客户的 AI 助手展开竞争。通过与主流商业工具的集成以及对实际工作流的关注，可以让技术资源有限的小公司更容易使用人工智能。 该服务基于 Anthropic 的代理 AI 系统 Claude Cowork 运行，可执行包括研究综合、文档准备和文件管理在内的多步骤知识工作。在发送、发布或付款前需要用户批准。Team 和 Enterprise 版本默认不使用客户数据进行模型训练。

telegram · zaihuapd · May 14, 12:41

**背景**: Claude Cowork 是 Anthropic 的知识工作产品，将 Claude Code 的代理能力带到桌面应用程序中。它可以代表用户执行多步骤任务，例如通过提取会议笔记和项目文档来起草报告。此次发布扩展了 Anthropic 针对企业客户之外不同市场细分领域的战略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/product/claude-cowork">Claude Cowork | Anthropic ’s agentic AI for knowledge work</a></li>
<li><a href="https://claude.com/product/cowork">Cowork : Claude Code power for knowledge... | Claude by Anthropic</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#Claude AI`, `#Small Business`, `#AI Products`, `#Business Automation`

---

<a id="item-13"></a>
## [OpenAI 因未经同意向 Meta 和 Google 分享用户数据被起诉](https://futurism.com/artificial-intelligence/openai-personal-information-meta-google) ⭐️ 7.0/10

一宗在加州提起的集体诉讼指控 OpenAI 在未获适当同意的情况下，使用 Meta Pixel 和 Google Analytics 追踪工具将用户聊天查询、电子邮件地址和用户 ID 分享给 Meta 和 Google。 这宗诉讼对 AI 公司的数据实践提出了重大法律挑战，可能为 AI 时代用户数据保护树立先例。如果胜诉，可能迫使整个行业就第三方数据共享的同意机制做出重大改变。 诉讼声称数据传输是通过安装在 OpenAI 平台上的 Meta Pixel 和 Google Analytics 追踪像素进行的，涉嫌违反加州的《隐私侵犯法》和《电子通信隐私法》。OpenAI 尚未回应置评请求。

telegram · zaihuapd · May 15, 03:45

**背景**: Meta Pixel（原名 Facebook Pixel）是一种 JavaScript 追踪代码，用于收集网站上的用户活动数据并与 Meta 的广告平台共享以优化广告投放。Google Analytics 执行类似的追踪功能。这两种工具都可以收集个人标识符和行为数据。加州拥有美国最严格的隐私法，包括《加州消费者隐私法》（CCPA），该法要求公司披露数据收集并获得同意。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.facebook.com/business/tools/meta-pixel/">Meta Pixel: Measure, Optimize & Retarget Ads on Facebook ...</a></li>
<li><a href="https://support.google.com/analytics/answer/9213390?hl=en">Measure activity across platforms with User-ID - Analytics Help</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#privacy`, `#legal`, `#Meta`, `#Google`, `#AI regulation`

---

<a id="item-14"></a>
## [硬盘固件黑客技术深度探索](https://icode4.coffee/?p=1465) ⭐️ 6.0/10

一篇技术博客文章探讨了硬盘固件黑客技术，展示了硬盘固件的反向工程和修改方法。 此研究揭示了存储设备中的关键安全漏洞，展示了攻击者如何可能利用硬盘固件植入持久性恶意软件或进行数据窃取。 文章深入探讨了针对硬盘的固件反向工程技术，社区评论还补充了相关案例，包括三星 840 EVO 固件反编译和 SSD 混淆绕过方法。

hackernews · jsploit · May 14, 16:19 · [社区讨论](https://news.ycombinator.com/item?id=48137553)

**背景**: 硬盘固件是控制硬盘操作的低级软件，包括数据读写、错误校正和硬件管理。固件修改可以让攻击者获得深层的系统访问权限，即使重装操作系统也无法清除。研究正值人们对供应链安全和硬件级威胁日益关注的背景下进行。

**社区讨论**: 评论强调了相关的安全问题：一位用户描述了使用 seccomp 在固件更新期间拦截解密后的固件来绕过 SSD 固件加密，另一位提到三星 840 EVO 固件在被三星加密之前的反编译情况。用户还讨论了 Red Balloon 公司面试 CTF 中涉及的物理硬盘以及廉价磁盘控制器固件修补的话题。

**标签**: `#hardware-security`, `#firmware`, `#reverse-engineering`, `#storage`, `#security-research`

---

<a id="item-15"></a>
## [美国批准英伟达 H200 芯片对约 10 家中国企业销售](https://www.reuters.com/business/retail-consumer/us-clears-h200-chip-sales-10-china-firms-nvidia-ceo-looks-breakthrough-2026-05-14/) ⭐️ 6.0/10

美国商务部已批准约 10 家中国企业购买英伟达 H200 芯片，买家包括阿里巴巴、腾讯、字节跳动和京东等。联想和富士康等分销商也获得许可，单一客户最多可购买 7.5 万颗芯片。 这一批准标志着中美科技关系的重要进展，因为 H200 是目前最先进的人工智能加速器之一。该决定反映了地缘政治紧张局势与半导体行业商业利益之间持续的权衡。 尽管获得批准，但目前尚未有任何交付完成，部分中国企业在北京方面的指导下转趋谨慎。黄仁勋此次访华被视为推动交易落地的重要尝试。

telegram · zaihuapd · May 14, 08:57

**背景**: 英伟达 H200 基于 Hopper 架构，代表着对 H100 的重大升级。它是首款提供 141 GB HBM3e 内存的 GPU，带宽达 4.8 TB/s，容量几乎是 H100 的两倍，内存带宽增加 1.4 倍。这使其特别适合生成式人工智能和大型语言模型工作负载。美国在持续的技术竞争中一直对先进芯片保持出口管制，这给英伟达在其最大市场之一的中国带来了复杂挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">NVIDIA H200 GPU</a></li>
<li><a href="https://www.trgdatacenters.com/resource/nvidia-h200-vs-h100/">NVIDIA GPUs H200 vs. H100 - A detailed comparison guide | TRG Datacenters</a></li>
<li><a href="https://vast.ai/article/nvidia-h100-vs-h200-two-hopper-based-heavyweights">NVIDIA H100 vs. H200: Two Hopper-based Heavyweights</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#US-China Tech Relations`, `#AI Chips`, `#Geopolitics`, `#Export Controls`

---

<a id="item-16"></a>
## [发达国家肥胖率上升趋稳，中低收入国家仍在加速](https://www.nature.com/articles/s41586-026-10383-0) ⭐️ 6.0/10

一项发表于《自然》杂志、覆盖 200 个国家、2.32 亿人、跨越 44 年（1980-2024 年）的研究发现，自 2000 年代以来，高收入国家的肥胖率已趋于稳定，而中低收入国家的肥胖率仍在持续稳定或加速上升，部分国家的肥胖率已反超发达国家。 这一发现标志着全球健康趋势的重大逆转，对世界公共卫生政策具有重要意义。研究表明，影响食物可得性和负担能力的社会、经济及技术因素可能帮助高收入国家遏制了肥胖率的上升，而中低收入国家仍需政策干预。 研究显示，高收入国家儿童青少年肥胖率的上升自 1990 年代起开始减速，意大利、葡萄牙、法国等在 2000 年代后甚至出现小幅下降。成人肥胖率的上升随后也呈现类似平台期，比青少年趋势晚约十年。

telegram · zaihuapd · May 14, 09:45

**背景**: 肥胖是一个重要的全球健康问题，与糖尿病、心血管疾病和某些癌症的风险增加相关。世界卫生组织已将肥胖确定为全球范围内日益严重的流行病。这项研究提供了近 50 年来几乎所有国家的综合流行病学数据，使其成为迄今为止最广泛的全球肥胖趋势分析之一。

**标签**: `#public-health`, `#epidemiology`, `#global-health`, `#obesity`, `#research`

---

<a id="item-17"></a>
## [华为、江淮与斯特兰蒂斯洽谈玛莎拉蒂新能源车合作](https://eu.36kr.com/zh/p/3807764479680774) ⭐️ 6.0/10

华为、江淮汽车与斯特兰蒂斯集团正就共同打造玛莎拉蒂品牌新能源车展开洽谈，华为提供核心技术，江淮负责研发生产，玛莎拉蒂提供造型设计与品牌背书。 这一合作代表了外国传统品牌与中国电动汽车技术提供商合作加速电动化转型的重要趋势，传统豪华车企在向电动汽车转型过程中面临挑战。 首款车型目前处于造型设计阶段，计划于明年下半年量产。国内版本归属华为尊界品牌，海外版本悬挂玛莎拉蒂车标。自去年年初以来研发工作已在进行，但尚未签署正式协议。

telegram · zaihuapd · May 14, 11:15

**背景**: 斯特兰蒂斯是由菲亚特克莱斯勒与标致雪铁龙集团合并成立的全球最大汽车集团之一，旗下拥有玛莎拉蒂、Jeep、法拉利等品牌。华为鸿蒙智行一直在快速扩展其电动汽车合作伙伴网络，尊界品牌代表其超豪华定位。玛莎拉蒂面临销量压力，需要加速电动化转型以满足更严格的排放法规。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/斯泰蘭蒂斯">斯 特 兰 蒂 斯 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.stellantis.com/">Official Global Website | Stellantis</a></li>
<li><a href="https://auto.news18a.com/news/storys_255822.html">所有人都在吹 尊 界 200...</a></li>

</ul>
</details>

**标签**: `#新能源汽车`, `#华为`, `#玛莎拉蒂`, `#电动汽车`, `#汽车合作`, `#江淮汽车`

---

<a id="item-18"></a>
## [DeepSeek 对话系统会话隔离漏洞可泄露用户对话](https://github.com/deepseek-ai/DeepSeek-R1/issues/840) ⭐️ 6.0/10

DeepSeek 的对话系统存在会话隔离漏洞，攻击者在全新的空对话中仅发送未闭合的<think>字符串，模型即会返回其他用户的对话历史片段，可能泄露代码、密钥、隐私等敏感信息。 这代表着一个广泛使用的人工智能平台的严重隐私泄露，因为它将机密用户数据暴露给未授权方，并破坏了用户对聊天系统会话隔离的基本信任。 该漏洞同时影响 DeepSeek Web 和 API 接口。报告者 cancat2024 于 2026 年 5 月 11 日晚间以负责任的态度提交了报告，未利用漏洞获取或传播他人隐私数据。

telegram · zaihuapd · May 14, 13:15

**背景**: 会话隔离是多用户系统的基本安全原则，确保一个用户的数据对其他用户不可访问。<think>标签是 DeepSeek 推理模型用于展示模型内部思考过程的部分。提示词注入是一种通过对抗性提示工程来操纵人工智能模型的已知安全漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://github.com/vllm-project/vllm/discussions/12708">Nested `` and `` tag in deepseek-r1 reasoning parser · vllm-project/vllm · Discussion #12708</a></li>

</ul>
</details>

**社区讨论**: 社区成员对该漏洞表示怀疑，一位群友认为这可能是幻觉，因为第三方部署的版本也有类似现象。

**标签**: `#security vulnerability`, `#DeepSeek`, `#privacy`, `#session isolation`, `#AI safety`

---

<a id="item-19"></a>
## [随着跨平台工具改进，技术锁定效应减弱](https://simonwillison.net/2026/May/14/not-so-locked-in/#atom-everything) ⭐️ 5.0/10

Simon Willison 分享了一个案例，一家公司使用编码代理将其原有的 iPhone 和 Android 应用重写为 React Native，并指出 React Native 已经大幅改进，如果需要还可以移植回原生代码。 这反映了一个更广泛的趋势，即技术锁定效应正在减弱，因为跨平台工具已经成熟，编码代理使切换平台变得更加容易。开发者不再需要担心被单一技术栈锁定。 该公司选择 React Native 是因为它现在能够满足他们的所有需求，尽管编码代理使分别开发 iOS/Android 应用的成本更低。Mitchell Hashimoto 将 Bun 从 Zig 迁移到 Rust 的例子说明，即使是编程语言本身也不再是一种锁定形式。

rss · Simon Willison · May 14, 22:53

**背景**: React Native 是一个用于使用 JavaScript 和 React 构建跨平台移动应用的框架。编码代理是能够自主编写和修改代码的人工智能工具。技术锁定的概念是指开发者变得依赖特定技术，切换到替代方案将非常昂贵或耗时。以前，选择编程语言或平台通常意味着永久锁定在该生态系统中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#software-development`, `#react-native`, `#technology-lock-in`, `#coding-agents`, `#cross-platform-development`

---

<a id="item-20"></a>
## [Mitchell Hashimoto：AI 时代编程语言日益变得可替代](https://simonwillison.net/2026/May/14/mitchell-hashimoto/#atom-everything) ⭐️ 5.0/10

Mitchell Hashimoto 评论说编程语言已变得越来越可替代，他以 Bun 最近从 Zig 重写为 Rust 为例证，并暗示 Bun 可以在一两周内移植到“任何他们想要的语言”。 这一观点挑战了将编程语言视为战略性锁定资产的传统看法。如果人工智能工具能使语言切换变得微不足道，这可能会重塑开发者选择技术的方式以及公司在特定语言生态系统中的投资方式。 Hashimoto 特别提到 Bun 能够在一两周内用任何语言重写，这证明了语言的可替代性。他将这视为“有趣”而非正面或负面，并指出 Rust“有用直到不再有用时可以被抛弃”。

rss · Simon Willison · May 14, 22:31

**背景**: Mitchell Hashimoto 是广泛使用的开发者工具（包括 Terraform 和 Vagrant）的创作者，也是 HashiCorp 的联合创始人。Bun 是一个 JavaScript 运行时，最初用 Zig 编写，最近宣布移植到 Rust。这一观察与人工智能驱动的代码生成使跨多种编程语言工作变得更容易的更广泛趋势相关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>

</ul>
</details>

**标签**: `#programming-languages`, `#rust`, `#zig`, `#developer-tools`, `#ai-impact`

---

<a id="item-21"></a>
## [Datasette IP 限流插件发布](https://simonwillison.net/2026/May/14/datasette-ip-rate-limit/#atom-everything) ⭐️ 5.0/10

Simon Willison 发布了 datasette-ip-rate-limit 0.1a0，这是一款可配置的 IP 限流插件，为 Datasette 构建，在 Codex AI（GPT-5.5 xhigh）的帮助下开发完成，现已部署在 datasette.io 上用于阻止恶意爬虫。 这解决了 Datasette 用户面临的恶意爬虫问题，展示了 AI 工具如何加速插件开发。其生产环境配置为面临类似问题的用户提供了模板。 该插件支持按路径配置规则，demo-databases 的窗口期为 60 秒，最大请求数为 60 次，封锁时长为 20 秒。它使用 Fly-Client-IP 头进行 IP 检测，这是由托管 datasette.io 的 Fly.io 平台提供的。

rss · Simon Willison · May 14, 04:10

**背景**: Datasette 是一个用 Python 构建的开源数据探索和发布工具。它支持插件系统来扩展功能。Fly-Client-IP 头由 Fly.io 的代理添加，用于识别原始客户端 IP 地址，但必须谨慎使用以避免欺骗问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>
<li><a href="https://fly.io/docs/networking/request-headers/">Request headers · Fly Docs</a></li>

</ul>
</details>

**标签**: `#Datasette`, `#Rate Limiting`, `#Python`, `#Plugins`, `#AI-Assisted Development`

---

<a id="item-22"></a>
## [Boris Mann 批评「11 个 AI 智能体」说法毫无意义](https://simonwillison.net/2026/May/13/boris-mann/#atom-everything) ⭐️ 5.0/10

Boris Mann 批评「11 个 AI 智能体」这一说法毫无意义，将其比作说「我有 11 个电子表格」或「11 个浏览器标签页」——数字本身并不能传达实际工作或能力的信息。 这一批评揭示了 AI 讨论中术语模糊的问题，「智能体」已成为缺乏明确定义的营销术语。这很重要，因为精确的术语对于有意义的 AI 能力、局限性及市场宣传的讨论至关重要。 Mann 的对比指出，简单地计算「AI 智能体」数量并不能提供有意义的信息——就像计算电子表格或浏览器标签页的数量无法说明实际做什么工作或任务的复杂性。

rss · Simon Willison · May 13, 16:15

**背景**: AI 智能体是使用 AI 代表用户追求目标并完成任务的软件系统。「AI 智能体」一词可追溯到 1990 年代的研究，研究员 Andrew Ng 在 2024 年向更广泛的受众推广了「智能体」的概念。定义的模糊性使「AI 智能体」成为一个笼统的营销术语，不同公司用它来描述各种类型的自主 AI 系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://cloud.google.com/discover/what-are-ai-agents">What are AI agents? Definition, examples, and types</a></li>
<li><a href="https://github.com/resources/articles/what-are-ai-agents">What are AI agents ? · GitHub</a></li>

</ul>
</details>

**标签**: `#ai-agents`, `#ai`, `#agent-definitions`, `#terminology`, `#discourse`

---

<a id="item-23"></a>
## [马化腾承认腾讯 AI 初期缺乏竞争力](https://t.me/zaihuapd/41377) ⭐️ 5.0/10

在腾讯股东大会上，CEO 马化腾回应了关于腾讯 AI 是否落后的问题，承认公司早期 AI 基础能力并不突出。他用了一个比喻：去年一度以为已经上船，后来发现船漏水，现在算是站上去了，但还坐不下去。 这一承认为了解腾讯与字节跳动、阿里巴巴等竞争对手相比的 AI 定位提供了难得的视角。这表明腾讯采取了更谨慎、稳健的 AI 发展方式，而非激进扩张，这可能影响腾讯未来几年的竞争战略。 马化腾特别提到，腾讯近年来通过人才建设、团队管理和内部培训来补短板。他强调，腾讯不会因他人布局就盲目跨过去抢地盘，而会结合自身优势稳步推进。

telegram · zaihuapd · May 14, 06:52

**背景**: 这次股东大会上的发言反映了腾讯在生成式 AI 竞争中寻求追赶的更广泛 AI 战略。与一些竞争对手发布激进的 AI 公告不同，腾讯采取了更谨慎的方式，专注于建设基础能力，而非竞相发布面向消费者的 AI 产品。

**标签**: `#Tencent`, `#AI Strategy`, `#Corporate News`, `#Pony Ma`, `#Chinese Tech`

---

<a id="item-24"></a>
## [谷歌测试新 Gmail 账户 5GB 免费存储](https://www.androidauthority.com/google-gmail-5gb-free-storage-test-3667002/) ⭐️ 5.0/10

这一变化可能影响数百万依赖 Gmail 免费存储来存放邮件和 Google Drive 文件的新用户。如果永久实施，将代表谷歌免费服务产品的重大转变，并可能推动更多用户转向付费存储方案。 该测试似乎是一项 A/B 测试，而非确认的永久性变更。谷歌尚未正式宣布这一政策转变，支持页面仍显示 15GB 为标准免费存储限额。目前尚不清楚这是区域性测试还是全球性政策变更。

telegram · zaihuapd · May 14, 14:07

**背景**: 自 2014 年以来，谷歌一直提供 15GB 的免费存储空间，在 Gmail、Google Drive 和 Google Photos 之间共享。这一存储池一直是所有谷歌账户用户的标准配置。当前的测试将新账户的存储空间减少到 5GB，除非用户通过手机号码验证身份，此举可能用于反垃圾邮件或数据收集目的。

**标签**: `#Google`, `#Gmail`, `#Cloud Storage`, `#Policy Change`, `#A/B Testing`

---

<a id="item-25"></a>
## [京东上线 AI 硬件自营专区 销售 RTX 5090 及受制裁 H100 芯片](https://u.jd.com/HaDkFMa) ⭐️ 5.0/10

RTX 5090 涡轮版被描述为无阉割的全球统一规格。RTX PRO 6000 面向专业渲染和数据中心应用。消息来源是 Telegram 优惠频道而非权威科技新闻媒体，使得独立验证较为困难。

telegram · zaihuapd · May 14, 15:15

**背景**: 美国从 2022 年开始对 NVIDIA 的 H100 等先进 AI 芯片实施出口限制，要求出口中国需获得特别许可。H100 因其高计算能力被特别针对，这些能力对 AI 训练很有价值。2025 年有报道称走私团伙试图向中国出口价值 1.6 亿美元的 H100 和 H200 GPU。NVIDIA 的 Blackwell 架构是 Hopper 和 Ada Lovelace 的继任者，RTX PRO 6000 配备 96GB GDDR7 内存。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2025/12/31/160-million-export-controlled-nvidia-gpus-allegedly-smuggled-to-china.html">$160 million export-controlled Nvidia GPUs allegedly ... - CNBC</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/">The Engine Behind AI Factories | NVIDIA Blackwell Architecture</a></li>
<li><a href="https://www.pny.com/en-eu/nvidia-rtx-pro-6000-blackwell-ws">NVIDIA RTX PRO 6000 Blackwell Workstation Edition | Professional GPUs | pny.com</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#AI hardware`, `#China tech`, `#export controls`, `#JD.com`

---

<a id="item-26"></a>
## [ChatGPT Android 版拆解发现 Codex 手机远控功能](https://t.me/zaihuapd/41388) ⭐️ 5.0/10

ChatGPT Android 版 1.2026.125 的 APK 被拆解后发现多处字符串，显示 OpenAI 正在为 Codex 开发手机远程控制桌面会话的功能，支持在手机上查找和重连远程会话。 这一发现表明 OpenAI 正在将 Codex 从 CLI 工具扩展到跨设备体验，可能让开发者能够通过移动设备远程控制编码会话，这可能会显著改变开发者的工作方式。 该功能要求桌面客户端与移动设备登录同一账号才能重连会话。目前仍处于早期开发阶段，没有可用的预览版本，也没有公布正式上线时间。

telegram · zaihuapd · May 14, 21:48

**背景**: OpenAI Codex 是 OpenAI 开发的 AI 驱动编码代理，旨在自动化软件工程任务。Codex CLI 在本地计算机上运行，而手机远程控制功能将把其功能扩展到移动设备。APK 拆解是一种常见技术，安全研究人员和开发者通过反编译 Android 应用来发现隐藏功能、字符串和潜在的未来功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI</a></li>
<li><a href="https://github.com/openai/codex">GitHub - openai/codex: Lightweight coding agent that runs in ...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#ChatGPT`, `#Codex`, `#reverse-engineering`, `#mobile-remote-control`

---

<a id="item-27"></a>
## [AMD FSR 4.1 将于 7 月支持 RX 7000，2027 年初支持 RX 6000](https://videocardz.com/newz/amd-fsr-upscaling-4-1-officially-coming-to-radeon-rx-7000-gpus-in-july-rx-6000-in-2027) ⭐️ 5.0/10

AMD 确认，其基于机器学习的 FSR 超分技术 FSR 4.1 将于 2025 年 7 月向 Radeon RX 7000 系列（RDNA 3）开放，发布时即支持超过 300 款游戏。RX 6000 系列（RDNA 2）将于 2027 年初获得 FSR 4.1 支持。 这一公告意义重大，因为它将 AMD 最新的 AI 超分技术带入上一代 RDNA 3 GPU。不过，RDNA 2 的支持时间延长至 2027 年，凸显了将机器学习模型移植到具有不同 AI 加速器架构的老旧硬件所面临的技术挑战。 FSR 4.1 专门针对第一代 AI 加速器使用 INT8 指令开发，这与 RX 9000 系列 RDNA 4 架构使用的 FP8 方案不同。相比 FSR 4.0，该更新提升了锐度并减少了涂抹和模糊，同时优化了 Ultra Performance 模式和动态分辨率缩放模式。

telegram · zaihuapd · May 15, 04:57

**背景**: FSR（FidelityFX Super Resolution）是 AMD 应对 Nvidia DLSS 的解决方案，使用机器学习将低分辨率图像 upscale 到更高分辨率，以提升游戏性能。RDNA 3 是 AMD 用于 RX 7000 系列的架构，而 RDNA 2 则用于 RX 6000 系列。关键区别在于 RDNA 4（RX 9000）拥有更新的 FP8 AI 加速能力，而 RDNA 3 及更早版本使用基于 INT8 整数的 AI 加速，需要更多优化工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://videocardz.com/newz/amd-fsr-upscaling-4-1-officially-coming-to-radeon-rx-7000-gpus-in-july-rx-6000-in-2027">AMD FSR Upscaling 4.1 officially coming to Radeon RX 7000 ...</a></li>
<li><a href="https://linustechtips.com/topic/1637457-amd-confirms-fsr-41-upscaling-for-radeon-rx-7000-series/">AMD confirms FSR 4.1 Upscaling for Radeon RX 7000 series</a></li>
<li><a href="https://www.techspot.com/article/3102-amd-fsr-41-tested/">Testing AMD FSR 4.1: Sharper Images, But DLSS Still Leads</a></li>

</ul>
</details>

**标签**: `#AMD`, `#FSR`, `#GPU`, `#graphics`, `#upscaling`

---

<a id="item-28"></a>
## [Surge 因非标准 TLS 设计拒绝支持 VLESS 协议](https://t.me/zaihuapd/41396) ⭐️ 5.0/10

Surge 开发者近日正式回应用户长期请求支持 VLESS 代理协议的诉求，表示不会将其合并至正式版。尽管已完成实验性实现，但非标准的 TLS 分层设计需要对 OpenSSL 或 BoringSSL 等上游 TLS 库进行定制化修改。 这一决定影响了网络代理工具社区，因为 VLESS 是绕过审查的流行协议。技术理由突出了协议兼容性与维护负担之间的权衡，特别是对于需要稳定上游 TLS 库更新的商业产品。 VLESS 及其变体（如 XTLS/Vision）改变了传统 TLS 的分层边界，需要对 TLS 库进行非标准修改。这种跨层设计增加了 TLS 子系统的复杂性、安全评估成本，并导致难以跟随上游库的更新。

telegram · zaihuapd · May 15, 05:36

**背景**: Surge 是一款面向高级用户的知名网络代理工具。VLESS 是一种轻量级代理协议，旨在绕过审查，常与 XTLS 配合使用以通过移除冗余加密层来优化 TLS 性能。XTLS 是 Xray-core 项目的一部分，Xray-core 是流行的审查规避实现工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vless.dev/">Quick guide to setting up a Vless Reality Proxy server</a></li>
<li><a href="https://github.com/XTLS/Xray-core">GitHub - XTLS /Xray-core: Xray, Penetrates Everything. Also the best...</a></li>

</ul>
</details>

**社区讨论**: 社区用户认可 Surge 技术解释的有效性，但对 VLESS 不会正式支持表示失望。有些人理解维护方面的担忧，而另一些人则继续寻找替代方案。

**标签**: `#Surge`, `#VLESS`, `#network-proxy`, `#TLS`, `#XTLS`

---