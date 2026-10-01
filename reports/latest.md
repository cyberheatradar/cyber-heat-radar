# 📡 サイレーダー 2026-10-02 05:00 JST

このレポートは、2026-10-01 17:00 JST〜2026-10-02 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 106
- [音声で扱う想定のトピック](#audio-topics): 9
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 73

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2023-46604: CISA KEV catalog addition](#topic-35470) | 57.0 | 74.0 | 51.0 | 音声 | 温度感上位枠 |
| 2 | [New Cisco SD-WAN zero-day exploited in-the-wild (CVE-2026-76504)](#topic-35199) | 55.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [Zimbra Vulnerability Exploited in the Wild Prior to Public Disclosure](#topic-28581) | 45.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 4 | [Warlock Ransomware Hits Large Spanish, Portuguese Orgs](#topic-35456) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Hallucinating Credibility: China-Aligned TA419 Impersonates its Way into US AI Policy Circles](#topic-35509) | 33.0 | 45.0 | 42.0 | 音声 | AI×Security枠 |
| 6 | [Researchers find Chinese hacking campaigns targeting AI firms, Asian governments](#topic-35415) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [OpenAI Disrupts Reasoning Extraction Campaign Linked to Moonshot AI Associates](#topic-35493) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 8 | [事務用NASがランサム被害、通常業務は再開 - 佐賀大](#topic-35443) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 9 | [Threat Coverage Digest: New Malware Reports and 1,100+ Detection Rules](#topic-35450) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-35470"></a>

### 1. CVE-2023-46604: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 57.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

CISAは、CVE-2023-46604をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
関連するArmatura Oneでは、埋め込みのApache ActiveMQに起因する脆弱性により、認証前に任意のオブジェクトのデシリアライズが起き、最悪の場合はホスト上での任意コード実行につながる可能性があるとされています。
KEV入りは、実際に悪用が確認されている脆弱性として優先対応の対象になることを意味します。
OT/制御システム分野に関わる製品である点からも、影響範囲の確認と更新の優先度が高い話題です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象バージョンのArmatura Oneを利用していないか確認し、該当する場合はベンダー修正版への更新を優先する。
- 制御系機器や関連ネットワークが外部から到達可能になっていないか見直し、不要な露出を抑える。
- CVE-2023-46604は他のApache ActiveMQ環境でも悪用文脈があるため、同種ミドルウェアを使うシステムも含めて棚卸しする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2023-46604 | 関連CVE | 1.00 | 候補あり（URL 22件以上） |
| 脆弱性 | CVE-2026-94591 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-94592 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-94593 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-94594 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2023-46604](https://nvd.nist.gov/vuln/detail/CVE-2023-46604) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Armatura LLC Armatura One](https://www.cisa.gov/news-events/ics-advisories/icsa-26-274-01) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-35199"></a>

### 2. New Cisco SD-WAN zero-day exploited in-the-wild (CVE-2026-76504)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 55.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Ciscoは、Cisco Catalyst SD-WAN Managerに存在するCVE-2026-76504について、実際の悪用を確認したと公表しました。
認証なしの遠隔攻撃者が管理者権限でAPIにアクセスできる可能性があるとされ、修正版は提供されていますが回避策は示されていません。
SD-WANの管理基盤に関わるため、影響を受けるとネットワーク運用全体に波及するおそれがあります。
すでに悪用観測があるとされているため、通常の脆弱性対応よりも早い確認と更新が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
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

- 影響を受けるCisco Catalyst SD-WAN Managerの稼働有無とバージョンを確認し、修正版の適用可否を早急に判断する。
- Ciscoが公開している侵害の痕跡や関連アドバイザリを参照し、管理画面やAPI周辺の不審なアクセス履歴を点検する。
- インターネットから到達可能な管理系インターフェースの露出を見直し、必要最小限のアクセス制御を維持する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-76504 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Catalyst SD-WAN Manager | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-76504](https://nvd.nist.gov/vuln/detail/CVE-2026-76504) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds Exploited Cisco Catalyst SD-WAN Manager Auth Bypass to KEV](https://thehackernews.com/2026/10/cisa-adds-exploited-cisco-catalyst-sd.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [New Cisco SD-WAN zero-day exploited in-the-wild (CVE-2026-76504)](https://www.helpnetsecurity.com/2026/10/01/new-cisco-sd-wan-zero-day-exploited-in-the-wild-cve-2026-76504/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Warns of Attackers Exploiting Critical Authentication Bypass in SD-WAN Man](https://thehackernews.com/2026/09/cisco-warns-of-attackers-exploiting.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Cisco Catalyst SD-WAN Manager API authentication bypass exploited in th](https://www.rapid7.com/blog/post/etr-critical-cisco-catalyst-sd-wan-manager-api-authentication-bypass-exploited-in-the-wild-cve-2026-76504) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of new SD-WAN zero-day exploited in attacks](https://www.bleepingcomputer.com/news/security/cisco-warns-of-new-sd-wan-authentication-bypass-zero-day-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Manager API Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-webauth-xr8beuuU) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/09/30/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-28581"></a>

### 3. Zimbra Vulnerability Exploited in the Wild Prior to Public Disclosure

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>サ⁠プ⁠ラ⁠イ⁠チ⁠ェ⁠ー⁠ン</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Zimbra Collaboration（ZCS）に存在するCVE-2026-73570は、公開前から実環境で悪用が観測された脆弱性として報じられています。
内容はOSコマンドインジェクションに起因するもので、条件によってはリモートコード実行につながるとされています。
メール基盤は組織内の認証情報や業務連絡に直結するため、侵害時の影響が大きくなりやすい点が注目されています。
さらに、公開前に悪用が確認されたことは、修正公開後も迅速な対応が必要であることを示しています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Zimbra Collaborationの該当バージョンが修正版に更新済みか確認し、未適用なら優先度を上げて適用する。
- インターネットに公開されたZimbraサーバーを重点的に点検し、不審な挙動や侵害痕跡の有無を確認する。
- メールサーバーは初期侵入の起点になりやすいため、関連アカウントの認証情報更新やログ監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-73570 | 関連CVE | 1.00 | 候補あり（URL 7件以上） |
| ベンダー | Zimbra | 言及あり | 0.80 | — |
| 製品 | Zimbra Collaboration | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |
| 製品 | Microsoft Azure | 言及あり | 0.80 | — |
| ベンダー | Citrix | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-73570](https://nvd.nist.gov/vuln/detail/CVE-2026-73570) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Microsoft catches hackers exploiting Zimbra bug before disclosure](https://www.theregister.com/security/2026/10/01/microsoft-catches-hackers-exploiting-zimbra-bug-before-disclosure/5300543) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zimbra Vulnerability Exploited in the Wild Prior to Public Disclosure](https://www.securityweek.com/zimbra-vulnerability-exploited-in-the-wild-prior-to-public-disclosure/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Week in review: Compromised Zimbra servers, previously patched Citrix NetScaler ](https://www.helpnetsecurity.com/2026/08/30/week-in-review-compromised-zimbra-servers-previously-patched-citrix-netscaler-flaw-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Unpatched Zimbra servers are falling to CVE-2026-73570 attacks](https://www.helpnetsecurity.com/2026/08/25/zimbra-cve-2026-73570-compromised/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Exploited Zimbra Flaw Highlights Shrinking Window to Patch](https://www.darkreading.com/vulnerabilities-threats/zimbra-flaw-exploitation-shrinking-window-patch) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/08/21/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit Zimbra SNMP Flaw for Unauthenticated Remote Code Execution](https://thehackernews.com/2026/08/attackers-exploit-zimbra-snmp-flaw-for.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35456"></a>

### 4. Warlock Ransomware Hits Large Spanish, Portuguese Orgs

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Warlockランサムウェアに関連する攻撃が、スペインとポルトガルの大規模組織に影響したと報じられています。
公開情報では、攻撃主体の詳細や背景について未確定な点もあり、現時点ではランサムウェア事案としての注意喚起が中心です。
ランサムウェアは業務停止やデータ流出につながるため、対象地域や業種にかかわらず警戒が必要です。
特に、攻撃主体の性質がはっきりしない段階でも、被害拡大を防ぐための初動対応が重要になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 重要資産のバックアップと復旧手順が実際に機能するか再確認する。
- 特権アカウントやリモート接続経路の監視・制御を強化する。
- 侵入検知、EDR、ログ保全を点検し、異常な暗号化や大量ファイル操作の兆候に備える。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Warlock Ransomware Hits Large Spanish, Portuguese Orgs](https://www.darkreading.com/cyberattacks-data-breaches/warlock-ransomware-spanish-portuguese) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35509"></a>

### 5. Hallucinating Credibility: China-Aligned TA419 Impersonates its Way into US AI Policy Circles

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>I⁠o⁠C</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>サ⁠プ⁠ラ⁠イ⁠チ⁠ェ⁠ー⁠ン</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>国⁠家⁠支⁠援</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 45.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Proofpointは、China-alignedの脅威アクターTA419が、米国のAI政策や規制に関わる専門家を狙い、経済学者やAI政策担当者になりすました認証情報窃取キャンペーンを行っていたと報告しました。
会話のきっかけとなる丁寧なメールから始め、クラウドサービスを装った偽ページへ誘導する流れが確認されています。
AI政策や規制をめぐる議論の当事者が狙われることで、機密情報やアカウントが侵害されるおそれがあります。
企業や研究機関にとっては、標的型フィッシングが技術部門だけでなく政策・渉外系の担当者にも広がっている点が重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 不審な依頼メールは、たとえ内容が業務関連に見えても送信者本人とは別経路で確認する。
- Microsoft 365 / Entra ID などの認証には、フィッシング耐性のある方式の導入を優先する。
- クラウド共有を装うリンクや不自然な短縮URLを含むメールについて、受信・認証・MFA後の挙動を含めて監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cloudflare | 言及あり | 0.80 | — |
| ベンダー | Proofpoint | 言及あり | 0.80 | — |
| ベンダー | Anthropic | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |
| 製品 | Microsoft Entra ID | 言及あり | 0.80 | — |
| 製品 | Exchange | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Hallucinating Credibility: China-Aligned TA419 Impersonates its Way into US AI P](https://www.proofpoint.com/us/blog/threat-insight/hallucinating-credibility-china-aligned-ta419-impersonates-its-way-us-ai-policy) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-35415"></a>

### 6. Researchers find Chinese hacking campaigns targeting AI firms, Asian governments

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

サイバーセキュリティ企業の報告により、中国に関連するとみられる複数の攻撃キャンペーンが確認されたとされています。
対象にはAI企業やアジアの政府機関が含まれ、西側の専門家を装ったフィッシングも報告されています。
AI関連企業と政府機関の両方が狙われている点から、技術情報と政策情報の両面で注意が必要です。攻撃手口そのものよりも、標的の選定やなりすましの傾向が今後の防御判断に影響します。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 受信メールや連絡先の真正性確認を徹底し、なりすましに対する社内周知を強化する。
- AI関連の研究・事業部門では、機密情報や認証情報の取り扱いを改めて見直す。
- 政府・公共分野や対外窓口を持つ組織は、フィッシング前提の監視とインシデント報告導線を整備する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Researchers find Chinese hacking campaigns targeting AI firms, Asian governments](https://therecord.media/china-linked-phishing-scheme-backdoor-taiwan) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35493"></a>

### 7. OpenAI Disrupts Reasoning Extraction Campaign Linked to Moonshot AI Associates

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>国⁠家⁠支⁠援</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

OpenAIは、自社のAIモデルから保護された推論情報を不正に抽出しようとする、組織的な蒸留キャンペーンを特定し、妨害したと明らかにしました。
報道によると、この活動の一部は北京拠点の中国企業Moonshot AIに関連する人物に結び付けられているとされていますが、詳細は限定的です。
生成AIの出力や推論過程を巡る保護は、モデルの知財や安全対策に直結します。
こうした事案は、AIサービス提供側だけでなく、企業が外部AIを業務利用する際の契約・利用条件・監査の重要性も示しています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 外部AIの利用条件で、出力の再学習・再利用・取得制限に関する規約を再確認する。
- 機密情報や業務ノウハウをAIに入力する際のガイドラインとログ管理を見直す。
- AIベンダーからの不正利用・保護機能に関する通知があれば、社内の利用影響を早めに評価する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | OpenAI | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [OpenAI Disrupts Reasoning Extraction Campaign Linked to Moonshot AI Associates](https://thehackernews.com/2026/10/openai-disrupts-reasoning-extraction.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35443"></a>

### 8. 事務用NASがランサム被害、通常業務は再開 - 佐賀大

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

佐賀大学は、事務用途で使っていた一部の情報システムにランサムウェア被害があったと明らかにしました。現時点では調査を継続しているものの、通常業務は再開しているとされています。
大学の事務系システムは、学内運営や各種手続きに直結するため、被害の影響が広がると業務継続に支障が出やすい分野です。
ランサムウェア被害は、バックアップや復旧手順、初動対応の重要性を改めて示しています。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 事務系NASや共有ストレージのバックアップ、復旧手順が実際に機能するか確認する。
- 業務再開後も、侵入経路の特定と関連アカウント・機器の点検を継続する。
- ファイル共有機器は更新状況や権限設定を見直し、被害拡大を防ぐ。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [事務用NASがランサム被害、通常業務は再開 - 佐賀大](https://www.security-next.com/190842) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35450"></a>

### 9. Threat Coverage Digest: New Malware Reports and 1,100+ Detection Rules

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

9月に、ネットワーク・ファイル・挙動の各面で検知カバレッジが拡張されたことが報告されました。
追加されたのは、76件の振る舞いシグネチャ、16件のYARA検知、1,098件のSuricataルールとされています。
また、LockBitやNanoCore、Vidar、XWorm、Zeusなど複数のマルウェア名が話題に含まれています。
検知ルールの拡充は、SOCやMSSPが不審活動を見つける際の手がかりを増やし、調査時の可視性向上につながります。
特定の脅威名が並ぶ一方で、個別の侵害事例を示す内容ではないため、運用面では検知強化の文脈で見るのが適切です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 新規の振る舞い検知、YARA、Suricataルールが自社の監視基盤に取り込まれているか確認する。
- 関連するマルウェア名に対する既存のアラートやログ相関が十分か見直す。
- 検知追加後は誤検知の有無と、アラートの優先度付けが実運用に合っているかを確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ランサムウェアグループ | LockBit | 主題 | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Adobe | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| マルウェア | NanoCore | 主題 | 0.80 | — |
| マルウェア | Vidar | 主題 | 0.80 | — |
| マルウェア | XWorm | 主題 | 0.80 | — |
| マルウェア | Zeus | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Threat Coverage Digest: New Malware Reports and 1,100+ Detection Rules](https://any.run/cybersecurity-blog/september-threat-coverage-2026/) | <nobr>内容確認・補足情報</nobr> |

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
| [ランサムウェア関連の法執行・司法措置](https://thehackernews.com/2026/10/police-arrest-16-year-old-suspected-of.html) | 28.0 | 30.0 | 42.0 |
| [KillSecランサムウェアを摘発、警察が10代の指導者とみられる人物を逮捕](https://therecord.media/killsec-ransomware-raas-arrests-europe) | 28.0 | 30.0 | 42.0 |
| [警察が16歳少年主導とされるKillSecランサムウェア集団を摘発](https://www.bleepingcomputer.com/news/security/police-dismantle-killsec-ransomware-gang-allegedly-led-by-16-year-old/) | 28.0 | 30.0 | 42.0 |
| [KillSecランサムウェアを警察が摘発、10代の首謀者とされる人物を特定](https://www.securityweek.com/police-shut-down-killsec-ransomware-identify-alleged-teen-leader/) | 28.0 | 30.0 | 42.0 |
| [Warlockランサムウェア攻撃者が水道・通信事業者を標的にした攻撃](https://www.security.com/threat-intelligence/warlock-ransomware-critical-infrastructure) | 28.0 | 30.0 | 42.0 |
| [Johnson Controls EasyIO NeoシリーズECおよびCWコントローラー](https://www.cisa.gov/news-events/ics-advisories/icsa-26-274-05) | 28.0 | 28.0 | 50.0 |
| [WordPressバックドアがファイル、データベース、共有メモリを使ってクリーンアップ後に自己再構築する問題](https://thehackernews.com/2026/10/wordpress-backdoor-rebuilds-itself.html) | 28.0 | 20.0 | 42.0 |
| [Malwarebytesが独立テストで再びTop Product賞を獲得](https://www.malwarebytes.com/blog/product/2026/10/malwarebytes-earns-another-top-product-award-in-independent-testing) | 28.0 | 20.0 | 42.0 |
| [米財務省、ATMマルウェア開発者とそのネットワークを制裁対象に指定](https://www.securityweek.com/treasury-blacklists-most-wanted-atm-malware-developer-and-his-network/) | 28.0 | 20.0 | 42.0 |
| [ThreatsDay: AI搭載のゼロデイ連鎖、54.3万件の生存シークレット、Model InspectionのRCEなど13件の注目トピック](https://thehackernews.com/2026/10/threatsday-ai-powered-zero-day-chain.html) | 27.0 | 20.0 | 43.0 |
| [AIエージェントがZammadのゼロデイを悪用しオランダの脆弱性開示非営利団体に侵入](https://www.helpnetsecurity.com/2026/10/01/divd-agentic-ai-attack-breach/) | 27.0 | 20.0 | 43.0 |
| [Zammadのゼロデイ脆弱性を悪用したAI搭載DIVDへの侵害](https://www.securityweek.com/zammad-zero-days-exploited-in-ai-powered-divd-hack/) | 27.0 | 20.0 | 43.0 |
| [OpenAIはテストの監視が不十分であるという社内警告を繰り返し無視して追加のセキュリティ対策をせず迅速なリリースを優先していた](https://gigazine.net/news/20261001-openai-ignored-warnings/) | 27.0 | 20.0 | 42.0 |
| [ハードウェアに合わせて自動最適化してオープンモデルを最大2倍高速化するAIエージェント向け推論エンジン「Magnitude」、Appleシリコン・NVIDIA・AMD・CPUに対応](https://gigazine.net/news/20261001-magnitude/) | 27.0 | 20.0 | 42.0 |
| [パナソニックCAIOが語る人とAIがともに進化する組織づくり--「AIトランスフォーメーション」の取り組み](https://japan.zdnet.com/article/35253160/) | 26.0 | 20.0 | 42.0 |
| [国家サイバー担当官：AIリスクと各国との競争管理に向けた官民連携の重要性](https://cyberscoop.com/sean-cairncross-ai-security-china-industry-collaboration/) | 25.0 | 20.0 | 42.0 |
| [Zero Trustの提唱者、AI支援攻撃に対してもモデルは堅固と主張](https://www.securityweek.com/zero-trust-creator-says-model-holds-firm-against-ai-assisted-attacks/) | 25.0 | 20.0 | 42.0 |
| [中国系スパイがAnthropic幹部や元ホワイトハウス高官を装ったAIフィッシング攻撃](https://www.theregister.com/security/2026/10/01/suspected-chinese-spies-spoofed-an-anthropic-exec-ex-white-house-official-in-ai-phishing/5300595) | 25.0 | 20.0 | 42.0 |
| [SOC担当者はAIの影響に概ね満足も、懸念は残る](https://www.cybersecuritydive.com/news/ai-security-operations-centers-careers-skills-swimlane/831882/) | 25.0 | 20.0 | 42.0 |
| [企業はAIと量子の脅威への備えに苦戦、PwCが指摘](https://www.securityweek.com/enterprises-struggle-to-prepare-for-ai-and-quantum-threats-pwc-says/) | 25.0 | 20.0 | 42.0 |
| [中国関連のフィッシング攻撃で標的にされたAI政策関係者](https://cyberscoop.com/china-cyber-espionage-ta419-phishing-us-ai-policy-experts/) | 25.0 | 20.0 | 42.0 |
| [Shadow AIとは何か：業務効率化の近道が企業秘密を漏えいさせる可能性](https://www.malwarebytes.com/blog/ai/2026/10/shadow-ai-explained-the-work-shortcut-that-could-leak-your-companys-secrets) | 25.0 | 20.0 | 42.0 |
| [中国関連のハッカーがAI専門家を装い米国の政策関係者を標的にした攻撃](https://www.infosecurity-magazine.com/news/ta419-impersonates-ai-experts-us/) | 25.0 | 20.0 | 42.0 |
| [DeepKeepのAI Lens、コーディングエージェントのデータ漏えいと破壊的コマンドを検知し承認へ回す](https://www.helpnetsecurity.com/2026/10/01/deepkeeps-ai-lens-flags-coding-agent-data-leaks-and-routes-destructive-commands-for-approval/) | 25.0 | 20.0 | 42.0 |
| [Exabeam、オンプレミス環境に残す必要があるデータ向けのAI支援セキュリティ調査を提供](https://www.helpnetsecurity.com/2026/10/01/exabeam-agentic-soc/) | 25.0 | 20.0 | 42.0 |
| [RadarFirstが支援するAIの偏り、データ漏えい、意図しない動作の調査](https://www.helpnetsecurity.com/2026/10/01/radarfirst-ai-incident-management/) | 25.0 | 20.0 | 42.0 |
| [Sophosがエージェント型AIで示す、企業が優先投資すべきセキュリティ修正項目](https://www.helpnetsecurity.com/2026/10/01/sophos-ciso-advantage/) | 25.0 | 20.0 | 42.0 |
| [AIが変えたのは攻撃速度であり、セキュリティの基本ではない](https://www.securityweek.com/ai-has-changed-attack-speed-not-security-fundamentals/) | 25.0 | 20.0 | 42.0 |
| [Legit Securityが脆弱なオープンソース依存関係への自動修正を拡張](https://www.helpnetsecurity.com/2026/10/01/legit-security-agentic-remediation-expansion/) | 25.0 | 20.0 | 42.0 |
| [1年後：Sovereign AIと選択のための戦い](https://blog.cloudflare.com/sovereign-ai-choice-one-year-later/) | 25.0 | 20.0 | 42.0 |
| [AIが変えるセキュリティオペレーションセンターに必要な役割](https://www.rapid7.com/blog/post/ai-changing-security-operations-center-roles-soc) | 25.0 | 20.0 | 42.0 |
| [Kevin Mandia氏のArmadin、25億ドル評価で2億5500万ドルを調達](https://www.securityweek.com/kevin-mandias-armadin-raises-255-million-at-2-5-billion-valuation/) | 25.0 | 20.0 | 42.0 |
| [脆弱性公開は急増しているが、AIが発見される欠陥の種類を変えている](https://www.itpro.com/security/hacking/vulnerability-disclosures-are-rocketing-but-ai-is-changing-the-types-of-flaw-being-discovered) | 25.0 | 20.0 | 42.0 |
| [ArmadinがAI攻撃的セキュリティプラットフォーム拡大のため2億5550万ドルを調達](https://www.helpnetsecurity.com/2026/10/01/armadin-raises-255-5-million-funding/) | 25.0 | 20.0 | 42.0 |
| [PwC調査で明らかになった、AI脅威へのサイバーセキュリティ準備不足](https://www.infosecurity-magazine.com/news/mitigating-adversarial-ai-top/) | 25.0 | 20.0 | 42.0 |
| [DraftKingsのAIによって損失を出した賭け手がさらに賭けるよう促されたと報告される](https://www.malwarebytes.com/blog/ai/2026/10/losing-gamblers-pushed-to-bet-more-by-draftkings-ai-report-says) | 25.0 | 20.0 | 42.0 |
| [CISA Malcolm関連情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-254-01) | 24.0 | 46.0 | 50.0 |
| [Monta monta.appに関する脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-274-02) | 24.0 | 46.0 | 50.0 |
| [ABB Protection and Control IED Manager PCM600の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-274-03) | 22.0 | 40.0 | 50.0 |
| [自分らしくいられる余裕を持つ](https://blog.talosintelligence.com/give-yourself-room-to-be-human/) | 22.0 | 20.0 | 48.0 |
| [相互接続されたサイバーリスクの時代に備える政府の対策](https://blogs.microsoft.com/on-the-issues/2026/10/01/preparing-governments-for-an-era-of-interconnected-cyber-risk/) | 22.0 | 20.0 | 42.0 |
| [2026年Microsoft Digital Defense Reportから得られた洞察](https://www.microsoft.com/en-us/security/blog/2026/10/01/insights-from-the-2026-microsoft-digital-defense-report/) | 22.0 | 20.0 | 42.0 |
| [Capital OneがSocketを活用してオープンソースのセキュリティを強化する方法](https://socket.dev/blog/capital-one-open-source-security) | 22.0 | 20.0 | 42.0 |
| [IIJ、SOCで正規アカウント悪用の検知を強化 - CrowdStrike ITPを活用](https://news.mynavi.jp/techplus/article/20261001-5058066/) | 21.0 | 20.0 | 42.0 |
| [申し込み画面に知らない人の名前や連絡先……チケットサイトで個人情報の誤表示 最大107人分](https://www.itmedia.co.jp/news/article/2610/01/2000001941/) | 21.0 | 20.0 | 42.0 |
| [免許証の悪用防止で申し込み集中 JICCがアプリ受付を一時休止 タイムズカー漏えいの影響か](https://www.itmedia.co.jp/news/article/2610/01/2000001943/) | 21.0 | 20.0 | 42.0 |
| [日本原子力機構に不正アクセス 研究者の顔写真付き身分証など漏えい](https://www.itmedia.co.jp/news/article/2610/01/2000001942/) | 21.0 | 20.0 | 42.0 |
| [Meari IoT Cloud PlatformのOpenAPIサービス](https://www.cisa.gov/news-events/ics-advisories/icsa-26-274-06) | 20.0 | 28.0 | 50.0 |
| [EUの寄せ集め技術政策が加盟国を中国ベンダーのリスクにさらす、シンクタンクが指摘](https://www.theregister.com/security/2026/10/01/eus-hodgepodge-tech-policy-exposes-members-to-chinese-vendor-risks-says-think-tank/5300599) | 20.0 | 20.0 | 42.0 |
| [Osavulがサイバーと物理の両領域にわたる敵対的意図を検知するために1000万ドルを調達](https://www.securityweek.com/osavul-lands-10-million-to-spot-hostile-intent-across-cyber-physical-domains/) | 20.0 | 20.0 | 42.0 |
| [偽のxStocks、Pendleなどのサイトが報酬投票を餌に暗号資産ユーザーを誘導](https://www.malwarebytes.com/blog/threat-intel/2026/10/fake-xstocks-pendle-and-other-sites-bait-crypto-users-with-rewards-votes) | 20.0 | 20.0 | 42.0 |
| [Hacker Conversations: Rob Juncker、Knock at the Door、そして道徳的コンパス](https://www.securityweek.com/hacker-conversations-rob-juncker-a-knock-at-the-door-and-a-moral-compass/) | 20.0 | 20.0 | 42.0 |
| [MI5、英国の研究者に中国スパイへの研究協力の可能性を警告](https://www.theregister.com/security/2026/10/01/mi5-warns-uk-academics-their-research-may-have-helped-chinese-spies/5300502) | 20.0 | 20.0 | 42.0 |
| [Zero Trustアーキテクチャの初期段階に潜む欠陥](https://www.bleepingcomputer.com/news/security/the-day-one-hole-in-zero-trust-architecture/) | 20.0 | 20.0 | 42.0 |
| [Kiteworksの最大深刻度コードインジェクション脆弱性を修正](https://www.bleepingcomputer.com/news/security/kiteworks-patches-max-severity-email-protection-gateway-code-injection-vulnerability/) | 20.0 | 20.0 | 42.0 |
| [CISOは「r3@lg00dp@$$w0rd」を設定したつもりだったが、パッチ適用を忘れていた](https://www.theregister.com/security/2026/10/01/ciso-thought-he-had-a-r3lg00dpw0rd-but-forgot-to-patch/5300314) | 20.0 | 20.0 | 42.0 |
| [偽のZoomインストーラーに潜むCloudSyncD macOSバックドア](https://www.infosecurity-magazine.com/news/cloudsyncd-macos-backdoor-fake/) | 20.0 | 20.0 | 42.0 |
| [Huntress Tragic Quadrant：企業に甚大な被害をもたらす上位サイバー脅威](https://www.huntress.com/blog/huntress-tragic-quadrant-cyber-threats) | 20.0 | 20.0 | 42.0 |
| [Symantec CBXの提供開始](https://www.security.com/feature-stories/symantec-cbx-here) | 20.0 | 20.0 | 42.0 |
| [大手ポーランド請求書発行プラットフォームへのサイバー攻撃で顧客データが流出](https://therecord.media/poland-cyberattack-invoice-software) | 20.0 | 20.0 | 42.0 |
| [Pentagonの侵害で300万人超の個人情報が流出](https://www.helpnetsecurity.com/2026/10/01/pentagon-dmdc-data-breach-3-million-people/) | 20.0 | 20.0 | 42.0 |
| [CISAがサイバーセキュリティ啓発月間を開始、次の250年を守るために](https://www.cisa.gov/news-events/news/cisa-launches-cybersecurity-awareness-month-securing-next-250) | 20.0 | 20.0 | 42.0 |
| [金融サービス企業がソフトウェアサプライチェーンを近代化する方法](https://thehackernews.com/2026/10/how-financial-services-companies-can.html) | 20.0 | 20.0 | 42.0 |
| [イングランドの学校でサイバーインシデント対応が改善している](https://www.theregister.com/security/2026/10/01/englands-schools-are-getting-better-at-mopping-up-cyber-incidents/5300465) | 20.0 | 20.0 | 42.0 |
| [FBIがShinyHuntersのメンバーに出頭を呼びかけ、首謀者とされる人物を逮捕](https://www.bitdefender.com/en-us/blog/hotforsecurity/fbi-shinyhunters-turn-themselves-in-arrest-leader) | 20.0 | 20.0 | 42.0 |
| [ShinyHunters容疑者を逮捕、殺人計画の疑いでも捜査対象に](https://www.bitdefender.com/en-us/blog/hotforsecurity/shinyhunters-suspect-arrested-now-investigated-alleged-murder-plots) | 20.0 | 20.0 | 42.0 |
| [国防総省の情報漏えいで数百万人の社会保障番号と軍事記録が流出](https://www.malwarebytes.com/blog/privacy/2026/10/pentagon-breach-exposes-social-security-numbers-and-military-records-of-millions) | 20.0 | 20.0 | 42.0 |
| [英国プライバシー監督機関、新理事会とマンチェスター本部で再出発](https://www.theregister.com/security/2026/10/01/uk-privacy-watchdog-starts-over-with-new-board-and-manchester-hq/5300439) | 20.0 | 20.0 | 42.0 |
| [英国の学校におけるサイバー攻撃への対応力向上](https://www.itpro.com/security/cyber-attacks/uk-schools-are-getting-better-at-dealing-with-cyber-attacks) | 20.0 | 20.0 | 42.0 |
| [一部の車載アプリが所有者のデータを大手テック企業に提供している問題](https://www.helpnetsecurity.com/2026/10/01/connected-car-apps-privacy-research/) | 20.0 | 20.0 | 42.0 |
| [3万人超の国防総省職員記録をハッカーが窃取](https://www.bleepingcomputer.com/news/security/hackers-breach-pentagon-human-resources-management-system-steal-data-of-nearly-3-million-people/) | 20.0 | 20.0 | 42.0 |
| [GitHub上で50万件の有効な認証情報が露出したままに](https://www.securityweek.com/500000-active-credentials-left-exposed-on-github/) | 20.0 | 20.0 | 42.0 |
| [英国の「オールドボーイズクラブ」化するサイバー業界で過去最少となった女性比率](https://www.theregister.com/security/2026/10/01/fewer-women-than-ever-in-uks-old-boys-club-cyber-industry/5300064) | 20.0 | 20.0 | 42.0 |

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
