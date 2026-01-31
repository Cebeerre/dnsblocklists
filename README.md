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

>[!NOTE]  
> To block **14 days of Hagezi’s NRDs**, you need to combine `nrd7_asterisk.txt` + `nrd14-8_asterisk.txt`.  

And as per Hagezi's recommendations from his repo:

> [!WARNING]
> These lists are very large and resource-intensive. They may cause high memory usage and contain false positives, since some legitimate domains are newly registered. Use with caution and whitelist critical services as needed.
             
> [!CAUTION]
> Use at your own risk. The NRD lists are provided as-is, without guarantees, support, or a process for removing false positives.

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
| Icon | Service | Link |
|------|---------|------|
| <img src="icons/4chan.svg" width="20" height="20"/> | 4chan | [4chan_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/4chan_asterisk.txt) |
| <img src="icons/500px.svg" width="20" height="20"/> | 500px | [500px_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/500px_asterisk.txt) |
| <img src="icons/9gag.svg" width="20" height="20"/> | 9GAG | [9gag_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/9gag_asterisk.txt) |
| <img src="icons/activision_blizzard.svg" width="20" height="20"/> | Activision Blizzard | [activision_blizzard_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/activision_blizzard_asterisk.txt) |
| <img src="icons/aliexpress.svg" width="20" height="20"/> | AliExpress | [aliexpress_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/aliexpress_asterisk.txt) |
| <img src="icons/amazon.svg" width="20" height="20"/> | Amazon | [amazon_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/amazon_asterisk.txt) |
| <img src="icons/amazon_streaming.svg" width="20" height="20"/> | Amazon Streaming | [amazon_streaming_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/amazon_streaming_asterisk.txt) |
| <img src="icons/amino.svg" width="20" height="20"/> | Amino | [amino_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/amino_asterisk.txt) |
| <img src="icons/apple_streaming.svg" width="20" height="20"/> | Apple Streaming | [apple_streaming_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/apple_streaming_asterisk.txt) |
| <img src="icons/battle_net.svg" width="20" height="20"/> | Battle.net | [battle_net_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/battle_net_asterisk.txt) |
| <img src="icons/betano.svg" width="20" height="20"/> | Betano | [betano_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/betano_asterisk.txt) |
| <img src="icons/betfair.svg" width="20" height="20"/> | Betfair | [betfair_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/betfair_asterisk.txt) |
| <img src="icons/betway.svg" width="20" height="20"/> | Betway | [betway_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/betway_asterisk.txt) |
| <img src="icons/bigo_live.svg" width="20" height="20"/> | Bigo Live | [bigo_live_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/bigo_live_asterisk.txt) |
| <img src="icons/bilibili.svg" width="20" height="20"/> | Bilibili | [bilibili_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/bilibili_asterisk.txt) |
| <img src="icons/blaze.svg" width="20" height="20"/> | Blaze | [blaze_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/blaze_asterisk.txt) |
| <img src="icons/blizzard_entertainment.svg" width="20" height="20"/> | Blizzard Entertainment | [blizzard_entertainment_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/blizzard_entertainment_asterisk.txt) |
| <img src="icons/bluesky.svg" width="20" height="20"/> | Bluesky | [bluesky_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/bluesky_asterisk.txt) |
| <img src="icons/box.svg" width="20" height="20"/> | Box | [box_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/box_asterisk.txt) |
| <img src="icons/canais_globo.svg" width="20" height="20"/> | Canais Globo | [canais_globo_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/canais_globo_asterisk.txt) |
| <img src="icons/chatgpt.svg" width="20" height="20"/> | ChatGPT | [chatgpt_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/chatgpt_asterisk.txt) |
| <img src="icons/claro.svg" width="20" height="20"/> | Claro | [claro_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/claro_asterisk.txt) |
| <img src="icons/claude.svg" width="20" height="20"/> | Claude | [claude_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/claude_asterisk.txt) |
| <img src="icons/cloudflare.svg" width="20" height="20"/> | Cloudflare | [cloudflare_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/cloudflare_asterisk.txt) |
| <img src="icons/clubhouse.svg" width="20" height="20"/> | Clubhouse | [clubhouse_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/clubhouse_asterisk.txt) |
| <img src="icons/coolapk.svg" width="20" height="20"/> | CoolApk | [coolapk_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/coolapk_asterisk.txt) |
| <img src="icons/copilot.svg" width="20" height="20"/> | Copilot | [copilot_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/copilot_asterisk.txt) |
| <img src="icons/crunchyroll.svg" width="20" height="20"/> | Crunchyroll | [crunchyroll_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/crunchyroll_asterisk.txt) |
| <img src="icons/dailymotion.svg" width="20" height="20"/> | Dailymotion | [dailymotion_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/dailymotion_asterisk.txt) |
| <img src="icons/deepseek.svg" width="20" height="20"/> | DeepSeek | [deepseek_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/deepseek_asterisk.txt) |
| <img src="icons/deezer.svg" width="20" height="20"/> | Deezer | [deezer_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/deezer_asterisk.txt) |
| <img src="icons/directvgo.svg" width="20" height="20"/> | DirecTV Go | [directvgo_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/directvgo_asterisk.txt) |
| <img src="icons/discord.svg" width="20" height="20"/> | Discord | [discord_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/discord_asterisk.txt) |
| <img src="icons/discoveryplus.svg" width="20" height="20"/> | Discovery+ | [discoveryplus_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/discoveryplus_asterisk.txt) |
| <img src="icons/disneyplus.svg" width="20" height="20"/> | Disney+ | [disneyplus_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/disneyplus_asterisk.txt) |
| <img src="icons/douban.svg" width="20" height="20"/> | Douban | [douban_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/douban_asterisk.txt) |
| <img src="icons/dropbox.svg" width="20" height="20"/> | Dropbox | [dropbox_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/dropbox_asterisk.txt) |
| <img src="icons/ebay.svg" width="20" height="20"/> | eBay | [ebay_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/ebay_asterisk.txt) |
| <img src="icons/electronic_arts.svg" width="20" height="20"/> | Electronic Arts | [electronic_arts_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/electronic_arts_asterisk.txt) |
| <img src="icons/epic_games.svg" width="20" height="20"/> | Epic Games | [epic_games_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/epic_games_asterisk.txt) |
| <img src="icons/espn.svg" width="20" height="20"/> | ESPN | [espn_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/espn_asterisk.txt) |
| <img src="icons/facebook.svg" width="20" height="20"/> | Facebook | [facebook_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/facebook_asterisk.txt) |
| <img src="icons/fifa.svg" width="20" height="20"/> | FIFA | [fifa_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/fifa_asterisk.txt) |
| <img src="icons/flickr.svg" width="20" height="20"/> | Flickr | [flickr_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/flickr_asterisk.txt) |
| <img src="icons/gemini.svg" width="20" height="20"/> | Gemini | [gemini_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/gemini_asterisk.txt) |
| <img src="icons/globoplay.svg" width="20" height="20"/> | Globoplay | [globoplay_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/globoplay_asterisk.txt) |
| <img src="icons/gog.svg" width="20" height="20"/> | GOG | [gog_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/gog_asterisk.txt) |
| <img src="icons/playstore.svg" width="20" height="20"/> | Google Play Store | [playstore_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/playstore_asterisk.txt) |
| <img src="icons/grok.svg" width="20" height="20"/> | Grok | [grok_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/grok_asterisk.txt) |
| <img src="icons/hbomax.svg" width="20" height="20"/> | HBO Max | [hbomax_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/hbomax_asterisk.txt) |
| <img src="icons/hulu.svg" width="20" height="20"/> | Hulu | [hulu_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/hulu_asterisk.txt) |
| <img src="icons/icloud_private_relay.svg" width="20" height="20"/> | iCloud Private Relay | [icloud_private_relay_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/icloud_private_relay_asterisk.txt) |
| <img src="icons/iheartradio.svg" width="20" height="20"/> | iHeartRadio | [iheartradio_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/iheartradio_asterisk.txt) |
| <img src="icons/imgur.svg" width="20" height="20"/> | Imgur | [imgur_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/imgur_asterisk.txt) |
| <img src="icons/instagram.svg" width="20" height="20"/> | Instagram | [instagram_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/instagram_asterisk.txt) |
| <img src="icons/io_interactive.svg" width="20" height="20"/> | IO Interactive | [io_interactive_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/io_interactive_asterisk.txt) |
| <img src="icons/iqiyi.svg" width="20" height="20"/> | iQIYI | [iqiyi_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/iqiyi_asterisk.txt) |
| <img src="icons/kakaotalk.svg" width="20" height="20"/> | KakaoTalk | [kakaotalk_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/kakaotalk_asterisk.txt) |
| <img src="icons/kik.svg" width="20" height="20"/> | Kik | [kik_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/kik_asterisk.txt) |
| <img src="icons/kook.svg" width="20" height="20"/> | KOOK | [kook_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/kook_asterisk.txt) |
| <img src="icons/lazada.svg" width="20" height="20"/> | Lazada | [lazada_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/lazada_asterisk.txt) |
| <img src="icons/leagueoflegends.svg" width="20" height="20"/> | League of Legends | [leagueoflegends_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/leagueoflegends_asterisk.txt) |
| <img src="icons/line.svg" width="20" height="20"/> | LINE | [line_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/line_asterisk.txt) |
| <img src="icons/linkedin.svg" width="20" height="20"/> | LinkedIn | [linkedin_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/linkedin_asterisk.txt) |
| <img src="icons/lionsgateplus.svg" width="20" height="20"/> | Lionsgate+ | [lionsgateplus_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/lionsgateplus_asterisk.txt) |
| <img src="icons/looke.svg" width="20" height="20"/> | Looke | [looke_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/looke_asterisk.txt) |
| <img src="icons/mail_ru.svg" width="20" height="20"/> | Mail.ru | [mail_ru_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/mail_ru_asterisk.txt) |
| <img src="icons/manus.svg" width="20" height="20"/> | Manus | [manus_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/manus_asterisk.txt) |
| <img src="icons/mastodon.svg" width="20" height="20"/> | Mastodon | [mastodon_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/mastodon_asterisk.txt) |
| <img src="icons/max.svg" width="20" height="20"/> | MAX | [max_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/max_asterisk.txt) |
| <img src="icons/mercado_libre.svg" width="20" height="20"/> | Mercado Libre | [mercado_libre_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/mercado_libre_asterisk.txt) |
| <img src="icons/meta_ai.svg" width="20" height="20"/> | Meta AI | [meta_ai_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/meta_ai_asterisk.txt) |
| <img src="icons/microsoft_teams.svg" width="20" height="20"/> | Microsoft Teams | [microsoft_teams_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/microsoft_teams_asterisk.txt) |
| <img src="icons/minecraft.svg" width="20" height="20"/> | Minecraft | [minecraft_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/minecraft_asterisk.txt) |
| <img src="icons/nebula.svg" width="20" height="20"/> | Nebula | [nebula_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/nebula_asterisk.txt) |
| <img src="icons/netflix.svg" width="20" height="20"/> | Netflix | [netflix_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/netflix_asterisk.txt) |
| <img src="icons/nintendo.svg" width="20" height="20"/> | Nintendo | [nintendo_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/nintendo_asterisk.txt) |
| <img src="icons/nvidia.svg" width="20" height="20"/> | Nvidia | [nvidia_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/nvidia_asterisk.txt) |
| <img src="icons/odysee.svg" width="20" height="20"/> | Odysee | [odysee_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/odysee_asterisk.txt) |
| <img src="icons/ok.svg" width="20" height="20"/> | OK.ru | [ok_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/ok_asterisk.txt) |
| <img src="icons/olvid.svg" width="20" height="20"/> | Olvid | [olvid_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/olvid_asterisk.txt) |
| <img src="icons/onlyfans.svg" width="20" height="20"/> | OnlyFans | [onlyfans_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/onlyfans_asterisk.txt) |
| <img src="icons/origin.svg" width="20" height="20"/> | Origin | [origin_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/origin_asterisk.txt) |
| <img src="icons/paramountplus.svg" width="20" height="20"/> | Paramount Plus | [paramountplus_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/paramountplus_asterisk.txt) |
| <img src="icons/peacock_tv.svg" width="20" height="20"/> | Peacock TV | [peacock_tv_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/peacock_tv_asterisk.txt) |
| <img src="icons/perplexity.svg" width="20" height="20"/> | Perplexity | [perplexity_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/perplexity_asterisk.txt) |
| <img src="icons/pinterest.svg" width="20" height="20"/> | Pinterest | [pinterest_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/pinterest_asterisk.txt) |
| <img src="icons/playstation.svg" width="20" height="20"/> | PlayStation | [playstation_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/playstation_asterisk.txt) |
| <img src="icons/plenty_of_fish.svg" width="20" height="20"/> | Plenty of Fish | [plenty_of_fish_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/plenty_of_fish_asterisk.txt) |
| <img src="icons/plex.svg" width="20" height="20"/> | Plex | [plex_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/plex_asterisk.txt) |
| <img src="icons/pluto_tv.svg" width="20" height="20"/> | Pluto TV | [pluto_tv_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/pluto_tv_asterisk.txt) |
| <img src="icons/privacy.svg" width="20" height="20"/> | Privacy | [privacy_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/privacy_asterisk.txt) |
| <img src="icons/proton.svg" width="20" height="20"/> | Proton | [proton_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/proton_asterisk.txt) |
| <img src="icons/qq.svg" width="20" height="20"/> | QQ | [qq_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/qq_asterisk.txt) |
| <img src="icons/rakuten_viki.svg" width="20" height="20"/> | Rakuten Viki | [rakuten_viki_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/rakuten_viki_asterisk.txt) |
| <img src="icons/reddit.svg" width="20" height="20"/> | Reddit | [reddit_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/reddit_asterisk.txt) |
| <img src="icons/riot_games.svg" width="20" height="20"/> | Riot Games | [riot_games_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/riot_games_asterisk.txt) |
| <img src="icons/roblox.svg" width="20" height="20"/> | Roblox | [roblox_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/roblox_asterisk.txt) |
| <img src="icons/rockstar_games.svg" width="20" height="20"/> | Rockstar Games | [rockstar_games_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/rockstar_games_asterisk.txt) |
| <img src="icons/samsung_tv_plus.svg" width="20" height="20"/> | Samsung TV Plus | [samsung_tv_plus_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/samsung_tv_plus_asterisk.txt) |
| <img src="icons/shein.svg" width="20" height="20"/> | Shein | [shein_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/shein_asterisk.txt) |
| <img src="icons/shopee.svg" width="20" height="20"/> | Shopee | [shopee_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/shopee_asterisk.txt) |
| <img src="icons/signal.svg" width="20" height="20"/> | Signal | [signal_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/signal_asterisk.txt) |
| <img src="icons/skype.svg" width="20" height="20"/> | Skype | [skype_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/skype_asterisk.txt) |
| <img src="icons/slack.svg" width="20" height="20"/> | Slack | [slack_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/slack_asterisk.txt) |
| <img src="icons/snapchat.svg" width="20" height="20"/> | Snapchat | [snapchat_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/snapchat_asterisk.txt) |
| <img src="icons/soundcloud.svg" width="20" height="20"/> | SoundCloud | [soundcloud_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/soundcloud_asterisk.txt) |
| <img src="icons/spotify.svg" width="20" height="20"/> | Spotify | [spotify_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/spotify_asterisk.txt) |
| <img src="icons/spotify_video.svg" width="20" height="20"/> | Spotify Video | [spotify_video_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/spotify_video_asterisk.txt) |
| <img src="icons/steam.svg" width="20" height="20"/> | Steam | [steam_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/steam_asterisk.txt) |
| <img src="icons/telegram.svg" width="20" height="20"/> | Telegram (Web) | [telegram_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/telegram_asterisk.txt) |
| <img src="icons/temu.svg" width="20" height="20"/> | Temu | [temu_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/temu_asterisk.txt) |
| <img src="icons/tidal.svg" width="20" height="20"/> | Tidal | [tidal_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/tidal_asterisk.txt) |
| <img src="icons/tiktok.svg" width="20" height="20"/> | TikTok | [tiktok_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/tiktok_asterisk.txt) |
| <img src="icons/tinder.svg" width="20" height="20"/> | Tinder | [tinder_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/tinder_asterisk.txt) |
| <img src="icons/tumblr.svg" width="20" height="20"/> | Tumblr | [tumblr_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/tumblr_asterisk.txt) |
| <img src="icons/twitch.svg" width="20" height="20"/> | Twitch | [twitch_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/twitch_asterisk.txt) |
| <img src="icons/ubisoft.svg" width="20" height="20"/> | Ubisoft | [ubisoft_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/ubisoft_asterisk.txt) |
| <img src="icons/valorant.svg" width="20" height="20"/> | Valorant | [valorant_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/valorant_asterisk.txt) |
| <img src="icons/viber.svg" width="20" height="20"/> | Viber | [viber_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/viber_asterisk.txt) |
| <img src="icons/vimeo.svg" width="20" height="20"/> | Vimeo | [vimeo_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/vimeo_asterisk.txt) |
| <img src="icons/vivo_play.svg" width="20" height="20"/> | Vivo Play | [vivo_play_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/vivo_play_asterisk.txt) |
| <img src="icons/vk.svg" width="20" height="20"/> | VK.com | [vk_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/vk_asterisk.txt) |
| <img src="icons/voot.svg" width="20" height="20"/> | Voot | [voot_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/voot_asterisk.txt) |
| <img src="icons/wargaming.svg" width="20" height="20"/> | Wargaming | [wargaming_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/wargaming_asterisk.txt) |
| <img src="icons/warnerbrosgames.svg" width="20" height="20"/> | Warner Bros. Games | [warnerbrosgames_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/warnerbrosgames_asterisk.txt) |
| <img src="icons/wechat.svg" width="20" height="20"/> | WeChat | [wechat_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/wechat_asterisk.txt) |
| <img src="icons/weibo.svg" width="20" height="20"/> | Weibo | [weibo_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/weibo_asterisk.txt) |
| <img src="icons/whatsapp.svg" width="20" height="20"/> | WhatsApp | [whatsapp_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/whatsapp_asterisk.txt) |
| <img src="icons/wizz.svg" width="20" height="20"/> | Wizz | [wizz_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/wizz_asterisk.txt) |
| <img src="icons/twitter.svg" width="20" height="20"/> | X (formerly Twitter) | [twitter_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/twitter_asterisk.txt) |
| <img src="icons/xboxlive.svg" width="20" height="20"/> | Xbox Live | [xboxlive_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/xboxlive_asterisk.txt) |
| <img src="icons/xiaohongshu.svg" width="20" height="20"/> | Xiaohongshu | [xiaohongshu_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/xiaohongshu_asterisk.txt) |
| <img src="icons/youtube.svg" width="20" height="20"/> | YouTube | [youtube_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/youtube_asterisk.txt) |
| <img src="icons/yy.svg" width="20" height="20"/> | YY | [yy_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/yy_asterisk.txt) |
| <img src="icons/zhihu.svg" width="20" height="20"/> | Zhihu | [zhihu_asterisk.txt](https://Cebeerre.github.io/dnsblocklists/webservices/zhihu_asterisk.txt) |
<!-- END:SERVICES -->


> [!NOTE]  
> Each generated list may include a section labeled **“Skipped unsupported rules”**.  
> These lines come directly from the AdGuard upstream sources but cannot be expressed in Blocky’s wildcard format.  
> Examples include:
> - Wildcards inside labels (e.g., `||awsdns-*.tld^`)  
> - Single-pipe Adblock anchors (e.g., `|domain^`)  
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
