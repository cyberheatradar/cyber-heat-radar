# 📡 サイレーダー 2026-07-09 05:00 JST

このレポートは、2026-07-08 17:00 JST〜2026-07-09 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 99
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 67

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CISA Urges Immediate Patching of Exploited ColdFusion, Langflow, Joomla Flaws](#topic-21403) | 38.0 | 38.0 | 47.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [CVE-2026-55255: CISA KEV catalog addition](#topic-21487) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 3 | [Felons, Fraudsters Flog Offensive Cybersecurity Startup](#topic-21507) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [New HalluSquatting Attack Could Trick AI Coding Assistants Into Installing Botnet Malware](#topic-21480) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Threat Actors Uses Agentic AI to Rapidly Compromise Cloud Target](#topic-21508) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [Thousands of malicious AI skills found capable of stealing data, running malware](#topic-21539) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [Codenotary launches AI security platform that learns from AI agent behavior](#topic-21546) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-21487"></a>

### 1. CVE-2026-55255: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

CISAが、Langflowに関する脆弱性CVE-2026-55255をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
公開情報では、同脆弱性が実際に悪用されている可能性が示されており、認証情報の収集に使われたとする報道もあります。
KEVへの追加は、攻撃者に実際に利用されていると判断された脆弱性であることを示すため、優先対応が必要になりやすい点が重要です。
LangflowはAIワークフロー構築に使われるため、利用組織の影響範囲が広がる可能性があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Langflowの利用有無と影響を確認し、該当環境を優先的に棚卸しする。
- ベンダーやCISAの案内に基づき、修正済みバージョンや回避策の適用状況を確認する。
- 認証情報の不審な使用やアクセスログの異常がないかを点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-55255 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 製品 | Langflow | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-55255](https://nvd.nist.gov/vuln/detail/CVE-2026-55255) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Attackers using Langflow flaw for credential harvesting (CVE-2026-55255)](https://www.helpnetsecurity.com/2026/07/08/langflow-vulnerability-cve-2026-55255-exploited/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21507"></a>

### 2. Felons, Fraudsters Flog Offensive Cybersecurity Startup

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

公開情報によると、ゼロデイ脆弱性の買い取りをうたうサイバーセキュリティ系スタートアップについて、その運営者の経歴や過去の事業実態に疑義があると報じられています。
報道では、以前の事業で使われた名称や活動内容にも不審点があるとされています。脆弱性の売買を扱う事業は、運営主体の信頼性が極めて重要です。
実在性や過去の経歴に懸念がある場合、研究者や取引先が関与可否を慎重に見極める必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 脆弱性報告や取引の際は、相手組織の実在性・法人情報・連絡経路を改めて確認する。
- 高額報酬や条件の良さだけで判断せず、契約条件、支払い実績、情報の取り扱い方針を精査する。
- 不審点がある場合は、社内の法務・CSIRT・調達部門で共有し、個別対応を避ける。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Felons, Fraudsters Flog Offensive Cybersecurity Startup](https://krebsonsecurity.com/2026/07/felons-fraudsters-flog-offensive-cybersecurity-startup/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21480"></a>

### 3. New HalluSquatting Attack Could Trick AI Coding Assistants Into Installing Botnet Malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

AIコーディング支援ツールが、存在しないプロジェクト名やパッケージ名をもっともらしく生成してしまう性質を悪用する新しい手法が紹介されています。
研究では、こうした“幻の名前”を先回りして登録し、支援ツール経由の取得先として誘導することで、意図しないソフトウェア導入につながり得るとされています。
開発者がAIの提案をそのまま信頼すると、正規に見えるが実際には別物のリポジトリやパッケージへ誘導されるリスクがあります。
AI支援開発の利用が広がるほど、サプライチェーン面の確認不足が影響しやすくなります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIが提案したパッケージ名やリポジトリ名は、その実在性と配布元の正当性を人手で確認する。
- 依存関係の追加や取得は、公式ドキュメントや既知の公開元と照合してから行う。
- AI支援ツールの利用時は、名前の曖昧さや自動取得機能に対する運用ルールを定める。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New HalluSquatting Attack Could Trick AI Coding Assistants Into Installing Botne](https://thehackernews.com/2026/07/new-hallusquatting-attack-could-trick.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21508"></a>

### 4. Threat Actors Uses Agentic AI to Rapidly Compromise Cloud Target

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

脅威アクターがエージェント型AIを用い、クラウド環境への侵入から展開までの所要時間を大幅に短縮したとする報告が紹介されています。
Sygniaの報告として、従来は数週間かかると見られる攻撃の流れが72時間に圧縮されたとされています。
攻撃側がAIを使って作業を高速化・効率化している可能性を示す事例として注目されています。クラウド運用では、検知や初動対応の猶予がこれまで以上に短くなる懸念があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- クラウドの監視とアラート対応の遅延を見直し、初動の判断基準を再確認する。
- ID・権限・認証情報の保護を強化し、異常な権限昇格や横展開の兆候を重点監視する。
- AIを悪用した自動化前提で、侵害後のスピードを想定したインシデント対応手順を確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Threat Actors Uses Agentic AI to Rapidly Compromise Cloud Target](https://www.infosecurity-magazine.com/news/threat-actor-agentic-ai-cloud/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21539"></a>

### 5. Thousands of malicious AI skills found capable of stealing data, running malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

ESETの脅威レポートをもとに、AIエージェント向けの「スキル」に悪意あるものが混在し、データ窃取やマルウェア実行、挙動の誘導に悪用され得ると報じられています。
公開情報では、約90万件のAIスキルを分析した結果、2万5000件超が不審とされたとされています。
AIエージェントは外部サービスやデータに広く触れるため、周辺のスキル管理が不十分だと攻撃面が広がります。
生成AIの導入が進むほど、モデル本体だけでなく周辺設定や拡張機能の検査が重要になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIエージェントに追加するスキルや拡張機能は、提供元・権限・挙動を確認し、不要なものは入れない。
- 外部データ参照やコマンド実行を許す構成では、最小権限と分離を徹底し、機密データへのアクセス範囲を絞る。
- 新規追加・更新時は監査ログや異常動作の監視を強め、想定外の通信や操作を早期に検知できるようにする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | ESET | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Thousands of malicious AI skills found capable of stealing data, running malware](https://www.helpnetsecurity.com/2026/07/08/eset-ai-threat-trends-report/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21546"></a>

### 6. Codenotary launches AI security platform that learns from AI agent behavior

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Codenotaryが、AIエージェントの挙動を学習して適応的に動作する企業向けAIセキュリティ基盤「AgentMon 3」を発表しました。
ユーザー固有の業務フローや観測された振る舞い、新たな脅威に応じてランタイムの保護方針を更新する点が特徴です。あわせてAWS Marketplaceでの提供も案内されています。
AIエージェントの利用が広がる中、実行時の挙動監視と保護をどう継続的に更新するかは重要な論点です。
AWS環境での導入しやすさもあり、企業のAI運用・セキュリティ設計に関わる話題として注目されます。

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

- AIエージェントの監視対象と許可範囲を、業務ごとに明確に定義できるか確認する。
- 動的に変化する保護ポリシーが、誤検知や業務影響をどの程度抑えられるか評価する。
- AWS利用中の組織では、既存のID管理、ログ管理、監査体制と整合するかを見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Amazon Web Services | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Codenotary launches AI security platform that learns from AI agent behavior](https://www.helpnetsecurity.com/2026/07/08/codenotary-launches-ai-security-platform-that-learns-from-ai-agent-behavior/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-21403"></a>

### 1. CISA Urges Immediate Patching of Exploited ColdFusion, Langflow, Joomla Flaws

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 38.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 47.0 |

#### 概要

CISAは、Adobe ColdFusion、Langflow、Joomlaに関連する4件の脆弱性をKnown Exploited Vulnerabilities（KEV）カタログに追加し、実際の悪用が確認されているとして対応を促しています。
公開情報では、少なくとも一部の脆弱性は深刻度が高く、影響範囲によっては任意コード実行につながるおそれがあるとされています。
KEV入りは、単なる理論上の脆弱性ではなく、優先度を上げて対処すべき対象であることを示します。
政府機関だけでなく、当該製品を利用する組織全般にとって、早期の修正適用と影響確認が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 利用中のAdobe ColdFusion、Langflow、Joomlaおよび関連拡張のバージョンを確認し、該当する修正の適用状況を点検する。
- 外部公開している管理画面や関連サービスがないか洗い出し、露出がある場合は優先的に保護を強化する。
- 修正適用までの間は、監視ログで不審なアクセスや異常なリクエストの兆候を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-48282 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Adobe | 言及あり | 0.80 | — |
| 製品 | Adobe ColdFusion | 言及あり | 0.80 | — |
| 製品 | Langflow | 言及あり | 0.80 | — |
| 製品 | Joomla | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Urges Immediate Patching of Exploited ColdFusion, Langflow, Joomla Flaws](https://www.securityweek.com/cisa-urges-immediate-patching-of-exploited-coldfusion-langflow-joomla-flaws/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds 4 Actively Exploited Adobe, Joomla, and Langflow Flaws to KEV](https://thehackernews.com/2026/07/cisa-adds-4-actively-exploited-adobe.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
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
| [HackersがRoundcubeの脆弱性を悪用し学術研究者を監視](https://www.bleepingcomputer.com/news/security/hackers-exploit-roundcube-flaw-to-spy-on-academic-researchers/) | 28.0 | 20.0 | 42.0 |
| [台湾、中国のスパイ活動キャンペーンへの関与疑惑で2人の実業家を起訴](https://therecord.media/taiwan-charges-businessmen-china-cyber-espionage-campaign) | 28.0 | 20.0 | 42.0 |
| [Entraのパスキー登録を狙うビッシング、Microsoft 365ユーザーが標的に](https://www.bleepingcomputer.com/news/security/entra-passkey-enrollment-vishing-targets-microsoft-365-users/) | 28.0 | 20.0 | 42.0 |
| [Vidar Infostealerがマルバタイジングキャンペーンで中小企業を標的に攻撃](https://www.darkreading.com/cyberattacks-data-breaches/vidar-infostealer-smb-malvertising-campaign) | 28.0 | 20.0 | 42.0 |
| [中国関連のAPTが新たな「Leash」バックドアで攻撃手法を拡大](https://www.securityweek.com/china-linked-apt-expands-arsenal-with-new-leash-backdoors/) | 28.0 | 20.0 | 42.0 |
| [Accentureで大規模データ侵害、顧客にリスクの可能性](https://www.cybersecuritydive.com/news/accenture-data-breach-access-keys-source-code/824694/) | 28.0 | 20.0 | 42.0 |
| [中国関連APT、新たなマルウェアでプロキシネットワークを拡大](https://www.infosecurity-magazine.com/news/uat-7810-china-apt-orb-proxy/) | 28.0 | 20.0 | 42.0 |
| [新たなGhostフィッシングの波が従来のメールセキュリティを破る](https://thehackernews.com/2026/07/new-ghost-phishing-wave-is-breaking.html) | 28.0 | 20.0 | 42.0 |
| [SCMBANKERマルウェアがClickFixの誘導でメキシコの銀行利用者を標的にする](https://thehackernews.com/2026/07/scmbanker-malware-uses-clickfix-lures.html) | 28.0 | 20.0 | 42.0 |
| [Accenture、35GBのデータ窃取主張を受けセキュリティインシデントを認める](https://www.helpnetsecurity.com/2026/07/08/accenture-data-breach-2026/) | 28.0 | 20.0 | 42.0 |
| [VidarインフォスティーラーとMonero暗号通貨マイナーを配布する新たな悪意あるキャンペーン](https://www.infosecurity-magazine.com/news/new-campaign-vidar-stealer-monero/) | 28.0 | 20.0 | 42.0 |
| [China-Linked UAT-7810、LONGLEASHマルウェアでORBネットワークを拡大](https://thehackernews.com/2026/07/china-linked-uat-7810-expands-orb.html) | 28.0 | 20.0 | 42.0 |
| [CISA、Langflowの認証バイパス脆弱性の修正を優先するよう連邦機関に指示](https://www.bleepingcomputer.com/news/security/cisa-orders-feds-to-prioritize-patching-langflow-auth-bypass-flaw/) | 27.0 | 20.0 | 43.0 |
| [MicrosoftをAI時代の速度で守る：SFIがクラウドを先回りして強化する方法](https://www.microsoft.com/en-us/security/blog/2026/07/08/protecting-microsoft-at-ai-speed-how-sfi-proactively-hardens-our-cloud/) | 27.0 | 20.0 | 42.0 |
| [フランスの非営利団体、AIサイバー脅威に関する世界的な情報収集・調査拠点を設立](https://cyberscoop.com/paris-peace-forum-intaic-ai-cyber-threats/) | 25.0 | 20.0 | 42.0 |
| [AIコーディングエージェントが攻撃者検知用のエンドポイントセキュリティルールを発動していることが判明](https://thehackernews.com/2026/07/ai-coding-agents-found-triggering.html) | 25.0 | 20.0 | 42.0 |
| [Cisco、2026年7月15日公開予定のセキュリティアドバイザリに関する事前通知](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-notice-ILh3ZrP5) | 25.0 | 20.0 | 42.0 |
| [NCSCがAI搭載の「Cyber Shield」で英国をハッカーから守る計画、その仕組みとは](https://www.itpro.com/security/the-ncsc-wants-to-build-an-ai-powered-cyber-shield-to-protect-the-uk-from-hackers-heres-how-itll-work) | 25.0 | 20.0 | 42.0 |
| [AIがサービスデスク攻撃を強化する3つの手口とその防ぎ方](https://www.bleepingcomputer.com/news/security/3-ways-ai-powers-service-desk-attacks-and-how-to-prevent-them/) | 25.0 | 20.0 | 42.0 |
| [トップAIコーディングエージェントの不具合が示す、Unix時代のセキュリティ問題は今もなお消えていない](https://www.theregister.com/security/2026/07/08/bug-in-top-ai-coding-agents-shows-that-unix-era-security-headaches-never-really-die/5268025) | 25.0 | 20.0 | 42.0 |
| [GhostApproval: AIコーディング支援ツールにおける信頼境界のギャップ](https://www.wiz.io/blog/ghostapproval-a-trust-boundary-gap-in-ai-coding-assistants) | 25.0 | 20.0 | 42.0 |
| [中国、開発者にClaude Codeの使用中止を要請し「バックドアコード」懸念が浮上](https://www.theregister.com/security/2026/07/08/china-ditch-older-claude-versions-with-backdoor-code/5268371) | 25.0 | 20.0 | 42.0 |
| [Blackpoint AI SOC AgentがIDベースの攻撃を自律的に封じ込める](https://www.helpnetsecurity.com/2026/07/08/blackpoint-cyber-ai-soc-agent/) | 25.0 | 20.0 | 42.0 |
| [First Recon AI Security Runtimeで企業のAIを監査対応の証跡付きで統制する方法](https://www.helpnetsecurity.com/2026/07/08/first-recon-ai-security-runtime-helps-enterprises-govern-ai-with-audit-ready-evidence/) | 25.0 | 20.0 | 42.0 |
| [EU、外国製AIシステムへの依存を減らすサイバー計画を発表](https://therecord.media/eu-unveils-cyber-plan-to-reduce-reliance-on-foreign-ai) | 25.0 | 20.0 | 42.0 |
| [セキュリティチームはより先手を打てる態勢にあるが、何がそれを阻んでいるのか](https://www.rapid7.com/blog/post/dr-teams-ready-for-preemptive-security-mdr-survey) | 25.0 | 20.0 | 42.0 |
| [Attestiv DeepScanがAIとフォレンジック分析を組み合わせてファイル検証を実現](https://www.helpnetsecurity.com/2026/07/08/attestiv-deepscan/) | 25.0 | 20.0 | 42.0 |
| [Google Dialogflow CXの不具合により攻撃者がAI会話を乗っ取れる脆弱性](https://www.securityweek.com/google-dialogflow-cx-bug-allowed-attackers-to-hijack-ai-conversations/) | 25.0 | 20.0 | 42.0 |
| [GitHub Copilotはチャットで有害な要求を拒否するが、コードではそれを生成する](https://thehackernews.com/2026/07/github-copilot-refuses-harmful-requests.html) | 25.0 | 20.0 | 42.0 |
| [GitHub Agentic Workflowsをプロンプトインジェクションにさらす重大な脆弱性](https://www.securityweek.com/critical-vulnerability-exposes-github-agentic-workflows-to-prompt-injection/) | 25.0 | 20.0 | 42.0 |
| [AIフロンティアの防御：パートナー向けブループリント](https://www.akamai.com/blog/partners/2026/jul/securing-ai-frontier-blueprint-partners) | 25.0 | 20.0 | 42.0 |
| [Crusoe、AIモデル開発向けにサーバーレスのファインチューニングを提供](https://www.helpnetsecurity.com/2026/07/08/crusoe-serverless-fine-tuning/) | 25.0 | 20.0 | 42.0 |
| [Automox MCP ServerにビジュアルレビューとAI駆動のパッチポリシー作成機能を追加](https://www.helpnetsecurity.com/2026/07/08/automox-mcp-server-2-2/) | 25.0 | 20.0 | 42.0 |
| [Found fast, fixed slow: AI仲介基盤が埋めるべき迅速発見と修正遅延のギャップ](https://cyberscoop.com/ai-executive-order-cybersecurity-clearinghouse-vulnerability-patching-gap/) | 25.0 | 20.0 | 42.0 |
| [NCSCが防衛向けの全国規模AI搭載「Cyber Shield」を発表](https://www.infosecurity-magazine.com/news/ncsc-national-cyber-sheild-ai/) | 25.0 | 20.0 | 42.0 |
| [AIエージェント向けの国家ID制度：エストニアは先例となるか](https://www.darkreading.com/cybersecurity-operations/state-ids-ai-agents-estonia) | 25.0 | 20.0 | 42.0 |
| [CVE-2026-0283: PAN-OSのLarge Scale VPN（LSVPN）における認証回避の脆弱性（重要度：中）](https://security.paloaltonetworks.com/CVE-2026-0283) | 24.0 | 46.0 | 50.0 |
| [CVE-2026-0286: PAN-OSのCLIにおける認証済みコマンドインジェクション脆弱性（重要度: 中）](https://security.paloaltonetworks.com/CVE-2026-0286) | 24.0 | 46.0 | 50.0 |
| [Ubiquiti、UniFi OSの新たな重大脆弱性を警告](https://www.bleepingcomputer.com/news/security/ubiquiti-warns-of-new-max-severity-unifi-os-vulnerability/) | 24.0 | 38.0 | 42.0 |
| [CVE-2026-0276 Cortex XDR Broker VMの権限昇格脆弱性（低）](https://security.paloaltonetworks.com/CVE-2026-0276) | 22.0 | 40.0 | 50.0 |
| [Ubiquiti、Connect・Talk・Access・Protect・OSのUniFi脆弱性を修正](https://thehackernews.com/2026/07/ubiquiti-patches-critical-unifi-flaws.html) | 22.0 | 40.0 | 50.0 |
| [PAN-OS管理Webインターフェースにおける情報漏えいの脆弱性（CVE-2026-0281）](https://security.paloaltonetworks.com/CVE-2026-0281) | 22.0 | 36.0 | 50.0 |
| [メルマガ送信サービスで情報流出、影響範囲など調査 - ディライトフル](https://www.security-next.com/186194) | 22.0 | 20.0 | 42.0 |
| [個人情報の保存先を誤り、意図せず学生に共有 - 近畿大](https://www.security-next.com/186754) | 22.0 | 20.0 | 42.0 |
| [配付名簿に不同意者の個人情報、法令を誤解釈 - 阿南市](https://www.security-next.com/186572) | 22.0 | 20.0 | 42.0 |
| [CVE-2026-0279 PAN-OSの複数のクロスサイトスクリプティング（XSS）脆弱性（重要度：低）](https://security.paloaltonetworks.com/CVE-2026-0279) | 21.0 | 34.0 | 50.0 |
| [CVE-2026-0277 Prisma Access AgentのiOSにおける証明書検証不備](https://security.paloaltonetworks.com/CVE-2026-0277) | 20.0 | 28.0 | 50.0 |
| [PAN-OSの管理Webインターフェースにおけるサーバーサイドリクエストフォージェリの脆弱性（CVE-2026-0285）](https://security.paloaltonetworks.com/CVE-2026-0285) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0278 Prisma Access AgentのWindows版における複数のDLPポリシーバイパス脆弱性](https://security.paloaltonetworks.com/CVE-2026-0278) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0284 PAN-OSのLarge Scale VPN（LSVPN）におけるXMLインジェクション脆弱性（重要度：中）](https://security.paloaltonetworks.com/CVE-2026-0284) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0287 PAN-OSのネットワークトラフィック処理におけるサービス妨害の脆弱性](https://security.paloaltonetworks.com/CVE-2026-0287) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0280 PAN-OSのIPv6ファイアウォールポリシー回避（重要度：LOW）](https://security.paloaltonetworks.com/CVE-2026-0280) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0282 PAN-OSの管理Webインターフェースにおけるファイル削除脆弱性（重要度: LOW）](https://security.paloaltonetworks.com/CVE-2026-0282) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0288: PAN-OSのUser-ID Terminal Server Agentにおけるバッファオーバーフロー脆弱性](https://security.paloaltonetworks.com/CVE-2026-0288) | 20.0 | 28.0 | 50.0 |
| [Accenture、ハッカーによるソースコード窃取主張後にデータ侵害を確認](https://www.securityweek.com/accenture-confirms-data-breach-after-hacker-claims-source-code-theft/) | 20.0 | 20.0 | 42.0 |
| [PAN-SA-2026-0010 ChromiumおよびPrisma Browser：2026年7月の月次脆弱性情報更新（重要度：高）](https://security.paloaltonetworks.com/PAN-SA-2026-0010) | 20.0 | 20.0 | 42.0 |
| [米国企業がサイバーリスクをより広範な戦略に組み込む動き](https://www.cybersecuritydive.com/news/us-enterprises-cyber-risk-strategic-focus/824707/) | 20.0 | 20.0 | 42.0 |
| [RedWing AndroidスパイウェアがTelegram上でサービスとして販売される](https://www.infosecurity-magazine.com/news/redwing-android-spyware-maas/) | 20.0 | 20.0 | 42.0 |
| [英国の元プライバシー担当責任者、通報した女性に対する法的措置を準備と大臣が発表](https://therecord.media/former-uk-privacy-chief-preparing-legal-action-against-woman-who-reported-him) | 20.0 | 20.0 | 42.0 |
| [Censys Internet MapがリアルタイムDNSデータをインターネットインフラに結び付ける](https://www.helpnetsecurity.com/2026/07/08/censys-internet-map-links-real-time-dns-data-to-internet-infrastructure/) | 20.0 | 20.0 | 42.0 |
| [FBIの通報を受け、スペインで親ロシア系ハクティビスト集団の支持者を逮捕](https://therecord.media/spain-arrest-alleged-supporter-noname-carr-zpentest) | 20.0 | 20.0 | 42.0 |
| [FalconStor Cloud Clean Roomで専用インフラなしの検証済み復旧を実現](https://www.helpnetsecurity.com/2026/07/08/falconstor-cloud-clean-room-enables-validated-recovery-without-dedicated-infrastructure/) | 20.0 | 20.0 | 42.0 |
| [次のあなたの車はあなたの顔を監視しているかもしれない](https://www.malwarebytes.com/blog/news/2026/07/your-next-car-could-be-watching-your-face) | 20.0 | 20.0 | 42.0 |
| [2026年、認証確認ステップが新たなATOの戦場に](https://thehackernews.com/2026/07/the-verification-step-is-new-ato.html) | 20.0 | 20.0 | 42.0 |
| [KDDIでデータ漏えい、1200万人超に影響](https://www.bleepingcomputer.com/news/security/japanese-telecom-giant-kddi-says-data-breach-affects-12-million-people/) | 20.0 | 20.0 | 42.0 |
| [NIST CSF 2.0実践ガイド：米国企業のリスク管理のための最新セキュリティプログラム構築](https://any.run/cybersecurity-blog/nist-csf-guide-for-cisos/) | 20.0 | 20.0 | 42.0 |
| [ScienceLogic、Skylar Oneに地理的なサービス可視化を追加](https://www.helpnetsecurity.com/2026/07/08/sciencelogic-adds-geographic-service-visibility-to-skylar-one/) | 20.0 | 20.0 | 42.0 |

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
