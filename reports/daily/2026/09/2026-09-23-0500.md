# 📡 サイレーダー 2026-09-23 05:00 JST

このレポートは、2026-09-22 17:00 JST〜2026-09-23 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 101
- [音声で扱う想定のトピック](#audio-topics): 10
- [GitHubのみ掲載想定のトピック](#github-only-topics): 2
- [低温だが記録しておくトピック](#low-record-topics): 64

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2025-20333: Cisco ASA/FTD persistence mechanism update](#topic-203) | 58.0 | 74.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [Attacker compromised nearly 1000 Zyxel switches since August (CVE-2026-7273)](#topic-33740) | 46.0 | 46.0 | 55.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [Spraying in the Andes: TeamFiltration Returns to Exploit Forgotten Service Accounts](#topic-33781) | 46.0 | 41.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [D-Link warns of max severity zero-day bug in DIR-822A routers](#topic-33799) | 44.0 | 56.0 | 52.0 | 音声 | 温度感上位枠 |
| 5 | [Check Point Warns of Management Server Zero-Day Exploited in Targeted Attacks](#topic-33757) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 6 | [New CVSS 10.0 VeloCloud Orchestrator Flaw Actively Exploited in Certificate-Based Setups](#topic-33802) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 7 | [ShinyHunters claims FBI hack, data theft in PeopleSoft zero-day breach](#topic-33755) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 8 | [NightmareEclipse's latest zero-day leaves Microsoft Defender stuck in the past](#topic-33769) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 9 | [Volexity spots another China-aligned threat group exploiting Chrome and Microsoft defects](#topic-31075) | 36.0 | 46.0 | 59.0 | GitHub | 音声枠上限によりGitHubのみ |
| 10 | [The Closed Quorum: Inside the first reported autonomous AI C2 implant](#topic-33831) | 35.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 11 | [Introducing CAIRN: Frontier tracking for AI-integrated malware](#topic-33832) | 35.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 12 | [New ClosedQuorum Windows malware uses AI for attack decisions](#topic-33758) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-203"></a>

### 1. CVE-2025-20333: Cisco ASA/FTD persistence mechanism update

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 58.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

CiscoのSecure Firewall ASA/FTDに関連するCVE-2025-20333について、CISAとCiscoが更新情報を出しています。
公開情報によると、以前の侵害に使われた可能性がある脆弱性として扱われており、修正済みリリースへ更新しても残る可能性のある永続化の仕組みが論点になっています。
境界装置での侵害が長期化すると、認証情報の窃取や内部侵入の足がかりになりやすいためです。
特に、更新後も残存しうる要素が示されている点は、通常のパッチ適用だけで安心できないことを意味します。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 7 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Cisco ASA/FTDの対象機器について、現行の修正済みリリース適用状況とCISA/Ciscoの追加対応指針を確認する。
- 更新後も不審な設定変更や管理系アクセスの痕跡が残っていないか、監査ログと構成を点検する。
- 影響が疑われる環境では、単なるアップデートだけでなく、ベンダー推奨の調査・封じ込め手順を優先する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2023-20198 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2025-20333 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2025-20362 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2025-20393 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-20333](https://nvd.nist.gov/vuln/detail/CVE-2025-20333) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CSuite Targets US and EU Organizations with Device-Code Phishing and Remote Acce](https://any.run/cybersecurity-blog/csuite-attack-analysis/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [OctLurk and SilkLurk: newly identified tailored backdoors in cyber-espionage cam](https://securelist.com/octlurk-silklurk-backdoors-central-asia/120840/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [US Threat Landscape Alert: 30 Active Malware Families Ranked by Real Sandbox Dat](https://any.run/cybersecurity-blog/usa-top-30-threats-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [From edge appliance to enterprise compromise: Multi-stage Linux intrusion via F5](https://www.microsoft.com/en-us/security/blog/2026/05/22/from-edge-appliance-to-enterprise-compromise-multi-stage-linux-intrusion-via-f5-and-confluence/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Continued Evolution of Persistence Mechanism Against Cisco Secure Firewall Adapt](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-persist-CISAED25-03) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Weekly Report: JPCERT/CCが「Cisco ASAおよびFTDにおける複数の脆弱性（CVE-2025-20333、CVE-2025-2036](https://www.jpcert.or.jp/wr/2026/wr260430.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: Cisco ASAおよびFTDにおける複数の脆弱性（CVE-2025-20333、CVE-2025-20362）に関する注意喚起  (更新)](https://www.jpcert.or.jp/at/2025/at250021.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-33781"></a>

### 2. Spraying in the Andes: TeamFiltration Returns to Exploit Forgotten Service Accounts

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>i⁠O⁠S</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 46.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 41.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Proofpointは、TeamFiltrationを用いたMicrosoft 365への認証試行キャンペーンを確認し、ラテンアメリカの複数テナントで5,700超のアカウントが対象になったと報告しました。
確認された侵害は、利用実態のないサービスアカウントに集中しており、未変更の既定パスワードやMFA未設定が背景にあった可能性が示されています。
人の利用を前提にしていないサービスアカウントは見落とされやすく、攻撃者にとって突破口になりやすいことを示しています。
クラウドID基盤では、パスワード管理とMFAの適用範囲が被害の分岐点になり得ます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 技術詳細により影響確認が進みやすい。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 未使用・休眠状態のサービスアカウントを棚卸しし、所有者・用途・最終利用日を明確にする。
- サービスアカウントにもMFAや条件付きアクセスを適用できるか確認し、少なくとも認証強度を見直す。
- 既定値のまま残ったパスワードや長期未変更の資格情報を洗い出し、定期ローテーションと無効化の運用を徹底する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Proofpoint | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Mozilla | 言及あり | 0.80 | — |
| ベンダー | Amazon Web Services | 言及あり | 0.80 | — |
| 製品 | Microsoft Office | 言及あり | 0.80 | — |
| 製品 | Microsoft Teams | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| 製品 | Microsoft Azure | 言及あり | 0.80 | — |
| 製品 | Ivanti Policy Secure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Spraying in the Andes: TeamFiltration Returns to Exploit Forgotten Service Accou](https://www.proofpoint.com/us/blog/threat-insight/Spraying-in-the-Andes-TeamFiltration-Returns) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-33799"></a>

### 3. D-Link warns of max severity zero-day bug in DIR-822A routers

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>P⁠o⁠C</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 44.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 52.0 |

#### 概要

D-Linkが、旧型のDIR-822AデュアルバンドWi-Fiルーターに影響する重大な脆弱性CVE-2026-86296について注意喚起しました。
公開されているPoCコードの存在が示されており、現時点では修正パッチは案内されていないとされています。
家庭や小規模環境で使われる可能性があるルーターに関するため、影響範囲が個別のPCより広くなり得ます。公開PoCがある状態では、未対策機器が狙われるリスクに備える必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- DIR-822Aの利用有無を確認し、該当機器があれば監視対象に入れる。
- ベンダーからの更新情報や回避策の案内を継続確認する。
- インターネット公開されている管理機能や不要な機能の有無を見直し、必要最小限の露出にする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-86296 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-86296](https://nvd.nist.gov/vuln/detail/CVE-2026-86296) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [D-Link warns of max severity zero-day bug in DIR-822A routers](https://www.bleepingcomputer.com/news/security/d-link-warns-of-max-severity-zero-day-bug-in-dir-822a-routers/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-33757"></a>

### 4. Check Point Warns of Management Server Zero-Day Exploited in Targeted Attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

Check Pointは、Security Management Serverに存在するゼロデイ脆弱性「CVE-2026-93616」が、7月23日に限られた標的型攻撃で悪用されたと警告しました。
公開情報によると、この問題はサーバー上のWebサービスにアクセスできる場合に認証なしでスクリプトを実行される可能性があり、同社は9月22日に修正を提供しています。
ファイアウォールポリシーを管理する中枢サーバーに関わるため、影響が及ぶと防御設定や運用の信頼性に直結します。
すでに悪用観測があるため、該当製品を使う組織では早急な確認と対処が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Check Point Security Management Serverの利用有無と、該当する修正版適用状況を確認する。
- 管理用Webサービスへの到達範囲を見直し、不要な公開や制限不足がないか点検する。
- ベンダーの案内に従い、侵害の兆候確認とログ保全を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-93616 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Check Point | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-93616](https://nvd.nist.gov/vuln/detail/CVE-2026-93616) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Check Point Warns of Management Server Zero-Day Exploited in Targeted Attacks](https://thehackernews.com/2026/09/check-point-warns-of-management-server.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Check Point warns of Management Server zero-day exploited in attacks](https://www.bleepingcomputer.com/news/security/check-point-patches-management-server-zero-day-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33802"></a>

### 5. New CVSS 10.0 VeloCloud Orchestrator Flaw Actively Exploited in Certificate-Based Setups

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

Aristaは、オンプレミス版VeloCloud Orchestrator（VCO）に存在する新たな脆弱性CVE-2026-93952について、実際の悪用を確認したとしています。
対象は、Edgeの認証に証明書を使う構成のVCOで、リモートの攻撃者が内部機能に不正にアクセスし、ホストに影響を与える可能性があるとされています。
CVSS 10.0とされる深刻な脆弱性で、しかも悪用観測があるため、該当環境では優先的な確認が必要です。
SD-WANの管理基盤に関わるため、影響がネットワーク運用全体へ波及する可能性があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 自組織のVeloCloud Orchestratorがオンプレミス構成かつ証明書ベース認証かを確認する。
- ベンダーの案内や修正パッチ、回避策の有無を確認し、適用計画を早めに立てる。
- VCO関連の監査ログや管理操作の記録を点検し、不審な挙動がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-93952 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-93952](https://nvd.nist.gov/vuln/detail/CVE-2026-93952) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [New CVSS 10.0 VeloCloud Orchestrator Flaw Actively Exploited in Certificate-Base](https://thehackernews.com/2026/09/new-cvss-100-velocloud-orchestrator.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33755"></a>

### 6. ShinyHunters claims FBI hack, data theft in PeopleSoft zero-day breach

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

ShinyHuntersが、Oracle PeopleSoftのゼロデイ脆弱性を悪用してFBIのシステムに侵入し、内部サービスへのアクセスや職員・応募者に関するデータの窃取を行ったと主張しています。
現時点では、この主張の真偽や被害範囲の詳細は公開情報だけでは断定できません。
政府機関に関わるとされる事案であり、認証系や人事系のような機微な情報を含む可能性があるため、注目されています。
ゼロデイの悪用主張が出ている点は、関連製品を利用する組織にとって早急な確認と監視強化の必要性を示します。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Oracle PeopleSoftの利用有無を確認し、該当バージョンや公開情報に基づく注意喚起を点検する。
- 人事・応募者情報など機微情報を扱うシステムのアクセスログと異常な操作を重点的に確認する。
- ベンダー公表の修正情報や暫定対策が出ていないかを継続監視し、適用可能な対策を優先する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Oracle | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ShinyHunters claims FBI hack, data theft in PeopleSoft zero-day breach](https://www.bleepingcomputer.com/news/security/shinyhunters-claims-fbi-hack-data-theft-in-peoplesoft-zero-day-breach/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33769"></a>

### 7. NightmareEclipse's latest zero-day leaves Microsoft Defender stuck in the past

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Microsoft Defenderに関するゼロデイ脆弱性が取り上げられており、製品自体は動作していても更新が適用できなくなる可能性が示されています。
公開情報では悪用観測ありとされており、保護機能の鮮度低下につながる点が懸念されています。
セキュリティ製品の更新が妨げられると、既知の脅威に対する防御力が短期間で低下するおそれがあります。エンドポイント防御の前提を揺るがすため、運用面の影響が大きい विषयです。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Microsoft Defenderの定義ファイルやエンジン更新状態を確認し、更新失敗がないか監視する。
- 対象環境で検知の遅れがないか、他の防御層や補完策の有無を点検する。
- ベンダーの修正情報や緩和策の案内を確認し、適用計画を早めに検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [NightmareEclipse's latest zero-day leaves Microsoft Defender stuck in the past](https://www.theregister.com/security/2026/09/22/nightmareeclipses-latest-zero-day-leaves-microsoft-defender-stuck-in-the-past/5298320) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33831"></a>

### 8. The Closed Quorum: Inside the first reported autonomous AI C2 implant

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Cisco Talosの報告によると、CLOSEDQUORUMと呼ばれるマルウェアは、攻撃者の継続的な操作なしにコマンド＆コントロール（C2）を自律的に行う挙動を示したとされています。
これは、攻撃チェーンの一部がAIの関与で自動化される可能性を示す事例として注目されています。
攻撃の一部が自律化すると、攻撃者の作業負担が下がり、検知や対処の時間的余裕が短くなるおそれがあります。
AIを悪用した脅威の実例として、監視やインシデント対応の前提を見直す材料になります。

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

- 自律的なC2や不自然な通信パターンを前提に、EDR/NDRの検知ルールを見直す。
- 未知の実行ファイルや外向き通信の監視を強化し、通常業務と異なる挙動を早期に把握する。
- AI関連の脅威事例として、SOCやCSIRT向けの共有・教育資料に反映する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | DeepSeek | 言及あり | 0.80 | — |
| ベンダー | Mistral AI | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Meta | 言及あり | 0.80 | — |
| ベンダー | Qwen | 言及あり | 0.80 | — |
| 製品 | Mozilla Firefox | 言及あり | 0.80 | — |
| 製品 | Ivanti Policy Secure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [The Closed Quorum: Inside the first reported autonomous AI C2 implant](https://blog.talosintelligence.com/the-closed-quorum-inside-the-first-reported-autonomous-ai-c2-implant/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-33832"></a>

### 9. Introducing CAIRN: Frontier tracking for AI-integrated malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Cisco Talosは、AIを組み込んだマルウェアの発見・分類・追跡を支援する研究用ツールキット「CAIRN」を公開するとしています。
AI活用型の脅威が新たに広がる中で、こうした観測・分析の枠組みを整える動きとして注目されています。
生成AIの利用が攻撃側にも広がる可能性があるため、検知や分類の手法を早期に整備する意義があります。
脅威インテリジェンスの観点でも、未知の挙動を継続的に追跡する基盤として関心を集めやすい話題です。

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

- AI関連の不審サンプルについて、既存の検知ルールだけでなく分類・追跡の観点でも確認体制を見直す。
- AI利用の有無にかかわらず、マルウェアの振る舞い・通信・実行時の特徴を継続的に観測できる運用を意識する。
- ベンダーや研究機関の発信する新しい分析手法を、脅威評価や教育資料の更新に反映する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Anthropic | 言及あり | 0.80 | — |
| ベンダー | DeepSeek | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Ivanti Policy Secure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Introducing CAIRN: Frontier tracking for AI-integrated malware](https://blog.talosintelligence.com/introducing-cairn-frontier-tracking-for-ai-integrated-malware/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-33758"></a>

### 10. New ClosedQuorum Windows malware uses AI for attack decisions

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

ClosedQuorumと呼ばれる新しいWindows向けマルウェアが、侵害後の段階で次に取る行動を判断するために複数のAIモデルを利用していると報じられています。
対象としてGoogle Gemini、DeepSeek、Qwen、Mistralが挙げられており、攻撃の一部意思決定を自動化する点が特徴とされています。
攻撃側がAIを組み込むことで、侵害後の判断や運用の自動化が進む可能性があるため、従来型の検知・対応だけでは追随しにくくなる懸念があります。
AIを悪用したマルウェアの具体例として、今後の脅威評価や対策検討の参考になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 侵害後の横展開や追加行動を前提に、EDR/ログ監視で不審なプロセス連鎖や異常な外向き通信を確認する。
- AI関連の話題に引きずられず、実際の検知観点は挙動ベースで整理し、既存のインシデント対応手順を見直す。
- 関連情報が初期段階のため、追加の一次情報やベンダー見解を確認し、過度な一般化を避ける。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Mistral AI | 言及あり | 0.80 | — |
| ベンダー | DeepSeek | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Qwen | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New ClosedQuorum Windows malware uses AI for attack decisions](https://www.bleepingcomputer.com/news/security/new-closedquorum-windows-malware-uses-ai-for-attack-decisions/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-33740"></a>

### 1. Attacker compromised nearly 1000 Zyxel switches since August (CVE-2026-7273)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 46.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

CVE-2026-7273は、Zyxel GS1900シリーズのスイッチに影響する脆弱性として報告され、すでに修正済みとされていますが、実際の悪用が確認されているとされています。
公開情報によれば、未対策機器を狙った活動により、複数国の多数の機器が影響を受けた可能性があります。
ネットワーク機器は社内通信の要所にあるため、侵害されると認証情報や通信の保護に広く影響し得ます。CISAのKEV掲載は、優先度を上げて対応すべき脆弱性であることを示しています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Zyxel GS1900シリーズの利用有無を確認し、該当機器があれば修正適用状況を点検する。
- インターネットや外部から到達可能な管理インターフェースがないか見直し、不要なら遮断する。
- 機器の設定変更履歴や不審なアクセス兆候を確認し、必要に応じて認証情報の見直しを行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-7273 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Veeam | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-7273](https://nvd.nist.gov/vuln/detail/CVE-2026-7273) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Attacker compromised nearly 1000 Zyxel switches since August (CVE-2026-7273)](https://www.helpnetsecurity.com/2026/09/22/zyxel-switches-cve-2026-7273-vulnerability-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zyxel and Veeam Flaws Under Active Exploitation With Command and SYSTEM Access](https://thehackernews.com/2026/09/zyxel-and-veeam-flaws-under-active.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA orders feds to patch Zyxel flaw exploited for data theft](https://www.bleepingcomputer.com/news/security/cisa-orders-feds-to-patch-actively-exploited-zyxel-flaw-by-thursday/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-31075"></a>

### 2. Volexity spots another China-aligned threat group exploiting Chrome and Microsoft defects

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

Volexityは、ChromeとMicrosoftの脆弱性を組み合わせた侵害活動について、別の中国寄りとみられる脅威グループの関与を指摘しました。
関連するChromeの脆弱性CVE-2026-85046は、既に実際の攻撃で悪用されたことが公表されており、Googleは修正版を配布しています。
既知の脆弱性が実際の攻撃に使われているため、単なる注意喚起ではなく優先度の高い対処が必要です。複数の脅威グループで同種の悪用が見られる点から、影響範囲が広がる可能性があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Chromeを最新版へ早急に更新し、展開状況を確認する。
- CISAの既知悪用脆弱性カタログや社内の優先度付けに基づき、関連端末の対応を前倒しする。
- ChromeやMicrosoft製品に関する異常な挙動、未説明のプロセス起動、ブラウザ経由の不審なアクセスを重点的に監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-85046 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-85880 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-87491 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Chromium | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-85046](https://nvd.nist.gov/vuln/detail/CVE-2026-85046) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Volexity spots another China-aligned threat group exploiting Chrome and Microsof](https://cyberscoop.com/volexity-uta0565-china-exploit-chain-chrome-microsoft/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Chinese espionage groups swarm to exploit triple-link chain of zero-days](https://cyberscoop.com/china-espionage-groups-exploit-chain-zero-days/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google patches actively exploited Chrome zero-day (CVE-2026-85046)](https://www.helpnetsecurity.com/2026/09/04/google-chrome-zero-day-cve-2026-85046/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/09/04/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [AIを使って次の動きを選ぶマルウェアを研究者が発見](https://www.helpnetsecurity.com/2026/09/22/cairn-open-source-framework-ai-malware-closedquorum/) | 33.0 | 20.0 | 42.0 |
| [本物のGoogleサインインを悪用して高額な未検証AIサブスクリプションを販売する詐欺師たち](https://www.helpnetsecurity.com/2026/09/22/fake-ai-subscription-sites-google-sign-in/) | 33.0 | 20.0 | 42.0 |
| [Shai-Hulud攻撃でCrowdSecのGitHubデータに被害](https://www.darkreading.com/cyberattacks-data-breaches/shai-hulud-attack-cyber-firm-crowdsec-github-data) | 28.0 | 45.0 | 42.0 |
| [悪意あるnpmパッケージindexed-btree、削除前にランタイムコードへローダーを隠蔽](https://thehackernews.com/2026/09/malicious-npm-package-indexed-btree-hid.html) | 28.0 | 45.0 | 42.0 |
| [ShinyHunters、Clopランサムウェアの競合をハッキングしたと主張](https://www.itpro.com/security/ransomware/cyber-criminal-groups-suffer-from-the-same-security-weaknesses-they-routinely-exploit-shinyhunters-claims-it-hacked-clop-ransomware-rival) | 28.0 | 30.0 | 42.0 |
| [Elsevierドメインが一時的に乗っ取られ、LAPSUS$の「Chapter II」ページへリダイレクトされた件](https://www.helpnetsecurity.com/2026/09/22/elsevier-domains-hijack-lapsus/) | 28.0 | 20.0 | 48.0 |
| [中国系ハッカーに悪用されているZyXELスイッチの最近の脆弱性](https://www.securityweek.com/recent-zyxel-switch-vulnerability-exploited-by-chinese-hackers/) | 28.0 | 20.0 | 42.0 |
| [悪意あるB-treeのNPMパッケージが数百万回ダウンロードを蓄積](https://www.securityweek.com/malicious-b-tree-npm-package-accumulates-millions-of-downloads/) | 28.0 | 20.0 | 42.0 |
| [日本、米国や同盟国が広範なスキームを明らかにする中で北朝鮮のラップトップファームを初摘発](https://www.securityweek.com/japan-dismantles-first-north-korean-laptop-farm-as-us-and-allies-detail-wider-scheme/) | 28.0 | 20.0 | 42.0 |
| [MetaのMuse AIアシスタントにMacバックドア化のゼロデイ脆弱性](https://www.malwarebytes.com/blog/bugs/2026/09/metas-muse-ai-assistant-has-a-zero-day-that-can-turn-it-into-a-mac-backdoor) | 27.0 | 20.0 | 43.0 |
| [無料でひとりでは無く複数人のチームで使うことができるAIエージェント「OneCLI」、オープンソースでセルフホスト可能](https://gigazine.net/news/20260922-onecli/) | 27.0 | 20.0 | 42.0 |
| [継続する不正事案の中で現実味を帯びるAI安全性をめぐる議論](https://www.darkreading.com/cyber-risk/rogue-incidents-debate-ai-safety-gets-real) | 25.0 | 20.0 | 42.0 |
| [Bifrost AI Gatewayの致命的な脆弱性により認証なしでコマンド実行が可能に](https://thehackernews.com/2026/09/critical-bifrost-ai-gateway-flaw-lets.html) | 25.0 | 20.0 | 42.0 |
| [Z.ai、コード収集を巡って謝罪しZCodeをオープンソース化](https://www.theregister.com/security/2026/09/22/zai-says-sorry-for-slurping-up-your-code-open-sources-zcode/5298300) | 25.0 | 20.0 | 42.0 |
| [Microsoftによる「Eviltokens」AIチャットボットの摘発後、英国で2人を逮捕](https://therecord.media/two-arrested-in-uk-after-microsoft-takedown-eviltokens) | 25.0 | 20.0 | 42.0 |
| [保険業界、AI関連サイバー保険請求の方針を明確化](https://www.cybersecuritydive.com/news/insurance-sector-begins-to-offer-clarity-on-ai-related-cyber-claims/831028/) | 25.0 | 20.0 | 42.0 |
| [中国を引き合いに、トランプ大統領がAI規制への不介入姿勢を一段と強調](https://cyberscoop.com/trump-hands-off-ai-regulation-china-race/) | 25.0 | 20.0 | 42.0 |
| [そのAIエージェントに承認を出したのは誰か？誰もいない？やっぱりね。](https://www.theregister.com/security/2026/09/22/sponsored/5297693) | 25.0 | 20.0 | 42.0 |
| [小売業者はシャドーAIを抑制する一方でエージェント型AIの拡大管理に苦戦](https://www.cybersecuritydive.com/news/retail-ai-agents-visibility-data-breaches-netskope/831002/) | 25.0 | 20.0 | 42.0 |
| [AIは防御側よりも攻撃者を大きく利すると英国当局者が指摘](https://therecord.media/ai-set-to-help-attackers-more-than-defenders) | 25.0 | 20.0 | 42.0 |
| [AI導入に対して遅れるインシデント対応体制、ISACAが指摘](https://www.infosecurity-magazine.com/news/orgs-lack-ai-incident-response/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントが横方向移動のルールを書き換える理由](https://thehackernews.com/2026/09/ai-agents-are-rewriting-rules-of.html) | 25.0 | 20.0 | 42.0 |
| [最新のディープフェイク事情がCISOに多くの懸念をもたらす](https://www.helpnetsecurity.com/2026/09/22/cisos-deepfake-incidents-social-engineering-survey/) | 25.0 | 20.0 | 42.0 |
| [Agent連携で拡大するWIN AIエコシステム](https://www.wiz.io/blog/wiz-mcp-agent-integrations) | 25.0 | 20.0 | 42.0 |
| [産業組織の3分の1超がサイバーセキュリティリスクを成長の最大障害と認識、調査で判明](https://www.darkreading.com/cyber-risk/third-industrial-orgs-see-cybersecurity-risk-top-obstacle) | 25.0 | 20.0 | 42.0 |
| [AIが後押しするボットおよびAPI脅威の急増](https://www.infosecurity-magazine.com/news/ai-drives-surge-in-bot-and-api/) | 25.0 | 20.0 | 42.0 |
| [サイバー部門は限界に達しつつあり、AIも負担軽減にほとんど役立っていない](https://www.itpro.com/security/rising-threats-and-under-resourcing-for-cybersecurity-is-taking-a-toll-on-the-people-tasked-with-managing-it-cyber-teams-are-being-pushed-to-breaking-point-and-ai-is-doing-little-to-alleviate-strain) | 25.0 | 20.0 | 42.0 |
| [研究者がClaudeを使ってOpenAIをハッキング](https://www.malwarebytes.com/blog/news/2026/09/researchers-used-claude-to-hack-openai) | 25.0 | 20.0 | 42.0 |
| [CISOはマルチモーダルディープフェイクに備えインシデント対応プレイブックを更新すべきとGartnerが警告](https://www.infosecurity-magazine.com/news/update-incident-response/) | 25.0 | 20.0 | 42.0 |
| [Siemens WTV676およびWTV776の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-265-08) | 24.0 | 46.0 | 50.0 |
| [Microsoftが当初スプーフィングと分類したSharePointの脆弱性、認証済みRCEを可能にする](https://thehackernews.com/2026/09/sharepoint-flaw-initially-listed-as.html) | 24.0 | 46.0 | 50.0 |
| [WordPressの「Click2Shell」脆弱性を修正](https://www.securityweek.com/wordpress-patches-click2shell-vulnerability/) | 24.0 | 38.0 | 42.0 |
| [ResearcherがMicrosoft Defenderの更新を妨害するBigDiskBusterのゼロデイPoCを公開](https://thehackernews.com/2026/09/researcher-drops-bigdiskbuster-zero-day.html) | 24.0 | 20.0 | 43.0 |
| [EvilTokensの正体解明：デバイスコードフィッシングの実態に迫る](https://www.microsoft.com/en-us/security/blog/2026/09/22/unmasking-eviltokens-getting-to-the-root-of-device-code-phishing/) | 22.0 | 20.0 | 48.0 |
| [トラフィックログのどこかで、ボットがただ見ているだけではない](https://www.helpnetsecurity.com/2026/09/22/ai-crawler-traffic-online-stores/) | 22.0 | 20.0 | 43.0 |
| [Windows Defenderのゼロデイ脆弱性によりMicrosoftのウイルス対策更新がブロックされる](https://www.bleepingcomputer.com/news/security/new-windows-defender-zero-day-blocks-microsoft-antivirus-updates/) | 22.0 | 20.0 | 43.0 |
| [OpenPLC Runtime v3の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-265-09) | 21.0 | 34.0 | 50.0 |
| [悪意のあるnpmパッケージがTwilioのバグバウンティ調査を装い、認証情報を窃取可能にする](https://thehackernews.com/2026/09/malicious-npm-package-poses-as-twilio.html) | 20.0 | 45.0 | 42.0 |
| [Siemens Siveillance Controlの脆弱性と対策](https://www.cisa.gov/news-events/ics-advisories/icsa-26-265-03) | 20.0 | 28.0 | 50.0 |
| [lwIP TCP/IP StackのMQTTクライアントアプリケーション](https://www.cisa.gov/news-events/ics-advisories/icsa-26-265-01) | 20.0 | 28.0 | 50.0 |
| [lwIP（Lightweight IP）における脆弱性と対策](https://www.cisa.gov/news-events/ics-advisories/icsa-26-265-02) | 20.0 | 28.0 | 50.0 |
| [新たなLinuxカーネルの脆弱性によりARM64 KVMゲストがホストメモリへの読み書きアクセスを取得可能に](https://thehackernews.com/2026/09/new-linux-kernel-flaw-gives-arm64-kvm.html) | 20.0 | 28.0 | 50.0 |
| [WordPressが一部サーバーでコード実行を可能にする重大な脆弱性を修正するパッチを公開](https://thehackernews.com/2026/09/wordpress-issues-patch-for-critical.html) | 20.0 | 20.0 | 42.0 |
| [BigCommerceのデータがRibon Appsの侵害で流出](https://www.securityweek.com/bigcommerce-data-stolen-via-ribon-apps-hack/) | 20.0 | 20.0 | 42.0 |
| [ShinyHuntersがFBIへの侵害を主張、「これは金銭目的ではない」](https://www.theregister.com/security/2026/09/22/shinyhunters-claims-fbi-hack-this-is-not-financially-motivated/5298385) | 20.0 | 20.0 | 42.0 |
| [WazuhでシャドーITの可視性ギャップを削減する方法](https://www.bleepingcomputer.com/news/security/reducing-shadow-it-visibility-gaps-with-wazuh/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、12,000件の侵害に関連するEvilTokensのデバイスコードフィッシングサービスを停止](https://thehackernews.com/2026/09/microsoft-takes-down-eviltokens-device.html) | 20.0 | 20.0 | 42.0 |
| [F5 BIG-IP APMに存在する緊急の脆弱性](https://cert.europa.eu/publications/security-advisories/2026-013/) | 20.0 | 20.0 | 42.0 |
| [AV-ComparativesのEPRテストでSES Completeが認証リーダーに認定](https://www.security.com/feature-stories/ses-complete-certified-leader-av-comparatives-epr-test) | 20.0 | 20.0 | 42.0 |
| [安価なスマートグラスに潜む重大なセキュリティ問題](https://www.malwarebytes.com/blog/news/2026/09/some-cheap-smart-glasses-are-a-security-disaster) | 20.0 | 20.0 | 42.0 |
| [英国警察がEvilTokensの容疑者2人を逮捕、Microsoftが50のフィッシングキットサイトを差し押さえ](https://www.theregister.com/security/2026/09/22/uk-cops-arrest-2-eviltokens-suspects-microsoft-seizes-50-phishing-kit-websites/5298317) | 20.0 | 20.0 | 42.0 |
| [EvilTokensのPhaaS、12,000件のMicrosoftアカウント侵害後に停止](https://www.bleepingcomputer.com/news/security/eviltokens-phaas-disrupted-after-compromising-12-000-microsoft-accounts/) | 20.0 | 20.0 | 42.0 |
| [Microsoftとパートナーが金融詐欺向けの包括的なサイバー犯罪サービスEvilTokensを阻止](https://cyberscoop.com/microsoft-eviltokens-cybercrime-service-takedown/) | 20.0 | 20.0 | 42.0 |
| [NCSCがサイバー防御へのエージェント活用を提唱、企業が受け入れるべき「不都合な真実」](https://www.itpro.com/security/ncsc-talks-up-agents-for-cyber-defense-but-theres-an-inconvenient-truth-businesses-need-to-accept) | 20.0 | 20.0 | 42.0 |
| [Cyeraが4億ドルを調達、企業価値は120億ドル超に到達](https://www.securityweek.com/cyera-raises-400-million-at-12-billion-valuation/) | 20.0 | 20.0 | 42.0 |
| [北朝鮮の攻撃者が3万台の端末を侵害し、1070万ドルを窃取](https://www.infosecurity-magazine.com/news/north-korean-waterplum-30000/) | 20.0 | 20.0 | 42.0 |
| [Nightmare Eclipseが身元を明かした後に新たなMicrosoft Defenderのエクスプロイトを公開](https://www.securityweek.com/nightmare-eclipse-drops-new-microsoft-defender-exploit-after-revealing-identity/) | 20.0 | 20.0 | 42.0 |
| [ロシアのインターネット遮断が接近するドローン攻撃の警告を妨害](https://therecord.media/russia-internet-shutdowns-disrupt-warnings-about-drone-attacks) | 20.0 | 20.0 | 42.0 |
| [OTネットワークセグメントの完全分離率は13％にとどまる分析](https://www.securityweek.com/only-13-of-ot-network-segments-are-fully-isolated-analysis/) | 20.0 | 20.0 | 42.0 |
| [次の知的財産窃取犯はCEOのように聞こえるかもしれない](https://www.helpnetsecurity.com/2026/09/22/csc-online-intellectual-property-risk-report/) | 20.0 | 20.0 | 42.0 |
| [エージェント型企業を統制するBeyond Identity](https://www.akamai.com/blog/security/2026/sep/beyond-identity-governing-the-agentic-enterprise) | 20.0 | 20.0 | 42.0 |
| [ネットワーク分割の不備が企業の攻撃対象領域を拡大している](https://www.infosecurity-magazine.com/news/segmentation-failures-expanding/) | 20.0 | 20.0 | 42.0 |
| [DORA施行2年目：SOCは実際に攻撃を可視化できるか](https://thehackernews.com/2026/09/dora-year-two-can-your-soc-actually-see.html) | 20.0 | 20.0 | 42.0 |
| [水道システムに新たな懸念、インフォスティーラーによる情報漏えい](https://cyberscoop.com/spycloud-study-water-utilities-infostealer-exposure/) | 20.0 | 20.0 | 42.0 |

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
