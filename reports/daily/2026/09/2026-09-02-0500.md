# 📡 サイレーダー 2026-09-02 05:00 JST

このレポートは、2026-09-01 17:00 JST〜2026-09-02 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 86
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 57

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Critical JFrog Artifactory Vulnerability Reportedly Exploited in the Wild](#topic-30390) | 55.0 | 64.0 | 55.0 | 音声 | 温度感上位枠 |
| 2 | [Financially Motivated Threat Actor BREEZE COMET Targets Brazil](#topic-30406) | 35.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [Critical Langflow flaw exploited to steal OpenAI and AWS keys](#topic-30389) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Fake Claude Opus 5 app delivers malware and wipes its own tracks](#topic-30422) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Russia-Aligned UAC-0099 Plants Nuclear Weapon Prompt in Malware to Disrupt AI Analysis](#topic-30461) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-30390"></a>

### 1. Critical JFrog Artifactory Vulnerability Reportedly Exploited in the Wild

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 55.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

JFrog Artifactoryの重大な脆弱性CVE-2026-82329について、公開から数日で実際の悪用が始まったと報じられています。
内容は認証バイパスに関するもので、条件次第では管理者権限の取得につながる可能性があるとされています。
Artifactoryはソフトウェア供給網や開発運用の基盤として使われることがあり、ここが侵害されると影響範囲が広がるおそれがあります。
公開直後の悪用報告があるため、対応の遅れが被害拡大につながりやすい点が注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当バージョンの利用有無を確認し、ベンダー案内に沿って速やかに修正を適用する。
- Artifactoryの管理者アカウント、APIトークン、認証関連の設定やログを点検し、不審な権限付与や操作がないか確認する。
- 外部公開している場合はアクセス制御を見直し、必要に応じて一時的な到達範囲の制限や監視強化を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-82329 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | watchTowr | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-82329](https://nvd.nist.gov/vuln/detail/CVE-2026-82329) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit Critical JFrog Artifactory Flaw to Mint Admin Tokens Days Afte](https://thehackernews.com/2026/09/attackers-exploit-critical-jfrog.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical JFrog Artifactory Vulnerability Reportedly Exploited in the Wild](https://www.securityweek.com/critical-jfrog-artifactory-vulnerability-reportedly-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-30406"></a>

### 2. Financially Motivated Threat Actor BREEZE COMET Targets Brazil

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>A⁠I</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Google Threat Intelligence Groupは、ブラジルの金融・小売・eCommerce組織を狙う金銭目的の脅威グループ「BREEZE COMET」を報告しました。
攻撃は銀行ソフトウェアや決済システムへの不正アクセスを通じた不正送金が目的とされ、初期侵入から横展開、権限昇格、痕跡削除まで多段階で行われたとされています。
金融機関や関連事業者の基幹システム、認証情報、クラウド環境が直接狙われており、単なる端末感染よりも業務影響が大きくなりやすい点が注目されます。
さらに、正規サイトやRMMツールの悪用、生成AIの活用が示唆されており、攻撃の効率化と拡大が懸念されます。

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

- 不審なRMM利用、未承認のリモート接続、PowerShellの不自然な実行を監視し、端末側のログとアラートを有効化する。
- AD、クラウド、CI/CD、Secrets管理を含む認証情報の保護を強化し、ハードコードされた鍵や過剰権限を点検する。
- 外向き通信や内部のRDP/SMBを必要最小限に制限し、正規に見える外部サイト経由の配布にも注意する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Mandiant | 言及あり | 0.80 | — |
| ベンダー | Trend Micro | 言及あり | 0.80 | — |
| ベンダー | HashiCorp | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Meta | 言及あり | 0.80 | — |
| 製品 | Active Directory | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |
| 製品 | HashiCorp Vault | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| マルウェア | XWorm | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Financially Motivated Threat Actor BREEZE COMET Targets Brazil](https://cloud.google.com/blog/topics/threat-intelligence/financially-motivated-threat-actor-breeze-comet-targets-brazil/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-30389"></a>

### 3. Critical Langflow flaw exploited to steal OpenAI and AWS keys

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>A⁠I</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Langflowに存在するとされる未認証のリモートコード実行脆弱性（CVE-2026-0768）が悪用され、認証情報やトークン、各種キーの窃取につながっていると報じられています。
対象にはOpenAIやAWS関連の鍵が含まれるとされ、AIアプリ基盤の脆弱性が広範な情報流出リスクに直結する点が懸念されています。
AI開発・運用環境で使われる基盤ソフトの脆弱性は、モデルそのものだけでなく周辺のクラウド資格情報まで波及し得ます。
特に未認証RCEが関与する場合、影響範囲が大きくなりやすいため早急な確認が重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Langflowの利用有無とバージョンを確認し、該当する場合は修正版への更新やベンダー案内の確認を進める。
- OpenAIやAWSを含むAPIキー、トークン、シークレットの棚卸しを行い、露出の可能性があるものはローテーションを検討する。
- AIアプリ基盤への不審なアクセスや実行痕跡、資格情報の不自然な利用を重点的に監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| 製品 | Langflow | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | OpenAI | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Critical Langflow flaw exploited to steal OpenAI and AWS keys](https://www.bleepingcomputer.com/news/security/critical-langflow-flaw-exploited-to-steal-openai-and-aws-keys/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-30422"></a>

### 4. Fake Claude Opus 5 app delivers malware and wipes its own tracks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

AnthropicやClaudeを装ったGitHubリポジトリが、無料利用をうたって利用者を誘導し、Windows向けの情報窃取型マルウェアを配布していたと報告されています。
表向きのAI関連コンテンツを入口にしたソーシャルエンジニアリングが使われており、感染後は痕跡を消すような挙動も指摘されています。
生成AIの人気や話題性を悪用して、正規サービス風の見た目で利用者をだます手口として注目されています。
資格情報や暗号資産ウォレットなど、被害が直接的な情報窃取につながる点も重要です。

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

- AIサービス名やブランドをかたる配布物・リポジトリは、正規性の確認を徹底する。
- Windows端末での不審な情報窃取系マルウェア対策として、EDRや多要素認証の有効化を見直す。
- 暗号資産ウォレットや重要資格情報の保管・利用端末を分離し、侵害時の影響を抑える。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Anthropic | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | Claude | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Fake Claude Opus 5 app delivers malware and wipes its own tracks](https://www.helpnetsecurity.com/2026/09/01/revstealer-malware-claude-opus-5-github/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-30461"></a>

### 5. Russia-Aligned UAC-0099 Plants Nuclear Weapon Prompt in Malware to Disrupt AI Analysis

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者は、AI支援の解析を妨げる目的で、マルウェア内にLLMの安全機構を誘発しやすい文言を仕込む新しい手法が使われたと報告しました。
報道によれば、この手法は「GuardBreaker」と呼ばれ、ロシア寄りとされる脅威グループUAC-0099に関連づけられています。
対象はウクライナの1件とされていますが、公開情報ベースでは詳細な影響範囲までは確認できません。攻撃者が防御側のAI分析を意図的に攪乱しようとしている点が注目されます。
マルウェア解析やトリアージでLLMを活用する運用では、出力の信頼性や検知ワークフローへの影響を再点検する必要があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI支援分析を使う場合、LLMの回答を単独で判断材料にせず、静的解析やサンドボックス結果と突き合わせる。
- 不自然な文言や誘導的テキストを含むサンプルを扱う際は、プロンプト汚染の可能性を前提に運用手順を見直す。
- 解析支援AIの利用ログや失敗パターンを確認し、誤検知・解析停止が起きた場合の手動フォールバックを用意する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | ESET | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Russia-Aligned UAC-0099 Plants Nuclear Weapon Prompt in Malware to Disrupt AI An](https://thehackernews.com/2026/09/russia-aligned-uac-0099-plants-nuclear.html) | <nobr>内容確認・補足情報</nobr> |

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
| [CISAレビューが脆弱性クラスの排除を提言](https://www.helpnetsecurity.com/2026/09/01/cisa-on-eliminating-recurring-security-weaknesses/) | 31.0 | 23.0 | 43.0 |
| [イランのサイバースパイ、航空・フィンテックの開発者を新たなマルウェアで標的に](https://therecord.media/iranian-cyber-spies-target-aviation-fintech-new-malware) | 28.0 | 45.0 | 42.0 |
| [RansomwareギャングがNutex Healthのデータ侵害を主張](https://www.securityweek.com/ransomware-gang-claims-nutex-health-data-breach/) | 28.0 | 30.0 | 42.0 |
| [Breeze Cometがブラジルの決済システムを悪用し数百件の不正取引を実行](https://thehackernews.com/2026/09/breeze-comet-executes-hundreds-of.html) | 28.0 | 20.0 | 42.0 |
| [VishingキャンペーンがMicrosoft Teamsを悪用し、攻撃者に社内ネットワークへの足がかりを与える](https://www.helpnetsecurity.com/2026/09/01/spring-ring-vishing-campaign-microsoft-teams/) | 28.0 | 20.0 | 42.0 |
| [ClickFixキャンペーン、Polygonブロックチェーンを悪用して31組織を侵害](https://www.darkreading.com/endpoint-security/clickfix-campaign-comprises-31-orgs-abuses-polygon-blockchain) | 28.0 | 20.0 | 42.0 |
| [イラン系ハッカーが採用担当者を装い、コーディングテストを通じてクロスプラットフォームRATを配布](https://thehackernews.com/2026/09/iranian-hackers-pose-as-recruiters-to.html) | 28.0 | 20.0 | 42.0 |
| [TerminalFixはClickFixに似ているが、異なるペイロードを配信する](https://www.malwarebytes.com/blog/news/2026/09/terminalfix-looks-like-clickfix-but-delivers-a-very-different-payload) | 28.0 | 20.0 | 42.0 |
| [脅威アクターはより高度な攻撃ではなく再現可能な攻撃を求めている](https://thehackernews.com/2026/09/threat-actors-dont-want-better-attacks.html) | 28.0 | 20.0 | 42.0 |
| [米国裁判所で5人のベネズエラ人がATMジャックポッティングで有罪を認める](https://www.securityweek.com/five-venezuelans-plead-guilty-in-us-court-to-atm-jackpotting/) | 28.0 | 20.0 | 42.0 |
| [米国でのATMジャックポット攻撃でベネズエラ人5人が有罪を認める](https://www.bleepingcomputer.com/news/security/five-venezuelans-plead-guilty-to-atm-jackpotting-attacks-in-us/) | 28.0 | 20.0 | 42.0 |
| [使い込むほど成長するAIエージェント「Hermes Agent」でタスクを自動実行させてみた、PCを放置していても時間になれば勝手に実行](https://gigazine.net/news/20260901-hermes-agent-cron-automation/) | 27.0 | 20.0 | 42.0 |
| [視聴者参加型の“終わらないAI番組”も可能に？ 実時間以下で動画を生成できる「Mini Max H3 Max」登場](https://www.itmedia.co.jp/news/article/2609/01/2000001045/) | 26.0 | 20.0 | 42.0 |
| [Anthropic、モデルの制御維持に向けて一層の努力を約束し、提携先にも協力を要請](https://www.theregister.com/ai-and-ml/2026/09/01/anthropic-pledges-to-try-harder-to-keep-models-under-control-asks-partners-to-chip-in/5293733) | 25.0 | 20.0 | 42.0 |
| [Sevii、AI加速攻撃に先回りする自律防御を展開](https://www.securityweek.com/sevii-targets-ai-speed-attacks-with-preemptive-autonomous-defense/) | 25.0 | 20.0 | 42.0 |
| [Frontier AIを用いて主要な産業用デバイスの脆弱性を悪用する支援に活用](https://www.cybersecuritydive.com/news/frontier-ai-exploit-flaws-water-PLCs-industrial-devices/829307/) | 25.0 | 20.0 | 42.0 |
| [Anthropic、最近のサイバーインシデント後にモデルテストを再開──セキュリティ強化へ新ルール導入](https://www.itpro.com/security/anthropic-resumes-model-testing-after-recent-cyber-incidents-but-its-introduced-new-rules-to-improve-security) | 25.0 | 20.0 | 42.0 |
| [攻撃者がMETR APIキーを窃取し、60万ドル相当のAIクレジットを消費](https://www.infosecurity-magazine.com/news/attackers-steal-metr-api-key/) | 25.0 | 20.0 | 42.0 |
| [エンタープライズの65%がAIエージェントの想定外の動作を確認](https://www.infosecurity-magazine.com/news/65-percent-enterprises-ai-agents/) | 25.0 | 20.0 | 42.0 |
| [AIでPLCエクスプロイトを移植する実験：数時間と数百ドルを要した](https://www.securityweek.com/experiment-porting-a-plc-exploit-with-ai-takes-hours-and-hundreds-of-dollars/) | 25.0 | 20.0 | 42.0 |
| [フロンティアAIによるサイバーリスクは世界の金融システムにとって「最も差し迫った懸念」、監督機関が警告](https://therecord.media/cyber-risk-from-frontier-ai-most-immediate-concern-to-global-finance) | 25.0 | 20.0 | 42.0 |
| [Siemensのアドバイザリを受けて警告されるAI搭載PLC攻撃](https://www.itpro.com/security/cyber-attacks/security-researchers-warn-of-ai-powered-plc-attacks-in-wake-of-siemens-advisories) | 25.0 | 20.0 | 42.0 |
| [Continuous Vulnerability Assessmentの紹介：AI脅威時代のリアルタイム防御](https://www.wiz.io/blog/introducing-cva) | 25.0 | 20.0 | 42.0 |
| [InfostealerがClaudeアカウントを乗っ取り、利用者に費用を発生させる問題](https://www.malwarebytes.com/blog/news/2026/09/infostealers-are-hijacking-claude-accounts-at-users-expense) | 25.0 | 20.0 | 42.0 |
| [The Collective Cyber Defenseが示す次のベンダー質問票の在り方](https://cyberscoop.com/collective-cyber-defense-letter-vendor-questionnaire-op-ed/) | 25.0 | 20.0 | 42.0 |
| [Financial Stability Boardが警鐘を鳴らすフロンティアAIのリスク](https://www.infosecurity-magazine.com/news/financial-stability-board-alarm/) | 25.0 | 20.0 | 42.0 |
| [Attackers Steal METR API Key and Consume AI Credits Worth About $600,000](https://thehackernews.com/2026/09/attackers-steal-metr-api-key-and.html) | 25.0 | 20.0 | 42.0 |
| [ハッカーがLangflowの重大な脆弱性の悪用を開始](https://www.securityweek.com/hackers-start-exploiting-critical-langflow-vulnerability/) | 24.0 | 46.0 | 50.0 |
| [Rockwell Automation Historian MEの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-244-06) | 24.0 | 46.0 | 50.0 |
| [約2万2000台のMicrosoft Exchangeサーバーが乗っ取り攻撃の脆弱性を抱える](https://www.bleepingcomputer.com/news/security/nearly-22-000-microsoft-exchange-servers-vulnerable-to-hijack-attacks/) | 24.0 | 38.0 | 42.0 |
| [WatchGuard製品の重大な脆弱性修正](https://www.securityweek.com/watchguard-patches-critical-vulnerabilities/) | 24.0 | 38.0 | 42.0 |
| [Rockwell Automation FactoryTalk Activation Managerの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-244-04) | 22.0 | 40.0 | 50.0 |
| [Microsoft Teams通知がSocketで利用可能に](https://socket.dev/blog/microsoft-teams) | 22.0 | 20.0 | 42.0 |
| [複数顧客にフィッシングメール、注文情報が流出か - 酒類販売事業者](https://www.security-next.com/189260) | 22.0 | 20.0 | 42.0 |
| [再委託先でメール誤送信、講座受講予定者のメアド流出 - 新潟県](https://www.security-next.com/189535) | 22.0 | 20.0 | 42.0 |
| [「ホロライブ」トレカゲームサイトに侵害痕跡 - 脆弱性公表受け調査で判明](https://www.security-next.com/189471) | 22.0 | 20.0 | 42.0 |
| [Anthropicが「開発中のAIで外部を攻撃しないための対策」を発表](https://gigazine.net/news/20260901-anthropic-alignment-security/) | 22.0 | 20.0 | 42.0 |
| [「Google Cloud Build」にRCE脆弱性 - 6月に修正済み](https://www.security-next.com/189666) | 22.0 | 20.0 | 42.0 |
| [Rockwell Automation Redundancy Module Configuration Toolの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-244-02) | 20.0 | 28.0 | 50.0 |
| [Rockwell Automation RSLinx Classicに関する脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-244-01) | 20.0 | 28.0 | 50.0 |
| [Rockwell Automation ControlLogix、CompactLogix、CompactLogix 5480、GuardLogix、Compact GuardLogixに関する脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-244-05) | 20.0 | 28.0 | 50.0 |
| [Rockwell Automation Logix Platformの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-244-03) | 20.0 | 28.0 | 50.0 |
| [Aesto Health、950万人超の患者に影響するデータ侵害を発表](https://www.bleepingcomputer.com/news/security/aesto-health-says-data-breach-affects-over-95-million-patients/) | 20.0 | 20.0 | 42.0 |
| [沿岸警備隊が海上サイバーセキュリティ政策室を設置](https://www.securityweek.com/coast-guard-establishes-office-of-maritime-cybersecurity-policy/) | 20.0 | 20.0 | 42.0 |
| [偽のGTA 6流出コピーが暗号資産ウォレットを吸い取る](https://www.malwarebytes.com/blog/scams/2026/09/fake-gta-6-leaked-copy-drains-your-crypto-wallet) | 20.0 | 20.0 | 42.0 |
| [ハイブリッドクラウド時代に追いつけないセキュリティポリシー](https://www.cybersecuritydive.com/news/security-policies-fail-keep-up-hybrid-cloud/829256/) | 20.0 | 20.0 | 42.0 |
| [Healthcare facilities運営会社Nutex、8月のインシデントで患者・従業員データが窃取されたと発表](https://therecord.media/nutex-health-data-breach) | 20.0 | 20.0 | 42.0 |
| [BGPハイジャック攻撃で悪意あるVirtualizor更新を配布するハッカー](https://www.bleepingcomputer.com/news/security/hackers-push-malicious-virtualizor-update-in-bgp-hijacking-attack/) | 20.0 | 20.0 | 42.0 |
| [Novocureのデータ侵害で1,400人超のがん患者に影響](https://www.bleepingcomputer.com/news/security/novocure-data-breach-affects-more-than-1-400-cancer-patients/) | 20.0 | 20.0 | 42.0 |
| [未修正のiPhoneを狙って暗号資産ウォレットのシードを窃取する13件の悪意あるPackagistパッケージ](https://thehackernews.com/2026/09/13-malicious-packagist-packages-target.html) | 20.0 | 20.0 | 42.0 |
| [最善のEdgeセキュリティでも高リスクセッションを見逃す理由](https://www.bleepingcomputer.com/news/security/why-even-the-best-edge-security-still-misses-high-risk-sessions/) | 20.0 | 20.0 | 42.0 |
| [内部告発者が、USPSが郵送投票を管理する新しい未検証のITシステムを導入していると指摘](https://cyberscoop.com/usps-whistleblower-ballot-system-2026-midterms/) | 20.0 | 20.0 | 42.0 |
| [ホワイトハウス、テキサス州で水インフラ保護の試験プログラムを開始](https://www.infosecurity-magazine.com/news/white-house-texas-protect-water/) | 20.0 | 20.0 | 42.0 |
| [Softaculous通信への33時間にわたるBGPハイジャックでセキュリティ対応が混乱](https://www.theregister.com/security/2026/09/01/33-hour-bgp-hijack-of-softaculous-traffic-prompts-security-scramble/5293608) | 20.0 | 20.0 | 42.0 |
| [Aesto Healthのデータ侵害で950万人に影響](https://www.securityweek.com/9-5-million-impacted-by-aesto-health-data-breach/) | 20.0 | 20.0 | 42.0 |
| [ベルリン、ネットワーク侵害後の脅迫に屈せず](https://www.helpnetsecurity.com/2026/09/01/berlin-data-breach-rhysida-ransomware/) | 20.0 | 20.0 | 42.0 |
| [医療大手McKesson、データ侵害インシデントを調査](https://www.infosecurity-magazine.com/news/healthcare-mckesson-investigates/) | 20.0 | 20.0 | 42.0 |

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
