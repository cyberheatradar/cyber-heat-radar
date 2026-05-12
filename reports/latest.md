# 📡 サイレーダー 2026-05-12 11:00 JST 試作版

このレポートは、2026-05-12 05:00 JST〜2026-05-12 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 94
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-31431: Copy Fail Linux kernel local privilege escalation](#topic-107) | 100.0 | 95.0 | 92.0 | GitHub | - |
| 2 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 74.0 | 82.0 | 81.0 | 音声 | 温度感上位枠 |
| 3 | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](#topic-31) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Threats Making WAVs - Incident Response to a Cryptomining Attack](#topic-29) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-12"></a>

### 1. Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>Windows</nobr> / <nobr>権限昇格</nobr> / <nobr>TTP</nobr> / <nobr>脆弱性</nobr> / <nobr>KEV</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 74.0 |
| <nobr>実務影響</nobr> | 82.0 |
| <nobr>確度</nobr> | 81.0 |

#### 概要

CVE-2025-60710は、Microsoft WindowsのTaskhost関連処理におけるローカル権限昇格の脆弱性として報告されています。
CISAのKnown Exploited Vulnerabilitiesにも関連付けられており、公開PoCの言及もあるため、優先的な確認対象とみられています。
権限昇格は、端末内での侵害拡大や管理者権限の取得につながるため、影響が大きい類型です。
さらに、実証コードの存在が示唆される場合は、検証や悪用のハードルが下がる点で注意が必要です。

#### CISA KEV詳細

- **CVE**: CVE-2025-60710
- **Vendor / Project**: Microsoft
- **Product**: Windows
- **Vulnerability Name**: Microsoft Windows Link Following Vulnerability
- **Date Added**: 2026-04-13
- **Due Date**: 2026-04-27
- **Known Ransomware Use**: Unknown

**Required Action**

> Apply mitigations per vendor instructions, follow applicable BOD 22-01 guidance for cloud services, or discontinue use of the product if mitigations are unavailable.

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- CISA KEV関連。
- 公開PoC・検証コード言及あり。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 公開PoCにより再現・悪用可能性が上がる。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 公開PoC・検証コード言及あり。
- 公開PoC/Exploitコード: 確認あり。
- 直接PoCリンク: 掲載しません。
- 確認方針: NVD、ベンダー公式、公的機関、信頼できる技術分析を優先し、GitHub等のコードは防御・検証目的で別途確認します。

#### 担当者向け確認ポイント

- Windows端末で該当CVEの影響有無を確認し、ベンダーの修正情報やCISA KEVの更新を追跡する。
- Taskhost関連の異常な挙動や不審な権限昇格の兆候がないか、端末監視・ログ確認を強化する。
- 資産の優先度を見直し、特に管理者権限を持つ端末や重要業務端末を先に対応する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-60710 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 影響ベンダー | 1.00 |
| 製品 | Windows | 影響製品 | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-60710](https://nvd.nist.gov/vuln/detail/CVE-2025-60710) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>公的機関</nobr> | [CISA KEV: CVE-2025-60710](https://www.cisa.gov/known-exploited-vulnerabilities-catalog?field_cve=CVE-2025-60710) | <nobr>KEV掲載内容、Date Added、Due Date、Required Action</nobr> |
| <nobr>公的機関データ</nobr> | [CISA KEV JSON](https://www.cisa.gov/sites/default/files/feeds/known_exploited_vulnerabilities.json) | <nobr>CISA公式の機械可読データ。CVE IDで検索して確認</nobr> |
| <nobr>出典</nobr> | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](https://github.com/Wh04m1001/CVE-2025-60710) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。
- 継続観測: 継続。

---

<a id="topic-31"></a>

### 2. PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>防御・運用</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Guardicore Labsによると、MySQLサーバーを狙うランサムウェア関連の活動が確認されています。
攻撃者は二重の脅迫を用い、盗んだデータの公開で被害組織に圧力をかける手口が示されています。MySQLは多くのシステムで基盤的に使われるため、影響範囲が広がる可能性があります。
ランサムウェアは暗号化だけでなく情報公開の脅しも組み合わせるため、復旧対応と情報管理の両面で負荷が高くなります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- MySQLの露出状況、認証設定、不要な外部公開の有無を点検する。
- バックアップの保全性と復旧手順を確認し、定期的にリストア検証を行う。
- 侵害兆候の監視と、データ漏えい時の連絡・判断フローを事前に整理しておく。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](https://akamai.com/blog/security/please-read-me-opportunistic-ransomware-devastating-mysql-servers) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 未評価。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-29"></a>

### 3. Threats Making WAVs - Incident Response to a Cryptomining Attack

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>防御・運用</nobr> / <nobr>マルウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

公開情報によると、WAVファイルの中に暗号資産のマイナーを隠した攻撃事案が分析されています。
報告では、検知から感染、ネットワーク上での拡散、マルウェア解析までが整理され、データセンター向けのインシデント対応改善点も示されています。
通常の音声ファイルに見える形式が悪用されると、初動で見逃される可能性があります。インシデント対応の観点では、侵入後の横展開や資源消費型の被害を早く把握できるかが重要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 音声ファイルを含む不審なアーティファクトでも、一般的な業務データとして扱い切らず、検査対象に含める。
- 暗号資産マイニング由来のCPU・メモリ・ネットワーク異常を、性能劣化や障害と切り分けて監視する。
- 感染後の拡散経路を追えるよう、ログ保全と端末・サーバーの相関確認を早めに行う。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Threats Making WAVs - Incident Response to a Cryptomining Attack](https://akamai.com/blog/security/threats-making-wavs-incident-reponse-cryptomining-attack) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 未評価。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-107"></a>

### 1. CVE-2026-31431: Copy Fail Linux kernel local privilege escalation

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>Linux</nobr> / <nobr>脆弱性</nobr> / <nobr>権限昇格</nobr> / <nobr>CVE</nobr> / <nobr>TTP</nobr> / <nobr>AI</nobr> / <nobr>ゼロデイ</nobr> |
| <nobr>温度状態</nobr> | 高温 |
| <nobr>温度感</nobr> | 100.0 |
| <nobr>実務影響</nobr> | 95.0 |
| <nobr>確度</nobr> | 92.0 |

#### 概要

Linuxカーネルにおける権限昇格の脆弱性「Copy Fail」として、CVE-2026-31431が注目されています。
公開情報では、悪用情報や公開PoCの言及があり、関連する技術コミュニティでも関心が高まっています。
ローカル権限昇格は、侵入後に管理者権限へ進む足掛かりになりやすく、被害の拡大につながるためです。
公開PoCの存在が示唆されている場合、未対応環境では優先的な確認が必要になります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 23 sources。
- CISA KEV関連。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 技術者コミュニティ反応: 強。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- 権限昇格系。
- 実務影響100は特別条件が揃う場合に限定するため、上限補正を適用。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 公開PoC・検証コード言及あり。
- 公開PoC/Exploitコード: 確認あり。
- 直接PoCリンク: 掲載しません。
- 確認方針: NVD、ベンダー公式、公的機関、信頼できる技術分析を優先し、GitHub等のコードは防御・検証目的で別途確認します。

#### 担当者向け確認ポイント

- Linuxカーネルの影響範囲を確認し、利用中のディストリビューションや配布パッケージの更新状況を点検する。
- ベンダーや配布元の修正情報、回避策、推奨設定の有無を確認し、適用計画を立てる。
- 権限昇格の兆候を含む監視を強化し、通常ユーザーから管理者権限への不自然な遷移を点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-31431 | 主要CVE | 1.00 |
| ベンダー | Linux | 影響ベンダー | 1.00 |
| 脆弱性 | CVE-2026-43284 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-43500 | 主要CVE | 1.00 |
| 製品 | Kernel | 影響製品 | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-31431](https://nvd.nist.gov/vuln/detail/CVE-2026-31431) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [はてな、マネフォ、そしてLinuxの脆弱性「Copy Fail」を読み解く　“見えている落とし穴”を避けるには](https://itmedia.co.jp/enterprise/articles/2605/12/news022.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | ['Dirty Frag' Exploit Poised to Blow Up on Enterprise Linux Distros](https://darkreading.com/vulnerabilities-threats/dirty-frag-exploit-blow-up-enterprise-linux-distros) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Linux developers weigh emergency “killswitch” for vulnerable kernel functions](https://helpnetsecurity.com/2026/05/11/linux-kernel-emergency-killswitch) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Dirty Frag: Linux kernel hit by second major security flaw in two weeks](https://therecord.media/dirty-frag-linux-kernel-hit-by-second-major-bug) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [New ‘Dirty Frag’ Linux Vulnerability Possibly Exploited in Attacks](https://securityweek.com/new-dirty-frag-linux-vulnerability-possibly-exploited-in-attacks) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Another Universal Linux Local Privilege Escalation (LPE) Vulnerability: Dirty Fr](https://isc.sans.edu/diary/rss/32968) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Linux Kernel Dirty Frag LPE Exploit Enables Root Access Across Major Distributio](https://thehackernews.com/2026/05/linux-kernel-dirty-frag-lpe-exploit.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: あり。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 強。
- 技術者コミュニティ反応: 強。
- 開発者コミュニティ反応: 中。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。
- 継続観測: 継続。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [決算短信開示 期末後 50 日超える見通し ～ ヘア化粧品のコタにランサムウェア攻撃](https://scan.netsecurity.ne.jp/article/2026/05/12/55243.html) | 29.0 | 30.0 | 42.0 |
| [国際看護学部入学生 431 名の個人情報が漏えいした可能性 ～ メディカ出版へのランサムウェア攻撃](https://scan.netsecurity.ne.jp/article/2026/05/12/55239.html) | 29.0 | 30.0 | 42.0 |
| [イスラエルの水インフラを標的にした未完成のマルウェア ほか [Scan PREMIUM Monthly Executive Summary 2026年4月度]](https://scan.netsecurity.ne.jp/article/2026/05/12/55247.html) | 29.0 | 20.0 | 42.0 |
| [UniFi Access におけるリモートコード実行の脆弱性（CVE-2025-52665）](https://catchify.sa/post/cve-2025-52665-rce-in-unifi-os-25-000) | 28.0 | 46.0 | 50.0 |
| [Netskopeのクロステナント認証バイパス脆弱性](https://blog.amberwolf.com/blog/2025/august/advisory---netskope-cross-tenant-authentication-bypass) | 28.0 | 38.0 | 42.0 |
| [「くら寿司 公式アプリ」に脆弱性、起動時の強制アップデートで対応 JVN報告](https://itmedia.co.jp/news/articles/2605/12/news048.html) | 28.0 | 23.0 | 43.0 |
| [Nansh0uキャンペーン―ハッカーの兵器庫がさらに強化される](https://akamai.com/blog/security/the-nansh0u-campaign-hackers-arsenal-grows-stronger) | 28.0 | 20.0 | 42.0 |
| [Oracle of Delphiが認証情報を窃取する](https://akamai.com/blog/security/the-oracle-of-delphi-steal-your-credentials) | 28.0 | 20.0 | 42.0 |
| [ClaudeのChrome拡張に脆弱性、他の拡張機能からAI操作が可能に](https://news.mynavi.jp/techplus/article/20260512-4449441) | 26.0 | 20.0 | 42.0 |
| [設計開発業務を生成AIで変革 生産性が1.3倍にアップ](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020600004/050700208) | 26.0 | 20.0 | 42.0 |
| [「Claude」は「夢」を見る--新機能がもたらす自己改善の仕組みとは](https://japan.zdnet.com/article/35247263) | 26.0 | 20.0 | 42.0 |
| [OpenAI、企業向けAI導入支援を本格展開 「Deployment Company」設立](https://itmedia.co.jp/news/articles/2605/12/news053.html) | 26.0 | 20.0 | 42.0 |
| [Security: OpenAI Sora 2の内部を探る - マルチモーダルLLMを駆動するシステムプロンプトの解明](https://mindgard.ai/resources/openai-sora-system-prompts) | 25.0 | 20.0 | 42.0 |
| [必見：Geminiをハッキングする多層的アプローチ](https://buganizer.cc/hacking-gemini-a-multi-layered-approach-md) | 25.0 | 20.0 | 42.0 |
| [Elastic Security MCP App: AIツール内で対話的に行うセキュリティ運用](https://elastic.co/security-labs/elastic-security-mcp-app) | 25.0 | 20.0 | 42.0 |
| [Citrix NetScalerのメモリリークと反射型XSS（CVE-2025-12101）](https://bit.ly/48bPzCO) | 23.0 | 34.0 | 50.0 |
| [MixMaster MMORPGのリバースエンジニアリングによるセキュリティ分析](https://3r4y.github.io/posts/mixmasterreverseengineering) | 22.0 | 20.0 | 42.0 |
| [OpenAIが攻撃者より先に脆弱性を検知・修正するセキュリティAI「Daybreak」を発表](https://gigazine.net/news/20260512-openai-daybreak) | 22.0 | 20.0 | 42.0 |
| [「デフォルトブラウザを選ぶ画面」でFirefoxを選択するユーザーが600万人に達し10秒に1回選ばれる状況に](https://gigazine.net/news/20260512-firefox-browser-choice) | 22.0 | 20.0 | 42.0 |
| [オブジェクトストレージ「Dell ECS」「ObjectScale」に深刻な脆弱性](https://security-next.com/184275) | 22.0 | 20.0 | 42.0 |
| [コンビニのおにぎりは1個何円まで許せる？GIGAZINE読者に聞いてみた](https://gigazine.net/news/20260512-gigazine-user-convenience-store-onigiri) | 22.0 | 20.0 | 42.0 |
| [JetBrains「TeamCity」にAPI露出の脆弱性 - ゲストも悪用可能](https://security-next.com/184269) | 22.0 | 20.0 | 42.0 |
| [Apple、全製品で多数の脆弱性を修正](https://isc.sans.edu/diary/rss/32976) | 22.0 | 20.0 | 42.0 |
| [New GhostLockツールがWindows APIを悪用してファイルアクセスを妨害](https://bleepingcomputer.com/news/security/new-ghostlock-tool-abuses-windows-api-to-block-file-access) | 22.0 | 20.0 | 42.0 |

---

## 📊 スコアの見方

| <nobr>指標</nobr> | 意味 |
|---|---|
| <nobr>温度状態</nobr> | 話題のライフサイクルを示す補助ラベルです。例: 低温、継続監視、温度上昇中、高温、冷却中。 |
| <nobr>温度感</nobr> | 話題として今どれだけ注目・拡散・更新されているかを示します。 |
| <nobr>実務影響</nobr> | 対象組織・担当者にとって、対応優先度や被害可能性がどれだけ大きいかを示します。 |
| <nobr>確度</nobr> | 公的機関、ベンダー公式、複数ソース、CVE/KEV、一次資料などにより、情報をどれだけ確認できているかを示します。事件報道系は、複数報道があっても司法文書・当局発表などの一次資料が弱い場合、脆弱性KEV系より低く出ることがあります。 |

スコアは、公開情報から抽出した特徴量と事前定義した重み付けに基づく参考指標です。詳しい算出方針は [スコアリング方針](../docs/scoring.md) を参照してください。

## 🔒 公開しない内部情報について

サイレーダーでは、温度感の補助シグナルとして、公的機関・ベンダー公式・信頼できる報道機関・技術者コミュニティ・国内外の公開反応などを利用します。

これらのシグナルは、一次情報、報道波及、技術者反応、開発者反応、PoC・悪用観測などに分けて評価します。

ただし、ランキング操作、スパム的誘導、監視回避を防ぐため、個別の監視対象、取得手段、検索条件、評価対象サービス名、内部的な重み付けやしきい値は公開しません。

また、公開反応の多さだけで掲載順位を決めることはありません。重要度の判定では、ベンダー公式情報、公的機関、一次資料、信頼できる技術分析、実務影響を優先します。

## ⚠️ 注意事項

このレポートは、収集・観測できた公開情報をもとにした参考情報です。完全性、正確性、即時性を保証するものではありません。

重要な判断を行う場合は、必ずベンダー公式情報、公的機関、一次情報を確認してください。

サイレーダーは、広告・スポンサー・企業関係に基づいて掲載順位や温度感スコアを変更しません。
