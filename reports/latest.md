# 📡 サイレーダー 2026-06-19 05:01 JST

このレポートは、2026-06-18 17:00 JST〜2026-06-19 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 99
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 68

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Microsoft working on a fix for RoguePlanet, a flaw that grants full PC control](#topic-17871) | 48.0 | 58.0 | 59.0 | 音声 | 温度感上位枠 |
| 2 | [DragonForce Hackers Abuse Microsoft Teams Relays to Hide Backdoor.Turn C2 Traffic](#topic-18165) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [CVE-2026-20253: CISA KEV catalog addition](#topic-17163) | 35.0 | 64.0 | 55.0 | 音声 | 温度感上位枠 |
| 4 | [消費者の60％がブランドメッセージに「AI」という言葉が含まれていると敬遠する](#topic-18205) | 35.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [ThreatsDay Bulletin: Claude Chat Abuse, NastyC2 npm Packages, Device-Code Phishing + 25 More Stories](#topic-18146) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [Scripting the disassembler: Local agentic reverse engineering through vbdec’s live COM object model](#topic-18215) | 30.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-17871"></a>

### 1. Microsoft working on a fix for RoguePlanet, a flaw that grants full PC control

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 48.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

Microsoft Defenderの脆弱性「RoguePlanet」について、修正パッチを準備していることが公表され、CVE-2026-50656として管理されています。
報告では権限昇格につながる問題とされており、影響が大きい可能性があるため注目されています。セキュリティ製品側の脆弱性は、端末防御の前提そのものに関わるため、見過ごせません。
修正が提供されるまでの間は、影響範囲の把握と対応準備が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Microsoftの更新情報を確認し、Defender関連の修正適用可否を早めに確認する。
- 影響を受ける可能性のあるWindows端末を棚卸しし、優先度を付けて監視する。
- 不審な権限昇格やDefender関連の異常挙動がないか、検知ルールとログを点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-33825 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-41091 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-45498 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-50656 | 関連CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-50656](https://nvd.nist.gov/vuln/detail/CVE-2026-50656) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Microsoft working on a fix for RoguePlanet, a flaw that grants full PC control](https://www.malwarebytes.com/blog/news/2026/06/microsoft-working-on-a-fix-for-rogueplanet-a-flaw-that-grants-full-pc-control) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Confirms RoguePlanet Defender Zero-Day, Says Patch is in Development](https://thehackernews.com/2026/06/microsoft-confirms-rogueplanet-defender_02022423645.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft working on patch for RoguePlanet Defender zero-day (CVE-2026-50656)](https://www.helpnetsecurity.com/2026/06/17/rogueplanet-zero-day-cve-2026-50656/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補あり（URL 3件以上 / 該当CVE 3件）。

---

<a id="topic-18165"></a>

### 2. DragonForce Hackers Abuse Microsoft Teams Relays to Hide Backdoor.Turn C2 Traffic

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

DragonForceに関連するとみられる攻撃者が、カスタムのGo製RAT「Backdoor.Turn」を使い、Microsoft Teamsのリレー基盤内にC2通信を紛れ込ませていたと報告されています。
Broadcom傘下のSymantecとCarbon Blackの分析では、これが米国の大手サービス企業を標的にした事例として確認されたとされています。
正規サービスの通信経路を悪用してC2を隠す手法は、検知や調査を難しくするため注目されています。
ランサムウェア関連の活動として、侵入後の遠隔操作や横展開の兆候を見逃さない対策が重要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Microsoft Teamsを含む正規クラウドサービス経由の不審な通信を、通常の業務通信と分けて監視する。
- ランサムウェア関連の侵入後活動を想定し、EDRやネットワーク監視で未知のRATや異常な外向き通信を点検する。
- 大規模サービス利用環境では、認証情報の保護と特権アカウントの監査を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [DragonForce Hackers Abuse Microsoft Teams Relays to Hide Backdoor.Turn C2 Traffi](https://thehackernews.com/2026/06/dragonforce-hackers-abuse-microsoft.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17163"></a>

### 3. CVE-2026-20253: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

CISAは、Splunk Enterpriseに関するCVE-2026-20253をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
公開情報では、認証なしで不正なファイル操作やリモートコード実行につながるおそれがある重大な脆弱性として案内されており、Splunk側も修正版を公開しています。
KEV入りは、実際に悪用が確認された脆弱性として優先対応が求められることを意味します。
Splunkのような運用・監視基盤は影響範囲が広く、放置すると侵害時の被害が大きくなり得ます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
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

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Splunk Enterpriseの該当バージョンを利用していないか確認し、提供元の修正版適用状況を点検する。
- 外部公開された管理系インターフェースや関連サービスの露出状況を見直し、不要な公開がないか確認する。
- 侵害兆候の有無を確認し、監視ログや変更履歴を重点的に点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20253 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20253](https://nvd.nist.gov/vuln/detail/CVE-2026-20253) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/06/18/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Splunk Enterprise Flaw Lets Attackers Run Code Without Authentication](https://thehackernews.com/2026/06/critical-splunk-enterprise-flaw-lets.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補あり（URL 3件以上 / 該当CVE 1件）。

---

<a id="topic-18205"></a>

### 4. 消費者の60％がブランドメッセージに「AI」という言葉が含まれていると敬遠する

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

WordPress VIPが公開した調査レポートでは、ブランドメッセージに「AI」という言葉が含まれると、消費者の一部が敬遠する傾向が示されたとされています。
AI活用が広がる一方で、企業の伝え方や見せ方が受け手の印象に影響する可能性がある、という文脈の話題です。
AI関連の訴求は注目を集めやすい反面、過度に前面へ出すと逆効果になる可能性があり、広報やマーケティングの設計に影響します。
セキュリティやITの文脈でも、AI機能の説明や信頼性の伝え方を見直すきっかけになります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI機能を強調する際は、価値や安全性を具体的に伝え、単なる“AI推し”に見えないよう配慮する。
- 顧客向け説明では、AIの利用目的・データの扱い・制御可能性を明確にし、誤解を減らす。
- ブランド表現や製品紹介文が受け手にどう響くか、定期的にレビューする。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [消費者の60％がブランドメッセージに「AI」という言葉が含まれていると敬遠する](https://gigazine.net/news/20260618-ai-brand-visibility-research/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-18146"></a>

### 5. ThreatsDay Bulletin: Claude Chat Abuse, NastyC2 npm Packages, Device-Code Phishing + 25 More Stories

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

今週の脅威まとめでは、Claudeを含むAIチャットの悪用、npmパッケージを使った不正な配布、デバイスコード認証を狙うフィッシングなど、複数の攻撃手口が取り上げられています。
特定の単一インシデントというより、既存の正規機能や開発基盤を悪用する動きが横断的に目立つ内容です。
AIサービスや開発者向けエコシステムは利用範囲が広く、攻撃者にとっても接点になりやすいため、影響が複数の環境に波及し得ます。
運用・開発・認証の各面で、正規機能を前提にした防御だけでは不十分であることを示しています。

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

- AIチャットや連携機能で不審なリンク・添付・外部誘導がないか確認し、利用ルールを見直す。
- npmなどの依存関係は、配布元・更新頻度・権限を定期点検し、不要なパッケージを減らす。
- デバイスコード認証を含む認証フローは、ユーザー教育と監視を強化し、想定外の承認要求を検知できるようにする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ai_model_or_project | Claude | 主題 | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ThreatsDay Bulletin: Claude Chat Abuse, NastyC2 npm Packages, Device-Code Phishi](https://thehackernews.com/2026/06/threatsday-bulletin-claude-chat-abuse.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-18215"></a>

### 6. Scripting the disassembler: Local agentic reverse engineering through vbdec’s live COM object model

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Cisco Talosは、VB6逆コンパイラ/逆アセンブラのvbdecにライブなCOMインターフェースを用意し、ローカルのAIエージェントと従来の解析ツールを組み合わせる逆解析の手法を紹介しました。
AIを無理に組み込むのではなく、既存の解析結果を外部から扱える形にすることで、解析支援の自動化を進める考え方です。
脆弱性の話ではなく、逆解析やマルウェア分析の実務にAIをどう安全に組み込むかという設計面の話として注目されます。
ローカル環境で完結する分析フローの整理は、機密コードを扱う現場でも関心を集めやすいテーマです。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 既存の解析ツールにAIを足す際は、ツール内部改造よりも外部インターフェース連携のほうが運用しやすい場合がある。
- ローカルAIを使う構成でも、解析対象データや生成結果の取り扱い、ログ保全の方針は事前に整理しておく。
- 自動化の恩恵がある一方で、AIの出力は補助として扱い、最終判断は従来の手動検証で確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Scripting the disassembler: Local agentic reverse engineering through vbdec’s li](https://blog.talosintelligence.com/scripting-the-disassembler/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補なし。

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
| [ポスト量子対応への道 第1回/2：リスクを理解する](https://blog.nviso.eu/2026/06/18/the-road-to-post-quantum-readiness-part-1/) | 30.0 | 20.0 | 48.0 |
| [豪州の砂糖生産会社、ランサムウェア攻撃を受け復旧作業を進める](https://therecord.media/mackay-sugar-cyberattack-claimed-gentlemen) | 28.0 | 30.0 | 42.0 |
| [Malware攻撃でRoblox開発者がゲームを丸ごと失う被害](https://www.helpnetsecurity.com/2026/06/18/roblox-game-takeover-malware-attacks/) | 28.0 | 30.0 | 42.0 |
| [GentleKillerが48製品の400以上のセキュリティプロセスを標的にする](https://www.helpnetsecurity.com/2026/06/18/eset-gentlemen-edr-killers/) | 28.0 | 30.0 | 42.0 |
| [上場イスラエル企業に関連付けられた「Popa」ボットネット](https://krebsonsecurity.com/2026/06/popa-botnet-linked-to-publicly-traded-israeli-firm/) | 28.0 | 20.0 | 48.0 |
| [Nintendo、WebMD子会社へのサイバー攻撃でデータ流出を確認](https://www.bleepingcomputer.com/news/security/nintendo-confirms-data-stolen-in-webmd-subsidiary-cyberattack/) | 28.0 | 20.0 | 42.0 |
| [USBワームがWindowsショートカットファイル経由で暗号資産窃取マルウェアを拡散](https://www.bleepingcomputer.com/news/security/usb-worm-spreads-crypto-stealing-malware-via-windows-shortcut-files/) | 28.0 | 20.0 | 42.0 |
| [MicrosoftがUSBのLNKワームとTorベースのC2を使うWindows Clipperマルウェアキャンペーンの詳細を公表](https://thehackernews.com/2026/06/microsoft-details-windows-clipper.html) | 28.0 | 20.0 | 42.0 |
| [Law enforcementによるSocGholish対策で106台のサーバー停止、1万5000サイトをクリーンアップ](https://www.helpnetsecurity.com/2026/06/18/law-enforcement-socgholish-operation-endgame/) | 28.0 | 20.0 | 42.0 |
| [KlueのOAuth侵害と「Icarus」によるSalesforceデータ窃取攻撃との関連](https://www.bleepingcomputer.com/news/security/klue-oauth-breach-linked-to-icarus-salesforce-data-theft-attacks/) | 28.0 | 20.0 | 42.0 |
| [Evil Corpに関連するSocGholish感染サイト約1万5000件を警察が削除](https://www.bleepingcomputer.com/news/security/law-enforcement-nukes-socgholish-malware-from-nearly-15-000-sites/) | 28.0 | 20.0 | 42.0 |
| [Fortinet VPNの認証情報と設定データが7万3000台分流出した重大セキュリティ事案](https://www.bitsight.com/blog/security-alert-fortibleed-fortinet-vpn-credentials-firewall-exposed) | 28.0 | 20.0 | 42.0 |
| [FortinetとIvantiの脆弱性悪用でLATAMのインフラが被害を受ける](https://www.infosecurity-magazine.com/news/operation-escaneo-cloudsek-latam/) | 28.0 | 20.0 | 42.0 |
| [レトロゲームファンを狙う偽GitHubマルウェアの新たな標的化](https://www.malwarebytes.com/blog/threat-intel/2026/06/retro-gaming-fans-are-the-new-target-for-fake-github-malware) | 28.0 | 20.0 | 42.0 |
| [Rokarolla Banking Trojanが200のアプリケーションを標的にする](https://www.securityweek.com/rokarolla-banking-trojan-targets-200-applications/) | 28.0 | 20.0 | 42.0 |
| [独自の脆弱性ハーネスを構築する方法](https://blog.cloudflare.com/build-your-own-vulnerability-harness/) | 25.0 | 20.0 | 42.0 |
| [ネットワーク内に潜む隠れたアクセスリスクを見つける孤立したAIエージェント](https://thehackernews.com/2026/06/orphaned-ai-agents-how-to-find-hidden.html) | 25.0 | 20.0 | 42.0 |
| [偽のGitHubスターとAI動画で暗号資産クリッパーを隠蔽](https://www.infosecurity-magazine.com/news/crypto-clipboard-hijacker-fake/) | 25.0 | 20.0 | 42.0 |
| [セキュリティチームがより早く動き始める必要がある理由](https://www.rapid7.com/blog/post/it-why-security-teams-need-to-start-earlier) | 25.0 | 20.0 | 42.0 |
| [大統領のAIに関する大統領令はサイバーセキュリティについて多くを語っている](https://www.wiz.io/blog/ai-executive-order-cybersecurity) | 25.0 | 20.0 | 42.0 |
| [eSentire、Atlas PreemptでAI主導のペネトレーションテストとMDRを連携](https://www.helpnetsecurity.com/2026/06/18/esentire-links-ai-led-penetration-testing-with-mdr-through-atlas-preempt/) | 25.0 | 20.0 | 42.0 |
| [サイバー犯罪者もAIに仕事を奪われることを心配している](https://www.infosecurity-magazine.com/news/cybercriminals-worried-ai-take/) | 25.0 | 20.0 | 42.0 |
| [AI支援ソフトウェア開発における「vibe coding spectrum」アプローチ](https://www.ncsc.gov.uk/blogs/the-vibe-coding-spectrum-approach-to-ai-assisted-software-development) | 25.0 | 20.0 | 42.0 |
| [Schneider Electric Easergy、EcoStruxture、PowerLogic、Saitel製品に関する脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-169-07) | 25.0 | 20.0 | 42.0 |
| [Dream、3億ドルの評価額で2億6000万ドルを調達](https://www.securityweek.com/dream-raises-260-million-at-3-billion-valuation/) | 25.0 | 20.0 | 42.0 |
| [F5、NGINX Open Sourceのリモートコード実行につながる2件の重大な脆弱性を修正](https://thehackernews.com/2026/06/f5-patches-two-critical-nginx-open.html) | 24.0 | 46.0 | 50.0 |
| [Rockwell Automation FactoryTalk Historian Site Editionの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-169-03) | 24.0 | 46.0 | 50.0 |
| [AVer PTCカメラに関する脆弱性とセキュリティ情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-169-01) | 24.0 | 46.0 | 50.0 |
| [AtlassianとSplunkが重大な脆弱性を修正](https://www.securityweek.com/atlassian-splunk-patch-critical-vulnerabilities/) | 24.0 | 38.0 | 42.0 |
| [F5、NGINXの重大および高リスク脆弱性を修正](https://www.securityweek.com/f5-patches-critical-high-severity-nginx-vulnerabilities/) | 24.0 | 38.0 | 42.0 |
| [攻撃コード不要](https://www.securityweek.com/no-exploits-required/) | 23.0 | 23.0 | 43.0 |
| [Human Kindとの近接遭遇](https://blog.talosintelligence.com/close-encounters-of-the-human-kind/) | 22.0 | 20.0 | 48.0 |
| [Microsoft Securityを統合した顧客が124%のROIを得たことを示すForresterの新調査](https://www.microsoft.com/en-us/security/blog/2026/06/18/new-forrester-study-shows-customers-who-unified-with-microsoft-security-benefited-from-124-roi/) | 22.0 | 20.0 | 42.0 |
| [給付認定の通知書を誤送付、送付先リストを作成ミス - 福岡市](https://www.security-next.com/185632) | 22.0 | 20.0 | 42.0 |
| [新聞広告に誤った二次元コード、誘導先に個人情報 - 広島県](https://www.security-next.com/185699) | 22.0 | 20.0 | 42.0 |
| [患者情報含むUSBメモリが所在不明 - 長崎みなとメディカルセンター](https://www.security-next.com/185696) | 22.0 | 20.0 | 42.0 |
| [ShapedPluginの更新フローが侵害されWordPressサイトにマルウェアを感染させる](https://www.bleepingcomputer.com/news/security/shapedplugin-update-flow-hacked-to-infect-wordpress-sites/) | 20.0 | 30.0 | 42.0 |
| [AzeoTech DAQFactory の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-169-02) | 20.0 | 28.0 | 50.0 |
| [Apollo Pharmacy 血糖値モニタリングシステム APG-01 BT](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-169-01) | 20.0 | 28.0 | 50.0 |
| [Mitsubishi ElectricのMELSEC iQ-FシリーズFX5-ENET/IP Ethernetモジュール](https://www.cisa.gov/news-events/ics-advisories/icsa-26-169-06) | 20.0 | 28.0 | 50.0 |
| [Schneider Electric EasyLogic T150およびSaitel DPの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-169-04) | 20.0 | 28.0 | 50.0 |
| [Mitsubishi Electric MELSEC iQ-F Seriesの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-169-05) | 20.0 | 28.0 | 50.0 |
| [Operation Escaneoが示すラテンアメリカの脅威情勢の変化](https://www.darkreading.com/cybersecurity-operations/operation-escaneo-signals-shift-latam-threat-landscape) | 20.0 | 20.0 | 42.0 |
| [FIFAのバグによりワールドカップ配信がリモート乗っ取りの危険にさらされる](https://www.darkreading.com/application-security/fifa-bug-world-cup-streams-remote-takeover) | 20.0 | 20.0 | 42.0 |
| [インターネットからアクセス可能なREDCapサーバーの大半が旧版のままにされている](https://www.securityweek.com/majority-of-internet-accessible-redcap-servers-outdated/) | 20.0 | 20.0 | 42.0 |
| [Klue App侵害を通じたSalesforceデータ窃取の継続](https://www.darkreading.com/cyberattacks-data-breaches/salesforce-data-thefts-klue-app-compromise) | 20.0 | 20.0 | 42.0 |
| [ソフトウェア開発のスピード偏重がTeamPCPの混乱攻撃を招いた理由](https://cyberscoop.com/teampcp-breaks-open-source-software-trust-model/) | 20.0 | 20.0 | 42.0 |
| [Accentureが産業向けサイバーセキュリティ強化で3社を総額41.8億ドルで買収](https://cyberscoop.com/accenture-industrial-cybersecurity-acquisition-dragos-netrise-runzero/) | 20.0 | 20.0 | 42.0 |
| [[Virtual Event] データ侵害の全容：自社で起きたときに取るべき対応](https://www.darkreading.com/events/anatomy-of-a-data-breach-what-to-do-if-it-happens-to-you) | 20.0 | 20.0 | 42.0 |
| [Googleが研究者に「Nice catch!」と称賛も、未修正の脆弱性にバグバウンティを拒否](https://www.theregister.com/security/2026/06/18/google-told-researcher-nice-catch-then-denied-bug-bounty-for-flaw-it-still-hasnt-fixed/5258076) | 20.0 | 20.0 | 42.0 |
| [Princess of Wales事件を受けたICOの医療従事者への注意喚起](https://www.infosecurity-magazine.com/news/ico-cautions-healthcare-worker/) | 20.0 | 20.0 | 42.0 |
| [Microsoft 365のバックアップだけでは不十分な5つの理由](https://www.bleepingcomputer.com/news/security/5-reasons-microsoft-365-backup-isnt-enough-for-business-data-protection/) | 20.0 | 20.0 | 42.0 |
| [全銀協 AI脅威にATM停止など想定](https://news.yahoo.co.jp/pickup/6584758?source=rss) | 20.0 | 20.0 | 42.0 |
| [AccentureがDragosの過半数株式を取得し、runZeroとNetRiseを含む41億ドル規模のOTサイバーセキュリティ強化へ](https://www.securityweek.com/accenture-to-acquire-majority-stake-in-dragos-all-of-runzero-netrise-in-4-1-billion-ot-cybersecurity-push/) | 20.0 | 20.0 | 42.0 |
| [DNSは最も重要で、かつ最も誤設定されやすいセキュリティ制御です](https://www.akamai.com/blog/security/2026/jun/dns-most-critical-most-misconfigured-security-control) | 20.0 | 20.0 | 42.0 |
| [Security Debtを解消するためのエクスポージャー問題への対処](https://www.darkreading.com/cyber-risk/security-debt-tackle-exposure-problem) | 20.0 | 20.0 | 42.0 |
| [Apple、会話を盗聴される恐れのあるBeats Studio Budsの脆弱性を修正](https://www.bleepingcomputer.com/news/security/apple-fixes-beats-studio-buds-flaw-that-let-hackers-spy-on-conversations/) | 20.0 | 20.0 | 42.0 |
| [国家支援の敵対勢力が英国の重要施設を標的とした重大攻撃の大半に関与](https://www.cybersecuritydive.com/news/nation-state-rivals-linked-to-majority-of-consequential-attacks-targeting-c/823242/) | 20.0 | 20.0 | 42.0 |
| [Telegram、試験問題流出チャンネルを取り締まれなかったと認める――インド政府が法廷で主張](https://www.bleepingcomputer.com/news/security/telegram-admits-it-couldnt-police-exam-leak-channels-india-tells-court/) | 20.0 | 20.0 | 42.0 |
| [FortiBleedのデータ漏えいで74,000件のFortinet firewall認証情報が流出](https://www.helpnetsecurity.com/2026/06/18/fortinet-fortibleed-data-leak/) | 20.0 | 20.0 | 42.0 |
| [英国の重要インフラ攻撃の4分の3は敵対的国家によるもの](https://www.itpro.com/security/hostile-states-behind-three-quarters-of-uk-critical-infrastructure-attacks) | 20.0 | 20.0 | 42.0 |
| [F5、NGINXの重大な脆弱性に対する緊急パッチを公開](https://www.bleepingcomputer.com/news/security/f5-issues-out-of-band-patches-for-critical-nginx-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [Cisco ISEにおける重大なコマンド実行脆弱性の修正](https://www.securityweek.com/critical-command-execution-vulnerability-patched-in-cisco-ise/) | 20.0 | 20.0 | 42.0 |
| [KodakがShinyHuntersの漏えい脅迫期限到来で侵害を確認](https://www.malwarebytes.com/blog/news/2026/06/kodak-confirms-breach-as-shinyhunters-leak-threat-reaches-deadline) | 20.0 | 20.0 | 42.0 |
| [英国の重要インフラへのサイバー攻撃の75％は敵対国家によるものとNCSCが警告](https://www.infosecurity-magazine.com/news/hostile-states-cni-75-percent-ncsc/) | 20.0 | 20.0 | 42.0 |
| [SailPoint、Entroを約2億ドルで買収へ](https://www.securityweek.com/sailpoint-to-acquire-entro-in-reported-200-million-deal/) | 20.0 | 20.0 | 42.0 |
| [デジタル化の進展に伴いAPACでサイバー犯罪が急増](https://www.infosecurity-magazine.com/news/cybercrime-surges-apac-digitization/) | 20.0 | 20.0 | 42.0 |
| [FortiBleed漏えいでFortinet VPN認証情報7万3000台分が流出](https://www.bleepingcomputer.com/news/security/fortibleed-leak-exposes-fortinet-vpn-credentials-for-73-000-devices/) | 10.0 | 20.0 | 42.0 |

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
