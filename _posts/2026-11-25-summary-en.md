---
layout: default
title: "Horizon Summary: 2026-11-25 (EN)"
date: 2026-11-25
lang: en
---

> From 84 items, 31 important content pieces were selected

---

**Technology News**
1. [OpenAI Preprint Claims Matrix Multiplication Exponent Is Exactly 9/4](#item-tech-news-1) ⭐️ 10.0/10
2. [Dirty Pipe Linux kernel root escalation PoC published, actively exploited](#item-tech-news-2) ⭐️ 9.0/10
3. [Check Point Management Servers Targeted via PRNG Cookie Forging](#item-tech-news-3) ⭐️ 8.0/10
4. [CVE-2022-26318: WatchGuard Firebox/XTM RCE PoC Published](#item-tech-news-4) ⭐️ 8.0/10
5. [WSO2 CVE-2022-29464 file upload RCE proof-of-concept published](#item-tech-news-5) ⭐️ 8.0/10
6. [Spring Cloud Gateway CVE-2022-22947 RCE PoC Published on GitHub](#item-tech-news-6) ⭐️ 8.0/10
7. [CVE-2022-22963: Spring Cloud Function SpEL RCE with Public PoC](#item-tech-news-7) ⭐️ 8.0/10
8. [Zabbix Frontend SAML Bypass Now in CISA KEV; PoC Published](#item-tech-news-8) ⭐️ 8.0/10
9. [CVE-2022-22965 Spring RCE PoC Published](#item-tech-news-9) ⭐️ 8.0/10
10. [CVE-2022-24086: Magento Checkout RCE Actively Exploited, PoC Released](#item-tech-news-10) ⭐️ 8.0/10
11. [Apache APISIX batch-requests plugin auth bypass exploited](#item-tech-news-11) ⭐️ 8.0/10
12. [CVE-2022-24990: TerraMaster NAS Unauthenticated RCE with PoC](#item-tech-news-12) ⭐️ 8.0/10
13. [Chrome V8 Type Confusion CVE-2022-1096 Gets Public PoC, CISA KEV Listing](#item-tech-news-13) ⭐️ 8.0/10
14. [CVE-2022-20699: Cisco RV Series Router RCE Public PoC Published](#item-tech-news-14) ⭐️ 8.0/10
15. [Linux Kernel CVE-2022-0185 Heap Overflow Enables Local Root and Container Escape](#item-tech-news-15) ⭐️ 8.0/10
16. [Rackspace Shuts Down Spot Cloud Platform After Security Breach](#item-tech-news-16) ⭐️ 8.0/10
17. [Hackers compromise Check Point servers in 22 organizations](#item-tech-news-17) ⭐️ 8.0/10
18. [VMware Patches Critical 9.8 vmdir Auth Bypass in vCenter](#item-tech-news-18) ⭐️ 8.0/10
19. [Single Bit Flip in .NET Files Bypasses Windows Code Integrity and VirtualBox Hardening](#item-tech-news-19) ⭐️ 8.0/10
20. [Microsoft Fixes Azure API Management Classic Flaw After NSM Disclosure](#item-tech-news-20) ⭐️ 8.0/10
21. [WHMCS Shopping Cart SQL Injection Exposes Customer Data and Admin Password Hashes](#item-tech-news-21) ⭐️ 8.0/10
22. [CISA Flags Actively Exploited N-able MailAssure, MONAI Label Flaws](#item-tech-news-22) ⭐️ 8.0/10
23. [VMware Patches Critical ESX and vCenter Vulnerabilities](#item-tech-news-23) ⭐️ 8.0/10
24. [Check Point Security Management Servers Hacked in AI-Assisted Campaign](#item-tech-news-24) ⭐️ 8.0/10
25. [Ternary Bonsai 2.5 27B Benchmarked Locally](#item-tech-news-25) ⭐️ 7.0/10
26. [GPT-6.2 designs protein minibinder structures through generated code](#item-tech-news-26) ⭐️ 7.0/10
27. [GTA 6 Unofficial Windows Port Uses Leaked Xbox Build](#item-tech-news-27) ⭐️ 7.0/10
28. [CISA Adds Three Exploited Vulnerabilities to KEV Catalog](#item-tech-news-28) ⭐️ 7.0/10
29. [AutomationDirect C-More EA9 Heap Buffer Overflow Fixed in V6.81](#item-tech-news-29) ⭐️ 7.0/10
30. [VMware Workspace ONE Access RCE PoC Published](#item-tech-news-30) ⭐️ 7.0/10
31. [CVE-2022-21882 Win32k Privilege Escalation Gets Public Proof-of-Concept](#item-tech-news-31) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI Preprint Claims Matrix Multiplication Exponent Is Exactly 9/4](https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/paper.pdf) ⭐️ 10.0/10

An OpenAI preprint dated November 24, 2026 claims that the matrix multiplication exponent is exactly 9/4 \(Θ\(n^2.25\)\) over every field, refuting the conjecture that the exponent is 2. The same preprint also claims polynomial-time algorithms for Smale’s ninth problem \(strongly polynomial linear programming\), parity games, and mean-payoff games. These are announced preprint results and have not been independently verified.

hackernews · E-Reverance · Nov 25, 01:19 · [Discussion](https://news.ycombinator.com/item?id=50637220)

**「Background」** The matrix multiplication exponent ω is the infimum of exponents such that n×n matrices can be multiplied in O\(n^\{ω+ε\}\) time for every ε&gt;0; establishing tight bounds has been a central open problem. Commenter brandonb notes that an O\(n^2.25\) upper bound was already known, so the preprint’s main new claim is the matching Ω\(n^2.25\) lower bound, yielding Θ\(n^2.25\).

**「Impact」** For complexity theorists, a verified lower bound Ω\(n^2.25\) would refute the long-standing conjecture that the exponent is 2 and settle the exact complexity of matrix multiplication; the claimed polynomial-time algorithms would also resolve three named open problems. The preprint has not yet been independently verified, and commenter brandonb notes the known O\(n^2.25\) algorithm is far from practical.

**「Community Discussion」** Commenters clarify the headline notation: brandonb explains the preprint proves a lower bound of Ω\(n^2.25\) while the upper bound was already known, and orlp argues the title should say Θ\(n^2.25\), not O\(n^2.25\). zone411 adds that OpenAI’s four papers claim to resolve eight problems from a top-500 open problems list.

**Tags**: `#matrix-multiplication`, `#computational-complexity`, `#theoretical-computer-science`, `#openai`, `#algorithms`

---

<a id="item-tech-news-2"></a>
### [Dirty Pipe Linux kernel root escalation PoC published, actively exploited](https://cve.now/CVE-2022-0847) ⭐️ 9.0/10

A public proof-of-concept exploit for CVE-2022-0847 \(Dirty Pipe\) has been published on GitHub. The Linux kernel flaw leaves a pipe buffer setting uninitialized, allowing a local low-privilege attacker to overwrite data in read-only files through the page cache and escalate privileges to root, including injecting code into root processes. CISA lists the vulnerability in its Known Exploited Vulnerabilities catalog, confirming active exploitation.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:01

**「Background」** The Linux kernel uses pipe buffers and the page cache to move data between processes and files. CVE-2022-0847 \(Dirty Pipe\) stems from an uninitialized pipe buffer flag, which lets a local low-privilege process modify page cache entries for files it should only be able to read.

**「Impact」** Unpatched Linux systems are exposed to local privilege escalation to root, and because a public PoC exists and exploitation is confirmed, administrators should apply kernel updates that fix CVE-2022-0847 and treat affected systems as compromised until patched.

**Tags**: `#security`, `#linux-kernel`, `#vulnerability`, `#privilege-escalation`, `#cve`

---

<a id="item-tech-news-3"></a>
### [Check Point Management Servers Targeted via PRNG Cookie Forging](https://www.greynoise.io/blog/check-point-security-management-servers-intrusion-campaign) ⭐️ 8.0/10

GreyNoise reports an active intrusion campaign against Check Point security management servers in which attackers exploit a predictable PRNG in the HFS login flow to forge admin session cookies. Each POST to the HFS loginSrp1 endpoint returns a signed session cookie whose &quot;sid&quot; is drawn from JavaScript&\#x27;s Math.random\(\); by logging in repeatedly, attackers reconstruct the V8 PRNG state, recover the HFS session-cookie signing key, and issue forged admin cookies. The source excerpt provided does not include indicators of compromise or remediation details.

hackernews · louiereederson · Nov 24, 16:32 · [Discussion](https://news.ycombinator.com/item?id=50630594)

**「How the session cookie attack works」** Check Point Security Management Servers expose an HFS login endpoint that returns a signed session cookie containing a &quot;sid&quot; value drawn from JavaScript&\#x27;s Math.random\(\). Because Math.random\(\) is not cryptographically secure, an attacker can collect several login responses to reconstruct the internal state of the Node.js V8 PRNG, recover the HFS session-cookie signing key, and forge a signed admin session cookie.

**「Impact」** Security teams using Check Point Security Management Server should assess whether the server is reachable from the internet and inspect HFS loginSrp1 logs for repeated login requests that could indicate PRNG-state reconstruction.

**「Community Discussion」** Commenters questioned how initial access was obtained, with one noting uncertainty about whether CVE-2026-16232 was the initial vector and whether affected management servers were internet-exposed. Another argued that making all random number generators at least somewhat secure would be a better root fix than patching the many applications that misuse Math.random.

**Tags**: `#security`, `#vulnerability`, `#Check Point`, `#PRNG`, `#intrusion`

---

<a id="item-tech-news-4"></a>
### [CVE-2022-26318: WatchGuard Firebox/XTM RCE PoC Published](https://cve.now/CVE-2022-26318) ⭐️ 8.0/10

CVE-2022-26318 affects WatchGuard Firebox and XTM appliances running Fireware OS, allowing an unauthenticated remote attacker to execute arbitrary code on the device. A proof-of-concept has been published on GitHub, and the vulnerability is being actively exploited in attacks. Security administrators using these appliances should treat this as an urgent issue.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:21

**「Background」** WatchGuard Firebox and XTM appliances run Fireware OS, a specialized operating system for network security devices. The vulnerability CVE-2022-26318 resides in this OS and requires no authentication, allowing remote attackers to execute arbitrary code on the device.

**「Impact」** Because the flaw enables unauthenticated remote code execution and has both a public exploit and active exploitation, unpatched Firebox or XTM appliances are at immediate risk of compromise. Administrators should confirm that vendor fixes or mitigations are applied and review WatchGuard&\#x27;s advisory for affected versions.

**Tags**: `#security`, `#CVE`, `#network-appliance`, `#RCE`, `#WatchGuard`

---

<a id="item-tech-news-5"></a>
### [WSO2 CVE-2022-29464 file upload RCE proof-of-concept published](https://cve.now/CVE-2022-29464) ⭐️ 8.0/10

A public proof-of-concept exploit for CVE-2022-29464 has been published on GitHub, including a Metasploit module. The vulnerability affects multiple WSO2 products, including API Manager, Identity Server, and Enterprise Integrator. An unauthenticated attacker can send a crafted request to the /fileupload endpoint to upload an arbitrary file, such as a malicious JSP, to a chosen location and execute code on the server.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:21

**「Earlier disclosure and current update」** CVE-2022-29464 is an unauthenticated file upload vulnerability in WSO2 API Manager, Identity Server, and Enterprise Integrator that allows remote attackers to place arbitrary files such as JSP webshells on the server via the /fileupload endpoint. The original advisory already described remote code execution without authentication; the current update adds that public proof-of-concept code, including a Metasploit module, has now been published on GitHub.

**「Impact」** Organizations running affected WSO2 products should patch or apply mitigations immediately, because public exploit code and a Metasploit module now make unauthenticated remote code execution straightforward for attackers.

**Tags**: `#security`, `#CVE`, `#WSO2`, `#remote code execution`, `#exploit`

---

<a id="item-tech-news-6"></a>
### [Spring Cloud Gateway CVE-2022-22947 RCE PoC Published on GitHub](https://cve.now/CVE-2022-22947) ⭐️ 8.0/10

Proof-of-concept exploit code for CVE-2022-22947 has been published on GitHub. The vulnerability allows a remote unauthenticated attacker to execute arbitrary code on the host by sending a crafted request to Spring Cloud Gateway, but only when the Gateway Actuator endpoint is enabled, exposed, and unsecured—a non-default configuration. Public exploit code includes a Metasploit module, and active attacks have been reported.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:11

**「Background」** Earlier disclosures identified CVE-2022-22947 as affecting Spring Cloud Gateway versions prior to 3.1.1 and 3.0.7, with the vulnerable condition being an enabled, exposed, and unsecured Gateway Actuator endpoint; exploitability arises from unsafe Spring Expression Language \(SpEL\) evaluation in routing configuration.

**「Impact」** Because public exploit code and active attacks exist, teams running Spring Cloud Gateway should immediately check whether the Actuator endpoint is enabled, exposed, and unsecured; if so, they should disable or secure it to prevent unauthenticated remote code execution.

<details><summary>References</summary>
<ul>
<li><a href="https://safeguard.sh/resources/blog/spring-cloud-gateway-actuator-rce-cve-2022-22947">Spring Cloud Gateway RCE Vulnerability (CVE-2022-22947)</a></li>
<li><a href="https://www.tenable.com/cve/CVE-2022-22947">CVE-2022-22947 - Tenable</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#Spring Cloud Gateway`, `#remote code execution`, `#CVE-2022-22947`

---

<a id="item-tech-news-7"></a>
### [CVE-2022-22963: Spring Cloud Function SpEL RCE with Public PoC](https://cve.now/CVE-2022-22963) ⭐️ 8.0/10

A proof-of-concept exploit for CVE-2022-22963 has been published on GitHub, confirming unauthenticated remote code execution in Spring Cloud Function&\#x27;s routing functionality. Attackers can run code and access local resources by sending a specially crafted SpEL routing expression without logging in. Public exploit code, including a Metasploit module, is available, and attacks using this vulnerability are actively occurring.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:11

**「Original vulnerability details」** CVE-2022-22963 was originally disclosed in Spring Cloud Function: when routing functionality is enabled, versions 3.1.6, 3.2.2, and older unsupported releases accept a specially crafted SpEL routing expression that may result in remote code execution and access to local resources, according to Spring&\#x27;s advisory. Third-party analysis lists the same affected version ranges, 3.1.6 or prior and 3.2.2 or prior.

**「Impact」** Organizations running affected Spring Cloud Function versions should immediately apply available patches or mitigations and investigate for signs of compromise, because unauthenticated remote code execution is being actively exploited.

<details><summary>References</summary>
<ul>
<li><a href="https://spring.io/security/cve-2022-22963/">spring .io/security/ cve - 2022 - 22963</a></li>
<li><a href="https://www.zscaler.com/blogs/security-research/analysis-spring-cloud-framework-vulnerabilities">Spring Cloud Framework Vulnerabilities | Zscaler Blog</a></li>

</ul>
</details>

**Tags**: `#CVE-2022-22963`, `#Spring Cloud Function`, `#Remote Code Execution`, `#SpEL Injection`, `#CISA KEV`

---

<a id="item-tech-news-8"></a>
### [Zabbix Frontend SAML Bypass Now in CISA KEV; PoC Published](https://cve.now/CVE-2022-23131) ⭐️ 8.0/10

CVE-2022-23131 affects Zabbix Frontend when SAML single sign-on is enabled, which is not the default setup. An unauthenticated remote attacker can change session data to gain admin access, provided they know a valid Zabbix username or the guest account is enabled. The vulnerability has been added to CISA&\#x27;s Known Exploited Vulnerabilities catalog, and a proof of concept has now been published on GitHub.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:11

**「Background」** Zabbix Frontend is the web-based management interface for the Zabbix monitoring platform. SAML single sign-on is an optional authentication configuration for that interface. The vulnerability allows an attacker who reaches the frontend remotely to modify session data without logging in.

**「Impact」** Zabbix deployments with SAML SSO enabled are exposed to remote administrative takeover by an unauthorized attacker who knows a valid username or has guest access enabled. Security teams should treat this as actively exploited and prioritize remediation.

**Tags**: `#security`, `#vulnerability`, `#Zabbix`, `#SAML`, `#authentication bypass`

---

<a id="item-tech-news-9"></a>
### [CVE-2022-22965 Spring RCE PoC Published](https://cve.now/CVE-2022-22965) ⭐️ 8.0/10

A proof-of-concept exploit for CVE-2022-22965 has been published on GitHub. The vulnerability affects Spring Framework applications using Spring MVC or Spring WebFlux on JDK 9 or later, and allows unauthenticated remote code execution through data binding. Exploitation requires a non-default setup: the application must be deployed as a WAR on Tomcat rather than as a Spring Boot executable JAR. The CVE is listed in CISA&\#x27;s Known Exploited Vulnerabilities catalog, indicating active exploitation.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:11

**「Background」** Spring MVC and Spring WebFlux use data binding to map HTTP request parameters to Java object properties; CVE-2022-22965 exploits this mechanism on JDK 9 or later. In the known attack path, the target application is packaged as a WAR and runs on Tomcat, exposing the relevant classloader behavior.

**「Impact」** Security teams running Spring MVC or Spring WebFlux applications on JDK 9+ as WARs on Tomcat should prioritize identifying and patching affected deployments, because an unauthenticated attacker can execute code remotely on the application server.

**Tags**: `#security`, `#vulnerability`, `#Spring Framework`, `#remote code execution`, `#CVE-2022-22965`

---

<a id="item-tech-news-10"></a>
### [CVE-2022-24086: Magento Checkout RCE Actively Exploited, PoC Released](https://cve.now/CVE-2022-24086) ⭐️ 8.0/10

Adobe Commerce \(Magento Commerce\) has a remote code execution vulnerability, CVE-2022-24086, caused by improper input validation in the checkout process. An attacker can execute arbitrary code on the server without authentication or user interaction, and the flaw is being actively exploited. A proof of concept has now been published on GitHub, increasing exploitability. The source does not list affected versions or a patch.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:11

**「Background」** Adobe Commerce \(formerly Magento Commerce\) is a widely used e-commerce platform whose checkout pages accept form input from unauthenticated visitors. An input-validation flaw in that checkout flow means deliberately malformed values can be treated as executable instructions by the server, rather than as ordinary customer data.

**「Impact」** Administrators of Adobe Commerce/Magento stores are at immediate risk because exploitation requires no login or user interaction, and the published proof of concept makes attacks easier to replicate.

**Tags**: `#cybersecurity`, `#vulnerability`, `#Magento`, `#remote-code-execution`, `#CVE`

---

<a id="item-tech-news-11"></a>
### [Apache APISIX batch-requests plugin auth bypass exploited](https://cve.now/CVE-2022-24112) ⭐️ 8.0/10

Apache APISIX has an authentication bypass in its batch-requests plugin \(CVE-2022-24112\) that lets an unauthenticated remote attacker spoof the client IP header and bypass Admin API IP restrictions. Under default configuration with the default API key, this leads to remote code execution; even without those defaults, the data panel IP restriction can still be bypassed. A proof of concept has been published on GitHub, the flaw is being actively exploited, and it is listed in CISA KEV.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:11

**「Background」** Apache APISIX is an open-source API gateway whose Admin API is normally restricted by client IP. Before the fix for CVE-2022-24112, the batch-requests plugin could be abused to spoof the client IP via a header such as X-REAL-IP, and the built-in default Admin API token edd1c9f034335f136f87ad84b625c8f1 granted access. Affected versions are earlier than 2.12.1, and CISA added this vulnerability to its Known Exploited Vulnerabilities catalog on 2022-08-25 after confirming exploitation.

**「Impact」** Apache APISIX operators should check whether the batch-requests plugin is enabled and whether the default Admin API key or IP restriction is still in use, since this combination permits unauthenticated remote code execution and active exploitation is already occurring.

<details><summary>References</summary>
<ul>
<li><a href="https://cve.now/CVE-2022-24112">CVE - 2022 - 24112 : Apache APISIX code execution in batch-requests</a></li>
<li><a href="https://turingpoint.de/en/cve/CVE-2022-24112/">CVE - 2022 - 24112 - Apache APISIX Authentication Bypass... | turingpoint</a></li>
<li><a href="https://sploitus.com/exploit?id=MSF:EXPLOIT-MULTI-HTTP-APACHE_APISIX_API_DEFAULT_TOKEN_RCE-">Apache Apisix &lt; 2.12.1 — Metasploit exploit for CVE - 2022 - 24112</a></li>

</ul>
</details>

**Tags**: `#security`, `#Apache APISIX`, `#CVE-2022-24112`, `#remote code execution`, `#API gateway`

---

<a id="item-tech-news-12"></a>
### [CVE-2022-24990: TerraMaster NAS Unauthenticated RCE with PoC](https://cve.now/CVE-2022-24990) ⭐️ 8.0/10

TerraMaster NAS devices are affected by CVE-2022-24990, an unauthenticated remote code execution vulnerability in the web interface. Attackers can abuse PHP object instantiation to run arbitrary code, including uploading a PHP webshell, without logging in. The flaw is listed as actively exploited in attacks, and a proof of concept has been published on GitHub.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:11

**「Background」** TerraMaster NAS web management interfaces rely on PHP endpoints in which attacker-controlled parameters can trigger object instantiation; this class of flaw can allow arbitrary PHP code to be executed on the device without prior authentication.

**「Impact」** Because the flaw is remotely reachable without authentication and is actively exploited, administrators should treat exposed TerraMaster NAS devices as potentially compromised, check for vendor patches, and restrict web interface access to trusted networks.

**Tags**: `#security`, `#vulnerability`, `#remote-code-execution`, `#NAS`, `#CVE`

---

<a id="item-tech-news-13"></a>
### [Chrome V8 Type Confusion CVE-2022-1096 Gets Public PoC, CISA KEV Listing](https://cve.now/CVE-2022-1096) ⭐️ 8.0/10

Google Chrome&\#x27;s V8 engine has a type confusion vulnerability, CVE-2022-1096, that can be reached remotely without authentication by convincing a user to open a crafted HTML page, causing memory corruption. The related Chromium advisory says the worst affected bundled issue could allow remote code execution. A proof of concept has now been published on GitHub, and the flaw is listed in CISA&\#x27;s Known Exploited Vulnerabilities catalog, indicating active exploitation.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:01

**「Background」** The CISA Known Exploited Vulnerabilities catalog tracks vulnerabilities with evidence of active exploitation; inclusion is a signal that defenders should treat the issue as an immediate patch priority.

**「Impact」** Users and administrators should apply the relevant Google Chrome or Chromium update immediately, because the public proof-of-concept and CISA KEV listing increase the likelihood that unpatched systems will be targeted.

**Tags**: `#security`, `#vulnerability`, `#chrome`, `#v8`, `#exploit`

---

<a id="item-tech-news-14"></a>
### [CVE-2022-20699: Cisco RV Series Router RCE Public PoC Published](https://cve.now/CVE-2022-20699) ⭐️ 8.0/10

A proof-of-concept exploit for CVE-2022-20699 has been published on GitHub. The flaw allows unauthenticated remote code execution with root privileges in Cisco Small Business RV160, RV260, RV340, and RV345 router firmware via crafted HTTP requests. Active exploitation is already occurring, with the greatest relevance for RV340 and RV345 routers used as SSL VPN gateways.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:01

**「Background」** CVE-2022-20699 is a vulnerability in the HTTP server of Cisco Small Business RV series firmware; it can be triggered without authentication, giving an attacker root-level control. The new GitHub PoC makes the previously exploited technique more accessible to other attackers.

**「Impact」** Organizations using affected RV series routers, especially RV340/RV345 SSL VPN gateways, should treat exposed devices as actively at risk because unauthenticated exploitation is already happening and a public PoC reduces the effort needed for further attacks.

**Tags**: `#cybersecurity`, `#vulnerability`, `#remote-code-execution`, `#Cisco`, `#router-firmware`

---

<a id="item-tech-news-15"></a>
### [Linux Kernel CVE-2022-0185 Heap Overflow Enables Local Root and Container Escape](https://cve.now/CVE-2022-0185) ⭐️ 8.0/10

A public proof-of-concept exploit for CVE-2022-0185, a heap buffer overflow in the Linux kernel&\#x27;s filesystem context handling, has been published on GitHub. The flaw lets a local attacker escalate privileges to root, and container escape has also been reported. The attacker reaches it locally by opening a filesystem that falls back to legacy handling, and the vulnerability is listed in CISA&\#x27;s Known Exploited Vulnerabilities catalog, indicating active exploitation.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:01

**「Background」** The Linux kernel&\#x27;s filesystem context subsystem can fall back to legacy handling for filesystems that do not use the newer context API, and an unprivileged local user can trigger this fallback path by opening such a filesystem. The heap buffer overflow occurs during this parsing, corrupting kernel memory.

**「Impact」** On unpatched systems, any local user can become root, and a compromised container can escape to the host. Security teams should treat this as an urgent patch priority due to active exploitation and the CISA KEV listing.

**Tags**: `#Linux kernel`, `#security vulnerability`, `#privilege escalation`, `#container escape`, `#CISA KEV`

---

<a id="item-tech-news-16"></a>
### [Rackspace Shuts Down Spot Cloud Platform After Security Breach](https://www.bleepingcomputer.com/news/security/rackspace-shuts-down-spot-cloud-platform-after-security-breach/) ⭐️ 8.0/10

Rackspace is shutting down its Rackspace Spot cloud platform after a security breach allowed hackers to access customer Kubernetes clusters and secrets. Customers are being given until December 8 to migrate their services and download their data.

rss · Bleeping Computer · Nov 24, 21:37

**「Background」** Rackspace Spot was a cloud platform for managing Kubernetes clusters and related workloads. According to the security notice, attackers gained access to customer Kubernetes clusters and secrets stored in the platform, which is why Rackspace is requiring customers to migrate services and download data by December 8.

**Tags**: `#cloud security`, `#Kubernetes`, `#data breach`, `#Rackspace`, `#incident response`

---

<a id="item-tech-news-17"></a>
### [Hackers compromise Check Point servers in 22 organizations](https://www.bleepingcomputer.com/news/security/hackers-compromise-check-point-servers-in-22-organizations/) ⭐️ 8.0/10

Threat actors have compromised two dozen Check Point security management servers across 22 organizations by exploiting multiple vulnerabilities, according to BleepingComputer. The campaign is ongoing, and the specific vulnerabilities and affected server versions have not been disclosed in the supplied report. The attackers are targeting Check Point Security Management infrastructure, which organizations use to administer security policies.

rss · Bleeping Computer · Nov 24, 16:15

**「Background」** Check Point Security Management Servers are centralized consoles that configure and monitor Check Point firewalls, storing policy rules and credentials; compromising one can let an attacker read or alter an organization&\#x27;s firewall configuration.

**「Impact」** Administrators of Check Point security management servers should investigate for signs of compromise, because the campaign is ongoing and attackers have already accessed servers at 22 organizations.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/check-point-security-management-servers/">Hackers Target Check Point Security Management Servers ...</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#vulnerability`, `#CheckPoint`, `#threat-intelligence`, `#network-security`

---

<a id="item-tech-news-18"></a>
### [VMware Patches Critical 9.8 vmdir Auth Bypass in vCenter](https://thehackernews.com/2026/11/vmware-vcenter-hit-by-another-critical.html) ⭐️ 8.0/10

Broadcom has shipped patches for 23 vulnerabilities across VMware ESX, vCenter, Workstation, Fusion, and Avi Load Balancer. The most severe is CVE-2026-123903, a CVSS 9.8 authentication bypass in the VMware Directory Service \(vmdir\) of vCenter. The vulnerability is reported to have been exploited as a zero-day before the patch.

rss · The Hacker News · Nov 24, 13:28

**「Background」** VMware vCenter Server uses the Directory Service \(vmdir\) to authenticate users and processes in vSphere environments. Because vCenter manages ESXi hosts and virtual machines, an authentication bypass in vmdir can give an unauthenticated attacker administrative control over the virtualization infrastructure.

**「Impact」** Administrators of affected VMware deployments should apply Broadcom&\#x27;s updates promptly, since the vmdir flaw allows authentication bypass and has reportedly been exploited in the wild.

**Tags**: `#security`, `#vulnerability`, `#VMware`, `#vCenter`, `#authentication bypass`

---

<a id="item-tech-news-19"></a>
### [Single Bit Flip in .NET Files Bypasses Windows Code Integrity and VirtualBox Hardening](https://thehackernews.com/2026/11/google-researcher-shows-how-single-bit.html) ⭐️ 8.0/10

Google Project Zero researcher James Forshaw demonstrated that flipping a single bit in a .NET file can bypass Windows code integrity and Oracle VirtualBox process hardening on Windows hosts. The technique exploits a quirk in how the .NET Framework loads a program file, allowing a local attacker to run untrusted code past both protections. The VirtualBox issue is tracked as CVE-2026-87268.

rss · The Hacker News · Nov 24, 12:02

**「Background」** Windows code integrity and VirtualBox process hardening block untrusted code by checking the signature or trust level of binaries before loading them. Google Project Zero&\#x27;s James Forshaw previously analyzed Oracle VirtualBox&\#x27;s process hardening on Windows in 2017, establishing the baseline protections that are relevant to this new .NET loading behavior.

**「Impact」** Defenders should not treat Windows code integrity or VirtualBox process hardening on Windows hosts as sufficient against a local attacker who can modify .NET files; the supplied report does not describe a patch or mitigation.

<details><summary>References</summary>
<ul>
<li><a href="https://projectzero.google/2026/11/virtualbox-process-hardening.html">VirtualBox Process Hardening on Windows 2026... - Project Zero</a></li>

</ul>
</details>

**Tags**: `#security`, `#windows`, `#.net`, `#vulnerability`, `#code-integrity`

---

<a id="item-tech-news-20"></a>
### [Microsoft Fixes Azure API Management Classic Flaw After NSM Disclosure](https://thehackernews.com/2026/11/microsoft-fixes-azure-api-management.html) ⭐️ 8.0/10

Microsoft has fixed a vulnerability in Azure API Management after Norway&\#x27;s National Security Authority \(NSM\) disclosed that an unknown actor had been actively searching APIM for access tokens, secrets, and named values. The flaw affected multiple businesses in Norway, including energy companies Equinor and Skagerak Energi. NSM said it is still uncertain how the actor obtained access.

rss · The Hacker News · Nov 24, 10:44

**「Azure API Management and Classic-tier exposure」** Azure API Management \(APIM\) is the Azure service that organizations use to publish, protect, and control access to their API interfaces. Norway&\#x27;s NSM had reported that the actively exploited vulnerability affected only APIM Classic deployments, not the v2 tier.

**「Impact」** Azure API Management customers, especially Norwegian organizations, should treat stored APIM access tokens, secrets, and named values as potentially exposed and apply Microsoft&\#x27;s fix while rotating credentials where exposure is suspected.

<details><summary>References</summary>
<ul>
<li><a href="https://dzen.ru/a/awVE-B3lampctOJ8">В Azure закрыли уязвимость. Почему компаниям всё равно... | Дзен</a></li>
<li><a href="https://pasqualepillitteri.it/ru/news/36314/equinor-skagerak-uyazvimost-azure-api-management">Equinor и Skagerak Energi атакованы через уязвимость в Azure ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#azure`, `#api-management`, `#vulnerability`, `#cloud`

---

<a id="item-tech-news-21"></a>
### [WHMCS Shopping Cart SQL Injection Exposes Customer Data and Admin Password Hashes](https://thehackernews.com/2026/11/whmcs-sql-injection-flaw-could-expose.html) ⭐️ 8.0/10

WHMCS disclosed a SQL injection vulnerability in its shopping cart that lets unauthenticated attackers retrieve customer records and administrator password hashes from installations of the billing and automation platform. The flaw requires no login and affects web hosting companies using WHMCS. The company also disclosed two additional flaws that require a logged-in client; the available report does not specify affected versions or patch availability.

rss · The Hacker News · Nov 24, 08:34

**「Background」** WHMCS is a billing, support, and automation platform widely used by web hosting providers to manage customer accounts, orders, and payments; its storefront and client area are normally reachable over the public internet. The shopping cart is part of that storefront and operates on the same database that holds customer records and administrator credential hashes. SQL injection occurs when unsanitized input is concatenated into a database query, enabling an attacker to alter the intended query and read data they should not access.

**「Immediate patching required」** WHMCS-based hosting providers should immediately apply the vendor&\#x27;s patch and treat stored administrator password hashes as compromised, because the unauthenticated SQL injection can be exploited to pull customer records and admin hashes from any unpatched installation.

**Tags**: `#security`, `#sql-injection`, `#WHMCS`, `#vulnerability`, `#web-hosting`

---

<a id="item-tech-news-22"></a>
### [CISA Flags Actively Exploited N-able MailAssure, MONAI Label Flaws](https://thehackernews.com/2026/11/hackers-exploit-n-able-mailassure-flaw.html) ⭐️ 8.0/10

On Monday, CISA added two actively exploited vulnerabilities to its Known Exploited Vulnerabilities catalog: CVE-2026-134624, a server-side request forgery vulnerability in N-able MailAssure&\#x27;s LDAP with a CVSS score of 9.3, and a vulnerability in MONAI Label that the report describes as an AI-related zero-day. The supplied excerpt includes the CVE and details for the MailAssure flaw but does not include the corresponding identifier for the MONAI Label flaw.

rss · The Hacker News · Nov 24, 06:02

**「Background」** MONAI Label is an open-source medical imaging labeling tool, and its zero-day path traversal vulnerability was reportedly discovered by Amazon&\#x27;s autonomous AI tool Cairn; versions 0.8.5 and earlier are affected, with a fix due in the next release. CISA&\#x27;s KEV catalog tracks vulnerabilities that are being actively exploited and triggers federal remediation timelines.

**「Impact」** Organizations using N-able MailAssure or MONAI Label should treat these vulnerabilities as actively exploited and consult CISA&\#x27;s KEV entry and vendor guidance for available mitigations or patches.

<details><summary>References</summary>
<ul>
<li><a href="https://www.immunitysec.com/">Cybersecurity Software &amp; Tools ( 2026 ) | ImmunitySec</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/hackers-use-autonomous-ai-tool-cairn-to-find-zero-day-take-over-server/">Hackers use autonomous AI tool Cairn to find zero - day , take over server</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#vulnerability`, `#AI security`, `#zero-day`, `#CISA KEV`

---

<a id="item-tech-news-23"></a>
### [VMware Patches Critical ESX and vCenter Vulnerabilities](https://www.securityweek.com/vmware-updates-patch-critical-esx-vcenter-vulnerabilities/) ⭐️ 8.0/10

VMware has released patches addressing critical vulnerabilities in ESX and vCenter. The flaws include an authentication bypass vulnerability in vCenter and vulnerabilities that could allow code execution on ESX hosts. The report does not list affected product versions, CVE identifiers, or specific patch availability details.

rss · SecurityWeek · Nov 24, 16:32

**「VMware infrastructure context」** VMware ESX is the hypervisor that runs virtual machines on physical hosts, while vCenter is the central management server for those hosts. The advisory identifies a critical authentication bypass in vCenter&\#x27;s VMware Directory Service \(CVE-2026-123903, CVSS 9.8\), which would give a network attacker Administrator-level access without credentials, and ESX flaws that permit code execution on the host.

**「Impact」** Unpatched vCenter deployments exposed to network access can be fully compromised via CVE-2026-123890, an unauthenticated authentication bypass, while ESX hosts are at risk of code execution; administrators should apply the VMSA-2026-0006.1 updates immediately.

<details><summary>References</summary>
<ul>
<li><a href="https://www.securityweek.com/vmware-updates-patch-critical-esx-vcenter-vulnerabilities/">VMware Updates Patch Critical ESX, vCenter Vulnerabilities</a></li>
<li>VMSA-2026-0006.1: VMware ESX, vCenter, Workstation, and Fusion ...</li>
<li>CVE-2026-123890: Critical Authentication Bypass in VMware ...</li>

</ul>
</details>

**Tags**: `#security`, `#virtualization`, `#VMware`, `#vulnerability`, `#patch`

---

<a id="item-tech-news-24"></a>
### [Check Point Security Management Servers Hacked in AI-Assisted Campaign](https://www.securityweek.com/check-point-security-management-servers-hacked-in-ai-assisted-campaign/) ⭐️ 8.0/10

Check Point Security Management Servers have been hacked in an AI-assisted campaign, SecurityWeek reports. The attacks originated from 99 IP addresses and targeted organizations across multiple industries and countries.

rss · SecurityWeek · Nov 24, 14:21

**「Background」** Check Point Security Management Servers are central components used to manage and enforce security policies across Check Point gateways, making them high-value targets because a compromise could allow attackers to alter or disable defenses. The SecurityWeek report says the attacks originated from 99 IP addresses and affected organizations in multiple industries and countries, but it does not specify the exact AI-assisted techniques used in the campaign.

**Tags**: `#cybersecurity`, `#Check Point`, `#AI-assisted attacks`, `#network security`, `#threat intelligence`

---

<a id="item-tech-news-25"></a>
### [Ternary Bonsai 2.5 27B Benchmarked Locally](https://prismml.com/news/bonsai-2-5-27b) ⭐️ 7.0/10

Ternary Bonsai 2.5 27B, a ternary-quantized model, is being tested by the community for local coding and agentic tasks. One user reports about 22–25 tokens/s generation and 128k context on an M5 Pro Mac Mini with 24GB RAM, while another says the model scores equivalent to Opus 4.6 on SWE-bench verified, with caveats about benchmark fit. These results are early community measurements, not official benchmarks.

hackernews · b0m · Nov 24, 20:08 · [Discussion](https://news.ycombinator.com/item?id=50633922)

**「Background」** Ternary Bonsai 2.5 27B builds on PrismML&\#x27;s earlier Ternary Bonsai 2 27B, keeping the Qwen3.8-27B hybrid-attention architecture and ternary weight format at 1.76 bits per weight \(5.93 GB versus 53.8 GB for FP16\). PrismML&\#x27;s announcement compares it against both Ternary Bonsai 2 27B and the full-precision Qwen3.8 27B base model, emphasizing gains in agentic execution, coding, and multi-turn tool use.

**「Local agentic coding feasibility」** Developers can run this model locally for agentic coding with a permissive license: the Apache-2.0 weights run via llama.cpp on NVIDIA/Intel and via MLX on Apple devices, the Q2\_0 GGUF is 5.93 GB with 262K context, and a Mac Mini M5 Pro 24G user measured 22–25 tokens/s generation with 128k context in memory.

**「Community Discussion」** Commenters debate whether the SWE-bench verified parity with Opus 4.6 indicates real small-model progress or benchmark overfitting, and ask for direct comparisons against similarly sized Q1/Q2 quantized models. One user&\#x27;s long-horizon local benchmark shows Bonsai2.5 matching Bonsai2&\#x27;s pass count while reducing steps by 17% and time by 29%.

<details><summary>References</summary>
<ul>
<li><a href="https://prismml.com/news/bonsai-2-5-27b">PrismML — Introducing Ternary Bonsai 2 . 5 27 B : Powering Agentic...</a></li>
<li><a href="https://huggingface.co/prism-ml/Ternary-Bonsai-2.5-27B-GGUF">prism-ml/ Ternary - Bonsai - 2 . 5 - 27 B -GGUF · Hugging Face</a></li>
<li><a href="https://prismml.com/news/bonsai-2-5-27b">PrismML — Introducing Ternary Bonsai 2 . 5 27 B : Powering Agentic...</a></li>
<li><a href="https://huggingface.co/prism-ml/Ternary-Bonsai-2.5-27B-GGUF">prism-ml/ Ternary - Bonsai - 2 . 5 - 27 B -GGUF · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#AI`, `#machine learning`, `#LLM`, `#quantization`, `#open-source`

---

<a id="item-tech-news-26"></a>
### [GPT-6.2 designs protein minibinder structures through generated code](https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/) ⭐️ 7.0/10

OpenAI reports that GPT-6.2 was given the 3-D structures of five target proteins and attachment points for minibinders, then wrote code to produce candidate minibinder structures without using specialized protein AI models. The resulting three-dimensional designs still required a separate AI model, SolubleMPNN, to generate amino acid sequences, and further specialized models to select candidates predicted to fold and bind properly. The announced capability is presented as a code-generation role rather than a replacement for sequence-design and validation tools.

hackernews · acossta · Nov 24, 21:02 · [Discussion](https://news.ycombinator.com/item?id=50634658)

**「Background」** Protein design typically proceeds in two steps: generating a desired three-dimensional backbone structure, and then finding an amino acid sequence that folds into that structure. Specialized inverse-folding models such as SolubleMPNN perform the sequence-design step, so a model that produces 3D minibinder designs still needs a downstream sequence tool before the proteins can be tested in the lab.

**「Impact」** Protein-design practitioners may use GPT-6.2 to accelerate writing code for structural design work, but they must still integrate SolubleMPNN and other specialized models for sequence generation and validation, so the model functions as an orchestrator rather than an end-to-end protein designer.

**「Community discussion」** Several commenters questioned whether GPT-6.2 actually designed the protein because SolubleMPNN generated the sequence, with one describing it as a glue layer between specialized tools. Another commenter noted the evidence seemed more computational than laboratory-validated.

**Tags**: `#AI`, `#protein design`, `#LLM`, `#bioinformatics`, `#OpenAI`

---

<a id="item-tech-news-27"></a>
### [GTA 6 Unofficial Windows Port Uses Leaked Xbox Build](https://twitter.com/raul_bs3/status/2125213756238291075) ⭐️ 7.0/10

Windows users can now run an unofficial GTA 6 port built from the leaked Xbox version. The projects xcl and VIctory take a Wine-like approach to recompile the Xbox binary, which was leaked by Cyberleek along with game resources and lacks special DRM or obfuscation. It is a community effort based on leaked material, not an official Rockstar PC release.

hackernews · andrem · Nov 24, 13:19 · [Discussion](https://news.ycombinator.com/item?id=50627783)

**「Background」** The Xbox Series X build of GTA 6 was leaked by Cyberleek, first as game resources and later as the executable. Because the Xbox environment is close to Windows, the leaked binary can run through Wine-like compatibility layers, with the main work focused on compatibility and graphics rather than full recompilation.

**「Impact」** Windows users who try the port should treat it as unsupported and legally risky; GitHub has banned the related Leonida recomp project, showing distribution is not guaranteed.

**「Community Discussion」** Some commenters argue the leak will not harm GTA 6’s commercial success, pointing to reported revenue around $4 billion against a $1–2 billion budget, while others predict publishers may shift to cloud-required components to prevent future decompilation and piracy.

**Tags**: `#reverse-engineering`, `#gaming`, `#windows`, `#compatibility`, `#open-source`

---

<a id="item-tech-news-28"></a>
### [CISA Adds Three Exploited Vulnerabilities to KEV Catalog](https://www.cisa.gov/news-events/alerts/2026/11/24/cisa-adds-three-known-exploited-vulnerabilities-catalog) ⭐️ 7.0/10

CISA added three vulnerabilities to its Known Exploited Vulnerabilities \(KEV\) Catalog based on evidence of active exploitation: CVE-2026-131914 \(Idunno AntiCsrf Deserialization of Untrusted Data\), CVE-2026-132165 \(Drupal Core Remote Code Execution\), and CVE-2026-132224 \(Optimizely Web Experimentation External Control of Critical State Data\). The alert, published November 24, 2026, states these vulnerabilities are a frequent attack vector and pose significant risks to the federal enterprise.

rss · CISA 全部安全公告 · Nov 24, 12:00

**「Background」** The KEV Catalog lists vulnerabilities with confirmed active exploitation to help organizations prioritize remediation. Binding Operational Directive \(BOD\) 26-04 requires Federal Civilian Executive Branch agencies to rapidly remediate KEV-listed CVEs on publicly exposed assets that grant total control post-exploitation, and to check whether threat actors compromised systems before a patch was applied.

**「Impact」** Federal agencies must prioritize remediation of these three vulnerabilities under BOD 26-04, and CISA encourages all organizations to adopt risk-based vulnerability management for KEV entries. Users of Drupal Core, Idunno AntiCsrf, and Optimizely Web Experimentation should treat these flaws as actively exploited and apply available vendor mitigations promptly.

**Tags**: `#cybersecurity`, `#vulnerability`, `#CISA`, `#Drupal`, `#patch management`

---

<a id="item-tech-news-29"></a>
### [AutomationDirect C-More EA9 Heap Buffer Overflow Fixed in V6.81](https://www.cisa.gov/news-events/ics-advisories/icsa-26-328-01) ⭐️ 7.0/10

CISA disclosed a heap-based buffer overflow vulnerability \(CVE-2026-127280, CVSS v3 7.8\) in AutomationDirect C-More EA9 Programming Software V6.80 and earlier. The software does not adequately validate data read from a project file, so a crafted file can overrun a heap buffer during file open, causing memory corruption and potentially arbitrary code execution if a user opens a malicious file. AutomationDirect has released V6.81 as the vendor fix.

rss · CISA 全部安全公告 · Nov 24, 12:00

**「Background」** CISA lists affected deployments in critical manufacturing, energy, and water/wastewater systems worldwide. The vulnerability is classified as CWE-122, a heap-based buffer overflow, meaning the application fails to validate project file data before heap memory operations.

**「Impact」** Users of C-More EA9 Programming Software V6.80 or earlier should update to V6.81. If updating is not possible, CISA recommends temporary compensating controls including isolating engineering workstations, restricting remote access, and scanning removable media before use.

**Tags**: `#security`, `#vulnerability`, `#ICS`, `#CISA`, `#industrial-software`

---

<a id="item-tech-news-30"></a>
### [VMware Workspace ONE Access RCE PoC Published](https://cve.now/CVE-2022-22954) ⭐️ 7.0/10

A proof-of-concept exploit for CVE-2022-22954 has been published on GitHub. The vulnerability is a server-side template injection in VMware Workspace ONE Access and Identity Manager that permits unauthenticated remote code execution over the network. It is currently being exploited in attacks, according to the report.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:11

**「Background」** Server-side template injection \(SSTI\) occurs when user-controlled input is passed to a template engine, enabling execution of attacker-supplied code on the server. Unit 42 reported that this vulnerability is trivial to exploit and can be triggered with a single HTTP request to a vulnerable device.

**「Impact」** Security teams using VMware Workspace ONE Access or Identity Manager should treat this as an urgent, actively exploited remote code execution risk and verify whether their deployments are exposed, prioritizing patching or mitigation steps from VMware.

<details><summary>References</summary>
<ul>
<li><a href="https://unit42.paloaltonetworks.com/cve-2022-22954-vmware-vulnerabilities/">Threat Brief: VMware Vulnerabilities Exploited in the Wild...</a></li>
<li><a href="https://1534169.hs-sites.com/vmware-identity-manager-attack-backdoor">VMWare Identity Manager Attack: New Backdoor Discovered</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#vulnerability`, `#remote code execution`, `#VMware`, `#server-side template injection`

---

<a id="item-tech-news-31"></a>
### [CVE-2022-21882 Win32k Privilege Escalation Gets Public Proof-of-Concept](https://cve.now/CVE-2022-21882) ⭐️ 7.0/10

A public proof-of-concept for CVE-2022-21882, a privilege escalation flaw in the Win32k component of Windows 10 and Windows Server \(including Windows Server 2019 and 2022\), has been published on GitHub. An attacker must already be able to run code with a low-privilege account and can then gain higher privileges than intended. The vulnerability is being actively exploited, so the update shifts the issue from a known CVE to one with publicly available exploit code.

rss · cve.now 新收录的 CISA KEV · Nov 25, 02:01

**「Background」** Win32k is the Windows kernel-mode graphics and windowing subsystem; a privilege escalation flaw there allows a process already running with low privileges to obtain higher, often SYSTEM-level, rights. CVE-2022-21882 is listed in CISA&\#x27;s Known Exploited Vulnerabilities catalog as actively exploited, and this update notes the additional availability of a public proof-of-concept on GitHub.

**「Impact」** The public proof-of-concept lowers the barrier for attackers who already have low-privileged code execution, making prompt patching or mitigation on affected Windows systems more urgent.

**Tags**: `#security`, `#windows`, `#vulnerability`, `#privilege-escalation`, `#exploit`

---