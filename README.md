# Blocky-Compatible Wildcard Lists

This repository exists purely for **convenience**.  
It provides domain blocklists already converted into the **wildcard asterisk (`*.domain`) format** for use with [Blocky](https://github.com/0xERR0R/blocky) (v0.23 or newer).

>[!NOTE]
>The wildcard is not strictly required by Blocky itself, but it is necessary if you want subdomains to be blocked as well. Blocky can consume plain domain lists, but in that case it only blocks the exact domain (the **apex domain**, e.g. `example.com`).
>
>- `example.com` → blocks only `example.com`  
>- `*.example.com` → blocks `example.com` and all its subdomains (`sub.example.com`, `a.b.example.com`, …)


⚠️ **Important:**  
- The blocklist data itself does **not** originate here.  
- This repo only automates fetching, converting, and publishing lists from their **original sources**.  
- All credit remain with the upstream projects.

---

## 📂 Repository Structure

### `NRD/`
Contains **Newly Registered Domain (NRD)** lists converted to wildcard format from multiple upstreams.

- **Hagezi NRD**  
  Source: [hagezi/dns-blocklists](https://github.com/hagezi/dns-blocklists)  
  Files:  
  - [nrd7_asterisk.txt](https://cebeerre.github.io/dnsblocklists/NRD/nrd7_asterisk.txt) → Domains registered in the **last 7 days**.  
  - [nrd14-8_asterisk.txt](https://cebeerre.github.io/dnsblocklists/NRD/nrd14-8_asterisk.txt) → Domains registered **between day 14 and day 8 ago**.

- **DNSBunker NRD**  
  Source: [xRuffKez/NRD (DNSBunker)](https://codeberg.org/xRuffKez/NRD)  
  Files:  
  - [nrd14_wildcard_dnsbuker.txt](https://cebeerre.github.io/dnsblocklists/NRD/nrd14_wildcard_dnsbuker.txt) → Domains registered in the **last 14 days**.

### `webservices/`
- Contains one file per web service, each in wildcard format.  
- Source: [AdGuardTeam/HostlistsRegistry](https://github.com/AdguardTeam/HostlistsRegistry).

<!-- BEGIN:SERVICES_TABLE -->
<!-- END:SERVICES_TABLE -->

> [!NOTE]  
> Each generated list may include a section labeled **“Skipped unsupported rules”**.  
> These lines come directly from the AdGuard upstream sources but cannot be expressed in Blocky’s wildcard format.  
> Examples include:
> - Wildcards inside labels (e.g., `||awsdns-*.tld^`)  
> - Single-pipe Adblock anchors (e.g., `|domain^`, likely typos for `||domain^`)  
> - Service discovery / mDNS / SRV records (with underscores or `.local`)  
> - Rules containing slashes, schemes, or parameters  
>
> Skipped rules are shown in the file header for transparency but are **not included** in the active blocklist.  

---

## 🔄 How It Works

- GitHub Actions workflows run on a schedule:  
  - **NRD lists** → refreshed **daily**.  
  - **Webservices lists** → refreshed **weekly**.  
- The workflows:  
  1. Fetch the upstream lists in their original formats.  
  2. Convert them into `*.domain` wildcard format.  
  3. Publish them here under `NRD/` or `webservices/`.  
