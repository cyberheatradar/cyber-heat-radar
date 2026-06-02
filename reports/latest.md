# 📡 サイレーダー 2026-06-03 05:00 JST

このレポートは、2026-06-02 17:00 JST〜2026-06-03 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 96
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 62

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Google fixes actively exploited Android vulnerability (CVE-2025-48595)](#topic-13941) | 43.0 | 46.0 | 55.0 | 音声 | 温度感上位枠 |
| 2 | [Tuskira Quell identifies, mitigates, and validates zero-day risk before breach](#topic-13949) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [CISA flags two-year-old Oracle flaw as actively exploited in attacks](#topic-13960) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [CISA Adds Two Known Exploited Vulnerabilities to Catalog](#topic-13971) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [Google fixes one actively exploited Android zero-day, 124 flaws](#topic-13980) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [Oracle WebLogic Vulnerability Exploited in the Wild](#topic-13437) | 33.0 | 46.0 | 55.0 | GitHub | 音声枠上限によりGitHubのみ |
| 7 | [Threat Actor Uses AI to Build EDR Evasion Tools](#topic-13982) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 8 | [Sophos uncovers AI-powered malware lab built for EDR evasion](#topic-13991) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-13941"></a>

### 1. Google fixes actively exploited Android vulnerability (CVE-2025-48595)

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>Android</nobr> / <nobr>CVE</nobr> / <nobr>ゼロデイ</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>政策・規制</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 43.0 |
| <nobr>実務影響</nobr> | 46.0 |
| <nobr>確度</nobr> | 55.0 |

#### 概要

GoogleはAndroid向けのセキュリティ更新で、CVE-2025-48595を修正しました。
公開情報によると、この脆弱性はAndroid Framework内の整数オーバーフローで、限定的かつ標的型の攻撃で悪用されていた可能性があるとされています。
すでに悪用が観測されている脆弱性のため、対応が遅れると端末が侵害されるリスクがあります。Androidは利用者が多く影響範囲が広いため、組織としての更新優先度が高い案件です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 対象端末で最新のAndroidセキュリティ更新が適用されているか確認する。
- MDMなどで更新状況を把握し、未適用端末を優先的に是正する。
- 高権限化の兆候や不審な端末挙動がないか、関連ログと端末監視を確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-48595 | 主要CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-48595](https://nvd.nist.gov/vuln/detail/CVE-2025-48595) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Android Update Patches Exploited Zero-Day, 123 Other Vulnerabilities](https://www.securityweek.com/android-update-patches-exploited-zero-day-123-other-vulnerabilities/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google fixes actively exploited Android vulnerability (CVE-2025-48595)](https://www.helpnetsecurity.com/2026/06/02/android-vulnerability-exploited-cve-2025-48595/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-13949"></a>

### 2. Tuskira Quell identifies, mitigates, and validates zero-day risk before breach

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ゼロデイ</nobr> / <nobr>防御・運用</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Tuskiraが、ゼロデイ脆弱性の公開から修正までの間に残るリスクを可視化・低減するという「Quell」を発表したと伝えられています。
環境内で到達可能か、既存の制御で止められるか、どの補完策が有効かを確認する考え方が示されています。
ゼロデイはパッチが出る前の短い期間でも被害につながるため、露出状況を把握して先回りで対策する発想は実務上の関心が高いです。
特に、資産が多く対策の優先順位付けが難しい組織では、リスクの絞り込みに役立つ可能性があります。

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

- 自組織で「到達可能な資産」と「実際に守れている資産」を分けて把握できているか確認する。
- ゼロデイの有無だけでなく、既存の防御設定や代替統制で止められるかを点検する。
- パッチ待ちの間に適用できる暫定対策の手順と責任分担を事前に整理しておく。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Tuskira Quell identifies, mitigates, and validates zero-day risk before breach](https://www.helpnetsecurity.com/2026/06/02/tuskira-quell-zero-day-defense/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 未確認。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-13960"></a>

### 3. CISA flags two-year-old Oracle flaw as actively exploited in attacks

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

CISAは、Oracle WebLogic Serverの高深刻度脆弱性について、すでに修正済みであるにもかかわらず攻撃で実際に悪用されているとして、対策を求めました。
材料からは、少なくとも2年前に修正された脆弱性がいまだに危険視されていることが読み取れます。
既知の脆弱性であっても、未対策のシステムでは継続して被害につながるおそれがあるためです。政府機関向けの注意喚起が出ている点からも、優先度の高い対応対象とみられます。

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

- Oracle WebLogic Serverの適用状況を確認し、関連パッチが適用済みか点検する。
- インターネット公開している管理系・アプリ系のWebLogic環境を優先的に棚卸しする。
- 脆弱性対応に加え、侵害の兆候がないかログと設定変更の有無を確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA flags two-year-old Oracle flaw as actively exploited in attacks](https://www.bleepingcomputer.com/news/security/cisa-orders-feds-to-patch-actively-exploited-oracle-weblogic-flaw/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-13971"></a>

### 4. CISA Adds Two Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>KEV</nobr> / <nobr>CVE</nobr> / <nobr>Linux</nobr> / <nobr>認証バイパス</nobr> / <nobr>Android</nobr> / <nobr>政策・規制</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

CISAは、実際に悪用された証拠があるとして、Known Exploited Vulnerabilities（KEV）Catalogに2件の脆弱性を追加しました。
対象はCVE-2022-0492（Linux Kernelの不適切な認証）とCVE-2025-48595（Android Frameworkの整数オーバーフロー）です。
KEVに載る脆弱性は、攻撃者に狙われる可能性が高いものとして優先対応が求められます。特に政府機関だけでなく、一般組織でも資産の棚卸しと修正優先度の見直しが必要です。

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

- 自組織でLinux KernelおよびAndroid Frameworkの該当影響有無を確認し、対象資産を洗い出す。
- KEV掲載を踏まえて、通常より高い優先度でパッチ適用や緩和策を進める。
- モバイル端末やLinux系ホストの監視を強化し、関連する異常挙動や侵害兆候を点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2022-0492 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2025-48595 | 主要CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Two Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/06/02/cisa-adds-two-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-13980"></a>

### 5. Google fixes one actively exploited Android zero-day, 124 flaws

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ゼロデイ</nobr> / <nobr>Android</nobr> / <nobr>脆弱性</nobr> / <nobr>攻撃キャンペーン</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

GoogleはAndroid向けの6月セキュリティ更新を公開し、合計124件の脆弱性に対処しました。
その中には、標的型攻撃で悪用が確認されたゼロデイ脆弱性が含まれているとされています。実際に悪用された脆弱性が含まれるため、対応の優先度が高い話題です。
Android端末の利用者だけでなく、端末管理やパッチ適用を担う運用側にとっても影響が大きいと考えられます。

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

- 該当するAndroid端末のセキュリティアップデート適用状況を確認する。
- 管理端末については、ベンダー別の配信状況と適用遅延を把握する。
- 悪用が確認された脆弱性として、関連端末の監視やインシデント対応体制を見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Google fixes one actively exploited Android zero-day, 124 flaws](https://www.bleepingcomputer.com/news/security/google-fixes-one-actively-exploited-android-zero-day-124-flaws/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-13982"></a>

### 6. Threat Actor Uses AI to Build EDR Evasion Tools

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脅威アクター</nobr> / <nobr>AI</nobr> / <nobr>防御・運用</nobr> / <nobr>マルウェア</nobr> |
| <nobr>分類理由</nobr> | AI×Security枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Sophosの分析によると、ある脅威アクターがAIのコーディングツールを使い、EDRの回避を目的としたマルウェアの作成と試験を行っていたとされています。
AIが攻撃コードの開発支援に使われる事例として、検知・防御側にとって無視しにくい動きです。
EDRは多くの組織で検知の中核にあるため、その回避を狙う手法がAIで補助される点は注目されます。
攻撃者の開発効率が上がる可能性があり、防御側は検知ルールや運用の見直しが求められます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- EDRのアラートだけに依存せず、ログ相関や異常挙動の確認を含めた検知設計を見直す。
- 不審なコード生成や実行の兆候を踏まえ、エンドポイント周辺の監視とハンティングを強化する。
- AI利用を前提に、攻撃手法の変化を継続的に追い、検知ロジックの更新頻度を上げる。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Threat Actor Uses AI to Build EDR Evasion Tools](https://www.infosecurity-magazine.com/news/ai-edr-evasion-tooling/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 未確認。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-13991"></a>

### 7. Sophos uncovers AI-powered malware lab built for EDR evasion

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>防御・運用</nobr> / <nobr>マルウェア</nobr> / <nobr>政策・規制</nobr> / <nobr>TTP</nobr> / <nobr>脅威アクター</nobr> |
| <nobr>分類理由</nobr> | AI×Security枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Sophosによると、AI技術を使ってEDRの検知回避を目的としたマルウェア検証環境が確認されたとされています。
顧客環境で不審な端点のアラートをきっかけに調査が進み、検証用ディレクトリから関連ファイルが見つかったとされています。
AIが攻撃の自動化だけでなく、防御製品の回避手法の研究・改善にも使われうることを示す事例として注目されます。
EDR運用側は、従来型の検知だけでなく挙動ベースの監視やチューニングの重要性を再認識する必要があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 検証用や一時的なディレクトリに置かれた不審ファイルも、調査対象として扱う。
- EDRのアラートを個別事象で終わらせず、関連する実行痕跡や通信パターンを横断的に確認する。
- 検知回避を意識した活動に備え、ルールや検知ロジックの継続的な見直しを行う。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Sophos uncovers AI-powered malware lab built for EDR evasion](https://www.helpnetsecurity.com/2026/06/02/ai-agents-edr-evasion-techniques/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・低信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-13437"></a>

### 1. Oracle WebLogic Vulnerability Exploited in the Wild

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>KEV</nobr> / <nobr>CVE</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 46.0 |
| <nobr>確度</nobr> | 55.0 |

#### 概要

Oracle WebLogic Vulnerability Exploited in the Wild に関する脆弱性情報です。
では英語本文の全文翻訳は行わず、参照リンク、関連する対象、スコア根拠を中心に整理しています。詳細はベンダー公式情報、公的機関情報、NVD等を確認してください。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 自組織で対象製品・関連資産を利用しているか確認する。
- ベンダー公式情報または公的機関情報を優先確認する。
- 対象バージョンか確認する。
- 修正版・緩和策の適用状況を確認する。
- インターネット露出の有無を確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2024-21182 | 主要CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2024-21182](https://nvd.nist.gov/vuln/detail/CVE-2024-21182) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Oracle WebLogic Vulnerability Exploited in the Wild](https://www.securityweek.com/oracle-weblogic-vulnerability-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/06/01/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [CISAとパートナー機関、Automatic Tank Gauge Systemsの強化を呼びかけ](https://www.cisa.gov/resources-tools/resources/cisa-and-partners-urge-hardening-automatic-tank-gauge-systems) | 32.0 | 38.0 | 48.0 |
| [グループ会社2社でランサム被害 - 青山財産ネットワークス](https://www.security-next.com/184515) | 30.0 | 30.0 | 42.0 |
| [Red Hatのnpmパッケージが新たなMini Shai-Huludマルウェア波で侵害される](https://www.helpnetsecurity.com/2026/06/02/red-hat-npm-packages-compromised-mini-shai-hulud/) | 28.0 | 45.0 | 42.0 |
| [ランサムウェアグループの利益はFTSE 350企業よりも急速に増加している](https://www.itpro.com/security/ransomware/ransomware-group-profits-are-rising-faster-than-ftse-350-firms) | 28.0 | 30.0 | 42.0 |
| [GamaredonがWinRARを悪用し、GammaWormとGammaSteelをウクライナに配布](https://thehackernews.com/2026/06/gamaredon-exploits-winrar-to-deliver.html) | 28.0 | 20.0 | 42.0 |
| [Zero-Knowledge脅威アクターと責任ある開示の終焉](https://www.securityweek.com/the-zero-knowledge-threat-actor-and-the-end-of-responsible-disclosure/) | 28.0 | 20.0 | 42.0 |
| [偽の発注書から遠隔アクセスへ：US企業を狙うJS.MonoGlyphRATの脅威分析](https://any.run/cybersecurity-blog/monoglyphrat-attacks-us-enterprise/) | 28.0 | 20.0 | 42.0 |
| [Operation FlutterBridge: macOSマルバタイジングキャンペーンが新たなFlutterShellバックドアを拡散](https://unit42.paloaltonetworks.com/flutterbridge-new-fluttershell-backdoor/) | 28.0 | 20.0 | 42.0 |
| [Pakistan関連のSideCopyがAfghanistan財務省を標的にXeno RATで攻撃](https://thehackernews.com/2026/06/pakistan-linked-sidecopy-targets.html) | 28.0 | 20.0 | 42.0 |
| [モバイルゲームに偽のウイルス警告が侵入している](https://www.malwarebytes.com/blog/mobile/2026/06/fake-virus-alerts-are-invading-mobile-games) | 28.0 | 20.0 | 42.0 |
| [AIエージェントが暴走する前に安全にするのはほぼ不可能](https://www.darkreading.com/cyber-risk/securing-ai-agents-rogue) | 25.0 | 20.0 | 42.0 |
| [ホワイトハウス、縮小版のAIに関する大統領令を発表](https://therecord.media/white-house-unveils-ai-executive-order) | 25.0 | 20.0 | 42.0 |
| [Trumpが強力なAIモデルへの政府の早期アクセスを求める大統領令に署名](https://www.cybersecuritydive.com/news/trump-ai-security-executive-order/821755/) | 25.0 | 20.0 | 42.0 |
| [DOD、全作戦にサイバーを統合しAIにもセキュリティを組み込む](https://cyberscoop.com/pentagon-cyber-integration-ai-security/) | 25.0 | 20.0 | 42.0 |
| [Trump政権が縮小版のAI大統領令を発表](https://cyberscoop.com/donald-trump-white-house-ai-executive-order-scaled-back/) | 25.0 | 20.0 | 42.0 |
| [Meta AIの悪用によりInstagramユーザーがアカウントを乗っ取られロックアウトされる](https://www.bleepingcomputer.com/news/security/instagram-users-locked-out-after-meta-ai-abused-to-steal-accounts/) | 25.0 | 20.0 | 42.0 |
| [Infosecurity Europe：AIを活用しないサイバーセキュリティチームは「失敗する運命にある」](https://www.infosecurity-magazine.com/news/cybersecurity-teams-doomed-to-fail/) | 25.0 | 20.0 | 42.0 |
| [なぜブラウザがAIセキュリティの最前線なのか](https://www.bleepingcomputer.com/news/security/why-the-browser-is-now-the-front-line-for-ai-security/) | 25.0 | 20.0 | 42.0 |
| [Anthropic、Project Glasswingの利用範囲を拡大](https://cyberscoop.com/anthropic-project-glasswing-expansion-critical-infrastructure-claude-mythos/) | 25.0 | 20.0 | 42.0 |
| [AnthropicがMythosを150の組織に追加共有、重要インフラ事業者も含む](https://www.cybersecuritydive.com/news/ai-anthropic-claude-mythos-project-glasswing-expand/821714/) | 25.0 | 20.0 | 42.0 |
| [Anthropic、Mythosの利用対象を150の新組織へ拡大](https://www.securityweek.com/anthropic-expanding-mythos-access-to-150-new-organizations/) | 25.0 | 20.0 | 42.0 |
| [NomaがAIエージェントとMCPサーバーに可視性とアクセスガバナンスを提供](https://www.helpnetsecurity.com/2026/06/02/noma-brings-visibility-and-access-governance-to-ai-agents-and-mcp-servers/) | 25.0 | 20.0 | 42.0 |
| [Infosecurity Europe: Bayer、AI脅威に対抗するためセキュリティ意識向上トレーニングを刷新](https://www.infosecurity-magazine.com/news/bayer-reinvents-security-awareness/) | 25.0 | 20.0 | 42.0 |
| [AIが攻撃までの時間を短縮し、サイバー耐性の抜本的見直しを迫っている――組織はどう備えるべきか](https://www.itpro.com/security/ai-is-shrinking-attack-windows-and-its-forcing-a-complete-rethink-of-cyber-resilience-heres-how-organizations-can-prepare) | 25.0 | 20.0 | 42.0 |
| [Beyond Assume-Breach: AIネイティブなセキュリティがエンタープライズ防御をどう変えるか](https://www.darkreading.com/cyber-risk/assume-breach-ai-native-security-reshape-enterprise-defense) | 25.0 | 20.0 | 42.0 |
| [AI駆動の脆弱性悪用が脆弱性管理を破壊している、その対処法](https://thehackernews.com/2026/06/ai-driven-exploitation-is-destroying.html) | 25.0 | 20.0 | 42.0 |
| [Meta AIが著名Instagramアカウントをハッカーに引き渡す](https://www.securityweek.com/meta-ai-hands-over-high-profile-instagram-accounts-to-hackers/) | 25.0 | 20.0 | 42.0 |
| [Infosecurity Europe：英国企業が進化するサイバーリスクに備えAI脅威対策を優先](https://www.infosecurity-magazine.com/news/uk-firms-prioritize-ai-threat/) | 25.0 | 20.0 | 42.0 |
| [Cybanetix、ユーザー・モデル・エージェントを保護するManaged AI Serviceを発表](https://www.helpnetsecurity.com/2026/06/02/cybanetix-managed-ai-service/) | 25.0 | 20.0 | 42.0 |
| [OpenAIが既存のAWS環境にフロンティアAIを導入](https://www.helpnetsecurity.com/2026/06/02/openai-models-and-codex-on-aws/) | 25.0 | 20.0 | 42.0 |
| [HP VoIP Phonesの重大な脆弱性により企業ネットワーク侵害が可能に](https://www.securityweek.com/critical-vulnerability-in-hp-voip-phones-enables-enterprise-network-breaches/) | 24.0 | 38.0 | 42.0 |
| [Microsoft Entraがパスキーを推進、アイデンティティセキュリティを強化](https://www.helpnetsecurity.com/2026/06/02/microsoft-entra-latest-security-updates/) | 22.0 | 20.0 | 43.0 |
| [Microsoft Build 2026: 開発ライフサイクル全体でコード、エージェント、モデルを保護する](https://www.microsoft.com/en-us/security/blog/2026/06/02/microsoft-build-2026-securing-code-agents-and-models-across-the-development-lifecycle/) | 22.0 | 20.0 | 42.0 |
| [海外子会社でM365に不正アクセス、スパムの踏み台に - TEIKOKU](https://www.security-next.com/184367) | 22.0 | 20.0 | 42.0 |
| [委託業者がメール誤送信、児童の保護者のメアド流出 - 大阪市](https://www.security-next.com/185204) | 22.0 | 20.0 | 42.0 |
| [マネーフォワードの銀行連携、再開率99％超でも「完全復旧」に至らないワケ](https://www.itmedia.co.jp/news/articles/2606/02/news097.html) | 21.0 | 20.0 | 42.0 |
| [Red Hat、ソフトウェアパイプライン侵害後に汚染されたパッケージを削除](https://therecord.media/red-hat-removes-tainted-packages-after-software-pipeline-compromise) | 20.0 | 45.0 | 42.0 |
| [AttackersがRed Hatのnpmスコープを乗っ取りクラウド機密情報を窃取](https://www.infosecurity-magazine.com/news/red-hat-npm-scope-backdoored/) | 20.0 | 45.0 | 42.0 |
| [Red Hatの32件のNPMパッケージを標的としたサプライチェーン攻撃](https://www.securityweek.com/supply-chain-attack-hits-32-red-hat-npm-packages/) | 20.0 | 45.0 | 42.0 |
| [Red Hatのnpmパッケージ数十件がサプライチェーン攻撃の標的に](https://www.cybersecuritydive.com/news/dozens-red-hat-npm-packages-supply-chain-attack/821723/) | 20.0 | 30.0 | 42.0 |
| [CVE-2026-48959: Perl用IO::Uncompress::Unzipの2.220未満におけるfastForwardの1バイト単位読み取りループによるCPU枯渇の脆弱性](https://nvd.nist.gov/vuln/detail/CVE-2026-48959) | 20.0 | 28.0 | 38.0 |
| [CVE-2026-6324 Libsoup: 符号なしから符号付きへの変換エラーによるHTTPリクエストスミグリング](https://nvd.nist.gov/vuln/detail/CVE-2026-6324) | 20.0 | 28.0 | 38.0 |
| [CVE-2026-10028 glib-networking gnutlsバックエンドの無限ループにより循環証明書チェーンを通じたリモートDoSが可能に](https://nvd.nist.gov/vuln/detail/CVE-2026-10028) | 20.0 | 28.0 | 38.0 |
| [巧妙な著作権通知を装ってGoogleのログイン情報を盗む手口](https://www.malwarebytes.com/blog/threat-intel/2026/06/these-convincing-copyright-notices-are-designed-to-steal-google-logins) | 20.0 | 20.0 | 42.0 |
| [Cyber Brief 26-06 - 2026年5月版](https://cert.europa.eu/publications/threat-intelligence/cb26-06/) | 20.0 | 20.0 | 42.0 |
| [サイバーセキュリティの深刻化する危機についての2つの新レポートが示す対立する見解](https://www.securityweek.com/two-new-reports-offer-competing-explanations-for-cybersecuritys-growing-crisis/) | 20.0 | 20.0 | 42.0 |
| [ロシア、外国の諜報機関が政府高官の携帯電話をハッキングしたと主張](https://therecord.media/russia-claims-foreign-spy-agencies-hacked-gov-officials) | 20.0 | 20.0 | 42.0 |
| [Infosecurity Europe：不確実性が続く中、NCSCがレジリエンス強化へ緊急対応を要請](https://www.infosecurity-magazine.com/news/ncsc-resilience-certainty-is-never/) | 20.0 | 20.0 | 42.0 |
| [1行のコードが数十億回のMicrosoft Androidアプリダウンロードを危険にさらした方法](https://www.securityweek.com/exclusive-how-one-line-of-code-put-billions-of-microsoft-android-app-downloads-at-risk/) | 20.0 | 20.0 | 42.0 |
| [Windows Searchの未修正NTLM強制認証脆弱性：URIハンドラー、同一バグ、CVEなし、修正なし](https://www.huntress.com/blog/unpatched-ntlm-coercion-windows-search-uri-handler) | 20.0 | 20.0 | 42.0 |
| [Infosecurity Europeに関するサイバーセキュリティ動向](https://www.darkreading.com/events/infosecurity-europe) | 20.0 | 20.0 | 42.0 |
| [Meta、10代向けフィードに厳格なガードレールを追加](https://www.helpnetsecurity.com/2026/06/02/meta-expands-teen-accounts-protections/) | 20.0 | 20.0 | 42.0 |
| [GTA VチートサービスAtlas Menuの侵害で6万4000件のアカウントが流出](https://www.helpnetsecurity.com/2026/06/02/atlas-menu-cheat-service-data-breach/) | 20.0 | 20.0 | 42.0 |
| [対立を協力へ変える：CIOとCISOが共に導く方法](https://www.cybersecuritydive.com/news/turning-tension-into-collaboration-how-cios-cisos-can-lead-together/821610/) | 20.0 | 20.0 | 42.0 |
| [Codexの知識業務機能が調査、レポート、スプレッドシートへ拡大](https://www.helpnetsecurity.com/2026/06/02/openai-codex-knowledge-work/) | 20.0 | 20.0 | 42.0 |
| [メキシコ全土におけるWardriving評価：2026年ワールドカップに向けて](https://securelist.com/wardriving-assessment-in-mexico-fifa-world-cup-2026/119996/) | 20.0 | 20.0 | 42.0 |
| [CISA、自動タンクゲージシステムのセキュリティ強化を呼びかけ](https://www.cisa.gov/news-events/news/cisa-urges-stronger-security-automatic-tank-gauge-systems) | 20.0 | 20.0 | 42.0 |
| [Diligentがサイバーリスク評価とレポート作成を自動化](https://www.helpnetsecurity.com/2026/06/02/diligent-automates-cyber-risk-assessments-and-reporting/) | 20.0 | 20.0 | 42.0 |
| [23andMe、数百万人分の遺伝情報を漏えいしたと訴訟で指摘される](https://www.malwarebytes.com/blog/data-breaches/2026/06/23andme-exposed-genetic-information-of-millions-lawsuit-says) | 20.0 | 20.0 | 42.0 |
| [KDE Linuxのセキュリティ監査、カーネルモジュールと未使用パッケージを削減](https://www.helpnetsecurity.com/2026/06/02/kde-linux-security-audit-update/) | 20.0 | 20.0 | 42.0 |
| [Infosecurity Europe調査、経営層の脅威インテリジェンス理解不足を警告](https://www.infosecurity-magazine.com/news/business-leaders-struggle-threat/) | 20.0 | 20.0 | 42.0 |
| [Dashlaneのブルートフォース攻撃により限定的な暗号化Vaultダウンロードが発生](https://www.securityweek.com/dashlane-brute-force-attack-leads-to-limited-encrypted-vault-downloads/) | 20.0 | 20.0 | 42.0 |

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
