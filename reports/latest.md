# 📡 サイレーダー 2026-08-22 05:00 JST

このレポートは、2026-08-21 17:00 JST〜2026-08-22 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 80
- [音声で扱う想定のトピック](#audio-topics): 4
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 51

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-73570: CISA KEV catalog addition](#topic-28581) | 45.0 | 64.0 | 55.0 | 音声 | 温度感上位枠 |
| 2 | [Critical Microsoft Entra ID vulnerability exploited in the wild (CVE-2026-69836)](#topic-28716) | 42.0 | 64.0 | 55.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [CISA orders feds to patch actively exploited TrueConf Server flaws](#topic-28805) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [In Other News: Zombie Card Attack, T-Mobile Cut Cable to Stop Hackers, GitHub Denies AI Caused Bug](#topic-28773) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Attackers impersonate popular AI brands to spread malware](#topic-28811) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-28581"></a>

### 1. CVE-2026-73570: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

CISAは、Zimbra Collaboration（ZCS）に影響するCVE-2026-73570をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
公開情報では、この脆弱性はすでに実環境で悪用が確認されているとされ、コマンドインジェクションを通じてリモートコード実行につながるおそれがあります。
KEVへの追加は、単なる理論上の脆弱性ではなく、優先度を上げて対処すべき実害のある問題であることを示します。
メール基盤として広く使われるZimbraの脆弱性であるため、影響範囲が大きくなりやすい点も注目されています。

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
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Zimbra Collaboration（ZCS）の利用有無と対象バージョンを確認し、ベンダーの修正適用状況を点検する。
- KEV掲載を踏まえ、資産管理・脆弱性管理の優先順位を引き上げる。
- 関連システムの不審な挙動や管理操作の痕跡を確認し、必要に応じて監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-73570 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Zimbra | 言及あり | 0.80 | — |
| 製品 | Zimbra Collaboration | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-73570](https://nvd.nist.gov/vuln/detail/CVE-2026-73570) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/08/21/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit Zimbra SNMP Flaw for Unauthenticated Remote Code Execution](https://thehackernews.com/2026/08/attackers-exploit-zimbra-snmp-flaw-for.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-28805"></a>

### 2. CISA orders feds to patch actively exploited TrueConf Server flaws

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

CISAは、TrueConf Serverに存在する2件の脆弱性について、米連邦機関に対し優先的な修正を求めました。
これらの問題は実際に悪用されているとされ、自己ホスト型の通信基盤を運用する組織では早急な対応が必要です。
公的機関が対応を促している点から、単なる理論上の脆弱性ではなく、現実のリスクとして扱う必要があります。
通信基盤は業務影響が大きいため、影響範囲の確認と修正の優先度判断が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- TrueConf Serverを利用中の環境では、対象バージョンや適用状況を確認し、ベンダー案内に沿って速やかに修正する。
- 外部公開されている管理画面や関連サービスがある場合は、アクセス制御や到達性を見直し、不要な露出を減らす。
- 修正までの間は、認証失敗や不審な管理操作などのログを重点的に監視し、影響の有無を確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA orders feds to patch actively exploited TrueConf Server flaws](https://www.bleepingcomputer.com/news/security/cisa-orders-feds-to-patch-actively-exploited-trueconf-server-flaws/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-28773"></a>

### 3. In Other News: Zombie Card Attack, T-Mobile Cut Cable to Stop Hackers, GitHub Denies AI Caused Bug

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

SecurityWeekが、複数の注目トピックをまとめた「In Other News」の一部として、T-Mobileの対応やGitHubのAI起因とされる不具合否定などを取り上げました。
材料からは個別事案の詳細や影響範囲までは断定できませんが、AIとセキュリティを巡る話題の一つとして注目されています。
AI関連の不具合や説明責任をめぐる話題は、開発・運用の現場で判断を誤ると影響が広がりやすいためです。
加えて、通信事業者や主要プラットフォームの対応は、同種事案への備えや社内説明の参考になります。

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

- AI起因と断定されているか、未確認かを切り分けて扱う。
- 障害・不具合時の社内外説明を、事実ベースで更新できる体制を確認する。
- 主要サービスや通信経路の変更・遮断が必要になるケースを想定し、代替手順を見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [In Other News: Zombie Card Attack, T-Mobile Cut Cable to Stop Hackers, GitHub De](https://www.securityweek.com/in-other-news-zombie-card-attack-t-mobile-cut-cable-to-stop-hackers-github-denies-ai-caused-bug/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-28811"></a>

### 4. Attackers impersonate popular AI brands to spread malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Sophosの分析によると、Perplexity、Claude、ChatGPT、Copilotなどの人気AIブランドを装って、情報窃取型マルウェアやバックドア、悪意あるブラウザ拡張機能などを広める動きが確認されています。
AI関連として分類された事案の中から、実際に悪意ある活動と確認されたケースがあったとされています。
AIサービスの知名度を悪用したなりすましは、利用者の警戒を下げやすく、フィッシングやマルウェア配布の入口になり得ます。
AIツールの導入や案内を装う偽サイト・偽配布物への注意が必要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIブランド名を含む配布物や拡張機能は、提供元の真正性を厳密に確認する。
- 利用者に対し、検索広告・SNS・メール経由の“公式風”案内を安易に開かないよう周知する。
- 端末保護では、ブラウザ拡張機能の許可管理とEDR/AVでの不審な挙動監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Sophos X-Ops | 言及あり | 0.80 | — |
| ベンダー | Sophos | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Attackers impersonate popular AI brands to spread malware](https://www.helpnetsecurity.com/2026/08/21/ai-brand-impersonation-malware-malware-research/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-28716"></a>

### 1. Critical Microsoft Entra ID vulnerability exploited in the wild (CVE-2026-69836)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 42.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

Microsoft Entra IDにおける重大な脆弱性CVE-2026-69836が報告され、初期情報では実環境での悪用が示唆されました。
もっとも、その後に一部報道ではMicrosoftが「悪用なし」に修正したとされており、現時点では悪用状況について情報が食い違っています。
Entra IDはMicrosoft 365やAzureなどの認証・アクセス制御の中核であり、影響範囲が広い点が注目されています。
CVSS 10.0のRCE脆弱性として扱われているため、誤検知や情報更新も含めて継続監視が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Microsoftの公式アドバイザリと関連通知を確認し、悪用有無の更新を追う。
- Entra ID関連の認証・アクセスログで不審な挙動がないか、通常より優先度を上げて確認する。
- Microsoft 365やAzureを含む依存サービスへの影響を整理し、インシデント対応の連絡系統を明確にしておく。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-69836 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft Entra ID | 言及あり | 0.80 | — |
| 製品 | Active Directory | 言及あり | 0.80 | — |
| 製品 | Microsoft Azure | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-69836](https://nvd.nist.gov/vuln/detail/CVE-2026-69836) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Critical Microsoft Entra ID vulnerability exploited in the wild (CVE-2026-69836)](https://www.helpnetsecurity.com/2026/08/21/microsoft-entra-id-vulnerability-cve-2026-69836/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches Severe Entra ID Flaw (CVSS 10.0) Allowing Remote Code Executio](https://thehackernews.com/2026/08/microsoft-entra-id-flaw-cvss-100.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft confirms maximum severity flaw in Entra ID targeted for exploitation](https://www.cybersecuritydive.com/news/microsoft-maximum-severity-flaw-entra-id-exploitation/828501/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [人気のRustクレートを汚染し開発者の認証情報を窃取する攻撃者](https://www.theregister.com/security/2026/08/21/hackers-poison-popular-rust-crates-to-steal-developers-credentials/5291075) | 28.0 | 45.0 | 42.0 |
| [カナダのSickKids病院、再びサイバー攻撃を受け職員データが窃取される](https://therecord.media/canada-hospital-for-sick-children-attacked-again-employee-data) | 28.0 | 30.0 | 42.0 |
| [AmnesiaStealerがmacOSに対話型ブラウザセッションハイジャックを導入](https://blog.polyswarm.io/amnesiastealer-introduces-interactive-browser-session-hijacking-to-macos) | 28.0 | 20.0 | 42.0 |
| [Microsoft Teamsを悪用したフィッシングキャンペーンで新たなSynkLoaderマルウェアが配布される](https://www.bleepingcomputer.com/news/security/new-synkloader-malware-pushed-in-microsoft-teams-phishing-campaign/) | 28.0 | 20.0 | 42.0 |
| [Androidの車載マルウェアが内蔵アップデータを悪用してAd FraudとProxy Botnetを拡散](https://thehackernews.com/2026/08/android-car-malware-spreads-through.html) | 28.0 | 20.0 | 42.0 |
| [Agent Teslaの新たなマルウェア亜種、回避能力を強化](https://www.infosecurity-magazine.com/news/agent-tesla-malware-evasion/) | 28.0 | 20.0 | 42.0 |
| [HackersがFTPサーバーのバナーを悪用して新たなWindowsマルウェアを配布](https://www.bleepingcomputer.com/news/security/hackers-abuse-ftp-server-banners-to-deliver-new-windows-malware/) | 28.0 | 20.0 | 42.0 |
| [車内に潜む見えない乗客](https://securelist.com/android-head-unit-malware/121106/) | 28.0 | 20.0 | 42.0 |
| [使い込むほど成長するAIエージェント「Hermes Agent」で実際に行った作業をスキル化して再利用してみた](https://gigazine.net/news/20260821-hermes-agent-skill/) | 27.0 | 20.0 | 42.0 |
| [AIの回答をコピペしないでくれと頼む運動「Don’t paste the AI, please.(AIが書いたものをコピペしないでください)」](https://gigazine.net/news/20260821-dont-paste-the-ai-please/) | 27.0 | 20.0 | 42.0 |
| [Anthropic、8月末にもIPO申請書類を公開か 調達額はSpaceXの過去最大に匹敵と米報道](https://www.itmedia.co.jp/news/article/2608/21/2000000688/) | 26.0 | 20.0 | 42.0 |
| [Cisco Crossworkのセキュリティ強化リリース（2026年8月）](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-hardening-crosswork-UzDTU9Vh) | 25.0 | 46.0 | 51.0 |
| [OWASPが新たなセキュリティ青写真でAIスキルの主要リスクを指摘](https://www.darkreading.com/application-security/owasp-flags-top-ai-skill-risks-security-blueprint) | 25.0 | 20.0 | 42.0 |
| [AI時代における新たな脅威インテリジェンス戦略](https://securityboulevard.com/2026/08/rethinking-threat-intelligence-new-tactics-for-the-age-of-ai/) | 25.0 | 20.0 | 42.0 |
| [GrokとGeminiで暗号化されたプロンプトがAI安全ガードレールを回避する問題](https://www.securityweek.com/encrypted-prompts-bypass-ai-safety-guardrails-in-grok-and-gemini/) | 25.0 | 20.0 | 42.0 |
| [OpenAIが本来あるべきだった制御機能を追加](https://www.darkreading.com/application-security/openai-adds-controls-already) | 25.0 | 20.0 | 42.0 |
| [WazuhとAIによるSOCワークフローの強化](https://thehackernews.com/2026/08/wazuh-and-ai-for-enhanced-soc-workflows.html) | 25.0 | 20.0 | 42.0 |
| [Isolated-vmの重大な脆弱性によりホスト上でRCEが発生](https://www.securityweek.com/critical-isolated-vm-vulnerability-leads-to-rce-on-host/) | 24.0 | 38.0 | 42.0 |
| [Microsoftが悪用されたEntra IDの脆弱性を修正](https://www.securityweek.com/microsoft-rolls-out-22-fresh-security-patches/) | 22.0 | 32.0 | 42.0 |
| [企業サイト侵害か、問い合わせ情報流出の可能性 - セントラルコンサルタント](https://www.security-next.com/188363) | 22.0 | 20.0 | 42.0 |
| [アクセス制限に不備、個人情報流出の可能性 - エリッツHD子会社](https://www.security-next.com/189196) | 22.0 | 20.0 | 42.0 |
| [委託先の患者支援システムで個人情報流出 - 旭化成セラピューティクス](https://www.security-next.com/187860) | 22.0 | 20.0 | 42.0 |
| [広報紙配布の宛名シール、別人宛名に重ね貼り - 大阪市](https://www.security-next.com/189129) | 22.0 | 20.0 | 42.0 |
| [調査票発送時の宛名に本来不要な国籍を記載 - 杉並区](https://www.security-next.com/188970) | 22.0 | 20.0 | 42.0 |
| [Homeland security cybercopsがTrueConf（Russia's Zoom）利用者にパッチ適用を呼びかけ](https://www.theregister.com/patches/2026/08/21/homeland-security-cybercops-say-patch-trueconf-russias-zoom-if-youre-using-it/5291156) | 20.0 | 20.0 | 42.0 |
| [元NSA長官ポール・ナカソネ氏、国家安全保障アドバイザリー会社を設立](https://www.securityweek.com/former-nsa-director-paul-nakasone-launches-national-security-advisory-firm/) | 20.0 | 20.0 | 42.0 |
| [U.S. Bank、第四者インシデントに関連する侵害主張を否定](https://therecord.media/us-bank-says-breach-claims-related-to-fourth-party-incident) | 20.0 | 20.0 | 42.0 |
| [流出した数百件のAWSキーにより企業アカウントを完全制御可能に](https://www.bleepingcomputer.com/news/security/hundreds-of-leaked-aws-keys-give-full-control-over-corporate-accounts/) | 20.0 | 20.0 | 42.0 |
| [Microsoft Defenderのドライバが起動時にセキュリティソフトを削除可能に悪用される](https://thehackernews.com/2026/08/microsoft-defenders-own-driver-can-be.html) | 20.0 | 20.0 | 42.0 |
| [今週の主な10件の情報漏えい事件](https://securityboulevard.com/2026/08/top-10-breaches-of-the-week-7/) | 20.0 | 20.0 | 42.0 |
| [米国民への政府によるハッキングについて監視機関による調査を議員が要請](https://cyberscoop.com/watchdog-review-federal-government-hacking-americans/) | 20.0 | 20.0 | 42.0 |
| [Palo AltoとNTT Dataが拡大するセキュリティ提携で10億ドル目標を設定](https://securityboulevard.com/2026/08/palo-alto-ntt-data-set-1b-goal-for-expanded-security-partnership/) | 20.0 | 20.0 | 42.0 |
| [防衛請負業者のCMMCへの自信は低迷、自己評価は改善しているものの](https://www.cybersecuritydive.com/news/defense-contractors-cmmc-cybersecurity-confidence-gap/828494/) | 20.0 | 20.0 | 42.0 |
| [Passkeyを悪用する新たなフィッシングツールキット、パスワードリセット後もアクセスを維持](https://www.securityweek.com/new-phishing-toolkit-uses-passkeys-to-maintain-access-after-password-resets/) | 20.0 | 20.0 | 42.0 |
| [Zombie Card: 期限切れのVisaクレジットカードが購入に利用される](https://www.malwarebytes.com/blog/news/2026/08/zombie-card-an-expired-visa-credit-card-can-be-used-for-purchases) | 20.0 | 20.0 | 42.0 |
| [オンラインプライバシーは可能か？ デジタルアイデンティティが役立つ方法](https://www.bleepingcomputer.com/news/security/is-online-privacy-possible-how-digital-identities-can-help/) | 20.0 | 20.0 | 42.0 |
| [Cyberプロに市庁舎防衛への協力を呼びかける](https://www.darkreading.com/cyber-risk/cyber-pros-help-city-hall) | 20.0 | 20.0 | 42.0 |
| [親ウクライナ派ハッカーが主張したサイバー攻撃をロシアのネットワーク監視企業が確認](https://therecord.media/russian-network-monitoring-firm-confirms-cyberattack-claimed-by-pro-ukraine-group) | 20.0 | 20.0 | 42.0 |
| [Copilotが「Meta-Hacking」で自らの脆弱性を露呈：Varonis](https://securityboulevard.com/2026/08/copilot-revealed-its-own-vulnerability-through-meta-hacking-varonis/) | 20.0 | 20.0 | 42.0 |
| [PCI DSS v4.0の期限迫る：5ステップのギャップ評価を今すぐ実施](https://securityboulevard.com/2026/08/pci-dss-v4-0-deadline-5-step-gap-assessments-now/) | 20.0 | 20.0 | 42.0 |
| [Data Privacy Regulations: Continuum GRCによる統合コンプライアンス](https://securityboulevard.com/2026/08/data-privacy-regulations-unified-compliance-by-continuum-grc/) | 20.0 | 20.0 | 42.0 |
| [北朝鮮系ハッカーと関連付けられたRustサプライチェーン攻撃](https://www.infosecurity-magazine.com/news/north-korean-rust-supply-chain/) | 20.0 | 20.0 | 42.0 |
| [CareCloudのデータ侵害で医療記録、SSN、銀行口座情報が流出](https://securityboulevard.com/2026/08/medical-records-ssns-and-bank-details-exposed-in-carecloud-data-breach/) | 20.0 | 20.0 | 42.0 |
| [HealthTechスタートアップにおけるSOC 2とHIPAAのペネトレーションテスト要件比較](https://securityboulevard.com/2026/08/soc-2-vs-hipaa-pentest-requirements-for-healthtech-startups/) | 20.0 | 20.0 | 42.0 |
| [Microsoftが警告するEntra IDの重大な脆弱性、攻撃で悪用を確認](https://www.bleepingcomputer.com/news/microsoft/microsoft-warns-of-max-severity-entra-id-flaw-exploited-in-attacks/) | 20.0 | 20.0 | 42.0 |
| [SickKidsのデータ侵害で従業員と採用応募者の情報が流出](https://www.bleepingcomputer.com/news/security/sickkids-data-breach-exposes-employee-and-job-applicant-info/) | 20.0 | 20.0 | 42.0 |
| [Cisco、CrossworkとSecure Workloadの9件の脆弱性を修正、うち5件はCVSS 10.0](https://thehackernews.com/2026/08/cisco-patches-nine-crosswork-and-secure.html) | 20.0 | 20.0 | 42.0 |
| [North Korean Hackersに関連するRustのサプライチェーン攻撃](https://www.securityweek.com/rust-supply-chain-attack-linked-to-north-korean-hackers/) | 20.0 | 20.0 | 42.0 |
| [DEF CONイベント後にサイバー犯罪者の標的となったとセキュリティ研究者らが警告](https://www.itpro.com/security/be-careful-who-you-talk-to-at-conferences-security-researchers-claim-they-were-targeted-by-cyber-criminals-after-def-con-event) | 20.0 | 20.0 | 42.0 |
| [契約業者のCMMCへの自信は高まる一方、実証能力は遅れがちに](https://www.securityweek.com/contractors-cmmc-confidence-rises-as-ability-to-prove-it-falls-behind/) | 20.0 | 20.0 | 42.0 |
| [楽天ブックス関係会社のPCに不正アクセス、ユーザー3万3333人分の個人情報などが漏えいの可能性](https://internet.watch.impress.co.jp/docs/news/2134682.html) | 20.0 | 20.0 | 42.0 |

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
