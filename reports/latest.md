# 📡 サイレーダー 2026-11-05 05:00 JST

このレポートは、2026-11-04 17:00 JST〜2026-11-05 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 90
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 62

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-55040: CISA KEV catalog addition](#topic-27420) | 47.0 | 74.0 | 60.0 | 音声 | 温度感上位枠 |
| 2 | [CISA flags WordPress RCE flaw as actively exploited in attacks](#topic-41282) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Cyber researchers issue warning over 'hybrid AI' ransomware capabilities after attacks on schools](#topic-41300) | 41.0 | 30.0 | 42.0 | 音声 | AI×Security枠 |
| 4 | [3AM Ransomware Used Human-AI Hybrid Tactics in UK School Estate Compromise](#topic-41286) | 33.0 | 30.0 | 42.0 | 音声 | AI×Security枠 |
| 5 | [Rigged Coding Assignment, Abused AI Tool Opened Path to $6 Billion Binance Heist](#topic-41303) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-27420"></a>

### 1. CVE-2026-55040: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 47.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 60.0 |

#### 概要

CVE-2026-55040: CISA KEV catalog addition について、公開記事が報じた内容をもとに整理しています。
関係組織、影響範囲、実務上の確認ポイントを参照リンクとスコア根拠から確認します。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 自組織で対象製品・関連資産を利用しているか確認する。
- ベンダー公式情報または公的機関情報を優先確認する。
- 対象バージョンか確認する。
- 修正版・緩和策の適用状況を確認する。
- インターネット露出の有無を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-55040 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-55040](https://nvd.nist.gov/vuln/detail/CVE-2026-55040) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [The Race Against the 3-Day Clock: How Rapid7 Helps Meet BOD 26-04 Compliance](https://www.rapid7.com/blog/post/it-racing-the-three-day-clock-cisa-bod-26-04) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers exploit critical SharePoint flaw after PoC goes public (CVE-2026-55040](https://www.helpnetsecurity.com/2026/08/13/microsoft-sharepoint-cve-2026-55040-poc-exploit/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit SharePoint Authentication Bypass After Public PoC Release](https://thehackernews.com/2026/08/attackers-exploit-sharepoint.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-41282"></a>

### 2. CISA flags WordPress RCE flaw as actively exploited in attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAが、最近修正されたWordPressの高深刻度脆弱性について、実際の攻撃で悪用が始まっていると注意喚起しました。
対象の問題はリモートでコード実行につながる可能性があるとされ、すでにパッチが提供されています。
公開後まもなく悪用が確認されるタイプの脆弱性は、未対応のサイトに被害が広がりやすいため注目されています。
WordPressは利用範囲が広く、対応の遅れがそのままリスク増大につながります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- WordPress本体と関連コンポーネントを最新状態に更新し、適用状況を優先確認する。
- 外部公開中のWordPressサイトは、管理画面や不審な改ざん・異常なアクセスの有無を点検する。
- WAFや監視ルールを見直し、同種の攻撃兆候を早期に検知できるようにする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | WordPress | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA flags WordPress RCE flaw as actively exploited in attacks](https://www.bleepingcomputer.com/news/security/cisa-flags-wordpress-rce-flaw-as-actively-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-41300"></a>

### 3. Cyber researchers issue warning over 'hybrid AI' ransomware capabilities after attacks on schools

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者らは、学校を狙った攻撃を受けて、ランサムウェアの一部でAIを組み合わせた「ハイブリッドAI」的な手口が使われた可能性について注意を呼びかけています。
材料によれば、3AMランサムウェアグループに関連するキャンペーンで、AIを用いた自動化が関与したとされています。
AIの活用が確認されれば、攻撃の自動化や大量化が進み、防御側の対応負荷が高まる可能性があります。
教育機関を含む組織にとって、従来のランサムウェア対策に加えてAI支援型の攻撃も想定した備えが必要になるためです。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIを使った攻撃の可能性を前提に、メール・認証・端末保護など基本対策の再点検を進める。
- ランサムウェア対策として、バックアップの隔離保管と復旧手順の確認を優先する。
- 教育機関や関連事業者は、フィッシングや不審な自動化挙動を含む異常検知の監視強化を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ランサムウェアグループ | 3AM | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Cyber researchers issue warning over 'hybrid AI' ransomware capabilities after a](https://www.itpro.com/security/ransomware/cyber-researchers-issue-warning-over-hybrid-ai-ransomware-capabilities-after-attacks-on-schools) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-41286"></a>

### 4. 3AM Ransomware Used Human-AI Hybrid Tactics in UK School Estate Compromise

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Infosecurity Magazineによると、3AMランサムウェアに関連する攻撃で、人間とAIを組み合わせたとみられる手法が用いられた可能性が示されています。
対象は英国の学校関連組織で、財務データが持ち出されたとされています。AIを組み合わせた攻撃は、従来のランサムウェア事案よりも手口の変化を示すものとして注目されます。
教育分野でも財務情報の流出が起きうることから、被害範囲の見極めと早期検知の重要性が改めて意識されます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 教育機関や関連事業者では、財務データを含む重要情報の保護とアクセス権限の点検を優先する。
- 不審な認証試行、権限昇格、データ外部送信の兆候を監視し、通常と異なる挙動を早めに把握する。
- ランサムウェア対策として、バックアップの分離保管と復旧手順の定期確認を継続する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ランサムウェアグループ | 3AM | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [3AM Ransomware Used Human-AI Hybrid Tactics in UK School Estate Compromise](https://www.infosecurity-magazine.com/news/3am-ransomware-hybrid-ai-uk-school/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-41303"></a>

### 5. Rigged Coding Assignment, Abused AI Tool Opened Path to $6 Billion Binance Heist

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Binanceの初回報告によると、巨額の資産流出は数カ月にわたる攻撃キャンペーンに起因し、3人のエンジニアの端末が侵害されたとされています。
報道では、偽装されたコーディング課題やAIツールの悪用が侵入の一因になった可能性が示されています。
大手暗号資産事業者を狙った長期的な侵害事案として、サプライチェーンや従業員端末の管理リスクを改めて示すため注目されています。
AIツールの業務利用が広がる中で、入力内容や連携先の統制が不十分だと攻撃面が広がり得る点も重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 従業員端末の保護だけでなく、開発・採用・課題提出など業務プロセス全体の不審な接点を点検する。
- AIツールの利用ルール、権限管理、機密情報の入力制御を見直す。
- 複数端末・複数工程にまたがる侵害を前提に、監視、ログ分析、異常検知の範囲を広げる。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Rigged Coding Assignment, Abused AI Tool Opened Path to $6 Billion Binance Heist](https://www.securityweek.com/rigged-coding-assignment-abused-ai-tool-opened-path-to-6-billion-binance-heist/) | <nobr>内容確認・補足情報</nobr> |

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
| [DebianとUbuntuのAPTの不具合により、MitM攻撃者が検証済みパッケージを差し替えてroot権限でコードを実行可能に](https://thehackernews.com/2026/11/debian-and-ubuntu-apt-flaw-lets-mitm.html) | 28.0 | 20.0 | 42.0 |
| [NIKKE PCゲームランチャーがハッキングされ、リモートアクセス・情報窃取マルウェアを拡散](https://www.bleepingcomputer.com/news/security/nikke-pc-game-launcher-hacked-to-spread-remote-access-data-stealing-malware/) | 28.0 | 20.0 | 42.0 |
| [Google, Partners Disrupt 1.3 Million-Device-Strong XCPE Botnet](https://www.darkreading.com/endpoint-security/google-13-million-device-strong-xcpe-botnet) | 28.0 | 20.0 | 42.0 |
| [Attacker abuses Microsoft Entra ID to target downstream MSP clients](https://www.cybersecuritydive.com/news/attacker-microsoft-entra-id-downstream-msp/873744/) | 28.0 | 20.0 | 42.0 |
| [Google Calendarを悪用したフィッシングキャンペーンがセッションを乗っ取り、MFAを回避](https://www.bleepingcomputer.com/news/security/google-calendar-phishing-campaign-hijacks-sessions-bypasses-mfa/) | 28.0 | 20.0 | 42.0 |
| [China-Aligned Group Abuses Sogou Input Method to Deliver Malware](https://www.infosecurity-magazine.com/news/slippynunchucks-sogou-dns-hijacking/) | 28.0 | 20.0 | 42.0 |
| [APT29-Linked Hackers Hijack Web Analytics Script to Deliver iOS and Android Exploits](https://thehackernews.com/2026/11/apt29-linked-hackers-hijack-web.html) | 28.0 | 20.0 | 42.0 |
| [APT29 Watering Holes Target Unpatched iPhones and Android Devices](https://www.infosecurity-magazine.com/news/apt29-watering-holes-iphones/) | 28.0 | 20.0 | 42.0 |
| [China-Aligned Hackers Hijack Sogou Input Method DNS Requests to Deploy DarkVigil Backdoor](https://thehackernews.com/2026/11/china-aligned-hackers-hijack-sogou.html) | 28.0 | 20.0 | 42.0 |
| [Russian Police Arrest 3 Suspected VasyGrek Hackers, Dismantle Criminal Infrastructure](https://thehackernews.com/2026/11/russian-police-arrest-3-suspected.html) | 28.0 | 20.0 | 42.0 |
| [富士フイルムが「磁気テープ」の製造能力を5倍に増強すると発表、AIブームによるデータアーカイブ需要増加に対応](https://gigazine.net/news/20261104-fujifilm-boost-tape-production-ai-fuels/) | 27.0 | 20.0 | 42.0 |
| [銀行系企業がAIの利用コストを約10分の1に削減した事例を公開、商用AIから自社運用モデルへの切り替えで](https://gigazine.net/news/20261104-revolut-cut-ai-cost/) | 27.0 | 20.0 | 42.0 |
| [米中間選挙で民主圧勝、「青い波」がAIブームに冷や水か 規制強化の公算](https://xtech.nikkei.com/atcl/nxt/column/18/00001/12155/) | 26.0 | 20.0 | 42.0 |
| [議事録も資料もAIが作るなら、人間は何をする？ AIエージェントへ舵を切る「Plaud」を試す](https://www.itmedia.co.jp/news/article/2611/04/2000002764/) | 26.0 | 20.0 | 42.0 |
| [Rapid7のAIマネジメントシステムがISO/IEC 42001認証を取得](https://www.rapid7.com/blog/post/ai-iso-iec-42001-certification-achieved) | 25.0 | 20.0 | 42.0 |
| [Researchers Uncover Prompt Adware Hidden in OpenAI Codex Jailbreak Toolkit](https://thehackernews.com/2026/11/researchers-uncover-prompt-adware.html) | 25.0 | 20.0 | 42.0 |
| [企業はサイバーセキュリティへの投資を増やしているが、AI監視にはなお苦戦している](https://www.cybersecuritydive.com/news/ai-security-governance-spending-dnsfilter/873725/) | 25.0 | 20.0 | 42.0 |
| [Sysdig、AIエージェント向けにランタイムセキュリティとガバナンスを追加](https://www.securityweek.com/sysdig-adds-runtime-security-and-governance-for-ai-agents/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントは最も過小評価されたリスクと指摘される Synthetic CISO の見解](https://www.akamai.com/blog/ai/2026/nov/synthetic-cisos-call-ai-agents-most-underestimated-risk) | 25.0 | 20.0 | 42.0 |
| [Impart、トラフィック経路にモデルを置かずに仮想パッチをAIで生成](https://www.helpnetsecurity.com/2026/11/04/impart-security-runtime-defense-harness/) | 25.0 | 20.0 | 42.0 |
| [AI関連の侵害が増加、WorkOS・Northflank・Trigger.devがハッキング被害を公表](https://www.securityweek.com/ai-linked-breaches-mount-as-workos-northflank-trigger-dev-disclose-hacks/) | 25.0 | 20.0 | 42.0 |
| [Agent Runtime Securityは基盤層なしでは機能しない理由](https://thehackernews.com/2026/11/radio-with-no-radar-why-agent-runtime.html) | 25.0 | 20.0 | 42.0 |
| [もしセキュリティチームが未来を見通せたら](https://www.security.com/expert-perspectives/what-if-your-security-teams-could-see-future) | 25.0 | 20.0 | 42.0 |
| [偽の採用面接が6.34億ドルのBinance窃盗につながる](https://www.helpnetsecurity.com/2026/11/04/binance-hack-north-korea-fake-job-interview/) | 25.0 | 20.0 | 42.0 |
| [SonicWall、EoLとなったGMSの脆弱性を修正せず、ファイル漏えいとデータベース改ざんの恐れ](https://thehackernews.com/2026/11/sonicwall-wont-patch-eol-gms-flaws-that.html) | 24.0 | 46.0 | 50.0 |
| [Barracuda ESGの認証回避脆弱性によりroot権限取得の道が開く](https://www.securityweek.com/barracuda-email-security-gateway-authentication-bypass-opens-path-to-root/) | 24.0 | 38.0 | 42.0 |
| [Critical Railsの脆弱性により細工されたImageMagickアップロードでサーバーファイルを書き込まれる問題](https://thehackernews.com/2026/11/critical-rails-flaw-lets-attackers.html) | 24.0 | 38.0 | 42.0 |
| [脆弱なメールスクリプトが再び狙われるクラシックな脅威](https://isc.sans.edu/diary/rss/33488) | 22.0 | 28.0 | 50.0 |
| [1つのプロンプトでHTTPヘッダーインジェクションを深刻化させる](https://portswigger.net/research/making-http-header-injection-critical-with-one-prompt) | 22.0 | 20.0 | 42.0 |
| [県立学校6校で生徒指導要録が所在不明 - 静岡県](https://www.security-next.com/192171) | 22.0 | 20.0 | 42.0 |
| [SDカードを挿入しないと時刻設定できないカーナビをジェイルブレイク](https://gigazine.net/news/20261104-carnavi-jailbreak/) | 22.0 | 20.0 | 42.0 |
| [ネット登録会員の個人情報が流出した可能性 - クラブツーリズム](https://www.security-next.com/192254) | 22.0 | 20.0 | 42.0 |
| [無印良品、クレカ「MUJI Card」カード番号全ケタ、約109万件漏えいか 不正アクセスで続報](https://www.itmedia.co.jp/news/article/2611/04/2000002885/) | 21.0 | 20.0 | 42.0 |
| [ブロックチェーン上の脆弱性突き止め、修正方法まで説明するAI JAISTが開発](https://news.mynavi.jp/techplus/article/20261104-5255031/) | 21.0 | 20.0 | 42.0 |
| [OpsShieldのサプライチェーン攻撃で配信された悪意あるcPGuard更新](https://www.securityweek.com/malicious-cpguard-updates-served-in-opsshield-supply-chain-attack/) | 20.0 | 45.0 | 42.0 |
| [Chrome 157 fixes 213 security issues, including 7 critical flaws](https://www.malwarebytes.com/blog/bugs/2026/11/chrome-157-fixes-213-security-issues-including-7-critical-flaws) | 20.0 | 28.0 | 50.0 |
| [French bank confirms cyber heist, hackers suspected to have stolen an estimated $133 million](https://therecord.media/french-bank-confirms-cyber-heist) | 20.0 | 20.0 | 42.0 |
| [Cyberattack disrupts blood storage refrigeration systems in France](https://www.bleepingcomputer.com/news/security/cyberattack-disrupts-blood-storage-refrigeration-systems-in-france/) | 20.0 | 20.0 | 42.0 |
| [mSecure tells users to change passwords but won’t say why](https://www.malwarebytes.com/blog/data-breaches/2026/11/msecure-tells-users-to-change-passwords-but-wont-say-why) | 20.0 | 20.0 | 42.0 |
| [Ukrainian news outlet Kyiv Independent hit by suspected Russian cyberattack](https://therecord.media/ukraine-kyiv-independent-cyberattack) | 20.0 | 20.0 | 42.0 |
| [mSecureパスワードマネージャーの不正アクセスでパスワードリセット警告が発生](https://www.bleepingcomputer.com/news/security/msecure-password-manager-hack-prompts-password-reset-warnings/) | 20.0 | 20.0 | 42.0 |
| [米政府のIT担当者、機密文書をエチオピアへ送信した罪を認める](https://www.theregister.com/security/2026/11/04/us-gov-it-worker-pleads-guilty-to-sending-top-secret-files-to-ethiopia/5307595) | 20.0 | 20.0 | 42.0 |
| [SonicWall warns of unpatched flaws in end-of-life GMS software](https://www.bleepingcomputer.com/news/security/sonicwall-warns-of-unpatched-flaws-in-end-of-life-gms-software/) | 20.0 | 20.0 | 42.0 |
| [インシデントは手書き管理では追いつかない](https://www.darkreading.com/cybersecurity-operations/incidents-move-fast-pen-paper) | 20.0 | 20.0 | 42.0 |
| [Agentic Data Security Firm Sentra Raises $150 Million](https://www.securityweek.com/agentic-data-security-firm-sentra-raises-150-million/) | 20.0 | 20.0 | 42.0 |
| [Cyberattack wipes cloud data at major Russian hosting provider Beget](https://therecord.media/russia-cyberattack-beget-cloud) | 20.0 | 20.0 | 42.0 |
| [French blood service hit by Europe-wide cyberattacks on refrigeration](https://therecord.media/france-cyberattack-blood-refrigeration) | 20.0 | 20.0 | 42.0 |
| [フランスの血液銀行を襲ったサイバー攻撃](https://www.helpnetsecurity.com/2026/11/04/cyberattack-hits-french-blood-banks/) | 20.0 | 20.0 | 42.0 |
| [US charges two Canadians accused of hacking US universities](https://www.bleepingcomputer.com/news/security/us-charges-two-canadians-accused-of-hacking-us-universities/) | 20.0 | 20.0 | 42.0 |
| [France Blood Service Cyber-Attack Sends Blood Storage Temperatures to 110°C](https://www.infosecurity-magazine.com/news/france-blood-service-cyberattack/) | 20.0 | 20.0 | 42.0 |
| [Canadian Extradited to US Over Cryptomining Hacks on University Supercomputers](https://www.securityweek.com/canadian-extradited-to-us-over-cryptomining-hacks-on-university-supercomputers/) | 20.0 | 20.0 | 42.0 |
| [French blood service hit by cyber attack threatening to turn stocks into “black pudding”](https://www.itpro.com/security/cyber-attacks/french-blood-service-hit-by-new-cyber-attack-threatening-to-turn-stocks-into-black-pudding) | 20.0 | 20.0 | 42.0 |
| [Cyberattack on French plasma stores is enough to make your blood boil](https://www.theregister.com/security/2026/11/04/cyberattack-on-french-plasma-stores-is-enough-to-make-your-blood-boil/5307519) | 20.0 | 20.0 | 42.0 |
| [Xen Hypervisorの脆弱性により悪意あるVMが他のVMのメモリを読み書き可能に](https://thehackernews.com/2026/11/xen-hypervisor-flaws-let-one-malicious.html) | 20.0 | 20.0 | 42.0 |
| [Poisoned cPGuardアップデートが数千台のWebホスティングサーバーを直撃](https://www.helpnetsecurity.com/2026/11/04/cpguard-update-supply-chain-compromised/) | 20.0 | 20.0 | 42.0 |
| [4年間の投資詐欺捜査で100台超のサーバーを押収](https://www.infosecurity-magazine.com/news/police-100-servers-fouryear/) | 20.0 | 20.0 | 42.0 |
| [Chrome 157、213件のセキュリティ修正を含んで公開、うち7件はCritical評価](https://www.securityweek.com/chrome-157-rolls-out-with-213-security-fixes-seven-rated-critical/) | 20.0 | 20.0 | 42.0 |
| [HackersがiOS・Android端末を狙うゼロクリック攻撃でn-day脆弱性を悪用](https://www.bleepingcomputer.com/news/security/hackers-use-n-day-exploits-in-zero-click-attacks-on-ios-android-devices/) | 20.0 | 20.0 | 42.0 |
| [Software Engineerの偽面接がBinanceの大規模窃取につながった件](https://www.infosecurity-magazine.com/news/fake-interview-software-engineer/) | 20.0 | 20.0 | 42.0 |
| [北朝鮮、Binanceハッキングへの米国主張に抗議し海上へミサイルを発射](https://www.securityweek.com/north-korea-launches-missiles-toward-the-sea-as-pyongyang-protests-against-us-claims-on-binance-hack/) | 20.0 | 20.0 | 42.0 |
| [Metaが公開したMuseの主要バグバウンティ報告、支払総額は120万ドルに到達](https://www.securityweek.com/meta-shares-top-muse-bug-bounty-findings-as-payouts-reach-1-2-million/) | 20.0 | 20.0 | 42.0 |
| [セキュリティ上の欠陥の4分の1が完全には修正されない理由](https://www.itpro.com/security/a-quarter-of-security-vulnerabilities-are-never-fully-fixed-and-ai-is-compounding-the-problem) | 20.0 | 20.0 | 42.0 |

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
