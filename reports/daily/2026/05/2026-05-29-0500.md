# 📡 サイレーダー 2026-05-29 05:00 JST

このレポートは、2026-05-28 17:00 JST〜2026-05-29 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 247
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [New Gogs zero-day flaw lets hackers get remote code execution](#topic-11823) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [Microsoft Slams Public Zero-Day Disclosures Amid GitHub Researcher Account Removal](#topic-11829) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Critical FortiClient EMS Vulnerability Exploited in Fresh Attacks](#topic-11763) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Qumulo NeuralProtect uses AI to detect and stop ransomware before encryption](#topic-11767) | 35.0 | 30.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [Fake ChatGPT download site infects Windows and Mac users with malware](#topic-11790) | 34.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-11823"></a>

### 1. New Gogs zero-day flaw lets hackers get remote code execution

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>RCE</nobr> / <nobr>ゼロデイ</nobr> / <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 41.0 |
| <nobr>実務影響</nobr> | 56.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

セルフホスト型Gitサービス「Gogs」に、未修正のゼロデイ脆弱性があるとされています。
公開されている情報では、インターネットから到達可能な環境でリモートコード実行につながる可能性が示されており、悪用観測もあるとされています。
Gogsを外部公開している組織では、サーバー上で任意コード実行につながるおそれがあるため、影響が大きい話題です。
ゼロデイであるため、修正版の有無や適用状況を早急に確認する必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Gogsを外部公開している資産がないか棚卸しし、該当インスタンスを優先確認する。
- ベンダー告知や修正版の有無を確認し、利用中バージョンへの影響を評価する。
- Webアクセスログや不審な変更、予期しないプロセス起動など、侵害の兆候を点検する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [New Gogs zero-day flaw lets hackers get remote code execution](https://www.bleepingcomputer.com/news/security/new-gogs-zero-day-flaw-lets-hackers-get-remote-code-execution/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-11829"></a>

### 2. Microsoft Slams Public Zero-Day Disclosures Amid GitHub Researcher Account Removal

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ゼロデイ</nobr> / <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Microsoftは、脆弱性の発見内容を公開前にベンダーへ共有する協調的な開示（CVD）の重要性を改めて訴えています。
背景には、研究者による複数のゼロデイ脆弱性に関する公開があり、公開の是非をめぐる議論が続いています。
ゼロデイ情報の公開は、対策の促進につながる一方で、未修正の状態が広く知られることでリスクが高まる可能性があります。
ベンダーと研究者の開示プロセスのあり方が、実務上の脆弱性対応に直結するため注目されています。

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

- 自組織で利用中のMicrosoft製品に未適用の更新や緩和策がないか確認する。
- 公開された脆弱性情報が自社環境に関係するか、優先度を付けて評価する。
- 脆弱性の報告・共有はCVDに沿って進め、影響確認と対策準備を早める。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft Slams Public Zero-Day Disclosures Amid GitHub Researcher Account Remov](https://thehackernews.com/2026/05/microsoft-slams-public-zero-day.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-11763"></a>

### 3. Critical FortiClient EMS Vulnerability Exploited in Fresh Attacks

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>KEV</nobr> / <nobr>ゼロデイ</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

FortinetのFortiClient EMSに関する脆弱性について、実際の悪用が新たに観測されたと報じられています。
Fortinetは4月に修正を提供し、ゼロデイとして悪用された可能性があるとして早急な適用を呼びかけていました。
管理製品の脆弱性が現実に悪用されているなら、対応の遅れがそのまま侵害リスクにつながります。対象製品を利用している組織は、修正適用状況と露出状況の確認が重要です。

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

- FortiClient EMSを利用している環境では、修正済みバージョンへの更新状況を確認する。
- 外部公開の有無や不要な到達経路がないかを点検し、アクセス制御を見直す。
- 侵害の兆候確認として、関連する認証・管理系のログを重点的に点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Fortinet | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Critical FortiClient EMS Vulnerability Exploited in Fresh Attacks](https://www.securityweek.com/critical-forticlient-ems-vulnerability-exploited-in-fresh-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-11767"></a>

### 4. Qumulo NeuralProtect uses AI to detect and stop ransomware before encryption

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> / <nobr>AI</nobr> / <nobr>ゼロデイ</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 35.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Qumuloが、ストレージ層でランサムウェアの兆候を検知し、暗号化される前に止めることを目指す「Qumulo NeuralProtect」を発表しました。
データ書き込み時点でAI分析を行い、既知・未知の脅威の両方に対応する設計とされています。
ランサムウェア対策が、被害後の復旧だけでなく、保存前に異常を見つけて抑止する方向へ進んでいる点が注目されます。
ストレージ基盤に組み込まれるため、バックアップやEDRとは別の防御層として検討される可能性があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 既存のバックアップ、EDR、ストレージ保護との役割分担を整理し、重複や抜けを確認する。
- 書き込み時点での検知・隔離が業務に与える影響、誤検知時の運用手順を確認する。
- 未知の脅威対応をうたう製品でも、検知精度や復旧フローは実環境で検証してから採用を判断する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Qumulo NeuralProtect uses AI to detect and stop ransomware before encryption](https://www.helpnetsecurity.com/2026/05/28/qumulo-neuralprotect-uses-ai-to-detect-and-stop-ransomware-before-encryption/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-11790"></a>

### 5. Fake ChatGPT download site infects Windows and Mac users with malware

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>Windows</nobr> / <nobr>マルウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 34.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

ChatGPTを探している利用者を狙った偽のダウンロードサイトが確認され、WindowsとMacの双方に対してそれぞれ異なる不正なファイルを配布していたとされています。
正規の入手先を装う形で誘導するため、見た目だけでは判別しにくい点が懸念されます。
生成AI関連サービスの人気に便乗した誘導は、利用者の注意をすり抜けやすく、端末感染につながるおそれがあります。
WindowsとMacの両環境が対象になっているため、特定OSだけを守ればよい話ではありません。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIサービス名を含む配布サイトや広告リンクを、正規の提供元かどうかを含めて確認する。
- 端末側ではEDR/AVの検知状況を見直し、未知のダウンロード実行や不審なアーカイブ展開を監視する。
- 社内周知では、検索経由の入手や非公式サイトからのインストールを避けるよう注意喚起する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |
| ai_model_or_project | ChatGPT | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Fake ChatGPT download site infects Windows and Mac users with malware](https://www.malwarebytes.com/blog/threat-intel/2026/05/fake-chatgpt-download-site-infects-windows-and-mac-users-with-malware) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり・低信頼。
- 攻撃・悪用観測シグナル: なし。

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
| [Gentlemenランサムウェア：自己拡散型Go暗号化ツールの解析](https://www.microsoft.com/en-us/security/blog/2026/05/28/the-gentlemen-ransomware-dissecting-a-self-propagating-go-encryptor/) | 30.0 | 30.0 | 42.0 |
| [問合管理システムがランサム被害、学習システムなどは影響なし - CKCグループ](https://www.security-next.com/184513) | 30.0 | 30.0 | 42.0 |
| [ランサムウェア集団のリークサイトにMyPillowが掲載、侵害は否定](https://www.bitdefender.com/en-us/blog/hotforsecurity/mypillow-ransomware-leak-site-denies-breach) | 28.0 | 30.0 | 42.0 |
| [2026年ワールドカップ：世界最大のスポーツイベントの攻撃対象領域について](https://unit42.paloaltonetworks.com/fifa-world-cup-attack-surface/) | 28.0 | 30.0 | 42.0 |
| [CVE-2026-46069: mwifiex_adapter_cleanup()におけるuse-after-freeの修正](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-46069) | 28.0 | 28.0 | 38.0 |
| [Threat ActorsがFortiClient EMSの重大な脆弱性を悪用して認証情報窃取マルウェアを配布](https://thehackernews.com/2026/05/threat-actors-exploit-critical.html) | 28.0 | 20.0 | 42.0 |
| [クルーズ大手Carnival、約600万人に影響するデータ侵害を確認](https://therecord.media/cruise-giant-carnival-confirms-data-breach-affecting-6-million) | 28.0 | 20.0 | 42.0 |
| [新しいBTMOB Androidマルウェアが端末を完全に乗っ取る可能性](https://www.securityweek.com/new-btmob-android-malware-enables-full-device-takeover/) | 28.0 | 20.0 | 42.0 |
| [新たな脅威アクターJinx-0164がmacOS上の暗号資産開発者を標的にする](https://www.infosecurity-magazine.com/news/jinx-0164-crypto-developers-macos/) | 28.0 | 20.0 | 42.0 |
| [BTMOB RATがMaaSモデルを通じてブラジルとラテンアメリカに拡散](https://www.darkreading.com/cyberattacks-data-breaches/btmob-rat-brazil-latam-maas-model) | 28.0 | 20.0 | 42.0 |
| [最近のAPTキャンペーンで標的となった石油輸送、ドローンメーカー、そして汚染されたコードライブラリ](https://www.helpnetsecurity.com/2026/05/28/eset-apt-activity-report/) | 28.0 | 20.0 | 42.0 |
| [Qevlarの新しいAIエージェントがCVE、インシデントデータ、実際の悪用シグナルを相関分析](https://www.helpnetsecurity.com/2026/05/28/qevlar-ai-agents/) | 27.0 | 20.0 | 43.0 |
| [AIエージェントの「記憶」は人間の記憶とどう異なるのか？](https://gigazine.net/news/20260528-ai-agent-memory-system/) | 27.0 | 20.0 | 42.0 |
| [AIによる「自律型戦争」は既に始まっている、Anthropicと国防総省との争いが自律型AI兵器のリスクを浮き彫りに](https://gigazine.net/news/20260528-ai-warfare-already/) | 27.0 | 20.0 | 42.0 |
| [「答弁原案も作成」 政府職員10万人が生成AI「源内」利用可能に デジタル庁が大規模実証開始](https://www.itmedia.co.jp/news/articles/2605/28/news136.html) | 26.0 | 20.0 | 42.0 |
| [AIがサイバーに与える影響をテーマに下院委員会が公聴会開催へ](https://cyberscoop.com/house-hearing-frontier-ai-cybersecurity-threats/) | 25.0 | 20.0 | 42.0 |
| [ロシア関連の「GreyVibe」攻撃者がAIを悪用してサイバー攻撃を強化](https://www.securityweek.com/russia-linked-greyvibe-attackers-use-ai-to-supercharge-cyberattacks/) | 25.0 | 20.0 | 42.0 |
| [LLM誘導によるEDRシグネチャ削減：Adversarial Oracles](https://www.praetorian.com/blog/llm-edr-signature-reduction/) | 25.0 | 20.0 | 42.0 |
| [Geordie、AIセキュリティおよびガバナンスプラットフォーム向けに3000万ドルを調達](https://www.securityweek.com/geordie-raises-30-million-for-ai-security-and-governance-platform/) | 25.0 | 20.0 | 42.0 |
| [Agentic AIは危険ではなく、組織の導入方法が問題である](https://www.darkreading.com/application-security/agentic-ai-risky) | 25.0 | 20.0 | 42.0 |
| [エンタープライズデータがシャドーAIツールに流れ込む問題](https://www.cybersecuritydive.com/news/shadow-ai-enterprise-data-policies-okta/821344/) | 25.0 | 20.0 | 42.0 |
| [Microsoft Copilotの信頼性テスト：検出ゼロ、モデル拡大、監視の強化](https://www.helpnetsecurity.com/2026/05/28/microsoft-365-copilot-iso-42001-certification/) | 25.0 | 20.0 | 42.0 |
| [ThreatsDay Bulletin: Claude Security Plugin、Azure特権昇格、Kali365 MFAバイパス、FIFA詐欺ほか15件以上](https://thehackernews.com/2026/05/threatsday-bulletin-claude-security.html) | 25.0 | 20.0 | 42.0 |
| [OpenAI、選挙に向けたChatGPTの誤情報対策を準備](https://www.helpnetsecurity.com/2026/05/28/chatgpt-ai-election-misinformation-deepfakes/) | 25.0 | 20.0 | 42.0 |

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
