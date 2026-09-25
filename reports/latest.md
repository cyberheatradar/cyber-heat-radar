# 📡 サイレーダー 2026-09-25 11:00 JST

このレポートは、2026-09-25 05:00 JST〜2026-09-25 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 63
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 37

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [米CISA、「Adobe Commerce」「WSO2」の脆弱性悪用を警告](#topic-34246) | 39.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [New Carbonato malware uses AI agents to hijack exposed Docker hosts](#topic-34298) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-34246"></a>

### 1. 米CISA、「Adobe Commerce」「WSO2」の脆弱性悪用を警告

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

米CISAは、Adobe CommerceとWSO2の脆弱性が実際に悪用されているとして注意喚起を行いました。
米行政機関に対しては、侵害の有無を確認しつつ、速やかな対応を取るよう求めています。
脆弱性の存在だけでなく悪用が確認されている点から、影響が現実化している可能性があるため注目されています。
対象製品を利用する組織は、通常のパッチ対応に加えて侵害確認も意識する必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象製品の利用有無を確認し、該当する場合はベンダーや公的機関の案内に沿って優先的に対処する。
- 関連する侵害兆候の有無を確認し、認証情報や管理画面への不審なアクセス履歴を点検する。
- 公開された修正情報や緩和策がある場合は適用状況を見直し、未適用なら早急に計画を立てる。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Adobe | 言及あり | 0.80 | — |
| 製品 | Adobe Commerce | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [米CISA、「Adobe Commerce」「WSO2」の脆弱性悪用を警告](https://www.security-next.com/190675) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34298"></a>

### 2. New Carbonato malware uses AI agents to hijack exposed Docker hosts

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Carbonatoと呼ばれる新しいマルウェアが、外部に露出したDockerデーモンを持つホストを狙っていると報じられています。
報道によれば、AIエージェントの仕組みを利用して対象環境に入り込み、制御を奪う手口が確認されています。
Dockerの公開設定や認証不備があると、コンテナ基盤がそのまま侵害されるおそれがあるため注意が必要です。
AI関連の仕組みが攻撃に組み込まれることで、従来の自動化型マルウェアよりも対応の見極めが難しくなる可能性があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Dockerデーモンが外部公開されていないか、認証やアクセス制御が適切かを確認する。
- コンテナ基盤の監査ログや不審なコンテナ作成・実行の兆候を点検する。
- インターネット公開が必要な場合は最小権限化し、ネットワーク境界で到達性を制限する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New Carbonato malware uses AI agents to hijack exposed Docker hosts](https://www.bleepingcomputer.com/news/security/new-carbonato-malware-uses-ai-agents-to-hijack-exposed-docker-hosts/) | <nobr>内容確認・補足情報</nobr> |

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
| [VIP・GOLDランク顧客の情報流出の可能性 ～ ファイブフォックスへのランサムウェア攻撃](https://scan.netsecurity.ne.jp/article/2026/09/25/56300.html) | 29.0 | 30.0 | 42.0 |
| [実行犯が示唆したダークウェブでの情報公開は確認されず ～ ワシントンホテルにランサムウェア攻撃](https://scan.netsecurity.ne.jp/article/2026/09/25/56299.html) | 29.0 | 30.0 | 42.0 |
| [ランサムウェアの被害報告件数が過去最多に ～ 警察庁 サイバー警察局便り](https://scan.netsecurity.ne.jp/article/2026/09/25/56296.html) | 29.0 | 30.0 | 42.0 |
| [カレンダーへの招待状を装うマルウェア感染攻撃が増加--身を守る方法](https://japan.zdnet.com/article/35252829/) | 29.0 | 20.0 | 42.0 |
| [MacSyncマルウェアが公開iCloudカレンダーを悪用して新たなペイロードを配信](https://www.bleepingcomputer.com/news/security/macsync-malware-uses-public-icloud-calendars-to-deliver-new-payloads/) | 28.0 | 20.0 | 42.0 |
| [「ServiceNow AI Platform」にSQLiなど複数脆弱性 - 修正版を提供](https://www.security-next.com/190682) | 27.0 | 20.0 | 42.0 |
| [これがコンサルの次の勝ち方…？デロイト新設「AI実装のプロ集団」の能力がスゴイ理由](https://www.sbbit.jp/article/cont1/186092?ref=rss) | 27.0 | 20.0 | 42.0 |
| [Google、リアルタイムで表情豊かに話すAIアバター「Gemini 3.8 Live with Live Avatar」提供開始 画像1枚で独自アバターも](https://www.itmedia.co.jp/news/article/2609/25/2000001730/) | 26.0 | 20.0 | 42.0 |
| [シャドー AI からエージェントまで一括保護 ～ クラウドストライクが AIDR「Falcon Guardian」発表](https://scan.netsecurity.ne.jp/article/2026/09/25/56294.html) | 26.0 | 20.0 | 42.0 |
| [AIにコードを書かせ放題で大丈夫？ 開発現場に迫る「AIコスト」の見えない問題](https://atmarkit.itmedia.co.jp/ait/articles/2609/25/news042.html) | 26.0 | 20.0 | 42.0 |
| [メタの新AIエージェント「Muse」 機密コンピューティングに注目](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/052100111/092400186/) | 26.0 | 20.0 | 42.0 |
| [AI変革に手応えあり](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/041700482/091700020/) | 26.0 | 20.0 | 42.0 |
| [「SaaSの死」は幻想 AIが代替できるわけがない](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/052100112/091700147/) | 26.0 | 20.0 | 42.0 |
| [オープンソースエージェント3種を悪用し、Fortune 500の大手ホスピタリティ企業や米国大手航空会社など25以上の組織に侵入した攻撃者](https://www.theregister.com/security/2026/09/25/crook-used-three-open-source-agents-to-break-into-a-fortune-500-hospitality-company-a-major-us-airline-and-25-other-orgs/5299012) | 25.0 | 20.0 | 42.0 |
| [SalesbleedがSalesforce Agentsを悪用してSlackフィッシングを可能にする](https://www.darkreading.com/application-security/salesbleed-exploits-salesforce-agents-slack-phishing) | 25.0 | 20.0 | 42.0 |
| [自律型AIによるハッキングが提起する法的責任の難問](https://www.securityweek.com/autonomous-ai-hacks-raise-thorny-questions-of-legal-accountability/) | 25.0 | 20.0 | 42.0 |
| [再有効化された GitHub Actions により数千のリポジトリが Mini Shai-Hulud にさらされる](https://socket.dev/blog/mini-shai-hulud-actions) | 22.0 | 45.0 | 42.0 |
| [アメリカ軍によるイランの小学校へのミサイル攻撃はデータベースの情報更新を怠りAIを過信したことが一因だったとの報道](https://gigazine.net/news/20260925-iran-school-maven-ai-kill-chain/) | 22.0 | 20.0 | 42.0 |
| [Webアプリの乱立でリスクが見えなくなっている!?―継続的な脆弱性診断が実現する統合セキュリティ管理](https://news.mynavi.jp/techplus/kikaku/20260925-4973555/) | 21.0 | 20.0 | 42.0 |
| [現代のサイバーセキュリティ人材戦略に不可欠な要素](https://ascii.jp/elem/000/004/436/4436701/?rss=) | 21.0 | 20.0 | 42.0 |
| [今日もどこかで情報漏えい 第52回「2026年8月の情報漏えい」約一割で逮捕・懲戒・行政指導](https://scan.netsecurity.ne.jp/article/2026/09/25/56306.html) | 21.0 | 20.0 | 42.0 |
| [カルビーのプロ野球チップス関連サービス「PhotoGoods」で個人情報漏えいの可能性](https://scan.netsecurity.ne.jp/article/2026/09/25/56305.html) | 21.0 | 20.0 | 42.0 |
| [ApplyNow 提供の採用管理プラットフォームに不正アクセス、マイナンバー含む個人データが漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/09/25/56304.html) | 21.0 | 20.0 | 42.0 |
| [極東開発工業子会社の日本トレクス、不正アクセスによるシステム障害を発表](https://scan.netsecurity.ne.jp/article/2026/09/25/56303.html) | 21.0 | 20.0 | 42.0 |
| [社内調査で発覚 ～ ライツフォル、外部 Q&A サイトにおける過去の「広告明示なし投稿」を公表](https://scan.netsecurity.ne.jp/article/2026/09/25/56302.html) | 21.0 | 20.0 | 42.0 |
| [京都パープルサンガでメール誤送信、ファンクラブ会員情報15,612件が漏えい](https://scan.netsecurity.ne.jp/article/2026/09/25/56301.html) | 21.0 | 20.0 | 42.0 |
| [早稲田大学比較法研究所、10月4日に公開講演会「医療DXとサイバーセキュリティ」をハイブリッド開催](https://scan.netsecurity.ne.jp/article/2026/09/25/56298.html) | 21.0 | 20.0 | 42.0 |
| [サイバーセキュリティ企業の「信頼と組織」を強化 ～ プルーフポイントが最高法務責任者と最高人事責任者を新任へ](https://scan.netsecurity.ne.jp/article/2026/09/25/56297.html) | 21.0 | 20.0 | 42.0 |
| [HENNGE One、個人情報・情報資産管理プラットフォーム「Flows」と SSO 連携](https://scan.netsecurity.ne.jp/article/2026/09/25/56295.html) | 21.0 | 20.0 | 42.0 |
| [グーグル、「Chrome」のパッチ適用を高速化する新戦略--リリース責任者に聞く狙い](https://japan.zdnet.com/article/35252785/) | 21.0 | 20.0 | 42.0 |
| [全日空商事でギフト不正交換 原因は第三者の不正アクセス](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/031800050/091400091/) | 21.0 | 20.0 | 42.0 |
| [ViewSonic vCastにおける複数の脆弱性](https://jvn.jp/vu/JVNVU96941087/) | 20.0 | 20.0 | 42.0 |
| [Norwegian Cruise Lineのドアアクセスコントローラにおける認証不備の脆弱性](https://jvn.jp/vu/JVNVU96565230/) | 20.0 | 20.0 | 42.0 |
| [CISA ICS Advisory / ICS Medical Advisory（2026年09月24日）](https://jvn.jp/vu/JVNVU93222287/) | 20.0 | 20.0 | 42.0 |
| [CISAによるバイオテック向けサイバー防御強化を求める下院・上院議員の法案提案](https://cyberscoop.com/biotech-critical-infrastructure-cybersecurity-legislation/) | 20.0 | 20.0 | 42.0 |
| [SectopRATが正規アプリケーションに潜伏して再来](https://www.darkreading.com/cyberattacks-data-breaches/sectoprat-returns-hiding-inside-legitimate-application) | 20.0 | 20.0 | 42.0 |
| [Salt Typhoonハッキングを受け、通信事業者向けサイバー規則の自主導入を求める法案が提出される](https://therecord.media/lawmakers-introduce-bill-for-voluntary-telecom-cyber-rules) | 20.0 | 20.0 | 42.0 |

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
