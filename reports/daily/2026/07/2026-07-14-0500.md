# 📡 サイレーダー 2026-07-14 05:00 JST

このレポートは、2026-07-13 17:00 JST〜2026-07-14 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 104
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 73

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2008-4128: CISA KEV catalog addition](#topic-22159) | 51.0 | 46.0 | 55.0 | 音声 | 温度感上位枠 |
| 2 | [CISA warns of actively exploited RCE flaws in Joomla extensions](#topic-22160) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [VPN service favored by ransomware groups is sanctioned by US](#topic-22147) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [⚡ Weekly Recap: ShareFile Threat, Citrix Bleed 2 Ransomware, AI Coding Attacks, and More](#topic-22161) | 33.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [BusySnake Stealer: Inside Armored Likho's AI-Assisted Malware Operation](#topic-22152) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [Attacker Uses Suspected AI-Generated PowerShell Script to Map Active Directory](#topic-22209) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-22159"></a>

### 1. CVE-2008-4128: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>K⁠E⁠V</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>i⁠O⁠S</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 51.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

CISAは、既知の悪用が確認された脆弱性としてCVE-2008-4128をKEVカタログに追加しました。
対象はCisco IOSのCSRF脆弱性で、公開情報では実際の悪用が根拠とされています。KEVへの追加は、組織に対して優先的な対応が求められるサインです。
古いCVEであっても、実際の悪用が観測されると防御上の優先度が上がります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Cisco IOSの該当製品を利用している環境は、保有資産と影響範囲を早急に確認する。
- ベンダー案内やCISAの優先度に沿って、修正・緩和策の適用可否を点検する。
- ネットワーク機器は放置されやすいため、対象機器の構成管理と更新状況の棚卸しを行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2008-4128 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2018-0171 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Apple iOS | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2008-4128](https://nvd.nist.gov/vuln/detail/CVE-2008-4128) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Officials once again warn defenders that Russian hackers are targeting network d](https://cyberscoop.com/russian-fsb-cisco-joint-cybersecurity-advisory/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/07/13/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-22160"></a>

### 2. CISA warns of actively exploited RCE flaws in Joomla extensions

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>R⁠C⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、Joomla向け拡張機能であるiCagendaとBalbooa Formsに関連する脆弱性について、実際の悪用が確認されていると警告しています。
報告では、任意のファイルアップロードを通じてリモートコード実行につながる可能性があるとされています。
CMS本体ではなく拡張機能が狙われているため、Joomlaを利用する環境でも見落とされやすい点が注目されています。
実悪用が示されていることから、公開状況や更新遅れがある環境では優先的な確認が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Joomla本体だけでなく、導入済み拡張機能の有無とバージョンを確認する。
- 対象拡張機能に更新版や修正版が出ているかを確認し、適用可能なら早急に更新する。
- 管理画面やWebサーバーのログを確認し、不審なファイルアップロードや改変の兆候がないか点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-48939 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-56291 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 製品 | Joomla | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA warns of actively exploited RCE flaws in Joomla extensions](https://www.bleepingcomputer.com/news/security/cisa-warns-of-actively-exploited-rce-flaws-in-joomla-extensions/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22147"></a>

### 3. VPN service favored by ransomware groups is sanctioned by US

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

米財務省は、ランサムウェアグループの活動を支援したとして、VPNサービス「First VPN Service（1VPNS）」とそのウクライナ人管理者に制裁を科したと発表しました。
あわせて、マルウェアの暗号化解除を妨げる“cryptors”に関与したとして、ベラルーシ国籍の男性も制裁対象になったとされています。
ランサムウェア関連の支援インフラに対して、米国が制裁を通じて対処を強めていることを示す事例です。攻撃そのものだけでなく、周辺のサービスや関係者も対象になり得る点が注目されます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- VPNや匿名化系サービスの利用実態を把握し、取引先や委託先のリスク評価に反映する。
- ランサムウェア関連の制裁情報を定期的に確認し、通信・決済・外部接続の統制に活かす。
- 自組織のログやアラートで、通常と異なるVPN経由のアクセスや不審な外部接続を継続監視する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [VPN service favored by ransomware groups is sanctioned by US](https://therecord.media/first-vpn-administrator-us-sanctions-ransomware-groups) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22161"></a>

### 4. ⚡ Weekly Recap: ShareFile Threat, Citrix Bleed 2 Ransomware, AI Coding Attacks, and More

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

今週のセキュリティ動向をまとめた記事では、Citrix ShareFileに関する脅威や、Citrix Bleed 2に関連するランサムウェア事案、AIを用いたコーディング攻撃などが取り上げられています。
内容全体としては、既知の脆弱性や信頼されたコードが引き続き悪用対象になっている点が示されています。
AIを活用した攻撃と従来型の脆弱性悪用が同時に進んでおり、防御側は複数のリスクを並行して見る必要があります。
特に、修正待ちの脆弱性が残っている環境では、攻撃機会が長引きやすい点が重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Citrix製品を含む公開済み脆弱性の適用状況を確認し、優先度の高いものから更新する。
- ShareFileなど外部公開サービスは、認証・アクセス制御・監査ログの見直しを行う。
- AI支援ツールの利用時は、生成コードのレビューと依存関係の確認を徹底し、信頼しすぎない運用にする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix ShareFile | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [⚡ Weekly Recap: ShareFile Threat, Citrix Bleed 2 Ransomware, AI Coding Attacks, ](https://thehackernews.com/2026/07/weekly-recap-sharefile-threat-citrix.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22152"></a>

### 5. BusySnake Stealer: Inside Armored Likho's AI-Assisted Malware Operation

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者は、BusySnake Stealerと呼ばれる未確認のPythonベースの情報窃取型マルウェアを用いたフィッシング अभियानを確認したとしています。
対象はロシア、カザフスタン、ブラジルの政府機関や電力関連組織で、初期侵入や配布にAI支援の仕組みやモジュール型の構成が使われている可能性が示されています。
標的が政府や重要インフラに及んでいる点から、情報漏えいだけでなく運用継続への影響も懸念されます。
モジュール型で検知を回避しやすい構成は、従来のシグネチャ中心の対策だけでは追いにくい可能性があります。

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

- フィッシング起点の侵入を想定し、認証情報の保護と多要素認証の徹底を見直す。
- 端末上の不審なスクリプト実行や外部からの不自然なダウンロード挙動を監視する。
- 重要インフラ関連組織では、EDRや振る舞い検知、脅威インテリジェンスの更新状況を確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [BusySnake Stealer: Inside Armored Likho's AI-Assisted Malware Operation](https://blog.polyswarm.io/busysnake-stealer-inside-armored-likhos-ai-assisted-malware-operation) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-22209"></a>

### 6. Attacker Uses Suspected AI-Generated PowerShell Script to Map Active Directory

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

セキュリティ研究者が、Active Directoryの情報を調べるために使われたとみられるPowerShellスクリプトを確認したとしています。
スクリプトはドメインコントローラーやユーザー、コンピューター、ドメインを列挙し、結果をファイルとして出力していたとされていますが、AI生成かどうかは「疑い」の段階です。
Active Directoryは多くの企業で認証や権限管理の中核にあるため、列挙活動は後続の侵害リスクを高めます。
AI支援の可能性があるスクリプトは、攻撃の作成コストを下げる懸念があるため注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- PowerShellの実行ログやAD関連の列挙挙動を点検し、通常業務との差分を把握する。
- ドメインコントローラー周辺の監視を強め、不要な管理権限や過剰な閲覧権限を見直す。
- 不審なスクリプト実行に備え、EDRやアプリ制御、PowerShellの監査設定を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | Active Directory | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Attacker Uses Suspected AI-Generated PowerShell Script to Map Active Directory](https://thehackernews.com/2026/07/attacker-uses-suspected-ai-generated.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
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
| [悪用が確認されたJoomla拡張機能の脆弱性について組織に警告](https://www.securityweek.com/organizations-warned-of-exploited-joomla-extension-vulnerabilities/) | 32.0 | 38.0 | 42.0 |
| [ロシアによる国家支援型標的型攻撃から守るためのルーター衛生管理の強化](https://www.cisa.gov/news-events/cybersecurity-advisories/aa26-194a) | 30.0 | 40.0 | 50.0 |
| [ランサムウェア交渉役・関係者に実刑判決](https://www.helpnetsecurity.com/2026/07/13/ransomware-negotiator-blackcat-sentence/) | 28.0 | 30.0 | 42.0 |
| [6月のランサムウェア攻撃の約5分の1を占めた単一のサイバー犯罪グループ](https://www.itpro.com/security/ransomware/this-one-cyber-crime-group-accounted-for-nearly-a-fifth-of-all-ransomware-attacks-in-june) | 28.0 | 30.0 | 42.0 |
| [ウクライナから送還されたハッカー、Ryukランサムウェア関連の罪を認める](https://www.infosecurity-magazine.com/news/hacker-extradited-ukraine-guilty/) | 28.0 | 30.0 | 42.0 |
| [HackersがJscramblerのnpmパッケージに情報窃取マルウェアを仕込む](https://www.bleepingcomputer.com/news/security/hackers-backdoor-jscrambler-npm-package-with-infostealer-malware/) | 28.0 | 20.0 | 42.0 |
| [Appleのクラッシュ報告ツールを装う新たなCrashStealerマルウェア](https://www.bleepingcomputer.com/news/security/new-crashstealer-malware-poses-as-apple-crash-reporting-tool/) | 28.0 | 20.0 | 42.0 |
| [CrashStealer macOSマルウェア、Notarizedドロッパーを使ってGatekeeperチェックを回避](https://thehackernews.com/2026/07/crashstealer-macos-malware-uses.html) | 28.0 | 20.0 | 42.0 |
| [GigaWiperで攻撃者が破壊的攻撃を任意に選択可能に](https://www.darkreading.com/cyberattacks-data-breaches/gigawiper-threat-actors-choose-their-own-destructive-attack) | 28.0 | 20.0 | 42.0 |
| [Breach at the Beach: Entra IDの究極CTFをプレイしよう](https://www.bleepingcomputer.com/news/security/breach-at-the-beach-play-the-ultimate-entra-id-ctf/) | 28.0 | 20.0 | 42.0 |
| [Cloudflare Precursor、継続的な行動分析で高度なボットを阻止](https://www.helpnetsecurity.com/2026/07/13/cloudflare-precursor/) | 28.0 | 20.0 | 42.0 |
| [脅威アクターがSQLインジェクション後も永続性を確立](https://www.huntress.com/blog/sql-injection-attacker-persistence) | 28.0 | 20.0 | 42.0 |
| [EU、ロシア情報機関の関係者による長期サイバースパイ活動を非難・制裁へ](https://www.securityweek.com/eu-targets-russian-intelligence-officers-accused-of-running-a-yearslong-cyber-spying-campaign/) | 28.0 | 20.0 | 42.0 |
| [Australian Cyber Agencyが警告するグローバルCMS悪用キャンペーン](https://www.infosecurity-magazine.com/news/australia-warns-global-cms/) | 28.0 | 20.0 | 42.0 |
| [画像に悪意あるAI指示を隠すGhostcommit攻撃](https://www.malwarebytes.com/blog/ai/2026/07/ghostcommit-attack-hides-malicious-ai-instructions-in-images) | 27.0 | 20.0 | 42.0 |
| [「Yellow Team」が切り拓くAIセキュリティの未来](https://www.darkreading.com/cybersecurity-operations/yellow-teams-defining-future-ai-security) | 25.0 | 20.0 | 42.0 |
| [1通のメールでAIエージェントに持続的な偽記憶を植え付ける新たなMemGhost攻撃](https://thehackernews.com/2026/07/new-memghost-attack-plants-persistent.html) | 25.0 | 20.0 | 42.0 |
| [Lumen、Cortex XSIAM連携でマネージド検知・対応を拡充](https://www.helpnetsecurity.com/2026/07/13/lumen-defender-amdr/) | 25.0 | 20.0 | 42.0 |
| [Forg365 PhaaSがMicrosoft 365を狙うデバイスコードとAitMによるセッション窃取攻撃](https://thehackernews.com/2026/07/forg365-phaas-targets-microsoft-365.html) | 25.0 | 20.0 | 42.0 |
| [メール詐欺師を逆手に取る「ScamBuster」](https://www.darkreading.com/cyberattacks-data-breaches/turning-tables-email-scammers-scambuster) | 25.0 | 20.0 | 42.0 |
| [Metaが一日中聞き取り、感情を追跡するAIの特許を出願](https://thehackernews.com/2026/07/meta-files-patent-for-ai-that-can.html) | 25.0 | 20.0 | 42.0 |
| [SOCにおける速い思考と遅い思考：自律型AIとアナリスト用Copilotの組み合わせが必要な理由](https://thehackernews.com/2026/07/thinking-fast-and-slow-in-soc-case-for.html) | 25.0 | 20.0 | 42.0 |
| [Claude Codeユーザーは7月19日まで利用上限が50%増加](https://www.helpnetsecurity.com/2026/07/13/claude-code-weekly-limits-promotion-extended/) | 25.0 | 20.0 | 42.0 |
| [AI生成コードがセキュリティ負債をガバナンスの課題に変えている](https://cyberscoop.com/governing-ai-code-security-risks-op-ed/) | 25.0 | 20.0 | 42.0 |
| [RabbitMQの脆弱性が企業システムを脅かす](https://www.securityweek.com/rabbitmq-vulnerability-threatens-enterprise-systems/) | 24.0 | 38.0 | 42.0 |
| [脳に電気刺激を与える治療法がわずか10日間でうつ病治療に著しい効果をもたらしたとの研究結果](https://gigazine.net/news/20260713-brain-zapping-improves-depression-10-days/) | 24.0 | 20.0 | 43.0 |
| [Microsoft Entra IDのセキュリティ更新：Entra IDでパスキーが既定の認証方式に](https://www.microsoft.com/en-us/security/blog/2026/07/13/microsoft-entra-id-security-updates-passkeys-are-the-default-authentication-method-in-entra-id/) | 22.0 | 20.0 | 42.0 |
| [高校で採点済み答案をグループウェアに誤掲載 - 宮城県](https://www.security-next.com/186975) | 22.0 | 20.0 | 42.0 |
| [支援先事業者宛のメールで誤送信 - いばらき中小企業グローバル推進機構](https://www.security-next.com/187131) | 22.0 | 20.0 | 42.0 |
| [イスラム過激派組織ボコ・ハラムがAIを使って爆発物の設計や武器の修理を行っていたことが判明](https://gigazine.net/news/20260713-terrorist-group-use-ai/) | 22.0 | 20.0 | 42.0 |
| [Steamの「理由を問わない」返金ポリシーは悪用されやすいとインディーゲーム開発者が訴え](https://gigazine.net/news/20260713-steam-refund-policy/) | 22.0 | 20.0 | 42.0 |
| [委託先のサーバから個人情報が流出した可能性 - 韓流エンタメ会社](https://www.security-next.com/186971) | 22.0 | 20.0 | 42.0 |
| [ニチレイに不正アクセス、冷凍食品の出荷に支障 システムに障害](https://www.itmedia.co.jp/news/articles/2607/13/news128.html) | 21.0 | 20.0 | 42.0 |
| [セキュリティの新指標「日本度」発表--実質的な国内統制とコミットを可視化](https://japan.zdnet.com/article/35250503/) | 21.0 | 20.0 | 42.0 |
| [7月13日 脅威インテリジェンスレポート](https://research.checkpoint.com/2026/13th-july-threat-intelligence-report/) | 20.0 | 45.0 | 42.0 |
| [EUと英国、ポーランドの送電網へのサイバー攻撃をロシアのスパイと正式に非難](https://www.theregister.com/security/2026/07/13/uk-eu-officially-pin-poland-energy-cyberattack-on-russia/5270458) | 20.0 | 20.0 | 48.0 |
| [メール侵害を通じてTelegramチャンネルに不正アクセスされたとロシアの著名ジャーナリストKsenia Sobchakが公表](https://therecord.media/ksenia-sobchak-russian-hackers-leak) | 20.0 | 20.0 | 42.0 |
| [LidlのITサービスプロバイダーが侵害され、顧客データが窃取される](https://www.helpnetsecurity.com/2026/07/13/lidl-data-breach-customer-data/) | 20.0 | 20.0 | 42.0 |
| [欧州諸国がロシアのTurlaに対しスパイ活動と「破壊的攻撃」で対抗](https://cyberscoop.com/eu-uk-russian-cyberespionage-sanctions/) | 20.0 | 20.0 | 42.0 |
| [Open DirectoryでEvilginxを用いた3人のフィッシング運用者が露出](https://www.infosecurity-magazine.com/news/open-directory-exposes-evilginx/) | 20.0 | 20.0 | 42.0 |
| [米当局、脆弱なネットワーク機器を標的とする国家関与のハッカーについて警告](https://www.cybersecuritydive.com/news/us-authorities-state-linked-hackers-vulnerable-networking-devices-Cisco/825062/) | 20.0 | 20.0 | 42.0 |
| [CISAの最近のGitHub流出から得られた教訓](https://krebsonsecurity.com/2026/07/lessons-learned-from-cisas-recent-github-leak/) | 20.0 | 20.0 | 42.0 |
| [効果的なパッチ管理戦略：7つのベストプラクティス](https://www.huntress.com/blog/patch-management-strategy) | 20.0 | 20.0 | 42.0 |
| [EUと英国、欧州を不安定化させる試みを受けロシアのサイバー作戦要員をブラックリスト化](https://www.helpnetsecurity.com/2026/07/13/eu-uk-russia-cyber-activity-sanctions/) | 20.0 | 20.0 | 42.0 |
| [パキスタンの警察システム、中国とインドのスパイ活動の標的に](https://www.infosecurity-magazine.com/news/chinese-indian-espionage-pakistani/) | 20.0 | 20.0 | 42.0 |
| [子どものオンライン利用は信頼だけでは不十分](https://www.malwarebytes.com/blog/podcast/2026/07/trusting-your-kids-online-isnt-enough-lock-and-code-s07e14) | 20.0 | 20.0 | 42.0 |
| [ハッカーがMicrosoft Entraのユーザーデータを警戒されずに収集する新手口を発見](https://www.cybersecuritydive.com/news/microsoft-entra-user-enumeration-bypass-proofpoint/825052/) | 20.0 | 20.0 | 42.0 |
| [Hacker Conversations: Jesse McGraw（GhostExodus）— ブラックハットハッカーから更生へ](https://www.securityweek.com/hacker-conversations-jesse-mcgraw-ghostexodus-from-blackhat-hacker-to-redemption/) | 20.0 | 20.0 | 42.0 |
| [Lidl、サービスプロバイダーへの侵害を受けオンラインショップの情報漏えいを公表](https://www.bleepingcomputer.com/news/security/lidl-discloses-online-shop-breach-after-service-provider-hack/) | 20.0 | 20.0 | 42.0 |
| [Tidal Cyber、資産・脆弱性・脅威をThreat-Led Defenseでつなぐ](https://www.helpnetsecurity.com/2026/07/13/tidal-cyber-threat-led-asset-visibility/) | 20.0 | 20.0 | 42.0 |
| [英国、ロシア系通話偽装プラットフォームに関与した容疑者を起訴](https://www.bleepingcomputer.com/news/security/uk-charges-suspects-linked-to-russian-coms-call-spoofing-platform/) | 20.0 | 20.0 | 42.0 |
| [クラウド環境を狙う新たなOAuthクライアントID詐称手法](https://www.infosecurity-magazine.com/news/novel-spoofing-technique-targets/) | 20.0 | 20.0 | 42.0 |
| [なぜIaCのカバレッジをセキュリティダッシュボードに表示すべきか](https://www.wiz.io/blog/iac-coverage-security-dashboard) | 20.0 | 20.0 | 42.0 |
| [サイバーセキュリティM&A速報：2026年6月に発表された37件の取引](https://www.securityweek.com/cybersecurity-ma-roundup-37-deals-announced-in-june-2026/) | 20.0 | 20.0 | 42.0 |
| [偽のOAuthクライアントIDが攻撃者のサインインログをすり抜けるのを助けている](https://www.helpnetsecurity.com/2026/07/13/entra-id-oauth-client-id-spoofing/) | 20.0 | 20.0 | 42.0 |
| [Progress SoftwareがShareFileへの外部セキュリティ脅威を警告](https://www.infosecurity-magazine.com/news/progress-warns-security-threat/) | 20.0 | 20.0 | 42.0 |
| [World Cupの因縁攻撃者、1年前のインフォスティーラー感染経由でアルゼンチンサッカー協会への侵入に成功か](https://www.theregister.com/security/2026/07/13/world-cup-grudge-attackers-may-have-scored-argentine-fa-access-via-year-old-infostealer-infection/5270302) | 20.0 | 20.0 | 42.0 |
| [英国と同盟国、ロシア諜報機関の標的化に備え重要分野に防御強化を促す](https://www.ncsc.gov.uk/news/uk-and-allies-urge-critical-sectors-to-improve-defences-against-russian-intelligence-targeting) | 20.0 | 20.0 | 42.0 |
| [Security threatによりProgressがShareFileアカウントを無効化、顧客にサーバー停止を要請](https://www.helpnetsecurity.com/2026/07/13/progress-sharefile-security-threat/) | 20.0 | 20.0 | 42.0 |
| [NCSCがロシア情報機関支援の脅威グループについて警告を発表](https://www.itpro.com/security/ncsc-issues-warning-over-russian-intelligence-backed-threat-group) | 20.0 | 20.0 | 42.0 |
| [EU、サイバー攻撃を行ったロシアGRUの軍事ハッカーに制裁](https://www.bleepingcomputer.com/news/security/eu-and-uk-hit-russia-with-first-joint-cyber-sanctions-package/) | 20.0 | 20.0 | 42.0 |
| [偽の暗号資産ギフトカードサイトを見分けるのが難しくなっている](https://www.malwarebytes.com/blog/threat-intel/2026/07/fake-crypto-gift-card-sites-are-getting-harder-to-spot) | 20.0 | 20.0 | 42.0 |
| [ロシア系国家ハッカーが世界中の脆弱なルーターを標的に、共同勧告が警告](https://www.infosecurity-magazine.com/news/russian-state-hackers-vulnerable/) | 20.0 | 20.0 | 42.0 |
| [Progress、謎のセキュリティ脅威によりShareFileサーバーの緊急停止を実施](https://www.theregister.com/security/2026/07/13/progress-orders-emergency-sharefile-server-shutdown-over-mystery-security-threat/5270281) | 20.0 | 20.0 | 42.0 |
| [ニチレイ、不正アクセスによるシステム障害が発生。入出庫などの業務に影響](https://internet.watch.impress.co.jp/docs/news/2124795.html) | 20.0 | 20.0 | 42.0 |
| [Zimbraの重大なコード実行脆弱性を修正](https://www.securityweek.com/zimbra-patches-critical-code-execution-vulnerability/) | 20.0 | 20.0 | 42.0 |
| [MITRE ATT&CK T1140とT1105における検知のギャップ](https://www.security.com/expert-perspectives/detection-gap-mitre-attck-t1140-and-t1105) | 20.0 | 20.0 | 42.0 |
| [米国と同盟国が警告するロシアによる重要インフラ攻撃](https://www.bleepingcomputer.com/news/security/us-and-allies-share-defense-tips-against-russian-hackers-targeting-critical-infrastructure/) | 20.0 | 20.0 | 42.0 |
| [FastNetMon、NetomicsでサードパーティのBGPルックアップを排除](https://www.helpnetsecurity.com/2026/07/13/fastnetmon-netomics/) | 20.0 | 20.0 | 42.0 |
| [企業の従業員が一日で行う最も危険なことはコピペかもしれない](https://www.cybersecuritydive.com/spons/copy-paste-might-be-the-riskiest-thing-your-enterprise-employees-do-all-day/824419/) | 20.0 | 20.0 | 42.0 |
| [サイバー犯罪者が情報の流れを上回るとき](https://www.cybersecuritydive.com/spons/when-cybercriminals-outrun-the-feed/824053/) | 20.0 | 20.0 | 42.0 |
| [Progress ShareFile Storage Zone Controllerのセキュリティ懸念によるシャットダウン要請](https://www.securityweek.com/progress-prompts-sharefile-storage-zone-controller-shutdown-amid-security-concerns/) | 20.0 | 20.0 | 42.0 |
| [Centers Laboratoryのデータ侵害、54万人に影響](https://www.securityweek.com/centers-laboratory-data-breach-affects-540000-individuals/) | 20.0 | 20.0 | 42.0 |

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
