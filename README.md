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
- **All credit remains with the upstream projects**.

---

## 🆕 Newly Registered Domains (NRD)

Blocklists of **newly registered domains**, which are often abused for malicious activity (phishing, malware distribution, scams).  

| 🔒 | Source | Description | Link |
|----|--------|-------------|------|
| 🚫 | [hagezi/dns-blocklists](https://github.com/hagezi/dns-blocklists) | NRDs from the **last 7 days** | [nrd7_asterisk.txt](https://cebeerre.github.io/dnsblocklists/NRD/nrd7_asterisk.txt) |
| 🚫 | [hagezi/dns-blocklists](https://github.com/hagezi/dns-blocklists) | NRDs registered **between day 14 and day 8 ago** | [nrd14-8_asterisk.txt](https://cebeerre.github.io/dnsblocklists/NRD/nrd14-8_asterisk.txt) |
| 🚫 | [xRuffKez/NRD (DNSBunker)](https://codeberg.org/xRuffKez/NRD) | NRDs from the **last 14 days** | [nrd14_wildcard_dnsbuker.txt](https://cebeerre.github.io/dnsblocklists/NRD/nrd14_wildcard_dnsbuker.txt) |

>[!NOTE]  
> To block **14 days of Hagezi’s NRDs**, you need to combine `nrd7_asterisk.txt` + `nrd14-8_asterisk.txt`.  
> I also provide DNSBunker’s 14-day list as an alternative source. Since I don’t know how either project curates or sources their data, using both together might increase coverage but also make lists very large.  
> Blocky will deduplicate entries automatically, but loading very large lists can increase startup times and **memory (RAM) usage**.

---

## 🌐 Webservice Blocklists

Blocklists targeting specific **web platforms and services**. 
Automatically generated from [AdGuardTeam/HostlistsRegistry](https://github.com/AdguardTeam/HostlistsRegistry).  
Each list is already in wildcard format for Blocky.

>[!TIP]  
> These lists can be handy for everyday scenarios:  
> - **At home** → block services like YouTube for parental control.  
> - **At the office** → block distractions like YouTube or LinkedIn to keep people focused 😁


<!-- START:SERVICES -->
## 🌐 Webservice Blocklists

| Icon | Service | Link |
|------|---------|------|

<!-- END:SERVICES -->


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
- The workflows:  
  1. Fetch the upstream lists in their original formats.  
  2. Convert them into `*.domain` wildcard format.  
  3. Publish them automatically to [GitHub Pages](https://cebeerre.github.io/dnsblocklists).  
