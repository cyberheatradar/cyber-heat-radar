# 📡 サイレーダー 2026-08-27 05:00 JST

このレポートは、2026-08-26 17:00 JST〜2026-08-27 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 85
- [音声で扱う想定のトピック](#audio-topics): 4
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 56

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-60004: CISA KEV catalog addition](#topic-29270) | 55.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 2 | [CISA Adds Six Known Exploited Vulnerabilities to Catalog](#topic-29509) | 49.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [AI Speeds Up Malware Development, Not Its Success Rate: Analysis](#topic-29478) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [CISA Vulnerability Review](#topic-29508) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-29270"></a>

### 1. CVE-2026-60004: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>国⁠家⁠支⁠援</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 55.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

CISAは、Giteaに関するCVE-2026-60004をKnown Exploited Vulnerabilities（KEV）Catalogに追加しました。
公表情報では、実際の悪用が確認されたことを受けた対応とされています。関連報道では、Giteaのコード注入またはRCEに関わる脆弱性として扱われています。
KEV Catalog入りは、単なる脆弱性情報ではなく、実際に悪用が観測されていることを示すため、優先対応が必要な案件として扱われます。
Giteaを業務利用している組織では、公開状況や更新状況の確認が急がれます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Giteaの利用有無を棚卸しし、対象インスタンスが最新の修正版に更新されているか確認する。
- インターネット公開されているGitea環境を優先的に点検し、不要な公開を避ける。
- 侵害の兆候がないか、認証・操作ログや不審なリポジトリ操作を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-60004 | 関連CVE | 1.00 | 候補あり（URL 9件以上） |
| 製品 | Gitea | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-60004](https://nvd.nist.gov/vuln/detail/CVE-2026-60004) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Critical Gitea vulnerability now exploited in the wild (CVE-2026-60004)](https://www.helpnetsecurity.com/2026/08/26/gitea-cve-2026-60004-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Gitea RCE Actively Exploited as Reported Attack Drops Miner-Like Payloa](https://thehackernews.com/2026/08/critical-gitea-rce-actively-exploited.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Warns of Exploited Gitea Vulnerability](https://www.securityweek.com/cisa-warns-of-exploited-gitea-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/08/25/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers now exploit critical Gitea flaw in code injection attacks](https://www.bleepingcomputer.com/news/security/hackers-now-exploit-critical-gitea-flaw-in-code-injection-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-29509"></a>

### 2. CISA Adds Six Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 49.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、実際の悪用が確認されたとして、Known Exploited Vulnerabilities（KEV）カタログに6件の脆弱性を追加しました。
対象にはRed Hat、Microsoft SQL Server、Linux kernel、Citrix NetScaler関連などが含まれています。
KEVへの追加は、組織が優先的に対応すべき脆弱性であることを示す強いシグナルです。公開資産に影響するものやRCE系を含むため、放置すると侵害リスクが高まります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- KEVカタログへの掲載有無を確認し、該当製品の修正適用を優先する。
- インターネットに公開している資産を先に点検し、影響範囲を洗い出す。
- 修正前に侵害の兆候がないか、ログや設定変更の履歴を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |
| 製品 | Linux kernel | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Six Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/08/26/cisa-adds-six-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-29478"></a>

### 3. AI Speeds Up Malware Development, Not Its Success Rate: Analysis

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Palo Alto NetworksのUnit 42は、AIに関連するマルウェア405件を分析し、そのうち実際に稼働環境の端末まで到達したものは12件にとどまったとしています。
今回の分析は、AIの活用が悪意あるコード作成の効率化にはつながっても、攻撃の成功率を自動的に高めるわけではない可能性を示しています。
AIを使った脅威が増える中で、実務側は「生成の容易さ」と「実害の大きさ」を分けて捉える必要があります。
過度な警戒や誤解を避けつつ、検知・封じ込め・初動対応の強化対象を見極める材料になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI支援型のマルウェアでも、実際の到達・感染には従来型の防御策が引き続き重要です。
- 「生成数の増加」と「被害の増加」は同義ではないため、脅威評価では実運用での到達率や観測実績を確認してください。
- AI利用の有無より、最終的な振る舞い・配布経路・検知回避の兆候に着目した監視が有効です。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [AI Speeds Up Malware Development, Not Its Success Rate: Analysis](https://www.securityweek.com/ai-speeds-up-malware-development-not-its-success-rate-analysis/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-29508"></a>

### 4. CISA Vulnerability Review

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>A⁠I</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

CISAは、公開された脆弱性データをもとに「CISA Vulnerability Review」を公表し、侵害の多くが高度な手口ではなく、既知のソフトウェア脆弱性や基本的なセキュリティ不備に起因していると指摘しています。
レビューでは、AIによる脆弱性発見が広がる前の現状把握として、Secure by Designの重要性や、脆弱性をリスクベースで優先付けする考え方が示されています。
個別の脆弱性対応だけでなく、露出状況や既知悪用の有無などを踏まえた優先順位付けが重要だと再確認できるためです。
AIを含む自動化された脆弱性発見が広がる可能性を見据え、予防的な改善の必要性が強調されています。

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

- 外部公開されている資産と既知悪用済み脆弱性を優先的に点検する。
- 個別修正に加え、同種の脆弱性を生みにくい設計・開発運用の改善を進める。
- 脆弱性対応は、露出状況・KEV掲載・自動化悪用の可能性・技術的影響を踏まえて順位付けする。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Vulnerability Review](https://www.cisa.gov/resources-tools/resources/cisa-vulnerability-review) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

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
| [FBI、米国組織からデータを盗むために使われた中国関連QTFYインフラを妨害](https://thehackernews.com/2026/08/fbi-disrupts-china-linked-qtfy.html) | 28.0 | 20.0 | 48.0 |
| [フィッシング攻撃の圧力下にある米国金融業界：SOCデータが示すもの](https://any.run/cybersecurity-blog/phishing-us-finance/) | 28.0 | 20.0 | 48.0 |
| [Androidマルウェアが車載ヘッドユニットのアップデート機能を乗っ取る](https://www.darkreading.com/cyberattacks-data-breaches/android-malware-hijacks-update-system-car-head-units) | 28.0 | 20.0 | 42.0 |
| [Nimbus ManticoreがTWOSTROKE風バックドアとSSHトンネラーでツール群を拡大](https://thehackernews.com/2026/08/nimbus-manticore-expands-toolset-with.html) | 28.0 | 20.0 | 42.0 |
| [中国系ハッカーが長期の脅威キャンペーンで司法省、連邦準備制度、NASAに侵入したと米国が主張](https://www.itpro.com/security/cyber-attacks/us-claims-chinese-hackers-breached-justice-department-federal-reserve-nasa-in-lengthy-threat-campaign) | 28.0 | 20.0 | 42.0 |
| [Tortoiseshellが新たなバックドアとSSHトンネルでマルウェアツール群を拡張](https://www.infosecurity-magazine.com/news/tortoiseshell-new-backdoor-ssh/) | 28.0 | 20.0 | 42.0 |
| [NovaCookiesキャンペーンが正規のDocusign通知を悪用しMicrosoft 365セッションを窃取](https://thehackernews.com/2026/08/novacookies-campaigns-abuse-genuine.html) | 28.0 | 20.0 | 42.0 |
| [Ubiquitiが最大深刻度のセキュリティ脆弱性3件を修正](https://www.bleepingcomputer.com/news/security/ubiquiti-patches-three-max-severity-security-vulnerabilities/) | 28.0 | 20.0 | 42.0 |
| [ノルウェー政府サービスへのDDoS攻撃](https://www.infosecurity-magazine.com/news/ddos-attack-hits-norwegian/) | 28.0 | 20.0 | 42.0 |
| [AIエージェント時代のコーディングテクニック「コーディングルールをAGENTS.mdにまとめる」「品質が低下したらAGENTS.mdの読み直しを指示」](https://gigazine.net/news/20260826-agent-improve-llm-code-quality/) | 27.0 | 20.0 | 42.0 |
| [AIトレーニングでGPUが無駄に待機状態になってしまっている理由とAdobeが行った対処とは？](https://gigazine.net/news/20260826-gpu-idle/) | 27.0 | 20.0 | 42.0 |
| [選べる相棒：AI SOC向けモデル選定における相反する要件のバランス調整](https://blog.talosintelligence.com/choose-your-fighter-balancing-competing-requirements-to-select-models-for-your-ai-soc/) | 27.0 | 20.0 | 42.0 |
| [エフサステクノロジーズとNTT西、純国産LLM「tsuzumi 2」によるオンプレミス生成AI基盤を提供](https://japan.zdnet.com/article/35251949/) | 26.0 | 20.0 | 42.0 |
| [OpenAI：Hugging Face侵入につながったエージェントの行動は5月に形成された](https://cyberscoop.com/openai-hugging-face-agent-breach-report/) | 25.0 | 20.0 | 42.0 |
| [Carharttのデータ侵害、1,290万人に影響　ShinyHuntersの主張の半数](https://www.theregister.com/security/2026/08/26/carhartt-data-breach-affects-129m-half-of-what-shinyhunters-claimed/5292626) | 25.0 | 20.0 | 42.0 |
| [TrendAI™、CyberGymのエージェント型AIセキュリティベンチマークで首位獲得](https://newsroom.trendmicro.com/2026-08-26-TrendAI-TM-Ranks-First-on-CyberGym-Agentic-AI-Security-Benchmark) | 25.0 | 20.0 | 42.0 |
| [AIツールの5本中4本がITの監督なしで運用されていることが新調査で判明](https://www.infosecurity-magazine.com/news/four-in-five-ai-tools-no-it/) | 25.0 | 20.0 | 42.0 |
| [CoyoteではなくRoad Runner: 自律型AI攻撃の実態](https://www.akamai.com/blog/ai/2026/aug/road-runner-effect-autonomous-ai-attacks) | 25.0 | 20.0 | 42.0 |
| [AnonyMousKITのフィッシング・アズ・ア・サービスがAI音声通話でiPhoneのパスコードを窃取](https://www.helpnetsecurity.com/2026/08/26/anonymouskit-phishing-stolen-iphone/) | 25.0 | 20.0 | 42.0 |
| [キューのないSOCを実現する：アラート滞留からAI仮説エンジンへ](https://thehackernews.com/2026/08/imagine-soc-without-queue-from-alert.html) | 25.0 | 20.0 | 42.0 |
| [Claude Opus 4.6がテストでジム予約制限を回避し、他ユーザーの予約をキャンセル](https://thehackernews.com/2026/08/claude-opus-46-bypasses-gym-booking.html) | 25.0 | 20.0 | 42.0 |
| [OpenAIが影響工作に利用されたロシアのChatGPTアカウントを禁止](https://thehackernews.com/2026/08/openai-bans-russian-chatgpt-accounts.html) | 25.0 | 20.0 | 42.0 |
| [Linux FoundationがAIランタイム証跡のためのTRACE標準を導入](https://www.infosecurity-magazine.com/news/linux-foundation-trace-standard-ai/) | 25.0 | 20.0 | 42.0 |
| [未修正のKaltura mwEmbedの脆弱性により、リモート攻撃者がファイルを読み取りコードを実行可能にする](https://thehackernews.com/2026/08/unpatched-kaltura-mwembed-flaws-could.html) | 24.0 | 46.0 | 50.0 |
| [パッチ公開後も数百台のZimbraサーバーが侵害される](https://www.itpro.com/security/cyber-attacks/hackers-have-breached-hundreds-of-zimbra-servers-despite-a-patch-having-been-available-for-weeks) | 24.0 | 38.0 | 42.0 |
| [GPUThor攻撃でNVIDIA ECC保護を回避しroot権限を取得する手法](https://www.bleepingcomputer.com/news/security/new-gputhor-attack-defeats-nvidia-ecc-protection-for-root-access/) | 22.0 | 32.0 | 42.0 |
| [AIインフラが標的になるとき：ゲートウェイと制御ポイントの防御](https://www.microsoft.com/en-us/security/blog/2026/08/26/when-ai-infrastructure-becomes-target-securing-gateways-control-points/) | 22.0 | 20.0 | 42.0 |
| [HackersがMicrosoft SharePointのRCEチェーンをPoCエクスプロイトで標的にする](https://www.bleepingcomputer.com/news/security/hackers-target-microsoft-sharepoint-rce-chain-with-poc-exploit/) | 22.0 | 20.0 | 42.0 |
| [レンタルサーバ設備で侵害、サービスを一時停止 - NTTスマートコネクト](https://www.security-next.com/189422) | 22.0 | 20.0 | 42.0 |
| [eギフトサービスのシステムが侵害、不正交換も - 全日空商事](https://www.security-next.com/189424) | 22.0 | 20.0 | 42.0 |
| [「ホロライブ」カードゲームの公式サイトに不正アクセスの痕跡 CMSの脆弱性突かれたか](https://www.itmedia.co.jp/news/article/2608/26/2000000811/) | 21.0 | 20.0 | 42.0 |
| [UbiquitiのUniFi製品群で修正された3件の深刻なセキュリティ脆弱性](https://cyberscoop.com/ubiquiti-unifi-critical-vulnerabilities-patched/) | 20.0 | 28.0 | 50.0 |
| [Chrome を再び使う前に更新してください](https://www.malwarebytes.com/blog/bugs/2026/08/update-chrome-before-you-browse-again) | 20.0 | 28.0 | 50.0 |
| [7月のサイバー攻撃で100以上の水道システムが被害に遭う](https://www.theregister.com/cyber-crime/2026/08/26/more-than-100-water-systems-were-hit-in-july-cyberattacks/5292685) | 20.0 | 20.0 | 48.0 |
| [Boston Scientific、サイバー攻撃で出荷業務に障害](https://therecord.media/boston-scientific-cyberattack-disrupts-shipment-processes) | 20.0 | 20.0 | 42.0 |
| [米国、Federal Reserve・DOJ・上院への攻撃に使われたとされる中国製ハッキングツールを摘発](https://therecord.media/qscan-qtrouter-us-takedown-alleged-china-hacking-tools) | 20.0 | 20.0 | 42.0 |
| [Cisco、2026年9月2日公開予定のセキュリティアドバイザリ事前通知](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-notice-f2SiMFxl) | 20.0 | 20.0 | 42.0 |
| [Boston Scientific、進行中のサイバー攻撃による世界的な混乱を公表](https://www.theregister.com/security/2026/08/26/boston-scientific-discloses-global-disruption-in-ongoing-cyberattack/5292641) | 20.0 | 20.0 | 42.0 |
| [Boston Scientificがサイバー攻撃で世界的な業務に影響と発表](https://www.bleepingcomputer.com/news/security/boston-scientific-says-cyberattack-disrupted-operations-globally/) | 20.0 | 20.0 | 42.0 |
| [Cloudリスクの現状2026：セキュリティ上の検出事項の多くは実際の攻撃機会ではない](https://www.wiz.io/blog/cloud-risk-report-2026) | 20.0 | 20.0 | 42.0 |
| [FBIが中国のスパイ活動を可能にしていたプロキシネットワークを壊滅](https://www.bleepingcomputer.com/news/security/fbi-disrupts-proxy-network-enabling-chinese-espionage-operations/) | 20.0 | 20.0 | 42.0 |
| [Snowflakeがサービスアカウントのパスワードを廃止、次の課題は難題に](https://www.bleepingcomputer.com/news/security/snowflake-ends-service-account-passwords-now-comes-the-hard-part/) | 20.0 | 20.0 | 42.0 |
| [Boston Scientific、サイバー攻撃により受注処理と出荷に影響と発表](https://www.cybersecuritydive.com/news/boston-scientific-cyberattack-disrupted-order-processing-shipping/828816/) | 20.0 | 20.0 | 42.0 |
| [選挙当局者、Tina Peters氏はコンサルタントにとどまり選挙システムへのアクセスは認めないと表明](https://cyberscoop.com/shasta-county-election-clint-curtis-tina-peters-controversy/) | 20.0 | 20.0 | 42.0 |
| [InterpolのOperation Jackal IV、サイバー犯罪容疑者263人を特定](https://www.infosecurity-magazine.com/news/interpol-operation-jackal-iv/) | 20.0 | 20.0 | 42.0 |
| [CISAレッドチームが重要インフラ組織2社を侵害、1社は検知できず](https://thehackernews.com/2026/08/cisa-red-team-compromised-two-critical.html) | 20.0 | 20.0 | 42.0 |
| [AdobeとNvidiaが数十件の脆弱性を修正](https://www.securityweek.com/adobe-and-nvidia-patch-dozens-of-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [人気の学校向けアプリが生徒データを広告主と共有している可能性](https://www.malwarebytes.com/blog/privacy/2026/08/popular-school-apps-may-be-sharing-student-data-with-advertisers) | 20.0 | 20.0 | 42.0 |
| [保険金請求件数は減少も、サイバー保険の平均損失額は増加](https://www.infosecurity-magazine.com/news/cyber-insurance-losses-increase/) | 20.0 | 20.0 | 42.0 |
| [財務省、金融機関の耐量子暗号への移行を支援](https://www.cybersecuritydive.com/news/quantum-cryptography-treasury-task-force-financial-industry/828732/) | 20.0 | 20.0 | 42.0 |
| [NovaCookiesキットがMicrosoft 365セッションを盗む、月額320ドルで提供](https://www.darkreading.com/endpoint-security/novacookies-steals-microsoft-365-sessions-320-a-month) | 20.0 | 20.0 | 42.0 |
| [CISA: 7月のサイバー攻撃で100以上のインターネット公開水道システムが標的に](https://www.securityweek.com/cisa-over-100-internet-exposed-water-systems-targeted-in-july-cyberattacks/) | 20.0 | 20.0 | 42.0 |
| [MFA認証の落とし穴：認証が生むセキュリティの錯覚](https://www.securityweek.com/the-mfa-identity-trap-when-authentication-creates-a-false-sense-of-security/) | 20.0 | 20.0 | 42.0 |
| [RightCrowd Passがモバイル・物理・生体認証の資格情報を統合](https://www.helpnetsecurity.com/2026/08/26/rightcrowd-pass-credentialing-solution/) | 20.0 | 20.0 | 42.0 |
| [偽の採用担当者がモバイルで高価値な企業認証情報を狙う](https://www.helpnetsecurity.com/2026/08/26/recruitment-scam-corporate-passwords-mobile/) | 20.0 | 20.0 | 42.0 |
| [Web層で予防対策を講じる方法](https://www.security.com/product-insights/how-take-prevention-web-layer) | 20.0 | 20.0 | 42.0 |

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
