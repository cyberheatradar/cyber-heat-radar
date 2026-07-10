# 📡 サイレーダー 2026-07-11 05:00 JST

このレポートは、2026-07-10 17:00 JST〜2026-07-11 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 85
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 53

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CISA Adds Two Known Exploited Vulnerabilities to Catalog](#topic-21929) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [JADEPUFFER: Agentic Ransomware Signals a New Era of AI-Driven Cyber Operations](#topic-21901) | 41.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [ランサムウェア交渉役・関係者に実刑判決](#topic-21785) | 39.0 | 30.0 | 57.0 | 音声 | 温度感上位枠 |
| 4 | [Destructive Windows backdoor stuffs multiple wipers and ransomware code into a single package](#topic-21886) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [GigaWiper Combines Multiple Malware for System-Level Sabotage](#topic-21958) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [‘HalluSquatting’ Turns AI Hallucinations Into Botnet Delivery Mechanism](#topic-21967) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-21929"></a>

### 1. CISA Adds Two Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、実際に悪用が確認されたとして、KEVカタログに2件の脆弱性を追加しました。
対象は iCagenda の CVE-2026-48939 と、Balbooa Forms の CVE-2026-56291 で、いずれも不適切なファイルアップロードに関する問題とされています。
KEVカタログへの追加は、当該脆弱性が現実の攻撃対象になっていることを示すため、対応優先度が高いと受け止められます。
特に公開されている資産や該当製品を使う環境では、早期の確認と修正が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当する iCagenda / Balbooa Forms の利用有無を棚卸しし、影響範囲を確認する。
- 公開資産を優先して、ベンダーの修正情報や緩和策を確認し、迅速に適用する。
- CISA の KEV 掲載を継続的に監視し、同様の実悪用が確認された項目を優先順位の高い対応対象にする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-48939 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-56291 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Two Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/07/10/cisa-adds-two-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21901"></a>

### 2. JADEPUFFER: Agentic Ransomware Signals a New Era of AI-Driven Cyber Operations

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者らは、JADEPUFFERと呼ばれるランサムウェア活動を、LLMを活用して複数の攻撃工程を自律的に進めた例として報告しました。
従来型の手動運用や既製マルウェアに依存する手口とは異なり、AIが攻撃の実行支援に使われた可能性が注目されています。
AIが攻撃の準備や運用を補助する形が現実の脅威として示された点が重要です。攻撃者の参入障壁が下がる懸念があり、防御側は従来の手口前提の対策だけでは不十分になる可能性があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 既知の脆弱性や不適切な設定の放置が、AI支援型の攻撃でも入口になり得るため、基本対策の棚卸しを優先する。
- 認証情報の保護と権限分離を再確認し、横展開や永続化を想定した監視を強化する。
- 異常な自動化や短時間での多段階操作を検知できるよう、ログ収集とアラート条件を見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [JADEPUFFER: Agentic Ransomware Signals a New Era of AI-Driven Cyber Operations](https://blog.polyswarm.io/jadepuffer-agentic-ransomware-signals-a-new-era-of-ai-driven-cyber-operations) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21785"></a>

### 3. ランサムウェア交渉役・関係者に実刑判決

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 57.0 |

#### 概要

米国で、ランサムウェア交渉に関わっていた元関係者に対し、実刑判決が言い渡されたと報じられています。
報道によれば、被害者側の立場で得た情報を外部の犯行グループに渡し、BlackCat/ALPHV関連の脅迫に関与したとされています。
被害対応や交渉の過程に信頼できるはずの関係者が混入すると、機密情報が漏えいし、交渉の安全性そのものが損なわれます。
ランサムウェア対応では、外部委託先や交渉窓口を含めた権限管理と監督の重要性が改めて示されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 交渉担当者やインシデント対応委託先の権限を最小限にし、アクセスログと職務分掌を厳格に管理する。
- 被害対応時に共有する情報を段階的に制限し、機密情報の取り扱いルールを事前に定める。
- 外部パートナーを含む対応プロセスに不自然な情報流通や利益相反の兆候がないか、監査可能な形で確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ランサムウェアグループ | BlackCat | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Third US Security Expert Sentenced to Prison for Helping Ransomware Gang](https://www.securityweek.com/third-us-security-expert-sentenced-to-prison-for-helping-ransomware-gang/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Working with the enemy: Ransomware negotiator-turned cyber criminal jailed after](https://www.itpro.com/security/ransomware/working-with-the-enemy-ransomware-negotiator-turned-cyber-criminal-jailed-after-working-with-hackers-to-extort-clients) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Former ransomware negotiator gets 4 years for BlackCat attacks](https://www.bleepingcomputer.com/news/security/us-ransomware-negotiator-gets-4-years-in-prison-for-blackcat-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Ransomware Negotiator Gets 70 Months in Prison for Aiding BlackCat Attacks](https://thehackernews.com/2026/07/ransomware-negotiator-gets-70-months-in.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Former DigitalMint ransomware negotiator who duped clients sentenced to 70 month](https://cyberscoop.com/digitalmint-ransomware-negotiator-angelo-martino-sentenced/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21886"></a>

### 4. Destructive Windows backdoor stuffs multiple wipers and ransomware code into a single package

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftによると、GigaWiperは少なくとも3系統のマルウェア要素を1つにまとめたモジュール型のツールとみられています。
Windows環境を対象に、破壊的な挙動を示すバックドアやワイパー、ランサムウェア系コードが同居している点が注目されています。
複数の攻撃要素を統合した設計であれば、検知や分析が難しくなる可能性があります。
ランサムウェア文脈に加えて破壊的影響も想定されるため、被害の広がりや復旧負荷の観点で警戒が必要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Windows端末やサーバーで、不審な永続化・権限昇格・異常なファイル改変の兆候を点検する。
- EDRやログ監視で、単一サンプルでも複数の不審挙動が重なるケースを優先的に調査する。
- 重要データのバックアップと復旧手順を見直し、破壊的挙動を含む事案に備える。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Destructive Windows backdoor stuffs multiple wipers and ransomware code into a s](https://www.theregister.com/security/2026/07/10/destructive-windows-backdoor-stuffs-multiple-wipers-and-ransomware-code-into-a-single-package/5270053) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-21958"></a>

### 5. GigaWiper Combines Multiple Malware for System-Level Sabotage

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

GigaWiperとされるマルウェアは、システム破壊を目的とした機能を複数組み合わせていると報じられています。
公開情報では、単体のワイパー機能に加え、ランサムウェア的な暗号化や複数回の消去コマンドが含まれるとされています。
データ保全だけでなく、システムそのものの破壊を狙う可能性があるため、通常のランサムウェア対策だけでは不十分なケースがあります。
被害が発生した場合の復旧難度や業務停止の影響が大きくなり得る点が注目されています。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- バックアップの分離保管と復元手順の定期確認を行う。
- 重要端末での権限管理、異常な暗号化・消去動作の監視を強化する。
- 侵入後の横展開を想定し、検知・封じ込め・初動連絡の手順を見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [GigaWiper Combines Multiple Malware for System-Level Sabotage](https://www.securityweek.com/gigawiper-combines-multiple-malware-for-system-level-sabotage/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21967"></a>

### 6. ‘HalluSquatting’ Turns AI Hallucinations Into Botnet Delivery Mechanism

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者が、AIアシスタントの誤生成（ハルシネーション）を悪用する「HalluSquatting」という手法を示したとされています。
公開情報では、人気のAIアシスタントを対象にした実証の中で、リモートコード実行につながる可能性が示されたとされています。
AIの回答品質や検索結果の誤りが、そのまま攻撃の足がかりになりうる点が注目されています。
AIを業務利用する場面では、出力の正確性だけでなく、外部参照や実行連携の設計にも注意が必要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIアシスタントの出力をそのまま信頼せず、参照先や実行前の検証を必須にする。
- 外部コンテンツを取り込む仕組みでは、正規ドメインやソースの真正性確認を強化する。
- AI連携機能に権限が集中しないよう、最小権限と監査ログの確認を見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [‘HalluSquatting’ Turns AI Hallucinations Into Botnet Delivery Mechanism](https://www.securityweek.com/hallusquatting-turns-ai-hallucinations-into-botnet-delivery-mechanism/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

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
| [Injective LabsのGitHub侵害によりウォレットキー窃取のnpmパッケージが配布される](https://thehackernews.com/2026/07/injective-labs-github-compromise-pushes.html) | 28.0 | 45.0 | 42.0 |
| [ランサムウェア関連の法執行・司法措置](https://www.bleepingcomputer.com/news/security/ryuk-ransomware-member-pleads-guilty-in-the-us-faces-15-years-in-prison/) | 28.0 | 30.0 | 42.0 |
| [その他のニュース：DHSデータベースが侵害、Adobeがパッチ頻度を引き上げ、カナダがランサムウェア作戦を妨害](https://www.securityweek.com/in-other-news-dhs-database-hacked-adobe-boosts-patch-cadence-canada-disrupts-ransomware-ops/) | 28.0 | 30.0 | 42.0 |
| [新型ランサムウェア、悪意あるドライバーを悪用してサイバーセキュリティ保護を解除](https://www.infosecurity-magazine.com/news/ransomware-removes-cybersecurity/) | 28.0 | 30.0 | 42.0 |
| [Microsoft、スパイ活動と破壊機能を併せ持つ新たな「GigaWiper」マルウェアに警告](https://www.infosecurity-magazine.com/news/new-gigawiper-espionage-destructive/) | 28.0 | 20.0 | 42.0 |
| [新たなWindowsマルウェアがPCを乗っ取り、データを消去可能にする](https://www.malwarebytes.com/blog/news/2026/07/this-new-windows-malware-can-take-over-your-pc-and-wipe-it-clean) | 28.0 | 20.0 | 42.0 |
| [中国とインド、同じパキスタン警察を標的にした別々のスパイ活動を実施](https://therecord.media/china-india-ran-separate-spy-campaigns-against-same-police-force) | 28.0 | 20.0 | 42.0 |
| [新たなMODBEACON RAT、暗号化されたC2通信にgRPCストリーミングを使用](https://thehackernews.com/2026/07/new-modbeacon-rat-uses-grpc-streaming.html) | 28.0 | 20.0 | 42.0 |
| [ハッカーが偽のMicrosoft Entraパスキー登録を使ってMicrosoft 365にアクセスする](https://thehackernews.com/2026/07/hackers-use-fake-microsoft-entra.html) | 28.0 | 20.0 | 42.0 |
| [200件のGitHubリポジトリで構成されたマルウェア感染ネットワーク](https://www.securityweek.com/network-of-200-github-repositories-used-for-malware-infection/) | 28.0 | 20.0 | 42.0 |
| [MicrosoftのSecure Future Initiativeに関する2026年7月の進捗レポート](https://www.microsoft.com/en-us/security/blog/2026/07/10/securing-our-future-july-2026-progress-report-on-microsofts-secure-future-initiative/) | 27.0 | 20.0 | 42.0 |
| [AnthropicとOpenAIのセキュリティツールがサイバー攻撃を助長する可能性、研究者が警告](https://www.infosecurity-magazine.com/news/anthropic-openai-report-exploit/) | 27.0 | 20.0 | 42.0 |
| [HTMLのフィッシング添付ファイルでの「Comment stuffing」によるAIベース検知回避](https://isc.sans.edu/diary/rss/33144) | 27.0 | 20.0 | 42.0 |
| [Researcherが3つのOpenClaw脆弱性を利用したWhatsApp経由のホスト攻撃チェーンを詳細に解説](https://thehackernews.com/2026/07/researcher-details-whatsapp-to-host.html) | 25.0 | 20.0 | 42.0 |
| [ディレクトリに潜むレプリカント：AIエージェントとアイデンティティセキュリティのギャップ](https://www.bleepingcomputer.com/news/security/the-replicant-in-your-directory-ai-agents-and-the-identity-security-gap/) | 25.0 | 20.0 | 42.0 |
| [AIコーディング：セキュリティリスクは生産性向上を上回るのか](https://www.darkreading.com/application-security/ai-coding-security-risks-productivity-gains) | 25.0 | 20.0 | 42.0 |
| [サイバーセキュリティ強化に使うAIエージェントが悪用される可能性、OpenAIとAnthropicのモデルを操る「Friendly Fire」攻撃で悪意あるコードを実行させる手口](https://www.itpro.com/security/the-agents-you-use-to-beef-up-cybersecurity-could-be-turned-against-you-friendly-fire-attacks-can-manipulate-openai-and-anthropic-models-into-running-malicious-code) | 25.0 | 20.0 | 42.0 |
| [本人の同意なしに健診結果を家族に説明 - 八重瀬町](https://www.security-next.com/186912) | 22.0 | 20.0 | 42.0 |
| [説明会の案内状を誤送信、全参加予定者の氏名 - 大阪市](https://www.security-next.com/187074) | 22.0 | 20.0 | 42.0 |
| [中学校の生徒情報含む私物メディアを鞄ごと紛失 - 江戸川区](https://www.security-next.com/186977) | 22.0 | 20.0 | 42.0 |
| [ボランティア情報含むページが閲覧可能に - 千歳JAL国際マラソン](https://www.security-next.com/186914) | 22.0 | 20.0 | 42.0 |
| [通販サイトに不正アクセスか、調査中 - アメニティメーカー](https://www.security-next.com/187124) | 22.0 | 20.0 | 42.0 |
| [Braveが「クレジットカードの発行」「BravePayの開発」などBATに関するロードマップを発表](https://gigazine.net/news/20260710-brave-bat-roadmap-4/) | 22.0 | 20.0 | 42.0 |
| [都民向け金融セミナーの申込サイトが一時消失 - 攻撃の痕跡も](https://www.security-next.com/187062) | 22.0 | 20.0 | 42.0 |
| [ZimbraがWebクライアントの重大なXSS脆弱性への対策を呼びかけ](https://www.bleepingcomputer.com/news/security/zimbra-urges-customers-to-patch-critical-web-client-xss-flaw/) | 21.0 | 26.0 | 42.0 |
| [CISA、大規模な5月の認証情報流出への対策を検討](https://cyberscoop.com/cisa-credential-leak-forensic-report/) | 20.0 | 20.0 | 42.0 |
| [サイバー犯罪者が攻撃を増やす中、医療機関に集まる理由](https://www.darkreading.com/threat-intelligence/cybercriminals-healthcare-businesses-attacks-surge) | 20.0 | 20.0 | 42.0 |
| [オランダのハッカーがOdidoの侵害に関与した疑い、警察が捜査](https://www.bleepingcomputer.com/news/security/police-suspects-dutch-hackers-were-involved-in-odido-breach/) | 20.0 | 20.0 | 42.0 |
| [Progress Tells ShareFile Customersに対し、セキュリティ脅威を受けStorage Zone Controllerの停止を要請](https://thehackernews.com/2026/07/urgent-progress-tells-sharefile.html) | 20.0 | 20.0 | 42.0 |
| [ProgressがShareFile管理者にサーバー停止を要請、信頼できる脅威のため](https://www.bleepingcomputer.com/news/security/progress-urges-sharefile-customers-to-shut-down-servers-over-credible-threat/) | 20.0 | 20.0 | 42.0 |
| [露出したAWS GovCloudキーへのインシデント対応をCISAが詳述](https://www.infosecurity-magazine.com/news/cisa-incident-response-exposed-aws/) | 20.0 | 20.0 | 42.0 |
| [U-Bootの6件の新たな脆弱性、悪意あるイメージでデバイスをクラッシュさせたり起動時にコード実行されたりする恐れ](https://thehackernews.com/2026/07/six-new-u-boot-flaws-could-let.html) | 20.0 | 20.0 | 42.0 |
| [HackersがGitea Dockerイメージの重大な認証バイパスを悪用](https://www.bleepingcomputer.com/news/security/hackers-exploit-critical-auth-bypass-in-gitea-docker-image/) | 20.0 | 20.0 | 42.0 |
| [収監中に押収された暗号資産を盗んだとして告発された資金洗浄業者](https://www.bleepingcomputer.com/news/security/money-launderer-accused-of-stealing-seized-crypto-while-in-prison/) | 20.0 | 20.0 | 42.0 |
| [CitrixBleed2脆弱性の武器化に関与した初期アクセスブローカー](https://www.cybersecuritydive.com/news/initial-access-broker-citrixbleed2-flaw-DragonForce/824961/) | 20.0 | 20.0 | 42.0 |
| [Laser AttackでTangem Walletのカードにパスワード再設定を強制、修正不能な脆弱性が判明](https://thehackernews.com/2026/07/laser-attack-resets-tangem-wallet.html) | 20.0 | 20.0 | 42.0 |
| [CISA、GitHubへのパスワードとクラウドアクセスキー漏えいにつながったセキュリティ不備を詳述](https://www.cybersecuritydive.com/news/cisa-github-passwords-leak-contractor-report/824953/) | 20.0 | 20.0 | 42.0 |
| [ATM暗号ソフトウェアの新たな脆弱性：大当たりか、それとも失敗か](https://www.darkreading.com/vulnerabilities-threats/atm-crypto-software-bugs-jackpot-bust) | 20.0 | 20.0 | 42.0 |
| [各国で広がるソーシャルメディア禁止の動き](https://www.darkreading.com/cyber-risk/more-countries-jump-on-the-social-media-ban-wagon) | 20.0 | 20.0 | 42.0 |
| [Incode、プライバシー重視の本人確認向け年齢推定にオンデバイス処理を導入](https://www.helpnetsecurity.com/2026/07/10/incode-on-device-age-estimation/) | 20.0 | 20.0 | 42.0 |
| [Fashion mart Miintoが侵害の詳細を公開、利用者にフィッシング詐欺への注意を呼びかけ](https://www.theregister.com/security/2026/07/10/miinto-fesses-up-to-breach-says-customers-open-to-phishing/5269891) | 20.0 | 20.0 | 42.0 |
| [中国・インド関連のハッカーがいずれも同じパキスタン警察組織を標的にした件](https://www.securityweek.com/china-india-linked-hackers-both-targeted-same-pakistani-police-force/) | 20.0 | 20.0 | 42.0 |
| [XQUICの未修正XRING脆弱性によりHTTP/3サーバーがリモートからクラッシュする問題](https://thehackernews.com/2026/07/unpatched-xring-flaw-in-xquic-lets.html) | 20.0 | 20.0 | 42.0 |
| [17000件から110万件へ：Lumen Technologiesが大規模に再構築したエクスポージャー管理](https://thehackernews.com/2026/07/from-17000-to-11-million-assets-how.html) | 20.0 | 20.0 | 42.0 |
| [公開されたハッカーのサーバーからWP-SHELLSTORMが数千のWordPressサイトにバックドアを仕掛けていたことが判明](https://thehackernews.com/2026/07/exposed-hacker-server-reveals-wp.html) | 20.0 | 20.0 | 42.0 |
| [OktaがMicrosoft 365顧客を標的としたビッシング攻撃に注意喚起](https://www.securityweek.com/okta-warns-of-vishing-attacks-targeting-microsoft-365-customers/) | 20.0 | 20.0 | 42.0 |
| [mule betting詐欺が一般人を勧誘する手口](https://www.malwarebytes.com/blog/scams/2026/07/how-mule-betting-scams-recruit-ordinary-people) | 20.0 | 20.0 | 42.0 |
| [2日連続のChromeアップデートで致命的な脆弱性を修正](https://www.malwarebytes.com/blog/news/2026/07/two-chrome-updates-in-two-days-fix-critical-vulnerabilities) | 20.0 | 20.0 | 42.0 |
| [Symantec Data Center SecurityがCommon Criteria認証を取得](https://www.security.com/product-insights/humble-brag-symantec-data-center-security-achieves-common-criteria-certification) | 20.0 | 20.0 | 42.0 |
| [Microsoft、セキュリティ更新プログラムの件数増加を警告](https://www.infosecurity-magazine.com/news/microsoft-increase-number-security/) | 20.0 | 20.0 | 42.0 |
| [Scot NHS Trustが産科患者データを含むメールの誤送信を調査](https://www.theregister.com/security/2026/07/10/scot-nhs-trust-probes-email-stuffup-involving-maternity-patients-data/5269749) | 20.0 | 20.0 | 42.0 |
| [「Ill Bloom」の脆弱性を悪用して暗号資産ウォレットから500万ドル超を流出させる攻撃者](https://thehackernews.com/2026/07/attackers-exploit-ill-bloom.html) | 20.0 | 20.0 | 42.0 |
| [NHS、患者データへの不正アクセスについて職員に警告](https://www.infosecurity-magazine.com/news/nhs-warns-staff-unauthorized/) | 20.0 | 20.0 | 42.0 |

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
