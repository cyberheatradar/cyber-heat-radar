# 📡 サイレーダー 2026-09-05 05:00 JST

このレポートは、2026-09-04 17:00 JST〜2026-09-05 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 72
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 43

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-85046: CISA KEV catalog addition](#topic-31075) | 51.0 | 46.0 | 55.0 | 音声 | 温度感上位枠 |
| 2 | [Sangoma Switchvox Vulnerabilities Exploited in the Wild](#topic-30655) | 45.0 | 64.0 | 59.0 | 音声 | 温度感上位枠 |
| 3 | [New CrowdStrike 'FalconFlank' zero-day grants SYSTEM privileges](#topic-31063) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Supply Chain of Distrust — Microsoft/GitHub Supply-Chain Compromise Targets AI Developers](#topic-31091) | 33.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Phishing Campaign Sends Millions of Emails Using Invisible Unicode to Evade Filters](#topic-31049) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-31075"></a>

### 1. CVE-2026-85046: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 51.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

CISAは、実際の悪用が確認された脆弱性としてCVE-2026-85046をKEVカタログに追加しました。
関連情報では、GoogleがChrome向けの修正を公開しており、Windows、macOS、Linux向けに更新版が配布されています。
KEV入りは、単なる既知の脆弱性ではなく、優先的な対応が必要とみなされていることを示します。
Chrome系の広範な利用環境に影響しうるため、組織内のブラウザ更新状況の確認が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Chromeの更新適用状況を早急に確認し、未適用端末を優先して更新する。
- CISA KEV掲載のため、資産管理・脆弱性管理の対象として優先度を引き上げる。
- ブラウザ利用端末で不審な挙動がないか確認し、関連ログや検知ルールを見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-85046 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Chromium | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-85046](https://nvd.nist.gov/vuln/detail/CVE-2026-85046) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Google patches actively exploited Chrome zero-day (CVE-2026-85046)](https://www.helpnetsecurity.com/2026/09/04/google-chrome-zero-day-cve-2026-85046/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/09/04/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google warns of new Chrome zero-day flaw exploited in attacks](https://www.bleepingcomputer.com/news/security/google-warns-of-new-chrome-zero-day-flaw-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google Patches 6th Chrome Zero-Day of 2026](https://www.securityweek.com/google-patches-6th-chrome-zero-day-of-2026/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-30655"></a>

### 2. Sangoma Switchvox Vulnerabilities Exploited in the Wild

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

Sangoma Switchvoxに存在するCVE-2026-9586について、複数の公開情報で実際の悪用が観測されていると報じられています。
対象はインターネットに公開された環境で、未認証のSQLインジェクションが遠隔コード実行につながる可能性があるとされています。
VoIP／統合コミュニケーション基盤は業務影響が大きく、侵害されると通話基盤や関連システムに波及するおそれがあります。
悪用が進行中とみられるため、修正適用の有無だけでなく、侵害痕跡の確認が急がれます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
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

#### 担当者向け確認ポイント

- Switchvoxの該当バージョンを利用しているかを確認し、提供元の修正・緩和策を速やかに適用する。
- インターネット公開の管理画面や関連サービスを点検し、不要な露出があれば制限する。
- 異常なログイン試行、SQLエラー、予期しないプロセス起動やシェル生成など、侵害の兆候を重点的に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-9586 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-9586](https://nvd.nist.gov/vuln/detail/CVE-2026-9586) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Sangoma Switchvox Vulnerabilities Exploited in the Wild](https://www.securityweek.com/sangoma-switchvox-vulnerabilities-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers exploit Sangoma Switchvox flaw to deploy reverse shells](https://www.bleepingcomputer.com/news/security/hackers-exploit-sangoma-switchvox-flaw-to-deploy-reverse-shells/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Exploitation of Sangoma Switchvox flaw is underway (CVE-2026-9586)](https://www.helpnetsecurity.com/2026/09/02/exploitation-of-sangoma-switchvox-flaw-underway-cve-2026-9586/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-31063"></a>

### 3. New CrowdStrike 'FalconFlank' zero-day grants SYSTEM privileges

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CrowdStrikeのFalcon製品に関するゼロデイ脆弱性「FalconFlank」が公開されたと報じられています。
更新済みのWindows環境でも権限昇格につながる可能性があるとされていますが、現時点では公開情報ベースの報道であり、詳細な検証状況は不明です。
権限昇格は、端末内での被害拡大や管理者権限の奪取につながり得るため、影響が大きくなりやすい類型です。
セキュリティ製品に関わる問題であれば、監視・防御の前提にも影響しうるため注目されます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- CrowdStrike Falconの利用有無と対象端末を確認し、ベンダーの修正情報や注意喚起を継続監視する。
- Windows端末で不審な権限昇格や設定変更の兆候がないか、EDRや監査ログを確認する。
- 関連する保護策や運用手順を見直し、必要に応じて優先度を上げて適用する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | CrowdStrike | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New CrowdStrike 'FalconFlank' zero-day grants SYSTEM privileges](https://www.bleepingcomputer.com/news/security/new-crowdstrike-falconflank-zero-day-grants-system-privileges/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-31091"></a>

### 4. Supply Chain of Distrust — Microsoft/GitHub Supply-Chain Compromise Targets AI Developers

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>サ⁠プ⁠ラ⁠イ⁠チ⁠ェ⁠ー⁠ン</nobr> / <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoft/GitHubに関するサプライチェーン侵害を扱う話題で、AI開発者向けのコーディング環境が単なる作業ツールではなく、重要な供給網の一部として見なされつつあることが示されています。
公開情報の範囲では、開発環境や関連ツールが攻撃対象になり得るという文脈が中心で、詳細な被害範囲は確認できません。
AI支援の開発環境は、ソースコードや認証情報、依存関係管理に近く、侵害されると影響が広がりやすいため注目されています。
開発・CI/CDの保護が、通常の端末対策以上に重要になっていることを示す事例です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI開発ツールやGitHub連携の権限・トークン管理を見直す。
- 依存関係や拡張機能の導入元を厳格に確認し、更新監視を行う。
- 開発端末とCI/CDでの監査ログ収集、異常検知、最小権限を徹底する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Supply Chain of Distrust — Microsoft/GitHub Supply-Chain Compromise Targets AI D](https://securityboulevard.com/2026/09/supply-chain-of-distrust-microsoft-github-supply-chain-compromise-targets-ai-developers/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-31049"></a>

### 5. Phishing Campaign Sends Millions of Emails Using Invisible Unicode to Evade Filters

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftは、不可視のUnicode文字を使ってメールフィルターの解析を回避しようとする大規模なフィッシングキャンペーンを確認したとしています。
受信者からは見えにくい形で文面を分割し、資金援助などを装う誘導文を通しやすくしていたと説明されています。
従来のキーワードベースや単純な文字列解析に依存する防御では、こうした見えない文字を使った回避を見落とす可能性があります。
メール防御の設定や検知ロジックを見直すきっかけになるため、実務上の示唆があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- メールゲートウェイやフィルターが不可視文字・特殊Unicodeを正規化できるか確認する。
- フィッシング判定を文面の見た目だけでなく、文字コードや正規化後の内容も含めて評価する。
- 不審な資金調達・請求・支払い関連メールについて、利用者向け注意喚起と報告導線を再確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Phishing Campaign Sends Millions of Emails Using Invisible Unicode to Evade Filt](https://thehackernews.com/2026/09/phishing-campaign-sends-millions-of.html) | <nobr>内容確認・補足情報</nobr> |

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
| [Super FormsとElementor ProのRCE脆弱性を狙う44万件超の攻撃試行](https://thehackernews.com/2026/09/over-440000-exploit-attempts-target.html) | 32.0 | 46.0 | 50.0 |
| [BlueDeltaがHOOKEDGEで欧州を標的にした諜報活動](https://blog.polyswarm.io/hooked-on-espionage-bluedelta-targets-europe-with-hookedge) | 28.0 | 20.0 | 42.0 |
| [Malwarebytes の近代化を支える見えない作業](https://www.malwarebytes.com/blog/inside-malwarebytes/2026/09/the-hidden-work-of-modernizing-malwarebytes) | 28.0 | 20.0 | 42.0 |
| [「DDoS攻撃の件数は減少も、攻撃は高度化」ボットネットの制御精度向上](https://www.itpro.com/security/cyber-attacks/attackers-are-steering-their-botnets-with-greater-precision-and-control-ddos-attack-numbers-might-be-dwindling-but-theyre-intensifying) | 28.0 | 20.0 | 42.0 |
| [使い込むほど成長するAIエージェント「Hermes Agent」の実行結果をメールで受け取ってみた](https://gigazine.net/news/20260905-hermes-agent-mail/) | 27.0 | 20.0 | 42.0 |
| [従業員が個人利用の生成AIに顧客情報を誤アップロード - RIZAP](https://www.security-next.com/189853) | 27.0 | 20.0 | 42.0 |
| [ChatGPT・Claude・Grokがほぼ同時刻にダウン](https://gigazine.net/news/20260904-openai-anthropic-spacexai-down/) | 27.0 | 20.0 | 42.0 |
| [12年前のPostgreSQL脆弱性でデータベースとサーバーが乗っ取り可能に](https://thehackernews.com/2026/09/postgresql-fixes-12-year-old-logical.html) | 26.0 | 28.0 | 54.0 |
| [サントリー新商品の店頭POPに“生成AI疑惑” 成分表示にも誤りで物議……同社に事実関係を聞いた](https://www.itmedia.co.jp/news/article/2609/04/2000001197/) | 26.0 | 20.0 | 42.0 |
| [OpenAI、重要インフラ防御者向けに最先端AI導入へ10億ドルを拠出](https://www.securityweek.com/openai-pledges-1-billion-to-bring-frontier-ai-to-critical-infrastructure-defenders/) | 25.0 | 20.0 | 42.0 |
| [Rogue OpenAIエージェントが5月に死んだドイツのWebサイトを通信に利用、Hugging Face事件の数カ月前](https://www.theregister.com/ai-and-ml/2026/09/04/rogue-openai-agents-used-dead-german-web-site-to-communicate-in-may-months-before-hugging-face-incident/5294554) | 25.0 | 20.0 | 42.0 |
| [OpenAIが最前線のサイバー防御者向けに資源と訓練を提供するため10億ドルを拠出へ](https://www.cybersecuritydive.com/news/openai-pledges-1-billion-resources-cyber-defenders/829676/) | 25.0 | 20.0 | 42.0 |
| [AIが隠れた脆弱性の時代を終わらせる――ベンダーは対応できているか](https://www.darkreading.com/vulnerabilities-threats/ai-ending-era-hidden-vulnerabilities-are-vendors-ready) | 25.0 | 20.0 | 42.0 |
| [Synology ActiveProtect Manager 2.0、AI駆動のセキュリティを強化](https://www.helpnetsecurity.com/2026/09/04/synology-activeprotect-manager-2-0-data-protection/) | 25.0 | 20.0 | 42.0 |
| [CatchがAIエグゼクティブアシスタント向けガードレール機能で500万ドルを調達](https://www.securityweek.com/catch-raises-5-million-for-ai-executive-assistant-with-guardrails/) | 25.0 | 20.0 | 42.0 |
| [AIコーディングエージェントが企業ネットワークに未知・未信頼のコードをインストールしている](https://securityboulevard.com/2026/09/ai-coding-agents-are-installing-unknown-untrusted-code-on-corporate-networks/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、AIサイバーセキュリティツールを社会インフラ向けに展開するため10億ドルを拠出](https://www.infosecurity-magazine.com/news/openai-pledges-ai-tools-essential/) | 25.0 | 20.0 | 42.0 |
| [「AIは生産性向上の付属機能ではなく運用インフラになりつつある」――昨日の3重AI障害は企業への警鐘だ](https://www.itpro.com/security/ai-is-increasingly-becoming-operational-infrastructure-rather-than-a-productivity-add-on-yesterdays-triple-ai-outage-should-be-a-wake-up-call-for-enterprises) | 25.0 | 20.0 | 42.0 |
| [NVIDIAがAIプラットフォームHugging Faceを130億ドルで買収](https://www.securityweek.com/nvidia-is-buying-ai-platform-hugging-face-for-13-billion/) | 25.0 | 20.0 | 42.0 |
| [AIは本当にアプリケーション保守コストを削減できるのか、それともコードを増やすだけなのか](https://securityboulevard.com/2026/09/can-ai-actually-reduce-application-maintenance-costs-or-does-it-just-generate-more-code/) | 25.0 | 20.0 | 42.0 |
| [SCOMの攻撃と防御：Management ServerリレーとRun As資格情報の取得](https://securityboulevard.com/2026/09/attacking-and-defending-scom-management-server-relay-and-obtaining-run-as-credentials/) | 25.0 | 20.0 | 42.0 |
| [HPEがAOS-CXの重大なRCE脆弱性を修正](https://www.securityweek.com/hpe-patches-critical-rce-vulnerabilities-in-aos-cx/) | 24.0 | 46.0 | 50.0 |
| [HP作成のOEMサービスで侵害 - 顧客情報流出の可能性](https://www.security-next.com/189127) | 22.0 | 20.0 | 42.0 |
| [生物多様性センターのサイトが改ざん、影響など調査 - 千葉県](https://www.security-next.com/189725) | 22.0 | 20.0 | 42.0 |
| [テスラがハンドルもペダルもない専用車両「Cybercab」をロボタクシーサービスに投入](https://gigazine.net/news/20260904-tesla-cybercab/) | 22.0 | 20.0 | 42.0 |
| [「Anthropicはいまだサプライチェーンリスクであると認識している」と国防次官が主張、ラトニック商務長官による「我々はAnthropicを信頼している」の発言翌日](https://gigazine.net/news/20260904-anthropic-lutnick-dod/) | 22.0 | 20.0 | 42.0 |
| [SEGAそっくりのロゴで「MAGA」――トランプ政権公開のWebゲームが物議 移民送還などを題材に 【追記あり】](https://www.itmedia.co.jp/news/article/2609/04/2000001191/) | 21.0 | 20.0 | 42.0 |
| [IDScanが153万人分の運転者情報に影響したとされるデータ侵害で提訴される](https://www.bleepingcomputer.com/news/security/idscan-sued-over-alleged-data-breach-affecting-153-million-drivers/) | 20.0 | 20.0 | 42.0 |
| [Microsoftのクラウド向けパッチ、Dropboxアカウントの侵害、Guardioの11億ドル評価額](https://www.securityweek.com/in-other-news-microsofts-cloud-patches-hacked-dropbox-accounts-guardios-1-1b-valuation/) | 20.0 | 20.0 | 42.0 |
| [企業は自動化攻撃への備えを6か月以内に整える必要がある](https://www.darkreading.com/cybersecurity-operations/companies-six-months-prepare-automated-attacks) | 20.0 | 20.0 | 42.0 |
| [Nvidiaの129億ドル規模のHugging Face提携が企業にもたらす恩恵](https://www.cybersecuritydive.com/news/Nvidia-acquires-hugging-face-enterprises/829697/) | 20.0 | 20.0 | 42.0 |
| [Citrix NetScalerの認証回避の重大な脆弱性が攻撃に悪用され始める](https://www.bleepingcomputer.com/news/security/hackers-target-critical-citrix-netscaler-auth-bypass-in-attacks/) | 20.0 | 20.0 | 42.0 |
| [Tedバックドアが被害者自身のHAProxyビルド内に潜みWebトラフィックを傍受](https://thehackernews.com/2026/09/new-ted-backdoor-hides-inside-victims.html) | 20.0 | 20.0 | 42.0 |
| [Passkey認証を破る39の新手法](https://www.bleepingcomputer.com/news/security/39-new-methods-that-compromise-passkey-authentication/) | 20.0 | 20.0 | 42.0 |
| [ウクライナのドローン脅威を受けロシアのデータセンターに新たなセキュリティ要件](https://therecord.media/russia-data-centers-ukraine-drone-threats) | 20.0 | 20.0 | 42.0 |
| [G7が組織に量子サイバー脅威への備えを促す](https://therecord.media/g7-urges-organizations-to-prepare-for-quantum-threats) | 20.0 | 20.0 | 42.0 |
| [X Moneyの展開に関連したパスワードリセット攻撃](https://www.malwarebytes.com/blog/scams/2026/09/x-money-rollout-linked-to-password-reset-attacks) | 20.0 | 20.0 | 42.0 |
| [VMware WorkstationおよびFusionの更新で重大な脆弱性を修正](https://www.securityweek.com/vmware-workstation-and-fusion-updates-patch-critical-vulnerability/) | 20.0 | 20.0 | 42.0 |
| [サイバーセキュリティを決定づけるスキルとしての判断力](https://cyberscoop.com/ai-security-operations-human-context-ciso-op-ed/) | 20.0 | 20.0 | 42.0 |
| [G7、量子耐性サイバーセキュリティ規則の迅速な整備を要請](https://www.infosecurity-magazine.com/news/g7-urges-quantum-safe-cyber-rules/) | 20.0 | 20.0 | 42.0 |
| [無料のストリーミングボックスが自宅回線を犯罪通信の中継に使っている可能性](https://www.malwarebytes.com/blog/news/2026/09/free-streaming-boxes-may-be-routing-criminal-traffic-through-your-home) | 20.0 | 20.0 | 42.0 |
| [Microsoft TeamsでQRコードを悪用したフィッシングが大幅に困難に](https://www.helpnetsecurity.com/2026/09/04/microsoft-teams-qr-code-phishing-protection/) | 20.0 | 20.0 | 42.0 |
| [Kaseya、Datto RMM向けに新たなコンプライアンスとAppleデバイス管理ツールを発表](https://www.itpro.com/security/data-protection/kaseya-announces-new-compliance-and-apple-device-management-tools-for-datto-rmm) | 20.0 | 20.0 | 42.0 |

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
