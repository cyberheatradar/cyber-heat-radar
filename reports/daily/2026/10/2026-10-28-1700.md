# 📡 サイレーダー 2026-10-28 17:00 JST

このレポートは、2026-10-28 11:00 JST〜2026-10-28 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 55
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 3
- [低温だが記録しておくトピック](#low-record-topics): 27

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [ShinyHunters-Exploited Oracle PeopleSoft Zero-Day Turns Out to Be Three Chained Flaws](#topic-16788) | 59.0 | 77.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-2026-109619) on Palo Alto Networks Products (Severity: CRITICAL)](#topic-38753) | 56.0 | 74.0 | 67.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [CVE-2026-111497: CISA KEV catalog addition](#topic-39379) | 40.0 | 64.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 4 | [「Adobe Campaign Classic」など4製品に脆弱性 - 「クリティカル」脆弱性も](#topic-40080) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-40080"></a>

### 1. 「Adobe Campaign Classic」など4製品に脆弱性 - 「クリティカル」脆弱性も

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Adobeは、「Adobe Campaign Classic」や「Adobe Connect」を含む4製品向けのセキュリティアップデートを公開しました。
修正対象には「クリティカル」とされる脆弱性も含まれているとされています。複数製品にまたがる修正であり、利用中の環境によっては広く影響を受ける可能性があります。
特に高深刻度の脆弱性が含まれるため、適用優先度の判断が重要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 利用中のAdobe製品と対象バージョンを確認し、該当する更新の有無を点検する。
- 公開された修正内容の深刻度を確認し、インターネット公開環境や重要業務系から優先して適用計画を立てる。
- アップデート適用までの間は、関連サービスの監視を強め、異常な挙動がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Adobe | 言及あり | 0.80 | — |
| 製品 | Adobe Campaign Classic | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [「Adobe Campaign Classic」など4製品に脆弱性 - 「クリティカル」脆弱性も](https://www.security-next.com/192042) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-16788"></a>

### 1. ShinyHunters-Exploited Oracle PeopleSoft Zero-Day Turns Out to Be Three Chained Flaws

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 59.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 77.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Oracle PeopleSoftの脆弱性CVE-2026-35273について、当初は1つの欠陥として扱われていたものが、実際には3つの連鎖した不備で構成されている可能性が報告されています。
公開情報では、ShinyHuntersに関連する活動の中でこの脆弱性が悪用されたとされ、未認証のリモートコード実行につながる深刻な問題として注目されています。
認証なしでのコード実行に結びつく可能性があるため、影響範囲が広くなりやすい点が重要です。
さらに、ゼロデイとしての悪用や継続的な攻撃文脈が示されており、パッチ適用だけでなく実際の侵害有無の確認も急がれます。

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

- PeopleSoftの該当バージョンで修正適用状況を確認し、未適用なら優先対応する。
- 外部公開面と管理系インターフェースの露出を見直し、不要な到達経路を制限する。
- 関連ログを点検し、異常なリクエストや不審なWebシェル設置の兆候がないか確認する。

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
| <nobr>出典</nobr> | [ShinyHunters-Exploited Oracle PeopleSoft Zero-Day Turns Out to Be Three Chained ](https://thehackernews.com/2026/10/shinyhunters-exploited-oracle.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-35273: SSRF to RCE in Oracle PeopleSoft](https://www.thezdi.com/blog/2026/10/20/cve-2026-35273-ssrf-to-rce-in-oracle-peoplesoft) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShinyHunters Extorted Boeing Spin-off Prior to Arrests](https://krebsonsecurity.com/2026/10/shinyhunters-extorted-boeing-spin-off-prior-to-arrests/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Dutch Police Arrest ‘Reformed’ Hacker in Shiny Hunters Investigation](https://krebsonsecurity.com/2026/09/dutch-police-arrest-reformed-hacker-in-shiny-hunters-investigation/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Bypass WAFs to Exploit Oracle PeopleSoft Flaw and Deploy Web Shells](https://thehackernews.com/2026/09/attackers-bypass-wafs-to-exploit-oracle.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [15th June – Threat Intelligence Report](https://research.checkpoint.com/2026/15th-june-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShinyHunters is actively extorting universities after exploiting an unpatched Or](https://cyberscoop.com/oracle-peoplesoft-zero-day-vulnerability-shinyhunters-extortion/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-38753"></a>

### 2. CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-2026-109619) on Palo Alto Networks Products (Severity: CRITICAL)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 56.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

PHPにおける2件の脆弱性（CVE-2026-109618、CVE-2026-109619）について、Palo Alto NetworksやJPCERT/CCなど複数の情報源が注意喚起しています。
公開情報では、認証不要のリモートコード実行につながる可能性が示されており、関連製品やPHPを利用する環境への影響が懸念されています。
公開PoCや悪用の文脈があるとされ、実際の攻撃に転用されるリスクが高まるためです。PHPは広く使われているため、Web基盤全体への影響が大きくなりやすい点が注目されています。

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

- PHPを利用するサーバーや関連製品が影響範囲に入るか確認し、ベンダーの案内に沿って修正版へ更新する。
- 外部公開されたWebサービスや管理系インターフェースを優先して点検し、不要な露出を減らす。
- ログや監視を強化し、不審な挙動や異常なプロセス生成がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-109618 | 関連CVE | 1.00 | 候補あり（URL 105件以上） |
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
| <nobr>出典</nobr> | [Weekly Report: PHPにおける複数の脆弱性（CVE-2026-109618、CVE-2026-109619）に関する注意喚起](https://www.jpcert.or.jp/wr/2026/wr261028.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in PHP Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-php-october26-Jj384Daq) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Introducing the Cloudflare PHP Capture the Flag challenge](https://blog.cloudflare.com/php-ctf/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Confirms Active Exploitation of Two PHP2Shell Flaws Enabling Remote Code Ex](https://thehackernews.com/2026/10/cisa-confirms-active-exploitation-of.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Millions of PHP Servers Face RCE Risk as PHP2Shell Exploitation Attempts Emerge](https://blog.polyswarm.io/millions-of-php-servers-face-rce-risk-as-php2shell-exploitation-attempts-emerge) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [26th October – Threat Intelligence Report](https://research.checkpoint.com/2026/26th-october-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（38件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-39379"></a>

### 3. CVE-2026-111497: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 40.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

CISA が CVE-2026-111497 を Known Exploited Vulnerabilities（KEV）カタログに追加したとされ、Node.<wbr>js に関連する Brotli まわりの脆弱性として注目されています。
公開情報では、Node.<wbr>js 側の修正公表後に、実環境での悪用を示す文脈や複数の技術系・製品系ソースでの言及が確認されています。
KEV への追加は、単なる脆弱性情報ではなく、実際の悪用可能性や優先対応の必要性が高いことを示すシグナルです。
Node.<wbr>js を利用する製品やサービスに影響が広がる可能性があるため、依存関係を含めた確認が重要になります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 11 sources。
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

- Node.<wbr>js を直接利用していなくても、組み込みライブラリや依存コンポーネント経由で影響を受ける可能性があるため、影響範囲を洗い出す。
- ベンダーや各製品の修正版・緩和策の案内を確認し、該当環境は優先的に更新計画へ載せる。
- Brotli を処理する機能や外部入力を受ける経路について、監視とログ確認を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-105482 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-105483 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-106069 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-111497 | 関連CVE | 1.00 | 候補あり（URL 27件以上） |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| ベンダー | Wiz | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-111497](https://nvd.nist.gov/vuln/detail/CVE-2026-111497) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-111497 Portfolio Status: Impact of Brotli Vulnerability (CVE-2026-11149](https://security.paloaltonetworks.com/CVE-2026-111497) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Adobe Commerce PolyShell Attacks Breach Hundreds of Stores as Brotli Exploit Tra](https://thehackernews.com/2026/10/adobe-commerce-polyshell-attacks-breach.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in node.js Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-oct2026-node-js-Jj3SQ19u) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Brotli bug reaches far beyond Node.<wbr>js (CVE-2026-111497)](https://www.helpnetsecurity.com/2026/10/27/node2shell-broccoli2shell-vulnerability-cve-2026-111497/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Experts temper emergency-level alarms over critical Brotli defect](https://cyberscoop.com/brotli-critical-vulnerability-decompression-library-node2shell-broccoli2shell/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [eMudhra, Brotli, and the Long Tail of a Security Fix](https://socket.dev/blog/emudhra-brotli-security-fix) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft releases emergency .<wbr>NET security fixes for Google Brotli bug](https://www.theregister.com/security/2026/10/26/microsoft-releases-emergency-net-security-fixes-for-google-brotli-bug/5305515) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（5件）。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [AI音声の詐欺電話、6人に1人が応じる可能性 だまされやすい手口とは 米ハーバード大やMetaが4100人で検証](https://www.itmedia.co.jp/news/article/2610/28/2000002612/) | 28.0 | 20.0 | 42.0 |
| [「禁止」するだけでは防げない？ パナソニックグループで約33万人分の個人情報が外部生成AIに](https://www.itmedia.co.jp/enterprise/articles/2610/28/news060.html) | 26.0 | 20.0 | 42.0 |
| [Anthropic、独自の“創薬活動”に着手 社員1人のバイオ企業を買収、小児難病の治療薬研究を進める](https://www.itmedia.co.jp/news/article/2610/28/2000002661/) | 26.0 | 20.0 | 42.0 |
| [Bellini CapitalのCISOが語るAIセキュリティガバナンスとパッチ適用高速化の限界](https://www.helpnetsecurity.com/2026/10/28/brian-blakley-bellini-capital-ai-security-governance/) | 25.0 | 20.0 | 42.0 |
| [「刑務所でベジマイトを食べるのはオーストラリア人の権利」と受刑者が主張するも敗訴](https://gigazine.net/news/20261028-prisons-right-to-eat-vegemite/) | 22.0 | 20.0 | 42.0 |
| [Kubernetes向けツール「consul-k8s」に脆弱性 - 修正版が公開](https://www.security-next.com/192027) | 22.0 | 20.0 | 42.0 |
| [イスラエル企業がStarlinkユーザーの位置情報特定や監視を目的として広告を出稿していた可能性大](https://gigazine.net/news/20261028-israeli-company-targeted-starlink-users/) | 22.0 | 20.0 | 42.0 |
| [資さんうどん、従業員の退職理由などが外部から閲覧可能に 委託先の勤怠システムに設定不備](https://www.itmedia.co.jp/news/article/2610/28/2000002667/) | 21.0 | 20.0 | 42.0 |
| [クラウドストライク、攻撃AIと防御AIを競わせる「SafeMind」で自律防御を加速](https://japan.zdnet.com/article/35254087/) | 21.0 | 20.0 | 42.0 |
| [GMO、攻撃者サイトの停止を確認 サイバー攻撃で盗んだ個人情報を掲載](https://xtech.nikkei.com/atcl/nxt/news/24/03444/) | 21.0 | 20.0 | 42.0 |
| [顧客も巻き込むサイバー脅迫 GMO攻撃が問う企業の防御と国の対処、被害の連鎖どう断つ](https://www.itmedia.co.jp/news/article/2610/28/2000002660/) | 21.0 | 20.0 | 42.0 |
| [GMO不正アクセスの犯人サイト、ドメイン停止を確認](https://www.itmedia.co.jp/news/article/2610/28/2000002659/) | 21.0 | 20.0 | 42.0 |
| [個人情報が漏えいしたらどうする？ IPAが被害別の対処法を公開](https://news.mynavi.jp/techplus/article/20261028-5209154/) | 21.0 | 20.0 | 42.0 |
| [ヤクルト本社サイト、不正アクセスで停止中 顧客情報への影響は「調査中」](https://www.itmedia.co.jp/news/article/2610/28/2000002657/) | 21.0 | 20.0 | 42.0 |
| [GMOがFX取引クラウド侵害の背後にいるハッカー発見に100万ドルの報奨金を提示](https://thehackernews.com/2026/10/japans-gmo-offers-1-million-bounty-to.html) | 20.0 | 20.0 | 42.0 |
| [TailscaleがSSHの脆弱性を修正、侵害された端末が他のサーバーでroot権限を得る恐れ](https://thehackernews.com/2026/10/tailscale-patches-ssh-flaws-that-could.html) | 20.0 | 20.0 | 42.0 |
| [AbuseBox: ブラックリスト、DNS、SSL、メールレコードを監視するオープンソースツール](https://www.helpnetsecurity.com/2026/10/28/abusebox-open-source-ip-blacklist-monitoring/) | 20.0 | 20.0 | 42.0 |
| [Third Serengeti Sweep、捜査の進展に伴い逮捕者数が1,400人超に](https://www.darkreading.com/cybersecurity-operations/third-serengeti-sweep-1400-arrests-investigations-mature) | 20.0 | 20.0 | 42.0 |
| [ヤマハの法人向けWi-Fiルーター「NWR100」に複数の脆弱性、ファームウェアの更新を](https://internet.watch.impress.co.jp/docs/news/2151895.html) | 20.0 | 20.0 | 42.0 |
| [NIST、量子耐性のない暗号の廃止に向けたカウントダウンを開始](https://www.helpnetsecurity.com/2026/10/28/nist-post-quantum-cryptography-migration-roadmap/) | 20.0 | 20.0 | 42.0 |
| [ヤマハ製NWR100における複数の脆弱性](https://jvn.jp/vu/JVNVU91027179/) | 20.0 | 20.0 | 42.0 |
| [GMOへの「劇場型」攻撃 狙いは](https://news.yahoo.co.jp/pickup/6600424?source=rss) | 20.0 | 20.0 | 42.0 |
| [自分たちのデータが見知らぬ企業に保管されていたことを被害者が発見](https://www.helpnetsecurity.com/2026/10/28/kroll-third-party-data-breaches-insurance-claims-report/) | 20.0 | 20.0 | 42.0 |
| [Yamaha LAN Monitor for WindowsのインストーラにおけるDLL読み込みに関する脆弱性](https://jvn.jp/jp/JVN23695234/) | 20.0 | 20.0 | 42.0 |
| [ヤマハ製YMS-VPN8およびYMS-VPN8-CPにおける引用符で囲まれていないファイルパスの脆弱性](https://jvn.jp/jp/JVN30675482/) | 20.0 | 20.0 | 42.0 |
| [Google Chromeの複数の脆弱性により任意コードが実行される可能性](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-google-chrome-could-allow-for-arbitrary-code-execution_2026-122) | 20.0 | 20.0 | 42.0 |
| [GMOを攻撃した集団のサイト停止](https://news.yahoo.co.jp/pickup/6600397?source=rss) | 20.0 | 20.0 | 42.0 |

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
