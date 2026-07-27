# 📡 サイレーダー 2026-07-28 05:00 JST

このレポートは、2026-07-27 17:00 JST〜2026-07-28 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 89
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 58

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Adversaries Don't Need a Zero-Day — They Read Your Rulebook](#topic-24460) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [PTC Windchill Vulnerability Exploited in Ransomware Campaign](#topic-24491) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [Rethinking security for the age of AI](#topic-24464) | 35.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Hackers used autonomous AI agent to spy on Thailand's finance ministry](#topic-24507) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [ランサム感染の可能性、店舗に影響なし - ファイブフォックス](#topic-24502) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-24460"></a>

### 1. Adversaries Don't Need a Zero-Day — They Read Your Rulebook

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

攻撃者がゼロデイ脆弱性を使わなくても、防御側のルールや検知ロジックを理解して回避する可能性がある、という点が論点になっています。
自律型のセキュリティツールへの信頼が揺らいでいる背景として、検知の前提や運用設定そのものが狙われうることが示唆されています。
新しい脆弱性がなくても防御をすり抜けられるなら、運用上の見直しや監視の強化が必要になるためです。
検知ルールの品質だけでなく、ルールの公開範囲やチューニング、例外設定の管理も重要になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 検知ルールやアラート条件の見直しを定期的に行い、固定化しすぎない。
- 自動化ツールの判断に依存しすぎず、重要イベントは別系統でも確認できるようにする。
- 例外設定や抑止ルールの棚卸しを行い、不要に広い緩和が残っていないか確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Adversaries Don't Need a Zero-Day — They Read Your Rulebook](https://www.darkreading.com/threat-intelligence/adversaries-do-not-need-zero-day-they-read-your-rulebook) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-24491"></a>

### 2. PTC Windchill Vulnerability Exploited in Ransomware Campaign

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

PTCの製品「Windchill」に関する脆弱性が、ランサムウェア攻撃の文脈で悪用されたと報じられています。
公開情報では、認証不要でリモートから任意コード実行につながる可能性がある深刻な不適切なデシリアライゼーション問題が指摘されています。
業務システムやPLM基盤のような企業利用の高い製品が標的になると、侵入後の影響が広範囲に及ぶおそれがあります。
ランサムウェア文脈での悪用報告は、優先度の高い確認・対策対象になりやすい点で注目されます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当製品の利用有無と影響範囲を確認し、ベンダー情報に基づいて修正・緩和策を適用する。
- インターネット公開の必要性を見直し、アクセス制御や到達範囲の最小化を検討する。
- 不審な管理操作・プロセス起動・暗号化兆候がないか、関連ログと端末の監視を強化する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [PTC Windchill Vulnerability Exploited in Ransomware Campaign](https://www.securityweek.com/ptc-windchill-vulnerability-exploited-in-ransomware-campaign/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-24464"></a>

### 3. Rethinking security for the age of AI

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftのセキュリティブログでは、AI時代に合わせてセキュリティの考え方を見直す必要性が示されました。
自律的に動作するシステムの登場や、攻撃側のコスト低下、守るべき対象の増大・複雑化が背景にあるとしています。
AIの活用が広がるほど、従来の前提だけでは防御や運用が追いつかない可能性があります。
セキュリティ担当者にとっては、AIを前提にした監視・検知・統制の再設計を考えるきっかけになります。

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

- AIを使うシステムの権限管理と監査ログを改めて確認する。
- 自動化された処理が誤動作した場合の検知・停止手順を整理する。
- 既存の境界防御だけでなく、継続監視や異常検知の運用を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Rethinking security for the age of AI](https://blogs.microsoft.com/blog/2026/07/27/rethinking-security-for-the-age-of-ai/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-24507"></a>

### 4. Hackers used autonomous AI agent to spy on Thailand's finance ministry

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者の調査により、攻撃者が自律型のAIエージェントを使ってタイ財務省を標的としたサイバー諜報活動を行っていたとされています。
現時点で確認できる範囲では、AIを実際の攻撃運用に組み込んだ事例として注目されています。
AIが防御側だけでなく攻撃側の運用にも使われうることを示す事例として、脅威の見方を更新する必要があります。
特に行政・財務分野の組織では、標的型の情報窃取への警戒を強める材料になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIを利用した偵察・情報収集の兆候を含め、標的型攻撃の検知観点を見直す。
- 行政・財務関連の重要情報へのアクセス権限や監査ログの確認を強化する。
- 不審な自動化挙動や通常と異なる問い合わせパターンを、既存の監視ルールで拾えるか点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Hackers used autonomous AI agent to spy on Thailand's finance ministry](https://therecord.media/thailand-hackers-ai-finance-ministry) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-24502"></a>

### 5. ランサム感染の可能性、店舗に影響なし - ファイブフォックス

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

ファイブフォックスは、本社の一部サーバがランサムウェアに感染した可能性があると明らかにしました。現時点では、店舗営業などへの影響はないとされています。
ランサムウェアの疑いがある事案であり、企業の社内サーバ運用や復旧対応の重要性が改めて注目されます。
店舗などの外部サービスに影響が出ていない点も含め、事業継続の観点で見られています。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 社内サーバの影響範囲を早期に切り分け、業務継続への波及がないか確認する。
- バックアップ、復旧手順、初動連絡体制が機能するか点検する。
- 感染の可能性がある段階でも、関係部門への周知と監視強化を進める。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ランサム感染の可能性、店舗に影響なし - ファイブフォックス](https://www.security-next.com/187382) | <nobr>内容確認・補足情報</nobr> |

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
| [重大なAD CSのドメイン乗っ取り脆弱性（CVE-2026-54121）のPoCエクスプロイト公開](https://www.helpnetsecurity.com/2026/07/27/certighost-cve-2026-54121-poc-exploit-released/) | 29.0 | 38.0 | 52.0 |
| [Coca-Cola、Fairlifeへのランサムウェア攻撃でデータ窃取を確認](https://www.bleepingcomputer.com/news/security/coca-cola-confirms-data-theft-in-fairlife-ransomware-attack/) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア攻撃後、Coca-Colaは乳製品部門の生産能力の大半を回復](https://www.cybersecuritydive.com/news/coca-cola-restores-most-production-capacity-at-dairy-unit-after-ransomware/826250/) | 28.0 | 30.0 | 42.0 |
| [Fairlifeへのランサムウェア攻撃後にCoca-Colaがデータ侵害を確認](https://www.securityweek.com/coca-cola-confirms-data-breach-after-fairlife-ransomware-attack/) | 28.0 | 30.0 | 42.0 |
| [RansomwareグループによるEDR無効化技術の悪用拡大](https://www.infosecurity-magazine.com/news/ransomware-q2-2026-edr-kill/) | 28.0 | 30.0 | 42.0 |
| [イランのPLC悪用キャンペーンが米国の重要インフラを標的にする](https://blog.polyswarm.io/iranian-plc-exploitation-campaign-targets-us-critical-infrastructure) | 28.0 | 20.0 | 42.0 |
| [マルウェアの影響でサウスカロライナ州とジョージア州の医療システムがオフィスを閉鎖](https://therecord.media/health-system-south-carolina-georgia-disruptions-malware) | 28.0 | 20.0 | 42.0 |
| [Googleのハッカー名混同対策？ またしても新しい命名システム](https://cyberscoop.com/google-threat-actor-naming-system/) | 28.0 | 20.0 | 42.0 |
| [Dysphoria IoTボットネット、JackSkid遮断後にブロックチェーンC2と被害者リレーを追加](https://thehackernews.com/2026/07/dysphoria-iot-botnet-adds-blockchain-c2.html) | 28.0 | 20.0 | 42.0 |
| [Telegramを狙ったフィッシングキャンペーン、亡命ベラルーシ人活動家やロシア人、カザフスタン人を標的に](https://therecord.media/telegram-belarus-activist-russia-cyberattack) | 28.0 | 20.0 | 42.0 |
| [Googleがサイバー脅威アクターの命名方法を変更](https://www.helpnetsecurity.com/2026/07/27/google-threat-actors-naming-system/) | 28.0 | 20.0 | 42.0 |
| [MedusaHVNCマルウェアが隠しWindowsデスクトップを使って検知を回避](https://www.securityweek.com/medusahvnc-malware-uses-hidden-windows-desktops-to-evade-detection/) | 28.0 | 20.0 | 42.0 |
| [偽のTeams更新を用いてLevel RMMとScreenConnectを展開するOperation BlueDash](https://thehackernews.com/2026/07/operation-bluedash-deploys-level-rmm.html) | 28.0 | 20.0 | 42.0 |
| [SourTradeのマルバタイジングキャンペーンがブラウザー上で密かにマルウェアを生成](https://www.infosecurity-magazine.com/news/malvertising-builds-malware-in/) | 28.0 | 20.0 | 42.0 |
| [Cruciferra CrypterがBYOVDとプロセスゴースティングでWindowsマルウェアを隠蔽](https://thehackernews.com/2026/07/cruciferra-crypter-uses-byovd-and.html) | 28.0 | 20.0 | 42.0 |
| [侵害された公開Wi-Fiゲートウェイを用いた企業認証情報の窃取](https://www.securityweek.com/hacked-public-wi-fi-gateways-used-to-harvest-corporate-credentials/) | 28.0 | 20.0 | 42.0 |
| [TELESHIMがTelegramをC2に悪用し中東政府を標的に攻撃](https://thehackernews.com/2026/07/teleshim-abuses-telegram-for-c2-in.html) | 28.0 | 20.0 | 42.0 |
| [グローバルAIレッドチーミングによるAIセキュリティ強化](https://www.microsoft.com/en-us/security/blog/2026/07/27/enhancing-ai-security-through-global-ai-red-teaming/) | 27.0 | 20.0 | 42.0 |
| [AIのトークン価格を10分の1にできる「プロンプトキャッシュ」の仕組みとは？](https://gigazine.net/news/20260727-prompt-caching/) | 27.0 | 20.0 | 42.0 |
| [AIがHugging FaceをハッキングしていたことにOpenAIは1週間気づかなかったと関係者が明かす](https://gigazine.net/news/20260727-ai-hacking-notice/) | 27.0 | 20.0 | 42.0 |
| [Z世代に聞く次の流行、「AIイラスト」が1位に 「Claude Code」も上位](https://www.itmedia.co.jp/news/articles/2607/27/news092.html) | 26.0 | 20.0 | 42.0 |
| [MicrosoftがMAI-Cyber-1-Flashを発表、コスト半減のサイバーセキュリティAIを約束](https://www.helpnetsecurity.com/2026/07/27/microsoft-mai-cyber-1-flash-ai-model/) | 25.0 | 20.0 | 42.0 |
| [OpenAIとHugging Faceへの攻撃を受け、テック大手がオープンAIモデルを支持](https://www.theregister.com/ai-and-ml/2026/07/27/tech-giants-link-hands-to-praise-open-ai-models-after-openai-hugging-face-attack/5279061) | 25.0 | 20.0 | 42.0 |
| [今あるDLPでオープンソースAIエージェントを安全に守る方法](https://www.security.com/product-insights/secure-open-source-ai-agents-dlp-you-have-now) | 25.0 | 20.0 | 42.0 |
| [IT業界大手、米国はAIで開放性と透明性を受け入れるべきと主張](https://www.cybersecuritydive.com/news/ai-open-source-weights-tech-industry-promote/826240/) | 25.0 | 20.0 | 42.0 |
| [テック大手、サイバー防御者向けにオープンAIを提供するため連携](https://www.helpnetsecurity.com/2026/07/27/nvidia-open-secure-ai-alliance/) | 25.0 | 20.0 | 42.0 |
| [Weekly Recap: Rogue AI Agents、Check Pointの脆弱性悪用、Slopsquatting、ClickFix誘導などの最新動向](https://thehackernews.com/2026/07/weekly-recap-rogue-ai-agents-check.html) | 25.0 | 20.0 | 42.0 |
| [Shadow AIエージェントの増加：見つけて保護する方法](https://www.bleepingcomputer.com/news/security/shadow-ai-agents-are-multiplying-heres-how-to-find-and-secure-them/) | 25.0 | 20.0 | 42.0 |
| [Dynatrace IntelligenceがAIエージェントでインシデントの切り分けと修復を自動化](https://www.helpnetsecurity.com/2026/07/27/dynatrace-intelligence/) | 25.0 | 20.0 | 42.0 |
| [Zenity、Runtime BoundariesでAIガバナンスを強化](https://www.helpnetsecurity.com/2026/07/27/zenity-exposure-management-runtime-boundaries/) | 25.0 | 20.0 | 42.0 |
| [JetStream Securityが侵害されたAIエージェントをオンデマンドで停止可能にする機能を提供](https://www.helpnetsecurity.com/2026/07/27/jetstream-ai-kill-switch/) | 25.0 | 20.0 | 42.0 |
| [7AI、Federated SIEMとAIワークフロービルダーを追加しプラットフォームを拡張](https://www.helpnetsecurity.com/2026/07/27/7ai-expands-platform-with-federated-siem-and-ai-workflow-builder/) | 25.0 | 20.0 | 42.0 |
| [C1、アイデンティティガバナンスプラットフォームにシャドーAI検出機能を追加](https://www.helpnetsecurity.com/2026/07/27/c1-adds-shadow-ai-discovery-to-its-identity-governance-platform/) | 25.0 | 20.0 | 42.0 |
| [Booz AllenがAI駆動の脅威検知プラットフォームでVellox Suiteを拡張](https://www.helpnetsecurity.com/2026/07/27/booz-allen-hamilton-vellox-ranger/) | 25.0 | 20.0 | 42.0 |
| [OpenAI攻撃を受け、Hugging Face CEOが「徹底した透明性」を要求](https://www.itpro.com/security/hugging-face-ceo-calls-for-radical-transparency-in-wake-of-openai-attack) | 25.0 | 20.0 | 42.0 |
| [「生成AIは友人」増 活用か依存か](https://news.yahoo.co.jp/pickup/6589523?source=rss) | 25.0 | 20.0 | 42.0 |
| [AnthropicのOpus 5はバグ発見でMythos 5に迫るも、エクスプロイトでは及ばず](https://www.securityweek.com/anthropics-opus-5-nears-mythos-5-on-finding-bugs-but-falls-short-on-exploits/) | 25.0 | 20.0 | 42.0 |
| [AWSがDevOpsチーム向けにファイアウォールインシデントを調査するAIアシスタントを提供](https://www.helpnetsecurity.com/2026/07/27/aws-devops-agent-network-firewall-troubleshooting/) | 25.0 | 20.0 | 42.0 |
| [AIセキュリティについてトロイの木馬が正しい点と誤っている点](https://www.cybersecuritydive.com/spons/what-the-trojan-horse-gets-right-and-wrong-about-ai-security/825935/) | 25.0 | 20.0 | 42.0 |
| [Mythos時代では、セキュリティはランタイムにある](https://www.cybersecuritydive.com/spons/in-the-mythos-era-security-belongs-at-runtime/825478/) | 25.0 | 20.0 | 42.0 |
| [Patched済みvBulletinの認証前コード実行脆弱性に対するPoC公開](https://thehackernews.com/2026/07/public-exploit-released-for-patched.html) | 24.0 | 38.0 | 42.0 |
| [フィッシング被害後、攻撃の踏み台に - スペース](https://www.security-next.com/186979) | 22.0 | 20.0 | 42.0 |
| [子会社SMS配信システムにサイバー攻撃 - ファブリカHD](https://www.security-next.com/187370) | 22.0 | 20.0 | 42.0 |
| [Java Spring Boot の「heapdump」スキャン、（7月27日月曜日）](https://isc.sans.edu/diary/rss/33188) | 22.0 | 20.0 | 42.0 |
| [検索結果に「詐欺ではありません」と表示させる詐欺手口、警視庁が注意喚起 AI要約も餌食に](https://www.itmedia.co.jp/news/articles/2607/27/news076.html) | 21.0 | 20.0 | 42.0 |
| [n8nのサンドボックスエスケープにより、ワークフロー編集者がn8nプロセスとしてOSコマンドを実行可能に](https://thehackernews.com/2026/07/n8n-sandbox-escape-lets-workflow.html) | 20.0 | 28.0 | 50.0 |
| [ShinyHuntersによるErnst & Youngのデータ侵害の主張](https://www.bleepingcomputer.com/news/security/ernst-and-young-data-breach-claimed-by-shinyhunters-extortion-gang/) | 20.0 | 20.0 | 42.0 |
| [ShinyHuntersのデータ流出を悪用するセクストーション詐欺師たち](https://www.malwarebytes.com/blog/scams/2026/07/sextortion-scammers-are-exploiting-shinyhunters-data-leaks) | 20.0 | 20.0 | 42.0 |
| [ダークウェブであなたのデータはいくらで売られるのか（Lock and Code S07E15）](https://www.malwarebytes.com/blog/podcast/2026/07/whats-your-data-worth-on-the-dark-web-lock-and-code-s07e15) | 20.0 | 20.0 | 42.0 |
| [GitHubとPyPIの新ポリシーでサプライチェーンセキュリティを強化](https://www.securityweek.com/new-github-pypi-policies-boost-supply-chain-security/) | 20.0 | 20.0 | 42.0 |
| [Microsoft Defender for Endpointの更新後、一部のLinux環境が無防備に](https://www.theregister.com/patches/2026/07/27/microsoft-defender-for-endpoint-leaves-some-linux-boxes-defenseless-after-update/5278914) | 20.0 | 20.0 | 42.0 |
| [Wyden上院議員、古い脆弱な公開VPNの廃止を連邦政府に要請](https://cyberscoop.com/wyden-calls-for-federal-legacy-vpn-purge-zero-trust/) | 20.0 | 20.0 | 42.0 |
| [ChatGPTがフィッシング攻撃で最もなりすまされるブランドに加わる](https://www.helpnetsecurity.com/2026/07/27/check-point-brand-phishing-trends-report/) | 20.0 | 20.0 | 42.0 |
| [Beelzebub、ハッカーを誘い込むプラットフォーム向けに340万ドルを調達](https://www.securityweek.com/beelzebub-raises-3-4-million-for-hacker-trapping-platform/) | 20.0 | 20.0 | 42.0 |
| [モバイルアプリの中に何が隠れているのか？Lookout MSECが解明へ](https://www.securityweek.com/whats-hiding-in-your-mobile-apps-lookout-msec-aims-to-find-out/) | 20.0 | 20.0 | 42.0 |
| [企業の量子耐性暗号への移行が遅れている、今収集今解読攻撃で将来コスト増の恐れ](https://www.itpro.com/security/enterprises-arent-moving-fast-enough-on-post-quantum-cryptography-preparations-harvest-now-decrypt-later-attacks-mean-it-could-cost-them) | 20.0 | 20.0 | 42.0 |
| [DentaQuestのデータ漏えい、2,300万人超に影響の可能性](https://www.securityweek.com/dentaquest-data-breach-potentially-impacts-over-23-million-people/) | 20.0 | 20.0 | 42.0 |
| [GitHub、毒入りパッケージの採用を抑えるためDependabotに3日間のクールダウンを追加](https://thehackernews.com/2026/07/github-adds-3-day-dependabot-cooldown.html) | 20.0 | 20.0 | 42.0 |

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
