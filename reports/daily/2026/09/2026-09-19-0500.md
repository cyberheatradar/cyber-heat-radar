# 📡 サイレーダー 2026-09-19 05:00 JST

このレポートは、2026-09-18 17:00 JST〜2026-09-19 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 84
- [音声で扱う想定のトピック](#audio-topics): 4
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 56

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [ランサムウェア関連の法執行・司法措置](#topic-33448) | 36.0 | 45.0 | 42.0 | 音声 | AI×Security枠 |
| 2 | [Cisco Secure Firewall Adaptive Security Appliance, Secure Firewall Threat Defense, and Secure Firewall Management Center Software Hardening Release: September 2026](#topic-32969) | 34.0 | 64.0 | 51.0 | 音声 | 温度感上位枠 |
| 3 | [New Android malware uses AI to steal bank logins and PINs](#topic-33441) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 4 | [Claimed Bug Bounty Hunter Likely Used LLM to Build PhantomRaven npm Stealer](#topic-33497) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-33448"></a>

### 1. ランサムウェア関連の法執行・司法措置

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 45.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

ランサムウェアに関連する開発者への法執行・司法措置が話題になっています。
あわせて、脅威インテリジェンスやサプライチェーン攻撃、WordPressプラグインの不具合に関する別トピックも同じ文脈で取り上げられています。
ランサムウェア対策は技術的な防御だけでなく、攻撃者側の摘発や訴追も抑止要因として重要です。さらに、開発者環境や供給網が絡む攻撃は、被害範囲が広がりやすいため注目されます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ランサムウェア関連の司法・法執行動向を継続的に確認し、脅威グループの変化を把握する。
- 開発者環境やサプライチェーンに影響しうる不具合・侵害情報を、利用中のツールや依存関係の観点で点検する。
- WordPressなど広く使われる基盤については、関連する脆弱性情報と更新状況を早めに確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-15315 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-15316 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Mandiant | 言及あり | 0.80 | — |
| 製品 | WordPress | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [In Other News: Ransomware Developer Sentenced, Plugin4Shell AI Attack, Critical ](https://www.securityweek.com/in-other-news-ransomware-developer-sentenced-plugin4shell-ai-attack-critical-sap-flaw/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32969"></a>

### 2. Cisco Secure Firewall Adaptive Security Appliance, Secure Firewall Threat Defense, and Secure Firewall Management Center Software Hardening Release: September 2026

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 34.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

Ciscoは、Secure Firewall ASA、FTD、FMC向けのソフトウェア更新で、内部調査で見つかった複数の脆弱性に対処したと公表しました。
対象の一部には、すでに実際の悪用が確認されているものが含まれるとされています。
ファイアウォール製品や管理基盤は境界防御の要であり、影響を受けると広範囲に波及する可能性があります。現時点で回避策は案内されていないため、更新適用の優先度が高い話題です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象バージョンを確認し、Ciscoの更新版適用を早急に検討する。
- 管理系インターフェースや認証関連の異常なアクセス履歴がないか確認する。
- 同系列の複数CVEがまとまっているため、個別ではなく関連製品を横断して点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20329](https://nvd.nist.gov/vuln/detail/CVE-2026-20329) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Firewall Adaptive Security Appliance, Secure Firewall Threat Defens](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-hardening-asaftdfmc-uvpPROhN) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33441"></a>

### 3. New Android malware uses AI to steal bank logins and PINs

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠n⁠d⁠r⁠o⁠i⁠d</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>i⁠O⁠S</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

新たなAndroid向けマルウェア「RatHat」が、感染端末上を操作しながら銀行のログイン情報、認証コード、画面ロックのPINなどを窃取できるとされています。
AIを利用した挙動が報じられており、モバイル端末を狙う金融系の脅威として注意が必要です。銀行認証情報やPINは、アカウント乗っ取りや不正送金につながり得る重要な情報です。
端末操作と情報窃取を組み合わせた手口が示唆されているため、モバイル端末の防御と認証の見直しが注目されます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- モバイル端末上の不審なアプリや権限要求を点検し、インストール経路を制限する。
- 金融系アプリや重要アカウントでは、SMS依存を減らし多要素認証の運用を見直す。
- 端末紛失・乗っ取りを想定し、異常なログインや認証失敗の監視、利用者への注意喚起を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Apple iOS | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New Android malware uses AI to steal bank logins and PINs](https://www.malwarebytes.com/blog/news/2026/09/new-android-malware-uses-ai-to-steal-bank-logins-and-pins) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33497"></a>

### 4. Claimed Bug Bounty Hunter Likely Used LLM to Build PhantomRaven npm Stealer

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

npm パッケージレジストリを通じて、JavaScript ベースの情報窃取型マルウェア「PhantomRaven」が配布されたと報じられています。
関連する開発者が大規模言語モデル（LLM）を使ってマルウェアを作成した可能性が高いとされ、根拠として冗長なコメントやプレースホルダーコードなどが挙げられています。
npm のような開発者向けエコシステムは、依存関係を通じて被害が広がるため、サプライチェーン上のリスクとして注意が必要です。
AI を使った不審コードの生成が疑われる点は、脅威アクターの開発効率化や検知の難しさに関わるため注目されています。

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

- npm 由来の依存パッケージは、公開直後の不自然な挙動やメタデータの違和感を含めて継続監視する。
- JavaScript 系の情報窃取マルウェアは、ソースの見た目だけでなく実行時の通信や権限利用を含めて評価する。
- LLM 生成が疑われるコードでは、コメントや未使用断片の多さに加え、署名・レピュテーション・配布経路の確認を重視する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Claimed Bug Bounty Hunter Likely Used LLM to Build PhantomRaven npm Stealer](https://thehackernews.com/2026/09/claimed-bug-bounty-hunter-likely-used.html) | <nobr>内容確認・補足情報</nobr> |

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
| [CISAがCatalogに既知の悪用済み脆弱性2件を追加](https://www.cisa.gov/news-events/alerts/2026/09/18/cisa-adds-two-known-exploited-vulnerabilities-catalog) | 45.0 | 38.0 | 43.0 |
| [偽のChatGPT請求メールが職場・家庭の利用者を標的にする](https://www.itpro.com/security/phishing/fake-chatgpt-billing-email-targets-work-and-home-users) | 33.0 | 20.0 | 42.0 |
| [最近の攻撃で展開されたSettraランサムウェア亜種](https://www.cybersecuritydive.com/news/settra-ransomware-variant-recent-attacks/830787/) | 28.0 | 30.0 | 42.0 |
| [小売・製造業への攻撃で新たなSettraランサムウェア亜種を展開](https://www.infosecurity-magazine.com/news/settra-ransomware-retail/) | 28.0 | 30.0 | 42.0 |
| [TraderTraitorが暗号資産無関連の被害者に仕掛けたAPIバックドアを再び確認、こちらからの連絡は不要](https://www.sentinelone.com/labs/dont-call-us-well-call-your-apis-tradertraitor-backdoors-resurface-on-victim-with-no-crypto-ties/) | 28.0 | 20.0 | 42.0 |
| [Transparent TribeがプライベートGitHubリポジトリをC2に使う新たなRust製バックドアを展開](https://thehackernews.com/2026/09/transparent-tribe-deploys-new-rust.html) | 28.0 | 20.0 | 42.0 |
| [Fake LastPass AuthenticatorのGitHubリポジトリが新たなRapuncel情報窃取型マルウェアを配布](https://www.bleepingcomputer.com/news/security/fake-lastpass-authenticator-github-repos-push-new-rapuncel-infostealer/) | 28.0 | 20.0 | 42.0 |
| [WeaselBiscuit Stealer、13のnpmパッケージを通じて拡散しChrome拡張機能のストレージを窃取](https://thehackernews.com/2026/09/weaselbiscuit-stealer-spreads-via-13.html) | 28.0 | 20.0 | 42.0 |
| [Brevoのサプライチェーン攻撃、10万件のWebサイトにマルウェアを注入](https://www.securityweek.com/brevo-supply-chain-attack-injects-malware-into-100000-websites/) | 28.0 | 20.0 | 42.0 |
| [国連が「UN System Data Commons」を公開、約4400万件の統計データをAIから利用可能に](https://gigazine.net/news/20260918-un-system-data-commons/) | 27.0 | 20.0 | 42.0 |
| [AIを用いて広範囲に存在するソフトウェアデコーダの脆弱性を発見](https://cyberscoop.com/hacktron-ai-heif-heist-vulnerability/) | 25.0 | 20.0 | 42.0 |
| [研究者がClaudeを使ってOpenAI従業員のChatGPTアカウントをハッキング](https://www.theregister.com/security/2026/09/18/researchers-used-claude-to-hack-openai-employees-chatgpt-accounts/5297517) | 25.0 | 20.0 | 42.0 |
| [WordPressのClick2Shell脆弱性、新規テーマのインストールを強制しコード実行に連鎖可能](https://thehackernews.com/2026/09/new-wordpress-click2shell-flaw-forces.html) | 25.0 | 20.0 | 42.0 |
| [AIは本当に人間の制御から逃れようとしたのか](https://www.malwarebytes.com/blog/ai/2026/09/did-an-ai-really-try-to-break-free-from-human-control) | 25.0 | 20.0 | 42.0 |
| [Microsoft、Azure AI Foundryの権限昇格の脆弱性を修正](https://thehackernews.com/2026/09/microsoft-patches-cvss-100-azure-ai.html) | 25.0 | 20.0 | 42.0 |
| [AI生成のエクスプロイトとサインイン脆弱性がOpenAIの内部コードへの侵入経路を開いた](https://www.securityweek.com/ai-built-exploit-and-sign-in-flaw-opened-path-to-internal-openai-code/) | 25.0 | 20.0 | 42.0 |
| [Plugin4Shellにより、リポジトリ所有者が4つのAIコーディングエージェントで固定済みプラグインコードを差し替え可能に](https://thehackernews.com/2026/09/plugin4shell-lets-repository-owners.html) | 25.0 | 20.0 | 42.0 |
| [Microsoft、AIおよびクラウド製品の18件の脆弱性を修正](https://www.securityweek.com/microsoft-patches-18-vulnerabilities-in-ai-cloud-products/) | 25.0 | 20.0 | 42.0 |
| [SNSで人をだますのがうまい「礼儀正しい」ボット](https://www.helpnetsecurity.com/2026/09/18/social-media-bot-detection-study/) | 25.0 | 20.0 | 42.0 |
| [ArcjetがAIエージェントにセキュリティ制御と監査証跡を追加](https://www.helpnetsecurity.com/2026/09/18/arcjet-agent-runtime-security/) | 25.0 | 20.0 | 42.0 |
| [ゼロクリックRCE脆弱性が4つの主要AIコーディングエージェントを直撃、2件は未修正](https://www.helpnetsecurity.com/2026/09/18/plugin4shell-ai-coding-agents-vulnerability/) | 25.0 | 20.0 | 42.0 |
| [Orkes Conductor の重大な脆弱性が攻撃で悪用される](https://www.securityweek.com/critical-orkes-conductor-vulnerability-exploited-in-attacks/) | 24.0 | 46.0 | 50.0 |
| [不正アクセスでサイト改ざん、内部に個人情報 - コンサル会社](https://www.security-next.com/189792) | 22.0 | 20.0 | 42.0 |
| [個人情報含む書類を民生委員の家族が誤廃棄 - 富津市](https://www.security-next.com/190134) | 22.0 | 20.0 | 42.0 |
| [理工学部教職員がフィッシング被害、不審メールが送信 - 日大](https://www.security-next.com/190198) | 22.0 | 20.0 | 42.0 |
| [SynologyのNAS向けOSに深刻な脆弱性 - 修正版を提供](https://www.security-next.com/190538) | 22.0 | 20.0 | 42.0 |
| [前回からわずか2日、「Chrome」が更新 - 「クリティカル」脆弱性を解消](https://www.security-next.com/190534) | 22.0 | 20.0 | 42.0 |
| [ニチレイ、計5万件超の個人情報漏えいを確認 7月のサイバー攻撃で](https://www.itmedia.co.jp/news/article/2609/18/2000001648/) | 21.0 | 20.0 | 42.0 |
| [肖像画をChatGPTに読み込ませて出力→加工して納品 委託先による著作権侵害で、小学館「サライ.jp」が謝罪](https://www.itmedia.co.jp/news/article/2609/18/2000001645/) | 21.0 | 20.0 | 42.0 |
| [Cisco Secure Firewall Adaptive Security ApplianceおよびSecure Firewall Threat Defense Softwareのログ機能におけるサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asa-ftd-logging-dos-ZXXNesfN) | 20.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall 3100および4200シリーズのDTLSサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-dtls-dos-Kp57HkyO) | 20.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Adaptive Security ApplianceおよびSecure Firewall Threat Defense SoftwareのIKEv2証明書認証におけるサービス妨害の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-ikev2cert-dos-uWyc2xtv) | 20.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall ASAおよびSecure Firewall Threat Defense SoftwareのObject Group Access Control Listバイパス脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ftd-acl-bypass-8p6vFvw) | 20.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Adaptive Security ApplianceおよびSecure Firewall Threat Defense SoftwareのTCP DNSサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-tcpdns-dos-p6dUnjr5) | 20.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Adaptive Security ApplianceおよびSecure Firewall Threat Defense SoftwareのEIGRPサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-eigrp-dos-GOhNejSj) | 20.0 | 46.0 | 50.0 |
| [北朝鮮系ハッカーが求職者を悪用して暗号資産とデータを窃取していることについて各国の治安機関が警告](https://cyberscoop.com/north-korea-waterplum-job-seeker-crypto-attacks/) | 20.0 | 20.0 | 48.0 |
| [MFAでは防げないOAuth同意悪用](https://www.darkreading.com/vulnerabilities-threats/mfa-oauth-consent-abuse) | 20.0 | 20.0 | 42.0 |
| [北朝鮮の偽求人面接で3万台のデバイスが感染](https://www.theregister.com/security/2026/09/18/north-koreas-fake-job-interviews-infected-30000-devices/5297461) | 20.0 | 20.0 | 42.0 |
| [Symantec PAMクラスタリングにおいて「Less Is More」が重要な理由](https://www.security.com/product-insights/part-1-why-less-more-symantec-pam-clustering) | 20.0 | 20.0 | 42.0 |
| [FBI、偽警官や政府機関のなりすまし詐欺で被害額16億ドルと発表](https://www.theregister.com/cyber-crime/2026/09/18/fbi-fake-cop-and-government-impersonation-scams-cost-victims-16b/5297499) | 20.0 | 20.0 | 42.0 |
| [Gyazoサーバーの脆弱性が悪用され、2360万件のユーザーレコードが窃取される](https://www.bleepingcomputer.com/news/security/gyazo-server-flaw-exploited-to-steal-236-million-user-records/) | 20.0 | 20.0 | 42.0 |
| [CISA、週次の脆弱性まとめを終了し優先順位付け重視へ移行](https://www.cybersecuritydive.com/news/cisa-vulnerability-bulletins-sunset-prioritization/830779/) | 20.0 | 20.0 | 42.0 |
| [事業に導入するための予防的セキュリティアーキテクチャとは何か](https://www.itpro.com/security/cyber-attacks/building-a-pre-emptive-security-architecture-what-is-it-and-how-can-your-business-adopt-one) | 20.0 | 20.0 | 42.0 |
| [Microsoft 365 のアクセスレビューによる安全な企業内共有](https://www.bleepingcomputer.com/news/security/secure-enterprise-sharing-with-access-reviews-for-microsoft-365/) | 20.0 | 20.0 | 42.0 |
| [Microsoft Teamsで管理者がカスタムファイル拡張子をブロック可能に](https://www.bleepingcomputer.com/news/security/microsoft-teams-will-let-admins-block-custom-file-extensions/) | 20.0 | 20.0 | 42.0 |
| [NightEagleが中国のハイテク産業を標的にした攻撃をロシアへ拡大](https://therecord.media/hacking-group-nighteagle-expands-russia-china) | 20.0 | 20.0 | 42.0 |
| [Microsoft Defender Antivirusがオフと表示される不具合を修正](https://www.bleepingcomputer.com/news/security/microsoft-fixes-bug-behind-defender-antivirus-is-turned-off-alerts/) | 20.0 | 20.0 | 42.0 |
| [Gyazoのデータ侵害で2300万件のユーザーレコードが流出](https://www.securityweek.com/23-million-user-records-compromised-in-gyazo-data-breach/) | 20.0 | 20.0 | 42.0 |
| [国際共同作戦でNightmareStresser DDoSサービスを停止](https://www.securityweek.com/nightmarestresser-ddos-service-disrupted-in-international-operation/) | 20.0 | 20.0 | 42.0 |
| [Vaultに見えるHeapビュー：AgentCore HarnessとIdentityの間にある不安な空白](https://unit42.paloaltonetworks.com/securing-aws-agentcore-harness-credentials/) | 20.0 | 20.0 | 42.0 |
| [CISA、脆弱性報告プラットフォームをより自動化へ刷新](https://www.infosecurity-magazine.com/news/cisa-upgrades-vulnerability/) | 20.0 | 20.0 | 42.0 |
| [NCSCがサイバー敵対者シミュレーションに関する助言を公表](https://www.itpro.com/security/ncsc-issues-advice-on-cyber-adversary-simulation) | 20.0 | 20.0 | 42.0 |
| [Check Pointの新たな脆弱性でハッカーがroot権限でコード実行可能に](https://www.bleepingcomputer.com/news/security/check-point-warns-critical-flaw-lets-hackers-execute-code-as-root/) | 20.0 | 20.0 | 42.0 |
| [ニチレイ、サイバー攻撃による個人情報漏えいを確認。配送先・取引先・従業員などの約5万件](https://internet.watch.impress.co.jp/docs/news/2142333.html) | 20.0 | 20.0 | 42.0 |
| [北朝鮮の攻撃グループがIT技術者に「技術力を確認したい」などと近づき暗号資産を窃取、警察庁・NCOが手口を解説 「世界にとっての安全保障、経済活動上の脅威」として注意喚起](https://internet.watch.impress.co.jp/docs/news/2142320.html) | 20.0 | 20.0 | 42.0 |
| [Androidアプリで個別デバイスコンポーネントごとのセキュリティパッチを確認可能に](https://www.helpnetsecurity.com/2026/09/18/google-androidx-security-state-libraries/) | 20.0 | 20.0 | 42.0 |

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
