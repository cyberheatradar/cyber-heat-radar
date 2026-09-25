# 📡 サイレーダー 2026-09-26 05:00 JST

このレポートは、2026-09-25 17:00 JST〜2026-09-26 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 82
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 53

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CISA Adds Two Known Exploited Vulnerabilities to Catalog](#topic-34326) | 46.0 | 38.0 | 47.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 / audio_eligible_by_public_rules_false |
| 2 | [Roundcube Pre-Auth SQL Injection Flaw Actively Exploited in the Wild](#topic-34302) | 38.0 | 46.0 | 55.0 | 音声 | 温度感上位枠 |
| 3 | [In Other News: Clop Leak Site Takeover, Docker Botnet Hunts AI Keys, Water Utility Exposure](#topic-34375) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 4 | [With the Rise of AI Agents, SOC 2 Should Adapt or Risk Irrelevance](#topic-34381) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-34302"></a>

### 1. Roundcube Pre-Auth SQL Injection Flaw Actively Exploited in the Wild

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 38.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

Roundcube Webmail の脆弱性「CVE-2026-48842」について、認証前に悪用可能なSQLインジェクションであり、実際の悪用が観測されていると報告されています。
影響範囲としては、Roundcube Webmail の 1.6.x 系の一部および 1.7.x 系の旧バージョンが挙げられています。
認証なしで悪用できる脆弱性は、外部公開されたメール環境にとって特にリスクが高く、早急な確認と更新が重要です。
すでに悪用観測があるため、単なる未修正脆弱性よりも優先度を上げて対応する必要があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Roundcube の導入有無とバージョンを確認し、該当する場合は修正版への更新状況を点検する。
- 外部公開の Webmail 入口について、アクセスログや不審な問い合わせの有無を確認する。
- 影響が疑われる場合は、関連アカウントの監査と必要に応じた認証情報の見直しを行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-48842 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-48842](https://nvd.nist.gov/vuln/detail/CVE-2026-48842) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Roundcube Pre-Auth SQL Injection Flaw Actively Exploited in the Wild](https://thehackernews.com/2026/09/roundcube-pre-auth-sql-injection-flaw.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Roundcube Webmail Vulnerability in Attackers’ Crosshairs](https://www.securityweek.com/roundcube-webmail-vulnerability-in-attackers-crosshairs/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-34375"></a>

### 2. In Other News: Clop Leak Site Takeover, Docker Botnet Hunts AI Keys, Water Utility Exposure

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

SecurityWeekは、Clopのリークサイトに関する動き、Docker環境を狙ってAI関連の鍵を探すボットネット、そして水道関連インフラの露出に関する複数の話題をまとめて伝えています。
いずれも個別の詳細は限定的ですが、AI利用環境やコンテナ、重要インフラ周辺のリスクが並行して意識されている状況を示しています。
AIサービスの利用拡大に伴い、認証情報や秘密鍵の管理不備が狙われやすくなっています。
加えて、コンテナ基盤や重要インフラの露出は、被害の広がりや運用停止につながる可能性があるため注意が必要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Dockerや関連基盤に置かれた秘密情報・API鍵の保管場所を見直し、不要な露出がないか確認する。
- AIアシスタントや連携サービスで使う認証情報の棚卸しとローテーション方針を確認する。
- 重要インフラや制御系に関わる公開設定、外部到達性、監視アラートを再点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ランサムウェアグループ | Clop | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [In Other News: Clop Leak Site Takeover, Docker Botnet Hunts AI Keys, Water Utili](https://www.securityweek.com/in-other-news-clop-leak-site-takeover-docker-botnet-hunts-ai-keys-water-utility-exposure/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34381"></a>

### 3. With the Rise of AI Agents, SOC 2 Should Adapt or Risk Irrelevance

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

AIエージェントが人間の認証情報を使って操作できるようになると、既存のSOC 2統制では人の操作と区別しにくい場面が出る可能性があると指摘されています。
こうした変化に対応するため、AIエージェント固有の識別や権限管理を含めて統制の見直しが必要だという論点です。
SOC 2は多くの企業で監査・信頼性の基準として使われており、AIエージェントの普及で前提が崩れると実務上の統制設計に影響します。
人と同様に振る舞う自動化主体をどう扱うかは、アクセス管理や監査証跡の考え方に直結します。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIエージェントを「人の操作」と同一視せず、専用の識別子や権限区分を設けられるか確認する。
- 監査証跡で、誰が・何を・どの主体が実行したのかを追跡できる形に整備する。
- 既存のSOC 2統制が自動化主体の利用を前提にしていない箇所がないか、アクセス管理と承認フローを点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [With the Rise of AI Agents, SOC 2 Should Adapt or Risk Irrelevance](https://www.bleepingcomputer.com/news/security/with-the-rise-of-ai-agents-soc-2-should-adapt-or-risk-irrelevance/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-34326"></a>

### 1. CISA Adds Two Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 46.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 47.0 |

#### 概要

CISAが、実際の悪用が確認されている脆弱性をKnown Exploited Vulnerabilities（KEV）カタログに追加したと公表しました。
材料にはWSO2やAdobe Commerce/Magentoに関する脆弱性が含まれており、公開情報上は複数の製品が対象として挙げられています。
KEVへの追加は、攻撃者による悪用が現実に起きている可能性を示すため、優先度の高い対応対象になります。
広く利用される製品が含まれる場合、未対処の環境への影響が大きくなりやすい点も注目されます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象製品の利用有無を確認し、該当する場合はベンダーの修正版や緩和策の適用状況を点検する。
- 資産管理と脆弱性管理の台帳を突き合わせ、外部公開されているインスタンスや更新停止環境を優先的に確認する。
- 監視ログやアラートを見直し、異常なアクセスや不審な管理操作の兆候がないか重点的に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| ベンダー | Adobe | 言及あり | 0.80 | — |
| 製品 | Adobe Commerce | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Two Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/09/25/cisa-adds-two-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [WSO2 and Adobe Commerce Flaws Exploited in Attacks, Added to CISA KEV](https://thehackernews.com/2026/09/wso2-and-adobe-commerce-flaws-exploited.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
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
| [侵害されたGitHub Actionsが再稼働し、Mini Shai-Huludマルウェアの実行を再開](https://thehackernews.com/2026/09/compromised-github-actions-came-back.html) | 28.0 | 45.0 | 42.0 |
| [KothamineマルウェアがTailscaleのtailcatを悪用してネットワーク検知を回避](https://www.malwarebytes.com/blog/threat-intel/2026/09/kothamine-malware-uses-tailscales-tailcat-to-evade-network-detection) | 28.0 | 20.0 | 42.0 |
| [FamousSparrowが新たなSparroWockyバックドアを用いて活動を拡大](https://blog.polyswarm.io/famoussparrow-takes-flight-with-new-sparrowocky-backdoor) | 28.0 | 20.0 | 42.0 |
| [PamStealer macOSマルウェア、ライブC2ペイロードの復号と多層的な永続化を追加](https://thehackernews.com/2026/09/pamstealer-macos-malware-adds-live-c2.html) | 28.0 | 20.0 | 42.0 |
| [Bitget、バックエンド侵害で北朝鮮系ハッカーに3億5160万ドルを盗まれた可能性があると発表](https://thehackernews.com/2026/09/bitget-says-suspected-north-korean.html) | 28.0 | 20.0 | 42.0 |
| [MacSync情報窃取マルウェア、iCloudカレンダーに悪意あるコマンドを隠蔽](https://www.helpnetsecurity.com/2026/09/25/macsync-info-stealing-malware-for-macos/) | 28.0 | 20.0 | 42.0 |
| [AIに「StarCraft」をリアルタイムで戦わせる「Brood War Bench」が登場、全モデルが初心者レベルながらCodex Astraは18戦全勝](https://gigazine.net/news/20260925-starcraft-brood-war-bench/) | 27.0 | 20.0 | 42.0 |
| [AIサンドボックス脱出：封じ込めよりもフォレンジック対応準備が重要な理由](https://www.darkreading.com/cyberattacks-data-breaches/ai-sandbox-escapes-forensic-readiness) | 25.0 | 20.0 | 42.0 |
| [見落としていたこと：Google GeminiがAI脱出パーティーに参加](https://www.darkreading.com/cyber-risk/what-we-missed-google-gemini-ai-escape-party) | 25.0 | 20.0 | 42.0 |
| [Anthropic、クラウドセッション限定でClaude Codeの無料クレジット最大250ドルを提供](https://www.bleepingcomputer.com/news/artificial-intelligence/anthropic-rolls-out-up-to-250-in-free-claude-code-credits-but-only-for-cloud-sessions/) | 25.0 | 20.0 | 42.0 |
| [企業は技術への安心感の高まりに伴いAIのサイバーセキュリティ活用を拡大している](https://www.cybersecuritydive.com/news/ai-cybersecurity-maturity-agents-kpmg/831385/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、より高速なCodexを備えた月額500ドルのChatGPT Pro Maxプランを準備中](https://www.bleepingcomputer.com/news/artificial-intelligence/openai-is-preparing-a-500-chatgpt-pro-max-plan-with-faster-codex/) | 25.0 | 20.0 | 42.0 |
| [Salesforce Agentforceのゼロクリック脆弱性が示すAIエージェントのリスク拡大](https://www.infosecurity-magazine.com/news/vulnerabilities-salesforce-ai/) | 25.0 | 20.0 | 42.0 |
| [ANY.RUNがRootedCON Valencia 2026で紹介する、サイバーセキュリティと次世代AIの融合](https://any.run/cybersecurity-blog/rootedcon-valencia-2026/) | 25.0 | 20.0 | 42.0 |
| [OpenAIエージェントが豪州Medicareポータルをハッキングしたとの主張に疑念が高まる](https://therecord.media/openai-australia-breach-cyber) | 25.0 | 20.0 | 42.0 |
| [SOCはすべてのアラートごとにゼロから始める必要はない](https://thehackernews.com/2026/09/the-soc-doesnt-need-to-start-over-with.html) | 25.0 | 20.0 | 42.0 |
| [OpenAIとAnthropic、英国AI Security Instituteへの新型AIモデル提供を停止する可能性](https://www.itpro.com/security/openai-and-anthropic-snub-uks-ai-security-institute-on-new-model-testing) | 25.0 | 20.0 | 42.0 |
| [CISOsの約半数がAIディープフェイク音声通話の被害に遭遇](https://www.itpro.com/security/cyber-crime/nearly-half-of-cisos-have-been-hit-by-ai-deepfake-voice-calls-heres-how-to-spot-the-tell-tale-signs-youre-being-scammed) | 25.0 | 20.0 | 42.0 |
| [Elementor WordPressの脆弱性により攻撃者が管理者アカウントを作成可能にする問題](https://www.bleepingcomputer.com/news/security/elementor-wordpress-flaw-lets-attackers-create-admin-accounts/) | 24.0 | 38.0 | 42.0 |
| [CISAが警告するSharePoint、WSO2、Adobe Commerceの脆弱性悪用攻撃](https://www.bleepingcomputer.com/news/security/cisa-warns-of-sharepoint-wso2-adobe-commerce-flaws-exploited-in-attacks/) | 24.0 | 38.0 | 42.0 |
| [Storm-3168による、侵害されたサービスプリンシパルを悪用したエージェント駆動型クラウド攻撃](https://www.microsoft.com/en-us/security/blog/2026/09/25/storm-3168-agentic-driven-cloud-attacks-using-compromised-service-principals/) | 22.0 | 20.0 | 42.0 |
| [3支店で個人情報含む書類を紛失、誤廃棄の可能性 - 横浜信金](https://www.security-next.com/190323) | 22.0 | 20.0 | 42.0 |
| [オープンキャンパスの関連案内でメール誤送信 - 福岡女学院大](https://www.security-next.com/190445) | 22.0 | 20.0 | 42.0 |
| [医療機器メーカー関係者が患者X線画像を持ち出し - 宝塚市立病院](https://www.security-next.com/190055) | 22.0 | 20.0 | 42.0 |
| [「Next.<wbr>js」の画像生成モジュールにRCEにつながる脆弱性](https://www.security-next.com/190616) | 22.0 | 20.0 | 42.0 |
| [川崎市施設のサイトに不正アクセス - サイト更新時に判明](https://www.security-next.com/190242) | 22.0 | 20.0 | 42.0 |
| [Adobe、7件のセキュリティアドバイザリを公開](https://www.security-next.com/190703) | 22.0 | 20.0 | 42.0 |
| [Gyazoへの不正アクセス、新たに約1.74億件の画像メタデータ流出](https://www.itmedia.co.jp/news/article/2609/25/2000001772/) | 21.0 | 20.0 | 42.0 |
| [富士通、ダークウェブ監視や脅威ハンティングを統合したセキュリティサービス](https://news.mynavi.jp/techplus/article/20260925-5026067/) | 21.0 | 20.0 | 42.0 |
| [Bitget、387.5百万ドルの暗号資産ウォレット流出を北朝鮮の犯行と非難](https://www.theregister.com/cyber-crime/2026/09/25/bitget-blames-north-korea-for-3875m-crypto-wallet-raid/5299218) | 20.0 | 20.0 | 48.0 |
| [Fake Google Security Team広告が「no script reading」と称しながら音声フィッシングでスクリプトを読み上げ、最後にその内容を印字](https://www.theregister.com/security/2026/09/25/fake-google-security-team-ad-says-no-script-reading-in-voice-phishing-then-prints-the-script/5299264) | 20.0 | 20.0 | 42.0 |
| [ShinyHuntersがThe Registerに語る：ビジネスを守るためにFBIをハッキングした](https://www.theregister.com/cyber-crime/2026/09/25/shinyhunters-tells-the-reg-we-hacked-the-fbi-to-protect-our-business/5299250) | 20.0 | 20.0 | 42.0 |
| [最高裁、州による市民権確認にSAVEデータベースの利用を認める](https://cyberscoop.com/supreme-court-save-database-voter-citizenship/) | 20.0 | 20.0 | 42.0 |
| [偽のデスクトップアプリを使って人事担当者をだまし、リモートアクセスを奪う攻撃](https://www.theregister.com/security/2026/09/25/crooks-use-fake-desktop-apps-to-fool-hr-staff-into-giving-them-remote-access/5299226) | 20.0 | 20.0 | 42.0 |
| [LinkedIn、偽プロフィールと職歴の確認強化を追加](https://www.malwarebytes.com/blog/news/2026/09/linkedin-adds-new-checks-for-fake-profiles-and-work-histories) | 20.0 | 20.0 | 42.0 |
| [ウェールズ警察へのサイバー攻撃、職員データに影響の可能性](https://therecord.media/wales-cyberattack-police-breach) | 20.0 | 20.0 | 42.0 |
| [ITワーカー詐欺を防ぐにはHRプロセスの刷新が必要](https://www.darkreading.com/cyber-risk/stopping-it-worker-scams-revamped-hr-process) | 20.0 | 20.0 | 42.0 |
| [北朝鮮による関与が疑われるBitgetの3億5100万ドル相当の暗号資産流出](https://www.securityweek.com/north-korea-suspected-in-351-million-bitget-crypto-heist/) | 20.0 | 20.0 | 42.0 |
| [AgentsがTurnstile SpinでWebサイトのセキュリティを設定可能に](https://blog.cloudflare.com/turnstile-spin/) | 20.0 | 20.0 | 42.0 |
| [犯罪者がプレースホルダードメインをClickFixの罠に悪用](https://www.malwarebytes.com/blog/news/2026/09/criminals-turn-placeholder-domain-into-clickfix-trap) | 20.0 | 20.0 | 42.0 |
| [CISAの選挙セキュリティ計画、パッチ適用の障壁と有権者データベース攻撃を警告](https://www.securityweek.com/cisa-election-security-plan-flags-patching-barriers-voter-database-attacks/) | 20.0 | 20.0 | 42.0 |
| [CISA、2026年中間選挙に向けた選挙セキュリティ計画を公開](https://www.infosecurity-magazine.com/news/cisa-election-security-midterms/) | 20.0 | 20.0 | 42.0 |
| [Rydoxマーケットプレイスのコソボ人運営者、米国裁判所で有罪認める](https://www.securityweek.com/kosovar-owner-of-rydox-marketplace-pleads-guilty-in-us-court/) | 20.0 | 20.0 | 42.0 |
| [脅威検知ダッシュボードがセキュリティカバレッジのギャップを隠している](https://www.helpnetsecurity.com/2026/09/25/threat-detections-coverage-gaps-report/) | 20.0 | 20.0 | 42.0 |
| [Rydoxマーケットプレイスの管理者が有罪を認め、22年の禁錮刑の可能性](https://www.bleepingcomputer.com/news/security/rydox-marketplace-admin-pleads-guilty-faces-22-years-in-prison/) | 20.0 | 20.0 | 42.0 |
| [Windows、Linux、Androidのファイル通知システムでユーザーの操作状況が漏えいする問題](https://www.securityweek.com/windows-linux-android-file-notification-systems-leak-user-activity/) | 20.0 | 20.0 | 42.0 |
| [Gyazo、不正アクセスで続報。過去に削除された画像のメタデータ約1.74億件も流出](https://internet.watch.impress.co.jp/docs/news/2143465.html) | 20.0 | 20.0 | 42.0 |
| [その配送割引オファーには毎月の課金が付くかもしれない](https://www.malwarebytes.com/blog/threat-intel/2026/09/that-shipping-rebate-offer-may-come-with-a-monthly-charge) | 20.0 | 20.0 | 42.0 |
| [RemControl Banking TrojanがAndroid端末を遠隔操作可能にする脅威](https://www.infosecurity-magazine.com/news/banking-trojan-remote-control/) | 20.0 | 20.0 | 42.0 |
| [Salesforce Agentforceの「SalesBleed」脆弱性によりゼロクリックでデータ流出が可能に](https://www.securityweek.com/salesbleed-flaws-in-salesforce-agentforce-enabled-zero-click-data-exfiltration/) | 20.0 | 20.0 | 42.0 |
| [CISAがCVEプログラムに大改革を計画する理由](https://www.itpro.com/security/how-cisa-plans-to-shake-up-the-cve-program) | 20.0 | 20.0 | 42.0 |
| [Bitgetの暗号資産取引所ハッキングで3億5160万ドルが流出](https://www.bleepingcomputer.com/news/security/hackers-steal-3516-million-in-bitget-crypto-exchange-hack/) | 20.0 | 20.0 | 42.0 |
| [Researchers Identify AliExpressを狙うフィッシングドメインを登録前に特定](https://www.infosecurity-magazine.com/news/aliexpress-phishing-flagged-early/) | 20.0 | 20.0 | 42.0 |

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
