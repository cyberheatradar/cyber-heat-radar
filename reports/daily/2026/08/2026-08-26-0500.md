# 📡 サイレーダー 2026-08-26 05:00 JST

このレポートは、2026-08-25 17:00 JST〜2026-08-26 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 91
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 62

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Unpatched Zimbra servers are falling to CVE-2026-73570 attacks](#topic-28581) | 45.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 2 | [CVE-2026-60004: CISA KEV catalog addition](#topic-29270) | 45.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 3 | [Australia Warns of Active Exploitation of Critical TeamCity Server Flaw](#topic-29282) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Fake OpenAI Codex download tricks macOS users into installing malware](#topic-29264) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [The State of AI-Enabled Malware August 2026: From Brand Abuse to Agentic Execution](#topic-29295) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-28581"></a>

### 1. Unpatched Zimbra servers are falling to CVE-2026-73570 attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Zimbra Collaboration（ZCS）に存在した既知の脆弱性CVE-2026-73570について、未適用のサーバーが実際に攻撃対象になっていると複数の情報源が伝えています。
公的機関の注意喚起や各社報道では、コマンドインジェクションによりリモートコード実行につながる可能性があるとして、すでに修正済みの更新適用が重要とされています。
メールやグループウェアは業務の中核にあるため、侵害されると情報漏えいや広範な業務影響につながりやすい点が注目されています。
さらに、既知の悪用が観測されているため、一般的な脆弱性対応よりも迅速な更新と棚卸しが求められます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Zimbra Collaboration の該当バージョンを使っているか確認し、修正版の適用状況を優先的に点検する。
- インターネット公開されている Zimbra サーバーを洗い出し、未更新・保守切れのものがないか確認する。
- 不審な認証や設定変更、通信の増加など侵害の兆候がないか、関連ログを重点的に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-73570 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Zimbra | 言及あり | 0.80 | — |
| 製品 | Zimbra Collaboration | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-73570](https://nvd.nist.gov/vuln/detail/CVE-2026-73570) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Unpatched Zimbra servers are falling to CVE-2026-73570 attacks](https://www.helpnetsecurity.com/2026/08/25/zimbra-cve-2026-73570-compromised/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Exploited Zimbra Flaw Highlights Shrinking Window to Patch](https://www.darkreading.com/vulnerabilities-threats/zimbra-flaw-exploitation-shrinking-window-patch) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/08/21/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit Zimbra SNMP Flaw for Unauthenticated Remote Code Execution](https://thehackernews.com/2026/08/attackers-exploit-zimbra-snmp-flaw-for.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA orders agencies to fix exploited Zimbra vulnerability](https://www.cybersecuritydive.com/news/cisa-zimbra-flaw-patch-mandate-kev/828718/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-29270"></a>

### 2. CVE-2026-60004: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

CISAは、実際の悪用が確認されたとして、CVE-2026-60004をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
対象はGiteaのコードインジェクション脆弱性とされています。KEV入りは、単なる脆弱性情報ではなく、優先度を上げて対処すべき対象であることを示します。
公開資産を含む環境では、影響確認と修正対応の遅れが被害拡大につながるおそれがあります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Giteaの利用有無と公開状況を確認し、該当バージョンの影響を評価する。
- 修正パッチや緩和策の適用を優先し、関連資産の対応状況を棚卸しする。
- 悪用済みの可能性を考慮し、認証情報や設定変更の有無、ログの異常を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-60004 | 関連CVE | 1.00 | 候補あり（URL 8件以上） |
| 製品 | Gitea | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-60004](https://nvd.nist.gov/vuln/detail/CVE-2026-60004) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/08/25/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-29282"></a>

### 3. Australia Warns of Active Exploitation of Critical TeamCity Server Flaw

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

オーストラリア当局が、TeamCityサーバーの重大な脆弱性について、実際の悪用が確認されているとして利用者に速やかな修正を呼びかけています。
米国政府による同様の警告に続くもので、少なくとも公開情報上では注意喚起の緊急性が高い状況です。
攻撃者による悪用が観測されている脆弱性は、対応の遅れがそのまま侵害リスクにつながります。
CI/CD基盤であるTeamCityが影響を受けると、開発・ビルド環境全体に波及する可能性があるため注目されています。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- TeamCityの該当製品・該当バージョンを確認し、ベンダーの修正済み版や緩和策を早急に適用する。
- インターネット公開されているTeamCityサーバーは優先的に棚卸しし、不要な露出やアクセス制限を見直す。
- 監査ログや認証関連の異常、想定外の管理操作の有無を点検し、侵害の兆候がないか確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Australia Warns of Active Exploitation of Critical TeamCity Server Flaw](https://www.infosecurity-magazine.com/news/australia-exploitation-teamcity/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-29264"></a>

### 4. Fake OpenAI Codex download tricks macOS users into installing malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

OpenAI CodexのmacOS向けダウンロードを装った偽ページと検索広告を使い、利用者に不正な操作をさせてマルウェアに誘導するキャンペーンが報告されています。
報告では、ファイルを直接配布するのではなく、ユーザー自身に実行させる手口が使われているとされています。
検索広告や正規サービスを装う手口は、利用者の警戒をすり抜けやすく、企業端末でも被害につながるおそれがあります。
AI関連ツールへの関心の高さが、こうしたなりすましの誘因になりやすい点も注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI関連ツールの入手先は、検索結果や広告ではなく公式案内で確認する。
- macOS端末では、ターミナル実行やコマンド貼り付けを求める不自然な案内に注意する。
- 利用者向けに、スポンサー広告や偽ダウンロードページを見分ける周知を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Active Directory | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | OpenAI | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Fake OpenAI Codex download tricks macOS users into installing malware](https://www.helpnetsecurity.com/2026/08/25/fake-openai-codex-download-macos-users/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-29295"></a>

### 5. The State of AI-Enabled Malware August 2026: From Brand Abuse to Agentic Execution

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報では、AIを悪用したマルウェアに関する脅威動向が整理されており、ブランドの悪用から自律的な実行まで、AI関連の攻撃手法の広がりが論点になっています。
あわせて、既存の行動検知やエンドポイント分析が、AIで作成されたコードを実行前に止めるうえで有効とされています。
生成AIの普及により、攻撃者が作成する不正コードや誘導の見た目が自然になり、従来の見分け方だけでは対応しづらくなる可能性があります。
防御側は、検知・隔離・実行前ブロックなど、挙動ベースの対策を改めて点検する必要があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- エンドポイントでの行動検知と実行前ブロックの有効性を確認する。
- ブランド名やサービス名をかたる不審な誘導に対する監視を強化する。
- AI生成物だからといって安全視せず、既存のマルウェア対策基準で評価する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [The State of AI-Enabled Malware August 2026: From Brand Abuse to Agentic Executi](https://unit42.paloaltonetworks.com/ai-enabled-malware-analysis/) | <nobr>内容確認・補足情報</nobr> |

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
| [偽のOpenAI Codex広告を通じてMacマルウェアを拡散する攻撃者](https://www.theregister.com/security/2026/08/25/crooks-push-mac-malware-through-fake-openai-codex-ads/5291899) | 33.0 | 20.0 | 42.0 |
| [miniOrangeのSAML脆弱性を狙う攻撃者、WordPress管理者権限を取得可能に](https://www.securityweek.com/wordpress-websites-targeted-via-miniorange-plugin-vulnerabilities/) | 30.0 | 46.0 | 54.0 |
| [24のnpmパッケージがunpkgミラーを悪用し、偽のCloudflare CAPTCHAページをホスト](https://thehackernews.com/2026/08/24-npm-packages-abuse-unpkg-mirrors-to.html) | 28.0 | 30.0 | 42.0 |
| [イラン関連のハッカーによる重要インフラ侵害に対する米国の制裁](https://thehackernews.com/2026/08/us-sanctions-iran-linked-hackers-behind.html) | 28.0 | 20.0 | 42.0 |
| [ゼロクリック型メール攻撃：企業が知っておくべきこと](https://www.itpro.com/security/phishing/zero-click-email-attacks-what-businesses-need-to-know) | 28.0 | 20.0 | 42.0 |
| [偽のリクルーター詐欺がモバイル端末上の企業認証情報を狙う](https://www.infosecurity-magazine.com/news/fake-recruiter-scams-corporate/) | 28.0 | 20.0 | 42.0 |
| [Hackersが侵害した270以上のZimbraサーバーへの継続的な攻撃](https://www.bleepingcomputer.com/news/security/hackers-breached-over-270-zimbra-servers-in-ongoing-attacks/) | 28.0 | 20.0 | 42.0 |
| [Mirage2FAの急増、Microsoft 365のログインフローを悪用して米国とEUの4,500社に影響](https://thehackernews.com/2026/08/mirage2fa-surge-hits-4500-us-and-eu.html) | 28.0 | 20.0 | 42.0 |
| [E4delとPINHOLE RATがFTPバナーをマルウェアコマンドの隠し通信路に悪用](https://thehackernews.com/2026/08/e4del-and-pinhole-rats-turn-ftp-banners.html) | 28.0 | 20.0 | 42.0 |
| [カー用ヘッドユニット向けに特化して作られた初のマルウェアがボットネットを形成](https://www.securityweek.com/first-malware-built-specifically-for-car-head-units-fuels-botnet/) | 28.0 | 20.0 | 42.0 |
| [カナダの税金を装った誘導から46カ国に広がった米国発のRMMキャンペーン](https://any.run/cybersecurity-blog/us-campaign-malware-analysis/) | 28.0 | 20.0 | 42.0 |
| [偽のMinecraftクライアントがインフラ停止後もWeedHackマルウェアを配布](https://www.infosecurity-magazine.com/news/fake-minecraft-weedhack-malware/) | 28.0 | 20.0 | 42.0 |
| [ReliaQuest、ShinyHuntersのインシデント後の侵害主張を否定](https://www.infosecurity-magazine.com/news/reliaquest-not-compromised-by/) | 28.0 | 20.0 | 42.0 |
| [AIエージェントの「ハーネス」とは？AIモデルを実際に働かせる4つの仕組み](https://gigazine.net/news/20260825-what-is-harness/) | 27.0 | 20.0 | 42.0 |
| [Anthropicの最上位AIモデル「Claude Fable 5」は企業需要が伸びず苦戦、AI企業のビジネスモデルが覆される可能性も](https://gigazine.net/news/20260825-anthropic-best-ai-model-struggles/) | 27.0 | 20.0 | 42.0 |
| [AI時代における運用主権の再確立と安全性の代償](https://blog.talosintelligence.com/the-safety-penalty-reclaiming-operational-sovereignty-in-the-age-of-ai/) | 27.0 | 20.0 | 42.0 |
| [大量に存在する画像生成AIを同じプロンプトで比較できる「Image benchmarks」をOpenRouterが公開](https://gigazine.net/news/20260825-openrouter-image-benchmarks/) | 27.0 | 20.0 | 42.0 |
| [「メタルギアオンライン」でロビー参加だけでPCを乗っ取られる恐れ、任意コード実行につながる脆弱性が判明](https://gigazine.net/news/20260825-metal-gear-online-3-rce/) | 26.0 | 46.0 | 50.0 |
| [2つのSOCの物語: 2件のレッドチーム評価から得られた知見](https://www.cisa.gov/news-events/cybersecurity-advisories/aa26-237a) | 25.0 | 35.0 | 49.0 |
| [Linux FoundationがAIランタイム証明のオープン標準TRACEを運営へ](https://www.securityweek.com/linux-foundation-to-govern-trace-an-open-standard-for-ai-runtime-attestation/) | 25.0 | 20.0 | 42.0 |
| [Alice、AIモデル防御とエンタープライズ向けガードレール拡充のために1.4億ドルを調達](https://www.securityweek.com/alice-raises-140m-to-expand-ai-model-defenses-and-enterprise-guardrails/) | 25.0 | 20.0 | 42.0 |
| [悪意あるWebページがNVIDIA NemoClawの背後にあるローカルAIモデルを汚染する可能性](https://thehackernews.com/2026/08/a-malicious-webpage-could-poison-your.html) | 25.0 | 20.0 | 42.0 |
| [ウクライナ、戦場データを英国に提供しAI訓練へ](https://therecord.media/ukraine-uk-ai-drone-data) | 25.0 | 20.0 | 42.0 |
| [AIを悪用したブランドなりすましによる新たな金融詐欺の手口](https://www.akamai.com/blog/security/2026/aug/new-face-financial-fraud-ai-powered-brand-abuse) | 25.0 | 20.0 | 42.0 |
| [Frontier AIがもたらす脆弱性管理の構造的変革](https://thehackernews.com/2026/08/frontier-ai-vulnerability-managements.html) | 25.0 | 20.0 | 42.0 |
| [台湾、NvidiaとSuper Microの社員を含む9人を中国への不正AIサーバー輸出で起訴](https://www.securityweek.com/taiwan-charges-9-over-illegal-ai-server-exports-to-china-including-nvidia-and-super-micro-staff/) | 25.0 | 20.0 | 42.0 |
| [Bitsightの新しい調査が示す、AI悪用は「脱獄プロンプト」を超えて進んでいる](https://www.bitsight.com/blog/ai-jailbreak-prompts-evolving-cyber-threats) | 25.0 | 20.0 | 42.0 |
| [パッチ適用の猶予は縮小中：セキュリティに新しい制御プレーンが必要な理由](https://azure.microsoft.com/en-us/blog/the-patch-window-is-collapsing-why-security-needs-a-new-control-plane/) | 22.0 | 20.0 | 48.0 |
| [IPアドレスをホスト名として難読化する手口](https://isc.sans.edu/diary/rss/33280) | 22.0 | 20.0 | 42.0 |
| [「Chrome」が「クリティカル」含む脆弱性7件を修正](https://www.security-next.com/189386) | 22.0 | 20.0 | 42.0 |
| [学習適応性検査の結果シートが所在不明 - 北教大付属校](https://www.security-next.com/189036) | 22.0 | 20.0 | 42.0 |
| [万博出演者の個人情報などが流出か - 2025年日本国際博覧会協会](https://www.security-next.com/189193) | 22.0 | 20.0 | 42.0 |
| [サイトが改ざん被害、偽認証画面を表示 - 日本ブラインドサッカー協会](https://www.security-next.com/189202) | 22.0 | 20.0 | 42.0 |
| [CISAがOracleの完璧な脆弱性に最短3日以内の修正期限を設定](https://www.theregister.com/security/2026/08/25/cisa-slaps-its-tightest-three-day-patching-deadline-on-perfect-10-oracle-flaw/5292107) | 20.0 | 28.0 | 50.0 |
| [Paylogixでハッカーが金融情報と健康情報を窃取](https://therecord.media/paylogix-cyberattack-akira-ransomware) | 20.0 | 20.0 | 42.0 |
| [NSAの精鋭ハッキング部隊や最高裁長官を名乗った男が逮捕される](https://cyberscoop.com/arrested-man-allegedly-impersonated-nsa-elite-hacking-unit-supreme-court-chief-justice/) | 20.0 | 20.0 | 42.0 |
| [水道分野は対応に成功、政府分野はCISAの模擬攻撃の検知・阻止に失敗](https://cyberscoop.com/cisa-red-team-report-government-water-cybersecurity/) | 20.0 | 20.0 | 42.0 |
| [1,449件のOracleパッチを適用してもなお受けたこの攻撃](https://www.theregister.com/security/2026/08/25/you-couldve-applied-all-1449-oracle-patches-and-still-been-hit-by-this-attack/5292335) | 20.0 | 20.0 | 42.0 |
| [ノルウェー政府のデジタルサービスを妨害した大規模DDoS攻撃](https://www.bleepingcomputer.com/news/security/massive-ddos-attack-disrupts-norways-government-digital-services/) | 20.0 | 20.0 | 42.0 |
| [Researchersが警告するSharePoint連続攻撃](https://www.cybersecuritydive.com/news/researchers-warn-about-chained-sharepoint-sequence/828726/) | 20.0 | 20.0 | 42.0 |
| [サイバーセキュリティは手頃に導入できなくなっているのか](https://www.darkreading.com/cybersecurity-operations/is-cyber-facing-an-affordability-crisis-) | 20.0 | 20.0 | 42.0 |
| [Nutex Healthがサイバー攻撃でデータ窃取被害を公表](https://www.bleepingcomputer.com/news/security/hospital-operator-nutex-health-says-data-stolen-in-cyberattack/) | 20.0 | 20.0 | 42.0 |
| [ZeroTokensフィッシングプラットフォームがリアルタイムで攻撃を誘導](https://www.infosecurity-magazine.com/news/zerotokens-phishing-real-time/) | 20.0 | 20.0 | 42.0 |
| [INTERPOLがBlack Axeの不正金融ネットワークを標的にした最新の国際一斉摘発](https://cyberscoop.com/interpol-operation-jackal-iv-black-axe-arrests/) | 20.0 | 20.0 | 42.0 |
| [偽の従業員からアカウント復旧まで：高まる本人確認リスク](https://www.bleepingcomputer.com/news/security/from-fake-workers-to-account-recovery-the-growing-identity-verification-risk/) | 20.0 | 20.0 | 42.0 |
| [INTERPOLの西アフリカ犯罪組織摘発で明らかになった新たな傾向](https://www.helpnetsecurity.com/2026/08/25/interpol-jackal-iv-west-african-crime-groups-arrests/) | 20.0 | 20.0 | 42.0 |
| [WhatsApp、iOSとAndroidでフィッシング耐性のあるサインイン向けに複数のパスキーを追加](https://thehackernews.com/2026/08/whatsapp-adds-multiple-passkeys-for.html) | 20.0 | 20.0 | 42.0 |
| [Fideo Lensがアイデンティティ、アカウント、デバイス間のつながりを可視化](https://www.helpnetsecurity.com/2026/08/25/fideo-lens-investigative-intelligence-platform/) | 20.0 | 20.0 | 42.0 |
| [WhatsAppに強化された2段階認証と複数のパスキー機能を追加](https://www.bleepingcomputer.com/news/security/whatsapp-adds-stronger-two-step-verification-multiple-passkeys/) | 20.0 | 20.0 | 42.0 |
| [WhatsApp、アカウントセキュリティ更新で複数パスキーと強化された2SVを追加](https://www.securityweek.com/whatsapp-adds-multiple-passkeys-and-stronger-2sv-in-account-security-update/) | 20.0 | 20.0 | 42.0 |
| [ICSサイバーセキュリティ会議でCyber-Physical Systems実習トレーニングが再び開催される](https://www.securityweek.com/hands-on-cyber-physical-systems-training-returns-to-ics-cybersecurity-conference/) | 20.0 | 20.0 | 42.0 |
| [英国政府、リスクの高いテクノロジー供給業者を秘密裏に排除する権限を模索](https://therecord.media/uk-technology-national-security) | 20.0 | 20.0 | 42.0 |
| [Marimo Notebookの欠陥により編集モードでセル実行前にMCPコマンドを実行可能にする問題](https://thehackernews.com/2026/08/marimo-notebook-flaw-could-run-mcp.html) | 20.0 | 20.0 | 42.0 |
| [CISAアドバイザリが示すレッドチームの知見と組織のリスク評価・脅威特定・効果的なインシデント対応の支援](https://www.cisa.gov/news-events/news/cisa-advisory-highlights-red-team-findings-help-organizations-assess-risk-identify-threats-and) | 20.0 | 20.0 | 42.0 |
| [大規模DDoS攻撃によりノルウェーの公共サービスが停止](https://therecord.media/norway-cyberattack-ddos-government) | 20.0 | 20.0 | 42.0 |
| [Grokがユーザーのチャットや位置情報などを盗み出すよう誘導される問題](https://www.malwarebytes.com/blog/ai/2026/08/encrypted-instructions-can-fool-ai-assistants-like-grok-and-gemini) | 20.0 | 20.0 | 42.0 |
| [世界的なサイバー犯罪一斉摘発で容疑者数十人を逮捕](https://www.bleepingcomputer.com/news/security/police-arrests-dozens-of-suspects-in-global-cybercrime-crackdown/) | 20.0 | 20.0 | 42.0 |
| [GTA 6リーク追跡で数千人のDiscordユーザーのデータが露出する可能性](https://www.malwarebytes.com/blog/privacy/2026/08/gta-6-leak-hunt-could-expose-data-belonging-to-thousands-of-discord-users) | 20.0 | 20.0 | 42.0 |
| [Silent Patchesは攻撃者を止めない、守る側を見えなくする](https://www.securityweek.com/silent-patches-dont-stop-attackers-they-blind-defenders/) | 20.0 | 20.0 | 42.0 |
| [米議員ら、CISAの予算削減は「同局が使命を果たす能力」に深刻な懸念を招くと指摘](https://www.itpro.com/security/us-lawmakers-say-cisa-cuts-raise-serious-concerns-about-the-agencys-ability-to-fulfil-its-mission) | 20.0 | 20.0 | 42.0 |
| [ShinyHuntersがソーシャルエンジニアリング攻撃で自社社員をだましたReliaQuestを挑発](https://www.helpnetsecurity.com/2026/08/25/reliaquest-breach-social-engineering/) | 20.0 | 20.0 | 42.0 |
| [米国、イランのサイバー攻撃に関与したMabna Instituteのハッカーを制裁](https://www.infosecurity-magazine.com/news/us-sanctions-mabna-institute/) | 20.0 | 20.0 | 42.0 |

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
