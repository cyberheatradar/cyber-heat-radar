# 📡 サイレーダー 2026-09-29 11:00 JST

このレポートは、2026-09-29 05:00 JST〜2026-09-29 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 68
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 42

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Citrix patches actively exploited NetScaler zero-days after a weekend of unofficial warnings](#topic-34525) | 47.0 | 64.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [Carbonato Botnet Puts an AI Agent on Hacked Docker Hosts](#topic-34819) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-34819"></a>

### 1. Carbonato Botnet Puts an AI Agent on Hacked Docker Hosts

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Carbonato Botnetに関する報告では、公開されたDockerホスト上でAIエージェントの仕組みが悪用され、Telegram経由でコマンド実行に使われたとされています。
また、AI関連APIキーの窃取が狙われた可能性が示されています。AIサービスの利用拡大に伴い、APIキーや認証情報が攻撃の標的になりやすくなっています。
Dockerの公開設定やコンテナ運用の不備があると、侵入後にAI関連資産へ波及するおそれがあります。

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

- Dockerホストの公開範囲と不要な管理ポートの露出を点検する。
- AI APIキーや各種シークレットの保管・権限・ローテーションを見直す。
- コンテナ内の不審な外部通信や、Telegram等を介した想定外の操作痕跡を監視する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Carbonato Botnet Puts an AI Agent on Hacked Docker Hosts](https://www.darkreading.com/identity-access-management-security/carbonato-botnet-ai-agent-hacked-docker-hosts) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-34525"></a>

### 1. Citrix patches actively exploited NetScaler zero-days after a weekend of unofficial warnings

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 47.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Citrixは、NetScaler ADCおよびNetScaler Gatewayに存在する2件の重大な脆弱性（CVE-2026-88771、CVE-2026-88772）について、実際の攻撃で悪用されていることを確認し、修正更新を公開しました。
公開情報では、これらはリモートコード実行につながるおそれがあるとされ、複数のセキュリティ組織やJPCERT/CCでも注意喚起が出ています。
ネットワーク境界で使われやすい製品の脆弱性で、侵害されると影響範囲が広がりやすいためです。すでに悪用観測がある点から、通常の脆弱性対応よりも迅速な評価と適用が求められます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
- 実悪用・ゼロデイ文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象のNetScaler ADC/Gatewayが影響を受ける版かを確認し、提供済みの修正更新を優先適用する。
- 外部公開しているNetScaler機器については、更新前後を問わず不審なアクセスや設定変更、侵害兆候の確認を行う。
- 資産一覧と保守窓口を整理し、同種の境界装置で今後も迅速に更新判断できる体制を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-88771 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-88772 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-88771](https://nvd.nist.gov/vuln/detail/CVE-2026-88771) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Citrix patches actively exploited NetScaler zero-days after a weekend of unoffic](https://cyberscoop.com/citrix-zero-days-delayed-disclosure/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: NetScaler Zero Days CVE-2026-88771 and CVE-2026-88772 Exploited in](https://unit42.paloaltonetworks.com/netscaler-zero-days-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-88771 and CVE-2026-88772: Two Critical Citrix NetScaler Flaws Under Act](https://www.bitsight.com/blog/critical-vulnerability-alert-cve-2026-88771-cve-2026-88772-citrix-netscaler-flaws-under-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zero-Day Exploitation of Citrix NetScaler ADC and Gateway: CVE-2026-88771 and CV](https://www.rapid7.com/blog/post/etr-zero-day-exploitation-of-citrix-netscaler-adc-and-gateway-cve-2026-88771-and-cve-2026-88772) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix NetScaler RCE zero-days exploited globally for weeks (CVE-2026-88771, CVE](https://www.helpnetsecurity.com/2026/09/28/citrix-netscaler-rce-zero-days-exploited-for-weeks-cve-2026-88771-cve-2026-88772/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: NetScaler ADCおよびNetScaler Gatewayにおける複数の脆弱性（CVE-2026-88771、CVE-2026-88772等](https://www.jpcert.or.jp/at/2026/at260029.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix Confirms 2 NetScaler Zero-Days After Admins Pulled the Plug](https://www.securityweek.com/citrix-confirms-2-netscaler-zero-days-after-admins-pulled-the-plug/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（2件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Keioがランサムウェア攻撃を受け、業務システムに障害発生](https://www.bleepingcomputer.com/news/security/japans-keio-confirms-ransomware-attack-disrupted-business-systems/) | 28.0 | 30.0 | 42.0 |
| [JadePufferがAzure IDを乗っ取り、クラウドリソースを破壊した](https://www.theregister.com/security/2026/09/28/jadepuffer-crims-hijacked-azure-identities-and-used-them-to-blow-up-cloud-resources/5299591) | 28.0 | 30.0 | 42.0 |
| [数カ月で消えるAI予算とシャドーAIの脅威--Datadog CPOに聞く「AI本格運用」を支えるIT戦略](https://japan.zdnet.com/article/35252559/) | 28.0 | 20.0 | 42.0 |
| [AI同士をターン制のバトルゲームで対決させて能力を測る「Tiny AI Arena」](https://gigazine.net/news/20260929-tiny-ai-arena/) | 27.0 | 20.0 | 42.0 |
| [M365 のメールや Teams を直接分析 ～ プルーフポイントが AI 活用調査機能を拡張、内部リスクの可視性を強化](https://scan.netsecurity.ne.jp/article/2026/09/29/56319.html) | 26.0 | 20.0 | 42.0 |
| [AIエージェント暴走 本番データを全削除](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/091700571/091700001/) | 26.0 | 20.0 | 42.0 |
| [日立が目指すAIエージェントを駆使する次世代SIへの変革](https://japan.zdnet.com/article/35252912/) | 26.0 | 20.0 | 42.0 |
| [生成AIで変革と内製化を一体推進 紙や手作業を相次ぎ撤廃](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020600004/092400218/) | 26.0 | 20.0 | 42.0 |
| [Anthropic、「Claude Sonnet 5.5」公開 料金据え置きで30％以上高速化、タスク当たりコスト最大3割減](https://www.itmedia.co.jp/news/article/2609/29/2000001823/) | 26.0 | 20.0 | 42.0 |
| [Authlibライブラリにおける署名検証が回避される脆弱性](https://jvn.jp/vu/JVNVU99151548/) | 23.0 | 20.0 | 43.0 |
| [Apple、iOS 26・macOS 26・macOS 15向け緊急パッチを公開（CVE-2026-86950）](https://isc.sans.edu/diary/rss/33376) | 22.0 | 28.0 | 50.0 |
| [1パケットで産業分野のOTサーバーをクラッシュさせる問題](https://www.darkreading.com/ics-ot-security/one-packet-crash-servers-tdengine) | 22.0 | 20.0 | 43.0 |
| [「macOS」にアップデート - iOSで悪用の可能性ある脆弱性に対処](https://www.security-next.com/190787) | 22.0 | 20.0 | 42.0 |
| [ニッポンレンタカーでも会員41人の情報漏えいのおそれ 免許証番号やクレカ下4ケタも](https://www.itmedia.co.jp/news/article/2609/29/2000001827/) | 21.0 | 20.0 | 42.0 |
| [サイバー犯罪対策は、背後にある人物やインフラストラクチャ、サービスを破壊する新たな戦略へ](https://ascii.jp/elem/000/004/436/4436707/?rss=) | 21.0 | 20.0 | 42.0 |
| [CSIRT支援室 第39回 魚の骨が、抜けた日。DEF CON CTF世界一までの20年](https://scan.netsecurity.ne.jp/article/2026/09/29/56335.html) | 21.0 | 20.0 | 42.0 |
| [負担を抑えた ISMS 運用と脆弱性診断とは？ エーアイセキュリティラボと SecureNavi が 9 / 30 セミナー開催](https://scan.netsecurity.ne.jp/article/2026/09/29/56334.html) | 21.0 | 20.0 | 42.0 |
| [不正プログラム設置 ～ 東京大学大学院医学系研究科公共健康医学専攻ウェブサイトに不正アクセス](https://scan.netsecurity.ne.jp/article/2026/09/29/56333.html) | 21.0 | 20.0 | 42.0 |
| [モンベル・グローバルサイトに不正アクセス、最大15名分の個人情報が第三者に不正に取得された可能性](https://scan.netsecurity.ne.jp/article/2026/09/29/56332.html) | 21.0 | 20.0 | 42.0 |
| [「スマレジEC・リピート」「スマレジEC・B2B」に不正アクセス、一部の個人データが閲覧・取得された可能性](https://scan.netsecurity.ne.jp/article/2026/09/29/56331.html) | 21.0 | 20.0 | 42.0 |
| [問題発生後の報告体制に改善すべき点 ～ 選挙ドットコム運営のイチニで「個別お打合せのご提案」と題するメールを誤送信](https://scan.netsecurity.ne.jp/article/2026/09/29/56330.html) | 21.0 | 20.0 | 42.0 |
| [扶桑電通が社外関係者と利用していた共有フォルダに不正アクセス、26,489件の個人情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/09/29/56329.html) | 21.0 | 20.0 | 42.0 |
| [商船三井クルーズで営業情報を保存した外部記憶媒体を紛失、就航準備中のクルーズ船「MITSUI OCEAN SAKURA」の船内で保管](https://scan.netsecurity.ne.jp/article/2026/09/29/56328.html) | 21.0 | 20.0 | 42.0 |
| [不開示情報のマスキングが不完全で個人情報が閲覧可能に、周知の徹底が不十分](https://scan.netsecurity.ne.jp/article/2026/09/29/56327.html) | 21.0 | 20.0 | 42.0 |
| [「ワンストップジョブサイトくまもと」が改ざん被害、フェイクアラートが表示される状態に](https://scan.netsecurity.ne.jp/article/2026/09/29/56326.html) | 21.0 | 20.0 | 42.0 |
| [非公開情報であることに気付かず承認 ～ 愛知県の出会いサポートポータルサイト「あいこんナビ」で個人情報を誤掲載](https://scan.netsecurity.ne.jp/article/2026/09/29/56325.html) | 21.0 | 20.0 | 42.0 |
| [eLTAXを騙る不審メールやQRコード経由の詐欺サイト確認](https://scan.netsecurity.ne.jp/article/2026/09/29/56324.html) | 21.0 | 20.0 | 42.0 |
| [感染したスマートフォンによる不正な商品購入も確認 ～ NTTドコモ、不正なアプリのインストールに注意を呼びかけ](https://scan.netsecurity.ne.jp/article/2026/09/29/56323.html) | 21.0 | 20.0 | 42.0 |
| [baserCMS 用プラグイン「アドオンマイグレーター」 に信頼できない制御領域からの機能の組み込みに関する脆弱性](https://scan.netsecurity.ne.jp/article/2026/09/29/56322.html) | 21.0 | 20.0 | 42.0 |
| [統合セキュリティプラットフォーム「Securify」のデモ展示、スリーシェイクが情報セキュリティ EXPO に出展](https://scan.netsecurity.ne.jp/article/2026/09/29/56321.html) | 21.0 | 20.0 | 42.0 |
| [求職者やエンジニアを狙うヘッドハンティング型攻撃 ～ 警察庁が注意喚起する「WaterPlum」の手口](https://scan.netsecurity.ne.jp/article/2026/09/29/56320.html) | 21.0 | 20.0 | 42.0 |
| [ネットワークも認証サーバも要らない「多要素認証」、Windows端末でどう実現？](https://atmarkit.itmedia.co.jp/ait/articles/2609/29/news030.html) | 21.0 | 20.0 | 42.0 |
| [AIの闇落ちを防ぐ 弱点をあぶり出せ](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/091700571/091700005/) | 21.0 | 20.0 | 42.0 |
| [脆弱性の嵐が始まる 担当者が燃え尽きる](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/091700571/091700003/) | 21.0 | 20.0 | 42.0 |
| [★取得はゴールではなく入口 IPAお助け隊“新類型”で自社の穴を先に見つけよう](https://www.itmedia.co.jp/enterprise/articles/2609/29/news020.html) | 21.0 | 20.0 | 42.0 |
| [新たに観測されるドメインの約20％は「中古」--攻撃者が引き継ぐ「信頼」の中身](https://japan.zdnet.com/article/35252907/) | 21.0 | 20.0 | 42.0 |
| [どうするSCS評価制度](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/041800013/091400107/) | 21.0 | 20.0 | 42.0 |
| [タイムズカー情報漏えい 識者警鐘](https://news.yahoo.co.jp/pickup/6596915?source=rss) | 20.0 | 20.0 | 42.0 |
| [不正アクセスにより情報漏えい発生の「Gyazo」、サービスを再開 画像はすべて本人のみ閲覧可能な状態に](https://internet.watch.impress.co.jp/docs/news/2143888.html) | 20.0 | 20.0 | 42.0 |
| [富士通、ダークウェブ監視・ASM、脅威ハンティングを組み合わせた法人向けセキュリティサービスを提供](https://internet.watch.impress.co.jp/docs/news/2143675.html) | 20.0 | 20.0 | 42.0 |
| [バッファロー「WSR-300HP」「WEX-G300」に複数の深刻な脆弱性、ファームウェア更新が提供中](https://internet.watch.impress.co.jp/docs/news/2143894.html) | 20.0 | 20.0 | 42.0 |
| [Times Car、660万件のユーザーアカウントに影響するデータ侵害を確認](https://www.bleepingcomputer.com/news/security/times-car-confirms-data-breach-affecting-66-million-user-accounts/) | 20.0 | 20.0 | 42.0 |

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
