# Awesome-Content-Ad-Blocking

# Top Content & Ad Blocking Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on DNS Sinkholing, Browser Extension Filtering & Network-Wide Privacy*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Content & Ad Blocking**. These tools enable individuals and organizations to block ads, trackers, malware domains, and unwanted content—from browser extensions that filter requests at the page level to network-wide DNS sinkholes that protect every device on your network without per-device configuration.

**Examples** include AdGuard Premium, NextDNS, Pi-hole, Control D, Brave Shields, Ghostery, 1Blocker, AdLock, CleanBrowsing, and uBlock Origin (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, DNS-level blocking, and open filtering engines—ideal for privacy-conscious users, homelab enthusiasts, and organizations seeking transparent, vendor-independent content filtering.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[AdGuard Premium](https://adguard.com/en/adguard-adblocker/overview.html)**  
  **The best full-system ad blocker**—**blocks ads in all applications, not just browsers** . AdGuard Desktop (macOS/Windows) intercepts ad requests at the network level before they reach any application—streaming apps, social media apps, and games included. **AdGuard Home** is the free, self-hosted DNS-level alternative for network-wide blocking . **The most comprehensive commercial option** for users who want ad-free experiences everywhere, not just in the browser.

- **[NextDNS](https://nextdns.io/)**  
  **Cloud-based DNS filtering** with ad blocking, tracker blocking, and parental controls. Features **per-device configuration**, **encrypted DNS (DoH/DoT)**, and **detailed analytics**. **The most flexible managed DNS filtering service**—works on any device that supports custom DNS.

- **[Control D](https://controld.com/)**  
  **Privacy-first DNS filtering** with ad blocking, malware protection, and custom rules. Features **encrypted DNS**, **per-profile configuration**, and **geographic content unblocking**.

- **[Brave Shields](https://brave.com/shields/)**  
  **Built-in ad and tracker blocking** in the Brave browser. Features **fingerprinting protection**, **HTTPS upgrades**, and **private search**. **The most seamless integrated blocking**—no extension required.

- **[Ghostery](https://www.ghostery.com/)**  
  **Privacy-focused tracker blocker** with ad blocking, cookie management, and **Ghostery Private Browser**. Features **transparent tracker detection** and **custom blocking rules**.

- **[CleanBrowsing](https://cleanbrowsing.org/)**  
  **DNS filtering service** for families and organizations. Features **content filtering**, **malware protection**, and **encrypted DNS**. **The most focused on parental controls** and content policy enforcement.

- **[1Blocker](https://1blocker.com/)**  
  **Powerful Safari content blocker** for iOS and macOS. Features **custom rules**, **element hiding**, and **script blocking**. **The best Safari-native option** for Apple users.

- **[AdLock](https://adlock.com/)**  
  **Cross-platform ad blocker** with browser extension and system-wide filtering. Features **YouTube ad blocking**, **anti-adblock circumvention**, and **battery-saving mode**.

## Open-Source GitHub Projects

- **[uBlock Origin](https://github.com/gorhill/uBlock)**  
  **High-efficiency, open-source content and ad blocker** (GPL-3.0) . **The gold standard for browser ad blocking**—created by Raymond Hill (gorhill) and widely regarded as one of the most trustworthy and effective ad-blocking extensions available . **65,524 GitHub stars** . **Key advantages**: **completely free with no "acceptable ads" program**—blocks all ads, not just non-paying advertisers' . **Uses 80-90% less memory than AdBlock Plus** while blocking more requests . **Critical 2026 consideration**: **Full functionality is only available in Firefox**—Google's Manifest V3 transition limits content blockers in Chrome, forcing the creation of **uBlock Origin Lite** with reduced capabilities . **Mozilla has committed to supporting Manifest V2 in Firefox**, making **Firefox + uBlock Origin the strongest combination for comprehensive tracker blocking** . **The reference implementation for browser content blocking**.

- **[Pi-hole](https://github.com/pi-hole/pi-hole)**  
  **A black hole for Internet advertisements** (EUPL-1.2) . **The original network-wide DNS ad blocker**—**50,000+ GitHub stars** and the largest community in self-hosted DNS filtering . **Network-wide blocking for every device on your network**—smart TVs, game consoles, smart home devices—without per-device configuration . **Features**: **detailed query log dashboard**, **group-based filtering per client**, **long-term query retention (years)**, **local DNS records**, and **DHCP server** . **Limitations**: **no built-in encrypted DNS (DoH/DoT)**—requires **Unbound** or **cloudflared** sidecar for encrypted upstream queries . **Higher resource usage (~120-180 MB RAM, ~300 MB Docker image)** . **The reference implementation for DNS sinkholing**.

- **[AdGuard Home](https://github.com/AdguardTeam/AdGuardHome)**  
  **Network-wide software for blocking ads and tracking** (GPL-3.0) . **The modern all-in-one DNS ad blocker**—**the most complete self-hosted solution** . **Native DoH/DoT/DoQ/DNSCrypt**—no sidecar services required . **Features**: **clean modern web UI**, **per-client filtering rules**, **DHCP server**, **parental controls + Safe Search enforcement**, **DNS rewrites for local network**, and **low resource usage (~60-80 MB RAM)** . **Single container deployment** . **Limitations**: **no built-in Prometheus metrics** (uses custom stats API), **no native multi-instance sync**, and **smaller community than Pi-hole** . **Best for**: most users—the best balance of features, simplicity, and resource usage .

- **[Blocky](https://github.com/0xERR0R/blocky)**  
  **Fast and lightweight DNS proxy as ad-blocker for local network** (Apache-2.0) . **The best lightweight / config-as-code DNS ad blocker**—**5,509 GitHub stars** . **~10-30 MB RAM and 15 MB Docker image**—the lightest option available . **YAML configuration**—version-control friendly, reproducible, **infrastructure-as-code practitioners' choice** . **Native DoH/DoT**—no add-ons required . **Built-in DNSSEC validation**, **Prometheus metrics**, **multi-instance sync via Redis**, and **per-client filtering in config** . **Runs from scratch image (minimal attack surface)** . **Limitations**: **no web UI (API only)**, **no DHCP server**, and **smaller community** . **Best for**: infrastructure-as-code users, resource-constrained hardware, and users who don't need a web dashboard .

- **[Technitium DNS Server](https://github.com/TechnitiumSoftware/DnsServer)**  
  **The DNS server that replaces Pi-hole, Unbound, and BIND** (GPL-3.0) . **The most comprehensive open-source DNS server**—**recursive resolver, sinkhole with blocklists, and authoritative zone server all in one process** . **Features**: **DoH/DoT/DoQ support**, **full DNSSEC (RSA, ECDSA, EdDSA, NSEC/NSEC3, DANE TLSA)**, **AXFR/IXFR zone transfers**, **Tor routing for forwarders**, **multi-network DHCP**, **clustering**, **SSO via OpenID Connect**, **TOTP 2FA**, and **built-in apps for DNS64, DNS Rebinding Protection, and Advanced Forwarding** . **Performance**: **100,000+ requests/second on Gigabit Ethernet**; **~200-300 MB RAM under load with Hagezi Pro (750,000 entries)** on Raspberry Pi 4 . **Web console** with Quick Add for popular blocklists (Hagezi) and **per-client/subnet blocking rules** . **Limitations**: **Windows 10/11 port 53 conflicts** (Internet Connection Sharing, Hyper-V, Docker Desktop, Defender Application Guard all fight for the port) . **Best for**: users who want DNS sinkholing, recursive resolution, and zone hosting in one tool .

- **[zdns](https://github.com/mpolden/zdns)**  
  **Privacy-focused DNS resolver and DNS sinkhole** (MIT) . **The minimal, portable DNS sinkhole**—**controls filtering at DNS level, similar to Pi-hole** . **Features**: **parallel resolving over multiple resolvers**, **efficient filtering and caching**, **DNS over TLS or DNS over HTTPS for upstream resolvers**, **zero run-time dependencies**, **DNS logging**, and **metrics** . **Runs on all platforms supported by Go**—VPS, container, laptop, Raspberry Pi, or home router . **REST API** for log and cache access . **Limitations**: **exact-domain matching only** (no regex support in current version), **SQLite-based logging** . **Best for**: users who want a simple, portable DNS sinkhole without Pi-hole's dependencies and feature scope .

- **[refunnel-rs](https://github.com/DavidMANZI-093/refunnel-rs)**  
  **A fast, lightweight DNS sinkhole written in Rust** (open-source) . **The Rust-native DNS sinkhole**—**blocks ads, trackers, and malware at the DNS layer** . **Features**: **DNS sinkhole returning `0.0.0.0`/`::` for blocked domains**, **StevenBlack-compatible blocklist (120,000+ domains out of the box)**, **LRU response cache (10,000 entries)**, **Cloudflare upstream (1.1.1.1:53)**, and **structured logging** . **Async core built on Tokio**—handles concurrent queries without blocking . **systemd service** with dedicated unprivileged user and minimal capabilities . **Limitations**: **exact-domain matching only**, **blocklist loaded once at startup (requires restart to update)**, **no web UI** . **Best for**: Rust users who want a minimal DNS sinkhole with fast lookups.

- **[sagittarius](https://github.com/LHelge/sagittarius)**  
  **A self-hosted DNS sinkhole (like Pi-hole / AdGuard Home), written in Rust and shipped as a single self-contained binary** (open-source) . **The modern Rust DNS sinkhole with web UI**—**DNS engine, storage, and web admin UI all included** . **Features**: **subscribable blocklists (hosts/domain-list formats)**, **manual allow/deny lists**, **per-list effectiveness tracking**, **pause blocking (5 min / 30 min / 1h / custom)**, **live query log and dashboard streamed over SSE**, **persistent query log (configurable retention, default 30 days)**, **encrypted upstreams (DoH/DoT) with selectable strategy**, **local DNS records with wildcards**, **reverse DNS for LAN**, and **conditional forwarding for private reverse zones** . **Architecture**: **Tokio async runtime**, **Tower middleware (rate limiting, backpressure)**, **custom DNS wire format parser**, **SQLite via sqlx**, **HashSet blacklist + HashMap blocklist with arc-swap hot-swapping**, **moka cache with TTL** . **Single binary install via systemd script** . **Best for**: users who want a Rust-native DNS sinkhole with a modern web UI and persistent query history.

- **[donutdns](https://github.com/shoenig/donutdns)**  
  **Block ads, trackers, and malicious sites with donutdns - simple alternative to pihole** (open-source) . **86 GitHub stars** . **Runs as a Docker container, standalone executable, or CoreDNS plugin** . **Supplies custom domain block/allow lists in addition to builtin lists** maintained by the ad-blocking community . **Best for**: users who want a simple, flexible DNS sinkhole that integrates with existing CoreDNS infrastructure.

- **[ha-sinkhole](https://github.com/radiusred/ha-sinkhole)**  
  **Local DNS sinkhole server, inspired by pi-hole but designed to be highly available** (open-source) . **The high-availability DNS sinkhole**—**uses VRRP to share a floating VIP among multiple nodes** . **Configuration: all DNS clients point to the VIP, and as long as at least one node is alive, DNS and sinkhole service remains operational** . **Minimum two machines for HA, more can be added for additional resilience** . **Works on Raspberry Pi, bare metal servers, local VMs, cloud instances, or a mixture** . **Ansible-based remote installer** with flexible node layout definition . **Limitations**: **container deployment unlikely to succeed**, **requires passwordless SSH and passwordless sudo on target nodes** . **Best for**: homelabs and small organizations that need DNS filtering to survive node failures.

### Additional Strong Open-Source Options

- **[Cloudflare Gateway Pi-hole Scripts (CGPS)](https://github.com/mrrfv/cloudflare-gateway-pihole-scripts)** — Use Cloudflare Gateway DNS/VPN to block ads, malware and tracking domains—free alternative to NextDNS, Pi-hole and AdGuard . **No servers to maintain, no Raspberry Pi to buy**—scripts create Cloudflare Gateway lists and rules from blocklist files . **Supports hosts files and domain lists**, **allowlist support**, **experimental SNI-based filtering**, and **GitHub Actions for automatic updates** . **Free plan supports up to 300,000 domains** . **Best for**: users who want Pi-hole-like filtering without running any infrastructure.
- **[AdGuard Filters](https://github.com/AdguardTeam/AdguardFilters)** — Curated adblock filter lists, content blocking rulesets, and DNS blocklists (GPL-3.0) . **The filter lists powering AdGuard products**—including specialized rules for cosmetic filtering, malware domains, and regional blocking .
- **[Jev Ad Block](https://github.com/lingengyuan/jev-adblock)** — Chrome MV3 ad blocker using Jev (TypeSafe System One) for semantic element judgment (GPL-3.0) . **The AI-powered ad blocker**—network rules block ad requests, content scripts hand candidate elements to Jev for semantic judgment, with local-rule fallback when API key is unavailable . **Community rules from EasyList China + CJX's Annoyance List** . **Best for**: users who want semantic ad detection beyond static filter lists.
- Community **n8n** workflows for DNS query monitoring and blocklist update automation.

**Frameworks for building custom systems**: Combine **AdGuard Home** for the most complete self-hosted DNS blocking experience with **Blocky** for config-as-code infrastructure, **Technitium** for recursive resolution and zone hosting, **uBlock Origin** for browser-level filtering, and **Pi-hole** for the largest community and integration ecosystem—creating a comprehensive content and ad blocking stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Content and ad blocking tools must respect website terms of service and applicable regulations. **Some jurisdictions are considering criminalizing browser-side blockers** . **Use responsibly and in compliance with local laws.**
- **Open-source ad blocking is mature and production-ready.** uBlock Origin is the gold standard for browser blocking with 29M+ Chrome users and 10M+ Firefox users . AdGuard Home is the most complete self-hosted DNS blocker . Pi-hole has the largest community and most integrations . **These are genuine alternatives to commercial platforms.**
- **The Manifest V3 transition is the critical 2026 consideration.** **Full uBlock Origin functionality is only available in Firefox**—Chrome's Manifest V3 replaces dynamic blocking APIs with a static declarative rule system that cannot match uBlock Origin's engine flexibility . **Mozilla has committed to supporting Manifest V2 in Firefox**, making **Firefox + uBlock Origin the strongest combination for comprehensive tracker blocking** . **On Chrome and Edge, uBlock Origin Lite provides reduced but meaningful protection** .
- **DNS-level vs. browser-level blocking serve different purposes.** **DNS sinkholes (Pi-hole, AdGuard Home, Blocky)** block requests before they leave your network—**protects every device including smart TVs, game consoles, and IoT devices** that cannot run extensions . **Browser extensions (uBlock Origin)** provide cosmetic filtering, element hiding, and script control that DNS blocking cannot . **The best setup combines both.**
- **The self-hosted DNS landscape has clear specializations.** **AdGuard Home** for the best all-in-one experience with native encrypted DNS . **Pi-hole** for the largest community and most integrations . **Blocky** for config-as-code infrastructure and minimal resource usage . **Technitium** for recursive resolution and zone hosting in addition to blocking . **Choose based on your operational model, not feature checklists**.
- **Free cloud alternatives exist.** Cloudflare Gateway Pi-hole Scripts provide Pi-hole-like filtering with **no servers to maintain and no Raspberry Pi to buy**—the free plan supports up to 300,000 domains . **Best for**: users who want network-wide blocking without running any infrastructure.
- Self-hosted open-source solutions require proper DNS configuration, blocklist curation, and ongoing maintenance. **Blocklist quality determines filtering effectiveness**—**StevenBlack/hosts** provides a curated base list (120,000+ domains) aggregated from multiple trusted sources . **Hagezi lists** are recommended for comprehensive coverage .

---

**Made for privacy-conscious users, homelab enthusiasts, and organizations building transparent content filtering solutions.**  
Let's make Content & Ad Blocking more open, data-driven, and network-wide.
