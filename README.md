# `Ekko` 自用Clash Rule规则

本项目生成适用于 [**Clash Premium 内核**](https://github.com/Dreamacro/clash/releases/tag/premium)的规则集（RULE-SET），同时适用于所有使用 Clash Premium 内核的 Clash 图形用户界面（GUI）客户端。使用 GitHub Actions 北京时间每天早上 6:30 自动构建，保证规则最新。适配[v2board](https://github.com/v2board/v2board)配置。

## 说明

本项目规则集（RULE-SET）的数据主要来源于项目 [@blackmatrix7](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Clash)

## Clash Premium 各版本下载地址

> ⚠️ 由于 Clash 及其部分周边生态项目于 2023 年 11 月上旬删库跑路，现提供部分官方原版安装包、可执行文件，详情见 [**hidden**](https://github.com/Loyalsoldier/clash-rules/tree/hidden) 分支。

* Clash Premium **命令行**版：
  * [官方版](https://github.com/Loyalsoldier/clash-rules/tree/hidden/software/clash-premium)（适用于 Windows、macOS、Linux、OpenWRT 等多种平台）
  * [衍生版 Clash.Meta](https://github.com/MetaCubeX/Clash.Meta/releases)（适用于 Windows、macOS、Linux、OpenWRT 等多种平台）
* Clash Premium **图形用户界面**版：
  * [ClashN](https://github.com/2dust/clashN/releases)（适用于 Windows）
  * [ClashX Pro](https://github.com/Loyalsoldier/clash-rules/tree/hidden/software/clashx-pro)（适用于 macOS）
  * [Clash-verge](https://github.com/zzzgydi/clash-verge/releases)（适用于 Windows、macOS、Linux）
  * [Clash for Windows](https://github.com/Loyalsoldier/clash-rules/tree/hidden/software/clash-for-windows)（适用于 Windows、macOS、Linux）
  * [Clash for Android](https://apkpure.com/clash-for-android/com.github.kr328.clash/versions)（适用于 Android）

### 使用方式

要想使用本项目的规则集，只需要在 Clash 配置文件中添加如下 `rule-providers` 和 `rules`。

#### Rule Providers 配置方式

```
rule-providers:
  YouTube:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/YouTube/YouTube.yaml"
    path: ./ruleset/YouTube.yaml
    interval: 864
  Google:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Google/Google.yaml"
    path: ./ruleset/Google.yaml
    interval: 864
  GitHub:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/GitHub/GitHub.yaml"
    path: ./ruleset/GitHub.yaml
    interval: 864
  OneDrive:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/OneDrive/OneDrive.yaml"
    path: ./ruleset/OneDrive.yaml
    interval: 864
  Microsoft:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Microsoft/Microsoft.yaml"
    path: ./ruleset/Microsoft.yaml
    interval: 864
  AppStore:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/AppStore/AppStore.yaml"
    path: ./ruleset/AppStore.yaml
    interval: 864
  iCloud:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/iCloud/iCloud.yaml"
    path: ./ruleset/iCloud.yaml
    interval: 864
  Apple:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Apple/Apple.yaml"
    path: ./ruleset/Apple.yaml
    interval: 864
  Telegram:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Telegram/Telegram.yaml"
    path: ./ruleset/Telegram.yaml
    interval: 864
  PotatoChat:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/PotatoChat/PotatoChat.yaml"
    path: ./ruleset/PotatoChat.yaml
    interval: 864
  KakaoTalk:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/KakaoTalk/KakaoTalk.yaml"
    path: ./ruleset/KakaoTalk.yaml
    interval: 864
  Line:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Line/Line.yaml"
    path: ./ruleset/Line.yaml
    interval: 864
  Netflix:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Netflix/Netflix.yaml"
    path: ./ruleset/Netflix.yaml
    interval: 864
  Dubox:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Dubox/Dubox.yaml"
    path: ./ruleset/Dubox.yaml
    interval: 864
  TikTok:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/TikTok/TikTok.yaml"
    path: ./ruleset/TikTok.yaml
    interval: 864
  Disney:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Disney/Disney.yaml"
    path: ./ruleset/Disney.yaml
    interval: 864
  Twitter:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Twitter/Twitter.yaml"
    path: ./ruleset/Twitter.yaml
    interval: 864
  Facebook:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Facebook/Facebook.yaml"
    path: ./ruleset/Facebook.yaml
    interval: 864
  Spotify:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Spotify/Spotify.yaml"
    path: ./ruleset/Spotify.yaml
    interval: 864
  Wikipedia:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Wikipedia/Wikipedia.yaml"
    path: ./ruleset/Wikipedia.yaml
    interval: 864
  Discord:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Discord/Discord.yaml"
    path: ./ruleset/Discord.yaml
    interval: 864
  PayPal:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/PayPal/PayPal.yaml"
    path: ./ruleset/PayPal.yaml
    interval: 864
  Spark:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Spark/Spark.yaml"
    path: ./ruleset/Spark.yaml
    interval: 864
  Sony:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Sony/Sony.yaml"
    path: ./ruleset/Sony.yaml
    interval: 864
  BBC:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/BBC/BBC.yaml"
    path: ./ruleset/BBC.yaml
    interval: 864
  Amazon:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Amazon/Amazon.yaml"
    path: ./ruleset/Amazon.yaml
    interval: 864
  Instagram:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Instagram/Instagram.yaml"
    path: ./ruleset/Instagram.yaml
    interval: 864
  Whatsapp:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Whatsapp/Whatsapp.yaml"
    path: ./ruleset/Whatsapp.yaml
    interval: 864
  Adobe:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Adobe/Adobe.yaml"
    path: ./ruleset/Adobe.yaml
    interval: 864
  Vimeo:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Vimeo/Vimeo.yaml"
    path: ./ruleset/Vimeo.yaml
    interval: 864
  Bestbuy:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Bestbuy/Bestbuy.yaml"
    path: ./ruleset/Bestbuy.yaml
    interval: 864
  Duckduckgo:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Duckduckgo/Duckduckgo.yaml"
    path: ./ruleset/Duckduckgo.yaml
    interval: 864
  GitBook:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/GitBook/GitBook.yaml"
    path: ./ruleset/GitBook.yaml
    interval: 864
  Gucci:
    type: http
    behavior: classical
    url: "https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/release/rule/Clash/Gucci/Gucci.yaml"
    path: ./ruleset/Gucci.yaml
    interval: 864
  Imgur:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Imgur/Imgur.yaml"
    path: ./ruleset/Imgur.yaml
    interval: 864
  Pinterest:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Pinterest/Pinterest.yaml"
    path: ./ruleset/Pinterest.yaml
    interval: 864
  Reddit:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Reddit/Reddit.yaml"
    path: ./ruleset/Reddit.yaml
    interval: 864
  Samsung:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Samsung/Samsung.yaml"
    path: ./ruleset/Samsung.yaml
    interval: 864
  Razer:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Razer/Razer.yaml"
    path: ./ruleset/Razer.yaml
    interval: 864
  Shopee:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Shopee/Shopee.yaml"
    path: ./ruleset/Shopee.yaml
    interval: 864
  Shopify:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Shopify/Shopify.yaml"
    path: ./ruleset/Shopify.yaml
    interval: 864
  Twitch:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Twitch/Twitch.yaml"
    path: ./ruleset/Twitch.yaml
    interval: 864
  VISA:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/VISA/VISA.yaml"
    path: ./ruleset/VISA.yaml
    interval: 864
  WIX:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/WIX/WIX.yaml"
    path: ./ruleset/WIX.yaml
    interval: 864
  Zoho:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Zoho/Zoho.yaml"
    path: ./ruleset/Zoho.yaml
    interval: 864
  eBay:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/eBay/eBay.yaml"
    path: ./ruleset/eBay.yaml
    interval: 864
  MOMOShop:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/MOMOShop/MOMOShop.yaml"
    path: ./ruleset/MOMOShop.yaml
    interval: 864
  Binance:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Binance/Binance.yaml"
    path: ./ruleset/Binance.yaml
    interval: 864
  OpenAI:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/OpenAI/OpenAI.yaml"
    path: ./ruleset/OpenAI.yaml
    interval: 864
  MicrosoftEdge:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/MicrosoftEdge/MicrosoftEdge.yaml"
    path: ./ruleset/MicrosoftEdge.yaml
    interval: 864
  Bing:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Bing/Bing.yaml"
    path: ./ruleset/Bing.yaml
    interval: 864
  Copilot:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Copilot/Copilot.yaml"
    path: ./ruleset/Copilot.yaml
    interval: 864
```

#### 白名单模式 Rules 配置方式（推荐）

* 白名单模式，意为「 **没有命中规则的网络流量，统统使用代理** 」，适用于服务器线路网络质量稳定、快速，不缺服务器流量的用户。
* 以下配置中，除了 `DIRECT` 和 `REJECT` 是默认存在于 Clash 中的 policy（路由策略/流量处理策略），其余均为自定义 policy，对应配置文件中 `proxies` 或 `proxy-groups` 中的 `name`。如你直接使用下面的 `rules` 规则，则需要在 `proxies` 或 `proxy-groups` 中手动配置一个 `name` 为 `PROXY` 的 policy。
* 如你希望 Apple、iCloud 和 Google 列表中的域名使用代理，则把 policy 由 `DIRECT` 改为 `PROXY`，以此类推，举一反三。
* 如你不希望进行 DNS 解析，可在 `GEOIP` 规则的最后加上 `,no-resolve`，如 `GEOIP,CN,DIRECT,no-resolve`。

```
rules:
  - DOMAIN,clash.razord.top,DIRECT
  - DOMAIN,yacd.haishan.me,DIRECT
  - RULE-SET,YouTube,PROXY
  - RULE-SET,Google,PROXY
  - RULE-SET,GitHub,PROXY
  - RULE-SET,OneDrive,PROXY
  - RULE-SET,Microsoft,PROXY
  - RULE-SET,AppStore,PROXY
  - RULE-SET,iCloud,PROXY
  - RULE-SET,Apple,PROXY
  - RULE-SET,Telegram,PROXY
  - RULE-SET,PotatoChat,PROXY
  - RULE-SET,KakaoTalk,PROXY
  - RULE-SET,Line,PROXY
  - RULE-SET,Netflix,PROXY
  - RULE-SET,Dubox,PROXY
  - RULE-SET,TikTok,PROXY
  - RULE-SET,Disney,PROXY
  - RULE-SET,Twitter,PROXY
  - RULE-SET,Facebook,PROXY
  - RULE-SET,Spotify,PROXY
  - RULE-SET,Wikipedia,PROXY
  - RULE-SET,Discord,PROXY
  - RULE-SET,PayPal,PROXY
  - RULE-SET,Spark,PROXY
  - RULE-SET,Sony,PROXY
  - RULE-SET,BBC,PROXY
  - RULE-SET,Amazon,PROXY
  - RULE-SET,Instagram,PROXY
  - RULE-SET,Whatsapp,PROXY
  - RULE-SET,Adobe,PROXY
  - RULE-SET,Vimeo,PROXY
  - RULE-SET,Bestbuy,PROXY
  - RULE-SET,Duckduckgo,PROXY
  - RULE-SET,GitBook,PROXY
  - RULE-SET,Gucci,PROXY
  - RULE-SET,Imgur,PROXY
  - RULE-SET,Pinterest,PROXY
  - RULE-SET,Reddit,PROXY
  - RULE-SET,Samsung,PROXY
  - RULE-SET,Razer,PROXY
  - RULE-SET,Shopee,PROXY
  - RULE-SET,Shopify,PROXY
  - RULE-SET,Twitch,PROXY
  - RULE-SET,VISA,PROXY
  - RULE-SET,WIX,PROXY
  - RULE-SET,Zoho,PROXY
  - RULE-SET,eBay,PROXY
  - RULE-SET,MOMOShop,PROXY
  - RULE-SET,Binance,PROXY
  - RULE-SET,OpenAI,PROXY
  - RULE-SET,MicrosoftEdge,PROXY
  - RULE-SET,Bing,PROXY
  - RULE-SET,Copilot,PROXY
  - GEOIP,LAN,DIRECT
  - GEOIP,CN,DIRECT
  - MATCH,PROXY
```

#### 黑名单模式 Rules 配置方式

* 黑名单模式，意为「 **只有命中规则的网络流量，才使用代理** 」，适用于服务器线路网络质量不稳定或不够快，或服务器流量紧缺的用户。通常也是软路由用户、家庭网关用户的常用模式。
* 以下配置中，除了 `DIRECT` 和 `REJECT` 是默认存在于 Clash 中的 policy（路由策略/流量处理策略），其余均为自定义 policy，对应配置文件中 `proxies` 或 `proxy-groups` 中的 `name`。如你直接使用下面的 `rules` 规则，则需要在 `proxies` 或 `proxy-groups` 中手动配置一个 `name` 为 `PROXY` 的 policy。

```
rules:
  - DOMAIN,clash.razord.top,DIRECT
  - DOMAIN,yacd.haishan.me,DIRECT
  - RULE-SET,YouTube,PROXY
  - RULE-SET,Google,PROXY
  - RULE-SET,GitHub,PROXY
  - RULE-SET,OneDrive,PROXY
  - RULE-SET,Microsoft,PROXY
  - RULE-SET,AppStore,PROXY
  - RULE-SET,iCloud,PROXY
  - RULE-SET,Apple,PROXY
  - RULE-SET,Telegram,PROXY
  - RULE-SET,PotatoChat,PROXY
  - RULE-SET,KakaoTalk,PROXY
  - RULE-SET,Line,PROXY
  - RULE-SET,Netflix,PROXY
  - RULE-SET,Dubox,PROXY
  - RULE-SET,TikTok,PROXY
  - RULE-SET,Disney,PROXY
  - RULE-SET,Twitter,PROXY
  - RULE-SET,Facebook,PROXY
  - RULE-SET,Spotify,PROXY
  - RULE-SET,Wikipedia,PROXY
  - RULE-SET,Discord,PROXY
  - RULE-SET,PayPal,PROXY
  - RULE-SET,Spark,PROXY
  - RULE-SET,Sony,PROXY
  - RULE-SET,BBC,PROXY
  - RULE-SET,Amazon,PROXY
  - RULE-SET,Instagram,PROXY
  - RULE-SET,Whatsapp,PROXY
  - RULE-SET,Adobe,PROXY
  - RULE-SET,Vimeo,PROXY
  - RULE-SET,Bestbuy,PROXY
  - RULE-SET,Duckduckgo,PROXY
  - RULE-SET,GitBook,PROXY
  - RULE-SET,Gucci,PROXY
  - RULE-SET,Imgur,PROXY
  - RULE-SET,Pinterest,PROXY
  - RULE-SET,Reddit,PROXY
  - RULE-SET,Samsung,PROXY
  - RULE-SET,Razer,PROXY
  - RULE-SET,Shopee,PROXY
  - RULE-SET,Shopify,PROXY
  - RULE-SET,Twitch,PROXY
  - RULE-SET,VISA,PROXY
  - RULE-SET,WIX,PROXY
  - RULE-SET,Zoho,PROXY
  - RULE-SET,eBay,PROXY
  - RULE-SET,MOMOShop,PROXY
  - RULE-SET,Binance,PROXY
  - RULE-SET,OpenAI,PROXY
  - RULE-SET,MicrosoftEdge,PROXY
  - RULE-SET,Bing,PROXY
  - RULE-SET,Copilot,PROXY
  - MATCH,DIRECT
```

## 适合v2board自定义的内容

使用前请在`resources/rules`新建一个文件`custom.clash.yaml`，然后将以下内容复制粘贴进去即可：

```
# port: 7890
# socks-port: 7891
# redir-port: 7892
# tproxy-port: 7893
mixed-port: 7890
allow-lan: true
bind-address: "*"
mode: rule
log-level: info
external-controller: 127.0.0.1:9090

dns:
  enable: true
  # listen: 0.0.0.0:53
  ipv6: false

  default-nameserver:
    - 223.5.5.5
    - 119.29.29.29
  enhanced-mode: fake-ip
  fake-ip-range: 198.18.0.1/16
  use-hosts: true
  nameserver:
    - https://doh.pub/dns-query
    - https://dns.alidns.com/dns-query
  fallback:
    - https://doh.dns.sb/dns-query
    - https://dns.cloudflare.com/dns-query
    - https://dns.twnic.tw/dns-query
    - tls://8.8.4.4:853
  fallback-filter:
    geoip: true
    ipcidr:
      - 240.0.0.0/4
      - 0.0.0.0/32

proxies:

proxy-groups:
  - { name: "PROXY", type: select, proxies: [] }
rule-providers:
  YouTube:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/YouTube/YouTube.yaml"
    path: ./ruleset/YouTube.yaml
    interval: 864
  Google:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Google/Google.yaml"
    path: ./ruleset/Google.yaml
    interval: 864
  GitHub:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/GitHub/GitHub.yaml"
    path: ./ruleset/GitHub.yaml
    interval: 864
  OneDrive:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/OneDrive/OneDrive.yaml"
    path: ./ruleset/OneDrive.yaml
    interval: 864
  Microsoft:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Microsoft/Microsoft.yaml"
    path: ./ruleset/Microsoft.yaml
    interval: 864
  AppStore:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/AppStore/AppStore.yaml"
    path: ./ruleset/AppStore.yaml
    interval: 864
  iCloud:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/iCloud/iCloud.yaml"
    path: ./ruleset/iCloud.yaml
    interval: 864
  Apple:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Apple/Apple.yaml"
    path: ./ruleset/Apple.yaml
    interval: 864
  Telegram:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Telegram/Telegram.yaml"
    path: ./ruleset/Telegram.yaml
    interval: 864
  PotatoChat:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/PotatoChat/PotatoChat.yaml"
    path: ./ruleset/PotatoChat.yaml
    interval: 864
  KakaoTalk:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/KakaoTalk/KakaoTalk.yaml"
    path: ./ruleset/KakaoTalk.yaml
    interval: 864
  Line:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Line/Line.yaml"
    path: ./ruleset/Line.yaml
    interval: 864
  Netflix:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Netflix/Netflix.yaml"
    path: ./ruleset/Netflix.yaml
    interval: 864
  Dubox:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Dubox/Dubox.yaml"
    path: ./ruleset/Dubox.yaml
    interval: 864
  TikTok:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/TikTok/TikTok.yaml"
    path: ./ruleset/TikTok.yaml
    interval: 864
  Disney:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Disney/Disney.yaml"
    path: ./ruleset/Disney.yaml
    interval: 864
  Twitter:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Twitter/Twitter.yaml"
    path: ./ruleset/Twitter.yaml
    interval: 864
  Facebook:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Facebook/Facebook.yaml"
    path: ./ruleset/Facebook.yaml
    interval: 864
  Spotify:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Spotify/Spotify.yaml"
    path: ./ruleset/Spotify.yaml
    interval: 864
  Wikipedia:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Wikipedia/Wikipedia.yaml"
    path: ./ruleset/Wikipedia.yaml
    interval: 864
  Discord:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Discord/Discord.yaml"
    path: ./ruleset/Discord.yaml
    interval: 864
  PayPal:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/PayPal/PayPal.yaml"
    path: ./ruleset/PayPal.yaml
    interval: 864
  Spark:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Spark/Spark.yaml"
    path: ./ruleset/Spark.yaml
    interval: 864
  Sony:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Sony/Sony.yaml"
    path: ./ruleset/Sony.yaml
    interval: 864
  BBC:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/BBC/BBC.yaml"
    path: ./ruleset/BBC.yaml
    interval: 864
  Amazon:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Amazon/Amazon.yaml"
    path: ./ruleset/Amazon.yaml
    interval: 864
  Instagram:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Instagram/Instagram.yaml"
    path: ./ruleset/Instagram.yaml
    interval: 864
  Whatsapp:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Whatsapp/Whatsapp.yaml"
    path: ./ruleset/Whatsapp.yaml
    interval: 864
  Adobe:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Adobe/Adobe.yaml"
    path: ./ruleset/Adobe.yaml
    interval: 864
  Vimeo:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Vimeo/Vimeo.yaml"
    path: ./ruleset/Vimeo.yaml
    interval: 864
  Bestbuy:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Bestbuy/Bestbuy.yaml"
    path: ./ruleset/Bestbuy.yaml
    interval: 864
  Duckduckgo:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Duckduckgo/Duckduckgo.yaml"
    path: ./ruleset/Duckduckgo.yaml
    interval: 864
  GitBook:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/GitBook/GitBook.yaml"
    path: ./ruleset/GitBook.yaml
    interval: 864
  Gucci:
    type: http
    behavior: classical
    url: "https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/release/rule/Clash/Gucci/Gucci.yaml"
    path: ./ruleset/Gucci.yaml
    interval: 864
  Imgur:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Imgur/Imgur.yaml"
    path: ./ruleset/Imgur.yaml
    interval: 864
  Pinterest:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Pinterest/Pinterest.yaml"
    path: ./ruleset/Pinterest.yaml
    interval: 864
  Reddit:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Reddit/Reddit.yaml"
    path: ./ruleset/Reddit.yaml
    interval: 864
  Samsung:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Samsung/Samsung.yaml"
    path: ./ruleset/Samsung.yaml
    interval: 864
  Razer:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Razer/Razer.yaml"
    path: ./ruleset/Razer.yaml
    interval: 864
  Shopee:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Shopee/Shopee.yaml"
    path: ./ruleset/Shopee.yaml
    interval: 864
  Shopify:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Shopify/Shopify.yaml"
    path: ./ruleset/Shopify.yaml
    interval: 864
  Twitch:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Twitch/Twitch.yaml"
    path: ./ruleset/Twitch.yaml
    interval: 864
  VISA:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/VISA/VISA.yaml"
    path: ./ruleset/VISA.yaml
    interval: 864
  WIX:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/WIX/WIX.yaml"
    path: ./ruleset/WIX.yaml
    interval: 864
  Zoho:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Zoho/Zoho.yaml"
    path: ./ruleset/Zoho.yaml
    interval: 864
  eBay:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/eBay/eBay.yaml"
    path: ./ruleset/eBay.yaml
    interval: 864
  MOMOShop:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/MOMOShop/MOMOShop.yaml"
    path: ./ruleset/MOMOShop.yaml
    interval: 864
  Binance:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Binance/Binance.yaml"
    path: ./ruleset/Binance.yaml
    interval: 864
  OpenAI:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/OpenAI/OpenAI.yaml"
    path: ./ruleset/OpenAI.yaml
    interval: 864
  MicrosoftEdge:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/MicrosoftEdge/MicrosoftEdge.yaml"
    path: ./ruleset/MicrosoftEdge.yaml
    interval: 864
  Bing:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Bing/Bing.yaml"
    path: ./ruleset/Bing.yaml
    interval: 864
  Copilot:
    type: http
    behavior: classical
    url: "https://cdn.jsdelivr.net/gh/blackmatrix7/ios_rule_script@master/rule/Clash/Copilot/Copilot.yaml"
    path: ./ruleset/Copilot.yaml
    interval: 864

rules:
  - RULE-SET,YouTube,PROXY
  - RULE-SET,Google,PROXY
  - RULE-SET,GitHub,PROXY
  - RULE-SET,OneDrive,PROXY
  - RULE-SET,Microsoft,PROXY
  - RULE-SET,AppStore,PROXY
  - RULE-SET,iCloud,PROXY
  - RULE-SET,Apple,PROXY
  - RULE-SET,Telegram,PROXY
  - RULE-SET,PotatoChat,PROXY
  - RULE-SET,KakaoTalk,PROXY
  - RULE-SET,Line,PROXY
  - RULE-SET,Netflix,PROXY
  - RULE-SET,Dubox,PROXY
  - RULE-SET,TikTok,PROXY
  - RULE-SET,Disney,PROXY
  - RULE-SET,Twitter,PROXY
  - RULE-SET,Facebook,PROXY
  - RULE-SET,Spotify,PROXY
  - RULE-SET,Wikipedia,PROXY
  - RULE-SET,Discord,PROXY
  - RULE-SET,PayPal,PROXY
  - RULE-SET,Spark,PROXY
  - RULE-SET,Sony,PROXY
  - RULE-SET,BBC,PROXY
  - RULE-SET,Amazon,PROXY
  - RULE-SET,Instagram,PROXY
  - RULE-SET,Whatsapp,PROXY
  - RULE-SET,Adobe,PROXY
  - RULE-SET,Vimeo,PROXY
  - RULE-SET,Bestbuy,PROXY
  - RULE-SET,Duckduckgo,PROXY
  - RULE-SET,GitBook,PROXY
  - RULE-SET,Gucci,PROXY
  - RULE-SET,Imgur,PROXY
  - RULE-SET,Pinterest,PROXY
  - RULE-SET,Reddit,PROXY
  - RULE-SET,Samsung,PROXY
  - RULE-SET,Razer,PROXY
  - RULE-SET,Shopee,PROXY
  - RULE-SET,Shopify,PROXY
  - RULE-SET,Twitch,PROXY
  - RULE-SET,VISA,PROXY
  - RULE-SET,WIX,PROXY
  - RULE-SET,Zoho,PROXY
  - RULE-SET,eBay,PROXY
  - RULE-SET,MOMOShop,PROXY
  - RULE-SET,Binance,PROXY
  - RULE-SET,OpenAI,PROXY
  - RULE-SET,MicrosoftEdge,PROXY
  - RULE-SET,Bing,PROXY
  - RULE-SET,Copilot,PROXY
  - GEOIP,LAN,DIRECT
  - GEOIP,CN,DIRECT
  - MATCH,PROXY

```

## 致谢

* [@blackmatrix7](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Clash)

## 项目 Star 数增长趋势


