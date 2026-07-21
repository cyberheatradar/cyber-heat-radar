# 📡 サイレーダー 2026-07-22 05:00 JST

このレポートは、2026-07-21 17:00 JST〜2026-07-22 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 99
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 66

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Qilin Ransomware Attackers Exploit PAN-OS Authentication Bypass for Initial Access](#topic-4247) | 56.0 | 77.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [SonicWall SMA zero-days were exploited weeks before disclosure](#topic-22364) | 52.0 | 74.0 | 67.0 | 音声 | 温度感上位枠 |
| 3 | [CISA Adds Four Known Exploited Vulnerabilities to Catalog](#topic-23517) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN Validator Authenticated Privilege Escalation Vulnerability](#topic-15753) | 43.0 | 58.0 | 66.0 | 音声 | 温度感上位枠 |
| 5 | [JadePuffer returns with ransomware built to target AI models and infrastructure](#topic-23487) | 41.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [Exploitation of ServiceNow Vulnerability Seen Days After Disclosure](#topic-23291) | 37.0 | 64.0 | 55.0 | 音声 | AI×Security枠 |
| 7 | [Pwn2Own Ireland 2026 – New Targets and Categories](#topic-23469) | 37.0 | 20.0 | 43.0 | 音声 | AI×Security枠 |
| 8 | [WordPress wp2shell Exploitation Grows as Public Exploit Fuels Mass Scanning](#topic-23164) | 33.0 | 56.0 | 67.0 | GitHub | 音声枠上限によりGitHubのみ |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-4247"></a>

### 1. Qilin Ransomware Attackers Exploit PAN-OS Authentication Bypass for Initial Access

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 56.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 77.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Palo Alto NetworksのPAN-OSおよびPrisma Accessに影響する認証バイパス脆弱性CVE-2026-0257が、GlobalProtect経由の初期侵入に悪用されたと報告されています。
公開情報では、Qilinランサムウェア関連の攻撃者がこの脆弱性を利用して侵入した可能性が示されており、複数環境で不審なVPN認証の痕跡が確認されています。
境界に面したVPN機器の認証回避は、外部からの侵入を直接許すため影響が大きく、ランサムウェアの侵入口として使われると被害が広がりやすくなります。
対象製品を運用している組織では、該当設定の有無と修正済み版への更新状況を早急に確認する必要があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 9 sources。
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

- PAN-OS / Prisma Accessで該当バージョンかつGlobalProtectの認証オーバーライド機能を使っているか確認する。
- ベンダーの修正版への更新を優先し、必要に応じて認証オーバーライド機能の無効化や証明書の見直しを行う。
- GlobalProtectの認証ログやVPN関連の不審な成功・失敗、想定外の認証痕跡を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-0257 | 関連CVE | 1.00 | 候補あり（URL 8件以上） |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Palo Alto | 言及あり | 0.80 | — |
| ランサムウェアグループ | Qilin | 主題 | 0.80 | — |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Arctic Wolf | 言及あり | 0.80 | — |
| 製品 | Palo Alto Networks PAN-OS | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-0257](https://nvd.nist.gov/vuln/detail/CVE-2026-0257) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Qilin Ransomware Attackers Exploit PAN-OS Authentication Bypass for Initial Acce](https://thehackernews.com/2026/07/qilin-ransomware-attackers-exploit-pan.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Palo Alto Warns of Active Exploitation of PAN-OS GlobalProtect VPN Flaw](https://thehackernews.com/2026/06/palo-alto-warns-of-active-exploitation.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: Active Exploitation of PAN-OS CVE-2026-0257](https://unit42.paloaltonetworks.com/active-exploitation-of-pan-os-cve-2026-0257/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0257 PAN-OS: GlobalProtect Authentication Bypass Vulnerabilities (Sever](https://security.paloaltonetworks.com/CVE-2026-0257) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers are exploiting Palo Alto Networks defect that initially flew under the](https://cyberscoop.com/palo-alto-networks-cve-2026-0257-exploited-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Recent Palo Alto Networks Vulnerability Exploited for Weeks](https://www.securityweek.com/recent-palo-alto-networks-vulnerability-exploited-for-weeks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers are exploiting Palo Alto GlobalProtect VPN authentication bypass (CVE-20](https://www.helpnetsecurity.com/2026/06/01/hackers-are-exploiting-palo-alto-globalprotect-vpn-authentication-bypass-cve-2026-0257/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-22364"></a>

### 2. SonicWall SMA zero-days were exploited weeks before disclosure

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 52.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

SonicWallのSecure Mobile Access（SMA）1000シリーズで、CVE-2026-15409とCVE-2026-15410がゼロデイとして悪用されていたことが報告されています。
公開後の修正だけでなく、公開前から攻撃に使われていた可能性が示されており、影響を受ける環境では更新と侵害有無の確認が求められています。
リモートアクセス用機器は社内ネットワークへの入口になりやすく、侵害されると認証情報の取得や長期潜伏につながるおそれがあります。
既に悪用が確認されているため、未適用環境の優先対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
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

- SMA 1000シリーズの対象バージョンを確認し、修正版への更新を優先する。
- 侵害の兆候がないか、認証情報・設定変更・不審な通信の有無を点検する。
- メーカーが示す注意喚起や対処方針に従い、必要に応じてパスワードやTOTPの見直しを行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-15409 | 関連CVE | 1.00 | 候補あり（URL 4件以上） |
| 脆弱性 | CVE-2026-15410 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | SonicWall | 言及あり | 0.80 | — |
| 製品 | SonicWall SMA | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-15409](https://nvd.nist.gov/vuln/detail/CVE-2026-15409) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [SonicWall SMA zero-days were exploited weeks before disclosure](https://www.helpnetsecurity.com/2026/07/21/sonicwall-sma-zero-days-exploited-cve-2026-15409-cve-2026-15410/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall Zero-Days Exploited to Deliver Custom Malware for Weeks Before Patch](https://www.securityweek.com/sonicwall-zero-days-exploited-to-deliver-custom-malware-for-weeks-before-patch/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Rapid7 MDR Team Discovers New SonicWall SMA1000 Zero Days being Actively Exploit](https://www.rapid7.com/blog/post/etr-rapid7-mdr-team-discovers-new-sonicwall-sma1000-zero-days-being-actively-exploited-cve-2026-15409-cve-2026-15410) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Two SonicWall SMA 1000 Zero-Days Exploited, One Could Enable Admin Commands](https://thehackernews.com/2026/07/two-sonicwall-sma-1000-zero-days.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall Issues Urgent SMA Patch Warning for Two Zero-Day Exploits](https://www.securityweek.com/sonicwall-issues-urgent-sma-patch-warning-for-two-zero-day-exploits/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall warns of SMA1000 flaws exploited in zero-day attacks, patch now](https://www.bleepingcomputer.com/news/security/sonicwall-warns-of-sma1000-flaws-exploited-in-zero-day-attacks-patch-now/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall SMA appliances targeted in zero-day attacks (CVE-2026-15409, CVE-2026-](https://www.helpnetsecurity.com/2026/07/14/sonicwall-sma-attacks-via-cve-2026-15409-cve-2026-15410/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-23517"></a>

### 3. CISA Adds Four Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、実際の悪用が確認されたとして、KEVカタログに4件の脆弱性を追加しました。
対象にはDD-WRT、Langflow、WordPress Coreに関する脆弱性が含まれています。
KEVカタログへの追加は、当該脆弱性が現実の攻撃で使われていることを示すため、優先的な対応が必要になります。
公開資産や広く使われる製品が含まれる場合、影響範囲が大きくなりやすい点も注目されます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象製品の利用有無を確認し、該当バージョンの棚卸しを行う。
- 公開資産を優先して、修正パッチや緩和策の適用状況を早急に点検する。
- 脆弱性の有無だけでなく、侵害兆候の確認とログの遡及確認を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2021-27137 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-0770 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-60137 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-63030 | 関連CVE | 1.00 | 候補あり（URL 22件以上） |
| 製品 | WordPress | 言及あり | 0.80 | — |
| 製品 | Langflow | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Four Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/07/21/cisa-adds-four-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-15753"></a>

### 4. Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN Validator Authenticated Privilege Escalation Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Catalyst SD-WAN Controller / Manager / Validator に、認証済みのローカル攻撃者が権限昇格できる脆弱性（CVE-2026-20245）が公表されました。
公開情報では、少なくとも一部で悪用が観測されており、影響製品では不正な高権限操作につながる可能性があるとされています。
SD-WAN はネットワーク制御の中核に当たるため、権限昇格が起きると管理基盤への影響が大きくなり得ます。
さらに、悪用観測がある一方で対策状況は製品や時点により差があるため、運用側の確認が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Cisco の案内に沿って、該当製品・該当バージョンの影響有無と修正状況を確認する。
- 管理者権限を持つアカウントの棚卸し、認証情報の見直し、多要素認証の適用状況を確認する。
- SD-WAN 管理系システムの監査ログを点検し、不審な権限変更や想定外のアカウント作成がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20127 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-20182 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-20245 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-33017 | 関連CVE | 1.00 | 候補あり（URL 8件以上） |
| 脆弱性 | CVE-2026-34908 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-34909 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34910 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-41947 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-41948 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-55255 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20245](https://nvd.nist.gov/vuln/detail/CVE-2026-20245) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN V](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-privesc-4uxFrdzx) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [22nd June – Threat Intelligence Report](https://research.checkpoint.com/2026/22nd-june-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [29th June – Threat Intelligence Report](https://research.checkpoint.com/2026/29th-june-threat-intelligence-report-2/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco SD-WAN Zero-Day Exploited Months Before Patching](https://www.securityweek.com/cisco-sd-wan-zero-day-exploited-months-before-patching/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Zero-Day CVE-2026-20245 Exploited to Gain Root Access](https://thehackernews.com/2026/06/cisco-catalyst-sd-wan-zero-day-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Mandiant reveals how Cisco SD-WAN zero-day attacks gained root access](https://www.bleepingcomputer.com/news/security/mandiant-reveals-how-cisco-sd-wan-zero-day-attacks-gained-root-access/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zero-Day Exploitation of Vulnerability (CVE-2026-20245) in Cisco Catalyst SD-WAN](https://cloud.google.com/blog/topics/threat-intelligence/zero-day-exploitation-cisco-catalyst-sd-wan-manager/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-23487"></a>

### 5. JadePuffer returns with ransomware built to target AI models and infrastructure

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

報道によると、JadePufferと呼ばれる脅威アクターが、AIモデルや機械学習基盤を標的にした新たなランサムウェア「ENCFORGE」を使おうとしているとされています。
以前に確認されたAIエージェント主導の恐喝活動と、今回のランサムウェアに埋め込まれた連絡先情報が一致するとされ、同一の関与が示唆されています。
AI基盤を狙うランサムウェアは、モデルや学習・推論環境、関連データの可用性に直接影響しうるため注目されています。
従来のIT資産だけでなく、AI運用基盤を含めた保護と復旧計画の見直しが必要になる可能性があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI/ML基盤に含まれる重要資産を棚卸しし、バックアップと復旧手順を通常の業務システムと分けて確認する。
- モデル、学習データ、推論環境、シークレット管理の権限を最小化し、不要な公開経路がないか点検する。
- ランサムウェアを想定した監視を、サーバーだけでなくコンテナ、オーケストレーション、MLOps基盤にも広げる。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [JadePuffer returns with ransomware built to target AI models and infrastructure](https://www.helpnetsecurity.com/2026/07/21/jadepuffer-encforge-ransomware/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23291"></a>

### 6. Exploitation of ServiceNow Vulnerability Seen Days After Disclosure

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>A⁠I</nobr> / <nobr>サ⁠プ⁠ラ⁠イ⁠チ⁠ェ⁠ー⁠ン</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

ServiceNow AI Platformに関する脆弱性CVE-2026-6875について、公開後まもなく実際の悪用が観測されたと複数の報道で伝えられています。
説明されている内容では、認証前にコード実行につながる可能性がある重大な脆弱性とされており、対象環境では注意が必要です。
認証なしで悪用される可能性がある脆弱性は、影響範囲が広く、侵害までの時間も短くなりやすい点が警戒されています。
ServiceNowは業務基盤として使われることが多いため、仮に影響を受けると運用や情報管理への波及が大きくなり得ます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ServiceNow AI Platformの該当バージョンや影響範囲を確認し、ベンダーの修正情報と回避策を優先して適用する。
- 外部公開されたServiceNowインスタンスについて、想定外の挙動や不審なコード実行の兆候がないか監視を強化する。
- 関連する認証情報や管理者権限の見直しを行い、侵害の可能性がある場合はログ保全と影響調査を急ぐ。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-6875 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-6875](https://nvd.nist.gov/vuln/detail/CVE-2026-6875) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Exploitation of ServiceNow Vulnerability Seen Days After Disclosure](https://www.securityweek.com/exploitation-of-servicenow-vulnerability-seen-days-after-disclosure/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ServiceNow pre-auth RCE exploited in the wild (CVE-2026-6875)](https://www.helpnetsecurity.com/2026/07/20/servicenow-cve-2026-6875-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco’s open-weight Antares models make vulnerability localization cheaper](https://www.helpnetsecurity.com/2026/07/21/cisco-antares-vulnerability-localization-released/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Open-source maintainers still work underfunded as sponsorship crosses $100 milli](https://www.helpnetsecurity.com/2026/07/21/open-source-github-sponsors-100-million/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23469"></a>

### 7. Pwn2Own Ireland 2026 – New Targets and Categories

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>A⁠I</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>i⁠O⁠S</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Pwn2Own Ireland 2026では、Corkでの開催に向けて新たな対象カテゴリとルールが公表されました。
今回はモバイル端末、スマートホーム、ウェルネス機器、プリンター、メッセージングに加え、AIインフラとAIコーディングエージェントが対象に含まれています。
AI関連の攻撃面が競技対象として明示されており、実運用で使われるAIインフラや開発支援ツールの脆弱性に注目が集まります。
公開競技での検証結果は、今後の製品改善や防御優先度の見直しにつながる可能性があります。

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

- AIインフラとAIコーディングエージェントは、従来のOSやアプリだけでなく新しい攻撃面として継続的に確認する。
- メッセージングやモバイルは、日常利用の機能がそのまま侵入経路になり得るため、更新適用状況と外部入力の扱いを再点検する。
- スマートホームやウェルネス機器は、ネットワーク越しに触れられる機能の棚卸しと、不要な公開機能の抑制が重要。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脅威アクター | PLATINUM | 主題 | 0.80 | — |
| ベンダー | Trend Micro | 言及あり | 0.80 | — |
| ベンダー | Apple | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Pwn2Own Ireland 2026 – New Targets and Categories](https://www.thezdi.com/blog/2026/7/21/pwn2own-ireland-2026-new-targets-and-categories) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-23164"></a>

### 1. WordPress wp2shell Exploitation Grows as Public Exploit Fuels Mass Scanning

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>A⁠I</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

WordPress Core の脆弱性 CVE-2026-63030（wp2shell）について、複数のセキュリティ情報で悪用の動きや公開PoCの存在が示されています。
影響を受ける可能性のある WordPress では、認証なしでコード実行につながるとされており、修正版への更新が案内されています。
WordPress は広く利用されているため、公開系サイトへの影響が大きくなりやすい点が注目されています。
公開PoCやスキャン増加の संकेतがあることで、未修正環境が狙われるリスクが高まります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 公開PoC・検証コード言及あり。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- WordPress を 6.9.5、7.0.2 などの修正版へ早急に更新し、対象ブランチを確認する。
- 公開されている WordPress サイトで不審な改ざんや見慣れないプラグイン追加、Web シェルの痕跡を点検する。
- 自動更新の適用状況を確認し、外部公開インスタンスの棚卸しを優先する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-60137 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-63030 | 関連CVE | 1.00 | 候補あり（URL 22件以上） |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| 製品 | WordPress | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-63030](https://nvd.nist.gov/vuln/detail/CVE-2026-63030) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Critical wp2shell WordPress flaws exploited to install webshells](https://www.bleepingcomputer.com/news/security/critical-wp2shell-wordpress-flaws-exploited-to-install-webshells/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [WordPress wp2shell Exploitation Grows as Public Exploit Fuels Mass Scanning](https://thehackernews.com/2026/07/wordpress-wp2shell-exploitation-grows.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [WordPress Exploitation Underway (CVE-2026-63030), (Mon, Jul 20th)](https://isc.sans.edu/diary/rss/33168) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Exploitation in the Wild of wp2shell](https://www.wiz.io/blog/wp2shell-cve-2026-63030-cve-2026-60137) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-63030: wp2shell a Critical Remote Code Execution Vulnerability in WordP](https://www.rapid7.com/blog/post/etr-cve-2026-63030-wp2shell-a-critical-remote-code-execution-vulnerability-in-wordpress-core) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 採用あり（1件）。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Estée Lauder、Oracle EBSのゼロデイ攻撃による影響を公表](https://www.securityweek.com/estee-lauder-discloses-impact-from-oracle-ebs-zero-day-hack/) | 37.0 | 38.0 | 43.0 |
| [WindowsのLegacyHiveゼロデイ脆弱性に非公式の無償パッチ公開](https://www.bleepingcomputer.com/news/security/windows-legacyhive-zero-day-flaw-gets-free-unofficial-patches/) | 37.0 | 38.0 | 43.0 |
| [毎週新たなランサムウェア脅威アクターが出現していると報告書が警告](https://www.infosecurity-magazine.com/news/new-ransomware-weekly/) | 36.0 | 30.0 | 42.0 |
| [サイバー攻撃17％増 生成AIプロンプト「26件に1件」が高リスク](https://www.itmedia.co.jp/enterprise/articles/2607/20/news007.html) | 34.0 | 30.0 | 42.0 |
| [重大なSharePointのRCE脆弱性CVE-2026-50522が公開PoC後に悪用拡大](https://thehackernews.com/2026/07/critical-sharepoint-rce-cve-2026-50522.html) | 33.0 | 56.0 | 52.0 |
| [Qilinランサムウェア攻撃グループが悪用するPalo Alto VPNの重大な脆弱性](https://www.bleepingcomputer.com/news/security/critical-globalprotect-vpn-bug-now-exploited-in-ransomware-attacks/) | 32.0 | 48.0 | 42.0 |
| [委託先の就職試験対策サイトがランサムウェア被害 - 福岡大](https://www.security-next.com/187122) | 30.0 | 30.0 | 42.0 |
| [Captive Portal Detectionの検出方法](https://isc.sans.edu/diary/rss/33172) | 30.0 | 20.0 | 42.0 |
| [AnubisランサムウェアがCoca-Cola Fairlifeへの攻撃を主張し、データ流出を予告](https://www.bleepingcomputer.com/news/security/anubis-ransomware-claims-coca-cola-fairlife-attack-threatens-data-leak/) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア被害者、被害の原因となった脆弱性を修正せず](https://www.cybersecuritydive.com/news/ransomware-lingering-weaknesses-black-kite/825791/) | 28.0 | 30.0 | 42.0 |
| [HollowGraphマルウェアがMicrosoft 365 CalendarをC&C通信に悪用](https://www.securityweek.com/new-hollowgraph-malware-abuses-microsoft-365-calendar-for-cc-communication/) | 28.0 | 20.0 | 42.0 |
| [偽CAPTCHAを悪用してユーザーに自分で攻撃させる手口に警戒呼びかけ](https://www.bitdefender.com/en-us/blog/hotforsecurity/ukraine-fake-captchas-hack-yourself) | 28.0 | 20.0 | 42.0 |
| [北朝鮮の「ClickFake」キャンペーン、Web3関係者を標的にする](https://www.infosecurity-magazine.com/news/north-korean-clickfake-campaign/) | 28.0 | 20.0 | 42.0 |
| [大規模AIプロジェクトで「高性能な計画役＋安価な実行役」を使うとコストが約8分の1になったとCursorが報告](https://gigazine.net/news/20260721-agent-swarm-model-economics/) | 27.0 | 20.0 | 42.0 |
| [HackerがAIの脱獄を攻撃用プラットフォームへ転用](https://www.darkreading.com/cyber-risk/hacker-ai-jailbreaks-offensive-attack-platform) | 25.0 | 20.0 | 42.0 |
| [トランプ政権のAI規制に対する方針はどこにあるのか](https://cyberscoop.com/trump-admin-ai-safety-cybersecurity-export-controls/) | 25.0 | 20.0 | 42.0 |
| [Cisco、ソースコード保護向けの低コストAIモデルを発表](https://www.securityweek.com/cisco-launches-low-cost-ai-models-for-source-code-security/) | 25.0 | 20.0 | 42.0 |
| [下院情報委員会法案に州・地方の脅威インテリジェンス、選挙セキュリティ、AIに関する規定を盛り込む](https://cyberscoop.com/house-intel-bill-includes-provisions-on-state-and-local-threat-intelligence-election-security-ai/) | 25.0 | 20.0 | 42.0 |
| [Google、Gemini 3.5 Flash Cyber AIを発表しソフトウェア脆弱性の発見・修正を支援](https://thehackernews.com/2026/07/google-launches-gemini-35-flash-cyber.html) | 25.0 | 20.0 | 42.0 |
| [AIエージェントが悪意あるGitHubリポジトリを推奨するよう誘導される問題](https://www.helpnetsecurity.com/2026/07/21/github-repos-malware-campaign-fakegit-ai-agents/) | 25.0 | 20.0 | 42.0 |
| [Teleport、Identity Securityプラットフォームに新たなAIエージェント行動制御を追加](https://www.helpnetsecurity.com/2026/07/21/teleport-identity-security-platform-expanded/) | 25.0 | 20.0 | 42.0 |
| [ロシア人ハッカーが脱獄したClaudeをペンテストプラットフォーム化](https://www.infosecurity-magazine.com/news/trim-jailbroken-claude-ai-pentest/) | 25.0 | 20.0 | 42.0 |
| [AI音楽プラットフォームSunoで5,500万人のユーザー情報が漏えいか、セキュリティ専門家が指摘](https://www.theregister.com/security/2026/07/21/breach-of-ai-music-platform-suno-affected-55m-user-accounts/5275514) | 25.0 | 20.0 | 42.0 |
| [Druva、AIワークロードにバックアップ、リカバリ、ガバナンスを提供](https://www.helpnetsecurity.com/2026/07/21/druva-brings-backup-recovery-and-governance-to-ai-workloads/) | 25.0 | 20.0 | 42.0 |
| [マイナ AIエージェントと連携へ](https://news.yahoo.co.jp/pickup/6588823?source=rss) | 25.0 | 20.0 | 42.0 |
| [AI生成コードのリスクは選び方で大きく変わる](https://www.darkreading.com/application-security/choose-wisely-ai-generated-coding-risk-varies) | 25.0 | 20.0 | 42.0 |
| [300 WINtegrationsが強力：AIの速度に対応するために構築されたオープンなセキュリティエコシステム](https://www.wiz.io/blog/wiz-integration-network-reaches-300) | 25.0 | 20.0 | 42.0 |
| [オープンソースのAndroid AIエージェントで、画面に見えない文字からホストPC上でコードが実行される可能性](https://thehackernews.com/2026/07/open-source-android-ai-agents-could-let.html) | 25.0 | 20.0 | 42.0 |
| [Rockwell Automation Studio 5000 Logix Designer の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-202-10) | 24.0 | 46.0 | 50.0 |
| [Tycon Systems TPDIN-Monitor-WEB2の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-202-01) | 24.0 | 46.0 | 50.0 |
| [AWS Kiroの脆弱性、改ざんされたWebページで設定を書き換えコード実行を可能にした](https://thehackernews.com/2026/07/aws-kiro-flaw-let-poisoned-web-page.html) | 24.0 | 38.0 | 42.0 |
| [ZimbraがSNMPコマンドインジェクションと4件のXSS脆弱性を修正](https://thehackernews.com/2026/07/zimbra-patches-critical-snmp-command.html) | 24.0 | 38.0 | 42.0 |
| [Zimbraの更新で致命的な脆弱性を修正](https://www.securityweek.com/zimbra-update-patches-critical-vulnerabilities/) | 24.0 | 38.0 | 42.0 |
| [Adobe、アドバイザリ12件で脆弱性89件に対応](https://www.security-next.com/187649) | 22.0 | 20.0 | 42.0 |
| [無料で使えるCloudflare Accessの「サービス認証」を設定して外出先のアプリから自宅のローカルAIにアクセスしてみた](https://gigazine.net/news/20260721-cloudflare-service-token/) | 22.0 | 20.0 | 42.0 |
| [児童発達支援センターで個人情報含む文書を誤廃棄 - 古河市](https://www.security-next.com/187220) | 22.0 | 20.0 | 42.0 |
| [個人情報を誤提供、システムの改修テストで - 農林中金](https://www.security-next.com/187071) | 22.0 | 20.0 | 42.0 |
| [Rockwell Automation 1734 POINT I/Oの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-202-09) | 20.0 | 28.0 | 50.0 |
| [Rockwell Automation 1718-AENTR/1719-AENTRの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-202-08) | 20.0 | 28.0 | 50.0 |
| [Rockwell Automation FactoryTalk Services Platformの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-202-07) | 20.0 | 28.0 | 50.0 |
| [北朝鮮のITワーカーによる資金調達がロシアの戦争努力を支援](https://cyberscoop.com/north-korea-it-worker-scheme-funds-russia-war-ukraine/) | 20.0 | 20.0 | 48.0 |
| [ワールドカップが教えるサイバーセキュリティのレジリエンス](https://cyberscoop.com/world-cup-2026-major-event-cybersecurity-resilience-op-ed/) | 20.0 | 20.0 | 48.0 |
| [Trump政権、重要サプライチェーン全体のソフトウェアと供給元の把握を防衛請負業者に命令](https://www.securityweek.com/trump-orders-defense-contractors-to-map-software-suppliers-across-critical-supply-chains/) | 20.0 | 20.0 | 42.0 |
| [KratosのPhishing-as-a-Serviceキット、国際法執行機関との攻防に敗れる](https://www.theregister.com/security/2026/07/21/german-authorities-lead-takedown-of-kratos-phishing-platform/5275666) | 20.0 | 20.0 | 42.0 |
| [wp2shellで改ざんされたWordPressサイトを訪問すると何が起こるか](https://www.malwarebytes.com/blog/bugs/2026/07/what-happens-if-you-visit-a-wordpress-site-hacked-through-wp2shell) | 20.0 | 20.0 | 42.0 |
| [重要インフラセキュリティにおけるアイデンティティのギャップを埋める](https://www.bleepingcomputer.com/news/security/closing-the-identity-gaps-in-critical-infrastructure-security/) | 20.0 | 20.0 | 42.0 |
| [新たな恐喝の組み合わせ：オフィスプリンター、小額の身代金、BitLocker](https://securelist.com/new-extortion-scheme-printers-bitlocker/120718/) | 20.0 | 20.0 | 42.0 |
| [イラン紛争をめぐるサイバー脅威の全体像：年央評価と注目点](https://www.sentinelone.com/labs/iran-war-cyber-threat-landscape-a-midyear-assessment-on-what-matters/) | 20.0 | 20.0 | 42.0 |
| [Ciscoがサイバー分野向け小規模言語モデル2種「Antares-350M」「Antares-1B」を発表、コードベース分析を強化し大規模モデルの一部コストで動作](https://www.itpro.com/security/cisco-just-launched-two-cyber-focused-small-language-models-antares-350m-and-antares-1b-aim-to-supercharge-codebase-analysis-and-they-run-at-a-fraction-of-the-compute-expense-of-popular-frontier-models) | 20.0 | 20.0 | 42.0 |
| [Empirical SecurityがシリーズAで2500万ドルを調達](https://www.securityweek.com/empirical-security-raises-25-million-in-series-a-funding/) | 20.0 | 20.0 | 42.0 |
| [SecurityWeek、産業サイバーセキュリティの優秀性を称えるCritical Impact Awardsを創設](https://www.securityweek.com/securityweek-launches-critical-impact-awards-to-recognize-excellence-in-industrial-cybersecurity/) | 20.0 | 20.0 | 42.0 |
| [FBI、IC3幹部をかたるDeepfake動画に警告](https://www.infosecurity-magazine.com/news/fbi-deepfake-videos-ic3/) | 20.0 | 20.0 | 42.0 |
| [New ClickLock Stealer、パスワードを渡すまでMacをロックする新たな手口](https://www.malwarebytes.com/blog/news/2026/07/new-clicklock-stealer-locks-your-mac-until-you-hand-over-your-password) | 20.0 | 20.0 | 42.0 |
| [N-dayはN時間化している。パッチ適用を速めても防げない。](https://thehackernews.com/2026/07/n-day-is-becoming-n-hour-patching.html) | 20.0 | 20.0 | 42.0 |
| [DMの「FBI捜査官」を信用するな](https://www.malwarebytes.com/blog/news/2026/07/dont-trust-that-fbi-agent-in-your-dms) | 20.0 | 20.0 | 42.0 |
| [CISO対談: Andreas Gaetje ― 経済学からKörber AGのCISOへ](https://www.securityweek.com/ciso-conversations-andreas-gaetje-from-economics-to-ciso-at-korber-ag/) | 20.0 | 20.0 | 42.0 |
| [新たなBit2Watt攻撃でクラウド利用者が脆弱性を使わずに電力網を妨害できる可能性](https://thehackernews.com/2026/07/new-bit2watt-attack-could-let-cloud.html) | 20.0 | 20.0 | 42.0 |
| [FIFAワールドカップの海賊版対策で米国が1,000件超のWebサイトを押収](https://www.bleepingcomputer.com/news/security/us-seizes-over-1-000-fifa-world-cup-illegal-streaming-domains/) | 20.0 | 20.0 | 42.0 |
| [Shufti、Glocal Platformで国境を越えたコンプライアンスを簡素化](https://www.helpnetsecurity.com/2026/07/21/shufti-simplifies-cross-border-compliance-with-the-glocal-platform/) | 20.0 | 20.0 | 42.0 |
| [すでに詐欺被害に遭った人を狙う偽FBI捜査官](https://www.helpnetsecurity.com/2026/07/21/fbi-ic3-impersonation-scam-warning/) | 20.0 | 20.0 | 42.0 |
| [Meta、顧客サポートデータを露出する脆弱性に7万8000ドルの報奨金を支払う](https://www.securityweek.com/meta-pays-78000-bounty-for-vulnerability-exposing-customer-support-data/) | 20.0 | 20.0 | 42.0 |
| [米国の病院向け財務ソフトウェア提供企業Craneware、データ窃取を報告](https://www.infosecurity-magazine.com/news/craneware-reports-data-theft/) | 20.0 | 20.0 | 42.0 |
| [Clover Health Investments、データ侵害を公表](https://www.securityweek.com/clover-health-investments-discloses-data-breach/) | 20.0 | 20.0 | 42.0 |
| [AWS、GuardDutyで脅威調査の初動を自動化へ](https://www.helpnetsecurity.com/2026/07/21/amazon-guardduty-investigation-agent-on-demand/) | 20.0 | 20.0 | 42.0 |
| [Estée Lauder、Oracle EBSの脆弱性に関連したデータ侵害を公表](https://www.helpnetsecurity.com/2026/07/21/estee-lauder-data-breach-oracle-ebs/) | 20.0 | 20.0 | 42.0 |
| [Project CAV3RNの新モジュール、OutlookのカレンダーイベントをC2に悪用しDNS AAAAレコードで設定を復元](https://securelist.com/project-cav3rn-cyberespionage-framework-using-outlook-and-dns/120757/) | 20.0 | 20.0 | 42.0 |

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
