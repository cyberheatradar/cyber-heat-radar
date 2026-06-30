# 📡 サイレーダー 2026-07-01 05:00 JST

このレポートは、2026-06-30 17:00 JST〜2026-07-01 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 96
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 63

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CISA: Windows BlueHammer flaw now exploited by ransomware gangs](#topic-20211) | 47.0 | 60.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [Oracle E-Business Suite Payments flaw under attack (CVE-2026-46817)](#topic-20074) | 45.0 | 56.0 | 56.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [Nissan Discloses Employee Data Breach Linked to Oracle Zero-Day](#topic-20128) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Nissan employee data exposed in Oracle PeopleSoft zero-day attacks](#topic-20126) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [BlueHammer Vulnerability Exploited in Ransomware Attacks](#topic-1324) | 35.0 | 88.0 | 78.0 | 音声 | 温度感上位枠 |
| 6 | [Securing AI agents: When AI tools move from reading to acting](#topic-20129) | 35.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 7 | [Langflow RCE Exploited to Deploy Monero Miner on Exposed AI App Endpoints](#topic-20130) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 8 | [SimpleHelp vulnerability exploited to deliver mighty Djinn Stealer (CVE-2026-48558)](#topic-20187) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-20211"></a>

### 1. CISA: Windows BlueHammer flaw now exploited by ransomware gangs

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 47.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 60.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、Microsoft Defenderに関係する権限昇格の脆弱性「BlueHammer」が、ランサムウェア समूहによって悪用されていると確認したとされています。
これまでゼロデイ攻撃で使われていた文脈もあり、継続的な悪用リスクが注目されています。
権限昇格の脆弱性は、侵入後に被害を拡大させる足がかりになりやすく、ランサムウェア被害の深刻化につながります。
公的機関が悪用観測を示している点から、優先度を上げて確認すべき案件です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Microsoft Defender関連の更新状況と影響範囲を確認し、適用漏れがないか点検する。
- 権限昇格の兆候や不審な管理者権限取得の痕跡がないか、監査ログを確認する。
- ランサムウェア対策として、バックアップの分離保管と復旧手順の再点検を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA: Windows BlueHammer flaw now exploited by ransomware gangs](https://www.bleepingcomputer.com/news/security/cisa-windows-bluehammer-flaw-now-exploited-by-ransomware-gangs/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20128"></a>

### 2. Nissan Discloses Employee Data Breach Linked to Oracle Zero-Day

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

日産は、Oracle PeopleSoft のゼロデイ脆弱性に関連した攻撃キャンペーンを通じて、従業員データが流出したと公表しました。
公開情報ベースでは、今回の件は個別企業への被害報告であり、ゼロデイ悪用の文脈で注目されています。
ゼロデイ脆弱性が実際の情報流出につながった可能性が示されており、利用中の業務システムの緊急確認が必要になるためです。
人事・従業員情報のような機微データが対象になると、二次被害や対応負荷も大きくなります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Oracle PeopleSoft を含む関連システムについて、ベンダー情報と適用可能な修正・回避策の有無を確認する。
- 従業員情報を扱う周辺システムのアクセス権、監査ログ、異常な通信や認証失敗の有無を点検する。
- 対象システムを利用していない場合でも、同種のゼロデイ悪用キャンペーンを前提に監視・脆弱性管理の優先度を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-35273 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Nissan Discloses Employee Data Breach Linked to Oracle Zero-Day](https://www.infosecurity-magazine.com/news/nissan-oracle-peoplesoft-zero-day/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20126"></a>

### 3. Nissan employee data exposed in Oracle PeopleSoft zero-day attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

日産に関連する従業員データが、Oracle PeopleSoftのゼロデイ攻撃により露出したと報じられています。
現時点で確認できる範囲では、同社は現従業員・元従業員に対し、銀行関連のパスワード変更とフィッシングメールへの警戒を呼びかけています。
人事・給与などの従業員情報は、なりすましやフィッシングに悪用されやすく、組織外への影響も広がりやすい分野です。
ゼロデイ攻撃が絡むため、既知の対策だけでは十分でない可能性があり、早期の確認と注意喚起が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- PeopleSoftなど業務基盤の脆弱性情報を継続監視し、影響有無を速やかに確認する。
- 従業員向けに、銀行口座情報や認証情報の変更・確認を促し、フィッシング警戒を再周知する。
- 人事・給与系データに関するアクセス権限、ログ監視、異常送信の検知体制を点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Nissan employee data exposed in Oracle PeopleSoft zero-day attacks](https://www.itpro.com/security/data-breaches/nissan-employee-data-exposed-in-oracle-peoplesoft-zero-day-attacks) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-1324"></a>

### 4. BlueHammer Vulnerability Exploited in Ransomware Attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 88.0 |
| <nobr>確⁠度</nobr> | 78.0 |

#### 概要

CVE-2026-33825は、Microsoft Defenderにおけるアクセス制御の粒度不足に関する脆弱性とされ、認証済みの攻撃者がローカルで権限を昇格できる可能性があります。
公開情報では、ランサムウェア攻撃の文脈で悪用が観測されたとされ、CISAのKnown Exploited Vulnerabilitiesにも掲載されています。
防御製品そのものに関わる脆弱性であり、端末や管理環境の権限悪用につながるおそれがあるため、影響範囲の確認が重要です。
すでに実悪用が示唆されているため、通常の脆弱性より優先度を上げて対応を検討する必要があります。

#### CISA KEV詳細

- **CVE**: CVE-2026-33825
- **Vendor / Project**: Microsoft
- **Product**: Defender
- **Vulnerability Name**: Microsoft Defender Insufficient Granularity of Access Control Vulnerability
- **Date Added**: 2026-04-22
- **Due Date**: 2026-05-06
- **Known Ransomware Use**: Known

**Required Action**

> Apply mitigations per vendor instructions, follow applicable BOD 22-01 guidance for cloud services, or discontinue use of the product if mitigations are unavailable.

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- CISA KEV関連。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 悪用情報あり。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- PoC/検証コード候補: 候補あり（該当CVE 1件 / URL 1件以上）。
- 直接PoCリンク: 掲載しません。
- 注意: 対象CVE・製品・バージョンとの一致確認が必要です。

#### 担当者向け確認ポイント

- Microsoft Defenderの該当バージョン・構成を特定し、修正状況を確認する。
- CISA KEV掲載の有無を踏まえ、パッチ適用や緩和策を優先度高く進める。
- 権限昇格や不審な管理操作の痕跡がないか、端末・管理ログを点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-33825 | 関連CVE | 1.00 |
| ベンダー | Microsoft | 影響ベンダー | 1.00 |
| 製品 | Defender | 影響製品 | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-33825](https://nvd.nist.gov/vuln/detail/CVE-2026-33825) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>公的機関</nobr> | [CISA KEV: CVE-2026-33825](https://www.cisa.gov/known-exploited-vulnerabilities-catalog?field_cve=CVE-2026-33825) | <nobr>KEV掲載内容、Date Added、Due Date、Required Action</nobr> |
| <nobr>公的機関データ</nobr> | [CISA KEV JSON](https://www.cisa.gov/sites/default/files/feeds/known_exploited_vulnerabilities.json) | <nobr>CISA公式の機械可読データ。CVE IDで検索して確認</nobr> |
| <nobr>出典</nobr> | [BlueHammer Vulnerability Exploited in Ransomware Attacks](https://www.securityweek.com/bluehammer-vulnerability-exploited-in-ransomware-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20129"></a>

### 5. Securing AI agents: When AI tools move from reading to acting

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>A⁠I</nobr> / <nobr>M⁠C⁠P</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoft Security Blogは、AIエージェントが「読む」だけでなく外部ツールを「実行する」段階に入ることで、信頼していたツール記述が悪用されるリスクを取り上げています。
記事では、MCPに関連するツールポイズニングにより、AIエージェントが意図しない操作を行い、データ損失につながり得る点が示されています。
AIエージェントの利用が広がるほど、単なる情報参照ではなく実行権限の扱いが重要になります。
ツール連携の設計や監視が不十分だと、正規機能を起点にした不正操作の影響が大きくなり得ます。

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

- AIエージェントに与えるツール権限を最小化し、実行系操作は明確な承認や分離を設ける。
- ツール説明やメタデータの信頼前提を見直し、変更検知やレビューの仕組みを入れる。
- エージェントの実行ログと異常なツール呼び出しを監視し、想定外の操作を早期に検知できるようにする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Securing AI agents: When AI tools move from reading to acting](https://www.microsoft.com/en-us/security/blog/2026/06/30/securing-ai-agents-ai-tools-move-from-reading-acting/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-20130"></a>

### 6. Langflow RCE Exploited to Deploy Monero Miner on Exposed AI App Endpoints

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、AIアプリ基盤のLangflowに存在する未認証のリモートコード実行脆弱性が悪用され、Moneroマイナーの配布に使われているとされています。
対象は外部に公開されたAIアプリのエンドポイントで、攻撃者が露出した環境を継続的に探索している可能性が示されています。
AI関連の業務アプリや開発基盤が、暗号資産マイニングを含む侵害の入口になり得る点が注目されます。
認証なしで実行される脆弱性は、公開範囲の広い環境ほど被害につながりやすいため、早急な確認が重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Langflowを含むAIアプリ基盤の公開状況を確認し、不要なインターネット露出を減らす。
- 該当バージョンや脆弱性情報を確認し、ベンダーの修正や回避策を適用する。
- リソース使用量の急増や不審なプロセス、予期しない外向き通信がないか監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-33017 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Langflow RCE Exploited to Deploy Monero Miner on Exposed AI App Endpoints](https://thehackernews.com/2026/06/langflow-rce-exploited-to-deploy-monero.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20187"></a>

### 7. SimpleHelp vulnerability exploited to deliver mighty Djinn Stealer (CVE-2026-48558)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>A⁠I</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

SimpleHelp RMMの認証回避の脆弱性CVE-2026-48558が、修正後も攻撃に悪用されていると報告されています。
攻撃では、新たに確認されたDjinn Stealerが配布され、Windows、macOS、Linux環境を対象に各種認証情報や開発・運用系の情報を狙うとされています。
RMM製品は管理対象が広いため、1件の脆弱性が複数端末や運用基盤に波及する可能性があります。
クラウドやソース管理、AI開発支援ツールに関する認証情報が狙われる点も、被害の範囲を広げやすい要因です。

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

- SimpleHelpの該当バージョン利用有無を確認し、ベンダー案内に沿って速やかに修正・更新する。
- RMM経由の不審な認証失敗、未承認の操作、配布物の変化などを重点的に監視する。
- 端末だけでなく、クラウド、ソース管理、SSH、ウォレット関連の資格情報の保護と再発行手順を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-48558 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [SimpleHelp vulnerability exploited to deliver mighty Djinn Stealer (CVE-2026-485](https://www.helpnetsecurity.com/2026/06/30/simplehelp-vulnerability-exploited-cve-2026-48558/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-20074"></a>

### 1. Oracle E-Business Suite Payments flaw under attack (CVE-2026-46817)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 56.0 |

#### 概要

Oracle E-Business Suite の決済機能に関する脆弱性 CVE-2026-46817 について、実環境での悪用が確認されたと複数の情報源が伝えています。
対象は Oracle Payments における権限管理や認証の不備とされ、CVSS 9.8 の深刻な問題として扱われています。
業務基盤として使われる可能性がある E-Business Suite に関わるため、影響範囲が大きくなり得ます。
公開PoCや悪用情報が出ている点から、修正適用の遅れがそのまま侵害リスクにつながりやすい状況です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
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

#### 攻撃・悪用観測シグナル

- シグナル種別: 公開PoC・検証コード言及あり。
- 公開PoC/Exploitコード: 確認あり。
- 直接PoCリンク: 掲載しません。
- 確認方針: NVD、ベンダー公式、公的機関、信頼できる技術分析を優先し、GitHub等のコードは防御・検証目的で別途確認します。

#### 担当者向け確認ポイント

- Oracle E-Business Suite の該当バージョンとパッチ適用状況を優先確認する。
- 外部公開された管理・決済関連の入口がないか、不要な露出を見直す。
- 侵害兆候の有無を監視し、関連ログや認証イベントを重点的に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-46817 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-46817](https://nvd.nist.gov/vuln/detail/CVE-2026-46817) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Oracle E-Business Suite Payments flaw under attack (CVE-2026-46817)](https://www.helpnetsecurity.com/2026/06/30/oracle-payments-cve-2026-46817-exploitation/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Oracle E-Business Suite Flaw CVE-2026-46817 Actively Exploited in the Wild](https://thehackernews.com/2026/06/oracle-e-business-suite-flaw-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [ランサム被害から復活したアスクル、AI駆動開発でゼロから基盤を再構築](https://xtech.nikkei.com/atcl/nxt/column/18/03664/062900004/) | 29.0 | 30.0 | 42.0 |
| [Edge拡張機能119件からマルウェア、260万人に影響か](https://news.mynavi.jp/techplus/article/20260630-4647101/) | 29.0 | 20.0 | 42.0 |
| [Huntress CEO、脅威ハンターがランサムウェア犯罪者に捜査情報を警告した件で「判断ミス」と認める](https://www.theregister.com/security/2026/06/30/huntress-ceo-says-threat-hunter-used-poor-judgment-in-alerting-ransomware-crim-about-law-enforcement-probe/5264532) | 28.0 | 30.0 | 42.0 |
| [BYOVDの流行：攻撃者が信頼されたWindowsドライバを武器化してセキュリティを無効化する方法](https://www.security.com/threat-intelligence/byovd-vulnerable-drivers) | 28.0 | 30.0 | 42.0 |
| [BlackfieldランサムウェアがNidec Corporationに200万ドルの身代金を要求](https://www.bleepingcomputer.com/news/security/blackfield-ransomware-asks-nidec-corporation-for-2-million-ransom/) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア組織が企業風の組織運営を武器化する手口](https://cyberscoop.com/ransomware-syndicates-corporate-organization-op-ed/) | 28.0 | 30.0 | 42.0 |
| [EU・アジアの宿泊業組織でフィッシャーが永続化を獲得](https://www.darkreading.com/cyberattacks-data-breaches/phishers-persistence-eu-asia-hospitality-orgs) | 28.0 | 20.0 | 42.0 |
| [Rustで再構築されたRustDuckボットネットがルーターとサーバーを乗っ取りDDoSに悪用](https://thehackernews.com/2026/06/rustduck-botnet-rebuilds-in-rust-to.html) | 28.0 | 20.0 | 42.0 |
| [Silent Swap Crypto Clipper、偽のGoogle Notes拡張機能を使ってウォレットアドレスを置き換え](https://thehackernews.com/2026/06/silent-swap-crypto-clipper-uses-fake.html) | 28.0 | 20.0 | 42.0 |
| [SimpleHelpの深刻な脆弱性がマルウェア配布に悪用される](https://www.infosecurity-magazine.com/news/simplehelp-rmm-vulnerability/) | 28.0 | 20.0 | 42.0 |
| [SimpleHelpの重大な脆弱性が機密資格情報を狙う攻撃で悪用される](https://www.cybersecuritydive.com/news/critical-flaw-simplehelp-exploited-attacks-credentials/824105/) | 28.0 | 20.0 | 42.0 |
| [Aikido Security、Rootを買収しオープンソース脆弱性のバックポート修正を拡充](https://www.helpnetsecurity.com/2026/06/30/aikido-security-root-acquisition/) | 28.0 | 20.0 | 42.0 |
| [ClickFixがサイバー犯罪者に好まれるマルウェア配布手法に](https://www.infosecurity-magazine.com/news/clickfix-cybercriminals-favorite/) | 28.0 | 20.0 | 42.0 |
| [FIFA 2026のサイバーリスクが示す数値分析](https://thehackernews.com/2026/06/what-numbers-say-about-fifa-2026-cyber.html) | 28.0 | 20.0 | 42.0 |
| [ハッカーがBlockchainを悪用し、Booking.comのフィッシングで日本のホテルを標的にする](https://www.infosecurity-magazine.com/news/hackers-blockchain-japan-hotels/) | 28.0 | 20.0 | 42.0 |
| [中国関連マルウェアを運ぶUSBドライブが日本の軍事ネットワークに約1年間感染させていた](https://www.bitdefender.com/en-us/blog/hotforsecurity/usb-drives-carrying-china-linked-malware-infected-japanese-military-networks-for-nearly-a-year) | 28.0 | 20.0 | 42.0 |
| [ToddyCat：隠されたメールアシスタントの実態 第2部](https://securelist.com/toddycat-apt-umbrij-tool-and-oauth/120251/) | 28.0 | 20.0 | 42.0 |
| [AirDropとQuick Shareの脆弱性により近隣の攻撃者がクラッシュや検証回避を引き起こせる問題](https://thehackernews.com/2026/06/airdrop-and-quick-share-flaws-let.html) | 28.0 | 20.0 | 42.0 |
| [Nissan従業員データがOracle PeopleSoftの侵害で流出](https://www.securityweek.com/nissan-employee-data-breached-in-oracle-peoplesoft-hack/) | 28.0 | 20.0 | 42.0 |
| [Microsoft Securityの最新情報：2026年6月](https://www.microsoft.com/en-us/security/blog/2026/06/30/whats-new-in-microsoft-security-june-2026/) | 27.0 | 20.0 | 42.0 |
| [Microsoft、毒されたMCPツール説明でAIエージェントがデータ漏えいする恐れを警告](https://thehackernews.com/2026/06/microsoft-warns-poisoned-mcp-tool.html) | 25.0 | 20.0 | 42.0 |
| [GuardFallがオープンソースAIコーディングエージェントを古いシェルインジェクションの脆弱性にさらす](https://thehackernews.com/2026/06/guardfall-exposes-open-source-ai-coding.html) | 25.0 | 20.0 | 42.0 |
| [282件のiOS向けAIアプリでAPIキーとOpenAIプロキシアクセスがネットワーク通信から漏えいしていることが判明](https://thehackernews.com/2026/06/282-ios-apps-found-leaking-llm-api-keys.html) | 25.0 | 20.0 | 42.0 |
| [JamfがMac向けにAIガバナンスとシャドーAI検知を提供](https://www.helpnetsecurity.com/2026/06/30/jamf-enables-ai-governance-and-shadow-ai-detection-on-mac/) | 25.0 | 20.0 | 42.0 |
| [OpenMatter NetworkがAIガバナンスに検証可能な信頼をもたらす](https://www.helpnetsecurity.com/2026/06/30/openmatter-network-cryptographically-verifiable-platform/) | 25.0 | 20.0 | 42.0 |
| [数十年前のBashの手口がAIコーディングエージェントをサプライチェーン攻撃にさらす](https://www.securityweek.com/decades-old-bash-tricks-expose-ai-coding-agents-to-supply-chain-attacks/) | 25.0 | 20.0 | 42.0 |
| [AI生成ワークフローは静かなセキュリティ危機です](https://www.darkreading.com/cyber-risk/ai-generated-workflows-silent-security-disaster) | 25.0 | 20.0 | 42.0 |
| [Train, triage, repeat: フィッシング対策を変えるAIエージェント](https://redcanary.com/blog/threat-detection/phishing-ai-agent/) | 25.0 | 20.0 | 42.0 |
| [Schneider Electric EcoStruxure IT Data Center Expertの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-181-03) | 25.0 | 20.0 | 42.0 |
| [Apple、AIセキュリティ懸念でソフトウェア修正を迅速化](https://www.itpro.com/software/apple-is-speeding-up-software-updates-due-to-ai-security-concerns-heres-what-you-need-to-know) | 25.0 | 20.0 | 42.0 |
| [AIのトークンコストがサイバーセキュリティを脅かす理由](https://www.securityweek.com/the-ai-token-costs-that-can-break-cybersecurity/) | 25.0 | 20.0 | 42.0 |
| [AIブラウザをだましてユーザー認証情報を漏えいさせる新たなBioShocking攻撃](https://thehackernews.com/2026/06/new-bioshocking-attack-tricks-ai.html) | 25.0 | 20.0 | 42.0 |
| [StoneFly Storage Concentratorの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-181-06) | 24.0 | 46.0 | 50.0 |
| [Schneider Electric EasyLogic T150およびSaitel DP RTUの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-181-04) | 24.0 | 46.0 | 50.0 |
| [Delta Electronics DVP12SE PLC の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-181-07) | 24.0 | 46.0 | 50.0 |
| [Frangoteam FUXA SCADA/HMIの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-181-02) | 24.0 | 46.0 | 50.0 |
| [OFFIS DCMTK Toolkitの脆弱性とセキュリティ対策](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-181-01) | 24.0 | 46.0 | 50.0 |
| [Oracle E-Business Suiteの最新脆弱性の悪用が始まる](https://www.securityweek.com/exploitation-of-recent-oracle-e-business-suite-vulnerability-begins/) | 24.0 | 38.0 | 42.0 |
| [量子安全移行の加速](https://www.microsoft.com/en-us/security/blog/2026/06/30/microsoft-advances-quantum-safe-security-as-the-risk-timeline-shifts/) | 22.0 | 20.0 | 42.0 |
| [中国のオープンウェイトモデル「GLM-5.2」が脆弱性検出ベンチマークでClaude Codeを上回る](https://gigazine.net/news/20260630-glm-5-2-beats-claude-cyber-benchmarks/) | 22.0 | 20.0 | 42.0 |
| [人口ゼロの孤島から送られたDMCA申請により記事がGoogleのインデックスから削除される](https://gigazine.net/news/20260630-pollen-google-dmca/) | 22.0 | 20.0 | 42.0 |
| [本の雑誌社のXアカウントが乗っ取り被害 - 注意を呼びかけ](https://www.security-next.com/186570) | 22.0 | 20.0 | 42.0 |
| [アフラック契約者サイトなどで顧客約438万人の個人情報が流出](https://www.security-next.com/186597) | 22.0 | 20.0 | 42.0 |
| [労働力調査の調査世帯一覧表を紛失 - 栃木県](https://www.security-next.com/186510) | 22.0 | 20.0 | 42.0 |
| [iOS/iPadOS 26.5.2提供開始、多数の不具合修正 macOSアップデートも](https://news.mynavi.jp/techplus/article/20260630-4647496/) | 21.0 | 20.0 | 42.0 |
| [アフラック生命保険に不正アクセス、438万人分の個人情報漏洩](https://xtech.nikkei.com/atcl/nxt/news/24/03280/) | 21.0 | 20.0 | 42.0 |
| [XZ Utilsの脆弱性がB&R製品に与える影響](https://www.cisa.gov/news-events/ics-advisories/icsa-26-181-05) | 20.0 | 28.0 | 50.0 |
| [Mitsubishi Electric MELSOFT Update Manager SW1DND-UDM-Mの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-181-01) | 20.0 | 28.0 | 50.0 |
| [Chrome Web Store上の偽Perplexity拡張機能が検索を追跡](https://www.bleepingcomputer.com/news/security/fake-perplexity-extension-on-chrome-web-store-tracked-searches/) | 20.0 | 20.0 | 42.0 |
| [DHS、重要インフラのサイバーセキュリティ向け後継評議会を発表へ](https://cyberscoop.com/dhs-anchor-ci-cybersecurity-information-sharing/) | 20.0 | 20.0 | 42.0 |
| [Apple、iOS・macOS Tahoe・Safari向けにセキュリティ更新を公開](https://www.malwarebytes.com/blog/news/2026/06/update-time-apple-releases-security-patches-for-ios-macos-tahoe-safari) | 20.0 | 20.0 | 42.0 |
| [DHSが官民のインフラセキュリティ連携のための新システムを提案](https://www.cybersecuritydive.com/news/critical-infrastructure-collaboration-dhs-anchor-ci/824081/) | 20.0 | 20.0 | 42.0 |
| [地下社会からの教訓：Business Email Compromiseへの対策方法](https://www.bleepingcomputer.com/news/security/lessons-from-the-underground-how-to-combat-business-email-compromise/) | 20.0 | 20.0 | 42.0 |
| [Microsoft 365のハードニングとHuntress Managed ISPM](https://www.huntress.com/blog/microsoft-365-identity-security-five-minute-admin) | 20.0 | 20.0 | 42.0 |
| [Aflac Japanのデータ侵害、438万人に影響](https://www.securityweek.com/aflac-japan-data-breach-impacts-4-38-million/) | 20.0 | 20.0 | 42.0 |
| [Hacker Conversations: Chris Thompson、元IBM X-Force Red責任者でRemoteThreat共同創業者](https://www.securityweek.com/hacker-conversations-chris-thompson-former-head-of-ibm-x-force-red-co-founder-of-remotethreat/) | 20.0 | 20.0 | 42.0 |
| [最高裁、携帯電話利用者の位置情報履歴にも憲法上のプライバシー保護が適用されると判断](https://www.securityweek.com/supreme-court-rules-constitutional-privacy-protections-apply-to-cellphone-users-location-history/) | 20.0 | 20.0 | 42.0 |
| [保険大手Aflac、子会社への不正アクセス後にデータ侵害を公表](https://www.bleepingcomputer.com/news/security/insurance-giant-aflac-discloses-data-breach-after-subsidiary-hack/) | 20.0 | 20.0 | 42.0 |
| [米国メーカーがサプライヤーのセキュリティギャップを解消し、第三者リスクを半減してSOCトリアージ速度を2倍にした方法](https://any.run/cybersecurity-blog/us-manufacturer-security-risk/) | 20.0 | 20.0 | 42.0 |
| [US、SignalとWhatsApp攻撃の背後にいるロシア関連ハッカーの情報に1000万ドルの報奨金を提示](https://www.itpro.com/security/cyber-crime/us-offers-usd10m-bounty-for-info-on-russia-linked-hackers-behind-signal-and-whatsapp-attacks) | 20.0 | 20.0 | 42.0 |
| [英国の医療分野でサイバー攻撃が10倍に増加](https://www.infosecurity-magazine.com/news/uk-healthcare-tenfold-increase/) | 20.0 | 20.0 | 42.0 |
| [Kali Linux 2026.2、VM起動時間を短縮しデスクトップ環境を刷新](https://www.helpnetsecurity.com/2026/06/30/kali-linux-2026-2-release/) | 20.0 | 20.0 | 42.0 |
| [Claude Fable 5とAI支援型サードパーティリスクの新たな現実](https://www.bitsight.com/de/blog/claude-fable-5-und-die-neue-realitaet-von-ki-gestuetztem-drittparteirisiko) | 10.0 | 20.0 | 42.0 |

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
