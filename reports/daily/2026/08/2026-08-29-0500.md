# 📡 サイレーダー 2026-08-29 05:00 JST

このレポートは、2026-08-28 17:00 JST〜2026-08-29 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 88
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 57

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [PaperCut NG/MF Critical Zero-Day Exploited in the Wild](#topic-29957) | 49.0 | 74.0 | 51.0 | 音声 | 温度感上位枠 |
| 2 | [ownCloud Flaw Exploited to Steal Nuclear Records From Philippine Research Body](#topic-29909) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [China-Made ZBT Routers Ship With Two Implants Giving Unauthenticated Attackers Root Access](#topic-29947) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [社内システムがランサム感染、個人情報流出の可能性 - ハンズHD](#topic-29926) | 38.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [PaperCut releases second emergency patch for exploited flaws](#topic-29898) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [UAT-10147 Uses AI-Assisted Workflows to Deploy SPECTRE Backdoor](#topic-29904) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [Frontier AI tipping the scales toward cyber adversaries](#topic-29914) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-29957"></a>

### 1. PaperCut NG/MF Critical Zero-Day Exploited in the Wild

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>Exploit Kit</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 49.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

PaperCut NG/MF に影響するゼロデイ脆弱性について、悪用が観測されたとしてベンダーが緊急対応を進めています。
後に CVE-2026-81578 として管理され、認証回避につながる問題を含む複数の不備が組み合わさって、深刻な影響につながる可能性があるとされています。
印刷管理基盤として企業や教育機関で広く使われる製品であり、公開 Web 経由で到達可能な環境では影響が大きくなりやすいです。
過去にも同製品の脆弱性が広く悪用された経緯があり、今回も迅速な対処が求められます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- PaperCut NG/MF を利用している場合は、該当バージョン向けの最新緊急パッチ適用状況を直ちに確認する。
- PaperCut の Web インターフェースを公開している環境では、信頼できる IP のみにアクセスを制限し、外部からの到達を最小化する。
- server.log の欠落・切り詰め・削除、または不審なエラー記録など、ベンダーが示す異常の有無を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-81578 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-81578](https://nvd.nist.gov/vuln/detail/CVE-2026-81578) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [PaperCut NG/MF Critical Zero-Day Exploited in the Wild](https://www.rapid7.com/blog/post/etr-papercut-ng-mf-critical-zero-day-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-29909"></a>

### 2. ownCloud Flaw Exploited to Steal Nuclear Records From Philippine Research Body

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、ownCloudに影響する重大な脆弱性CVE-2023-49105をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
報道によると、この脆弱性はフィリピンの研究機関を狙う攻撃に悪用されたとされており、対象には核関連の記録が含まれていたと伝えられています。
実際の悪用が報告されているため、単なる理論上の脆弱性ではなく、対応の優先度が高い事案と受け止められています。
KEV掲載は、未修正環境が継続的に狙われる可能性を示す重要なシグナルです。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ownCloudの該当バージョンや公開状況を確認し、速やかに修正済みバージョンへの更新を検討する。
- インターネット公開中のownCloudインスタンスがないか棚卸しし、不要な公開を見直す。
- 関連ログを確認し、不審なアクセスや設定変更、未知のアカウント作成がないか点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ownCloud Flaw Exploited to Steal Nuclear Records From Philippine Research Body](https://thehackernews.com/2026/08/snowflake-github-actions-flaw-lets.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-29947"></a>

### 3. China-Made ZBT Routers Ship With Two Implants Giving Unauthenticated Attackers Root Access

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

ZBT製ルーターのファームウェアに、未認証の遠隔攻撃者がroot権限でコマンドを実行できる可能性のある、未公開の工場出荷時インプラント2件が見つかったと報告されています。
これらはそれぞれCVE-2026-74232、CVE-2026-74233として追跡されています。
認証なしで高権限の操作につながる可能性があるため、対象機器ではネットワーク境界の突破や設定改ざんのリスクが高まります。
ルーターは通信の要所であり、影響があれば社内外の広い範囲に波及し得ます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象機器の機種・ファームウェア版を確認し、ベンダーや配布元の更新情報を継続監視する。
- 外部公開している管理画面や不要なリモート管理機能がないか点検し、露出を最小化する。
- 異常な再起動、設定変更、未知のプロセス実行など、ルーター上の不審挙動を監視する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [China-Made ZBT Routers Ship With Two Implants Giving Unauthenticated Attackers R](https://thehackernews.com/2026/08/china-made-zbt-routers-ship-with-two.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-29926"></a>

### 4. 社内システムがランサム感染、個人情報流出の可能性 - ハンズHD

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 38.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

ハンズホールディングスは、社内システムへのマルウェア感染について、ランサムウェアによる被害だったと明らかにしました。
従業員の個人情報が流出した可能性があるとしており、影響範囲の確認が続いているとみられます。
ランサムウェア被害は業務停止だけでなく、個人情報の流出につながる可能性があるため、企業の事業継続と情報管理の両面で重要です。
従業員情報を含むインシデントは、通知対応や再発防止策の整備状況も注目されます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 社内システムの侵害を前提に、アカウント管理、端末保護、バックアップ運用の見直しを確認する。
- 従業員情報など個人データを扱うシステムの保護状況と、漏えい時の連絡・対応手順を点検する。
- ランサムウェアを想定した初動対応、隔離、復旧、関係部署への連携手順が実際に機能するか確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [社内システムがランサム感染、個人情報流出の可能性 - ハンズHD](https://www.security-next.com/189528) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-29898"></a>

### 5. PaperCut releases second emergency patch for exploited flaws

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

PaperCut NG/MF において、初回の修正を回避できる複数の方法が見つかったとして、同社が2回目の緊急セキュリティ更新を公開しました。
対象となった脆弱性は実際に悪用されているとされ、既存の修正だけでは不十分だったことが示唆されています。
印刷管理ソフトは企業内で広く使われることがあり、影響を受ける環境では迅速な更新対応が重要です。すでに悪用が観測されている点から、放置すると侵害リスクが高まる可能性があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- PaperCut NG/MF を利用している場合は、適用済みの更新が最新か再確認し、追加の緊急パッチを優先して適用する。
- 公開情報ベースで、当該製品の露出状況や更新漏れがないかを点検する。
- 不審な管理画面アクセスや関連ログの急増がないか確認し、異常があれば早めに調査する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [PaperCut releases second emergency patch for exploited flaws](https://www.bleepingcomputer.com/news/security/papercut-releases-second-emergency-patch-for-exploited-flaws/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-29904"></a>

### 6. UAT-10147 Uses AI-Assisted Workflows to Deploy SPECTRE Backdoor

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>A⁠I</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Cisco Talosの分析として、UAT-10147とされる脅威アクターが、AI支援の手法を含む複数の攻撃ワークフローを使い、SPECTREバックドアを展開していると報告されています。
対象はインターネット公開のWindowsおよびLinuxサーバーで、政府、教育、メディア、技術、ゲーム分野などが含まれます。
AI支援の運用が、既知脆弱性の悪用や各種ツールの組み合わせをより効率化している可能性が示されており、従来型の防御だけでは見逃しやすい点が注目されています。
SPECTREは横展開後の操作、認証情報窃取、検知回避などに関わる機能があるとされ、侵害後の影響が広がりやすい点も懸念されます。

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

- インターネット公開のWindows/Linuxサーバーについて、脆弱性管理と露出資産の棚卸しを優先する。
- EDRやログだけに依存せず、認証情報の保護、権限分離、異常なプロセス挙動の監視を組み合わせる。
- 不審なバックドアやドライバ利用の兆候に備え、インシデント対応手順と復旧手順を事前に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [UAT-10147 Uses AI-Assisted Workflows to Deploy SPECTRE Backdoor](https://blog.polyswarm.io/uat-10147-uses-ai-assisted-workflows-to-deploy-spectre-backdoor) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-29914"></a>

### 7. Frontier AI tipping the scales toward cyber adversaries

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Palo Alto NetworksのUnit 42によると、攻撃者がAIを悪用してサイバー攻撃を加速させている可能性があるとされています。
現時点では、従来の防御策だけでは対応しきれない場面が増える懸念が示されています。AIの活用は攻撃の自動化や効率化につながり、防御側の検知・対応の負荷を高めます。
AIを前提にした脅威の変化として、企業のセキュリティ運用や対策見直しの材料になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 生成AIや自動化ツールの利用状況を踏まえ、検知ルールや監視の見直しを検討する。
- フィッシングやなりすましなど、AIで巧妙化しやすい脅威への訓練・注意喚起を強化する。
- 脅威情報とインシデント対応手順を、従来型の手口だけでなくAI悪用も想定して点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Frontier AI tipping the scales toward cyber adversaries](https://www.cybersecuritydive.com/news/frontier-ai-tipping-scales-cyber-adversaries/829088/) | <nobr>内容確認・補足情報</nobr> |

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
| [ゼロデイ優位性：Akamaiが業界公開前に防御する方法](https://www.akamai.com/blog/security/2026/aug/zero-day-akamai-defends-before-industry-discloses) | 37.0 | 38.0 | 43.0 |
| [PaperCutが悪用されたゼロデイ脆弱性に緊急パッチを公開](https://www.securityweek.com/papercut-releases-emergency-patch-for-exploited-zero-day/) | 37.0 | 38.0 | 43.0 |
| [PaperCutのゼロデイ脆弱性が攻撃で悪用、NGおよびMFの全バージョンに影響](https://thehackernews.com/2026/08/papercut-zero-day-exploited-in-attacks.html) | 37.0 | 38.0 | 43.0 |
| [その他のニュース：Log4jのRCE懸念、Minimusのサービス終了、イラン人ハッカーへの制裁](https://www.securityweek.com/in-other-news-log4j-rce-scare-minimus-shutdown-iranian-hacker-sanctions/) | 32.0 | 48.0 | 42.0 |
| [Socket、Microsoft Edge拡張機能のエコシステムを保護へ](https://socket.dev/blog/edge-extension-security) | 30.0 | 20.0 | 42.0 |
| [ATF、ランサムウェア攻撃主張を受けサイバーインシデントを確認](https://www.securityweek.com/atf-confirms-cyber-incident-after-ransomware-group-claims-attack/) | 28.0 | 30.0 | 42.0 |
| [ChromeとEdgeの19件の拡張機能でウォレット窃取と暗号資産流出のコードを確認](https://thehackernews.com/2026/08/19-chrome-and-edge-extensions-found.html) | 28.0 | 20.0 | 42.0 |
| [偽のボイスメールSVG添付ファイルを悪用した大規模フィッシングキャンペーン](https://www.infosecurity-magazine.com/news/fake-voicemail-svg-files-bypass/) | 28.0 | 20.0 | 42.0 |
| [APT28関連のHOOKEDGEバックドアが欧州の政府・外交機関を標的にする](https://thehackernews.com/2026/08/apt28-linked-hookedge-backdoor-targets.html) | 28.0 | 20.0 | 42.0 |
| [中国製AIモデル「GLM-5.3」が約束通りオープンモデルとして無償公開される、Claude Fable 5やGPT-5.6 Solに匹敵する高性能モデル](https://gigazine.net/news/20260829-glm-5-3-open/) | 27.0 | 20.0 | 42.0 |
| [eSIM内蔵イヤホンで会話を録音・文字起こし・要約してAIエージェントにプレゼン資料作成などをお願いできるウェアラブルAI「Plaud One」が登場](https://gigazine.net/news/20260828-plaud-one/) | 27.0 | 20.0 | 42.0 |
| [Shai-HuludハッカーによるTeamPCPの世界規模サプライチェーン犯罪でOpenAIなど数千件被害、男女2人を起訴](https://www.bitdefender.com/en-us/blog/hotforsecurity/shai-hulud-hackers-charged-teampcps) | 25.0 | 45.0 | 42.0 |
| [AI脅威の増加でオフェンシブセキュリティへの投資が急増](https://www.darkreading.com/cybersecurity-operations/offensive-security-investments-surge-ai-threats-increase) | 25.0 | 20.0 | 42.0 |
| [AIによって脆弱性発見は加速しているが、防御側は追いつけるのか？](https://www.bleepingcomputer.com/news/security/ai-is-accelerating-vulnerability-discovery-can-defenders-keep-up/) | 25.0 | 20.0 | 42.0 |
| [AIのキルスイッチを定義するのは難しいが必要である](https://www.darkreading.com/cybersecurity-operations/defining-ai-kill-switch-hard-but-necessary) | 25.0 | 20.0 | 42.0 |
| [OpenAI Agentsが自社システム上でLinuxカーネルの脆弱性を悪用された件](https://www.securityweek.com/openai-agents-exploited-linux-kernel-flaw-on-companys-own-systems/) | 25.0 | 20.0 | 42.0 |
| [Hugging Faceを攻撃したAIエージェント群は未来への警告である](https://www.malwarebytes.com/blog/ai/2026/08/the-ai-agent-swarm-that-attacked-hugging-face-is-a-warning-for-the-future) | 25.0 | 20.0 | 42.0 |
| [OpenAI主導のサイバー防衛誓約に主要テクノロジー・セキュリティ企業が賛同](https://www.securityweek.com/tech-cybersecurity-giants-unite-behind-openai-led-cyber-defense-pledge/) | 25.0 | 20.0 | 42.0 |
| [問題を生み出した業界が、その解決策を売ろうとしている話](https://www.theregister.com/security/2026/08/28/industry-that-built-the-problem-offers-to-sell-you-the-solution/5293207) | 25.0 | 20.0 | 42.0 |
| [中国製AIを排除したつもりでも要注意、Ciscoが指摘するモデルの系譜確認](https://www.securityweek.com/think-youve-eliminated-chinese-ai-check-the-models-lineage-cisco-says/) | 25.0 | 20.0 | 42.0 |
| [「脅威の状況は急速に変化している」CrowdStrike CEOジョージ・カーツ氏、AIがサイバーセキュリティのリスクを高めると警告し、同社は「過去最大の市場機会」に乗り出す](https://www.itpro.com/security/the-threat-landscape-is-moving-so-quickly-crowdstrike-ceo-george-kurtz-warns-ai-is-raising-the-stakes-in-cybersecurity-and-the-firm-is-poised-to-capitalize-on-the-largest-market-opportunity-in-our-history) | 25.0 | 20.0 | 42.0 |
| [AIを活用したサイバー攻撃の急増に対処する猶予は狭まりつつあると大手IT企業が警告](https://www.infosecurity-magazine.com/news/window-ai-attacks-narrowing-tech/) | 25.0 | 20.0 | 42.0 |
| [Anthropic 機器とAI接続規格開発](https://news.yahoo.co.jp/pickup/6593415?source=rss) | 25.0 | 20.0 | 42.0 |
| [Unitree G1 EDU人型ロボットの2件の脆弱性でroot権限のRCEが可能、1件はBluetoothから開始](https://thehackernews.com/2026/08/two-unitree-g1-edu-humanoid-robot-flaws.html) | 24.0 | 46.0 | 50.0 |
| [GiveWP WordPress寄付プラグインの脆弱性により攻撃者がサーバー上でコマンドを実行可能に](https://www.bleepingcomputer.com/news/security/givewp-wordpress-donation-plugin-flaw-lets-hackers-execute-server-commands/) | 24.0 | 38.0 | 42.0 |
| [攻撃者がPaperCutの2つの脆弱性を連鎖させ、認証なしでコードを実行](https://thehackernews.com/2026/08/attackers-chain-two-papercut-flaws-to.html) | 24.0 | 38.0 | 42.0 |
| [8,300台超のGiteaサーバーにコード実行攻撃の脆弱性](https://www.bleepingcomputer.com/news/security/over-8-300-gitea-servers-vulnerable-to-code-execution-attacks/) | 24.0 | 38.0 | 42.0 |
| [ServiceNowの3件のCVSS 10.0脆弱性で未認証の攻撃者がコード実行やSQL実行を可能にする問題](https://thehackernews.com/2026/08/three-cvss-100-servicenow-flaws-could.html) | 24.0 | 38.0 | 42.0 |
| [ServiceNowが警告する3件の最高深刻度のセキュリティ脆弱性](https://www.bleepingcomputer.com/news/security/servicenow-warns-of-three-max-severity-security-vulnerabilities/) | 22.0 | 32.0 | 42.0 |
| [Metasploitまとめ：ペイロードとエクスプロイト、そしてスキャナーも！](https://www.rapid7.com/blog/post/pt-metasploit-wrap-up-payloads-exploits-scanners) | 22.0 | 20.0 | 42.0 |
| [社内システムに脆弱性、調査で侵害痕跡を確認 - チューリッヒ保険](https://www.security-next.com/189532) | 22.0 | 20.0 | 42.0 |
| [Vulnpocalypseが変えるバグバウンティ経済の再評価](https://www.darkreading.com/vulnerabilities-threats/vulnpocalypse-repricing-bug-bounty-economy) | 22.0 | 20.0 | 42.0 |
| [教職員メルアカに不正アクセス、スパムの踏み台に - 日大法学部](https://www.security-next.com/189530) | 22.0 | 20.0 | 42.0 |
| [Adobe、セキュリティアドバイザリ7件を公開 - 6件がクリティカル](https://www.security-next.com/189564) | 22.0 | 20.0 | 42.0 |
| [WatchGuard「Fireware OS」に深刻な脆弱性 - 緊急対応を呼びかけ](https://www.security-next.com/189551) | 22.0 | 20.0 | 42.0 |
| [国防総省によるAnthropicのサプライチェーンリスク指定は違法だと連邦判事が判断](https://gigazine.net/news/20260828-anthropic-pentagon-blacklist-lawsuit/) | 22.0 | 20.0 | 42.0 |
| [イエローハット、最大180万人分の情報漏えいか 作業予約システムに不正アクセス](https://www.itmedia.co.jp/news/article/2608/28/2000000922/) | 21.0 | 20.0 | 42.0 |
| [cPanelの深刻な脆弱性により、1つのホスティング顧客がサーバー全体をroot権限で制御できる可能性](https://thehackernews.com/2026/08/critical-cpanel-flaw-could-let-one.html) | 20.0 | 28.0 | 50.0 |
| [IPTVサービスを違法配信し130万ドルを稼いだ68歳の男が収監](https://www.bleepingcomputer.com/news/security/68-year-old-imprisoned-after-making-13-million-by-pirating-iptv-services/) | 20.0 | 20.0 | 42.0 |
| [PaperCut、プリンタ管理ソフトの脆弱性を悪用する攻撃を警告](https://therecord.media/papercut-warns-of-hackers-using-printer-management-vulnerabilities) | 20.0 | 20.0 | 42.0 |
| [Android 17でOS全体にECHを追加し、ネットワーク事業者からWebサイト閲覧を隠蔽可能に](https://thehackernews.com/2026/08/android-17-adds-os-wide-ech-to-hide.html) | 20.0 | 20.0 | 42.0 |
| [従業員向けフィッシング模擬訓練入門ガイド](https://www.huntress.com/blog/a-beginners-guide-to-phishing-simulation-training-for-employees) | 20.0 | 20.0 | 42.0 |
| [自分で学ぶフィッシング攻撃](https://www.huntress.com/blog/teach-yourself-to-phish-the-strategy-behind-phishing-simulations) | 20.0 | 20.0 | 42.0 |
| [次世代フィッシングの新手口に備えよ](https://www.huntress.com/blog/advanced-phishing-tradecraft) | 20.0 | 20.0 | 42.0 |
| [米国政府の情報提供者摘発者が外国スパイに国家機密を漏洩した罪を認める](https://www.theregister.com/security/2026/08/28/us-government-snitch-finder-pleads-guilty-to-leaking-state-secrets-to-foreign-spies/5293248) | 20.0 | 20.0 | 42.0 |
| [OTにはサイバー欺瞞が必要です](https://www.darkreading.com/ics-ot-security/you-need-cyber-deception-ot) | 20.0 | 20.0 | 42.0 |
| [WhatsAppアカウントを新しいパスキーと2段階認証の強化で保護する](https://www.malwarebytes.com/blog/mobile/2026/08/protect-your-whatsapp-account-with-new-passkey-and-2fa-upgrades) | 20.0 | 20.0 | 42.0 |
| [中国のヒト型ロボ 本当の脅威は](https://news.yahoo.co.jp/pickup/6593448?source=rss) | 20.0 | 20.0 | 42.0 |
| [CISAが特定した2件のレッドチーム演習で結果を分けたセキュリティ上の障壁](https://www.cybersecuritydive.com/news/cisa-red-team-exercises-lessons-cloud-soc/828733/) | 20.0 | 20.0 | 42.0 |
| [Hasbroが従業員に影響するデータ侵害を公表](https://www.bleepingcomputer.com/news/security/toy-making-giant-hasbro-disclose-data-breach-affecting-employees/) | 20.0 | 20.0 | 42.0 |
| [2026年にIdentity Fabricが重要となる主な理由](https://thehackernews.com/2026/08/key-reasons-why-identity-fabric-matters.html) | 20.0 | 20.0 | 42.0 |
| [CISA: 最も悪用される脆弱性は数十年前に排除されているべきだった](https://www.theregister.com/security/2026/08/28/cisa-most-exploited-vulnerabilities-should-have-been-eradicated-decades-ago/5293194) | 20.0 | 20.0 | 42.0 |
| [北朝鮮系の遠隔勤務者、IT以外へも就職活動を拡大](https://www.helpnetsecurity.com/2026/08/28/north-korean-remote-workers-jobs-sales-and-marketing/) | 20.0 | 20.0 | 42.0 |
| [偽の北朝鮮系IT労働者が急増、新規採用者がハッカーか見抜く方法](https://www.itpro.com/security/fake-north-korean-it-workers-are-rampant-heres-how-to-spot-the-telltale-signs-a-new-hire-is-a-hacker) | 20.0 | 20.0 | 42.0 |
| [Manchester Airports Groupへの攻撃、最大870万人の顧客に影響した侵害の現時点で判明していること](https://www.itpro.com/security/cyber-attacks/manchester-airports-group-attack-everything-we-know-so-far-as-8-7-million-customers-impacted-in-breach) | 20.0 | 20.0 | 42.0 |
| [Android 17、新たなWi-Fi追跡やウェブ閲覧ののぞき見に対する保護を追加](https://www.helpnetsecurity.com/2026/08/28/android-17-network-security-features/) | 20.0 | 20.0 | 42.0 |
| [Windows 11のKB5120998更新プログラムが公開、35件の変更と修正を実施](https://www.bleepingcomputer.com/news/security/windows-11-kb5120998-update-released-with-35-changes-and-fixes/) | 20.0 | 20.0 | 42.0 |

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
