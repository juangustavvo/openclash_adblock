# OpenClash AdBlock
Ini adalah adblock untuk openclash, source list diambil dari **Energized Blu**. Source list diupdate setiap hari secara otomatis oleh bot github.

| PACK NAME | DESCRIPTION | Sources |
|---------|:-------:|:-----:|
Blu | Mid range lightweight protection. | *Core List + Blu Go + AdGuard DNS & Tracking, Anudeep's Adservers, Better.fyi Trackers, Disconnect Advertising Filter List, EasyPrivacy, Hexxium Creations Threat List, hosts-blocklists, KADhosts, neoHosts, and YousList* | **30** |

Untuk menggunakan, edit `config.yaml` pada `/etc/openclash/config/config.yaml` seperti ini:
```
rule-providers:
  adblock:
    type: http
    behavior: classical
    path: "./rule_provider/energized_blu_adblock.yaml"
    url: https://raw.githubusercontent.com/hillz2/openclash_adblock/main/energized_blu_adblock.yaml
    interval: 14400 # Update rules every 4 hours
rules:
# Block ads
- RULE-SET,adblock,REJECT
```
Setelah di test dengan situs [Adblock Test](https://d3ward.github.io/toolz/adblock.html) hasilnya:
[![2022-06-08-213555-1920x986-scrot.png](https://i.postimg.cc/0yCf9YQK/2022-06-08-213555-1920x986-scrot.png)](https://postimg.cc/CRzDNfbw)

Hasil di situs adblock test bisa berbeda beda karena source list diupdate setiap hari.
**Sumber: [Energized Protection](https://github.com/EnergizedProtection/block)**
