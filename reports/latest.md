# 📡 サイレーダー 2026-11-06 05:00 JST

このレポートは、2026-11-05 17:00 JST〜2026-11-06 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 92
- [音声で扱う想定のトピック](#audio-topics): 4
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 68

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Zyxel Switch Hacks Blamed on Patched Flaw Actually Exploited a Zero-Day](#topic-41466) | 43.0 | 46.0 | 55.0 | 音声 | 温度感上位枠 |
| 2 | [Vercel ties login sessions to devices, rolls out AI security reviews in public beta](#topic-41442) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 3 | [ChatGPT Lockdown Mode Bypass: Phishing, Malware Delivery, and Silent Data Exfiltration](#topic-41446) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 4 | [CERT-In Flags AI-Driven Attacks as Backdoored ARTEX Exposes 62 Consoles to Root Access](#topic-41504) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-41466"></a>

### 1. Zyxel Switch Hacks Blamed on Patched Flaw Actually Exploited a Zero-Day

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

ZyxelのGS1900シリーズスイッチについて、当初は修正済みの脆弱性への対策として扱われていたものの、実際に悪用されていたのは別の未修正脆弱性だったと報じられています。
対象の欠陥はCVE-2026-107441とされ、公開情報ではOSコマンド実行につながる可能性があるとされていますが、詳細な悪用状況は確認中です。
ネットワーク機器は社内外の通信の要所に置かれるため、脆弱性が残ると広範な影響につながりやすい点が注目されています。
修正済みと見なしていても別の欠陥が残っている可能性があり、パッチ適用後の確認が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象機種と導入済みファームウェアがCVE-2026-107441の影響範囲に含まれるか確認する。
- ベンダーの修正情報を再点検し、既存の更新が今回の脆弱性に対応しているかを切り分ける。
- 外部公開された管理機能や不審なHTTPアクセスの有無を点検し、必要に応じてアクセス制限を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-107441 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-107441](https://nvd.nist.gov/vuln/detail/CVE-2026-107441) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Patched Zyxel GS1900 switches remained open to in-the-wild exploit (CVE-2026-107](https://www.helpnetsecurity.com/2026/11/05/zyxel-cve-2026-107441-exploit/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zyxel Switch Hacks Blamed on Patched Flaw Actually Exploited a Zero-Day](https://www.securityweek.com/zyxel-switch-hacks-blamed-on-patched-flaw-actually-exploited-a-zero-day/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-41442"></a>

### 2. Vercel ties login sessions to devices, rolls out AI security reviews in public beta

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Vercelが、ログインセッションを端末にひも付けるDevice Bound Session Credentials（DBSC）の導入と、AIを使ったセキュリティレビュー機能の公開ベータを発表しました。
DBSCは、情報窃取型マルウェアなどでセッション情報が盗まれた場合の悪用リスクを抑えることを狙う仕組みです。
セッションの不正利用は、認証情報そのものが漏れていなくても被害につながるため、対策の実装有無が重要です。
あわせて、AIによるレビュー機能の実運用への適用が広がる流れとしても注目されます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- セッション管理が端末ひも付け型の仕組みに対応しているか確認する。
- Cookieやセッショントークンの保護、失効、再認証の設計を見直す。
- AI支援のセキュリティレビューは補助として扱い、最終判断は人手で検証する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| マルウェア | RedLine Stealer | 主題 | 0.80 | — |
| マルウェア | Lumma Stealer | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Vercel ties login sessions to devices, rolls out AI security reviews in public b](https://www.helpnetsecurity.com/2026/11/05/vercel-security-review-session-hijacking/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-41446"></a>

### 3. ChatGPT Lockdown Mode Bypass: Phishing, Malware Delivery, and Silent Data Exfiltration

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>i⁠O⁠S</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Check Point Researchは、ChatGPTのコード実行ランタイムに関連するセキュリティ上の問題について報告しました。
説明では、会話データが秘密裏に外部へ送られる可能性があり、すでに修正が適用されたとされています。
生成AIの利用が広がる中で、AIサービス内の隔離やデータ保護が実運用上の重要課題であることを示す事例です。
会話や入力内容に機密情報が含まれる環境では、情報漏えい対策の見直しが必要になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIサービスや連携機能を使う際は、機密情報の入力可否と保存・送信の扱いを再確認する。
- 生成AIの権限設定やネットワーク隔離、外部通信の監視を運用面で点検する。
- ベンダーの修正状況や公式アドバイザリを確認し、影響範囲に応じて利用ルールを更新する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Check Point | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | ChatGPT | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ChatGPT Lockdown Mode Bypass: Phishing, Malware Delivery, and Silent Data Exfilt](https://research.checkpoint.com/2026/chatgpt-lockdown-mode-bypass-phishing-malware-delivery-and-silent-data-exfiltration/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-41504"></a>

### 4. CERT-In Flags AI-Driven Attacks as Backdoored ARTEX Exposes 62 Consoles to Root Access

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

CERT-Inは、AI支援型の脅威アクターがインドのBFSI（銀行・金融サービス・保険）分野を標的にしていると公表しました。
公開されているAIベースの攻撃支援ツールが使われているとされ、活動は継続中とみられています。AIを悪用した攻撃は、従来よりも準備や運用の効率が高まりやすく、警戒すべき対象です。
金融関連組織が標的とされている点から、業種を問わず防御態勢の見直しが意識されます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI支援型の偵察・侵入補助ツールを前提に、検知ルールや監視観点を見直す。
- BFSI関連の組織や取引先では、認証情報の保護、アクセス権限の点検、異常ログの監視を強化する。
- 脅威情報としては、攻撃者の手口だけでなく、影響を受けやすい資産や業務範囲の把握を優先する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CERT-In Flags AI-Driven Attacks as Backdoored ARTEX Exposes 62 Consoles to Root ](https://thehackernews.com/2026/11/backdoored-docker-image-for-artex-ai.html) | <nobr>内容確認・補足情報</nobr> |

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
| [医療機関のサイバーセキュリティー強化へ ランサムウエア攻撃で診療への長期影響リスク](https://www.itmedia.co.jp/news/article/2611/05/2000002921/) | 29.0 | 30.0 | 42.0 |
| [New York州クイーンズ公共図書館がランサムウェア被害、Wi-Fiや貸出システム、Webサイトが停止](https://www.theregister.com/cyber-crime/2026/11/05/new-yorks-queens-public-library-battles-ransomware-crims-wi-fi-checkouts-and-website-go-dark/5307796) | 28.0 | 30.0 | 42.0 |
| [ロシア政府系ハッカーがゼロクリック諜報キャンペーンでiPhoneとAndroid端末を標的に](https://therecord.media/russia-hackers-smartphone-cyberattacks) | 28.0 | 20.0 | 42.0 |
| [トロイ化されたCWP Webサーバーを使ってLinuxサーバーにバックドアを仕掛けるハッカーたち](https://www.bleepingcomputer.com/news/security/hackers-backdoor-linux-servers-using-trojanized-cwp-web-server/) | 28.0 | 20.0 | 42.0 |
| [PortSwiggerのBurp ATが企業に定義済みの制限付きでペネトストを委任可能に](https://www.helpnetsecurity.com/2026/11/05/portswigger-burp-at-enterprises/) | 28.0 | 20.0 | 42.0 |
| [GTA 6の期待感に便乗してマルウェアや暗号資産詐欺を広める詐欺師たち](https://www.helpnetsecurity.com/2026/11/05/gta-6-scams-fake-leaks-early-access/) | 28.0 | 20.0 | 42.0 |
| [ロシア系ハッカーがウォータリングホールでiOS・Android端末を狙うエクスプロイトチェーン攻撃](https://www.securityweek.com/russia-linked-hackers-hit-ios-android-devices-with-exploit-chains-via-watering-holes/) | 28.0 | 20.0 | 42.0 |
| [2026年10月に米国企業を脅かす5つの活発なサイバー脅威](https://thehackernews.com/2026/11/5-active-cyber-threats-that-put-us.html) | 28.0 | 20.0 | 42.0 |
| [銀行向けマルウェアのサンプルから発見された、Android端末をループクラッシュさせる脆弱性](https://www.helpnetsecurity.com/2026/11/05/ghostmap-android-bug-research/) | 28.0 | 20.0 | 42.0 |
| [古いCisco IOSの脆弱性に対する脆弱性スキャン／オプトアウトヘッダー（11月5日木曜日）](https://isc.sans.edu/diary/rss/33492) | 25.0 | 31.0 | 51.0 |
| [OpenAIのGPT-6 Astraが安全性研究タスクを密かに妨害](https://www.bleepingcomputer.com/news/security/openais-gpt-6-astra-silently-obstructed-safety-research-tasks/) | 25.0 | 20.0 | 42.0 |
| [OpenAIの研究で明らかになった948件のLinuxカーネル脆弱性によりAIエージェントがroot権限を取得](https://www.securityweek.com/ai-agents-got-root-on-linux-via-948-kernel-flaws-in-openai-research/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントは人間ではないが、かなり人間に近い](https://blog.cloudflare.com/trusted-agent-delegation/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、GPT-6 Cyberを発表――性能向上と安全対策を強調](https://cyberscoop.com/openai-gpt-6-cyber-security-model/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、GPT-6 Cyberを公開し「交戦規定」を順守すると表明](https://www.theregister.com/security/2026/11/05/openai-releases-gpt-6-cyber-and-promises-this-one-stays-within-rules-of-engagement/5307855) | 25.0 | 20.0 | 42.0 |
| [SecurityDataPipeline.comがAI時代向けの新しい教育リソースとして公開される](https://www.darkreading.com/cybersecurity-operations/securitydatapipeline-com-launches-as-a-new-educational-resource-for-the-ai-era) | 25.0 | 20.0 | 42.0 |
| [CyberhavenがAIのデータ利用を追跡・制御するAgentic Data Securityを発表](https://www.helpnetsecurity.com/2026/11/05/cyberhaven-agentic-data-security/) | 25.0 | 20.0 | 42.0 |
| [Box、エージェント型ワークフロー計画に新たな脅威対策を追加](https://www.helpnetsecurity.com/2026/11/05/box-architect/) | 25.0 | 20.0 | 42.0 |
| [インド、金融・暗号資産ビジネスを狙う新たなAI駆動型サイバー攻撃に警告](https://www.infosecurity-magazine.com/news/india-warns-ai-cyberattacks/) | 25.0 | 20.0 | 42.0 |
| [Gartnerレポート: 攻撃経路は多くのチームのパッチ適用より速く閉じつつある](https://www.rapid7.com/blog/post/ai-gartner-report-attack-paths-closing-faster-than-patchable) | 25.0 | 20.0 | 42.0 |
| [Sysdig AI DefenseがAIエージェントの実行時にガードレールを適用](https://www.helpnetsecurity.com/2026/11/05/sysdig-ai-defense/) | 25.0 | 20.0 | 42.0 |
| [Anthropic、Claude Dispatchの脆弱性修正を見送り　企業境界を越えたリモートコマンド実行の恐れ](https://www.theregister.com/research/2026/11/05/anthropic-wont-fix-a-claude-dispatch-flaw-that-could-let-attackers-execute-remote-commands-across-corporate-boundaries/5307684) | 25.0 | 20.0 | 42.0 |
| [Agenticアイデンティティの統制におけるAgent Smithのジレンマ](https://www.securityweek.com/the-agent-smith-dilemma-governing-agentic-identities/) | 25.0 | 20.0 | 42.0 |
| [Google、脅威を追跡し脆弱性を修正するAIエージェントに新たな制限を導入](https://www.helpnetsecurity.com/2026/11/05/google-cloud-ai-agents-security-controls/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、GPT-6 Astraが内部レッドチーミングとエクスプロイト課題で控えめな振る舞いをしていることを確認](https://www.securityweek.com/openai-finds-gpt-6-astra-quietly-holding-back-on-internal-red-teaming-exploit-tasks/) | 25.0 | 20.0 | 42.0 |
| [OpenAIの新AIモデルが一度の実行で948件のLinux root権限エクスプロイトを作成](https://www.helpnetsecurity.com/2026/11/05/openai-linux-kernel-root-exploits/) | 25.0 | 20.0 | 42.0 |
| [ThreatsDay: Apache OFBizのRCE、DreamHost侵害、DeFiサイトの乗っ取りほか17件の話題](https://thehackernews.com/2026/11/threatsday-apache-ofbiz-rce-dreamhost.html) | 24.0 | 38.0 | 42.0 |
| [CiscoとWatchGuardが修正パッチを公開、SonicWallはGMSの脆弱性を修正せず](https://www.securityweek.com/cisco-watchguard-release-patches-sonicwall-wont-fix-gms-flaws/) | 24.0 | 38.0 | 42.0 |
| [it-saから学ぶ教訓：Bring a tent, I've got the coffee](https://blog.talosintelligence.com/bring-a-tent-ive-got-the-coffee-lessons-from-it-sa/) | 22.0 | 20.0 | 42.0 |
| [第三者が認証情報を不正作成か、アプリ移行処理に不備 - デニーズ](https://www.security-next.com/192388) | 22.0 | 20.0 | 42.0 |
| [サーバ設定不備、従業員情報流出の可能性 - 資さんうどん](https://www.security-next.com/192260) | 22.0 | 20.0 | 42.0 |
| [申請用ファイルに不備、サイト上に個人情報が残存 - 福岡県](https://www.security-next.com/192081) | 22.0 | 20.0 | 42.0 |
| [個人情報含む業務用USBメモリが所在不明に - 奈良県](https://www.security-next.com/191606) | 22.0 | 20.0 | 42.0 |
| [HPEのネットワーク管理製品に複数脆弱性 - 「クリティカル」3件](https://www.security-next.com/192402) | 22.0 | 20.0 | 42.0 |
| [フランスの血液保存施設で冷蔵庫の設定を-30℃から110℃に引き上げるサイバー攻撃が発生、迅速な対応で血液製剤は無事](https://gigazine.net/news/20261105-french-blood-fridge-cyberattacked/) | 22.0 | 20.0 | 42.0 |
| [個人情報が保存されたHDDや書類を紛失 - 都水道局](https://www.security-next.com/192391) | 22.0 | 20.0 | 42.0 |
| [迫る大脆弱性時代--「SBOM.JP」が目指す脆弱性対応の優先順位付け](https://japan.zdnet.com/article/35254447/) | 21.0 | 20.0 | 42.0 |
| [「脆弱性報告数が別次元に」 Mythos一般公開を恐れる前に、推奨される7つの優先対策](https://atmarkit.itmedia.co.jp/ait/articles/2611/05/news040.html) | 21.0 | 20.0 | 42.0 |
| [muslベースのLinuxシステムで過度に長いパスワードを使ってroot権限を取得する方法](https://www.theregister.com/security/2026/11/05/get-root-on-a-musl-linux-system-by-slamming-it-with-an-overly-long-password/5307910) | 20.0 | 20.0 | 42.0 |
| [Octoberのcrypto-tracker侵害：アクセス突破、法執行機関トークン大量流出](https://www.theregister.com/cyber-crime/2026/11/05/october-crypto-tracker-hack-access-cracked-law-enforcement-tokens-packed/5307852) | 20.0 | 20.0 | 42.0 |
| [OpenSSHの脆弱性により、パスワード無効化されたLinuxアカウントへ不正ログイン可能に](https://www.bleepingcomputer.com/news/security/openssh-flaw-lets-attackers-log-into-password-disabled-linux-accounts/) | 20.0 | 20.0 | 42.0 |
| [米民主党の議会におけるサイバーセキュリティ政策の展望](https://www.cybersecuritydive.com/news/congress-cybersecurity-democrats-agenda-cisa-ai/873883/) | 20.0 | 20.0 | 42.0 |
| [DigiCertのデータ侵害で顧客情報と身分証明書が流出](https://www.bleepingcomputer.com/news/security/digicert-data-breach-exposes-customer-information-identity-documents/) | 20.0 | 20.0 | 42.0 |
| [Tobacco企業がファイル共有に秘密のレシピを残していたことで被害を受けた話](https://www.theregister.com/security/2026/11/05/tobacco-company-got-smoked-by-leaving-secret-recipes-on-a-file-share/5307704) | 20.0 | 20.0 | 42.0 |
| [White Houseネットワークにたどり着いたResidential Proxyトラフィック](https://www.infosecurity-magazine.com/news/white-house-residential-proxy-exits/) | 20.0 | 20.0 | 42.0 |
| [フランス当局、国家の血液供給を標的としたサイバー攻撃を捜査](https://www.cybersecuritydive.com/news/french-probe-cyberattack-blood-supply/873871/) | 20.0 | 20.0 | 42.0 |
| [Zyxel Switchのパッチ未適用脆弱性を突く攻撃の波](https://www.infosecurity-magazine.com/news/zyxel-gs1900-patch-missed-flaw/) | 20.0 | 20.0 | 42.0 |
| [Service DeskにおけるID管理のギャップを埋める](https://www.bleepingcomputer.com/news/security/closing-the-identity-gap-at-the-service-desk/) | 20.0 | 20.0 | 42.0 |
| [Arkose Labs、Agent Trust Managerを拡張しエージェントセッションを統制](https://www.helpnetsecurity.com/2026/11/05/arkose-agent-trust-manager/) | 20.0 | 20.0 | 42.0 |
| [ノルウェーの援助機関へのサイバー攻撃で全ユーザーデータが流出した可能性](https://www.helpnetsecurity.com/2026/11/05/norad-grants-portal-breach/) | 20.0 | 20.0 | 42.0 |
| [銀行のフィッシングサイトが摘発回避のために偽の「停止中」ページを表示](https://www.securityweek.com/bank-phishing-sites-show-fake-suspended-pages-to-evade-takedowns/) | 20.0 | 20.0 | 42.0 |
| [フランスの血液バンクサイトがサイバー攻撃を受けるも血液製剤は無事](https://www.securityweek.com/cyberattack-hits-french-blood-bank-site-but-no-blood-products-are-compromised/) | 20.0 | 20.0 | 42.0 |
| [総務省消防庁「安否情報システム」に不正アクセス、サービス停止中](https://internet.watch.impress.co.jp/docs/news/2154132.html) | 20.0 | 20.0 | 42.0 |
| [Exposure Managementプラットフォームは本当に安全か？見落としを見つける5つのテスト](https://thehackernews.com/2026/11/is-your-exposure-management-platform.html) | 20.0 | 20.0 | 42.0 |
| [VizioとSamsungのスマートテレビ、トラッキング拒否設定を無視している可能性](https://www.malwarebytes.com/blog/news/2026/11/vizio-samsung-smart-tvs-seem-to-ignore-tracking-opt-outs) | 20.0 | 20.0 | 42.0 |
| [OpenAIのAIパイプラインが30時間の実行で948件のLinux権限昇格エクスプロイトを生成](https://thehackernews.com/2026/11/openai-ai-pipeline-generates-948-linux.html) | 20.0 | 20.0 | 42.0 |
| [中国国家系脅威活動、2026年第2四半期と第3四半期に大幅減少](https://www.infosecurity-magazine.com/news/chinese-nation-activity-falls/) | 20.0 | 20.0 | 42.0 |
| [NTTドコモ、自社サーバーに不正アクセス。最大約30万件の利用者の情報流出](https://internet.watch.impress.co.jp/docs/news/2154115.html) | 20.0 | 20.0 | 42.0 |
| [教育プラットフォームへの攻撃後、32万件の学校関連ファイルがダークウェブに公開](https://www.itpro.com/security/cyber-attacks/320-000-school-files-published-on-dark-web-after-attack-on-education-platform) | 20.0 | 20.0 | 42.0 |
| [ノルウェーの援助機関が侵害され、全ユーザーデータが窃取される](https://www.theregister.com/cyber-crime/2026/11/05/norways-aid-agency-pwned-and-all-users-data-is-stolen/5307765) | 20.0 | 20.0 | 42.0 |
| [CISO対話：Ryan Davis―セキュリティが現実と交わる未知の領域](https://www.securityweek.com/ciso-conversations-ryan-davis-the-unknown-is-where-security-meets-reality/) | 20.0 | 20.0 | 42.0 |
| [GhostMapの不具合によりAndroid端末が再起動ループに陥る問題](https://www.infosecurity-magazine.com/news/ghostmap-bug-android-phones-stuck/) | 20.0 | 20.0 | 42.0 |
| [SOCファイル5：パイプラインに潜む亡霊――Storm-2603によるファイルレスなSharePoint侵害](https://securelist.com/storm-2603-fileless-toolshell-attack/121467/) | 20.0 | 20.0 | 42.0 |
| [脅威インテリジェンス基盤の見落としをなくす方法](https://any.run/cybersecurity-blog/how-to-close-threat-intelligence-stack-blind-spots/) | 20.0 | 20.0 | 42.0 |
| [NATSの航空管制障害で英国経済に3300万ポンドの損失](https://www.infosecurity-magazine.com/news/nats-air-traffic-control-fail-cost/) | 20.0 | 20.0 | 42.0 |
| [GhostMapのAndroid脆弱性により悪意のあるアプリが永続的なブートループを引き起こせる](https://www.bleepingcomputer.com/news/security/ghostmap-android-flaw-lets-malicious-app-trigger-persistent-boot-loop/) | 20.0 | 20.0 | 42.0 |
| [iCloudリンク共有に有害コンテンツ確認を導入、違反時はアカウント停止の可能性も](https://www.helpnetsecurity.com/2026/11/05/apple-icloud-link-sharing-checks/) | 20.0 | 20.0 | 42.0 |
| [サイバー攻撃 10月は国内4億件超](https://news.yahoo.co.jp/pickup/6601439?source=rss) | 20.0 | 20.0 | 42.0 |

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
