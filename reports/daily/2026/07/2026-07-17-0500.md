# 📡 サイレーダー 2026-07-17 05:00 JST

このレポートは、2026-07-16 17:00 JST〜2026-07-17 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 112
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 82

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CISA Adds Three Known Exploited Vulnerabilities to Catalog](#topic-22576) | 45.0 | 56.0 | 47.0 | 音声 | 温度感上位枠 |
| 2 | [CISA orders feds to patch actively exploited Oracle flaw by Saturday](#topic-22886) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Spirals: New Stealthy Ransomware Deployed Against Asian IT Company](#topic-22905) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Iran-nexus actors using AI to enhance cyber playbook](#topic-22828) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Russian cybercriminal used jailbroken Gemini CLI to rebuild botnet infrastructure in six minutes](#topic-22862) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-22576"></a>

### 1. CISA Adds Three Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 47.0 |

#### 概要

CISA は、実際の悪用が確認されている脆弱性として、Fortinet FortiSandbox と Microsoft SharePoint に関する3件を Known Exploited Vulnerabilities（KEV）カタログに追加しました。
公開情報では、これらは攻撃者による悪用の証拠があるとされ、企業・組織の防御優先度が高い案件と位置づけられています。
KEV への追加は、単なる脆弱性情報ではなく、すでに攻撃に使われている可能性が高いことを示します。
特に広く使われる製品に関わる場合、未対応の環境が残っていると被害につながりやすいため注意が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象製品の保有有無を確認し、該当バージョンの修正状況を点検する。
- CISA の KEV 収載状況を踏まえて、通常の優先度より前倒しで対応計画を見直す。
- 関連製品のログや不審な管理操作を確認し、侵害の兆候がないか点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-15409 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-15410 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-25089 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-39808 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-58644 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Fortinet | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| ランサムウェアグループ | Akira | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Three Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/07/16/cisa-adds-three-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall customers under threat as attackers exploit 2 zero-days](https://cyberscoop.com/sonicwall-zero-day-vulnerabilities-exploited/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22886"></a>

### 2. CISA orders feds to patch actively exploited Oracle flaw by Saturday

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAが、Oracle E-Business Suiteに関する重大な脆弱性について、連邦機関に対し土曜日までに対策を完了するよう求めたと報じられています。
公開情報では、すでに悪用が確認されている文脈で扱われており、対象製品を利用する組織では早急な確認が必要です。
業務基盤として使われる可能性があるERP製品の脆弱性で、実際の悪用が示されている点が重視されています。
政府機関に期限付きで対応が求められていることから、他組織でも同様の優先対応が検討されます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Oracle E-Business Suiteの利用有無と、関連する公開済みの対策状況を確認する。
- 該当システムの露出状況を見直し、必要に応じてアクセス制限や監視を強化する。
- ベンダー提供の修正版や公表済みガイダンスを確認し、優先度を上げて適用する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2024-21182 | 関連CVE | 1.00 | 候補あり（URL 4件以上） |
| 脆弱性 | CVE-2025-61884 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-46817 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Oracle | 言及あり | 0.80 | — |
| 製品 | Oracle E-Business Suite | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA orders feds to patch actively exploited Oracle flaw by Saturday](https://www.bleepingcomputer.com/news/security/cisa-orders-feds-to-patch-actively-exploited-oracle-flaw-by-saturday/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22905"></a>

### 3. Spirals: New Stealthy Ransomware Deployed Against Asian IT Company

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Broadcom/Symantecの脅威情報によると、アジアのIT企業を標的に、これまで確認されていないランサムウェアのペイロードが使われたとされています。
攻撃は2026年6月に発生したとされ、運用者の手口から今後より広いキャンペーンにつながる可能性が示されています。
新規性のあるランサムウェア事案として、同種の攻撃が他組織へ波及するかどうかが注目点です。公開一次情報に基づく脅威情報であるため、実務上は早めの警戒と備えの確認に意味があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ランサムウェア対策として、バックアップの隔離保管と復元手順の定期確認を行う。
- 侵入後の横展開や権限昇格を想定し、EDR・ログ監視・管理者アカウントの利用状況を点検する。
- フィッシング、脆弱性悪用、認証情報の不正利用など初期侵入経路の防御を改めて確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Spirals: New Stealthy Ransomware Deployed Against Asian IT Company](https://www.security.com/threat-intelligence/ransomware-spirals-extortion) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22828"></a>

### 4. Iran-nexus actors using AI to enhance cyber playbook

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

イラン関連とみられる攻撃者やハクティビストが、ChatGPTなどのAIツールを悪用して、マルウェア開発やフィッシング、産業施設の情報収集に関わる作業を補助していたとする報告が出ています。
現時点では、AIが攻撃そのものを自動化したというより、既存の手口を効率化・高度化する用途で使われた可能性が示されています。
生成AIは防御側だけでなく攻撃側にも利用されうるため、脅威アクターの作業効率が上がると、従来型のフィッシングや調査活動の質が変わる可能性があります。
特に、対象組織の公開情報や業務文脈を踏まえた不審メールや偵察が増えると、見分けにくさが増します。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 従業員向けのフィッシング訓練と、外部要因を含む認証強化（MFA、条件付きアクセス）を継続する。
- 公開情報の露出を点検し、施設名・担当者情報・業務手順などが攻撃者の下調べに使われないよう整理する。
- AI生成文面を含む可能性を前提に、メール・チャット・問い合わせの不自然な依頼は複数経路で確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Iran-nexus actors using AI to enhance cyber playbook](https://www.cybersecuritydive.com/news/iran-nexus-actors-ai-cyber-ChatGPT-malware/825415/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22862"></a>

### 5. Russian cybercriminal used jailbroken Gemini CLI to rebuild botnet infrastructure in six minutes

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

TrendAIによると、ロシア語話者とみられる攻撃者が、改変されたGemini CLIを使って小規模なC2基盤の構築と運用を行ったとされています。
報道では、複数回の対話セッションを通じて、歯科クリニックの端末群やデータベースへのアクセスに関与した可能性が示されています。
生成AIのコマンドライン型エージェントが、攻撃者の作業効率化に悪用されうることを示す事例として注目されています。
AIツールの安全対策や利用制御が、実運用上の重要課題であることを再認識させます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIエージェントを業務利用する際は、権限範囲と実行制御を明確にする。
- 不審な自動化や短時間での基盤変更を検知できるよう、C2や管理系操作の監視を強化する。
- 外部連携するAIツールは、プロンプト注入や不正利用を前提にログ・監査を残す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Google | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | Gemini | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Russian cybercriminal used jailbroken Gemini CLI to rebuild botnet infrastructur](https://www.helpnetsecurity.com/2026/07/16/jailbroken-google-gemini-cli-botnet/) | <nobr>内容確認・補足情報</nobr> |

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
| [20以上の乗っ取られた政府サイトが攻撃経路に利用された](https://thehackernews.com/2026/07/20-hijacked-government-websites.html) | 30.0 | 20.0 | 42.0 |
| [UAT-11795が金銭目的のキャンペーンで新型Starland RATと独自WLDR C2インプラントを展開](https://blog.talosintelligence.com/uat-11795-deploys-novel-starland-rat-and-bespoke-wldr-c2-implant-in-financially-motivated-campaign/) | 30.0 | 20.0 | 42.0 |
| [AI支援による脆弱性管理の設計図を読み解く](https://cloud.google.com/blog/topics/threat-intelligence/ai-assisted-vulnerability-management/) | 29.0 | 45.0 | 43.0 |
| [ThreatsDay: ゲームチート用スパイウェア、24時間型ランサムウェア、Chrome Syncによる追跡など12件の話題](https://thehackernews.com/2026/07/threatsday-game-cheat-spyware-24-hour.html) | 28.0 | 30.0 | 42.0 |
| [ValorC3、SaaS保護を不変のクラウドバックアップで強化](https://www.helpnetsecurity.com/2026/07/16/valorc3-backup-as-a-service-baas/) | 28.0 | 30.0 | 42.0 |
| [新たなSpiralsランサムウェアが24時間以内に被害ネットワークを暗号化](https://www.bleepingcomputer.com/news/security/new-spirals-ransomware-encrypts-victim-network-in-under-24-hours/) | 28.0 | 30.0 | 42.0 |
| [Rockwell Automation Flex 5000 Adapterの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-197-08) | 28.0 | 28.0 | 50.0 |
| [ANY.RUNが明らかにした改ざん政府サイトによるマルウェア配布の隠れたインフラストラクチャー](https://any.run/cybersecurity-blog/phantomenigma-research/) | 28.0 | 20.0 | 48.0 |
| [PhishingキャンペーンがLuaローダーをTrueTypeフォントファイルに偽装](https://www.infosecurity-magazine.com/news/phishing-lua-loader-truetype-font/) | 28.0 | 20.0 | 42.0 |
| [Sandwormハッカーがウクライナ人向けに仕掛けたCAPTCHAの手口](https://therecord.media/ukraine-sandworm-hacks-captcha-powershell) | 28.0 | 20.0 | 42.0 |
| [Air-gappedネットワーク向けの安全なパッチ管理を簡素化するAdaptiva](https://www.helpnetsecurity.com/2026/07/16/adaptiva-airgap-for-onesite-patch/) | 28.0 | 20.0 | 42.0 |
| [ViPNet更新システムを通じて新たな悪意あるモジュールを展開するHelloNetキャンペーン](https://securelist.com/tr/hellonet-vipnet/120700/) | 28.0 | 20.0 | 42.0 |
| [ClickFixを利用して拡散しデータ窃取とコマンド実行を行う新たなTELEPUZマルウェア](https://thehackernews.com/2026/07/new-telepuz-malware-spreads-via.html) | 28.0 | 20.0 | 42.0 |
| [ClickLock Stealerがソーシャルエンジニアリングとプロセス終了でmacOSのセキュリティを回避](https://www.securityweek.com/clicklock-stealer-bypasses-macos-security-with-social-engineering-process-killing/) | 28.0 | 20.0 | 42.0 |
| [台湾で再び確認されたDaxinとStupigのログイン前SYSTEMバックドア](https://thehackernews.com/2026/07/daxin-resurfaces-in-taiwan-alongside.html) | 28.0 | 20.0 | 42.0 |
| [Russian hackersがWebExやZoomアプリをトロイの木馬化してStarlandマルウェアを配布](https://www.bleepingcomputer.com/news/security/russian-hackers-trojanize-webex-zoom-apps-to-push-starland-malware/) | 28.0 | 20.0 | 42.0 |
| [AIエージェントの最小権限：ID、アクセス、ツールのバインディング](https://www.microsoft.com/en-us/security/blog/2026/07/16/least-privilege-for-ai-agents-identity-access-and-tool-binding/) | 27.0 | 20.0 | 42.0 |
| [SunoがShai-Huludワームによる侵害を受け、流出コードでAI音楽スクレイピングが露呈](https://socket.dev/blog/suno-breach-shai-hulud-worm) | 27.0 | 20.0 | 42.0 |
| [Public AttackerKBプラットフォームの終了](https://www.rapid7.com/blog/post/ve-sunsetting-public-attackerkb-platform) | 27.0 | 20.0 | 42.0 |
| [Claude Chrome拡張機能の欠陥により悪意ある拡張機能がAI操作を誘発可能](https://www.bleepingcomputer.com/news/security/claude-chrome-extension-flaw-lets-malicious-extensions-trigger-ai-actions/) | 25.0 | 20.0 | 42.0 |
| [自律型AIエージェントの封じ込めにマイクロセグメンテーションを活用する](https://www.akamai.com/blog/security/2026/jul/microsegmentation-contain-autonomous-ai-agents) | 25.0 | 20.0 | 42.0 |
| [OpenAI 初のハードウェアを販売](https://news.yahoo.co.jp/pickup/6588199?source=rss) | 25.0 | 20.0 | 42.0 |
| [AIエージェントがセキュリティの常識を覆した 今こそ必要な新たな対策とは](https://www.bleepingcomputer.com/news/security/ai-agents-broke-the-security-playbook-heres-what-replaces-it/) | 25.0 | 20.0 | 42.0 |
| [単一のプロンプトでChatGPTがサイバー攻撃の一連の流れを実行可能に、研究者が指摘](https://www.infosecurity-magazine.com/news/chatgpt55-to-execute-full/) | 25.0 | 20.0 | 42.0 |
| [AIデータセンターは保護が追いつかないまま急速に建設されている](https://www.securityweek.com/ai-data-centers-are-being-built-faster-than-they-can-be-secured/) | 25.0 | 20.0 | 42.0 |
| [1PasswordがAnthropicと提携し、Claudeに認証情報へのアクセスを提供](https://www.itpro.com/security/1password-teams-up-with-anthropic-to-give-claude-access-to-your-credentials) | 25.0 | 20.0 | 42.0 |
| [新たなAgentデータ注入攻撃でAIエージェントが誤クリックや攻撃者コマンド実行の恐れ](https://thehackernews.com/2026/07/new-agent-data-injection-attack-can.html) | 25.0 | 20.0 | 42.0 |
| [IntruderがWebアプリケーション向けのAI搭載オンデマンド侵入テストを提供](https://www.helpnetsecurity.com/2026/07/16/intruder-brings-ai-powered-on-demand-penetration-testing-to-web-applications/) | 25.0 | 20.0 | 42.0 |
| [AIはバグを見つけられるが、証明には依然として人間の知識が必要](https://thehackernews.com/2026/07/ai-can-find-bugs-but-human-knowledge.html) | 25.0 | 20.0 | 42.0 |
| [SANS、セキュリティチームでのAI利用急増に伴うAIガバナンスの欠如に警鐘](https://www.infosecurity-magazine.com/news/sans-warns-of-ai-governance-gap/) | 25.0 | 20.0 | 42.0 |
| [Lineation.ai、自律型AIエージェント向けのランタイムセキュリティに注力](https://www.helpnetsecurity.com/2026/07/16/lineation-ai-zero-trust-control-plane/) | 25.0 | 20.0 | 42.0 |
| [米国、AI駆動の脆弱性管理を調整する「Gold Eagle」を開始](https://www.infosecurity-magazine.com/news/us-gold-eagle-ai-vulnerability/) | 25.0 | 20.0 | 42.0 |
| [OpenAIのGPT-Red、GPT-5.6 Solの防御強化に向けてプロンプトインジェクション試験を自動化](https://thehackernews.com/2026/07/openais-gpt-red-automates-prompt.html) | 25.0 | 20.0 | 42.0 |
| [SALTO ProAccess Spaceの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-197-07) | 22.0 | 40.0 | 50.0 |
| [AutomationDirect Productivity Suiteの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-197-04) | 22.0 | 40.0 | 50.0 |
| [Windows 11 24H2 Home と Pro のサポート終了まであと90日](https://www.bleepingcomputer.com/news/microsoft/windows-11-24h2-home-and-pro-reach-end-of-support-in-90-days/) | 22.0 | 20.0 | 43.0 |
| [Patch Warsが始まった](https://blog.talosintelligence.com/begun-the-patch-wars-have/) | 22.0 | 20.0 | 42.0 |
| [職員が患者情報を使用、他医療機関の開業を案内 - 済生会宇都宮病院](https://www.security-next.com/186910) | 22.0 | 20.0 | 42.0 |
| [設定ミスでイベント申込者情報が閲覧可能に - 開催中止に](https://www.security-next.com/187128) | 22.0 | 20.0 | 42.0 |
| [委託先コンサルが個人情報含む記憶媒体を紛失 - 旭市](https://www.security-next.com/187230) | 22.0 | 20.0 | 42.0 |
| [自動化された脅威ハンティングを受け入れるべき時か？](https://blog.talosintelligence.com/the-hunters-paradox-is-it-time-to-embrace-automated-threat-hunting/) | 22.0 | 20.0 | 42.0 |
| [Claudeのメモリから氏名や勤務先を盗み出す攻撃手法が発見される、ウェブ閲覧機能を悪用して外部サイトへ送信](https://gigazine.net/news/20260716-claude-memory-heist/) | 22.0 | 20.0 | 42.0 |
| [「SAP」が月例更新、16件の新規アドバイザリ - 3件が「クリティカル」](https://www.security-next.com/187482) | 22.0 | 20.0 | 42.0 |
| [Rockwell Automation FactoryTalk DataMosaixの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-197-09) | 21.0 | 34.0 | 50.0 |
| [Rockwell Automation CompactLogix、ControlLogix、Compact GuardLogix、GuardLogixの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-197-06) | 20.0 | 28.0 | 50.0 |
| [Rockwell Automation 1756-EN2、1756-EN3、1756-ENBTの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-197-02) | 20.0 | 28.0 | 50.0 |
| [Rockwell Automation Arenaにおける脆弱性問題](https://www.cisa.gov/news-events/ics-advisories/icsa-26-197-01) | 20.0 | 28.0 | 50.0 |
| [Siemens SICAM 8の脆弱性とセキュリティリスク](https://www.cisa.gov/news-events/ics-advisories/icsa-26-197-05) | 20.0 | 28.0 | 50.0 |
| [NASA Core Flight System (cFS) Health & Safety (HS) アプリケーション](https://www.cisa.gov/news-events/ics-advisories/icsa-26-197-03) | 20.0 | 28.0 | 50.0 |
| [Adobe、Chrome、Firefox、VMware、Zoomのセキュリティ更新情報](https://www.malwarebytes.com/blog/bugs/2026/07/security-updates-available-for-adobe-chrome-firefox-vmware-and-zoom) | 20.0 | 28.0 | 50.0 |
| [Scattered Spiderの2人、Transport for Londonへの攻撃で実刑判決](https://www.theregister.com/cyber-crime/2026/07/16/brit-scattered-spider-duo-handed-tickets-to-prison-over-transport-for-london-attack/5272446) | 20.0 | 20.0 | 48.0 |
| [OkoBotの新たなフレームワークが20種類のペイロードを展開してデータと暗号資産を窃取](https://www.bleepingcomputer.com/news/security/new-okobot-framework-deploys-20-payloads-to-steal-data-crypto/) | 20.0 | 20.0 | 42.0 |
| [ロシアの3人がサイバー犯罪を助長したとされる耐弾性ホスティング事業運営で起訴](https://cyberscoop.com/russian-nationals-medialand-mlcloud-indicted-bulletproof-hosting/) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderのハッカー2人、TfLへの2900万ポンド規模の侵害でそれぞれ5年半の判決](https://thehackernews.com/2026/07/two-scattered-spider-hackers-get-55.html) | 20.0 | 20.0 | 42.0 |
| [「この文字列をコピーしてmacOSのTerminalに貼り付ければPCが直る」とする手口](https://www.theregister.com/cyber-crime/2026/07/16/cmon-just-copy-this-text-string-and-paste-it-into-your-macos-terminal-itll-fix-your-computer-honest/5273701) | 20.0 | 20.0 | 42.0 |
| [レガシーシステムがもたらす現実の影響：OTセキュリティの実態](https://www.securityweek.com/legacy-systems-real-world-impacts-the-reality-of-ot-security/) | 20.0 | 20.0 | 42.0 |
| [米国の航空サイバーセキュリティ規制当局を阻むネットワークセキュリティの欠陥と監督戦略の不備](https://www.cybersecuritydive.com/news/aviation-cybersecurity-faa-tsa-gao-report/825416/) | 20.0 | 20.0 | 42.0 |
| [Flockカメラに対する反発が広がる](https://www.malwarebytes.com/blog/news/2026/07/the-backlash-against-flock-cameras-is-spreading) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderメンバー、Transport for Londonへのハッキングで禁錮刑に　被害額は2900万ポンド](https://www.helpnetsecurity.com/2026/07/16/ransport-for-london-cyberattack-prison-time/) | 20.0 | 20.0 | 42.0 |
| [23andMe、遺伝子データ漏えい訴訟で1800万ドルを支払いへ](https://www.bleepingcomputer.com/news/security/23andme-to-pay-18-million-in-new-genetics-data-breach-settlement/) | 20.0 | 20.0 | 42.0 |
| [n8nのトークン交換の欠陥により、別のIssuerのユーザーとしてログインされるおそれ](https://thehackernews.com/2026/07/n8n-token-exchange-flaw-could-let.html) | 20.0 | 20.0 | 42.0 |
| [Kill Loopを使ってパスワード入力を強要するモジュール型macOS情報窃取マルウェア](https://www.infosecurity-magazine.com/news/clicklock-macos-stealer-clickfix/) | 20.0 | 20.0 | 42.0 |
| [UKでTwo Scattered Spiderのハッカー2人に禁錮刑、判決下る](https://www.securityweek.com/two-scattered-spider-hackers-sentenced-to-jail-in-uk/) | 20.0 | 20.0 | 42.0 |
| [新たなClickLock macOS Stealer、被害者がパスワードを入力するまで210msごとにアプリを終了させる](https://thehackernews.com/2026/07/new-clicklock-macos-stealer-kills-apps.html) | 20.0 | 20.0 | 42.0 |
| [TfLハッキングの背後にいたScattered Spiderのメンバーに懲役5年の判決](https://www.bleepingcomputer.com/news/security/scattered-spider-members-behind-transport-for-london-hack-get-five-years-in-prison/) | 20.0 | 20.0 | 42.0 |
| [GoSerpent：高度なデータ収集と持続的な情報窃取を伴う脅威の進化](https://securelist.com/goserpent-backdoor-in-southeast-asia/120687/) | 20.0 | 20.0 | 42.0 |
| [Scattered SpiderによるTransport for Londonへの29百万ポンド規模のハッキングで5年半の判決](https://therecord.media/scattered-spider-hackers-tfl-sentenced) | 20.0 | 20.0 | 42.0 |
| [TfLへのサイバー攻撃の背後にあった「Selfish Bravado」、2人に実刑判決](https://www.infosecurity-magazine.com/news/selfish-bravado-behind-tfl/) | 20.0 | 20.0 | 42.0 |
| [Windows 10の延命、そのセキュリティ代償が迫る](https://www.theregister.com/os-platforms/2026/07/16/windows-10-refuses-to-die-and-the-security-bill-is-coming-due/5271987) | 20.0 | 20.0 | 42.0 |
| [Oak、ステルスモードを解除し6,000万ドルの資金調達を発表](https://www.securityweek.com/oak-emerges-from-stealth-mode-with-60-million-in-funding/) | 20.0 | 20.0 | 42.0 |
| [SplunkとZoomの重大な脆弱性修正](https://www.securityweek.com/splunk-zoom-patch-critical-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [Microsoft Entra IDでPasskeysが既定の認証方式に、ユーザーへの影響と適用時期は](https://www.itpro.com/security/microsoft-entra-id-passkey-default-authentication-dealine-september-2026) | 20.0 | 20.0 | 42.0 |
| [ルーマニアの土地登記簿がサイバー攻撃を受け、データが販売されている疑い](https://www.helpnetsecurity.com/2026/07/16/romania-ancpi-cyber-attack/) | 20.0 | 20.0 | 42.0 |
| [Telegram短縮リンクが制裁対象VPN接続を原因に停止状態に](https://www.theregister.com/security/2026/07/16/telegram-shortlinks-knocked-offline-over-sanctioned-vpn-connection/5271964) | 20.0 | 20.0 | 42.0 |
| [Samsung、健康データ削除の脅しを撤回](https://www.malwarebytes.com/blog/privacy/2026/07/samsung-backs-down-on-threat-to-delete-health-data) | 20.0 | 20.0 | 42.0 |
| [Tenable One、コードのリスクとエンタープライズの露出データを統合](https://www.helpnetsecurity.com/2026/07/16/tenable-expands-one-exposure-management-platform/) | 20.0 | 20.0 | 42.0 |
| [未修正のShark Vacuumの脆弱性により、地域全体の他の掃除機を制御される可能性](https://thehackernews.com/2026/07/unpatched-shark-vacuum-flaw-could-let.html) | 20.0 | 20.0 | 42.0 |
| [F5がNGINXおよびBIG-IPの複数の脆弱性を修正](https://www.securityweek.com/f5-patches-multiple-nginx-big-ip-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [Smashing Security podcast #476: リモート操作の人力車と不正な書籍マーケター](https://grahamcluley.com/smashing-security-podcast-476/) | 20.0 | 20.0 | 42.0 |
| [中国の大手サイバーセキュリティ企業、軍関連調達で相次ぐ入札禁止措置に直面](https://www.securityweek.com/chinas-top-cybersecurity-firms-hit-by-mounting-military-procurement-bans/) | 20.0 | 20.0 | 42.0 |
| [MicrosoftがWindowsのSSOプロンプトを管理しやすく改善](https://www.helpnetsecurity.com/2026/07/16/windows-sso-policy-admin-control/) | 20.0 | 20.0 | 42.0 |
| [警察が月1億ユーロを盗んだ投資詐欺ネットワークを摘発](https://www.helpnetsecurity.com/2026/07/16/dutch-police-investment-fraud-ring-dismantled/) | 20.0 | 20.0 | 42.0 |

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
