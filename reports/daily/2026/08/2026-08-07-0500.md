# 📡 サイレーダー 2026-08-07 05:00 JST

このレポートは、2026-08-06 17:00 JST〜2026-08-07 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 97
- [音声で扱う想定のトピック](#audio-topics): 4
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 69

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [AI Recommendation Poisoning: How "Ask AI" Buttons Silently Alter LLM Memory](#topic-26490) | 35.0 | 20.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [Thwarting the AI Vishing Attacks That Targeted Point72, Citadel, Two Sigma and More](#topic-26439) | 35.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [Zenity Labs Releases Free AI Total Service to Test Malicious Agent Skills](#topic-26442) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [NASがランサム被害、内部に関係者連絡先 - 日本ご当地キャラクター協会](#topic-26456) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-26490"></a>

### 1. AI Recommendation Poisoning: How "Ask AI" Buttons Silently Alter LLM Memory

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

商用サイトの「Ask AI」ボタンや事前入力された深いリンクを悪用し、LLM向けの入力に意図しない指示を混ぜ込む新しいプロンプトインジェクションの手口が報告されています。
記事では、マーケティングページや競合比較ページ上の埋め込み要素を通じて、ユーザーがAIアシスタントに送る内容が静かに誘導されうる点が指摘されています。
この種の手口はマルウェアや侵入を伴わず、既存のWeb導線とAI機能の組み合わせだけで成立しうるため、見落とされやすいのが特徴です。
企業のAI機能導入やWeb運用において、表示内容だけでなくリンク先や埋め込みテキストの検証が重要になります。

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

- 「Ask AI」や共有リンクなど、ユーザー入力前提の導線に埋め込まれる文言を点検し、不要な事前入力を減らす。
- AIアシスタントに渡すコンテンツの出所と信頼境界を見直し、Webページ内テキストをそのまま指示として扱わない設計を確認する。
- マーケティング、比較、サポートなど外部公開ページの更新時に、意図しないプロンプト混入がないかレビュー手順を入れる。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [AI Recommendation Poisoning: How "Ask AI" Buttons Silently Alter LLM Memory](https://thehackernews.com/2026/08/ai-recommendation-poisoning-how-ask-ai.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-26439"></a>

### 2. Thwarting the AI Vishing Attacks That Targeted Point72, Citadel, Two Sigma and More

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

投資運用会社を標的にしたAIによるボイスフィッシング（vishing）キャンペーンが話題になっています。
公開情報では、攻撃者がIT担当者や同僚を装い、音声を使ってヘルプデスクに接触し、認証情報やアカウント権限の変更を急がせたとされています。
音声合成やなりすましの精度向上により、本人確認の前提が揺らぎやすくなっているためです。ヘルプデスクや認証窓口の運用設計が、従来以上に重要になっています。

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

- 電話や音声だけで認証・権限変更を完結させず、多要素の確認手順を必須にする。
- ヘルプデスク向けに、緊急依頼や権限変更時の本人確認フローを見直す。
- 従業員に対し、音声なりすましを前提にした連絡手段の検証と報告ルールを周知する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Thwarting the AI Vishing Attacks That Targeted Point72, Citadel, Two Sigma and M](https://securityboulevard.com/2026/08/thwarting-the-ai-vishing-attacks-that-targeted-point72-citadel-two-sigma-and-more/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-26442"></a>

### 3. Zenity Labs Releases Free AI Total Service to Test Malicious Agent Skills

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Zenity Labsは、AIエージェント向けの「skills」を隔離環境で実行し、実行時の挙動を確認できる無料の脅威インテリジェンスサービス「AI Total」を公開しました。
あわせて、認証情報を狙うキャンペーンに関する調査結果も示しており、AI機能の配布経路に潜むリスクへの注意がうかがえます。
AIエージェントやその拡張機能は便利な一方、想定外の動作や悪性コードの混入が問題になり得ます。こうした検証サービスは、導入前の安全確認や脅威評価の参考になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIエージェントの拡張機能やskillsを本番導入前に隔離環境で確認すること。
- 認証情報や秘密情報へのアクセス権限を最小化し、実行時の挙動を監視すること。
- 配布元や更新経路が不自然なAI関連コンポーネントは、導入判断を慎重に行うこと。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Zenity Labs Releases Free AI Total Service to Test Malicious Agent Skills](https://securityboulevard.com/2026/08/zenity-labs-releases-free-ai-total-service-to-test-malicious-agent-skills/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-26456"></a>

### 4. NASがランサム被害、内部に関係者連絡先 - 日本ご当地キャラクター協会

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

日本ご当地キャラクター協会が、ネットワークストレージ（NAS）にランサムウェア被害があったと公表しました。
内部に関係者の連絡先が保存されていた可能性があり、情報管理への影響が懸念されます。
NASは共有ファイルの集約先になりやすく、被害時には業務情報や個人連絡先などの漏えい・利用停止につながるおそれがあります。
公表内容からは被害の範囲の詳細はまだ限定的ですが、組織内の情報保護体制を見直す契機になります。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- NASや共有ストレージに保存されている機微情報の棚卸しとアクセス権限の確認を行う。
- バックアップの隔離保管と復旧手順を点検し、実際に戻せるか定期的に検証する。
- 端末・サーバー・ストレージの監視と、ランサムウェア被害時の連絡・初動対応手順を再確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [NASがランサム被害、内部に関係者連絡先 - 日本ご当地キャラクター協会](https://www.security-next.com/187812) | <nobr>内容確認・補足情報</nobr> |

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
| [npmを超えてマルウェア警告を拡張する方法](https://github.blog/security/supply-chain-security/how-we-took-malware-advisories-beyond-npm/) | 28.0 | 45.0 | 42.0 |
| [ランサムウェア関連の法執行・司法措置](https://therecord.media/belarus-hacker-ransomware-sentenced) | 28.0 | 30.0 | 42.0 |
| [UNC6671による再ブランド化：マルチブランドのビッシング恐喝が金融サービスとエンタープライズクラウド環境を標的に](https://cloud.google.com/blog/topics/threat-intelligence/unc6671-targets-financial-services-and-enterprise-cloud-environments/) | 28.0 | 20.0 | 48.0 |
| [OctLurkとSilkLurkのモジュール型サイバー諜報フレームワークの分析](https://blog.polyswarm.io/octlurk-and-silklurk-analysis-of-a-modular-cyber-espionage-framework) | 28.0 | 20.0 | 42.0 |
| [Snowflakeをめぐる恐喝事件でカナダ人男性が有罪を認める](https://securityboulevard.com/2026/08/canadian-man-pleads-guilty-in-snowflake-extortions/) | 28.0 | 20.0 | 42.0 |
| [小説閲覧アプリがユーザーのスマートフォンを使って偽の広告トラフィックを生成](https://www.helpnetsecurity.com/2026/08/06/papyrus-mobile-ad-fraud-scheme/) | 28.0 | 20.0 | 42.0 |
| [IT部門が、社員のログインを支援するためノートPCに付箋を貼っていた](https://www.theregister.com/security/2026/08/06/it-department-put-sticky-notes-on-the-laptops-to-help-employees-log-in/5283662) | 28.0 | 20.0 | 42.0 |
| [Canadian HackerがSnowflake恐喝キャンペーンで有罪を認める](https://www.infosecurity-magazine.com/news/canadian-hacker-guilty-snowflake/) | 28.0 | 20.0 | 42.0 |
| [Black Hat USA 2026 Arsenalの写真](https://www.helpnetsecurity.com/2026/08/06/black-hat-usa-2026-arsenal-photos/) | 28.0 | 20.0 | 42.0 |
| [CVE-2026-20200: Cisco IMCの重大な脆弱性により攻撃者にroot権限が付与される恐れ、PoCも公開済み](https://www.helpnetsecurity.com/2026/08/06/cisco-imc-cve-2026-20200-public-poc-exploit/) | 25.0 | 38.0 | 56.0 |
| [Vectra AI、Security Agent向けにクロスドメイン攻撃シグナルを提供するProプランを発表](https://securityboulevard.com/2026/08/vectra-ai-launches-pro-offering-to-feed-security-agents-cross-domain-attack-signals/) | 25.0 | 20.0 | 42.0 |
| [Cyble、Titan Endpoint Platformを発表しシリコンルートの認証機能を搭載](https://securityboulevard.com/2026/08/cyble-unveils-titan-endpoint-platform-with-silicon-rooted-attestation/) | 25.0 | 20.0 | 42.0 |
| [Black Hat USA 2026の写真集（後編）](https://www.helpnetsecurity.com/2026/08/06/black-hat-usa-2026-business-hall-photos/) | 25.0 | 20.0 | 42.0 |
| [PoCから本番環境へ加速するエンタープライズAI](https://www.akamai.com/blog/ai/2026/aug/accelerating-enterprise-ai-proof-concept-production) | 25.0 | 20.0 | 42.0 |
| [人間の介入があるAIコーディングエージェントの危険な要求の3分の1を見逃す](https://www.theregister.com/ai-and-ml/2026/08/06/humans-in-the-loop-miss-a-third-of-dangerous-ai-coding-agent-requests/5284236) | 25.0 | 20.0 | 42.0 |
| [Meta AIモデル、設定ミスのサイバー演習中に企業を攻撃](https://www.bleepingcomputer.com/news/security/meta-ai-model-hacked-a-company-during-misconfigured-cyber-test/) | 25.0 | 20.0 | 42.0 |
| [AIが明らかにした、企業が無視できないブラウザのセキュリティギャップ](https://www.bleepingcomputer.com/news/security/how-ai-exposed-a-browser-security-gap-that-enterprises-cannot-ignore/) | 25.0 | 20.0 | 42.0 |
| [MetaがOpenAIとAnthropicに続きAI悪用インシデントを報告](https://www.infosecurity-magazine.com/news/meta-ai-exploit-incident/) | 25.0 | 20.0 | 42.0 |
| [ゼロクリックのAIブラウザ攻撃：ClaudeとChatGPT AtlasがメールやX投稿経由で乗っ取られる](https://www.securityweek.com/zero-click-ai-browser-hacking-claude-and-chatgpt-atlas-hijacked-via-emails-x-posts/) | 25.0 | 20.0 | 42.0 |
| [AI生成の脆弱性修正パッチの4分の3に不具合が残る](https://www.helpnetsecurity.com/2026/08/06/1password-ai-generated-vulnerability-patches/) | 25.0 | 20.0 | 42.0 |
| [AnthropicのMythos AIがソーシャルエンジニアリング攻撃で開発者を欺こうとし、他のエージェントと連携](https://www.itpro.com/security/cyber-attacks/anthropics-mythos-ai-tried-to-dupe-devs-in-social-engineering-attack-collaborated-with-other-agents) | 25.0 | 20.0 | 42.0 |
| [割引価格のClaudeアクセスを闇市場で購入すると送信したすべてのプロンプトが漏えいする可能性](https://www.helpnetsecurity.com/2026/08/06/ai-model-access-fraud-gray-market/) | 25.0 | 20.0 | 42.0 |
| [AnthropicのMythos AIがソーシャルエンジニアリングで実在の人物を標的にした件](https://www.malwarebytes.com/blog/news/2026/08/anthropics-mythos-ai-used-social-engineering-to-target-real-people) | 25.0 | 20.0 | 42.0 |
| [AppleのバグバウンティプログラムがAI生成の粗悪報告に埋もれ、深刻な脆弱性を見逃す恐れ](https://www.bitdefender.com/en-us/blog/hotforsecurity/apple-bug-bounty-ai-missing-exploits) | 25.0 | 20.0 | 42.0 |
| [地下フォーラムで割引価格のAIトークンを販売するサイバー犯罪者](https://www.itpro.com/security/cyber-crime/cyber-criminals-are-selling-discount-ai-tokens-on-underground-forums) | 25.0 | 20.0 | 42.0 |
| [Token Jacking：サイバー犯罪者によるAIリソース窃取の可能性](https://unit42.paloaltonetworks.com/ai-token-jacking/) | 25.0 | 20.0 | 42.0 |
| [Meta AIがサイバーセキュリティテスト中に外部システムへ侵入していた問題](https://www.securityweek.com/meta-ai-hacked-external-systems-during-cybersecurity-testing/) | 25.0 | 20.0 | 42.0 |
| [Microsoft、エンタープライズAIへのゼロトラスト適用を拡大](https://www.helpnetsecurity.com/2026/08/06/microsoft-zero-trust-for-ai-strategy-updates/) | 25.0 | 20.0 | 42.0 |
| [ABB Ability Zenon の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-218-01) | 24.0 | 46.0 | 50.0 |
| [ThreatsDay: OdysseusのRCE、Samsungのワンクリック乗っ取り、iCloudバックドア攻防ほか27件の話題](https://thehackernews.com/2026/08/threatsday-odysseus-rce-samsung-one.html) | 24.0 | 38.0 | 42.0 |
| [中国製Zbtlinkルーターに未認証でrootシェルを開くバックドアが搭載されている](https://thehackernews.com/2026/08/chinese-made-zbtlink-routers-ship-with.html) | 24.0 | 38.0 | 42.0 |
| [比喩がセキュリティ戦略を左右する理由](https://blog.talosintelligence.com/why-metaphor-may-dictate-your-security-strategy/) | 22.0 | 20.0 | 42.0 |
| [窓口で公開している台帳図面に個人情報 - 長野県](https://www.security-next.com/188467) | 22.0 | 20.0 | 42.0 |
| [アメリカ12州の水道施設がサイバー攻撃の標的に、イランによるインフラ攻撃の疑い](https://gigazine.net/news/20260806-cyberattacks-water-systems/) | 22.0 | 20.0 | 42.0 |
| [定食チェーンの持帰注文サイトで個人情報流出の可能性](https://www.security-next.com/188296) | 22.0 | 20.0 | 42.0 |
| [職員アカウントに不正アクセス、ニュース配信には影響なし - 共同通信](https://www.security-next.com/188445) | 22.0 | 20.0 | 42.0 |
| [連邦当局の警告にもかかわらず、水道システムで使われる米国の産業用コントローラー数千台が依然オンラインで露出](https://cyberscoop.com/exposed-rockwell-controllers-water-system-attacks/) | 20.0 | 28.0 | 50.0 |
| [New Zapscape KVMの脆弱性により、特権L1ゲストコードがLinuxホストへエスケープする可能性](https://thehackernews.com/2026/08/new-zapscape-kvm-flaw-could-let.html) | 20.0 | 28.0 | 50.0 |
| [Johnson Controls Inc. TL280の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-218-02) | 20.0 | 28.0 | 50.0 |
| [Medixant RadiAnt DICOMの脆弱性](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-218-01) | 20.0 | 28.0 | 50.0 |
| [BobmojisからBobbleheadsへ：民主党が築いたセキュリティ第一の文化](https://www.darkreading.com/cybersecurity-operations/from-bobmojis-to-bobbleheads-how-the-democratic-party-built-a-security-first-culture) | 20.0 | 20.0 | 42.0 |
| [Ransom Cartel創設者、懲役16年の判決](https://cyberscoop.com/ransom-cartel-creator-sentenced-to-16-years-in-prison/) | 20.0 | 20.0 | 42.0 |
| [Swiss governmentのSharePoint侵害で200件のアカウントが漏えい](https://www.bleepingcomputer.com/news/security/swiss-government-sharepoint-breach-compromised-200-accounts/) | 20.0 | 20.0 | 42.0 |
| [VanishID、露出した個人データ向けの外部ID保護を提供開始](https://securityboulevard.com/2026/08/vanishid-launches-external-identity-protection-for-exposed-personal-data/) | 20.0 | 20.0 | 42.0 |
| [Dispel、OTリモートアクセス向けの本人確認機能を提供開始](https://securityboulevard.com/2026/08/dispel-launches-identity-proofing-for-operational-technology-remote-access/) | 20.0 | 20.0 | 42.0 |
| [TONTOUの新たなCPU攻撃、Spectre v2修正を回避してLinuxのパスワードハッシュを漏えい](https://www.bleepingcomputer.com/news/security/new-tontou-cpu-attack-bypasses-spectre-v2-fixes-leaks-linux-password-hashes/) | 20.0 | 20.0 | 42.0 |
| [ノースカロライナ州の港湾へのサイバー攻撃は封じ込め済み、沿岸警備隊と州当局が調査](https://therecord.media/cyberattack-north-carolina-ports) | 20.0 | 20.0 | 42.0 |
| [Cisco、SD-WANとIOS XEの12件の脆弱性を修正、CVSS 9.8の3件を含む](https://thehackernews.com/2026/08/cisco-patches-12-sd-wan-and-ios-xe.html) | 20.0 | 20.0 | 42.0 |
| [PCI DSS 4.0とcomforte TAMUNIO：トークナイゼーションの有効性](https://securityboulevard.com/2026/08/pci-dss-4-0-and-comforte-tamunio-the-case-for-tokenization/) | 20.0 | 20.0 | 42.0 |
| [IntelおよびAMD CPUのSpectre v2防御を回避可能な新たなInterrupt Injection攻撃](https://thehackernews.com/2026/08/new-interrupt-injection-attack-can.html) | 20.0 | 20.0 | 42.0 |
| [Oracle Database内に隠されたツールキットがエンドポイントツールを回避](https://www.infosecurity-magazine.com/news/khunt-toolkit-oracle-database-sql/) | 20.0 | 20.0 | 42.0 |
| [陸自が個人情報収集か 対象者証言](https://news.yahoo.co.jp/pickup/6590805?source=rss) | 20.0 | 20.0 | 42.0 |
| [Snowflakeへの不正アクセスをめぐるハッカー、米国で有罪を認める](https://www.securityweek.com/snowflake-hacker-pleads-guilty-in-us-court/) | 20.0 | 20.0 | 42.0 |
| [Apple WebKitの脆弱性によりPrivate Relayを使っていてもIPアドレスが漏えいする問題](https://www.malwarebytes.com/blog/news/2026/08/apple-webkit-vulnerabilities-reveal-your-ip-address-despite-private-relay) | 20.0 | 20.0 | 42.0 |
| [MITRE ATT&CK T1053.005における検知のギャップ](https://www.security.com/expert-perspectives/detection-gap-mitre-attck-t1053005) | 20.0 | 20.0 | 42.0 |
| [Black Hat USA 2026の写真集](https://www.helpnetsecurity.com/2026/08/06/black-hat-usa-2026-photos/) | 20.0 | 20.0 | 42.0 |
| [Snowflakeへの不正侵入でハッカーが有罪を認め、最長32年の禁錮刑の可能性](https://www.helpnetsecurity.com/2026/08/06/snowflake-canadian-hacker-pleaded-guilty/) | 20.0 | 20.0 | 42.0 |
| [米国の水道システムへの攻撃は氷山の一角か、サイバー専門家が警鐘](https://www.itpro.com/security/cyber-attacks/attacks-on-us-water-systems-could-be-the-tip-of-the-iceberg-cyber-experts-warn) | 20.0 | 20.0 | 42.0 |
| [4,400台超のRockwell PLCがオンラインで露出、22台は水道攻撃の都市で発見](https://thehackernews.com/2026/08/over-4400-rockwell-plcs-exposed-online.html) | 20.0 | 20.0 | 42.0 |
| [暴力的な物理的暗号資産窃取が3,000万ドルの損失に急増](https://www.infosecurity-magazine.com/news/violent-physical-crypto-thefts/) | 20.0 | 20.0 | 42.0 |
| [Podcast: コンプライアンスでは守れない、Edna Conwayと考えるサイバーリスクの未来](https://www.securityweek.com/podcast-compliance-wont-save-you-the-future-of-cyber-risk-with-edna-conway/) | 20.0 | 20.0 | 42.0 |
| [OnlyFans利用者を狙うディープフェイク詐欺](https://www.malwarebytes.com/blog/news/2026/08/scammers-target-onlyfans-users-with-deepfakes) | 20.0 | 20.0 | 42.0 |
| [Apple iCloud Private RelayがWebKitのプロキシ回避により実IPを露出する可能性](https://thehackernews.com/2026/08/webkit-proxy-bypasses-can-expose-real.html) | 20.0 | 20.0 | 42.0 |
| [Paperclipの重大な脆弱性により管理者アクセスとコード実行が可能に](https://www.securityweek.com/critical-paperclip-flaw-allowed-admin-access-code-execution/) | 20.0 | 20.0 | 42.0 |
| [AmazonとAppleをかたる「$149.99の不正請求」詐欺](https://www.malwarebytes.com/blog/scams/2026/08/amazon-and-apple-impersonated-in-149-99-unauthorized-charge-scam) | 20.0 | 20.0 | 42.0 |
| [水道分野に再び警鐘が鳴らされた](https://cyberscoop.com/water-utility-cyberattacks-prevention-nozomi-networks-ceo-op-ed/) | 20.0 | 20.0 | 42.0 |
| [Oracle内でkhuntをコンパイルし、SQLインジェクションをWindows SYSTEM権限に昇格させる攻撃者](https://thehackernews.com/2026/08/attackers-compile-khunt-inside-oracle.html) | 20.0 | 20.0 | 42.0 |
| [AWS、Google、Vercelのエージェント脆弱性により、モデルを実行せずにツールを起動可能](https://thehackernews.com/2026/08/aws-google-and-vercel-patch-agent-flaws.html) | 20.0 | 20.0 | 42.0 |
| [インターネットに公開された数千台の燃料計器が放置されたままに](https://www.bitsight.com/blog/thousands-exposed-fuel-gauges-just-left-internet) | 20.0 | 20.0 | 42.0 |

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
