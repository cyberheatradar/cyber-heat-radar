# 📡 サイレーダー 2026-05-19 05:00 JST

このレポートは、2026-05-18 17:00 JST〜2026-05-19 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 91
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [Attackers are exploiting critical NGINX vulnerability (CVE-2026-42945)](#topic-4593) | 38.0 | 67.0 | 61.0 | 音声 | 温度感上位枠 |
| 2 | [Security Researchers Find 47 Zero-Days at Pwn2Own Berlin](#topic-6756) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Inside TeamPCP’s Supply Chain Offensive](#topic-6703) | 33.0 | 45.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [5 Steps to Managing Shadow AI Tools Without Slowing Down Employees](#topic-6702) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [The Boring Stuff is Dangerous Now](#topic-5582) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-4593"></a>

### 1. Attackers are exploiting critical NGINX vulnerability (CVE-2026-42945)

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>RCE</nobr> / <nobr>KEV</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 38.0 |
| <nobr>実務影響</nobr> | 67.0 |
| <nobr>確度</nobr> | 61.0 |

#### 概要

NGINXのngx_http_rewrite_moduleに存在する重大な脆弱性CVE-2026-42945について、外部研究者から公開された後、実際に悪用されている可能性が複数報告されています。
影響を受ける範囲はNGINX PlusとNGINX Openの広いバージョン帯に及ぶとされ、条件次第でサービス停止やリモートコード実行につながるおそれがあるとされています。
広く使われるWebサーバー製品の脆弱性であり、公開後まもなく悪用観測が出ている点が重要です。公開情報だけでも影響確認や対応の優先度判断を急ぐ必要があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 技術詳細・再現情報あり。
- 技術者コミュニティ反応: 弱。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 技術詳細により影響確認が進みやすい。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 技術詳細・悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 技術詳細、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 自組織のNGINX稼働有無と該当バージョンを確認し、影響範囲を特定する。
- ベンダーの修正版・回避策の案内を確認し、適用可能なものから速やかに反映する。
- NGINXの異常終了、予期しない再起動、アクセスログ上の不審なHTTPリクエスト増加を監視する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-42945 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-42945](https://nvd.nist.gov/vuln/detail/CVE-2026-42945) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Attackers are exploiting critical NGINX vulnerability (CVE-2026-42945)](https://helpnetsecurity.com/2026/05/18/ngnix-vulnerability-exploited-cve-2026-42945) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [NGINX CVE-2026-42945 Exploited in the Wild, Causing Worker Crashes and Possible ](https://thehackernews.com/2026/05/nginx-cve-2026-42945-exploited-in-wild.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [NGINXでリモートコード実行の脆弱性が発見される、影響を受けるバージョンはこれ](https://gigazine.net/news/20260515-nginx-remote-code-execution) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [18-Year-Old NGINX Rewrite Module Flaw Enables Unauthenticated RCE](https://thehackernews.com/2026/05/18-year-old-nginx-rewrite-module-flaw.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-42945 NGINX ngx_http_rewrite_module vulnerability](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-42945) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 技術詳細・悪用観測あり。
- 継続観測: 継続。

---

<a id="topic-6756"></a>

### 2. Security Researchers Find 47 Zero-Days at Pwn2Own Berlin

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Pwn2Own Berlinで、研究者らが47件のゼロデイ脆弱性を発見したと報じられています。
公開情報によると、この場では新たな脆弱性の実証が多数行われ、研究コミュニティには総額130万ドルが授与されたとされています。
ゼロデイ脆弱性は、未修正のまま悪用されると被害につながる可能性があるため注目されています。
今回のように多数の新規脆弱性が見つかると、今後の修正対応や影響範囲の確認が重要になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 自組織で利用中の製品や機器に、関連する脆弱性情報や修正パッチが出ていないか確認する。
- 資産管理と脆弱性管理の対象を見直し、影響を受ける可能性のある製品の優先度を上げる。
- ベンダー告知やセキュリティアドバイザリを継続監視し、修正公開後は速やかに適用計画を立てる。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Security Researchers Find 47 Zero-Days at Pwn2Own Berlin](https://infosecurity-magazine.com/news/security-researchers-47-zerodays) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 初出。

---

<a id="topic-6703"></a>

### 3. Inside TeamPCP’s Supply Chain Offensive

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>サプライチェーン</nobr> / <nobr>脅威アクター</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>AI</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 45.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

TeamPCPに関連するとされるソフトウェア供給網キャンペーンが、GitHub Actions、PyPI、Docker Hub、VS Code/OpenVSX、npm などの開発基盤を悪用した可能性があると報告されています。
公開情報によれば、悪意あるパッケージやワークフロー、リリース経路の侵害を通じて、開発者の認証情報収集や下流への影響拡大が懸念されています。
開発・配布の信頼経路が狙われると、単一組織にとどまらず利用者や依存先へ被害が波及しうるため注目されています。
CI/CD やパッケージ管理の安全性を改めて点検する必要性を示す事例です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 依存パッケージ、Actions/CI設定、公開リリース経路の整合性を確認し、想定外の変更がないか監視する。
- 開発者アカウントの認証強化と秘密情報の再点検を行い、不要なトークンや古い資格情報を整理する。
- 利用中のレジストリや拡張機能について、配布元・署名・更新履歴を確認し、異常があれば一時停止や隔離を検討する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Inside TeamPCP’s Supply Chain Offensive](https://blog.polyswarm.io/inside-teampcps-supply-chain-offensive) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-6702"></a>

### 4. 5 Steps to Managing Shadow AI Tools Without Slowing Down Employees

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

従業員が業務中に、セキュリティ部門の確認を経ないままAIツールを利用する「シャドーAI」が広がっているとされています。
今回の話題では、業務の効率を落とさずにAI利用を管理するための、実務的なガバナンスの考え方が整理されています。
生成AIの利用が現場主導で進む一方、入力データの取り扱いや利用ルールが不明確だと、情報漏えいやコンプライアンス上の問題につながる可能性があります。
禁止一辺倒ではなく、使わせながら統制する運用が求められている点が注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 社内で実際に使われているAIツールの把握と、許可・非許可の基準整理を進める。
- 機密情報や個人情報の入力ルール、例外申請、ログ確認などを含む運用を整備する。
- 利便性を損ねないよう、承認済みの代替ツールや案内を用意して現場の迂回利用を減らす。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [5 Steps to Managing Shadow AI Tools Without Slowing Down Employees](https://bleepingcomputer.com/news/security/5-steps-to-managing-shadow-ai-tools-without-slowing-down-employees) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-5582"></a>

### 5. The Boring Stuff is Dangerous Now

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>AIエージェント</nobr> / <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

AIエージェントが見落とされがちな脆弱性を見つけて悪用する可能性がある一方で、開発現場ではAI生成コードが大量に使われており、品質や安全性のばらつきが懸念されています。
こうした状況は、従来は「地味」と見なされてきた実装上の不備が、攻撃対象としてより重要になることを示しています。
AIの活用拡大により、脆弱性の発見・悪用と、脆弱なコードの混入が同時に起こりやすくなっています。防御側は、従来の優先順位だけでなく、コード品質管理や検証の見直しを迫られます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI生成コードを含む開発フローで、レビューとテストの強化を前提にする。
- 見落とされやすい小さな不備も、攻撃面の拡大要因として継続的に点検する。
- AIエージェントの利用や自動化導入時は、出力の妥当性確認と権限管理を厳格にする。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [The Boring Stuff Is Dangerous Now](https://darkreading.com/cyber-risk/ai-code-and-agents-forces-defenders-adapt) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

今回はGitHubのみ掲載の注目トピックはありません。

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [開発者ワークステーションもソフトウェアサプライチェーンの一部になった](https://thehackernews.com/2026/05/developer-workstations-are-now-part-of.html) | 28.0 | 45.0 | 42.0 |
| [悪意のある4つのnpmパッケージが情報窃取マルウェアとPhantom BotのDDoSマルウェアを配布](https://thehackernews.com/2026/05/four-malicious-npm-packages-deliver.html) | 28.0 | 40.0 | 42.0 |
| [2026年第1四半期のIT脅威の進化：モバイル以外の統計](https://securelist.com/malware-report-q1-2026-pc-iot-statistics/119828) | 28.0 | 28.0 | 50.0 |
| [INTERPOLが中東・北アフリカ13か国でサイバー犯罪一斉摘発を主導](https://cyberscoop.com/interpol-operation-ramz-middle-east-north-africa) | 28.0 | 20.0 | 42.0 |
| [漏えいした Shai-Hulud マルウェアが新たな npm 情報窃取キャンペーンを助長](https://bleepingcomputer.com/news/security/leaked-shai-hulud-malware-fuels-new-npm-infostealer-campaign) | 28.0 | 20.0 | 42.0 |
| [オランダ警察が顔写真を掲示し、74人の詐欺容疑者を摘発](https://helpnetsecurity.com/2026/05/18/dutch-police-game-over-fraudsters-campaign) | 28.0 | 20.0 | 42.0 |
| [イランのサイバー攻勢、燃料タンク侵害で拡大](https://darkreading.com/cyberattacks-data-breaches/fuel-tank-breaches-expand-scope-irans-cyber-offensive) | 28.0 | 20.0 | 42.0 |
| [脅威アクターによる防御回避：攻撃者がAVとEDRを無効化する手口](https://huntress.com/blog/how-attackers-disable-av-edr) | 28.0 | 20.0 | 42.0 |
| [Shai-Huludワームの初期クローンが出現](https://securityweek.com/first-shai-hulud-worm-clones-emerge) | 28.0 | 20.0 | 42.0 |
| [攻撃者がGrafana LabsのGitHubにアクセスし、コードをダウンロード](https://helpnetsecurity.com/2026/05/18/attackers-accessed-downloaded-code-from-grafana-labs-github) | 28.0 | 20.0 | 42.0 |
| [INTERPOLによるフィッシングおよび詐欺ネットワーク摘発で201人を逮捕](https://helpnetsecurity.com/2026/05/18/interpol-mena-cybercrime-operation-ramz-201-arrests) | 28.0 | 20.0 | 42.0 |
| [Weekly Recap: Exchangeのゼロデイ、npmワーム、偽AIリポジトリ、Ciscoの脆弱性悪用など](https://thehackernews.com/2026/05/weekly-recap-exchange-0-day-npm-worm.html) | 27.0 | 45.0 | 43.0 |
| [AI時代に成長企業を守るための効果的な対策](https://microsoft.com/en-us/security/blog/2026/05/18/how-to-better-protect-your-growing-business-in-an-ai-powered-world) | 27.0 | 20.0 | 42.0 |
| [TaskhostのWindowsタスクにおけるローカル権限昇格の脆弱性（CVE-2025-60710）](https://github.com/Wh04m1001/CVE-2025-60710) | 25.0 | 82.0 | 81.0 |
| [AIがソフトウェア保守担当者を大量の不要なセキュリティ報告で圧倒している](https://helpnetsecurity.com/2026/05/18/problems-with-ai-assisted-vulnerability-research) | 25.0 | 20.0 | 42.0 |
| [AI企業が金融口座への接続を進める中で懸念されるプライバシーリスク](https://therecord.media/experts-warn-of-privacy-cyer-risks-ai-finance) | 25.0 | 20.0 | 42.0 |
| [SmartBear、ReadyAPIをAI搭載のAPIテスト機能で拡張](https://helpnetsecurity.com/2026/05/18/smartbear-readyapi) | 25.0 | 20.0 | 42.0 |
| [政府のコンテストが切り開いたAIベースのバグハンティング革命](https://cybersecuritydive.com/news/ai-vulnerability-discovery-darpa-challenge-critical-infrastructure/819494) | 25.0 | 20.0 | 42.0 |
| [NCSCがAgentic AI利用のセキュリティ確保に関するガイダンスを公開](https://infosecurity-magazine.com/news/ncsc-publishes-guidance-securing) | 25.0 | 20.0 | 42.0 |
| [AI、自動化、エコシステムが切り拓くパートナーシップの未来](https://security.com/expert-perspectives/resilient-channel-series-part-6) | 25.0 | 20.0 | 42.0 |
| [Bank of England、FCA、財務省がフロンティアAIへの警鐘を鳴らす](https://infosecurity-magazine.com/news/bank-england-fca-treasury-alarm) | 25.0 | 20.0 | 42.0 |
| [Ivanti、Fortinet、SAP、VMware、n8nのパッチ適用が必要なRCE、SQLインジェクション、権限昇格の脆弱性](https://thehackernews.com/2026/05/ivanti-fortinet-sap-vmware-n8n-patch.html) | 24.0 | 46.0 | 50.0 |
| [海外子会社にサイバー攻撃、個人情報流出の可能性 - 象印](https://security-next.com/184511) | 22.0 | 20.0 | 42.0 |
| [「Apache Flink」にコードインジェクションの脆弱性 - 重要度「クリティカル」](https://security-next.com/184554) | 22.0 | 20.0 | 42.0 |

---

## 📊 スコアの見方

| <nobr>指標</nobr> | 意味 |
|---|---|
| <nobr>温度状態</nobr> | 話題のライフサイクルを示す補助ラベルです。例: 低温、継続監視、温度上昇中、高温、冷却中。 |
| <nobr>温度感</nobr> | 話題として今どれだけ注目・拡散・更新されているかを示します。 |
| <nobr>実務影響</nobr> | 対象組織・担当者にとって、対応優先度や被害可能性がどれだけ大きいかを示します。 |
| <nobr>確度</nobr> | 公的機関、ベンダー公式、複数ソース、CVE/KEV、一次資料などにより、情報をどれだけ確認できているかを示します。事件報道系は、複数報道があっても司法文書・当局発表などの一次資料が弱い場合、脆弱性KEV系より低く出ることがあります。 |

スコアは、公開情報から抽出した特徴量と事前定義した重み付けに基づく参考指標です。詳しい算出方針は [スコアリング方針](../docs/scoring.md) を参照してください。

## 🔒 公開しない内部情報について

サイレーダーでは、温度感の補助シグナルとして、公的機関・ベンダー公式・信頼できる報道機関・技術者コミュニティ・国内外の公開反応などを利用します。

これらのシグナルは、一次情報、報道波及、技術者反応、開発者反応、PoC・悪用観測などに分けて評価します。

ただし、ランキング操作、スパム的誘導、監視回避を防ぐため、個別の監視対象、取得手段、検索条件、評価対象サービス名、内部的な重み付けやしきい値は公開しません。

また、公開反応の多さだけで掲載順位を決めることはありません。重要度の判定では、ベンダー公式情報、公的機関、一次資料、信頼できる技術分析、実務影響を優先します。

## ⚠️ 注意事項

このレポートは、収集・観測できた公開情報をもとにした参考情報です。完全性、正確性、即時性を保証するものではありません。

重要な判断を行う場合は、必ずベンダー公式情報、公的機関、一次情報を確認してください。

サイレーダーは、広告・スポンサー・企業関係に基づいて掲載順位や温度感スコアを変更しません。
