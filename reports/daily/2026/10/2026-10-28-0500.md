# 📡 サイレーダー 2026-10-28 05:00 JST

このレポートは、2026-10-27 17:00 JST〜2026-10-28 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 117
- [音声で扱う想定のトピック](#audio-topics): 10
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 79

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-35273: SSRF to RCE in Oracle PeopleSoft](#topic-16788) | 59.0 | 77.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [Introducing the Cloudflare PHP Capture the Flag challenge](#topic-38753) | 56.0 | 74.0 | 67.0 | 音声 | 温度感上位枠 |
| 3 | [Apple Backports Fix for Exploited CoreGraphics Flaw to Older iPhones and iPads](#topic-34785) | 43.0 | 56.0 | 67.0 | 音声 | 温度感上位枠 |
| 4 | [Brotli bug reaches far beyond Node.<wbr>js (CVE-2026-111497)](#topic-39379) | 39.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 5 | [iOS, macOS 27.2 Patch 286 Bugs; Fix for Exploited Flaw Backported to iOS 18](#topic-39925) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [This is Fine: What NetScaler Zero-Days Tell Us About the New Normal](#topic-39948) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 7 | [CISA confirms PHP2Shell vulnerabilities now exploited in attacks](#topic-39970) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 8 | [CyberStrikeAI Uses 44 AI Agents to Automate Hacking Operations Against Japan Targets](#topic-39859) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 9 | ['Aokigahara' Stealer Targets 'Developer Keyrings' & AI Assistants](#topic-39863) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 10 | [Tricks from the Past deployed via signed ChatGPT and Claude binaries](#topic-39903) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-16788"></a>

### 1. CVE-2026-35273: SSRF to RCE in Oracle PeopleSoft

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 59.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 77.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Oracle PeopleSoftに関するCVE-2026-35273は、未認証のリモートコード実行につながる深刻な脆弱性として扱われており、複数の公開情報で悪用の動きが示されています。
報告内容では、ShinyHuntersに関連する攻撃キャンペーンの文脈で、Webシェルの展開やデータ窃取につながる可能性が示唆されています。
認証不要でRCEに至る可能性がある脆弱性は、外部公開されたPeopleSoft環境にとって影響が大きく、侵入後の横展開や情報流出の起点になり得ます。
加えて、実際の悪用観測があるため、単なる理論上の脆弱性よりも優先度高く対応すべき対象です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 11 sources。
- 実悪用・ゼロデイ文脈。
- 技術詳細・再現情報あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 技術詳細により影響確認が進みやすい。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- PeopleSoftの対象バージョンと公開範囲を確認し、ベンダー案内に沿って速やかに修正適用の要否を判断する。
- 外部公開面で不審なリクエスト、異常なアウトバウンド通信、Webシェルの痕跡がないか点検する。
- 関連する認証情報の漏えい可能性を考慮し、必要に応じてアカウント監査やパスワード・鍵の見直しを行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-35273 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-41091 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-45657 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-50507 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ランサムウェアグループ | Clop | 主題 | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Oracle | 言及あり | 0.80 | — |
| 脅威アクター | Scattered Spider | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-35273](https://nvd.nist.gov/vuln/detail/CVE-2026-35273) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-35273: SSRF to RCE in Oracle PeopleSoft](https://www.thezdi.com/blog/2026/10/20/cve-2026-35273-ssrf-to-rce-in-oracle-peoplesoft) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShinyHunters Extorted Boeing Spin-off Prior to Arrests](https://krebsonsecurity.com/2026/10/shinyhunters-extorted-boeing-spin-off-prior-to-arrests/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Dutch Police Arrest ‘Reformed’ Hacker in Shiny Hunters Investigation](https://krebsonsecurity.com/2026/09/dutch-police-arrest-reformed-hacker-in-shiny-hunters-investigation/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Bypass WAFs to Exploit Oracle PeopleSoft Flaw and Deploy Web Shells](https://thehackernews.com/2026/09/attackers-bypass-wafs-to-exploit-oracle.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [15th June – Threat Intelligence Report](https://research.checkpoint.com/2026/15th-june-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShinyHunters is actively extorting universities after exploiting an unpatched Or](https://cyberscoop.com/oracle-peoplesoft-zero-day-vulnerability-shinyhunters-extortion/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Active Exploitation of Oracle PeopleSoft Zero-Day (CVE-2026-35273)](https://www.rapid7.com/blog/post/etr-active-exploitation-of-oracle-peoplesoft-zero-day-cve-2026-35273) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-38753"></a>

### 2. Introducing the Cloudflare PHP Capture the Flag challenge

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 56.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Cloudflareは、PHPの脆弱性を題材にしたCapture the Flagチャレンジを公開し、WAFの防御を検証する取り組みを始めました。
対象となっているCVE-2026-109618は、複数の情報源で深刻なPHP脆弱性として扱われており、公開PoCや悪用の文脈も観測されています。
PHPを利用するWeb基盤では影響範囲が広くなりやすく、脆弱性の理解と早期対策が重要です。公開PoCの存在は、実環境での悪用リスクが高まる要因として注目されます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 27 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- PHP関連のセキュリティ更新が適用済みか、影響を受ける製品・構成を確認する。
- WAFや周辺防御が該当クラスの攻撃をどこまで検知・遮断できるかを点検する。
- CVE関連の情報更新を継続監視し、利用中のCMSやミドルウェアへの波及有無を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-109618 | 関連CVE | 1.00 | 候補あり（URL 103件以上） |
| 脆弱性 | CVE-2026-109619 | 関連CVE | 1.00 | 候補あり（URL 14件以上） |
| 脆弱性 | CVE-2026-110264 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-114625 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-115560 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-109618](https://nvd.nist.gov/vuln/detail/CVE-2026-109618) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-](https://security.paloaltonetworks.com/CVE-2026-109618) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Introducing the Cloudflare PHP Capture the Flag challenge](https://blog.cloudflare.com/php-ctf/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Confirms Active Exploitation of Two PHP2Shell Flaws Enabling Remote Code Ex](https://thehackernews.com/2026/10/cisa-confirms-active-exploitation-of.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in PHP Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-php-october26-Jj384Daq) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Millions of PHP Servers Face RCE Risk as PHP2Shell Exploitation Attempts Emerge](https://blog.polyswarm.io/millions-of-php-servers-face-rce-risk-as-php2shell-exploitation-attempts-emerge) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [26th October – Threat Intelligence Report](https://research.checkpoint.com/2026/26th-october-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP2Shell security flaws now sucessfully exploited in the wild](https://www.bleepingcomputer.com/news/security/php2shell-security-flaws-now-sucessfully-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（37件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-34785"></a>

### 3. Apple Backports Fix for Exploited CoreGraphics Flaw to Older iPhones and iPads

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>i⁠O⁠S</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Appleは、CoreGraphicsの脆弱性CVE-2026-86950に対する修正を、古いiPhoneやiPad向けにもバックポートして配信しました。
この脆弱性は実際の攻撃で悪用されていたとされ、悪意あるファイルの処理を通じて任意コード実行につながる可能性があると報じられています。
既に悪用が確認されている脆弱性に対する修正であり、対象端末では早急な更新が重要です。公開PoCの言及もあるため、未更新端末のリスク評価が一段と高まります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- iOS / iPadOS / macOS の該当バージョンを確認し、速やかに適用状況を点検する。
- 悪意あるファイルの取り扱いに注意し、ユーザーへの警戒喚起を行う。
- 対象資産のOS世代が古い場合は、更新可否と代替保護策を優先的に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-86950 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Apple | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Apple iOS | 言及あり | 0.80 | — |
| ベンダー | Meta | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-86950](https://nvd.nist.gov/vuln/detail/CVE-2026-86950) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Apple Backports Fix for Exploited CoreGraphics Flaw to Older iPhones and iPads](https://thehackernews.com/2026/10/apple-backports-fix-for-exploited.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple CoreGraphics PoC Emerges as WhatsApp PDF Checks Hint at Possible Delivery ](https://thehackernews.com/2026/10/apple-coregraphics-poc-emerges-as.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Patches CoreGraphics Zero Day Exploited in Attacks](https://www.infosecurity-magazine.com/news/apple-patches-coregraphics-zero/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Zero-Day Vulnerability Weaponized in Targeted Attacks](https://www.darkreading.com/cyberattacks-data-breaches/apple-zero-day-vulnerability-weaponized-targeted-attacks) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple patches CoreGraphics zero-day already exploited in targeted attacks](https://www.theregister.com/security/2026/09/29/apple-patches-coregraphics-zero-day-already-exploited-in-targeted-attacks/5299721) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Update your iPhone, iPad, or Mac: Flaw could run attackers’ code](https://www.malwarebytes.com/blog/bugs/2026/09/update-your-iphone-ipad-or-mac-flaw-could-run-attackers-code) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple squashes zero-day bug exploited in “extremely sophisticated” attack (CVE-2](https://www.helpnetsecurity.com/2026/09/29/apple-core-graphics-zero-day-cve-2026-86950-fixed/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-39379"></a>

### 4. Brotli bug reaches far beyond Node.<wbr>js (CVE-2026-111497)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

CVE-2026-111497は、Brotli圧縮ライブラリに起因する脆弱性で、Node.<wbr>jsに限らずBrotliを組み込む複数の製品や配布物に影響が及ぶ可能性が指摘されています。
公開情報では、Node.<wbr>jsの公式ビルド上で任意コード実行につながる挙動が確認されたとされ、関連製品側でも修正や再ビルド対応が進んでいます。
圧縮ライブラリは多くのアプリケーションやランタイムに組み込まれているため、影響範囲が単一製品にとどまらない点が注目されています。
実運用では、直接Brotliを使っていなくても依存関係経由で影響を受ける可能性があるため、棚卸しと更新確認が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 10 sources。
- 実悪用・ゼロデイ文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Node.<wbr>js本体だけでなく、Brotliを内包する各種ランタイム、ミドルウェア、配布パッケージの更新状況を確認する。
- HTTPレスポンスの自動展開や圧縮データの処理を行う機能が有効な製品は、ベンダーの修正版提供状況と適用手順を確認する。
- 依存コンポーネントの見落としを防ぐため、SBOMやパッケージ一覧を使ってBrotli関連の採用有無を洗い出す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-111497 | 関連CVE | 1.00 | 候補あり（URL 24件以上） |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| ベンダー | Wiz | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| マルウェア | ZLib | 主題 | 0.80 | — |
| ベンダー | watchTowr | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-111497](https://nvd.nist.gov/vuln/detail/CVE-2026-111497) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Brotli bug reaches far beyond Node.<wbr>js (CVE-2026-111497)](https://www.helpnetsecurity.com/2026/10/27/node2shell-broccoli2shell-vulnerability-cve-2026-111497/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-111497 Portfolio Status: Impact of Brotli Vulnerability (CVE-2026-11149](https://security.paloaltonetworks.com/CVE-2026-111497) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Experts temper emergency-level alarms over critical Brotli defect](https://cyberscoop.com/brotli-critical-vulnerability-decompression-library-node2shell-broccoli2shell/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [eMudhra, Brotli, and the Long Tail of a Security Fix](https://socket.dev/blog/emudhra-brotli-security-fix) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft releases emergency .<wbr>NET security fixes for Google Brotli bug](https://www.theregister.com/security/2026/10/26/microsoft-releases-emergency-net-security-fixes-for-google-brotli-bug/5305515) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP Issues Second Windows Security Update in Five Days to Fix Brotli Code Execut](https://thehackernews.com/2026/10/php-issues-second-windows-security.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-111497: Critical out-of-bounds write in the Node.<wbr>js Brotli decoder](https://www.rapid7.com/blog/post/etr-cve-2026-111497-critical-out-of-bounds-write-in-the-node-js-brotli-decoder) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（4件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-39925"></a>

### 5. iOS, macOS 27.2 Patch 286 Bugs; Fix for Exploited Flaw Backported to iOS 18

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>i⁠O⁠S</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

AppleはiOSおよびmacOS 27.2で計286件の脆弱性修正を公表し、あわせて悪用が観測されたCoreGraphicsのゼロデイ修正を旧バージョンのiPhone向けにも適用しました。
対象範囲が広く、特定の脆弱性については既に悪用情報があるため、更新の優先度が高い内容です。広範な修正に加え、実際の悪用が示唆される脆弱性が含まれている点が注目されています。
古いiOSへのバックポートも行われており、幅広い端末で対応が必要になる可能性があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- iPhone、iPad、Macの適用対象バージョンを確認し、可能な限り早期に更新を進める。
- 資産管理上、古いOSを使い続けている端末が残っていないか棚卸しする。
- 脆弱性修正後も、端末保護や異常挙動の監視を継続し、影響有無を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Apple | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Apple iOS | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [iOS, macOS 27.2 Patch 286 Bugs; Fix for Exploited Flaw Backported to iOS 18](https://www.securityweek.com/ios-macos-27-2-patch-286-bugs-fix-for-exploited-flaw-backported-to-ios-18/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-39948"></a>

### 6. This is Fine: What NetScaler Zero-Days Tell Us About the New Normal

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | - |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Citrix NetScalerに関するゼロデイ脆弱性をめぐる話題で、継続的なパッチ提供が必要になる状況が示唆されています。
材料では悪用観測があるとされており、脆弱性対応のスピードが重要なテーマになっています。
ネットワーク境界に位置する製品で問題が起きると、影響範囲が広がりやすいため注目されています。
ゼロデイや悪用情報が伴う場合は、公開後の修正待ちでは間に合わない可能性があるためです。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Citrix NetScalerの最新情報を確認し、該当する修正版や緩和策の有無を早急に把握する。
- 外部公開機器の露出状況を点検し、不要なアクセス経路や設定の見直しを行う。
- ベンダー告知と自組織の監視を突き合わせ、侵害兆候がないか重点的に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Citrix | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [This is Fine: What NetScaler Zero-Days Tell Us About the New Normal](https://www.securityweek.com/this-is-fine-what-netscaler-zero-days-tell-us-about-the-new-normal/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-39970"></a>

### 7. CISA confirms PHP2Shell vulnerabilities now exploited in attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAがPHP2Shellの脆弱性を、実際の攻撃で悪用が確認されたものとして管理対象に追加したと報じられています。
対象となる連邦機関には、期限までの修正対応が求められているとされています。悪用が確認された脆弱性は、放置すると被害拡大につながりやすく、優先度の高い対応が必要です。
公的機関での期限付き対応は、一般の組織にとっても早急な確認・更新の目安になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- PHP2Shellに該当する環境がないかを確認し、影響範囲を把握する。
- 該当する場合は、ベンダーの修正版や推奨対策を優先適用する。
- 関連システムのログと不審な挙動を点検し、侵害兆候がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-109618 | 関連CVE | 1.00 | 候補あり（URL 103件以上） |
| 脆弱性 | CVE-2026-109619 | 関連CVE | 1.00 | 候補あり（URL 14件以上） |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA confirms PHP2Shell vulnerabilities now exploited in attacks](https://www.bleepingcomputer.com/news/security/cisa-confirms-php2shell-vulnerabilities-now-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-39859"></a>

### 8. CyberStrikeAI Uses 44 AI Agents to Automate Hacking Operations Against Japan Targets

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、AIを用いて日本の組織を狙ったとされる3件のサイバー攻撃が報告されています。
調査では、攻撃者が使ったとみられる公開サーバー環境が分析され、AIが攻撃の主導または支援に使われていた可能性が示されています。
攻撃の一部にAIが組み込まれているとされ、従来型の手口よりも作業の自動化や高度化が進む懸念があります。
日本の組織が対象に含まれているため、国内の防御・監視体制の見直しにつながる話題です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIを含む攻撃では、短時間で複数の手口が並行しやすいため、認証・端末・メール・クラウドの監視を横断的に確認する。
- 不審な公開サーバーや外部公開資産の棚卸しを進め、不要な露出や設定不備がないか点検する。
- AI由来かどうかに関わらず、初期侵入の検知とインシデント対応手順を再確認し、異常な操作・通信の検出精度を高める。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CyberStrikeAI Uses 44 AI Agents to Automate Hacking Operations Against Japan Tar](https://thehackernews.com/2026/10/cyberstrikeai-uses-44-ai-agents-to.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-39863"></a>

### 9. 'Aokigahara' Stealer Targets 'Developer Keyrings' & AI Assistants

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

『Aokigahara』と呼ばれる情報窃取型マルウェアが、開発者向けの認証情報管理やAIアシスタントの利用環境を狙っていると報じられています。
1台の端末が侵害されるだけで、AIセッションや業務データ、開発基盤に関わる情報が広く漏えいする可能性がある点が注目されています。
AIツールの利用が広がる中で、従来の情報窃取マルウェアが狙う範囲も広がっていることを示す事例です。
開発者端末やAI関連の認証情報は、侵害時の影響が大きいため、運用面での注意が必要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 開発者端末で使う認証情報管理や秘密情報の保存場所を見直し、不要な保存を避ける。
- AIアシスタントや関連サービスのセッション管理・アクセス制御を確認し、異常な利用やログインを監視する。
- 端末侵害を前提に、EDRやログ監視で情報窃取の兆候を早期に検知できる体制を整える。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | ['Aokigahara' Stealer Targets 'Developer Keyrings' & AI Assistants](https://www.darkreading.com/endpoint-security/aokigahara-stealer-developer-keyrings-ai-assistants) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-39903"></a>

### 10. Tricks from the Past deployed via signed ChatGPT and Claude binaries

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Check Point Research は、ChatGPT や Claude など人気のAIツールを装った偽のGitHubプロジェクトを通じて、独自のマルウェア連鎖が配布されていたと報告しています。
掲載情報では、署名付きのバイナリが悪用されていた可能性が示されており、AI関連アプリを装う手口が確認されています。
AIツールへの関心の高さを悪用するため、利用者や開発者が正規アプリと見分けにくい点が注意点です。
署名済みバイナリが関与しているとされるため、一般的な信頼判断だけでは不十分になり得ます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI関連の新規GitHubプロジェクトや配布物は、提供元・公開履歴・署名情報を含めて慎重に確認する。
- エンドポイント側では、未承認の実行ファイルや不審な子プロセス、外部通信の増加を監視する。
- ユーザー向けには、AIデスクトップアプリの入手元を公式チャネルに限定し、導入前の検証手順を徹底する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Check Point | 言及あり | 0.80 | — |
| ベンダー | Anthropic | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Mozilla | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| ベンダー | Meta | 言及あり | 0.80 | — |
| ベンダー | F5 | 言及あり | 0.80 | — |
| 製品 | Cursor | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | ChatGPT | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Tricks from the Past deployed via signed ChatGPT and Claude binaries](https://research.checkpoint.com/2026/tricks-from-the-past-deployed-via-signed-chatgpt-and-claude-binaries/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

今回はGitHubのみ掲載の注目トピックはありません。

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [CISAが既知の悪用済み脆弱性カタログに2件を追加](https://www.cisa.gov/news-events/alerts/2026/10/27/cisa-adds-two-known-exploited-vulnerabilities-catalog) | 45.0 | 38.0 | 43.0 |
| [AI生成の偽ログインページがアカウント乗っ取りを容易にしている](https://thehackernews.com/2026/10/ai-generated-fake-login-pages-are.html) | 33.0 | 20.0 | 42.0 |
| [盗まれたGitHubトークンを悪用するGheistキャンペーンで秘密情報が非公開リポジトリから流出し続ける](https://www.helpnetsecurity.com/2026/10/27/gheist-github-token-abuse/) | 28.0 | 45.0 | 42.0 |
| [HiveおよびNefilimランサムウェアの関係者が70か月の懲役刑に処される](https://cyberscoop.com/nefilim-hive-ransomware-affiliate-artem-stryzhak-sentenced/) | 28.0 | 30.0 | 42.0 |
| [サイバーインシデントによりUNM Healthが手術を中止し救急搬送先を変更](https://www.infosecurity-magazine.com/news/cyber-unmhealth-surgeries/) | 28.0 | 30.0 | 42.0 |
| [Teamsの外部チャットを悪用した攻撃で15分未満に組織侵入](https://www.infosecurity-magazine.com/news/exploit-teams-chat-breach/) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア侵入前にセキュリティツールが停止すると何が起きるのか](https://cyberscoop.com/warlock-ransomware-storm-2603-sharepoint-attacks-op-ed/) | 28.0 | 30.0 | 42.0 |
| [スパムで受信箱を埋めた後、Microsoft TeamsでITサポートを装うハッカー](https://www.helpnetsecurity.com/2026/10/27/microsoft-teams-social-engineering-fake-it-help-desk/) | 28.0 | 20.0 | 42.0 |
| [悪意あるアプリが燃料価格やドローン攻撃へのロシア人の不安につけ込む](https://therecord.media/malicious-apps-russian-anxiety-gas-prices-drone-strikes) | 28.0 | 20.0 | 42.0 |
| [Lazarusが韓国のセキュリティソフトを悪用し、耐量子暗号を用いてマルウェアを展開](https://thehackernews.com/2026/10/lazarus-abuses-south-korean-security.html) | 28.0 | 20.0 | 42.0 |
| [Australia、Amadeyマルウェアのバックエンドに介入し、18万台の感染端末へのアクセスを遮断](https://thehackernews.com/2026/10/australia-gets-into-amadey-malware.html) | 28.0 | 20.0 | 42.0 |
| [AIハッカーが人気の産業制御ソフトウェアで4件の重大な脆弱性を4時間未満で発見](https://www.theregister.com/security/2026/10/27/ai-hacker-finds-4-severe-bugs-in-popular-industrial-control-software-in-under-4-hours/5305811) | 25.0 | 20.0 | 42.0 |
| [AIがサイバーセキュリティ専門家のスキルを奪う可能性に警戒せよ](https://www.darkreading.com/cybersecurity-operations/ai-kill-off-cybersecurity-pros-skills) | 25.0 | 20.0 | 42.0 |
| [WarpがAIエージェントのログとユーザーテレメトリデータ流出の侵害を公表](https://www.bleepingcomputer.com/news/security/warp-discloses-breach-exposing-ai-agent-logs-user-telemetry-data/) | 25.0 | 20.0 | 42.0 |
| [OpenAIのコンパクション脆弱性によりAIの推論内容が研究者に露出した問題](https://www.infosecurity-magazine.com/news/openai-compaction-flaw-ai/) | 25.0 | 20.0 | 42.0 |
| [Microsoft Teamsに新たなAI機能、フィッシング攻撃対策を強化](https://www.itpro.com/security/phishing/microsoft-teams-is-getting-a-suite-new-ai-features-to-crack-down-on-phishing-attacks) | 25.0 | 20.0 | 42.0 |
| [ISC2、AIセキュリティ人材の未来に向けてCyber-AI Workforce Coalitionを発足](https://www.infosecurity-magazine.com/news/isc2-launches-cyberai-workforce/) | 25.0 | 20.0 | 42.0 |
| [SocureがAIエージェントを本人確認済みの個人・企業に紐づける](https://www.helpnetsecurity.com/2026/10/27/socure-agent-intelligence/) | 25.0 | 20.0 | 42.0 |
| [DNSFilter、LUMINATEでDNSセキュリティ・AI制御・リモートワーク保護を統合](https://www.helpnetsecurity.com/2026/10/27/dnsfilter-luminate/) | 25.0 | 20.0 | 42.0 |
| [AI時代の愛と欺瞞、人工的な親密さ](https://www.malwarebytes.com/blog/ai/2026/10/artificial-intimacy-love-and-lies-in-the-age-of-ai) | 25.0 | 20.0 | 42.0 |
| [ExeonがシャドーAIと自律エージェントへの脅威検知を拡張](https://www.helpnetsecurity.com/2026/10/27/exeon-expands-threat-detection-to-shadow-ai-and-autonomous-agents/) | 25.0 | 20.0 | 42.0 |
| [ThreatAware、AI構築のセキュリティアプリケーションにガバナンスを導入](https://www.helpnetsecurity.com/2026/10/27/threataware-dimension-governed-workspace/) | 25.0 | 20.0 | 42.0 |
| [Anthropic投資家向けに明らかにされたリスクに、暴走AIによる潜在的被害も含まれる](https://www.securityweek.com/risks-spelled-out-for-anthropic-investors-include-possible-harms-from-runaway-ai/) | 25.0 | 20.0 | 42.0 |
| [ISC2による初のAIセキュリティ認定資格、2027年初頭に登場見込み](https://www.infosecurity-magazine.com/news/first-isc2-ai-security/) | 25.0 | 20.0 | 42.0 |
| [OpenAIの圧縮処理の不備により隠された推論保護を回避可能に](https://thehackernews.com/2026/10/openai-compaction-flaw-let-researchers.html) | 25.0 | 20.0 | 42.0 |
| [EPICS Baseの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-300-01) | 24.0 | 46.0 | 50.0 |
| [HPE、ネットワーキング製品の多数の重大な脆弱性を修正](https://www.securityweek.com/hpe-patches-dozens-of-critical-flaws-in-networking-products/) | 24.0 | 38.0 | 42.0 |
| [Mitsubishi ElectricのGENESIS、GENESIS64、ICONICS Suite、Hyper Historian、AnalytiX、MobileHMI、IoTWorX、MC Works64、GENESIS32、BizVizに関する脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-300-02) | 22.0 | 36.0 | 50.0 |
| [TailscaleのSSH脆弱性によりroot権限昇格の可能性](https://www.bleepingcomputer.com/news/security/tailscale-warns-of-serious-ssh-flaws-allowing-root-privilege-escalation/) | 22.0 | 32.0 | 42.0 |
| [Firefoxの悪意ある拡張機能がPhantom、Jupiter、Bitgetを装ってウォレットの秘密情報を窃取](https://socket.dev/blog/firefox-wallet-impersonators) | 22.0 | 20.0 | 42.0 |
| [49システムで情報流出、横展開など確認 - ユミルリンク](https://www.security-next.com/192029) | 22.0 | 20.0 | 42.0 |
| [連邦SOCからTalosへ：Ryan Fettermanが語る実践的なセキュリティ研究](https://blog.talosintelligence.com/from-federal-socs-to-talos-ryan-fetterman-on-practical-security-research/) | 22.0 | 20.0 | 42.0 |
| [バンナム子会社に不正アクセス - 「一番くじONLINE」配送情報が流出か](https://www.security-next.com/191994) | 22.0 | 20.0 | 42.0 |
| [婚活イベントで申込者情報を誤公開、開催中止に - 岡山県](https://www.security-next.com/191915) | 22.0 | 20.0 | 42.0 |
| [GMO、不正アクセス関与者の特定に総額1.6億円の懸賞金 見舞金最大300万円](https://xtech.nikkei.com/atcl/nxt/news/24/03442/) | 21.0 | 20.0 | 42.0 |
| [GMO、不正アクセス実行犯の手がかりに懸賞金 1億5000万円規模](https://www.itmedia.co.jp/news/article/2610/27/2000002642/) | 21.0 | 20.0 | 42.0 |
| [So-net、会員情報約259万件が漏えい 一部メールサービスではパスワードも流出](https://www.itmedia.co.jp/news/article/2610/27/2000002643/) | 21.0 | 20.0 | 42.0 |
| [富士通、企業のサイバー防衛を支援するソリューションを提供](https://news.mynavi.jp/techplus/article/20261027-5205058/) | 21.0 | 20.0 | 42.0 |
| [オムロンとNTTドコモビジネス、製造現場向けOT/IT統合セキュリティで協業](https://news.mynavi.jp/techplus/article/20261027-5204816/) | 21.0 | 20.0 | 42.0 |
| [GMO、攻撃者の公開情報に「アクセスは絶対に控えて」 悪質な拡散者には法的措置を準備](https://www.itmedia.co.jp/news/article/2610/27/2000002640/) | 21.0 | 20.0 | 42.0 |
| [北海道企業の26.5%以上がサイバー攻撃を経験、HENNGEらの調査で判明](https://news.mynavi.jp/techplus/article/20261027-5204508/) | 21.0 | 20.0 | 42.0 |
| [Microsoft Authenticatorの脆弱性により権限不要のAndroidアプリがWorkアカウントのトークンを窃取可能に](https://thehackernews.com/2026/10/microsoft-authenticator-flaw-let.html) | 20.0 | 28.0 | 50.0 |
| [University of New MexicoのHealth Sciences Centerへのサイバー攻撃で休講が2日目に突入](https://www.theregister.com/cyber-crime/2026/10/27/day-2-of-canceled-classes-at-university-of-new-mexico-after-health-sciences-center-cyberattack/5305690) | 20.0 | 20.0 | 42.0 |
| [953件のオンラインストアにスキャナー回避コードを感染させたハッカー](https://www.infosecurity-magazine.com/news/hackers-infect-953-online-stores/) | 20.0 | 20.0 | 42.0 |
| [選挙を狙う5つの詐欺に注意](https://www.malwarebytes.com/blog/scams/2026/10/five-election-scams-to-watch-out-for) | 20.0 | 20.0 | 42.0 |
| [🎙️SECURITY.COMのポッドキャスト：スコアの裏側](https://www.security.com/expert-perspectives/security-dot-com-podcast-behind-scores) | 20.0 | 20.0 | 42.0 |
| [CISAとセキュリティ研究者、PHPの脆弱性悪用を確認](https://www.cybersecuritydive.com/news/cisa-security-researchers-exploitation-php-flaws/872886/) | 20.0 | 20.0 | 42.0 |
| [Tailscaleが「Tailworm」脆弱性の無調整公開を受けて緊急修正を実施](https://www.securityweek.com/tailscale-rushes-patches-after-uncoordinated-disclosure-of-tailworm-flaws/) | 20.0 | 20.0 | 42.0 |
| [National cyber director、サウスカロライナ州で農村部病院向けの最新パイロットを開始](https://cyberscoop.com/oncd-rural-hospital-cybersecurity-pilot-project-lifeline-250/) | 20.0 | 20.0 | 42.0 |
| [英国警察データを保有するサプライヤーがハッカーに繰り返し侵害されたと監督機関が指摘](https://therecord.media/uk-police-data-breached-from-suppliers-watchdog-report) | 20.0 | 20.0 | 42.0 |
| [University of New Mexico病院、サイバー攻撃後に救急車の受け入れを転換](https://therecord.media/university-of-new-mexico-hospital-diverts-cyber-incident) | 20.0 | 20.0 | 42.0 |
| [CISAがPHP2Shellへの攻撃を確認、研究者が攻撃成功を観測](https://www.theregister.com/cyber-crime/2026/10/27/cisa-confirms-php2shell-under-attack-as-researchers-clock-successful-exploits/5305681) | 20.0 | 20.0 | 42.0 |
| [Apple製品の複数の脆弱性により任意のコードが実行される可能性](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-apple-products-could-allow-for-arbitrary-code-execution_2026-121) | 20.0 | 20.0 | 42.0 |
| [米国、地方の病院向けに無料のサイバーセキュリティ支援プログラムを開始](https://www.cybersecuritydive.com/news/healthcare-cybersecurity-white-house-pilot-program-launch/872872/) | 20.0 | 20.0 | 42.0 |
| [GMO不正アクセス 警視庁が捜査](https://news.yahoo.co.jp/pickup/6600351?source=rss) | 20.0 | 20.0 | 42.0 |
| [SkyW4lkerが露呈：米国企業を狙うMicrosoft 365フィッシング脅威の拡大](https://any.run/cybersecurity-blog/skyw4lker-phishing-kit-analysis/) | 20.0 | 20.0 | 42.0 |
| [Huntress Tragic Quadrant：企業への被害が最も大きい脅威のランキング](https://www.bleepingcomputer.com/news/security/the-huntress-tragic-quadrant-ranking-threats-hitting-businesses-hardest/) | 20.0 | 20.0 | 42.0 |
| [GoAheadのTLS脆弱性により失効したクライアント証明書が許可されセッション復号が可能に](https://thehackernews.com/2026/10/goahead-tls-flaws-allow-revoked-client.html) | 20.0 | 20.0 | 42.0 |
| [ベンダーのキー漏えいでデンバー健康保険プラン加入者23万8000人のデータが危険にさらされる](https://www.securityweek.com/vendor-key-leak-puts-data-of-238000-denver-health-plan-members-at-risk/) | 20.0 | 20.0 | 42.0 |
| [PHP2Shellの悪用試行と対処動向](https://www.wiz.io/blog/php2shell-exploitation-so-far) | 20.0 | 20.0 | 42.0 |
| [CISA、PHPの脆弱性悪用試行を警告　連邦機関に数日以内の修正を要請](https://therecord.media/php-vulnerabilities-cisa-kev) | 20.0 | 20.0 | 42.0 |
| [英国の警察・消防機関にサイバー能力強化を促す呼びかけ](https://www.itpro.com/security/uk-police-and-fire-services-urged-to-bolster-cyber-capabilities) | 20.0 | 20.0 | 42.0 |
| [オーストラリアの諜報機関、ハッキング標的と情報を共有し相互提供を求める](https://therecord.media/australia-spies-share-intel-and-want-victims-to-share-back) | 20.0 | 20.0 | 42.0 |
| [Sekoia、厳格なデータ管理を求める組織向けに自社ホスト型デプロイを導入](https://www.helpnetsecurity.com/2026/10/27/sekoia-self-hosted/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、証明書更新を含むWindowsの緊急修正を公開](https://www.theregister.com/security/2026/10/27/microsoft-releases-out-of-band-windows-fixes-with-certificate-updates/5305637) | 20.0 | 20.0 | 42.0 |
| [University of New Mexicoの病院でサイバー攻撃が発生、恐喝グループが犯行を主張](https://www.helpnetsecurity.com/2026/10/27/university-of-new-mexico-hospitals-cyberattack/) | 20.0 | 20.0 | 42.0 |
| [Rapid7 Command PlatformでSCIMを用いたユーザーアクセス管理の簡素化](https://www.rapid7.com/blog/post/pt-scim-simplifies-user-access-management-uam-command-platform) | 20.0 | 20.0 | 42.0 |
| [Webが少し荒れ模様の今、安全に閲覧する方法](https://www.malwarebytes.com/blog/news/2026/10/the-webs-having-a-rough-week-heres-how-to-browse-safely) | 20.0 | 20.0 | 42.0 |
| [CISA、米国の重要インフラからサイバー攻撃者を排除する計画を示す](https://www.helpnetsecurity.com/2026/10/27/cisa-2030-cyber-resilience-strategy/) | 20.0 | 20.0 | 42.0 |
| [説明のないDreamHostのインシデントでメールとFTPのパスワードがリセットされる](https://www.securityweek.com/unexplained-dreamhost-incident-prompts-email-ftp-password-resets/) | 20.0 | 20.0 | 42.0 |
| [ドイツ極右政党AfD向けメールホスティング事業者への攻撃で34万5,000件のアカウントが流出](https://www.theregister.com/cyber-crime/2026/10/27/attack-on-email-hosting-provider-for-german-far-right-party-afd-exposed-345k-accounts/5305660) | 20.0 | 20.0 | 42.0 |
| [コペンハーゲン大学へのサイバー攻撃で52万5000人分のデータが流出](https://www.helpnetsecurity.com/2026/10/27/university-of-copenhagen-cyberattack-data-breach/) | 20.0 | 20.0 | 42.0 |
| [Copenhagen Universityの侵害で50万人分のデータが漏えい](https://www.infosecurity-magazine.com/news/copenhagen-university-data-breach/) | 20.0 | 20.0 | 42.0 |
| [Samsung TVはマイクなしでもサウンドバー経由で音声を聞ける可能性があると研究者が指摘](https://www.malwarebytes.com/blog/privacy/2026/10/samsung-tvs-without-mics-may-listen-through-soundbars-researcher-says) | 20.0 | 20.0 | 42.0 |
| [DreamHostのインシデントでパスワード再設定が必要に、顧客のメールとFTPアカウントがロックアウト](https://www.helpnetsecurity.com/2026/10/27/dreamhost-incident-email-ftp-password-resets/) | 20.0 | 20.0 | 42.0 |
| [Dead Popcorn Timeアップデーターが数百万台のコンピューターを乗っ取りの危険にさらした](https://www.securityweek.com/dead-popcorn-time-updater-put-millions-of-computers-at-risk-of-takeover/) | 20.0 | 20.0 | 42.0 |
| [警察と消防のサイバーセキュリティ強化を監督機関が要請](https://www.infosecurity-magazine.com/news/watchdog-police-fire-service/) | 20.0 | 20.0 | 42.0 |
| [エネルギー大手ENGIE、顧客に影響するデータ侵害を公表](https://www.bleepingcomputer.com/news/security/energy-giant-engie-discloses-data-breach-affecting-customers/) | 20.0 | 20.0 | 42.0 |
| [ユミルリンク「Cuenote FC」不正アクセスの影響広がる、JR東海、りそなグループらが相次ぎ発表 インプレスのメルマガ配信にも影響の可能性](https://internet.watch.impress.co.jp/docs/news/2151621.html) | 20.0 | 20.0 | 42.0 |

---

## 📊 スコアの見方

| 指⁠標 | 意味 |
|---|---|
| 温⁠度⁠状⁠態 | 話題のライフサイクルを示す補助ラベルです。例: 初出、継続監視、温度上昇中、高温、冷却中、再燃、低温。 |
| 温⁠度⁠感 | 話題として今どれだけ注目・拡散・更新されているかを示します。 |
| 実⁠務⁠影⁠響 | 対象組織・担当者にとって、対応優先度や被害可能性がどれだけ大きいかを示します。 |
| 確⁠度 | 公的機関、ベンダー公式、複数ソース、CVE/KEV、一次資料などにより、情報をどれだけ確認できているかを示します。事件報道系は、複数報道があっても司法文書・当局発表などの一次資料が弱い場合、脆弱性KEV系より低く出ることがあります。 |

スコアは、公開情報から抽出した特徴量と事前定義した重み付けに基づく参考指標です。詳しい算出方針は [スコアリング方針](https://github.com/cyberheatradar/cyber-heat-radar/blob/main/docs/scoring.md) を参照してください。

## 🔒 公開しない内部情報について

サイレーダーでは、温度感の補助シグナルとして、公的機関・ベンダー公式・信頼できる報道機関・技術者コミュニティ・国内外の公開反応などを利用します。

これらのシグナルは、一次情報、報道波及、技術者反応、開発者反応、PoC・悪用観測などに分けて評価します。

ただし、ランキング操作、スパム的誘導、監視回避を防ぐため、個別の監視対象、取得手段、検索条件、評価対象サービス名、内部的な重み付けやしきい値は公開しません。

また、公開反応の多さだけで掲載順位を決めることはありません。重要度の判定では、ベンダー公式情報、公的機関、一次資料、信頼できる技術分析、実務影響を優先します。

## ⚠️ 注意事項

このレポートは、収集・観測できた公開情報をもとにした参考情報です。完全性、正確性、即時性を保証するものではありません。

重要な判断を行う場合は、必ずベンダー公式情報、公的機関、一次情報を確認してください。

サイレーダーは、広告・スポンサー・企業関係に基づいて掲載順位や温度感スコアを変更しません。
