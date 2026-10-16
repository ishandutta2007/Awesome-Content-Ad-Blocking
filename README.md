<div align="center">

<img src="./assets/banner.svg" alt="Awesome Content &amp; Ad Blocking Banner" width="100%" />

# 🛡️ Awesome Content & Ad Blocking: DNS Sinkholes, Privacy Resolvers & Browser Extensions 🚫

<a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a><a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
<a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://awesome.re/badge.svg" alt="Awesome List"/></a>
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License: MIT"/></a>
<a href="#-table-of-contents"><img src="https://img.shields.io/badge/Tracked%20Projects-25%2B-brightgreen.svg" alt="Tracked Projects"/></a>
<a href="#"><img src="https://img.shields.io/badge/Last%20Updated-October%202026-blue.svg" alt="Last Updated"/></a>
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>

<p align="center">
  <strong>Curated ecosystem of SaaS platforms, DNS sinkholes, privacy resolvers, and open-source ad blockers.</strong><br>
  <em>Focused on DNS Sinkholing, Manifest V3 / V2 Browser Filtering, Network-Wide Privacy, and Ad-Free Infrastructure.</em>
</p>

</div>

---

## 📌 Overview

This repository indexes the content and ad blocking landscape across commercial **SaaS platforms**, **cloud encrypted DNS resolvers**, and community-driven **open-source projects**. These tools empower individuals, homelabs, and enterprises to block intrusive advertisements, stop telemetry trackers, prevent phishing/malware domains, and bypass aggressive anti-adblock mechanisms.

Whether you are configuring network-wide protection via DNS sinkholes ([Pi-hole](https://github.com/pi-hole/pi-hole), [AdGuard Home](https://github.com/AdguardTeam/AdGuardHome)) or page-level cosmetic filtering via browser extensions ([uBlock Origin](https://github.com/gorhill/uBlock)), this guide tracks key architectural trade-offs, pricing models, company valuations, and repository adoption metrics.

---

## 📑 Table of Contents

- [📊 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [☁️ SaaS & Hosted Ad Blocking Platforms](#️-saas--hosted-ad-blocking-platforms)
- [💻 Open-Source GitHub Projects](#-open-source-github-projects)
- [⚖️ Architectural Comparison: DNS Sinkholing vs. Browser Extension Filtering](#️-architectural-comparison-dns-sinkholing-vs-browser-extension-filtering)
- [⭐ Star History](#-star-history)
- [💖 Support & Sponsorship](#-support--sponsorship)
- [🤝 How to Contribute](#-how-to-contribute)
- [⚠️ Disclaimer & Regulatory Notes](#️-disclaimer--regulatory-notes)

---

## 📊 Sector Overview & Market Dynamics

The global ad blocking software market is estimated at **$3.5B – $4.3B** (projected to reach **$7.5B – $11.5B** by the early 2030s at a **CAGR of ~11.5%**), driven by increasing user privacy regulations (GDPR, CCPA), surging mobile and smart TV ad density, and browser-engine shifts such as Chromium's Manifest V3. The sector remains **highly fragmented** across direct-to-consumer mobile utilities, cloud encrypted DNS resolvers (DoH/DoT/DoQ), corporate network firewalls, and deeply entrenched open-source filter engines, where no single vendor holds a monopoly or "winner-take-all" advantage due to strong user commitment to open community filter rulesets (e.g., EasyList, StevenBlack, Hagezi).

---

## ☁️ SaaS & Hosted Ad Blocking Platforms

Below is a comparison of commercial and hosted ad-blocking, privacy DNS, and system-wide content filtering solutions. Companies are sorted in descending order by **Company Scale (Valuation / Revenue)**.

| SaaS / Product Name | Starting Tier Price | Free Tier / Trial Limits | Company Scale (Valuation / Revenue) | Core Features & Deployment |
| :--- | :--- | :--- | :--- | :--- |
| **[Ghostery](https://www.ghostery.com/)** | **$1.99 / month** (Optional Contributor tier; core extension is 100% free) | **Free forever plan**: Unlimited tracker & ad blocking, cookie consent auto-rejection, and open-source browser on all devices | **€2.66 Billion (~$2.9B) Revenue** (Parent: Hubert Burda Media) | Tracker intelligence, anti-tracking script blocking, cookie pop-up elimination, and privacy-first browser engine. |
| **[Brave Shields](https://brave.com/shields/)** | **$9.99 / month** (Brave Firewall + VPN; built-in Shields engine is 100% free) | **Free forever plan**: Built directly into Brave browser with unlimited cosmetic ad, tracker, and fingerprinting blocking across desktop & mobile | **$980 Million Valuation** (~$52M–$100M ARR; 100M+ MAU) | Integrated native Rust/C++ network request blocking, fingerprint randomization, bounce tracking mitigation, and Brave Search privacy. |
| **[AdGuard Premium](https://adguard.com/en/adguard-adblocker/overview.html)** | **$2.49 / month** (AdGuard DNS Personal) or **$2.49 / month** ($29.88/yr Personal App License) | **14-day full free trial** for standalone desktop/mobile apps; **Free forever tier for AdGuard DNS** capped at **300,000 queries/month** (2 devices, 1 server) | **~$5.4 Million Annual Revenue** (Profitable, bootstrapped; 150M+ users) | Full-system network socket filtering (intercepts in-app, game, and streaming ads), cosmetic DOM hiding, and cloud DoH/DoT/DoQ profiles. |
| **[1Blocker](https://1blocker.com/)** | **$2.99 / month** or **$14.99 / year** ($39.99 Lifetime) | **Free forever plan**: Allows activating any 1 functional rule category at a time (e.g., Block Ads only or Block Trackers only) across iOS and macOS | **~$2.0 Million Estimated Revenue** (Independent consumer app leader) | Native Apple Safari Content Blocking API integration, local processing with zero battery drain, custom rule generation, and iCloud sync. |
| **[Control D](https://controld.com/)** | **$3.00 / month** ($30/year "Some Control" plan) | **14-day full free trial** (no credit card required); **Free forever tier**: Unlimited DNS queries using pre-configured public DNS IP profiles (no custom web dashboard) | **~$1.0 Million Estimated ARR** (Spin-off from Windscribe VPN) | Modern encrypted DNS (DoH/DoT/Do3), 15+ native filter lists, granular scheduling, per-device service blocking, and optional geo-proxy IP routing. |
| **[NextDNS](https://nextdns.io/)** | **$1.99 / month** or **$19.90 / year** (Pro plan) | **Free forever plan**: **300,000 DNS queries/month** with unlimited devices and full configuration; seamlessly falls back to non-blocking DNS after limit | **Bootstrapped** (Est. sub-$1M ARR; 1M+ active endpoints) | Cloud-hosted customizable DNS sinkhole, per-client analytics, parental control categories, safe search enforcement, and DoH/DoT/DoQ support. |
| **[CleanBrowsing](https://cleanbrowsing.org/)** | **$4.99 / month** (billed $59.99/year Basic Plan) | **Free forever plan**: 3 pre-configured public Anycast DNS resolver pairs (Security, Adult, and Family Filter) with unlimited DNS queries | **~$330,000 Estimated ARR** (Specialized family & education cybersecurity) | Family safety and institutional DNS filtering, automated adult domain sinkholing, phishing defense, and enforced Google/Bing SafeSearch. |
| **[AdLock](https://adlock.com/)** | **$1.05 / month** (multi-year billing) or **$3.50 / month** ($24.99 Lifetime deals) | **14-day free trial** for Windows/Android apps (full functionality, 1 device); **Free forever plan** for standard browser extension | **Independent / Bootstrapped** (Micro-ISV) | System-wide daemon blocking ads inside games, Skype, and apps; anti-adblock circumvention scripts; and HTTPS traffic scanning. |

---

## 💻 Open-Source GitHub Projects

Curated open-source DNS sinkholes, filtering proxies, and browser extensions. Repositories are sorted in descending order by **GitHub Star Counts** with linked star badges.

| Repository | Stars | License | Primary Role & Description |
| :--- | :--- | :--- | :--- |
| **[uBlock Origin](https://github.com/gorhill/uBlock)** | [![GitHub stars](https://img.shields.io/github/stars/gorhill/uBlock?style=social&color=white)](https://github.com/gorhill/uBlock/stargazers) | `GPL-3.0` | **Gold-standard browser extension content blocker**. Created by Raymond Hill (`gorhill`). Memory-efficient CPU/RAM footprint with deep procedural DOM cosmetic filtering, dynamic script injection blocking, and zero commercial "Acceptable Ads" compromises. |
| **[Pi-hole](https://github.com/pi-hole/pi-hole)** | [![GitHub stars](https://img.shields.io/github/stars/pi-hole/pi-hole?style=social&color=white)](https://github.com/pi-hole/pi-hole/stargazers) | `EUPL-1.2` | **The foundational network-wide DNS sinkhole**. Intercepts DNS queries for all local network devices (Smart TVs, IoT, mobile) with detailed web dashboard analytics, FTLDNS engine, group filtering, DHCP server, and massive homelab community support. |
| **[AdGuard Home](https://github.com/AdguardTeam/AdGuardHome)** | [![GitHub stars](https://img.shields.io/github/stars/AdguardTeam/AdGuardHome?style=social&color=white)](https://github.com/AdguardTeam/AdGuardHome/stargazers) | `GPL-3.0` | **Modern all-in-one network DNS sinkhole & DoH/DoT server**. Shipped as a self-contained Go binary with native upstream encryption (DoH, DoT, DoQ, DNSCrypt), parental control toggles, DNS rewrites, and per-client rule assignments. |
| **[StevenBlack/hosts](https://github.com/StevenBlack/hosts)** | [![GitHub stars](https://img.shields.io/github/stars/StevenBlack/hosts?style=social&color=white)](https://github.com/StevenBlack/hosts/stargazers) | `MIT` | **Consolidated hosts file for DNS and system-level blocking**. Aggregates, de-duplicates, and validates 120,000+ domain entries across reputable community blocklists with optional extension categories (porn, social, gambling, fake news). |
| **[Hagezi DNS Blocklists](https://github.com/hagezi/dns-blocklists)** | [![GitHub stars](https://img.shields.io/github/stars/hagezi/dns-blocklists?style=social&color=white)](https://github.com/hagezi/dns-blocklists/stargazers) | `GPL-3.0` | **Comprehensive multi-tiered DNS filter lists**. Curated to minimize false positives across Light, Multi Normal, Multi Pro, and Ultimate tiers; compatible with Pi-hole, AdGuard Home, Technitium, NextDNS, and Unbound. |
| **[Technitium DNS Server](https://github.com/TechnitiumSoftware/DnsServer)** | [![GitHub stars](https://img.shields.io/github/stars/TechnitiumSoftware/DnsServer?style=social&color=white)](https://github.com/TechnitiumSoftware/DnsServer/stargazers) | `GPL-3.0` | **Enterprise-grade authoritative & recursive DNS resolver with sinkhole engine**. Built in C# .NET with native DNSSEC, DoH/DoT/DoQ forwarders, multi-network DHCP, clustering, and high-throughput query handling (100k+ QPS). |
| **[Blocky](https://github.com/0xERR0R/blocky)** | [![GitHub stars](https://img.shields.io/github/stars/0xERR0R/blocky?style=social&color=white)](https://github.com/0xERR0R/blocky/stargazers) | `Apache-2.0` | **Ultra-lightweight Go DNS proxy and ad blocker**. Tailored for GitOps and Infrastructure-as-Code workflows via clean YAML configuration, Prometheus metrics, Redis multi-instance sync, and ~15MB scratch Docker deployment. |
| **[Bromite](https://github.com/bromite/bromite)** | [![GitHub stars](https://img.shields.io/github/stars/bromite/bromite?style=social&color=white)](https://github.com/bromite/bromite/stargazers) | `GPL-3.0` | **Customized Chromium browser with built-in ad blocking & privacy enhancements**. Hardened for Android with fine-grained tracking protection and fast content filtering engine patches. |
| **[AdGuard Filters](https://github.com/AdguardTeam/AdguardFilters)** | [![GitHub stars](https://img.shields.io/github/stars/AdguardTeam/AdguardFilters?style=social&color=white)](https://github.com/AdguardTeam/AdguardFilters/stargazers) | `GPL-3.0` | **Comprehensive ad blocking and privacy rulesets**. Powers AdGuard apps, extensions, and DNS; contains specialized cosmetic rules, anti-annoyance filters, mobile-specific rules, and URL tracking parameter removers. |
| **[AdGuard Browser Extension](https://github.com/AdguardTeam/AdguardBrowserExtension)** | [![GitHub stars](https://img.shields.io/github/stars/AdguardTeam/AdguardBrowserExtension?style=social&color=white)](https://github.com/AdguardTeam/AdguardBrowserExtension/stargazers) | `LGPL-3.0` | **Full-featured open-source browser extension**. Capable of handling sophisticated cosmetic rules, scriptlet injection, cookie notice removal, and filtering on Chromium, Firefox, and Safari. |
| **[Brave Core](https://github.com/brave/brave-core)** | [![GitHub stars](https://img.shields.io/github/stars/brave/brave-core?style=social&color=white)](https://github.com/brave/brave-core/stargazers) | `MPL-2.0` | **Core engine for Brave Browser**. Integrates custom Rust network-filtering libraries (`ad-block`) that match EasyList/uBlock rules natively at the network stack before HTTP requests are dispatched. |
| **[Cloudflare Gateway Pi-hole Scripts (CGPS)](https://github.com/mrrfv/cloudflare-gateway-pihole-scripts)** | [![GitHub stars](https://img.shields.io/github/stars/mrrfv/cloudflare-gateway-pihole-scripts?style=social&color=white)](https://github.com/mrrfv/cloudflare-gateway-pihole-scripts/stargazers) | `MIT` | **Serverless cloud ad blocker using Cloudflare Zero Trust Gateway**. Python automation scripts converting Pi-hole / hosts blocklists into Cloudflare Gateway firewall rules (protecting up to 300,000 domains on the free plan). |
| **[uBlock Origin (Firefox Legacy)](https://github.com/gorhill/uBlock-for-firefox-legacy)** | [![GitHub stars](https://img.shields.io/github/stars/gorhill/uBlock-for-firefox-legacy?style=social&color=white)](https://github.com/gorhill/uBlock-for-firefox-legacy/stargazers) | `GPL-3.0` | **uBlock Origin for legacy XUL Firefox and forks** (Waterfox, Pale Moon, Basilisk). Maintained for classic browser engine architectures with raw webRequest access. |
| **[donutdns](https://github.com/shoenig/donutdns)** | [![GitHub stars](https://img.shields.io/github/stars/shoenig/donutdns?style=social&color=white)](https://github.com/shoenig/donutdns/stargazers) | `Apache-2.0` | **Modular DNS sinkhole and CoreDNS plugin**. Runs as a standalone container or CoreDNS module; supports community domain lists, zero-configuration defaults, and lightweight memory consumption. |
| **[zdns](https://github.com/mpolden/zdns)** | [![GitHub stars](https://img.shields.io/github/stars/mpolden/zdns?style=social&color=white)](https://github.com/mpolden/zdns/stargazers) | `MIT` | **Minimalist Go DNS sinkhole & caching resolver**. Features parallel upstream queries, DNS-over-TLS/HTTPS upstreams, zero external runtime dependencies, and lightweight SQLite query logging. |
| **[refunnel-rs](https://github.com/DavidMANZI-093/refunnel-rs)** | [![GitHub stars](https://img.shields.io/github/stars/DavidMANZI-093/refunnel-rs?style=social&color=white)](https://github.com/DavidMANZI-093/refunnel-rs/stargazers) | `GPL-3.0` | **High-performance async DNS sinkhole in Rust**. Built on Tokio with StevenBlack hosts integration, memory LRU cache, and fast zero-latency `0.0.0.0` blocking before queries leave the network. |
| **[sagittarius](https://github.com/LHelge/sagittarius)** | [![GitHub stars](https://img.shields.io/github/stars/LHelge/sagittarius?style=social&color=white)](https://github.com/LHelge/sagittarius/stargazers) | `GPL-3.0` | **Single-binary Rust DNS sinkhole with embedded Web UI**. Features live SSE query logs, customizable retention, hot-swapping blocklists with `arc-swap`, and encrypted DoH/DoT upstream forwarders. |
| **[ha-sinkhole](https://github.com/radiusred/ha-sinkhole)** | [![GitHub stars](https://img.shields.io/github/stars/radiusred/ha-sinkhole?style=social&color=white)](https://github.com/radiusred/ha-sinkhole/stargazers) | `MIT` | **High-availability DNS sinkhole cluster**. Uses Keepalived and VRRP to share a floating Virtual IP (VIP) across multiple Pi-hole / DNS nodes, preventing single-point DNS network failure. |
| **[Jev Ad Block](https://github.com/lingengyuan/jev-adblock)** | [![GitHub stars](https://img.shields.io/github/stars/lingengyuan/jev-adblock?style=social&color=white)](https://github.com/lingengyuan/jev-adblock/stargazers) | `GPL-3.0` | **Manifest V3 semantic AI ad blocker**. Combines static declarative network rules with AI semantic element analysis to recognize obfuscated advertisements that traditional regex filter lists miss. |

---

## ⚖️ Architectural Comparison: DNS Sinkholing vs. Browser Extension Filtering

| Capability / Threat Vector | DNS Sinkhole (Pi-hole, AdGuard Home, NextDNS) | Browser Content Blocker (uBlock Origin, Brave) |
| :--- | :--- | :--- |
| **Scope of Protection** | **Entire Network & All Devices** (IoT, Smart TVs, Phones, Game Consoles) | **Browser Tab Only** (Single browser profile) |
| **Setup Overhead** | Router DHCP / DNS configuration or local server deployment | 1-click browser extension install |
| **Cosmetic Filtering & Blank Space Hiding** | ❌ Cannot alter HTML/CSS; leaves collapsed or blank ad spaces | ✅ Fully removes white space, sponsored banners, and DOM containers |
| **First-Party & CNAME Cloaked Tracking** | ❌ Often cannot distinguish first-party subdomains from CDN assets | ✅ Inspects HTTP request context and removes third-party scriptlet execution |
| **Streaming / In-App Video Ads (YouTube/Twitch)** | ❌ Fails when ads and content originate from the same CDN domain | ✅ Injects player scriptlets and intercepts streaming manifest payloads |
| **Manifest V3 Resistance** | ✅ 100% immune to browser engine API changes | ⚠️ Chromium restricts dynamic declarativeNetRequest rules; Firefox maintains MV2 |

> 💡 **Recommended Strategy**: Combine an upstream **DNS Sinkhole** (e.g., [AdGuard Home](https://github.com/AdguardTeam/AdGuardHome) or [NextDNS](https://nextdns.io/)) for baseline network-wide telemetry blocking with **[uBlock Origin](https://github.com/gorhill/uBlock) on Firefox** for in-depth cosmetic element hiding and anti-circumvention protection.

---

## 🤝 How to Contribute

We welcome additions and updates from developers, homelab maintainers, and privacy advocates:

1. 🍴 **Fork the repository** to your personal GitHub account.
2. 🔍 Ensure your proposed project or platform fits Content/Ad Blocking, DNS filtering, or Anti-Tracking.
3. 📝 Follow the established markdown table format with accurate pricing, free tier limits, company revenue/valuation details, and linked GitHub star badges.
4. 🚀 Test markdown formatting and submit a clear Pull Request.

---

## ⭐ Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-Content-Ad-Blocking&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-Content-Ad-Blocking&type=date&legend=top-left)

---

## 💖 Support & Sponsorship

Thank you for visiting and using **Awesome-Content-Ad-Blocking**! 🎉 

If this curated repository helped you find the right ad blocker, secure your homelab DNS, or enhance your online privacy:
- ⭐ **Star this repository** to help others discover it!
- 🍴 **Fork and contribute** new open-source tools and filter lists.
- 📢 **Share this project** with friends, colleagues, and homelab communities.
- ☕ **Buy me a coffee**: Support ongoing curation and maintenance via the [GitHub Sponsor Dashboard](https://github.com/sponsors/ishandutta2007).

---

## ⚠️ Disclaimer & Regulatory Notes

- ⚖️ This repository is a community-maintained index for privacy research and educational purposes.
- 📜 Content blocking tools should be configured responsibly in compliance with local laws and target service agreements.
- 🛡️ While commercial ad tech continues to adapt through server-side ad insertion (SSAI) and browser Manifest V3 constraints, open-source filter lists and independent resolvers remain resilient, transparent alternatives to data-harvesting networks.
