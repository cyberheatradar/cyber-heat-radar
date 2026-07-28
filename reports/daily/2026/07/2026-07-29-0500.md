# 📡 サイレーダー 2026-07-29 05:00 JST

このレポートは、2026-07-28 17:00 JST〜2026-07-29 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 111
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 80

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Arista patches actively exploited VeloCloud bug as CISA puts admins on the clock](#topic-24769) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [Microsoft launches agentic security platform designed to combat AI-based attacks](#topic-24675) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [Cyberhaven launches Flow to secure data across human and AI workflows](#topic-24704) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [The Next Evolution of MDR: Preemptive Defense and Agentic Investigation](#topic-24709) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Notes from Underground: Adversarial Prompt Injection](#topic-24733) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-24769"></a>

### 1. Arista patches actively exploited VeloCloud bug as CISA puts admins on the clock

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

AristaがVeloCloud関連の脆弱性に対する修正を公開し、当該問題はすでに悪用が観測されているとされています。
未認証でのコマンドインジェクションに関係する可能性があり、管理対象のEdge機器に影響するおそれがあるとされています。
実際の悪用が示唆されているため、放置すると管理機器の侵害につながる可能性があります。CISAが管理者対応を促している点からも、影響範囲の確認と迅速な適用が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象となるArista VeloCloud関連機器の有無を確認し、修正状況を把握する。
- ベンダー公開情報とCISAの勧告を確認し、優先度を上げて更新を検討する。
- 管理インターフェースや関連ログを点検し、不審な操作や侵入の兆候がないか確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Arista patches actively exploited VeloCloud bug as CISA puts admins on the clock](https://www.theregister.com/security/2026/07/28/arista-patches-actively-exploited-velocloud-bug-as-cisa-puts-admins-on-the-clock/5279414) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-24675"></a>

### 2. Microsoft launches agentic security platform designed to combat AI-based attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftが、AIを悪用した攻撃への対策を意識した「agentic」型のセキュリティ基盤を発表したとされています。
背景には、攻撃者が自律的な手法を使ってキャンペーンを展開できるのではないかという懸念があり、AI時代の防御強化が話題になっています。
AIを使った攻撃の高度化が進む中、防御側も自動化・連携を前提にした体制が求められていることを示す動きです。製品発表として、組織の検知・対応プロセス見直しのきっかけになり得ます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI関連の脅威を前提に、検知・対応フローの自動化余地を確認する。
- 生成AIやエージェント利用時の権限管理、監査、ログ取得の運用を点検する。
- ベンダーの新機能は、既存のSOC/IR運用とどう連携するかを評価する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft launches agentic security platform designed to combat AI-based attacks](https://www.cybersecuritydive.com/news/microsoft-agentic-security-platform-ai-attacks/826365/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-24704"></a>

### 3. Cyberhaven launches Flow to secure data across human and AI workflows

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Cyberhavenは、人的作業とAIワークフローの両方を対象にデータを保護するAIネイティブなデータセキュリティ基盤「Flow」を発表しました。
公開情報では、データの作成・複製・分割・共有といった流れに応じて、行動やID、データのつながりを踏まえて保護を行うことが示されています。
生成AIの利用拡大で、データが人とAIエージェントの間を行き来する場面が増えており、従来の境界型対策だけでは追随しにくくなっています。
データの所在だけでなく、文脈や操作の変化を追う保護の考え方として注目されています。

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

- AI利用時にどのデータが作成・複製・共有されるかを把握し、保護対象を見直す。
- 端末・ブラウザ・AI利用環境をまたぐデータの流れを可視化できるか確認する。
- IDや行動に基づく制御を、既存のDLPやゼロトラスト施策とどう組み合わせるか検討する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Cyberhaven launches Flow to secure data across human and AI workflows](https://www.helpnetsecurity.com/2026/07/28/cyberhaven-flow/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-24709"></a>

### 4. The Next Evolution of MDR: Preemptive Defense and Agentic Investigation

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>A⁠I</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

MDR（Managed Detection and Response）は、アラートを受けてから調べるだけでなく、露出情報や脅威インテリジェンスを先回りして活用する方向に進化しているとされています。
記事では、AIによる反復作業の自動化と、分析結果の最終判断を担う人間の役割を組み合わせることで、調査と対応をより早く進める考え方が示されています。
攻撃の進行が速まる中で、従来の事後対応型の運用だけでは間に合わない可能性があるためです。実務上は、検知・露出管理・インシデント対応を分断せずに連携できるかが重要になります。

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

- アラート対応時に、資産重要度・外部公開状況・脆弱性情報を同時に確認できる運用になっているか見直す。
- AIに繰り返し作業を任せる場合でも、最終判断と説明責任は人が担う前提を明確にする。
- 検知後の対応だけでなく、既知の露出や新規脆弱性を先に評価し、優先順位付けに反映する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [The Next Evolution of MDR: Preemptive Defense and Agentic Investigation](https://www.rapid7.com/blog/post/dr-the-next-evolution-mdr-preemptive-defense-agentic-investigation) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-24733"></a>

### 5. Notes from Underground: Adversarial Prompt Injection

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Proofpointは、地下フォーラムで間接プロンプトインジェクション（IDPI）を悪用するツールや手口の議論・販売が増えていると報告しています。
対象はメール、PDF、カレンダー招待、悪性広告などで、AIエージェントや自動処理系が外部コンテンツを解釈する際に影響を受ける可能性があるとしています。
生成AIやエージェント機能を業務利用する組織では、ユーザーが直接操作しなくても外部入力経由で意図しない動作につながる懸念があります。
現時点では実運用での大規模被害は限定的とみられる一方、今後の攻撃手法の前兆として注意が必要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- メール、添付ファイル、カレンダー招待、Webページなど、AIが自動要約・解析する入力元を重点的に見直す。
- 外部コンテンツを扱うAI/エージェントでは、信頼境界の分離、権限の最小化、危険な指示の無視などの設計を確認する。
- 可視化されない文字列や埋め込みテキストを含む不審な文書・招待・広告に対する検知とレビュー手順を整える。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Proofpoint | 言及あり | 0.80 | — |
| 製品 | Ivanti Connect Secure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Notes from Underground: Adversarial Prompt Injection](https://www.proofpoint.com/us/blog/threat-insight/notes-underground-adversarial-prompt-injection) | <nobr>内容確認・補足情報</nobr> |

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
| [TeamCityの重大な脆弱性により、ログインせずにOSコマンドを実行される可能性](https://www.helpnetsecurity.com/2026/07/28/teamcity-rce-cve-2026-63077-fixed/) | 30.0 | 46.0 | 54.0 |
| [Coca-Cola傘下のFairlifeがデータ侵害を受けたことを公表](https://www.infosecurity-magazine.com/news/coca-cola-subsidiary-fairlife-data/) | 28.0 | 30.0 | 42.0 |
| [Coca-Cola、Fairlifeへのランサムウェア攻撃でデータ窃取を確認](https://www.helpnetsecurity.com/2026/07/28/coca-cola-fairlife-dairy-subsidiary-ransomware-attack/) | 28.0 | 30.0 | 42.0 |
| [Microsoft Active Directory Certificates の「Certighost」脆弱性](https://www.darkreading.com/vulnerabilities-threats/certighost-flaw-microsoft-active-directory-certificates) | 28.0 | 20.0 | 42.0 |
| [Tengu Botnetがプロセスを終了されると侵害済みLinuxデバイスを再起動する](https://thehackernews.com/2026/07/tengu-botnet-reboots-compromised-linux.html) | 28.0 | 20.0 | 42.0 |
| [現代の詐欺に対応するためにMalwarebytes Mobile Securityを再構築](https://www.malwarebytes.com/blog/product/2026/07/we-rebuilt-malwarebytes-mobile-security-for-the-scams-of-today) | 28.0 | 20.0 | 42.0 |
| [Googleが新たな脅威アクター命名体系を採用](https://www.securityweek.com/google-adopts-new-threat-actor-naming-system/) | 28.0 | 20.0 | 42.0 |
| [Mirage Kittenが中東・アフリカ地域を新たなマルウェアで標的に](https://securelist.com/mirage-kitten-new-tools/120811/) | 28.0 | 20.0 | 42.0 |
| [AI支援のバグハントでLinux Kernelのnet/schedに0-dayを発見](https://www.infosecurity-magazine.com/news/ai-linux-kernel-zero-day-net-sched/) | 27.0 | 20.0 | 43.0 |
| [JFrog、OpenAIモデルがHugging Face侵害前にArtifactoryのゼロデイを悪用したことを確認](https://thehackernews.com/2026/07/jfrog-confirms-openai-models-exploited.html) | 27.0 | 20.0 | 43.0 |
| [Anthropic「一律禁止は提唱していない」 オープンウェイト支持書簡への不参加を説明](https://www.itmedia.co.jp/news/article/2607/28/2000000231/) | 26.0 | 20.0 | 42.0 |
| [Claude AIがポスト量子テストスキームを解析し、7ラウンドAESのより高速な攻撃法を発見](https://thehackernews.com/2026/07/claude-ai-just-cracked-post-quantum.html) | 25.0 | 20.0 | 42.0 |
| [公開されたMCPサーバーの背後に潜むリスク](https://www.wiz.io/blog/the-risk-hiding-behind-exposed-mcp-servers) | 25.0 | 20.0 | 42.0 |
| [Hugging Faceの侵害で再燃するオープンウェイト論争と責任問題](https://www.helpnetsecurity.com/2026/07/28/hugging-face-breach-ciso-playbook-open-weight-llms/) | 25.0 | 20.0 | 42.0 |
| [AIで見つかった脆弱性は、話題ほど悪用しやすくなっていない](https://www.theregister.com/security/2026/07/28/ai-found-bugs-arent-proving-any-easier-to-exploit-despite-the-hype/5279637) | 25.0 | 20.0 | 42.0 |
| [AI支援セキュリティツールでバグ発見は増加も、脅威レベルは変わらず](https://cyberscoop.com/ai-assisted-security-tools-are-finding-more-bugs-but-the-threat-level-has-not-changed/) | 25.0 | 20.0 | 42.0 |
| [パートナーがネットワークを防御しAIへの不安を和らげる方法](https://www.akamai.com/blog/partners/2026/jul/partners-defend-network-ease-ai-anxiety) | 25.0 | 20.0 | 42.0 |
| [企業は一般的なサイバー脅威よりもAIリスクを懸念している](https://www.cybersecuritydive.com/news/ai-cybersecurity-threats-business-fears/826352/) | 25.0 | 20.0 | 42.0 |
| [Prescient Security、Caitにアタックサーフェスマネジメントを追加し、AI支援ペンテストを拡充](https://www.helpnetsecurity.com/2026/07/28/prescient-security-cait/) | 25.0 | 20.0 | 42.0 |
| [OTセキュリティスタートアップFrenosが152万ドルを調達](https://www.securityweek.com/ot-security-startup-frenos-raises-1-52-million/) | 25.0 | 20.0 | 42.0 |
| [Intel 471、AIエージェントとMCP対応でVerity471を拡張し脅威インテリジェンスを強化](https://www.helpnetsecurity.com/2026/07/28/intel-471-expands-verity471-with-ai-agent-and-mcp-support-for-threat-intelligence/) | 25.0 | 20.0 | 42.0 |
| [SpecterOpsがAWSの攻撃経路管理とAIをハイブリッドIDセキュリティに導入](https://www.helpnetsecurity.com/2026/07/28/specterops-bloodhound-hunter/) | 25.0 | 20.0 | 42.0 |
| [Microsoft、AI活用脅威に対抗するため一連のAIセキュリティ施策を発表](https://www.infosecurity-magazine.com/news/microsoft-ai-security-initiatives/) | 25.0 | 20.0 | 42.0 |
| [Team Cymru、AI搭載の脅威インテリジェンスとインシデント対応向け「Pure Signal Command」を発表](https://www.helpnetsecurity.com/2026/07/28/team-cymru-pure-signal-command/) | 25.0 | 20.0 | 42.0 |
| [共有されたClaudeのチャットがGoogle検索で見つかる状態にあった問題](https://www.malwarebytes.com/blog/privacy/2026/07/shared-claude-chats-were-searchable-on-google) | 25.0 | 20.0 | 42.0 |
| [Microsoftが初のサイバーセキュリティAIモデル「MAI-Cyber-1-Flash」を発表](https://www.securityweek.com/microsoft-unveils-mai-cyber-1-flash-its-first-cybersecurity-ai-model/) | 25.0 | 20.0 | 42.0 |
| [VERITASプロジェクトがAIのセキュリティ確保の方法を変える可能性](https://www.helpnetsecurity.com/2026/07/28/veritas-ai-scientific-research-infrastructure-security/) | 25.0 | 20.0 | 42.0 |
| [Hush Security、AIエージェントガバナンスで3,000万ドルを調達](https://www.securityweek.com/hush-security-raises-30-million-for-ai-agent-governance/) | 25.0 | 20.0 | 42.0 |
| [Microsoftが最新の自社開発モデルを発表、セキュリティ向け低価格AIを提供し「主要モデルの半額で世界水準の性能」を実現](https://www.itpro.com/security/it-delivers-world-class-performance-at-50-percent-of-the-cost-of-leading-models-microsoft-unveils-cut-price-ai-for-security-with-latest-in-house-model-launch) | 25.0 | 20.0 | 42.0 |
| [CRESTの新しいAI標準、AI活用ペンテスト認定を実現](https://www.infosecurity-magazine.com/news/crest-ai-pentesting-accreditation/) | 25.0 | 20.0 | 42.0 |
| [研究者が、AIの助けでLinuxのトラフィック制御の競合状態をroot権限取得エクスプロイトに発展させたと報告](https://thehackernews.com/2026/07/researcher-says-ai-helped-develop-linux.html) | 25.0 | 20.0 | 42.0 |
| [OpenWrtの重大なDHCPv6脆弱性、未認証の攻撃者によるroot権限でのコード実行を許す可能性](https://thehackernews.com/2026/07/critical-openwrt-dhcpv6-flaw-could-let.html) | 24.0 | 46.0 | 50.0 |
| [vBulletinで公開済みエクスプロイトを伴う認証前RCEの重大な脆弱性を修正](https://www.bleepingcomputer.com/news/security/vbulletin-fixes-critical-pre-auth-rce-flaw-with-public-exploit/) | 24.0 | 38.0 | 42.0 |
| [VeloCloud Orchestrator（VCO）オンプレミス版の脆弱性によりリモートコード実行が可能になる可能性](https://www.cisecurity.org/advisory/a-vulnerability-in-velocloud-orchestrator-vco-on-prem-could-allow-for-remote-code-execution_2026-072) | 24.0 | 38.0 | 42.0 |
| [Joyfillのnpmベータ版2件が侵害されDEV#POPPERリモートアクセス型トロイの木馬を配布](https://socket.dev/blog/joyfill-npm-beta-releases-compromised) | 22.0 | 30.0 | 42.0 |
| [製品サイトが侵害、サーバ内に個人情報も - ナカバヤシ](https://www.security-next.com/187949) | 22.0 | 20.0 | 42.0 |
| [メール本文に講座受講者メアドを誤記載 - 茨城県立こころの医療センター](https://www.security-next.com/187664) | 22.0 | 20.0 | 42.0 |
| [通販サイトにサイバー攻撃、個人情報流出の可能性 - ANAグループ会社](https://www.security-next.com/187942) | 22.0 | 20.0 | 42.0 |
| [Facebookで他人のコンテンツを盗んだ上で「昔の投稿を編集してアップロード」することで権利を奪う詐欺が横行している](https://gigazine.net/news/20260728-facebook-copyright/) | 22.0 | 20.0 | 42.0 |
| [IR動向Q2 2026：フィッシングと武器化されたリモート管理ツールが攻撃チェーンを牽引](https://blog.talosintelligence.com/ir-trends-q2-2026/) | 22.0 | 20.0 | 42.0 |
| [高校で生徒証明写真データ含む光ディスクを紛失 - 大阪府](https://www.security-next.com/187867) | 22.0 | 20.0 | 42.0 |
| [熊本で非常時Wi-Fi「00000JAPAN」発動中 KDDIが無料開放、他社ユーザーも利用可](https://www.itmedia.co.jp/news/article/2607/28/2000000246/) | 21.0 | 20.0 | 42.0 |
| [マイクロソフト、エージェント型セキュリティシステム「Project Perception」を発表](https://japan.zdnet.com/article/35251024/) | 21.0 | 20.0 | 42.0 |
| [npmとGitHub Actionsに対するサプライチェーン攻撃の妨害](https://github.blog/security/supply-chain-security/disrupting-supply-chain-attacks-on-npm-and-github-actions/) | 20.0 | 45.0 | 42.0 |
| [MikroTik RouterOSとCloud Hosted Routerの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-209-05) | 20.0 | 28.0 | 50.0 |
| [ABB KNX Update Toolの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-209-07) | 20.0 | 28.0 | 50.0 |
| [igloohome Smart Lockのモバイルアプリケーション](https://www.cisa.gov/news-events/ics-advisories/icsa-26-209-06) | 20.0 | 28.0 | 50.0 |
| [iPhone、iPad、Macを更新してAppleのセキュリティ上の脆弱性を修正してください](https://www.malwarebytes.com/blog/news/2026/07/july-apple-updates-are-especially-important-if-you-receive-images) | 20.0 | 28.0 | 50.0 |
| [AiTMフィッシングへの耐性強化：SOCリーダーが知っておくべきこと](https://any.run/cybersecurity-blog/enterprise-phishing-resilience/) | 20.0 | 20.0 | 48.0 |
| [ミネソタ州30以上の自治体で水道事業を妨害した協調的サイバー攻撃](https://statescoop.com/coordinated-cyberattack-disrupts-water-utilities-in-30-minnesota-communities/) | 20.0 | 20.0 | 42.0 |
| [CISA、サイバー攻撃時に重要システムを隔離するための助言を共有](https://www.bleepingcomputer.com/news/security/cisa-shares-advice-on-isolating-vital-systems-during-cyberattacks/) | 20.0 | 20.0 | 42.0 |
| [Adobe製品に存在する複数の脆弱性により任意コード実行が可能となる可能性](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-adobe-products-could-allow-for-arbitrary-code-execution_2026-073) | 20.0 | 20.0 | 42.0 |
| [FBI、AnthropicのMythosを法執行上の課題と認識](https://fedscoop.com/fbi-anthropic-mythos-law-enforcement-challenge/) | 20.0 | 20.0 | 42.0 |
| [DEF CONがMeta風の「覗き見グラス」を禁止](https://www.theregister.com/security/2026/07/28/def-con-bans-meta-style-pervert-glasses/5279763) | 20.0 | 20.0 | 42.0 |
| [Hugging Face Diffusersのバグによりカスタムコード保護が回避される問題](https://www.infosecurity-magazine.com/news/hugging-face-diffusers-trust/) | 20.0 | 20.0 | 42.0 |
| [Cyera、Oasis Securityを10億ドルで買収](https://www.securityweek.com/cyera-acquiring-oasis-security-in-1-billion-deal/) | 20.0 | 20.0 | 42.0 |
| [Bank of Barodaがサイバーインシデントを確認、ハッカーによるデータ窃取主張を受けて](https://therecord.media/india-bank-of-baroda-reports-cybersecurity-incident) | 20.0 | 20.0 | 42.0 |
| [24,650台のインターネット公開BMCがログイン前にIPMIパスワードハッシュを漏えい](https://thehackernews.com/2026/07/24650-internet-exposed-bmcs-disclose.html) | 20.0 | 20.0 | 42.0 |
| [Apple、iOSで87件、macOS Tahoeで155件の脆弱性を修正](https://www.securityweek.com/apple-patches-87-vulnerabilities-in-ios-155-in-macos-tahoe/) | 20.0 | 20.0 | 42.0 |
| [あなたのSSOは最新の認証情報攻撃から守られていますか](https://www.bleepingcomputer.com/news/security/is-your-sso-protected-against-modern-credential-attacks/) | 20.0 | 20.0 | 42.0 |
| [セキュリティ懸念でCharity bankがオンラインサービスを停止](https://www.theregister.com/security/2026/07/28/charity-bank-pulls-online-services-over-security-fears/5279615) | 20.0 | 20.0 | 42.0 |
| [慈善団体向け銀行がセキュリティ懸念でオンラインサービスを停止](https://www.theregister.com/security/2026/07/28/bank-for-charities-pulls-online-services-over-security-fears/5279615) | 20.0 | 20.0 | 42.0 |
| [BlackCloak、経営層の信頼する周辺人物までディープフェイク対策を拡大](https://www.helpnetsecurity.com/2026/07/28/blackcloak-deepfake-protection/) | 20.0 | 20.0 | 42.0 |
| [Bugcrowd、エージェント型ペネトレーションテスト向けのSavant Pathseekerを発表](https://www.helpnetsecurity.com/2026/07/28/bugcrowd-introduces-savant-pathseeker-for-agentic-penetration-testing-with-exploit-validation/) | 20.0 | 20.0 | 42.0 |
| [Rapid7 Cyber GRCが利用可能に：セキュリティ対応をコンプライアンス証跡へ تبدیل](https://www.rapid7.com/blog/post/pt-cyber-grc-available-prove-compliance-security) | 20.0 | 20.0 | 42.0 |
| [フィッシングがサイバー攻撃の初期侵入手段の主流に、攻撃者は回避技術を高度化](https://www.infosecurity-magazine.com/news/phishing-dominates-initial-entry/) | 20.0 | 20.0 | 42.0 |
| [米国は6Gの主導権とセキュリティ確保に向けて人材を求めている、さもないと北京に先を越される](https://www.theregister.com/networks/2026/07/28/uncle-sam-needs-you-to-fight-for-6g-leadership-and-security-lest-beijing-get-there-first/5279525) | 20.0 | 20.0 | 42.0 |
| [元Citigroup CISOのBlauner氏が語る、優れたセキュリティリーダーの条件](https://www.darkreading.com/cybersecurity-operations/former-citigroup-ciso-blauner-great-security-leader) | 20.0 | 20.0 | 42.0 |
| [2万4000件超の公開サーバーBMCで数十年前の脆弱性によりパスワードハッシュが漏えい](https://www.bleepingcomputer.com/news/security/over-24-000-exposed-server-bmcs-leak-password-hash-via-decades-old-flaw/) | 20.0 | 20.0 | 42.0 |
| [認証前にパスワードハッシュを漏えいする露出したBMCの脆弱性](https://www.helpnetsecurity.com/2026/07/28/exposed-bmc-ipmi-vulnerability-research/) | 20.0 | 20.0 | 42.0 |
| [CI Fortifyの重要システム分離に関する注意事項](https://www.cisa.gov/resources-tools/resources/ci-fortify-advice-isolating-vital-systems) | 20.0 | 20.0 | 42.0 |
| [サイバー攻撃発生時に組織の復旧を支援する方法](https://www.ncsc.gov.uk/blogs/when-cyber-attacks-happen-helping-organisations-recover) | 20.0 | 20.0 | 42.0 |
| [CISAが豪州などと連携し、重要インフラの運用技術と支援システムを分離するためのガイダンスを公表](https://www.cisa.gov/news-events/news/cisa-joins-australia-and-others-publish-guidance-isolate-operational-technology-and-enabling-systems) | 20.0 | 20.0 | 42.0 |
| [VaticanのClick To Prayアプリで70万人の個人情報が漏えい](https://www.malwarebytes.com/blog/privacy/2026/07/vaticans-click-to-pray-app-exposed-personal-data-from-700000-users) | 20.0 | 20.0 | 42.0 |
| [WizによるCISA BOD 26-04の脆弱性対応とトリアージ活動の迅速化](https://www.wiz.io/blog/cisa-bod-26-04-alignment-with-wiz) | 20.0 | 20.0 | 42.0 |
| [Act Security、ステルス状態から登場しパッチ問題に対処](https://www.securityweek.com/act-security-emerges-from-stealth-to-fight-the-patch-problem/) | 20.0 | 20.0 | 42.0 |
| [Hacker Conversations: Tal KollanderのBlack HatからHack Blockerへの歩み](https://www.securityweek.com/hacker-conversations-tal-kollanders-journey-from-black-hat-to-hack-blocker/) | 20.0 | 20.0 | 42.0 |
| [エレコムの法人向けWi-Fiアクセスポイントおよび家庭向けWi-Fiルーター7製品に脆弱性、最新版ファームウェアへの更新を 法人向け「WAB-M1775-PS」、家庭向け「WRC-X3000GS3-B」などが対象](https://internet.watch.impress.co.jp/docs/news/2128662.html) | 20.0 | 20.0 | 42.0 |
| [AWS、2027年1月1日にShield AdvancedのL7自動緩和機能を終了へ](https://www.helpnetsecurity.com/2026/07/28/aws-waf-anti-ddos-rule-group/) | 20.0 | 20.0 | 42.0 |
| [医療請求会社MCBSでデータ漏えい、126万人に影響](https://www.bleepingcomputer.com/news/security/data-breach-at-medical-billing-firm-mcbs-affects-126-million-people/) | 20.0 | 20.0 | 42.0 |

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
