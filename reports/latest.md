# 📡 サイレーダー 2026-09-18 11:00 JST

このレポートは、2026-09-18 05:00 JST〜2026-09-18 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 54
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 27

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cisco alerts customers to second actively exploited zero-day in as many days](#topic-32957) | 47.0 | 64.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [New RatHat Android malware uses AI to automate device control](#topic-33352) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-33352"></a>

### 1. New RatHat Android malware uses AI to automate device control

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠n⁠d⁠r⁠o⁠i⁠d</nobr> / <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

RatHatと呼ばれる新しいAndroidマルウェアが確認され、感染端末の遠隔操作を支援するAI機能を備えているとされています。
攻撃者が端末内の操作をより効率的に進められる可能性がある点が特徴です。
AIを悪用して端末操作を支援するマルウェアは、従来型のモバイル脅威とは異なる運用のしやすさを攻撃者に与える懸念があります。
Android利用環境では、検知や利用者教育だけでなく、端末管理の観点でも注意が必要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Android端末のアプリ導入元や権限付与の状況を改めて確認する。
- モバイル端末管理（MDM/MAM）やEDRで、不審な挙動や権限の過剰要求を監視する。
- AI機能をうたう不審なアプリや、想定外の端末制御挙動に関する注意喚起を周知する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New RatHat Android malware uses AI to automate device control](https://www.bleepingcomputer.com/news/security/new-rathat-android-malware-uses-ai-to-automate-device-control/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-32957"></a>

### 1. Cisco alerts customers to second actively exploited zero-day in as many days

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 47.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Identity Services Engine（ISE）のAPIに認証回避の脆弱性があり、未認証のリモート攻撃者による悪用が報告されています。
Ciscoは修正版ソフトウェアを公開しており、現時点で有効な回避策は案内されていません。
ISEは認証やアクセス制御の中核を担う製品であり、影響を受けると管理面への不正アクセスにつながるおそれがあります。
さらに、短期間に別のCisco脆弱性も悪用観測が伝えられており、運用現場での優先度が高い事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
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

- Cisco ISE / ISE-PIC の影響対象バージョンを確認し、案内済みの修正版への更新を優先する。
- 管理インターフェースや関連APIへの到達範囲を見直し、不要な露出がないか確認する。
- 認証回避の兆候として、管理系ログや想定外のアクセスを重点的に点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-76460 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-76461 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Identity Services Engine | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-76460](https://nvd.nist.gov/vuln/detail/CVE-2026-76460) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco alerts customers to second actively exploited zero-day in as many days](https://cyberscoop.com/cisco-ise-zero-day-cve-2026-76460/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco drops another exploited zero-day, this time a perfect 10](https://www.theregister.com/security/2026/09/17/cisco-drops-another-exploited-zero-day-this-time-a-perfect-10/5297180) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-76460: A critical Cisco ISE authentication bypass under active exploita](https://www.bitsight.com/blog/critical-vulnerability-alert-cve-2026-76460-cisco-ise-authentication-bypass) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Unauthenticated attackers are bypassing Cisco ISE’s management interface (CVE-20](https://www.helpnetsecurity.com/2026/09/17/cisco-ise-vulnerability-exploited-cve-2026-76460/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Identity Services Engine Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ISE-ABP-VNSW7Tn5) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
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
| [ターゲットは「セッショントークンと API キー」Okta が警告する AI アクセス権の闇取引](https://scan.netsecurity.ne.jp/article/2026/09/18/56263.html) | 26.0 | 20.0 | 42.0 |
| [レノボ・エンタープライズ・ソリューションズ張社長が語るAI推論時代とデータセンターの未来](https://japan.zdnet.com/article/35252319/) | 26.0 | 20.0 | 42.0 |
| [「Factorio」の乱数生成器を解析して「レジェンド品質のアイテム」が出る未来を予測する試み](https://gigazine.net/news/20260918-reversing-factorio-rng/) | 25.0 | 20.0 | 43.0 |
| [AIコーディングエージェントの0クリックRCE脆弱性で攻撃者に王国の鍵が渡る可能性](https://www.theregister.com/security/2026/09/17/ai-coding-agents-0-click-rce-flaw-could-hand-attackers-keys-to-the-kingdom/5297335) | 25.0 | 20.0 | 42.0 |
| [DB管理ツール「pgAdmin 4」に複数の脆弱性 - 修正版が公開](https://www.security-next.com/190497) | 22.0 | 20.0 | 42.0 |
| [塩尻警察署で個人情報が記載された「交通安全施設損壊事案報告書」等が所在不明に](https://scan.netsecurity.ne.jp/article/2026/09/18/56275.html) | 21.0 | 20.0 | 42.0 |
| [マネジメントサービスセンターのホームページに不正アクセス、管理者権限の取得や改ざんを確認](https://scan.netsecurity.ne.jp/article/2026/09/18/56274.html) | 21.0 | 20.0 | 42.0 |
| [フィッシング詐欺等によるものとみられる不正アクセス・不正取引を確認 ～ 静銀ティーエム証券](https://scan.netsecurity.ne.jp/article/2026/09/18/56273.html) | 21.0 | 20.0 | 42.0 |
| [ウェブ画面設定誤りが原因「オペラ銀河鉄道の夜」合唱申込フォーム入力の個人情報が閲覧可能に](https://scan.netsecurity.ne.jp/article/2026/09/18/56272.html) | 21.0 | 20.0 | 42.0 |
| [サーバ上にバックドア等の不正プログラムを設置 ～ 繋が運営するコーポレートサイトに不正アクセス](https://scan.netsecurity.ne.jp/article/2026/09/18/56271.html) | 21.0 | 20.0 | 42.0 |
| [顧客情報の一括エクスポートを確認 ～ カインドオルが利用するECプラットフォームに不正アクセス](https://scan.netsecurity.ne.jp/article/2026/09/18/56270.html) | 21.0 | 20.0 | 42.0 |
| [警察官を名乗る者から「捜査に必要と求められ」～ 安藤ハザマの名刺情報 5,000件が流出](https://scan.netsecurity.ne.jp/article/2026/09/18/56269.html) | 21.0 | 20.0 | 42.0 |
| [任意の OS コマンド実行の恐れ Lite-On 製 O-RU「FF-RFI079I4」「FF-RFI078I4」に脆弱性](https://scan.netsecurity.ne.jp/article/2026/09/18/56268.html) | 21.0 | 20.0 | 42.0 |
| [Android アプリ「【保護者専用】まなびポケット」にアクセス制限不備の脆弱性](https://scan.netsecurity.ne.jp/article/2026/09/18/56267.html) | 21.0 | 20.0 | 42.0 |
| [Cisco Secure Email Gateway に SQLインジェクションの脆弱性 すでに悪用も確認](https://scan.netsecurity.ne.jp/article/2026/09/18/56266.html) | 21.0 | 20.0 | 42.0 |
| [登山アプリ「YAMAP」Android 版にアクセス制限不備の脆弱性](https://scan.netsecurity.ne.jp/article/2026/09/18/56265.html) | 21.0 | 20.0 | 42.0 |
| [任天堂、Nintendo Switch の脆弱性を公表 ～ QRコード読み取りで情報漏えいの恐れ](https://scan.netsecurity.ne.jp/article/2026/09/18/56264.html) | 21.0 | 20.0 | 42.0 |
| [xxx.soumu.go.jp などのサブドメインも拒否に ～ 総務省を装うフィッシングメール対策強化](https://scan.netsecurity.ne.jp/article/2026/09/18/56262.html) | 21.0 | 20.0 | 42.0 |
| [WhatsApp セキュリティアドバイザリを公開](https://scan.netsecurity.ne.jp/article/2026/09/18/56261.html) | 21.0 | 20.0 | 42.0 |
| [「EU CRAで考える製品セキュリティ品質」GMOイエラエ伊藤氏が「第11回 IoTセキュリティフォーラム 2026」で登壇](https://scan.netsecurity.ne.jp/article/2026/09/18/56260.html) | 21.0 | 20.0 | 42.0 |
| [脆弱性診断の結果をどう読む？ CVSSだけで改修順を決めてはいけない理由](https://www.itmedia.co.jp/enterprise/articles/2609/18/news009.html) | 21.0 | 20.0 | 42.0 |
| [トークンを守るには「盗まれる前提」の対策を NISTとCISAが指針を発表](https://www.itmedia.co.jp/enterprise/articles/2609/18/news019.html) | 21.0 | 20.0 | 42.0 |
| [「システムが動けば復旧完了」ではない--「信頼できる状態」に戻すための条件](https://japan.zdnet.com/article/35252514/) | 21.0 | 20.0 | 42.0 |
| [CISA ICS Advisory / ICS Medical Advisory（2026年09月17日）](https://jvn.jp/vu/JVNVU91030326/) | 20.0 | 20.0 | 42.0 |
| [DokployにおけるOSコマンドインジェクションの脆弱性](https://jvn.jp/vu/JVNVU94707104/) | 20.0 | 20.0 | 42.0 |
| [アドバンテック、産業用セルラールーター「EKI-1642WI-JA」の「JC-STAR」★1取得を発表](https://internet.watch.impress.co.jp/docs/news/2141952.html) | 20.0 | 20.0 | 42.0 |
| [CISA、毎週の脆弱性まとめを廃止しリスク重視へ転換](https://www.darkreading.com/cyber-risk/cisa-ditches-weekly-vuln-roundups-risk-based-focus) | 20.0 | 20.0 | 42.0 |

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
