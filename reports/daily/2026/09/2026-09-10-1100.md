# 📡 サイレーダー 2026-09-10 11:00 JST

このレポートは、2026-09-10 05:00 JST〜2026-09-10 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 64
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 38

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Chinese espionage groups swarm to exploit triple-link chain of zero-days](#topic-31075) | 36.0 | 46.0 | 59.0 | 音声 | 温度感上位枠 |
| 2 | [Cisco confirms CVE-2026-20079 Secure FMC flaw exploited in attacks](#topic-24944) | 34.0 | 64.0 | 59.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-31075"></a>

### 1. Chinese espionage groups swarm to exploit triple-link chain of zero-days

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

Google Chromeの脆弱性CVE-2026-85046は、実際の悪用が確認されており、関連する更新プログラムが配信されています。
公開情報では、複数の中国関連とされる攻撃グループが、ゼロデイの連鎖を用いて組織を狙っていると報じられています。既知の悪用がある脆弱性は、優先度の高い対応対象になります。
ブラウザは業務利用が広く、更新遅延がそのままリスクにつながりやすいためです。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ChromeおよびChromium系ブラウザの更新適用状況を至急確認する。
- CISA KEVなどの既知悪用脆弱性リストに載る前提で、資産棚卸しと優先順位付けを行う。
- 関連する端末で不審な挙動やブラウザ起点の侵入痕跡がないか監視を強める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-85046 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-85880 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-87491 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Chromium | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-85046](https://nvd.nist.gov/vuln/detail/CVE-2026-85046) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Chinese espionage groups swarm to exploit triple-link chain of zero-days](https://cyberscoop.com/china-espionage-groups-exploit-chain-zero-days/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google patches actively exploited Chrome zero-day (CVE-2026-85046)](https://www.helpnetsecurity.com/2026/09/04/google-chrome-zero-day-cve-2026-85046/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/09/04/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-24944"></a>

### 2. Cisco confirms CVE-2026-20079 Secure FMC flaw exploited in attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 34.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

Ciscoは、Secure Firewall Management Center（FMC）ソフトウェアの認証回避の脆弱性「CVE-2026-20079」について、攻撃で悪用されていることを確認したとしています。
影響を受ける環境では、未認証の遠隔攻撃者により認証を回避され、基盤OS上で高権限の操作につながる可能性があると説明されています。
FMCはファイアウォール運用の中核に関わるため、影響が出ると管理面への波及が大きくなり得ます。すでに悪用が観測されているとされ、更新適用の優先度が高い事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Ciscoが提供する修正済みソフトウェアへの更新を優先すること。
- FMC管理インターフェースの公開状況を確認し、外部から到達可能な構成を見直すこと。
- 認証回避や不審なHTTPアクセス、管理系の異常挙動がないかログを確認すること。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20079 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-20316 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Adaptive Security Appliance | 言及あり | 0.80 | — |
| 製品 | Cisco Firepower Threat Defense | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20079](https://nvd.nist.gov/vuln/detail/CVE-2026-20079) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco confirms CVE-2026-20079 Secure FMC flaw exploited in attacks](https://www.bleepingcomputer.com/news/security/cisco-confirms-cve-2026-20079-secure-fmc-flaw-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Active exploitation of Cisco Secure Firewall Management Center vulnerabilities](https://blog.talosintelligence.com/fmc-ongoing-exploitation/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Firewall Management Center Software Authentication Bypass Vulnerabi](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-onprem-fmc-authbypass-5JPp45V2) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

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
| [REVISIO 役職員が使用する PC がマルウェア感染、ローカル環境に保存されていた個人情報が外部漏えいした可能性を否定できず](https://scan.netsecurity.ne.jp/article/2026/09/10/56189.html) | 29.0 | 20.0 | 42.0 |
| [AdaptHealth、7月のサイバー攻撃で410万人分の情報流出を確認](https://www.bleepingcomputer.com/news/security/adapthealth-confirms-41-million-people-exposed-in-july-cyberattack/) | 28.0 | 20.0 | 42.0 |
| [AIエージェント管理基盤の「実行」と「運用」に新展開か--Datadogの取り組みから探る](https://japan.zdnet.com/article/35252446/) | 26.0 | 20.0 | 42.0 |
| [「Claude」による不正アクセス、4件目が判明──Anthropic、「アライメントの失敗」と評価を修正](https://www.itmedia.co.jp/news/article/2609/10/2000001346/) | 26.0 | 20.0 | 42.0 |
| [AI の暴走・セキュリティリスクを解消、テリロジーが業務自動化「palton AI」を発表](https://scan.netsecurity.ne.jp/article/2026/09/10/56181.html) | 26.0 | 20.0 | 42.0 |
| [AI 時代の CSIRT のあり方を探る「NCA Annual Conference 2026」12月2日～4日 開催](https://scan.netsecurity.ne.jp/article/2026/09/10/56175.html) | 26.0 | 20.0 | 42.0 |
| [「AI-Ready」な内製化への道 先進3社に見る3つのポイント](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/051500549/090900005/) | 26.0 | 20.0 | 42.0 |
| [Anthropicが明らかにしたAIによる4件目の犯罪の可能性](https://www.theregister.com/ai-and-ml/2026/09/10/anthropic-reveals-fourth-likely-crime-committed-by-its-ai/5295412) | 25.0 | 20.0 | 42.0 |
| [ChromeとWindowsを標的とする新たなBlue Moonキット、AI駆動型エクスプロイトの新現実を反映](https://www.theregister.com/research/2026/09/09/novel-blue-moon-kit-targeting-chrome-and-windows-reflects-new-reality-of-ai-driven-exploits/5295399) | 25.0 | 20.0 | 42.0 |
| [NTTらの投資ファンド「IOWN AI Fund」、初号投資として光回路スイッチを開発するiPronicsに出資](https://internet.watch.impress.co.jp/docs/news/2139491.html) | 25.0 | 20.0 | 42.0 |
| [「FortiOS」や「NetScaler」など脆弱性4件の悪用を警告 - 米当局](https://www.security-next.com/190122) | 24.0 | 20.0 | 43.0 |
| [悪意のあるChromeおよびFirefox拡張機能が暗号資産トレーダーのセッションとウォレットデータを窃取](https://socket.dev/blog/chrome-firefox-crypto-data-theft) | 22.0 | 20.0 | 48.0 |
| [「Adobe Acrobat/Reader」にセキュリティ更新 - 脆弱性32件を解消](https://www.security-next.com/190081) | 22.0 | 20.0 | 42.0 |
| [クラウドWebアプリケーションにおける脅威マトリクス：脅威の対応関係を可視化する](https://www.microsoft.com/en-us/security/blog/2026/09/09/threat-matrix-mapping-threats-across-cloud-web-applications/) | 22.0 | 20.0 | 42.0 |
| [民間企業をサイバー作戦へ参加させる米国の新制度 ほか [Scan PREMIUM Monthly Executive Summary 2026年8月度]](https://scan.netsecurity.ne.jp/article/2026/09/10/56192.html) | 21.0 | 20.0 | 42.0 |
| [東京科学大学の情報基盤に不正アクセス、個人情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/09/10/56191.html) | 21.0 | 20.0 | 42.0 |
| [NEXCO東日本の東京外環プロジェクトホームページで不正アクセス疑い](https://scan.netsecurity.ne.jp/article/2026/09/10/56190.html) | 21.0 | 20.0 | 42.0 |
| [非表示のシートが含まれていることに気づかないまま掲載 ～ 大川市ホームページで公開した名簿データ](https://scan.netsecurity.ne.jp/article/2026/09/10/56188.html) | 21.0 | 20.0 | 42.0 |
| [スプーンのウェブサイトが改ざん被害、偽のセキュリティ確認画面等が表示される事象](https://scan.netsecurity.ne.jp/article/2026/09/10/56187.html) | 21.0 | 20.0 | 42.0 |
| [耳鼻咽喉科の廃棄予定の問診票を裏紙使用し患者に交付](https://scan.netsecurity.ne.jp/article/2026/09/10/56186.html) | 21.0 | 20.0 | 42.0 |
| [クラウド環境の不正アクセス制限に脆弱性、入居申込者情報が流出した可能性](https://scan.netsecurity.ne.jp/article/2026/09/10/56185.html) | 21.0 | 20.0 | 42.0 |
| [9 / 26 開催「Platform Engineering Kaigi 2026」にスリーシェイクのエンジニア 鈴木勝史氏 加藤泰隆氏が登壇](https://scan.netsecurity.ne.jp/article/2026/09/10/56184.html) | 21.0 | 20.0 | 42.0 |
| [被害額2,108億円 前年同期比+632億円 ～ 令和8(2026)年7月末における特殊詐欺の認知検挙状況](https://scan.netsecurity.ne.jp/article/2026/09/10/56183.html) | 21.0 | 20.0 | 42.0 |
| [弁護士が知っておくべきサイバーセキュリティ 12 のポイント ～ 東京弁護士会](https://scan.netsecurity.ne.jp/article/2026/09/10/56182.html) | 21.0 | 20.0 | 42.0 |
| [権威 DNS サーバ Knot DNS が複数のセキュリティ修正を公開](https://scan.netsecurity.ne.jp/article/2026/09/10/56180.html) | 21.0 | 20.0 | 42.0 |
| [GMOナショナルセキュリティが国家レベルのサイバー脅威や経済安全保障上のリスクを分析する専門部署「インテリジェンス課」を新設](https://scan.netsecurity.ne.jp/article/2026/09/10/56179.html) | 21.0 | 20.0 | 42.0 |
| [10 / 27・28 開催「地方自治情報化推進フェア 2026」に HENNGE が出展、赤瀬礼旺氏と板垣慎介氏による講演も](https://scan.netsecurity.ne.jp/article/2026/09/10/56178.html) | 21.0 | 20.0 | 42.0 |
| [スリーシェイクの早川大貴氏、クラウドネイティブ技術を推進する CNCF Ambassadors 2026-2028 に就任](https://scan.netsecurity.ne.jp/article/2026/09/10/56177.html) | 21.0 | 20.0 | 42.0 |
| [GMOサイバーセキュリティ byイエラエが台湾の国立台北科技大学および電信技術センターと低軌道（LEO）衛星のサイバーセキュリティで業務提携](https://scan.netsecurity.ne.jp/article/2026/09/10/56176.html) | 21.0 | 20.0 | 42.0 |
| [日本のセキュリティ課題は「ツール導入」から「組織とプロセス」へ移行 ～ サイバーリーズン分析](https://scan.netsecurity.ne.jp/article/2026/09/10/56174.html) | 21.0 | 20.0 | 42.0 |
| [バックアップデータがAIの金鉱に--Cohesityが狙うセカンダリーデータの新価値](https://japan.zdnet.com/article/35252439/) | 21.0 | 20.0 | 42.0 |
| [MariaDBに「USAGEだけ」で管理者を乗っ取れる脆弱性 認証情報を書き換えるその手口](https://atmarkit.itmedia.co.jp/ait/articles/2609/10/news016.html) | 21.0 | 20.0 | 42.0 |
| [Smashing Security podcast #484: サイトが無音であなたを追跡する仕組み](https://grahamcluley.com/smashing-security-podcast-484/) | 20.0 | 20.0 | 42.0 |
| [OpenSSLの新しいアルファ版ビルドでポスト量子暗号を高速化](https://www.helpnetsecurity.com/2026/09/10/openssl-4-1-0-alpha1-released/) | 20.0 | 20.0 | 42.0 |
| [【ガートナー警鐘】サイバー保険「入っても補償なし」…？知らないと怖い「免責条項」](https://www.sbbit.jp/article/fj/186801?ref=rss) | 20.0 | 20.0 | 42.0 |
| [CISA長官、最悪の事態を防ぐため同庁は迅速に変わる必要があると発言](https://therecord.media/cisa-hiring-nick-andersen-warning) | 20.0 | 20.0 | 42.0 |
| [Mythosの脆弱性情報が人手による処理の限界に直面](https://www.darkreading.com/application-security/mythos-vulnerability-firehose-hits-human-bottleneck) | 20.0 | 20.0 | 42.0 |
| [Skullcandy Dime 3イヤホンにBluetoothハイジャッキングの脆弱性が判明](https://www.bleepingcomputer.com/news/security/skullcandy-dime-3-earbuds-expose-users-to-bluetooth-hijacking/) | 20.0 | 20.0 | 42.0 |

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
