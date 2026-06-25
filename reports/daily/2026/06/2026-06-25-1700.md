# 📡 サイレーダー 2026-06-25 17:00 JST

このレポートは、2026-06-25 11:00 JST〜2026-06-25 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 42
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 15

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cisco Catalyst SD-WAN Zero-Day CVE-2026-20245 Exploited to Gain Root Access](#topic-15753) | 43.0 | 58.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [MicrosoftとEuropol、情報窃取マルウェア「StealC」「Amadey」の基盤を一斉摘発 C2サーバ200台超を停止](#topic-19281) | 37.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [Most teams will ship AI-written infrastructure code with little review](#topic-19273) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-19281"></a>

### 1. MicrosoftとEuropol、情報窃取マルウェア「StealC」「Amadey」の基盤を一斉摘発 C2サーバ200台超を停止

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

MicrosoftとEuropolは、情報窃取型マルウェア「StealC」と、その配布に使われるローダ「Amadey」の基盤を停止させたと発表しました。
取り締まり活動「Operation Endgame」の一環で、Microsoftは200台を超えるC2サーバを停止し、約1万8000台の被害端末を特定・保護したとしています。
これらのマルウェアは認証情報の窃取に使われ、ランサムウェア攻撃の足掛かりになる可能性があります。
インフラ停止は被害拡大の抑止につながる一方、同種の脅威への継続的な警戒は必要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 認証情報の漏えい疑いがないか、ログやEDRのアラートを改めて確認する。
- 外部アクセス用の多要素認証やパスワード再利用対策を徹底する。
- 情報窃取型マルウェアを入口にしたランサムウェア連鎖を前提に、初動対応手順を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [MicrosoftとEuropol、情報窃取マルウェア「StealC」「Amadey」の基盤を一斉摘発　C2サーバ200台超を停止](https://www.itmedia.co.jp/news/articles/2606/25/news084.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-19273"></a>

### 2. Most teams will ship AI-written infrastructure code with little review

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

AIを使って作成されたインフラコードが、十分な確認を経ないまま本番環境へ流れ込みやすいという点が注目されています。
開発者側はAIで素早くコード化できても、デプロイや運用を担うDevOps／プラットフォーム側では同じ速度向上が得られず、レビューや統制に差が生じる可能性があります。
インフラコードは設定ミスや権限設定の不備があると、可用性や機密性に影響しやすいためです。
AI利用の拡大そのものより、レビューや責任分界が追いつかない運用上のギャップが問題視されています。

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

- AI生成コードを通常のコードと同じではなく、設定・権限・依存関係を重点的に確認する。
- 開発者と運用担当の間でレビュー基準を揃え、IaCや変更管理の承認フローを明確にする。
- AI利用の可視化を進め、重要なインフラ変更は自動チェックと人手レビューを併用する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Most teams will ship AI-written infrastructure code with little review](https://www.helpnetsecurity.com/2026/06/25/ai-infrastructure-governance-gap-report/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-15753"></a>

### 1. Cisco Catalyst SD-WAN Zero-Day CVE-2026-20245 Exploited to Gain Root Access

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Catalyst SD-WAN Managerの脆弱性CVE-2026-20245が、認証済みの攻撃者により権限昇格に悪用されていることが報告されています。
公開情報では、攻撃者はroot権限に到達していたとされますが、Ciscoが確認しているのは限定的な事例で、成功手段の全容が広く確定したわけではありません。
SD-WANの管理基盤が侵害されると、ネットワーク全体の運用や可視性に影響が及ぶ可能性があります。
ゼロデイかつ未修正の段階で悪用観測があるため、影響範囲の把握と対応優先度の判断が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 7 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Ciscoの公式アドバイザリと適用可能な修正状況を確認し、該当製品の露出を洗い出す。
- 管理系アカウントの認証情報保護を強化し、不要な権限付与や古い特権アカウントを点検する。
- SD-WAN管理面の監査ログを確認し、想定外の権限変更や不審なファイル操作の痕跡を探す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20127 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20182 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20245 | 関連CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20245](https://nvd.nist.gov/vuln/detail/CVE-2026-20245) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco SD-WAN Zero-Day Exploited Months Before Patching](https://www.securityweek.com/cisco-sd-wan-zero-day-exploited-months-before-patching/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Zero-Day CVE-2026-20245 Exploited to Gain Root Access](https://thehackernews.com/2026/06/cisco-catalyst-sd-wan-zero-day-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Mandiant reveals how Cisco SD-WAN zero-day attacks gained root access](https://www.bleepingcomputer.com/news/security/mandiant-reveals-how-cisco-sd-wan-zero-day-attacks-gained-root-access/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zero-Day Exploitation of Vulnerability (CVE-2026-20245) in Cisco Catalyst SD-WAN](https://cloud.google.com/blog/topics/threat-intelligence/zero-day-exploitation-cisco-catalyst-sd-wan-manager/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN V](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-privesc-4uxFrdzx) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco customers encounter another SD-WAN zero-day under attack](https://cyberscoop.com/cisco-sdwan-zero-day-vulnerability-exploited-cve202620245/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Manager CVE-2026-20245 Flaw Actively Exploited – No Patch ](https://thehackernews.com/2026/06/cisco-catalyst-sd-wan-manager-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補あり（URL 7件以上 / 該当CVE 3件）。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [7種類の実行環境を再現するAIモデル「Qwen-AgentWorld」が登場、実環境不要でAIエージェントが行動結果を事前予測できるよう訓練可能](https://gigazine.net/news/20260625-qwen-agentworld/) | 29.0 | 20.0 | 42.0 |
| [Claude Mythosがアメリカ政府の機密システムの脆弱性を発見](https://gigazine.net/news/20260625-anthropic-mythos-found-vulnerabilities/) | 27.0 | 20.0 | 42.0 |
| [KPMGコンサルティング、「顧客理解AIエージェント」を核とした支援サービスを提供](https://japan.zdnet.com/article/35249389/) | 26.0 | 20.0 | 42.0 |
| [Windowsの脆弱性探索に100超のAIエージェント活用 Microsoftの月例パッチの裏で稼働するシステムとは](https://atmarkit.itmedia.co.jp/ait/articles/2606/25/news045.html) | 26.0 | 20.0 | 42.0 |
| [LLMのセキュリティ助言は難所を確認すると甘くなる](https://www.helpnetsecurity.com/2026/06/25/helpbench-llm-security-advice/) | 25.0 | 20.0 | 42.0 |
| [正解のないAIハッカーの評価方法](https://www.helpnetsecurity.com/2026/06/25/ai-offensive-cyber-evaluations-benchmark/) | 25.0 | 20.0 | 42.0 |
| [オープンソース開発におけるAI活用のベストプラクティス](https://www.helpnetsecurity.com/2026/06/25/foss-ai-in-open-source/) | 25.0 | 20.0 | 42.0 |
| [海賊版サイトにおける大手ブランドの広告シェアが1年間で80％急増したとEUの調査で判明](https://gigazine.net/news/20260625-pirate-ads-euipo/) | 22.0 | 20.0 | 42.0 |
| [AnthropicがAlibabaを「蒸留攻撃」で非難、Claudeに2880万回以上のアクセスか](https://gigazine.net/news/20260625-anthropic-accuses-alibaba/) | 22.0 | 20.0 | 42.0 |
| [流出の恐れがある@niftyの「メールパスワード」って何？ 「ログインパスワード」とは違うの？](https://www.itmedia.co.jp/news/articles/2606/25/news088.html) | 21.0 | 20.0 | 42.0 |
| [@nifty、ログイン通知メール一時停止 「負荷集中」のため](https://www.itmedia.co.jp/news/articles/2606/25/news076.html) | 21.0 | 20.0 | 42.0 |
| [国家支援の攻撃者が豪州の重要インフラを破壊し得る状態に侵入していたことが判明](https://www.theregister.com/security/2026/06/25/nation-state-actors-cracked-critical-australian-infrastructure-to-cripple-it-at-a-time-of-their-choosing/5261877) | 20.0 | 20.0 | 48.0 |
| [英国の学校ネットワークが無防備に放置され、学生が侵入を発見](https://www.theregister.com/security/2026/06/25/uk-schools-network-left-wide-open-for-invasion-student-found/5261567) | 20.0 | 20.0 | 42.0 |
| [今週、エンジニアリングリーダーが必ず確認すべき稼働率の問い](https://www.helpnetsecurity.com/2026/06/25/mattias-geniar-oh-dear-preventing-outages/) | 20.0 | 20.0 | 42.0 |
| [次回のサイバー保険更新で求められること](https://www.helpnetsecurity.com/2026/06/25/cyber-insurance-controls-video/) | 20.0 | 20.0 | 42.0 |

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
