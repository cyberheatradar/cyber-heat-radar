# 📡 サイレーダー 2026-11-05 11:00 JST

このレポートは、2026-11-05 05:00 JST〜2026-11-05 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 51
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 26

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2025-20333: Cisco ASA/FTD persistence mechanism update](#topic-203) | 58.0 | 74.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [Zyxel fixes zero-day exploited to hack nearly 1,000 network switches](#topic-41379) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-203"></a>

### 1. CVE-2025-20333: Cisco ASA/FTD persistence mechanism update

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 58.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

CISAとCiscoは、Cisco Secure Firewall ASA/FTDに関連する脅威対応情報を更新し、ArcaneDoorとされる攻撃者が、既知の修正版へ更新しても残る持続化の仕組みを新たに使っていると説明しました。
この持続化はFXOS上に存在するとされ、初期侵入は2025年9月に修正されたCVE-2025-20333とCVE-2025-20362の悪用から始まった可能性が示されています。
脆弱性の修正だけでは十分でない可能性があり、更新済み機器でも継続的な侵害確認が必要になるためです。境界機器は組織全体への侵入口になりやすく、影響範囲が大きい点でも注目されます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 7 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ASA/FTDを利用している環境では、修正版適用済みでも侵害の有無を別途確認すること。
- CISAやCiscoの最新勧告を確認し、該当機器の調査・隔離・再構築の要否を判断すること。
- VPN Web Server関連の脆弱性対策だけでなく、管理面のアクセス制御やログ監視も見直すこと。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-20333 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2025-20362 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-111497 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-119977 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-97229 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-20333](https://nvd.nist.gov/vuln/detail/CVE-2025-20333) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Weekly Report: Cisco Secure Firewall ASAおよびFTD Softwareにサービス運用妨害（DoS）の脆弱性](https://www.jpcert.or.jp/wr/2026/wr261105.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CSuite Targets US and EU Organizations with Device-Code Phishing and Remote Acce](https://any.run/cybersecurity-blog/csuite-attack-analysis/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [OctLurk and SilkLurk: newly identified tailored backdoors in cyber-espionage cam](https://securelist.com/octlurk-silklurk-backdoors-central-asia/120840/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [US Threat Landscape Alert: 30 Active Malware Families Ranked by Real Sandbox Dat](https://any.run/cybersecurity-blog/usa-top-30-threats-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [From edge appliance to enterprise compromise: Multi-stage Linux intrusion via F5](https://www.microsoft.com/en-us/security/blog/2026/05/22/from-edge-appliance-to-enterprise-compromise-multi-stage-linux-intrusion-via-f5-and-confluence/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Continued Evolution of Persistence Mechanism Against Cisco Secure Firewall Adapt](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-persist-CISAED25-03) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Weekly Report: JPCERT/CCが「Cisco ASAおよびFTDにおける複数の脆弱性（CVE-2025-20333、CVE-2025-2036](https://www.jpcert.or.jp/wr/2026/wr260430.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-41379"></a>

### 2. Zyxel fixes zero-day exploited to hack nearly 1,000 network switches

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Zyxelは、GS1900シリーズのネットワークスイッチに存在したゼロデイ脆弱性への修正を公表しました。
報道によると、この脆弱性は実際に悪用され、世界で約1,000台の機器が侵害され、設定ファイルや認証情報が取得されたとされています。
ネットワーク機器は組織内の通信基盤を担うため、侵害されると広範な影響につながるおそれがあります。
すでに悪用が確認されている点から、単なる脆弱性情報ではなく、優先度の高い対応対象と見なす必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- GS1900シリーズの利用有無を確認し、提供済みの修正を速やかに適用する。
- 設定ファイルや認証情報の流出可能性を考慮し、関連アカウントのパスワード変更や認証情報の点検を行う。
- 機器の管理画面やログを確認し、不審な設定変更やアクセスの痕跡がないかを確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-107441 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-7273 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Zyxel fixes zero-day exploited to hack nearly 1,000 network switches](https://www.bleepingcomputer.com/news/security/zyxel-fixes-zero-day-exploited-to-hack-nearly-1-000-network-switches/) | <nobr>内容確認・補足情報</nobr> |

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
| [ドン・キホーテ委託先にランサムウェア攻撃、時計修理を依頼者の個人情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/11/05/56678.html) | 29.0 | 30.0 | 42.0 |
| [Smashing Security podcast #491: AIエージェントが銀行を震え上がらせる理由](https://grahamcluley.com/smashing-security-podcast-491/) | 28.0 | 30.0 | 42.0 |
| [重大なRailsの脆弱性が脆弱なサーバーを危険にさらす](https://www.darkreading.com/application-security/critical-rails-bug-derail-vulnerable-servers) | 28.0 | 20.0 | 42.0 |
| [Vercelが盗まれたセッションCookie攻撃への新たな対策を導入](https://www.bleepingcomputer.com/news/security/vercel-rolls-out-new-protection-against-stolen-session-cookie-attacks/) | 28.0 | 20.0 | 42.0 |
| [マルチベンダーのAIエージェント活用に向けて「ガバナンスの統一」に注力せよ](https://japan.zdnet.com/article/35254360/) | 26.0 | 20.0 | 42.0 |
| [Cisco、AI エージェントの暴走を検知する「Project Quarry」をオープンソース化](https://scan.netsecurity.ne.jp/article/2026/11/05/56682.html) | 26.0 | 20.0 | 42.0 |
| [「Muse」を使っていなくてもAIエージェントが非公開のメッセージにアクセスできる仕組みとは](https://japan.zdnet.com/article/35254098/) | 26.0 | 20.0 | 42.0 |
| [「マインクラフト」で50体のAIエージェントによる協調動作を試す](https://japan.zdnet.com/article/35254319/) | 26.0 | 20.0 | 42.0 |
| [仏銀行Credit Mutuel Arkeaにサイバー攻撃 委託先経由で侵入、不正送金の被害は約1億ユーロか](https://www.itmedia.co.jp/news/article/2611/05/2000002891/) | 21.0 | 20.0 | 42.0 |
| [仏血液センターの冷蔵設備にサイバー攻撃 温度設定を不正変更、血液製剤への被害は回避](https://www.itmedia.co.jp/news/article/2611/05/2000002890/) | 21.0 | 20.0 | 42.0 |
| [2026年のフィッシング動向と対策の現状 ～ Internet Week 2026](https://scan.netsecurity.ne.jp/article/2026/11/05/56681.html) | 21.0 | 20.0 | 42.0 |
| [GMOペイメントゲートウェイ、ライフカード向けサービスで顧客情報一部流出の可能性](https://scan.netsecurity.ne.jp/article/2026/11/05/56680.html) | 21.0 | 20.0 | 42.0 |
| [ライフネット生命の一部システムに不正アクセス、KDDIが保有する顧客情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/11/05/56679.html) | 21.0 | 20.0 | 42.0 |
| [日本郵政グループ労働組合に不正アクセス、4万件以上の組合員情報が漏えい](https://scan.netsecurity.ne.jp/article/2026/11/05/56677.html) | 21.0 | 20.0 | 42.0 |
| [障害者支援アプリ運営委託事業者ミラボに不正アクセス、設計段階で想定していなかった不備](https://scan.netsecurity.ne.jp/article/2026/11/05/56676.html) | 21.0 | 20.0 | 42.0 |
| [ドトールコーヒーのシステムに不正アクセス、従業員及び退職者 計951名の個人情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/11/05/56675.html) | 21.0 | 20.0 | 42.0 |
| [ギフティへの不正アクセスによるeギフトの不正発行、約5.5億円の損失見込み](https://scan.netsecurity.ne.jp/article/2026/11/05/56674.html) | 21.0 | 20.0 | 42.0 |
| [LINE連携基盤「COMSBI エンタープライズ基盤」に不正アクセス](https://scan.netsecurity.ne.jp/article/2026/11/05/56673.html) | 21.0 | 20.0 | 42.0 |
| [バリューデザインへの不正アクセス、一部のモスカード番号等が流出](https://scan.netsecurity.ne.jp/article/2026/11/05/56672.html) | 21.0 | 20.0 | 42.0 |
| [ヤマハ製 YMS-VPN8 および YMS-VPN8-CP に引用符で囲まれていないファイルパスの脆弱性](https://scan.netsecurity.ne.jp/article/2026/11/05/56671.html) | 21.0 | 20.0 | 42.0 |
| [Yamaha LAN Monitor for Windows のインストーラにDLL読み込みに関する脆弱性](https://scan.netsecurity.ne.jp/article/2026/11/05/56670.html) | 21.0 | 20.0 | 42.0 |
| [ヤマハ製 NWR100 に複数の脆弱性](https://scan.netsecurity.ne.jp/article/2026/11/05/56669.html) | 21.0 | 20.0 | 42.0 |
| [仏銀行サイバー攻撃 177億円流出](https://news.yahoo.co.jp/pickup/6601387?source=rss) | 20.0 | 20.0 | 42.0 |
| [民主党が議会を掌握するとサイバーセキュリティはどう変わるのか](https://cyberscoop.com/democrats-congress-cybersecurity-cisa-ai-priorities/) | 20.0 | 20.0 | 42.0 |
| [Apple、iCloudを監視対象に　公開共有リンクのスキャンを開始](https://www.theregister.com/security/2026/11/04/apple-turns-icloud-into-spy-cloud-will-start-looking-at-public-share-links/5307681) | 20.0 | 20.0 | 42.0 |
| [スペインのITプロバイダーAmadeusへの攻撃後、アジアの航空会社で相次ぐデータ侵害の発表](https://therecord.media/asian-airlines-announce-data-breach-it-provider-incident) | 20.0 | 20.0 | 42.0 |

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
