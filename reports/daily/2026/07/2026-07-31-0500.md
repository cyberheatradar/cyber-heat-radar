# 📡 サイレーダー 2026-07-31 05:00 JST

このレポートは、2026-07-30 17:00 JST〜2026-07-31 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 120
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 87

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cisco FMC static credentials exploited by attackers (CVE-2026-20316)](#topic-24943) | 47.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 2 | [Batten Down Your Packages: Mitigation Guidance for Supply Chain Compromise](#topic-25188) | 43.0 | 45.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Laundry Bear’s new Microsoft Exchange attack triggers on email open (CVE-2026-42897)](#topic-5098) | 42.0 | 52.0 | 66.0 | 音声 | 温度感上位枠 |
| 4 | [CVE-2025-20333: Cisco ASA/FTD persistence mechanism update](#topic-203) | 41.0 | 56.0 | 65.0 | 音声 | 温度感上位枠 |
| 5 | [Microsoft 2026年7月 Patch Tuesday 関連まとめ](#topic-22358) | 36.0 | 48.0 | 57.0 | 音声 | 温度感上位枠 |
| 6 | [注意喚起: Ruby on RailsのActive Storageにおけるリモートコード実行につながる脆弱性（CVE-2026-66066）に関する注意喚起 (公開)](#topic-24929) | 35.0 | 56.0 | 60.0 | GitHub | 音声枠上限によりGitHubのみ |
| 7 | [The Fuyao Enterprise: Building an Ad-Fraud Empire with AI and Kids’ Coding Blocks](#topic-25231) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 8 | [Chinese-Speaking Threat Actor Harnesses AI Models for Autonomous Cyberattacks](#topic-25249) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-24943"></a>

### 1. Cisco FMC static credentials exploited by attackers (CVE-2026-20316)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 47.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Cisco Secure Firewall Management Center（FMC）ソフトウェアのWebインターフェースに、静的な低権限アカウントの認証情報が存在する脆弱性（CVE-2026-20316）が公表され、悪用が観測されているとされています。
影響を受ける機器では、未認証の遠隔攻撃者がログインして機微情報にアクセスできる可能性があると案内されています。
FMCは複数のファイアウォール機器を集中管理する基盤のため、影響が広がると管理情報へのアクセスリスクが問題になります。
公開インターネットから到達可能な管理面では攻撃面が大きくなり、他の脆弱性と組み合わさる懸念もあります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Ciscoの修正済みソフトウェア更新の適用状況を確認する。
- FMC管理インターフェースが外部公開されていないか点検し、到達範囲を最小化する。
- 管理ログを確認し、不審なログインや想定外のアクセスの有無を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20316 | 主題CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20316](https://nvd.nist.gov/vuln/detail/CVE-2026-20316) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco FMC static credentials exploited by attackers (CVE-2026-20316)](https://www.helpnetsecurity.com/2026/07/30/cisco-fmc-cve-2026-20316-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure FMC Zero-Day Exploited in the Wild](https://www.securityweek.com/cisco-secure-fmc-zero-day-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of FMC static credential flaw exploited in zero-day attacks](https://www.bleepingcomputer.com/news/security/cisco-warns-of-fmc-static-credential-flaw-exploited-in-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Firewall Management Center Software Static Credential Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-fmc-static-cred-BET3Cjh) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-25188"></a>

### 2. Batten Down Your Packages: Mitigation Guidance for Supply Chain Compromise

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>サ⁠プ⁠ラ⁠イ⁠チ⁠ェ⁠ー⁠ン</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>M⁠C⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 45.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Google Threat Intelligence Group（GTIG）は、オープンソースのソフトウェアレポジトリや依存関係を狙うサプライチェーン侵害が2025年から2026年初頭にかけて拡大していると報告しています。
特に、公開パッケージの改ざんや開発者向けツールを起点に、認証情報の窃取やCI/CD環境への影響につながる事例が確認されたとしています。
一方で、従来型のソフトウェア供給網の改ざんは、相対的にはまれだと分析しています。
開発環境や依存パッケージの侵害は、単一組織にとどまらず下流の多数の利用者へ波及し得るため、被害規模が大きくなりやすい点が注目されています。
AIを用いた開発や自動化が進むほど、信頼済みとみなされやすいコードやツールの混入リスクが高まる可能性があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- ランサムウェア文脈。
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 依存関係、ビルドツール、外部ベンダーを含む資産棚卸しとSBOM管理を継続し、影響範囲を把握できるようにする。
- CI/CDやリポジトリの権限設定を見直し、長寿命トークンの抑制、短命資格情報、最小権限、保護ルールの徹底を進める。
- 新規公開パッケージや更新の取り込みには確認手順を設け、署名検証、スキャン、隔離された実行環境などで段階的に検証する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脅威アクター | AppleJeus | 主題 | 0.80 | — |
| 脅威アクター | APT29 | 主題 | 0.80 | — |
| ベンダー | Mandiant | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Okta | 言及あり | 0.80 | — |
| ベンダー | Wiz | 言及あり | 0.80 | — |
| 製品 | Apache Log4j | 言及あり | 0.80 | — |
| マルウェア | SectopRAT | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Batten Down Your Packages: Mitigation Guidance for Supply Chain Compromise](https://cloud.google.com/blog/topics/threat-intelligence/mitigation-guidance-for-supply-chain-compromise/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-5098"></a>

### 3. Laundry Bear’s new Microsoft Exchange attack triggers on email open (CVE-2026-42897)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 42.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 52.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Microsoft Exchange Serverの脆弱性CVE-2026-42897が、メールを開いた際の表示をきっかけに悪用される事例が報告されています。
公開情報では、標的型のメール経由で政府機関や民間組織が狙われ、実際の悪用が観測されたとされています。
CISAの既知悪用脆弱性カタログにも追加されており、単なる注意喚起ではなく、実際に攻撃で使われている可能性が高い点が重要です。
Exchange/OWAは組織内の認証やメール運用の要所であるため、影響範囲が広がりやすい脆弱性です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- XSS系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Microsoftの案内やCISAの情報を確認し、対象バージョンと緩和策の適用状況を早急に点検する。
- Exchange/OWAへの不審なアクセスや、メール閲覧を起点とする異常な挙動がないか監視を強める。
- 標的型メールの受信者に対し、見慣れないメールやリンクを開く前の確認を再徹底する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-42897 | 主題CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Exchange | 言及あり | 0.80 | — |
| ベンダー | Proofpoint | 言及あり | 0.80 | — |
| ベンダー | Zimbra | 言及あり | 0.80 | — |
| 製品 | Microsoft Exchange Server | 言及あり | 0.80 | — |
| 製品 | WordPress | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-42897](https://nvd.nist.gov/vuln/detail/CVE-2026-42897) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Laundry Bear’s new Microsoft Exchange attack triggers on email open (CVE-2026-42](https://www.helpnetsecurity.com/2026/07/30/cve-2026-42897-microsoft-exchange-email-attack/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cleaning Out Inboxes: TA488 Comes for Outlook with Another Half-Click Exploit](https://www.proofpoint.com/us/blog/threat-insight/cleaning-out-inboxes-ta488-comes-outlook-another-half-click-exploit) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches Exploited Exchange Server Vulnerability](https://www.securityweek.com/microsoft-patches-exploited-exchange-server-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Exchange Zero-Day Under Attack, No Patch Available](https://www.darkreading.com/vulnerabilities-threats/microsoft-exchange-zero-day-no-patch) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Warns of Exchange Server Zero-Day Exploited in the Wild](https://www.securityweek.com/microsoft-warns-of-exchange-server-zero-day-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/05/15/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Unpatched Microsoft Exchange Server vulnerability exploited (CVE-2026-42897)](https://www.helpnetsecurity.com/2026/05/15/exchange-server-cve-2026-42897-exploited/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: あり（2件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-203"></a>

### 4. CVE-2025-20333: Cisco ASA/FTD persistence mechanism update

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 65.0 |

#### 概要

Cisco Secure Firewall ASA/FTDに関するCVE-2025-20333を含む注意喚起が更新され、修正済みリリースへ更新後も残りうる永続化の仕組みが確認されたとされています。
初期侵入は、修正前に存在したVPN Web Server関連の脆弱性の悪用から始まった可能性が示されていますが、詳細は限定的です。
境界防御機器で侵入後の永続化が残りうる点は、単なるパッチ適用だけでは不十分なケースがあることを示します。
Cisco機器を運用する組織では、侵害有無の確認と更新後の再点検が重要になります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ASA/FTDの対象機器が修正済みリリースに更新されているかを確認し、更新済みでも侵害兆候の点検を行う。
- VPN Web Server周辺の異常な挙動や不審な設定変更、想定外の管理系アクセス履歴を確認する。
- CISAやJPCERT/CC、Ciscoの最新注意喚起を参照し、資産影響範囲と優先度を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-20333 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2025-20362 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-20333](https://nvd.nist.gov/vuln/detail/CVE-2025-20333) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [OctLurk and SilkLurk: newly identified tailored backdoors in cyber-espionage cam](https://securelist.com/octlurk-silklurk-backdoors-central-asia/120840/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [US Threat Landscape Alert: 30 Active Malware Families Ranked by Real Sandbox Dat](https://any.run/cybersecurity-blog/usa-top-30-threats-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [From edge appliance to enterprise compromise: Multi-stage Linux intrusion via F5](https://www.microsoft.com/en-us/security/blog/2026/05/22/from-edge-appliance-to-enterprise-compromise-multi-stage-linux-intrusion-via-f5-and-confluence/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Continued Evolution of Persistence Mechanism Against Cisco Secure Firewall Adapt](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-persist-CISAED25-03) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Weekly Report: JPCERT/CCが「Cisco ASAおよびFTDにおける複数の脆弱性（CVE-2025-20333、CVE-2025-2036](https://www.jpcert.or.jp/wr/2026/wr260430.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: Cisco ASAおよびFTDにおける複数の脆弱性（CVE-2025-20333、CVE-2025-20362）に関する注意喚起  (更新)](https://www.jpcert.or.jp/at/2025/at250021.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [It pays to be a forever student](https://blog.talosintelligence.com/it-pays-to-be-a-forever-student/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-22358"></a>

### 5. Microsoft 2026年7月 Patch Tuesday 関連まとめ

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>i⁠O⁠S</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>A⁠I</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 57.0 |

#### 概要

Microsoftの2026年7月 Patch Tuesdayでは、Microsoft製品向けに622件の脆弱性修正が公開され、Edgeに含まれるChromium由来の427件は別枠で扱われています。
今回の修正には重大度の高いものが62件含まれ、事前公表されたものや、既に悪用が確認されているものもあるとされています。
修正件数が非常に多く、しかも既知の悪用事例が含まれるため、優先度をつけた迅速な対応が必要です。
企業環境では、OSだけでなくEdgeや周辺のMicrosoft製品まで含めて影響確認を行う必要があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 13 sources。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 既に悪用済みとされる脆弱性を最優先で確認し、適用状況を点検する。
- EdgeのChromium更新分も含め、Microsoft製品全体のパッチ適用計画を見直す。
- 重要システムでは、展開前後の不具合確認と資産ごとの適用優先度付けを行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-26145 | 主題CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-27690 | 主題CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-33842 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34328 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34346 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34348 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34349 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-40378 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-40400 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-40422 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [The July 2026 Apple Security Update Review](https://www.thezdi.com/blog/2026/7/29/the-july-2026-apple-security-update-review) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Why Microsoft paused Patch Tuesday updates for some Dell devices](https://www.itpro.com/security/why-microsoft-paused-patch-tuesday-updates-for-some-dell-devices) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft cancels Patch Tuesday for some Dell users over surprise shutdowns, ove](https://www.theregister.com/os-platforms/2026/07/15/microsoft-cancels-patch-tuesday-for-some-dell-users-over-surprise-shutdowns-overheating-devices/5271691) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [July 2026 Patch Tuesday fixes 622 Microsoft CVEs, including three zero-days](https://www.malwarebytes.com/blog/bugs/2026/07/july-2026-patch-tuesday-fixes-622-microsoft-cves-including-three-zero-days) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft smashes Patch Tuesday record for second successive month](https://therecord.media/microsoft-vulnerabilities-patch-tuesday-release) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Researcher Drops New Windows Zero-Day PoC Hours After Microsoft Patch Tuesday](https://thehackernews.com/2026/07/researcher-drops-new-windows-zero-day.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [AI-driven bug hunting fuels record Microsoft Patch Tuesday](https://www.helpnetsecurity.com/2026/07/15/microsoft-patch-tuesday-sharepoint-cve-2026-56164/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches 570 CVEs in Record Patch Tuesday](https://www.infosecurity-magazine.com/news/microsoft-570-cves-patch-tuesday/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（1件）。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-25231"></a>

### 6. The Fuyao Enterprise: Building an Ad-Fraud Empire with AI and Kids’ Coding Blocks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>A⁠I</nobr> / <nobr>A⁠n⁠d⁠r⁠o⁠i⁠d</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

BitsightのTRACEチームが、Android TV向けの隠れたボットネットとされる「Fuyao Enterprise」を公表しました。
報告では、AIで生成された多数のデジタル人間を使い、大規模な広告不正に関与している可能性が示されています。
広告不正は広告費の損失だけでなく、配信や計測の信頼性を損なうため、広告関連の事業者に影響し得ます。
AIを組み合わせた手口は、従来型の不正検知だけでは見逃される可能性があるため注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 広告配信や計測の異常なトラフィック増加、視聴・クリック指標の不自然な偏りを確認する。
- Android TV関連の流入や端末群からのアクセスについて、ボットらしい挙動の検知ルールを見直す。
- 不正広告やアドフラウド対策では、端末属性・行動パターン・IP分布など複数の観点で相関確認を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | Active Directory | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [The Fuyao Enterprise: Building an Ad-Fraud Empire with AI and Kids’ Coding Block](https://www.bitsight.com/blog/fuyao-enterprise-building-ad-fraud-empire-ai-and-kids-coding-blocks) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-25249"></a>

### 7. Chinese-Speaking Threat Actor Harnesses AI Models for Autonomous Cyberattacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Unit 42は、中国語を話す脅威アクターがAIモデルを使い、複数の脆弱性に対する自動スキャンと手動での悪用を組み合わせていると報告しました。
公開情報では、AIを攻撃の一部に取り込む動きが確認されており、従来型の手口と組み合わせた運用が示唆されています。
攻撃者がAIを使って探索や初期段階の作業を効率化すると、攻撃の実行速度や規模が変わる可能性があります。防御側は、AI由来の自動化を前提にした監視・検知の見直しが必要になります。

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

- 外部公開資産の露出確認と、脆弱性管理の優先度付けを再点検する。
- 通常のスキャン増加だけでなく、短時間で広範囲を探る挙動を監視対象に含める。
- 自動化された探索と手動操作が混在する前提で、アラートの相関分析を強化する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Chinese-Speaking Threat Actor Harnesses AI Models for Autonomous Cyberattacks](https://unit42.paloaltonetworks.com/autonomous-ai-cyber-attack-campaign/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-24929"></a>

### 1. 注意喚起: Ruby on RailsのActive Storageにおけるリモートコード実行につながる脆弱性（CVE-2026-66066）に関する注意喚起 (公開)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 60.0 |

#### 概要

Ruby on RailsのActive Storageに関する脆弱性CVE-2026-66066について、JPCERT/CCが注意喚起を出しています。
公開情報では、画像処理に関連してアプリケーションサーバ上のファイルが読み取られる可能性があり、条件次第で機密情報の露出につながるおそれがあるとされています。
Rails製アプリは広く使われており、Active Storageを利用している環境では影響範囲の確認が急がれます。
秘密情報の漏えいは、認証情報やクラウド設定の悪用、さらなる侵害につながる可能性があるためです。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
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

- Active Storageと画像処理ライブラリの利用有無を確認し、影響を受ける構成かを把握する。
- Ruby on Railsの修正版適用状況を確認し、未適用なら優先的に更新する。
- アプリケーションの秘密情報、外部連携の認証情報、アクセスログの異常を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-66066 | 主題CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-66066](https://nvd.nist.gov/vuln/detail/CVE-2026-66066) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [KindaRails2Shell: CVE-2026-66066, Critical Arbitrary File Read and Possible Remo](https://www.rapid7.com/blog/post/etr-kindarails2shell-cve-2026-66066-critical-arbitrary-file-read-and-possible-remote-code-execution-in-ruby-on-rails) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: Ruby on RailsのActive Storageにおけるリモートコード実行につながる脆弱性（CVE-2026-66066）に関する注意喚起 ](https://www.jpcert.or.jp/at/2026/at260021.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Rails Flaw Could Let Unauthenticated Attackers Read Server Files via Im](https://thehackernews.com/2026/07/critical-rails-flaw-could-let.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: あり（1件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Microsoft Teamsを悪用したvishing攻撃がChaosランサムウェア攻撃につながる](https://www.bleepingcomputer.com/news/security/microsoft-teams-vishing-attacks-lead-to-chaos-ransomware-attacks/) | 36.0 | 30.0 | 42.0 |
| [Microsoft Teamsを悪用する偽ITサポート経由のランサムウェア攻撃](https://www.cybersecuritydive.com/news/hackers-microsoft-teams-ransomware-it-support/826591/) | 36.0 | 30.0 | 42.0 |
| [ランサム被害で個人情報流出の可能性 - FA機器開発会社](https://www.security-next.com/187746) | 30.0 | 30.0 | 42.0 |
| [VMware vCenterの重大な脆弱性により認証回避とリモートコード実行が可能に（CVE-2026-59309、CVE-2026-59310）](https://www.rapid7.com/blog/post/etr-critical-vmware-vcenter-vulnerabilities-allow-authentication-bypass-and-remote-code-execution-cve-2026-59309-cve-2026-59310) | 29.0 | 56.0 | 56.0 |
| [北朝鮮のLazarus Groupがランサムウェア攻撃者とツールを共有、韓国当局が警告](https://therecord.media/north-korea-hackers-ransomware) | 28.0 | 30.0 | 42.0 |
| [Toy Ghoulsの新たなおもちゃ: GenieLockerランサムウェア](https://securelist.com/genielocker-ransomware-for-windows-linux-and-esxi/120843/) | 28.0 | 30.0 | 42.0 |
| [Malwarebytes for Windows、Microsoft Storeで提供開始](https://www.malwarebytes.com/blog/product/2026/07/malwarebytes-for-windows-now-available-on-the-microsoft-store) | 28.0 | 20.0 | 42.0 |
| [侵入後に攻撃者が内部で行うこと](https://www.bleepingcomputer.com/news/security/after-the-break-in-what-attackers-do-once-theyre-already-inside/) | 28.0 | 20.0 | 42.0 |
| [Teamsを装ったフィッシング अभियानで正規のMicrosoftログインページが悪用される](https://www.infosecurity-magazine.com/news/teams-phishing-abused-legit/) | 28.0 | 20.0 | 42.0 |
| [攻撃者がMicrosoftの正規ログインシステムを悪用してフィッシング攻撃を隠蔽している](https://www.helpnetsecurity.com/2026/07/30/microsoft-authentication-system-phishing/) | 28.0 | 20.0 | 42.0 |
| [ハッカーが韓国の改ざんサイト経由でAnySign4PCを悪用し、プロンプトなしでバックドアを設置](https://thehackernews.com/2026/07/hackers-exploit-anysign4pc-via-hacked.html) | 28.0 | 20.0 | 42.0 |
| [SilverFoxが3つのドライバを用いるBYOVDチェーンとValleyRATで日本の製造業者を標的にする](https://thehackernews.com/2026/07/silverfox-targets-japanese-manufacturer.html) | 28.0 | 20.0 | 42.0 |
| [Google Cloud Next Tokyoが開幕、三上代表「AIエージェントは本番運用へ」](https://xtech.nikkei.com/atcl/nxt/news/24/03322/) | 28.0 | 20.0 | 42.0 |
| [Chinese Open-weight AIモデル：サイバーセキュリティ上のリスクと恩恵](https://www.f5.com/labs/articles/chinese-open-weight-ai-models-cybersecurity-risks-and-rewards) | 27.0 | 20.0 | 42.0 |
| [熊本地震でSNSにデマ拡散 偽の救助要請や募金詐欺、AIを信じ本物を誤判定も](https://www.itmedia.co.jp/news/article/2607/30/2000000311/) | 26.0 | 20.0 | 42.0 |
| [Jscramblerが統合クライアントサイドセキュリティプラットフォームを発表](https://www.helpnetsecurity.com/2026/07/30/jscrambler-unified-client-side-security-platform/) | 25.0 | 20.0 | 42.0 |
| [AIがChromeの脆弱性発見でより重要な役割を担う](https://www.helpnetsecurity.com/2026/07/30/google-chrome-ai-security-workflow/) | 25.0 | 20.0 | 42.0 |
| [Google、AIの支援でChromeの2回のリリースで1,072件のセキュリティバグを修正](https://www.bleepingcomputer.com/news/google/google-says-ai-helped-chrome-fix-1-072-security-bugs-in-two-releases/) | 25.0 | 20.0 | 42.0 |
| [AI時代におけるスキャンの再考：Wizのエージェンティックコードセキュリティシステム](https://www.wiz.io/blog/agentic-code-security) | 25.0 | 20.0 | 42.0 |
| [Claude Mythos ― 誇張と実態：セキュリティチームが知るべきこと](https://www.darkreading.com/cybersecurity-operations/claude-mythos-hype-vs-reality) | 25.0 | 20.0 | 42.0 |
| [ThreatsDay: AIを活用したハッキング、370件のChrome脆弱性、SonicWallへの攻撃、DNSハイジャックほか22件の話題](https://thehackernews.com/2026/07/threatsday-ai-powered-hacking-370.html) | 25.0 | 20.0 | 42.0 |
| [Rapid7がIDC MarketScapeのWorldwide MDR Service for Midmarket 2026 Vendor AssessmentでLeaderに選出](https://www.rapid7.com/blog/post/dr-idc-marketscape-leader-worldwide-mdr-service-midmarket-2026-vendor-assessment) | 25.0 | 20.0 | 42.0 |
| [Novee、モバイルアプリに継続的なAIペンテストを導入](https://www.helpnetsecurity.com/2026/07/30/novee-ai-penetration-testing-platform/) | 25.0 | 20.0 | 42.0 |
| [Shadow AIと経営層の抵抗でAIガバナンスに苦慮するCISOたち](https://www.cybersecuritydive.com/news/ai-governance-shadow-cisos-okta/826587/) | 25.0 | 20.0 | 42.0 |
| [ブラックボックスの外で考える：防御側に必要なオープンソースAI](https://www.akamai.com/blog/news/2026/jul/thinking-outside-black-box-defenders-open-source-ai) | 25.0 | 20.0 | 42.0 |
| [AIと自動化はSysadminの期待に届かず](https://www.infosecurity-magazine.com/news/ai-automation-fall-short-sysadmin/) | 25.0 | 20.0 | 42.0 |
| [隠しプロンプトによりMicrosoft CopilotがAIワーム化する問題](https://www.malwarebytes.com/blog/ai/2026/07/hidden-microsoft-copilot-ai-worm) | 25.0 | 20.0 | 42.0 |
| [Onyx Security、企業内のAIエージェント管理に向け1億1300万ドルを調達](https://www.securityweek.com/onyx-security-raises-113-million-to-control-ai-agents-in-the-enterprise/) | 25.0 | 20.0 | 42.0 |
| [「DangleGeddon」：AIが放置されたDNSレコードを大規模に悪用する可能性](https://www.securityweek.com/danglegeddon-ai-could-weaponize-forgotten-dns-records-at-global-scale/) | 25.0 | 20.0 | 42.0 |
| [オープンソースソフトウェアのセキュリティ原則と実践](https://www.cisa.gov/resources-tools/resources/open-source-software-security-principles-and-practices) | 25.0 | 20.0 | 42.0 |
| [Schneider Electric IGSSの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-211-04) | 25.0 | 20.0 | 42.0 |
| [Microsoft Copilot for Wordが隠しプロンプトを新規ドキュメントにコピーする問題](https://thehackernews.com/2026/07/microsoft-copilot-for-word-can-copy.html) | 25.0 | 20.0 | 42.0 |
| [Orca Security、AI生成・開発者作成アプリケーションの保護を強化](https://www.helpnetsecurity.com/2026/07/30/orca-ai-appgen-security-code-security-auditor/) | 25.0 | 20.0 | 42.0 |
| [ネットワークがAIセキュリティの制御プレーンとなった](https://thehackernews.com/2026/07/the-network-has-become-control-plane.html) | 25.0 | 20.0 | 42.0 |
| [PortSwiggerがエージェント型AIのセキュリティテスト向けBurp ATを発表](https://www.helpnetsecurity.com/2026/07/30/portswigger-burp-at/) | 25.0 | 20.0 | 42.0 |
| [Critical Rufloの脆弱性により攻撃者が不正AIスウォームを生成可能に](https://www.securityweek.com/critical-ruflo-flaw-lets-attackers-spawn-rogue-ai-swarms/) | 25.0 | 20.0 | 42.0 |
| [組織として安全にAIシステムを調達する方法](https://securityboulevard.com/2026/07/procuring-ai-systems-securely-as-an-organisation/) | 25.0 | 20.0 | 42.0 |
| [MZ Automation GmbHのlibiec61850に関する脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-211-10) | 24.0 | 46.0 | 50.0 |
| [Toptech SystemsのRCU II+およびMultiload II+](https://www.cisa.gov/news-events/ics-advisories/icsa-26-211-03) | 24.0 | 46.0 | 50.0 |
| [「It’s the Climb」に着目していたあなたは正しかった、Miley](https://blog.talosintelligence.com/you-were-onto-something-with-its-the-climb-miley/) | 22.0 | 20.0 | 42.0 |
| [Microsoft Security の新機能：2026年7月](https://www.microsoft.com/en-us/security/blog/2026/07/30/whats-new-in-microsoft-security-july-2026/) | 22.0 | 20.0 | 42.0 |
| [インシデント件数減少、ただしサイト改ざんは倍増](https://www.security-next.com/187818) | 22.0 | 20.0 | 42.0 |
| [講座受講者リストをメールに誤添付 - 北九州市](https://www.security-next.com/188065) | 22.0 | 20.0 | 42.0 |
| [Black Hat特集：振り返って再訪する](https://blog.talosintelligence.com/black-hat-special-rewind-and-revisit/) | 22.0 | 20.0 | 42.0 |
| [インク通販サイトに不正アクセス - 個人情報流出の可能性](https://www.security-next.com/188056) | 22.0 | 20.0 | 42.0 |
| [Johnson Controls OpenBlue Employeeに関する脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-211-02) | 21.0 | 34.0 | 50.0 |
| [エラー解消のつもりが自ら攻撃を実行する「ClickFix」が108％増 日本の割合が最多14％](https://www.itmedia.co.jp/enterprise/articles/2607/30/news071.html) | 21.0 | 20.0 | 42.0 |
| [深まる先端AIモデルのサイバー攻撃能力への懸念 「恐れるな」とGartnerのアナリストが語る理由](https://atmarkit.itmedia.co.jp/ait/articles/2607/30/news075.html) | 21.0 | 20.0 | 42.0 |
| [Amazonが警告する北朝鮮系ハッカーによる主要なオープンソースサプライチェーン攻撃](https://therecord.media/north-korea-hackers-amazon-malware) | 20.0 | 35.0 | 42.0 |
| [Amazon links Debug、Chalkのnpmサプライチェーン攻撃を北朝鮮のハッカーに関連付け](https://www.bleepingcomputer.com/news/security/amazon-links-debug-chalk-npm-supply-chain-attacks-to-north-korean-hackers/) | 20.0 | 30.0 | 42.0 |
| [MZ Automation lib60870の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-211-11) | 20.0 | 28.0 | 50.0 |
| [MikroTik RouterOSの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-211-01) | 20.0 | 28.0 | 50.0 |
| [Watchfire Controller Software に関する脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-211-09) | 20.0 | 28.0 | 50.0 |
| [NASA Core Flight System (cFS) Health & Safety (HS) アプリケーション](https://www.cisa.gov/news-events/ics-advisories/icsa-26-211-06) | 20.0 | 28.0 | 50.0 |
| [Mitsubishi Electric CC-Link IE TSN通信プロトコル](https://www.cisa.gov/news-events/ics-advisories/icsa-26-211-07) | 20.0 | 28.0 | 50.0 |
| [o6 Automation open62541の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-211-08) | 20.0 | 28.0 | 50.0 |
| [Rockwell Automation CompactLogix 5380 ControlLogix 5580 / 1756-EN4TR通信モジュール](https://www.cisa.gov/news-events/ics-advisories/icsa-26-211-05) | 20.0 | 28.0 | 50.0 |
| [そのTVストリーミングスティックを買う前に読むべきこと](https://krebsonsecurity.com/2026/07/read-this-before-you-buy-that-tv-streaming-stick/) | 20.0 | 20.0 | 48.0 |
| [Okta、ID脅威検知企業Permisoを買収へ](https://www.securityweek.com/okta-to-acquire-identity-threat-detection-firm-permiso/) | 20.0 | 20.0 | 42.0 |
| [半導体大手Analog Devices、データ侵害を報告](https://therecord.media/analog-devices-semiconductor-company-data-breach) | 20.0 | 20.0 | 42.0 |
| [CISAが連邦機関にオープンソースソフトウェアのセキュリティ対策を推奨](https://cyberscoop.com/cisa-open-source-software-security-guidance/) | 20.0 | 20.0 | 42.0 |
| [VMwareが認証回避と仮想マシン脱出を可能にする3件の重大な脆弱性を修正](https://www.bleepingcomputer.com/news/security/vmware-fixes-three-critical-flaws-allowing-auth-bypass-vm-escapes/) | 20.0 | 20.0 | 42.0 |
| [ShinyHuntersがBrinks Homeへの侵害を主張、窃取データの公開を予告](https://www.bleepingcomputer.com/news/security/shinyhunters-claims-brinks-home-breach-threatens-to-leak-stolen-data/) | 20.0 | 20.0 | 42.0 |
| [Timeless Compliance: より良い問いがより大きなフレームワークに勝る理由](https://www.securityweek.com/timeless-compliance-why-better-questions-beat-bigger-frameworks/) | 20.0 | 20.0 | 42.0 |
| [Jailed Flockの破壊者、3台のカメラを破壊し数千ドルの損害を発生させる](https://www.theregister.com/security/2026/07/30/jailed-flock-vandal-wipes-out-three-cameras-racks-up-thousands-in-damages/5281224) | 20.0 | 20.0 | 42.0 |
| [電気通信攻撃から部隊を守る方法はわかっているのに、実行していない](https://defensescoop.com/2026/07/30/we-know-how-to-protect-our-troops-from-telecom-attacks-were-just-not-doing-it/) | 20.0 | 20.0 | 42.0 |
| [Analog Devicesがデータ侵害を公表、業務への影響はなし](https://www.bleepingcomputer.com/news/security/analog-devices-discloses-data-breach-says-operations-unaffected/) | 20.0 | 20.0 | 42.0 |
| [ロマンス詐欺被害者から1000万ドルを盗んだガーナ国籍の男に懲役7年の判決](https://cyberscoop.com/ghanaian-national-sentenced-romance-scam/) | 20.0 | 20.0 | 42.0 |
| [政府向けサービスのAPIセキュリティ：市民向けアプリケーションを保護する方法](https://www.akamai.com/blog/security/2026/jul/api-security-government-citizen-facing-applications) | 20.0 | 20.0 | 42.0 |
| [DataBahn、エージェント型データパイプライン管理で4000万ドルを調達](https://www.securityweek.com/databahn-raises-40-million-for-agentic-data-pipeline-management/) | 20.0 | 20.0 | 42.0 |
| [Hims & Hersの健康データプライバシー不備をめぐり提訴](https://www.malwarebytes.com/blog/privacy/2026/07/hims-hers-sued-over-alleged-health-data-privacy-failures) | 20.0 | 20.0 | 42.0 |
| [Azure Cosmos DBの欠陥によりプラットフォーム全体のキーが露出し、任意のデータベースにアクセス可能だった問題](https://thehackernews.com/2026/07/azure-cosmos-db-flaw-exposed-platform.html) | 20.0 | 20.0 | 42.0 |
| [Discern Security、Series Aで1300万ドルを調達](https://www.securityweek.com/discern-security-raises-13-million-in-series-a-funding/) | 20.0 | 20.0 | 42.0 |
| [Cantinaがステルスから登場、800万ドルの資金調達を実施](https://www.securityweek.com/cantina-emerges-from-stealth-with-8-million-in-funding/) | 20.0 | 20.0 | 42.0 |
| [CISAが新たなSBOMベースラインを設定](https://www.helpnetsecurity.com/2026/07/30/cisa-sbom-guidance-updated/) | 20.0 | 20.0 | 42.0 |
| [CosmosEscape：Azure Cosmos DBのすべてのデータベースを乗っ取る手法](https://www.wiz.io/blog/cosmosescape-taking-over-every-database-in-azure-cosmos-db) | 20.0 | 20.0 | 42.0 |
| [Cyber extortionists、英国教育省からデータを窃取](https://therecord.media/united-kingdom-ransomware-education) | 20.0 | 20.0 | 42.0 |
| [CISAガイドが連邦機関によるオープンソースソフトウェアの安全かつ効果的な利用を支援](https://www.cisa.gov/news-events/news/cisa-guide-helps-federal-agencies-securely-and-effectively-use-open-source-software) | 20.0 | 20.0 | 42.0 |
| [Department for Educationへのサイバー攻撃で校長データがアクセスされる](https://www.itpro.com/security/data-breaches/head-teacher-data-accessed-in-department-for-education-cyber-attack) | 20.0 | 20.0 | 42.0 |
| [Analog Devicesがデータ侵害を公表](https://www.securityweek.com/semiconductor-firm-analog-devices-discloses-data-breach/) | 20.0 | 20.0 | 42.0 |
| [Russian spiesがZimbraからOutlookへ拡大した半クリックメール攻撃](https://www.theregister.com/security/2026/07/30/russian-spies-take-their-half-click-email-attack-from-zimbra-to-outlook/5281033) | 20.0 | 20.0 | 42.0 |
| [データセンター資産の5分の1は攻撃者の容易な標的にある](https://www.securityweek.com/1-in-5-data-center-assets-are-within-easy-reach-of-attackers/) | 20.0 | 20.0 | 42.0 |
| [北朝鮮の精鋭ハッカーが自国政府に反旗を翻し、摘発された](https://www.bitdefender.com/en-us/blog/hotforsecurity/north-korea-hackers-own-government) | 20.0 | 20.0 | 42.0 |
| [Google、Chromeの370件の脆弱性を修正するパッチを公開](https://www.infosecurity-magazine.com/news/google-patches-370-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [30以上のミネソタ州の水道事業体を襲った協調サイバー攻撃](https://www.helpnetsecurity.com/2026/07/30/minnesota-water-utilities-coordinated-cyberattack/) | 20.0 | 20.0 | 42.0 |
| [NCSC、ネットワーク機器に「フォレンジック可観測性」の組み込みを呼びかけ](https://www.infosecurity-magazine.com/news/ncsc-calls-device-manufacturers/) | 20.0 | 20.0 | 42.0 |
| [米国と同盟国がSBOMガイダンスを更新](https://www.securityweek.com/us-and-allies-update-sbom-guidance/) | 20.0 | 20.0 | 42.0 |

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
