# Blocky-Compatible Wildcard Lists

This repository exists purely for **convenience**.  
It provides domain blocklists already converted into the **wildcard asterisk (`*.domain`) format** required by [Blocky](https://github.com/0xERR0R/blocky) (v0.23 or newer).  

⚠️ **Important:**  
- The blocklist data itself does **not** originate here.  
- This repo only automates fetching, converting, and publishing lists from their **original sources**.  
- All credit remain with the upstream projects.

---

## 📂 Repository Structure

### `NRD/`
- Contains **Newly Registered Domain (NRD)** lists converted to wildcard format.  
- Source: [hagezi/dns-blocklists](https://github.com/hagezi/dns-blocklists).  
- Files:  
  - `nrd7_asterisk.txt` → Domains registered in the **last 7 days**.  
  - `nrd14-8_asterisk.txt` → Domains registered **between day 14 and day 8 ago**.

>[!NOTE]
>To block NRDs from the last 14 days, combine the domain lists from 7 days ago and 14 days ago. 
         
### `webservices/`
- Contains one file per web service, each in wildcard format.  
- Source: [AdGuardTeam/HostlistsRegistry](https://github.com/AdguardTeam/HostlistsRegistry).  
- Example files:  
  - `4chan_asterisk.txt` → Wildcard blocklist for 4chan domains.  
  - `500px_asterisk.txt` → Wildcard blocklist for 500px domains.  
  - …and so on, one for each service in the registry.  

---

## 🔄 How It Works

- GitHub Actions workflows run on a schedule:  
  - **NRD lists** → refreshed **daily**.  
  - **Webservices lists** → refreshed **weekly**.  
- The workflows:  
  1. Fetch the upstream lists in their original formats.  
  2. Convert them into `*.domain` wildcard format.  
  3. Publish them here under `NRD/` or `webservices/`.  
