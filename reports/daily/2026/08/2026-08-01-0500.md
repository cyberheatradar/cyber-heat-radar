# 📡 サイレーダー 2026-08-01 05:00 JST

このレポートは、2026-07-31 17:00 JST〜2026-08-01 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 85
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 55

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cisco Secure Firewall Management Center Software Static Credential Vulnerability](#topic-24943) | 42.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 2 | [ESET tracks rise in malicious AI skills and adaptable malware](#topic-25404) | 41.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [Hacker uses DeepSeek AI to autonomously attack vulnerable servers](#topic-25390) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Cybercrime goes subscription: AI, malware and infrastructure on demand](#topic-25414) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Horizon3.ai expands NodeZero with automated web application attack path testing](#topic-25475) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-24943"></a>

### 1. Cisco Secure Firewall Management Center Software Static Credential Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 42.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Cisco Secure Firewall Management Center（FMC）SoftwareのWebインターフェースに、低権限アカウントの静的認証情報に起因する脆弱性（CVE-2026-20316）が報告されています。
公開情報では、認証されていない遠隔の攻撃者が影響を受ける機器へ不正にログインし、機微情報にアクセスできる可能性があるとされています。
FMCは複数のファイアウォール機器を集中管理する製品のため、管理基盤への不正アクセスは運用全体に影響し得ます。
さらに、公開情報では実際の悪用が示唆されており、早期の更新対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Ciscoの修正アップデート適用状況を確認し、影響対象のFMCを優先的に更新する。
- FMC管理インターフェースをインターネットから直接公開しない運用を再確認する。
- 管理画面への不審なログインや権限の低いアカウント利用の痕跡がないか監査する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20316 | 主題CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20316](https://nvd.nist.gov/vuln/detail/CVE-2026-20316) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Firewall Management Center Software Static Credential Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-fmc-static-cred-BET3Cjh) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco FMC static credentials exploited by attackers (CVE-2026-20316)](https://www.helpnetsecurity.com/2026/07/30/cisco-fmc-cve-2026-20316-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure FMC Zero-Day Exploited in the Wild](https://www.securityweek.com/cisco-secure-fmc-zero-day-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of FMC static credential flaw exploited in zero-day attacks](https://www.bleepingcomputer.com/news/security/cisco-warns-of-fmc-static-credential-flaw-exploited-in-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-25404"></a>

### 2. ESET tracks rise in malicious AI skills and adaptable malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

ESETの脅威レポートでは、攻撃者がAI関連の機能や新しい技術、利用者の行動変化に合わせて手口を適応させている状況が取り上げられています。
あわせて、AI支援型マルウェア、ClickFix攻撃、quishing（QRコードを悪用したフィッシング）の増加、セキュリティソフトの無効化を狙うランサムウェア関連ツールにも言及されています。
AIの普及に合わせて攻撃手法も変化しており、従来のフィッシングやマルウェア対策だけでは不十分になる可能性があります。
特にメール、QRコード、偽の操作誘導を組み合わせた手口は利用者教育と技術的対策の両面が重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI関連の新しい誘導手口や、ユーザー操作を促す不審な画面・文面に対する注意喚起を見直す。
- メール経由のフィッシングだけでなく、QRコードを使う誘導や偽の手順案内も検知・周知対象に含める。
- ランサムウェア対策として、セキュリティソフトの保護状態監視や復旧手順の確認を継続する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | ESET | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ESET tracks rise in malicious AI skills and adaptable malware](https://www.bleepingcomputer.com/news/security/eset-tracks-rise-in-malicious-ai-skills-and-adaptable-malware/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-25390"></a>

### 3. Hacker uses DeepSeek AI to autonomously attack vulnerable servers

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、攻撃者がDeepSeekのAIモデルとオープンソースのエージェントを組み合わせ、露出したサーバーへの攻撃をより自律的に進めているとされています。
現時点では、AIが攻撃の一部を自動化し、人手の関与を減らしている可能性が示されています。
攻撃の自動化が進むと、短時間で多数の対象を狙う動きが増え、検知や対応の負荷が高まるおそれがあります。
AIサービスやエージェントの悪用は、従来の攻撃手口よりも運用面の変化として注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 露出しているサーバーや管理画面の棚卸しを行い、不要な公開を減らす。
- 外部から到達可能な認証・監査・アラート設定を見直し、異常な試行の増加を早めに把握できるようにする。
- AI利用そのものよりも、既存の脆弱性放置や設定不備が悪用されやすい点を前提に、パッチ適用と基礎的な防御を優先する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | DeepSeek | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | DeepSeek | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Hacker uses DeepSeek AI to autonomously attack vulnerable servers](https://www.bleepingcomputer.com/news/security/hacker-uses-deepseek-ai-to-autonomously-attack-vulnerable-servers/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-25414"></a>

### 4. Cybercrime goes subscription: AI, malware and infrastructure on demand

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

サイバー犯罪が、AIやマルウェア、インフラを必要に応じて購入・レンタルできる「サービス型」のエコシステムとして商業化しているという指摘です。
こうした仕組みにより、比較的スキルの低い攻撃者でも大規模な攻撃を行いやすくなり、追跡や阻止が難しくなるとされています。
攻撃の実行に必要な機能が分業・外部化されることで、脅威の裾野が広がる点が注目されています。
防御側にとっては、個別の攻撃手口だけでなく、短命なインフラや自動化された運用を前提にした対策が必要になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 短命なドメインやインフラの増減を前提に、監視・遮断の運用を見直す。
- AIを悪用した偽装や自動化を想定し、認証・メール・Webの各経路で多層防御を強化する。
- 脅威インテリジェンスを使い、単発の事案ではなく犯罪サービスの再利用傾向も含めて評価する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Cybercrime goes subscription: AI, malware and infrastructure on demand](https://www.helpnetsecurity.com/2026/07/31/infoblox-domain-abuse-campaigns-report/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-25475"></a>

### 5. Horizon3.ai expands NodeZero with automated web application attack path testing

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Horizon3.aiは、NodeZeroにWebアプリケーション向けの自動テスト機能を拡張したとしています。
公開情報では、アプリケーションの脆弱性を起点に、認証情報の悪用や横展開、クラウド環境への到達、データ露出につながる攻撃経路の把握を支援する内容だと説明されています。
Webアプリケーションは業務システムやクラウド利用の入口になることが多く、攻撃経路をまとめて確認できる点は防御側の優先順位付けに役立ちます。
生成AIを使った開発で脆弱なアプリが増えているという文脈とも重なり、検証需要が高まりやすい話題です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 自社のWebアプリが単体の脆弱性だけでなく、認証情報やクラウド権限まで波及しうるかを点検する。
- 自動テスト結果はそのまま採用せず、重要資産に直結する経路を優先して検証・修正する。
- 生成AI支援の開発で作られたアプリは、公開前後のレビューと設定確認を通常より丁寧に行う。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Horizon3.ai expands NodeZero with automated web application attack path testing](https://www.helpnetsecurity.com/2026/07/31/horizon3-ai-nodezero-webapp-pentesting/) | <nobr>内容確認・補足情報</nobr> |

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
| [Rapid7がBlack Hat USA 2026で示す予防的セキュリティの実演](https://www.rapid7.com/blog/post/dr-black-hat-usa-2026-preemptive-security-in-action) | 35.0 | 20.0 | 42.0 |
| [サーバでランサム被害を確認、影響など調査 - 八王子中高校](https://www.security-next.com/187991) | 30.0 | 30.0 | 42.0 |
| [Xcode Assassinが再来：最新XCSSETの詳細分析](https://unit42.paloaltonetworks.com/xcsset-v40-malware-analysis/) | 29.0 | 20.0 | 43.0 |
| [Mirage Kittenが中東・アフリカを標的にNightLedgerバックドアを展開するスパイ活動キャンペーン](https://blog.polyswarm.io/mirage-kitten-deploys-nightledger-backdoor-in-espionage-campaign-targeting-the-middle-east-and-africa) | 28.0 | 20.0 | 42.0 |
| [HollowFrame Loaderが弁護士事務所へのスピアフィッシング攻撃でMatryoshkaバックドアを展開](https://thehackernews.com/2026/07/hollowframe-loader-deploys-matryoshka.html) | 28.0 | 20.0 | 42.0 |
| [Chinese Hacker Commands DeepSeek via Telegram to Launch Autonomous Attacks](https://thehackernews.com/2026/07/chinese-hacker-commands-deepseek-via.html) | 28.0 | 20.0 | 42.0 |
| [Fake Flash PlayerインストーラーによるAtlasRAT配布](https://www.malwarebytes.com/blog/news/2026/07/fake-flash-player-installs-atlasrat) | 28.0 | 20.0 | 42.0 |
| [AWSがAxiosなどのnpmサプライチェーン攻撃を北朝鮮系グループの仕業と非難](https://www.infosecurity-magazine.com/news/aws-north-korea-axios-npm-supply/) | 28.0 | 20.0 | 42.0 |
| [Ghostty開発者が新会社「Superlogical」を始動、人間とAIの作業を統合するターミナル基盤を構築へ](https://gigazine.net/news/20260731-mitchell-hashimoto-superlogical/) | 27.0 | 20.0 | 42.0 |
| [Google Cloud、AIで脆弱性検出から修復まで自動化 - 「Google AI Threat Defense」で実現するAI時代の防御戦略](https://news.mynavi.jp/techplus/article/20260731-4761265/) | 26.0 | 20.0 | 42.0 |
| [AnthropicのAIも他社侵入、しかも3件 設定ミスでネットアクセス可能に](https://xtech.nikkei.com/atcl/nxt/column/18/00001/11940/) | 26.0 | 20.0 | 42.0 |
| [生成AIを駆使してゲームデモを作成、スクエニ遠矢氏が講演](https://xtech.nikkei.com/atcl/nxt/column/18/03696/072900007/) | 26.0 | 20.0 | 42.0 |
| [CEDEC2026で語られた生成AI活用事例、コンテンツ生成とQA自動化](https://xtech.nikkei.com/atcl/nxt/column/18/03696/072900006/) | 26.0 | 20.0 | 42.0 |
| [OpenAI、最新のGPT 5.6モデルがよりコスト効率的になっていると発表](https://www.bleepingcomputer.com/news/artificial-intelligence/openai-says-its-new-gpt-56-models-are-becoming-more-cost-efficient/) | 25.0 | 20.0 | 42.0 |
| [OpenAIとAnthropicの封じ込め侵害は少し不気味だが、かなり滑稽でもある](https://www.itpro.com/technology/artificial-intelligence/the-openai-and-anthropic-containment-breaches-are-a-bit-spooky-but-also-quite-silly) | 25.0 | 20.0 | 42.0 |
| [OpenAIのオープンソースツール、AWSが北朝鮮と関連付けたハッキング、Mythosの暗号資産調査](https://www.securityweek.com/in-other-news-openai-open-source-tool-aws-links-hacks-to-north-korea-mythos-crypto-research/) | 25.0 | 20.0 | 42.0 |
| [Anthropic、人的ミスでClaude AIモデルがテスト環境を脱出し第三者を攻撃できたと発表](https://www.cybersecuritydive.com/news/anthropic-claude-ai-hacking-test/826708/) | 25.0 | 20.0 | 42.0 |
| [AnthropicとOpenAI、どちらのエージェントがより暴走するかを競う](https://www.theregister.com/security/2026/07/31/anthropic-and-openai-are-competing-to-see-whose-agents-can-go-rogue-harder/5281797) | 25.0 | 20.0 | 42.0 |
| [Symantec DSPMがより深いデータインサイトを提供開始](https://www.security.com/product-insights/symantec-dspm-here-deliver-deeper-data-insights) | 25.0 | 20.0 | 42.0 |
| [攻撃的AIの実運用化：現代のセキュリティのためのオープンフレームワーク](https://www.akamai.com/blog/security/2026/jul/operationalizing-offensive-ai-open-framework-security) | 25.0 | 20.0 | 42.0 |
| [EUが生成AIの監督強化 暴走を抑止](https://news.yahoo.co.jp/pickup/6590082?source=rss) | 25.0 | 20.0 | 42.0 |
| [犯罪者がAIと子ども向けコーディングソフトを悪用し、数百万ドル規模の広告不正収益を築く](https://www.helpnetsecurity.com/2026/07/31/fuyao-ad-fraud-botnet-android-tv-boxes/) | 25.0 | 20.0 | 42.0 |
| [AnthropicのAIが実世界の企業をハッキングした3件の事例を公表](https://therecord.media/anthropic-ai-hacked-three-real-companies) | 25.0 | 20.0 | 42.0 |
| [AIがフィッシング攻撃を加速させる500万ドルの脅威](https://www.fortra.com/blog/5-million-threat-ai-supercharging-phishing-attacks) | 25.0 | 20.0 | 42.0 |
| [Google AIが13年前のChrome脆弱性を発見、過去最高の修正ペースの中で](https://www.securityweek.com/googles-ai-agent-uncovers-13-year-old-chrome-flaw-amid-record-patching-pace/) | 25.0 | 20.0 | 42.0 |
| [Anthropic、サイバーセキュリティテストで制御喪失を認める](https://www.itpro.com/security/anthropic-joins-openai-in-admitting-loss-of-control-in-cybersecurity-tests) | 25.0 | 20.0 | 42.0 |
| [EU、AIディープフェイクや違法画像、ハッキング対策を強化する新チームをブリュッセルに設置](https://www.securityweek.com/eu-to-crack-down-on-ai-deepfakes-illicit-imagery-and-hacking-with-new-team-in-brussels/) | 25.0 | 20.0 | 42.0 |
| [Agentic AI時代の防御においてHugging Faceの侵害が示すもの](https://cyberscoop.com/hugging-face-breach-agentic-ai-security-op-ed/) | 25.0 | 20.0 | 42.0 |
| [AnthropicのClaudeがセキュリティテスト中に3社へ侵入した件](https://www.helpnetsecurity.com/2026/07/31/anthropic-claude-cybersecurity-incidents/) | 25.0 | 20.0 | 42.0 |
| [OpenAIの開示を受け、Anthropicが自社モデルへのハッキングを確認した3組織](https://www.securityweek.com/after-openai-disclosure-anthropic-finds-its-own-models-hacked-3-organizations/) | 25.0 | 20.0 | 42.0 |
| [Zero TrustはAIで止まる](https://securityboulevard.com/2026/07/zero-trust-stops-at-the-ai/) | 25.0 | 20.0 | 42.0 |
| [OpenAIができることはAnthropicならさらにうまくできる](https://securityboulevard.com/2026/07/anything-openai-can-do-anthropic-can-do-better/) | 25.0 | 20.0 | 42.0 |
| [AnthropicがClaudeのテスト脱出と3社への侵害を公表](https://www.infosecurity-magazine.com/news/anthropic-claude-breached-three/) | 25.0 | 20.0 | 42.0 |
| [Traefik Labs、APIおよびAIゲートウェイ向けの安全なランタイム「Distro Zero」を発表](https://www.helpnetsecurity.com/2026/07/31/traefik-labs-distro-zero-image/) | 25.0 | 20.0 | 42.0 |
| [講座受講者一覧表を紛失、メモから発覚 - 厚木市](https://www.security-next.com/187995) | 22.0 | 20.0 | 42.0 |
| [従業員が顧客クレカをスキミング - サムギョプサル店](https://www.security-next.com/187468) | 22.0 | 20.0 | 42.0 |
| [ウクライナのゼレンスキー大統領が「ロシア国内のドローン攻撃にStarlinkを利用させてほしい」とトランプ大統領に要求](https://gigazine.net/news/20260731-zelensky-trump-starlink-drone-strikes-russia/) | 22.0 | 20.0 | 42.0 |
| [契約照会システムで利用者の個人情報が閲覧可能に - 生保協会](https://www.security-next.com/188063) | 22.0 | 20.0 | 42.0 |
| [一般消費者が「空調服」と書いたら商標権侵害？ 公式Xの注意喚起が波紋、弁理士の見解は](https://www.itmedia.co.jp/news/article/2607/31/2000000328/) | 21.0 | 20.0 | 42.0 |
| [Cisco Secure Firewall Management Center Softwareの認証回避の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-onprem-fmc-authbypass-5JPp45V2) | 20.0 | 46.0 | 50.0 |
| [CISAが新たなSBOMガイダンスを公表、適切だったのか？](https://www.darkreading.com/cybersecurity-operations/cisa-issues-fresh-sbom-guidance) | 20.0 | 20.0 | 42.0 |
| [CISAが警告、水道システムへの攻撃急増　ミネソタ州の事案を調査中](https://therecord.media/cisa-warns-of-spike-in-water-system-attacks) | 20.0 | 20.0 | 42.0 |
| [Cyber Commandがシリコンバレーにオフィスを計画、イノベーションを推進](https://therecord.media/cyber-command-plans-silicon-valley-office-to-drive-innovation) | 20.0 | 20.0 | 42.0 |
| [CISAが米国の水道事業者に対するサイバー攻撃による業務妨害を警告](https://www.bleepingcomputer.com/news/security/cisa-warns-of-cyberattacks-disrupting-us-water-utilities/) | 20.0 | 20.0 | 42.0 |
| [物理セキュリティ業界で最も有名なブランドがShinyHuntersに侵害される](https://www.theregister.com/security/2026/07/31/the-most-famous-brand-in-physical-security-got-pwned-by-shinyhunters/5281924) | 20.0 | 20.0 | 42.0 |
| [Fortniteの偽報酬でプレイヤーのアカウントが盗まれる](https://www.malwarebytes.com/blog/scams/2026/07/fake-fortnite-rewards-are-stealing-players-accounts) | 20.0 | 20.0 | 42.0 |
| [ミネソタ州の水道システムへのサイバー攻撃、当局がイラン系ハッカーに警戒呼びかけ](https://www.securityweek.com/cyberattacks-on-minnesota-water-systems-investigated-as-officials-warn-about-iranian-hackers/) | 20.0 | 20.0 | 42.0 |
| [Root of Trustを取り除いた後、それは誰のものでもない](https://www.darkreading.com/cyber-risk/morning-after-we-pull-root-of-trust-nobody-owns-it) | 20.0 | 20.0 | 42.0 |
| [CAF Bankオンライン口座へのアクセスをなお妨げられている慈善団体](https://www.theregister.com/security/2026/07/31/charities-remain-locked-out-of-caf-bank-online-accounts/5281711) | 20.0 | 20.0 | 42.0 |
| [Interpolがグローバルシステムを活用して詐欺支払いを抑止](https://www.darkreading.com/cybersecurity-operations/interpol-leverages-global-system-curtail-fraud-payments) | 20.0 | 20.0 | 42.0 |
| [米国フェンシング界がアマチュアスポーツにおける隠れた身元確認課題に取り組む](https://www.darkreading.com/identity-access-management-security/usa-fencing-hidden-identity-challenge-amateur-sports) | 20.0 | 20.0 | 42.0 |
| [Chromeの最近3回のリリースで1,442件の脆弱性を修正、過去23回分の合計を上回る](https://thehackernews.com/2026/07/three-recent-chrome-releases-fix-1442.html) | 20.0 | 20.0 | 42.0 |
| [4Gおよび5Gコアに84件の脆弱性、セッションハイジャックの欠陥も発見](https://thehackernews.com/2026/07/researchers-report-84-flaws-in-4g-and.html) | 20.0 | 20.0 | 42.0 |
| [Device Code Phishingが2026年に急増している6つの理由](https://thehackernews.com/2026/07/6-reasons-why-device-code-phishing-is.html) | 20.0 | 20.0 | 42.0 |
| [Azure Cosmos DBを侵害可能にした重大な脆弱性](https://www.securityweek.com/critical-flaw-led-to-azure-cosmos-db-pwnage/) | 20.0 | 20.0 | 42.0 |

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
