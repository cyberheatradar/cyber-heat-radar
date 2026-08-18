# 📡 サイレーダー 2026-08-19 05:00 JST

このレポートは、2026-08-18 17:00 JST〜2026-08-19 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 90
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 62

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CISA gives feds 3 days to fix actively exploited Ray RCE bug](#topic-27918) | 54.0 | 96.0 | 82.0 | 音声 | 温度感上位枠 |
| 2 | [CISA Adds Four Known Exploited Vulnerabilities to Catalog](#topic-28016) | 50.0 | 56.0 | 47.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [CISA: Windows Task Host flaw now exploited by ransomware gangs](#topic-28130) | 45.0 | 48.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [New Report: AI threats are here. Why Q2 2026 signals the end of traditional patch cycles](#topic-28100) | 41.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-27918"></a>

### 1. CISA gives feds 3 days to fix actively exploited Ray RCE bug

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>i⁠O⁠S</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 54.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 96.0 |
| <nobr>確⁠度</nobr> | 82.0 |

#### 概要

CISAは、Ray-Projectの分散処理フレームワークRayに関するCVE-2025-62593をKnown Exploited Vulnerabilities（KEV）カタログに追加し、実際に悪用が確認されている脆弱性として注意喚起しました。
公表情報では、コード注入によりリモートコード実行につながる可能性があるとされ、米連邦機関には短期間での修正対応が求められています。
KEV入りは「理論上の脆弱性」ではなく、すでに攻撃者に利用されている可能性が高いことを示します。
特に公開環境や開発用途でRayを使っている組織では、優先度を上げて確認すべき案件です。

#### CISA KEV詳細

- **CVE**: CVE-2025-62593
- **Vendor / Project**: Ray-Project
- **Product**: Ray
- **Vulnerability Name**: Ray-Project Ray Code Injection Vulnerability
- **Date Added**: 2026-08-17
- **Due Date**: 2026-08-20
- **Known Ransomware Use**: Unknown

**Required Action**

> Apply mitigations in accordance with vendor instructions, ensuring compliance with CISA’s BOD 26-04 Prioritizing Security Updates Based on Risk (see URL in Notes) guidance and CISA’s “Forensics Triage Requirements” (see URL in Notes). Follow applicable BOD 26-04 guidance for cloud services or discontinue use of the product if mitigations are unavailable. Stakeholders are responsible for evaluating each asset's internet exposure and ensuring adherence to BOD 26-04 patching guidelines.

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- CISA KEV関連。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Rayの利用有無と公開到達性を確認し、該当バージョンの修正適用を優先する。
- Rayを開発・検証用途で使っている場合でも、ブラウザ経由の影響可能性を含めて影響範囲を見直す。
- KEV掲載対象として、単なるパッチ適用だけでなく、公開資産の棚卸しと侵害痕跡の確認を並行して進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-62593 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Ray-Project | 影響ベンダー | 1.00 | — |
| 製品 | Ray | 影響製品 | 1.00 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-62593](https://nvd.nist.gov/vuln/detail/CVE-2025-62593) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>公的機関</nobr> | [CISA KEV: CVE-2025-62593](https://www.cisa.gov/known-exploited-vulnerabilities-catalog?field_cve=CVE-2025-62593) | <nobr>KEV掲載内容、Date Added、Due Date、Required Action</nobr> |
| <nobr>公的機関データ</nobr> | [CISA KEV JSON](https://www.cisa.gov/sites/default/files/feeds/known_exploited_vulnerabilities.json) | <nobr>CISA公式の機械可読データ。CVE IDで検索して確認</nobr> |
| <nobr>出典</nobr> | [CISA gives feds 3 days to fix actively exploited Ray RCE bug](https://www.theregister.com/security/2026/08/18/cisa-gives-feds-3-days-to-fix-actively-exploited-ray-rce-bug/5289007) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/08/17/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-28130"></a>

### 2. CISA: Windows Task Host flaw now exploited by ransomware gangs

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、Windows Task Hostの高深刻度の脆弱性がランサムウェア攻撃グループにも悪用されていると確認しました。
この脆弱性は4月に「実際に悪用されている」として警告されており、今回あらためて攻撃利用の広がりが示されています。
公的機関が悪用継続を確認しているため、未対応のWindows環境では被害リスクが高まります。
ランサムウェア文脈での利用が示されたことで、通常の脆弱性対応よりも優先度を上げて確認する必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象Windows環境で該当脆弱性の修正適用状況を早急に確認する。
- CISAやベンダーの更新情報を継続監視し、追加の緩和策が出ていないか確認する。
- ランサムウェア対策として、バックアップの保全状況と復旧手順の実効性を点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA: Windows Task Host flaw now exploited by ransomware gangs](https://www.bleepingcomputer.com/news/security/cisa-windows-task-host-flaw-now-exploited-by-ransomware-gangs/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-28100"></a>

### 3. New Report: AI threats are here. Why Q2 2026 signals the end of traditional patch cycles

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>国⁠家⁠支⁠援</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Rapid7の四半期脅威レポートによると、Q2 2026は高・重大度の脆弱性公表件数が大きく増えた一方、実際に悪用される脆弱性は横ばいで、公開から悪用までの時間短縮が課題として浮き彫りになりました。
レポートは、認証不要で到達できる初期侵入のしやすさや、ランサムウェア、国家支援型とみられる活動の継続も指摘しています。
脆弱性の数が増え続ける中で、従来の「速く広くパッチを当てる」運用だけでは追いつきにくくなっていることを示しています。
実務では、重要資産と到達可能な露出を見極めて優先順位を付ける必要性が高まっています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 高・重大度だけでなく、外部から到達可能かどうかを基準に優先順位を付ける。
- 認証不要で露出しやすいサービスや境界機器の棚卸しと保護を見直す。
- ランサムウェアやコラボレーション基盤を悪用した社会工学の動向を継続監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ランサムウェアグループ | Qilin | 主題 | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| 製品 | Microsoft Teams | 言及あり | 0.80 | — |
| 製品 | Ivanti Connect Secure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New Report: AI threats are here. Why Q2 2026 signals the end of traditional patc](https://www.rapid7.com/blog/post/tr-new-report-ai-threats-q2-2026-ends-traditional-patch-cycles) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-28016"></a>

### 1. CISA Adds Four Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>A⁠I</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 50.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 47.0 |

#### 概要

CISAは、実際の悪用が確認されているとして、4件の脆弱性をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
対象にはMicrosoft、Broadcom、Appleの製品に関わる脆弱性が含まれており、組織での優先対応が必要な案件とみられます。
KEVへの追加は、単なる既知の脆弱性ではなく、攻撃者に実際に狙われている可能性が高いことを示します。
該当製品を運用している組織では、資産確認と修正適用の優先度を上げる判断材料になります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象製品の利用有無と影響範囲を早急に棚卸しする。
- ベンダーの修正版・緩和策の適用状況を確認し、優先度を上げて対応する。
- 外部公開面や管理系機能の露出を点検し、監視と検知ルールを強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Broadcom | 言及あり | 0.80 | — |
| ベンダー | Apple | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Exchange | 言及あり | 0.80 | — |
| 製品 | VMware vCenter Server | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Four Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/08/18/cisa-adds-four-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Flags Actively Exploited Ray Flaw That Can Trigger Browser-Based RCE](https://thehackernews.com/2026/08/cisa-flags-actively-exploited-ray-flaw.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Agentic Source Code Reviewによる敵対的AIへの先手対応](https://cloud.google.com/blog/topics/threat-intelligence/staying-ahead-of-adversarial-ai-through-agentic-source-code-review/) | 29.0 | 20.0 | 43.0 |
| [Medusaランサムウェアが新たに数百件の被害を確認、グループの戦術を更新した勧告で判明](https://cyberscoop.com/medusa-ransomware-tactics-cisa-advisory/) | 28.0 | 30.0 | 48.0 |
| [Medusaランサムウェアの被害者200件超をこの1年で特定、CISAが発表](https://therecord.media/more-than-200-medusa-ransomware-victims-in-last-year-cisa) | 28.0 | 30.0 | 42.0 |
| [ClopがWindchillのデータ窃取攻撃向けに独自のWebシェルを作成](https://www.bleepingcomputer.com/news/security/clop-created-custom-web-shell-for-windchill-data-theft-attacks/) | 28.0 | 30.0 | 42.0 |
| [Ransom Bustersがランサムウェアのサーバーをハッキングしたと主張、被害者に最大6万ドルを要求](https://thehackernews.com/2026/08/ransom-busters-claims-it-hacked.html) | 28.0 | 30.0 | 42.0 |
| [数千件の侵害されたWordPressサイトを用いた一つの作戦：StopAndProtectの正体を暴く](https://research.checkpoint.com/2026/thousands-of-hacked-wordpress-sites-one-operation-unmasking-stopandprotect/) | 28.0 | 30.0 | 42.0 |
| [『Ransom Busters』：ランサムウェア攻撃者がインシデント復旧サービスを装う](https://www.darkreading.com/cyberattacks-data-breaches/ransom-busters-ransomware-actor-incident-recovery-service) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア攻撃の4分の3は中堅企業を標的にしている](https://www.infosecurity-magazine.com/news/threequarters-ransomware-attacks/) | 28.0 | 30.0 | 42.0 |
| [CISA Malcolmに関するサイバーセキュリティ情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-230-01) | 28.0 | 28.0 | 50.0 |
| [NETSCOUT、Adaptive DDoS Protectionを拡張しアウトバウンド攻撃の軽減機能を追加](https://www.helpnetsecurity.com/2026/08/18/netscout-expands-adaptive-ddos-protection-with-outbound-attack-mitigation/) | 28.0 | 20.0 | 42.0 |
| [Microsoftのクラウド上で完全に活動する静かな「TwinLoot」サイバー脅威](https://www.darkreading.com/cloud-security/silent-twinloot-threat-operates-microsoft-cloud) | 28.0 | 20.0 | 42.0 |
| [2025年以降、1人の攻撃者がSalesforceとServiceNowのポータルをスクレイピングしていた](https://thehackernews.com/2026/08/one-attacker-has-scraped-both.html) | 28.0 | 20.0 | 42.0 |
| [Typosquattingされた16件のRubyGemsパッケージがブラウザ認証情報と暗号資産ウォレットを窃取](https://thehackernews.com/2026/08/16-typosquatted-rubygems-packages-steal.html) | 28.0 | 20.0 | 42.0 |
| [Hackerが企業のAzureテナントから数百万件のレコードを盗んだと主張](https://www.helpnetsecurity.com/2026/08/18/azure-data-leak-fortune-500-companies/) | 28.0 | 20.0 | 42.0 |
| [生成AIで巧妙化するデマ──熊本地震で露見した「10年前にはなかった新たな手法」 識者に聞く](https://www.itmedia.co.jp/news/article/2608/18/2000000600/) | 26.0 | 20.0 | 42.0 |
| [GitLabの重大な脆弱性により攻撃者が公開プロジェクトを改ざん・削除可能に（CVE-2026-19478）](https://www.helpnetsecurity.com/2026/08/18/gitlab-critical-code-injection-flaw-cve-2026-19478/) | 25.0 | 46.0 | 54.0 |
| [WizのAIエージェントが発見した、Advanced Securityで見逃されたSnowflakeのGitHubリポジトリの重大な脆弱性](https://www.infosecurity-magazine.com/news/wiz-ai-agent-finds-snowflake/) | 25.0 | 20.0 | 42.0 |
| [CISO対話：Nico Waisman ― 独学ハッカーからXBOWでのAI駆動型オフェンシブセキュリティへ](https://www.securityweek.com/ciso-conversations-nico-waisman-from-self-taught-hacker-to-ai-driven-offensive-security-at-xbow/) | 25.0 | 20.0 | 42.0 |
| [Copilotをだまして自身をハッキングする方法を研究者に答えさせる手口](https://www.theregister.com/research/2026/08/18/copilot-tricked-into-telling-reseachers-how-to-hack-itself/5288857) | 25.0 | 20.0 | 42.0 |
| [AI主導の脆弱性急増が従来のパッチ適用モデルを崩す](https://www.securityweek.com/ai-driven-vulnerability-surge-breaks-the-traditional-patching-model/) | 25.0 | 20.0 | 42.0 |
| [Akamai Valkey Managed Database: エンタープライズAI向けのリアルタイムメモリ](https://www.akamai.com/blog/cloud/2026/aug/valkey-managed-database-real-time-memory-enterprise-ai) | 25.0 | 20.0 | 42.0 |
| [AIエージェント間で永続的なプロンプトファイルを通じて感染する「マインドウイルス」](https://thehackernews.com/2026/08/ai-mind-viruses-can-spread-between.html) | 25.0 | 20.0 | 42.0 |
| [Xpander、AI管理とガバナンスのために750万ドルを調達](https://www.securityweek.com/xpander-raises-7-5-million-for-ai-management-and-governance/) | 25.0 | 20.0 | 42.0 |
| [Fortinet、AIセキュリティ企業のVirtue AIを買収](https://www.securityweek.com/fortinet-acquires-ai-security-company-virtue-ai/) | 25.0 | 20.0 | 42.0 |
| [AI搭載の脆弱性情報集約基盤は強い懐疑と大きな課題に直面している](https://www.cybersecuritydive.com/news/ai-vulnerability-clearinghouse-us-government-challenges/827710/) | 25.0 | 20.0 | 42.0 |
| [2026年 Wiz パートナーアライアンス賞受賞者の発表](https://www.wiz.io/blog/2026-partner-award-winners) | 25.0 | 20.0 | 42.0 |
| [Googleの1万ドル返金テストが示す、AIエージェントにゼロトラストが必要な理由](https://www.helpnetsecurity.com/2026/08/18/google-zero-trust-ai-agents/) | 25.0 | 20.0 | 42.0 |
| [自律型AIセキュリティに欠けている暗号学的アテステーション層](https://securityboulevard.com/2026/08/cryptographic-attestation-is-the-missing-layer-for-autonomous-ai-security/) | 25.0 | 20.0 | 42.0 |
| [AIの массов導入が継続的な脅威露出管理への移行をどう再定義するか](https://securityboulevard.com/2026/08/how-the-mass-adoption-of-ai-is-redefining-the-shift-to-continuous-threat-exposure-management/) | 25.0 | 20.0 | 42.0 |
| [AIファクトリーの盲点は信頼：Confidential AI が欠けたインフラ層である理由](https://securityboulevard.com/2026/08/the-ai-factorys-blind-spot-is-trust-why-confidential-ai-is-the-missing-infrastructure-layer/) | 25.0 | 20.0 | 42.0 |
| [AIの速度でソフトウェアを保護する：4年間のデータが示すもの](https://securityboulevard.com/2026/08/securing-software-at-the-speed-of-ai-what-four-years-of-data-reveal/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、AIエージェントによる研究環境侵害を受け防御を強化](https://www.helpnetsecurity.com/2026/08/18/openai-strengthening-security-measures/) | 25.0 | 20.0 | 42.0 |
| [Model Context Protocol（MCP）ツール連携のセキュリティ確保](https://securityboulevard.com/2026/08/securing-model-context-protocol-mcp-tool-integrations/) | 25.0 | 20.0 | 42.0 |
| [英国の法務規制当局、AI悪用への懸念を表明](https://www.infosecurity-magazine.com/news/uk-legal-regulator-raises-ai/) | 25.0 | 20.0 | 42.0 |
| [Formプラグインの欠陥により30万件のWordPressサイトがハッキングにさらされる可能性](https://www.securityweek.com/300000-wordpress-sites-potentially-exposed-to-hacking-due-to-form-plugin-flaw/) | 24.0 | 46.0 | 50.0 |
| [GitLab、重大なコード注入の脆弱性に緊急パッチを公開](https://www.cybersecuritydive.com/news/gitlab-emergency-patch-critical-code-injection/828151/) | 24.0 | 38.0 | 42.0 |
| [NASA地上管制ソフトウェアの脆弱性により認証不要のコマンド実行が可能に](https://www.infosecurity-magazine.com/news/nasa-ground-control-software-flaw/) | 24.0 | 38.0 | 42.0 |
| [GitLabの重大なコードインジェクション脆弱性を修正](https://www.securityweek.com/gitlab-patches-critical-code-injection-vulnerability/) | 24.0 | 38.0 | 42.0 |
| [MacSync Stealerのインフラを行動ベースのピボットで追跡する](https://www.microsoft.com/en-us/security/blog/2026/08/18/hunting-macsync-stealer-infrastructure-through-behavioral-pivots/) | 22.0 | 20.0 | 42.0 |
| [メルアカに不正アクセス、個人情報流出の可能性 - ナイス](https://www.security-next.com/188537) | 22.0 | 20.0 | 42.0 |
| [利用予定のウェブシステムに攻撃 - ウォーターサーバ事業者](https://www.security-next.com/188461) | 22.0 | 20.0 | 42.0 |
| [Apple、コード実行につながる画像処理の脆弱性を修正](https://www.malwarebytes.com/blog/bugs/2026/08/apple-fixes-another-image-processing-flaw-that-could-allow-code-execution) | 20.0 | 28.0 | 50.0 |
| [Microsoft Copilot Personalの脆弱性により、1回のクリックで接続済みアプリからデータを流出させる可能性](https://thehackernews.com/2026/08/microsoft-copilot-personal-flaws-could.html) | 20.0 | 20.0 | 42.0 |
| [Attackers が MLflow の SSRF 脆弱性を悪用してクラウド認証情報とシークレットを窃取](https://thehackernews.com/2026/08/attackers-exploit-mlflow-ssrf-flaw-to.html) | 20.0 | 20.0 | 42.0 |
| [ソフトウェアサプライチェーンセキュリティがチャネルパートナーにとって次の説明責任の課題となる理由](https://www.itpro.com/security/why-software-supply-chain-security-is-the-next-accountability-challenge-for-channel-partners) | 20.0 | 20.0 | 42.0 |
| [ベルリン、セキュリティ侵害を受け州の2省庁を政府ネットワークから遮断](https://therecord.media/berlin-cuts-two-state-ministries-off-government-breach) | 20.0 | 20.0 | 42.0 |
| [サイバー攻撃を受けたUniversity of Texas、San Antonioでシステムを停止](https://therecord.media/university-of-texas-forced-to-take-systems-offline-cyberattack-san-antonio) | 20.0 | 20.0 | 42.0 |
| [エンタープライズアプリケーションは重大・高リスクの脆弱性を4.31倍多く抱える](https://www.infosecurity-magazine.com/news/enterprise-apps-critical-high/) | 20.0 | 20.0 | 42.0 |
| [Apple、スパイウェア悪用の恐れがある画像処理の脆弱性を修正](https://www.theregister.com/security/2026/08/18/apple-plugs-image-processing-hole-ripe-for-spyware-abuse/5289031) | 20.0 | 20.0 | 42.0 |
| [既知の攻撃は制御できても、行動はどうか？](https://www.bleepingcomputer.com/news/security/your-controls-block-known-attacks-what-about-the-behavior/) | 20.0 | 20.0 | 42.0 |
| [TWINLOOTがSharePointとTeamsを悪用して認証情報を窃取しネットワーク内を横断移動](https://thehackernews.com/2026/08/twinloot-abuses-sharepoint-and-teams-to.html) | 20.0 | 20.0 | 42.0 |
| [Akamai、Forrester Waveのマイクロセグメンテーションソリューション分野でリーダーに選出](https://www.akamai.com/blog/security/2026/aug/akamai-2026-forrester-wave-leader-microsegmentation) | 20.0 | 20.0 | 42.0 |
| [陸自の個人情報収集 昨年公益通報](https://news.yahoo.co.jp/pickup/6592210?source=rss) | 20.0 | 20.0 | 42.0 |
| [UT San Antonioの学生サービスを妨げたサイバーインシデント](https://www.infosecurity-magazine.com/news/cyber-incident-ut-san-antonio/) | 20.0 | 20.0 | 42.0 |
| [「リンクを知っている全員」に共有したGoogle Docsの取り扱いに注意](https://www.malwarebytes.com/blog/news/2026/08/be-careful-what-you-put-in-anyone-with-the-link-google-docs) | 20.0 | 20.0 | 42.0 |
| [HackerがMcDonald’s、Vodafone、KyndrylなどからAzure顧客レコード数百万件を窃取したと主張、判明していること](https://www.itpro.com/security/data-breaches/hacker-claims-to-have-stolen-millions-of-azure-customer-records-from-mcdonalds-vodafone-kyndryl-and-others-heres-what-we-know-so-far) | 20.0 | 20.0 | 42.0 |
| [Heights Financeのデータ侵害：顧客が知っておくべきこと](https://www.malwarebytes.com/blog/data-breaches/2026/08/heights-finance-data-breach-what-customers-need-to-know) | 20.0 | 20.0 | 42.0 |
| [レガシーな運用モデルはITの複雑化に追いつけない、Cloud Security Allianceの調査で判明](https://cloudsecurityalliance.org/articles/legacy-operating-models-can-t-keep-pace-with-it-complexity-cloud-security-alliance-survey-finds) | 20.0 | 20.0 | 42.0 |
| [Mirage2FAが企業のMicrosoft 365セッションを乗っ取り、米国で4,000以上の被害者に影響](https://any.run/cybersecurity-blog/mirage2fa-phishing-targets-us-companies/) | 20.0 | 20.0 | 42.0 |
| [Heights Financeのデータ侵害で少なくとも120万人に影響](https://www.securityweek.com/heights-finance-data-breach-impacts-at-least-1-2-million-individuals/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、サイバー犯罪者に悪用されてきたWMICツールの削除を開始](https://www.bleepingcomputer.com/news/microsoft/microsoft-removes-wmic-lolbin-tool-in-windows-11-beta-builds/) | 20.0 | 20.0 | 42.0 |
| [AisuruのLANパーティー招待者は誰か？](https://www.bitsight.com/blog/who-invited-aisuru-lan-party) | 20.0 | 20.0 | 42.0 |

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
