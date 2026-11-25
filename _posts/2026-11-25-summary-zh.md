---
layout: default
title: "Horizon Summary: 2026-11-25 (ZH)"
date: 2026-11-25
lang: zh
---

> 从 82 条内容中筛选出 8 条重要资讯。

---

**科技新闻**
1. [OpenAI 预印本称矩阵乘法指数恰为 9/4](#item-tech-news-1) ⭐️ 9.0/10
2. [CVE-2022-22965 Spring 数据绑定远程代码执行 PoC 已公开](#item-tech-news-2) ⭐️ 9.0/10
3. [Check Point 管理服务器遭活跃入侵](#item-tech-news-3) ⭐️ 8.0/10
4. [WatchGuard Firebox/XTM 严重 RCE 漏洞遭利用，PoC 已公开](#item-tech-news-4) ⭐️ 8.0/10
5. [CVE-2022-29464 WSO2 未授权 RCE PoC 公开](#item-tech-news-5) ⭐️ 8.0/10
6. [CVE-2022-22963：Spring Cloud Function SpEL 路由表达式远程代码执行（PoC 已公开）](#item-tech-news-6) ⭐️ 8.0/10
7. [Adobe Magento 结账漏洞遭在野利用，PoC 已公开](#item-tech-news-7) ⭐️ 8.0/10
8. [Apache APISIX batch-requests 插件 X-REAL-IP 绕过导致远程代码执行](#item-tech-news-8) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenAI 预印本称矩阵乘法指数恰为 9/4](https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/paper.pdf) ⭐️ 9.0/10

OpenAI 数学团队发布的一篇预印本声称，在所有域上矩阵乘法的精确指数为 9/4，即 Θ\(n^2.25\)，并由此否定了“矩阵乘法指数等于 2”的猜想。该预印本还称给出了强多项式线性规划、平均收益博弈、奇偶博弈等问题的多项式时间算法。需注意这些成果仍为尚未经过独立验证的预印本声明，并非已发表的同行评审结果。

hackernews · E-Reverance · 11月25日 01:19 · [社区讨论](https://news.ycombinator.com/item?id=50637220)

**「背景」** 矩阵乘法指数 ω 描述 n×n 矩阵相乘的最优渐近复杂度。OpenAI 在 2026 年 10 月批量发布的数学预印本中，已有一篇论文证明上界 ω≤9/4（低于此前约 2.258）；本次新预印本则声称进一步证明了匹配下界 Ω\(n^\{9/4\}\)，从而将指数精确确定为 9/4，并反驳了“ω=2”的猜想。

**「影响」** 如果该下界证明成立，它将排除任何渐近复杂度低于 O\(n^2.25\) 的矩阵乘法算法；此前 2.25 只是已知上界，且近期已有达到该上界（但远非实用）的算法。对算法研究者和复杂性理论而言，这明确了追求更快渐近指数的理论边界。

**「社区讨论」** 有评论纠正原帖标题：应写作 Θ\(n^2.25\) 而非 O\(n^2.25\)，并强调该结果的核心是证明下界 Ω\(n^2.25\)；brandonb 澄清上界 2.25 此前已知。另有评论推测 OpenAI 使用未公开模型做内部研究且未披露训练“配方”，并质疑这种投入更多是公关而非公共利益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=8JAbhoBGL3M">OpenAI just solved math - YouTube</a></li>
<li><a href="https://officechai.com/ai/openai-has-found-a-far-faster-way-to-multiply-matrices-the-math-that-underpins-all-of-modern-ai/">OpenAI Has Found A Far Faster Way To Multiply Matrices , The Math...</a></li>

</ul>
</details>

**标签**: `#matrix multiplication`, `#computational complexity`, `#algorithms`, `#OpenAI`, `#mathematics`

---

<a id="item-tech-news-2"></a>
### [CVE-2022-22965 Spring 数据绑定远程代码执行 PoC 已公开](https://cve.now/CVE-2022-22965) ⭐️ 9.0/10

GitHub 上已公开 CVE-2022-22965 的概念验证代码。该漏洞影响 JDK 9 及以上版本中通过数据绑定使用 Spring MVC 或 Spring WebFlux 的应用，攻击者可在未登录的情况下远程执行代码。已知利用方式要求非默认部署：应用以 WAR 包部署在 Tomcat 上，而不是作为 Spring Boot 可执行 jar 运行。该漏洞已被列入 CISA KEV，表明存在实际攻击。

rss · cve.now 新收录的 CISA KEV · 11月25日 02:11

**「背景」** Spring 的数据绑定机制会将 HTTP 请求参数映射到 Java 对象属性。该漏洞仅在 JDK 9 及以上、应用以 WAR 包部署到 Tomcat（而非 Spring Boot 可执行 jar）的非默认配置下可利用，因此并非所有 Spring Framework 应用都受影响。

**「影响」** 对于以 JDK 9+ 运行、且以 WAR 形式部署在 Tomcat 上的 Spring MVC/WebFlux 应用，应视为被积极利用的高危风险：运营者需立即检查部署形态并应用补丁或缓解措施，避免未认证的远程代码执行。

**标签**: `#security`, `#spring-framework`, `#remote-code-execution`, `#cve-2022-22965`, `#java`

---

<a id="item-tech-news-3"></a>
### [Check Point 管理服务器遭活跃入侵](https://www.greynoise.io/blog/check-point-security-management-servers-intrusion-campaign) ⭐️ 8.0/10

GreyNoise 发布报告，披露一起针对 Check Point 安全管理服务器的在野入侵活动。攻击者扫描并利用 HFS 服务器的 loginSrp1 端点，通过多次登录收集由 JavaScript Math.random\(\) 生成的 sid 值，重建 V8 PRNG 内部状态，从而恢复 HFS 会话 Cookie 签名密钥并伪造管理员会话 Cookie。报告未说明攻击者如何获得初始访问权限；有评论推测可能与 CVE-2026-16232 有关，但该说法尚未得到确认。

hackernews · louiereederson · 11月24日 16:32 · [社区讨论](https://news.ycombinator.com/item?id=50630594)

**「背景：CVE-2026-16232 认证绕过」** 2026 年 7 月 22 日，Check Point 披露了 CVE-2026-16232，这是 SmartConsole 登录过程中的认证绕过漏洞。据 NVD 描述，未认证的远程攻击者可利用该漏洞获取应用登录令牌，并以完全管理员权限进行认证；成功利用需要管理服务器 IP 可从互联网访问且未设置可信客户端（GUI 客户端）限制。该漏洞被评论者推测为本次入侵活动中攻击者获得初始访问权限的途径。

**「影响」** 受影响 Check Point 管理员应立即核查安全管理服务器是否暴露在公网，并审计管理员会话和登录日志，因为攻击者能伪造有效的管理员 Cookie 获得管理权限。

**「社区讨论」** 有评论指出初始访问路径仍不明确，并推测 CVE-2026-16232 可能是初始向量；另有评论认为应修复 Math.random 本身，而不是依赖应用避免将其用于安全场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.checkpoint.com/results/sk/sk185169">sk185169 - CVE-2026-16232 - Authentication bypass with ...</a></li>
<li><a href="https://app.opencve.io/cve/CVE-2026-16232">CVE-2026-16232 - Vulnerability Details - OpenCVE</a></li>
<li><a href="https://nvd.nist.gov/vuln/detail/cve-2026-16232">NVD-CVE-2026-16232</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerability`, `#Check Point`, `#session forgery`, `#PRNG`

---

<a id="item-tech-news-4"></a>
### [WatchGuard Firebox/XTM 严重 RCE 漏洞遭利用，PoC 已公开](https://cve.now/CVE-2022-26318) ⭐️ 8.0/10

CVE-2022-26318 是 WatchGuard Firebox 和 XTM 设备 Fireware OS 中的未认证远程代码执行漏洞，现已被 CISA 新增至已知被利用漏洞 \(KEV\) 目录。GitHub 上已发布公开概念验证 \(PoC\) 代码，且该漏洞正被攻击者实际利用。攻击者可在未登录的情况下远程在受影响设备上执行任意代码。

rss · cve.now 新收录的 CISA KEV · 11月25日 02:21

**「背景」** WatchGuard Firebox 和 XTM 是运行 Fireware OS 的网络安全设备。该漏洞属于无需身份验证的远程代码执行问题，公开的概念验证代码发布后，攻击者更容易利用。

**「影响与行动」** 受影响设备若暴露在互联网且未修补，存在被远程完全控制的风险；管理员应尽快对照 WatchGuard 公告升级 Fireware OS 或应用缓解措施，并检查是否存在入侵迹象。

**标签**: `#security`, `#vulnerability`, `#remote code execution`, `#network appliance`, `#CVE-2022-26318`

---

<a id="item-tech-news-5"></a>
### [CVE-2022-29464 WSO2 未授权 RCE PoC 公开](https://cve.now/CVE-2022-29464) ⭐️ 8.0/10

CVE-2022-29464 是 WSO2 多款产品（API Manager、Identity Server、Enterprise Integrator）中未认证的远程代码执行漏洞，攻击者可向 /fileupload 端点发送特制请求上传任意文件（如恶意 JSP）并在服务器执行代码。该漏洞已公开 GitHub 概念验证和 Metasploit 模块，并被 CISA 列入已知被利用漏洞目录。

rss · cve.now 新收录的 CISA KEV · 11月25日 02:21

**「背景」** 该漏洞最初由 DEVCORE 的 Orange Tsai 报告，WSO2 于 2022 年 1 月向客户提供临时缓解措施，并于 2 月为受支持的产品版本发布修复。官方公告指出，漏洞源于对用户输入校验不当，攻击者可上传任意文件至服务器上用户可控的位置，进而实现远程代码执行。

**「影响」** 公开利用代码意味着未修补的 WSO2 实例面临被主动扫描和入侵的实质性风险，管理员应优先确认相关产品是否可达 /fileupload 端点，并按厂商指引补救。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://security.docs.wso2.com/en/latest/security-announcements/security-advisories/2022/WSO2-2021-1738/">Security Advisory WSO2-2021-1738/CVE-2022-29464 NVD-CVE-2022-29464 CVE-2022-29464 - Vulnerability Details - OpenCVE CVE-2022-29464: Critical WSO2 Products Vulnerability Details CVE-2022-29464: WSO2 Multiple Products | Exploited</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#remote-code-execution`, `#WSO2`, `#CVE`

---

<a id="item-tech-news-6"></a>
### [CVE-2022-22963：Spring Cloud Function SpEL 路由表达式远程代码执行（PoC 已公开）](https://cve.now/CVE-2022-22963) ⭐️ 8.0/10

受影响的是 Spring Cloud Function 的路由功能：攻击者无需登录，即可通过发送特制的 SpEL 路由表达式远程执行代码并访问本地资源。GitHub 上已公开概念验证（PoC），Metasploit 模块也已提供，且已有利用该漏洞的攻击发生。

rss · cve.now 新收录的 CISA KEV · 11月25日 02:11

**「背景」** Spring Cloud Function 的路由功能允许通过 HTTP 头中的 spring.cloud.function.routing-expression 值动态选择要调用的函数，该表达式使用 Spring Expression Language \(SpEL\) 求值。由于该路由表达式可被远程未认证用户直接控制，攻击者能够注入执行任意代码的 SpEL 表达式，从而在服务器上运行命令并访问本地资源。

**「影响」** 使用受影响的 Spring Cloud Function 路由功能的部署面临无需认证的远程代码执行和本地资源访问风险，且已有公开 PoC 和实际攻击；管理员应优先排查并采取缓解措施。

**标签**: `#CVE-2022-22963`, `#Spring Cloud Function`, `#Remote Code Execution`, `#SpEL Injection`, `#Security Vulnerability`

---

<a id="item-tech-news-7"></a>
### [Adobe Magento 结账漏洞遭在野利用，PoC 已公开](https://cve.now/CVE-2022-24086) ⭐️ 8.0/10

Adobe Commerce（Magento Commerce）的结账流程存在输入验证缺陷（CVE-2022-24086），攻击者无需登录或用户交互即可远程执行任意代码。该漏洞已出现在野利用，GitHub 上公开了概念验证代码，并被列入 CISA KEV。

rss · cve.now 新收录的 CISA KEV · 11月25日 02:11

**「背景」** 该漏洞此前已被披露为 Adobe Commerce / Magento 结账流程中的输入验证缺陷，并被列入 CISA 已知被利用漏洞目录；本次更新指出 GitHub 上已发布概念验证代码，使漏洞利用细节公开化。

**「影响」** 未打补丁的 Adobe Commerce/Magento 实例可能被攻击者远程完全控制，相关管理员应尽快确认版本并采取缓解措施。

**标签**: `#security`, `#vulnerability`, `#remote-code-execution`, `#Adobe Commerce`, `#CVE`

---

<a id="item-tech-news-8"></a>
### [Apache APISIX batch-requests 插件 X-REAL-IP 绕过导致远程代码执行](https://cve.now/CVE-2022-24112) ⭐️ 8.0/10

CVE-2022-24112 影响 Apache APISIX 的 batch-requests 插件：攻击者通过 X-REAL-IP 头覆盖客户端 IP，可绕过 Admin API 的 IP 限制。在默认配置且使用默认 API key 时，该漏洞导致远程代码执行；即使非默认配置，数据面板的 IP 限制也可被绕过。GitHub 上已公开概念验证代码，该漏洞无需登录即可远程利用，且已出现实际攻击。

rss · cve.now 新收录的 CISA KEV · 11月25日 02:11

**「背景」** Apache APISIX 是开源 API 网关，batch-requests 插件支持客户端一次提交多个请求；Admin API 默认通过 IP 白名单和固定 API key 进行保护。该插件在处理客户端 IP 时信任 X-REAL-IP 头，导致攻击者可通过伪造该头绕过 IP 限制。

**「影响」** 未认证攻击者可远程利用该漏洞在受影响网关上执行任意代码，尤其是仍使用默认 API key 和默认 Admin API 配置的部署。管理员应立即限制 Admin API 访问、更换默认密钥，并升级或禁用 batch-requests 插件。

**标签**: `#security`, `#Apache APISIX`, `#CVE-2022-24112`, `#remote code execution`, `#vulnerability`

---