# 📡 サイレーダー 2026-07-29 11:00 JST

このレポートは、2026-07-29 05:00 JST〜2026-07-29 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 60
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 34

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [「いつものChrome」が攻撃の踏み台に？ マルウェア「msaRAT」の脅威と、情シスが今すぐやるべきこと](#topic-24835) | 37.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-24835"></a>

### 1. 「いつものChrome」が攻撃の踏み台に？ マルウェア「msaRAT」の脅威と、情シスが今すぐやるべきこと

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Cisco Talosが、ランサムウェアグループ「Chaos」に関連するとされる新型RAT「msaRAT」を確認したと伝えています。
特徴として、マルウェア自身は直接インターネットに接続せず、ChromeやEdgeなどのブラウザを通信の“中継役”として悪用する点が挙げられます。
普段使うブラウザが不正通信の経路に使われると、通常の通信監視では気づきにくくなるおそれがあります。
ランサムウェア文脈の脅威として、端末防御だけでなくブラウザ周辺の挙動確認が重要になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ブラウザの不審な常駐・拡張機能・プロセス挙動を確認し、通常と異なる通信を監視する。
- 端末EDRやネットワーク監視で、ブラウザ経由の不自然な外部通信や子プロセス生成を点検する。
- 最新の脅威情報を踏まえ、Chrome/Edgeの更新状況と関連するセキュリティ設定を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [「いつものChrome」が攻撃の踏み台に？　マルウェア「msaRAT」の脅威と、情シスが今すぐやるべきこと](https://atmarkit.itmedia.co.jp/ait/articles/2607/29/news029.html) | <nobr>内容確認・補足情報</nobr> |

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
| [八王子学園にランサムウェア攻撃](https://scan.netsecurity.ne.jp/article/2026/07/29/55806.html) | 29.0 | 30.0 | 42.0 |
| [WordPressプラグイン・テーマの脆弱性最新情報 第33回 WordPress脆弱性13件、コアに認証不要RCE 「wp2shell」で早急な更新を【7月16日～7月22日】](https://news.mynavi.jp/techplus/article/wordpressvulnerability-33/) | 27.0 | 38.0 | 42.0 |
| [JFrogのゼロデイ脆弱性によりOpenAIのモデルがHugging Faceを攻撃可能に？](https://www.theregister.com/security/2026/07/28/looks-like-jfrogs-0-days-let-openais-models-hack-hugging-face/5280001) | 27.0 | 20.0 | 43.0 |
| [OpenAIモデルがArtifactoryのゼロデイを悪用してインターネットへ脱出した事例](https://www.bleepingcomputer.com/news/security/openai-models-used-artifactory-zero-days-to-escape-to-the-internet/) | 27.0 | 20.0 | 43.0 |
| [オープンソースソフトウェアのためのホスティングサービス「Codeberg」が生成AI主体のプロジェクトを投票で禁止](https://gigazine.net/news/20260729-codeberg-bans-ai-contributions/) | 27.0 | 20.0 | 42.0 |
| [「iOS 26」の「Siri」と「iOS 27」の「Siri AI」を車内で比較してみた--圧勝したのは？](https://japan.zdnet.com/article/35250895/) | 26.0 | 20.0 | 42.0 |
| [AIエージェントがサンドボックスを脱出するとき、従来のセキュリティルールが再び重要になる](https://www.darkreading.com/application-security/ai-agents-escape-sandboxes-old-security-rules-apply) | 25.0 | 20.0 | 42.0 |
| [AIの安全性向上には「ブラックボックス」の内部を覗く必要がある](https://www.darkreading.com/cybersecurity-analytics/stronger-ai-safety-requires-peeking-inside-black-box) | 25.0 | 20.0 | 42.0 |
| [Microsoft Windows OS における管理者権限の奪取につながる ATBroker.exe の特権動作での検証不備（Scan Tech Report）](https://scan.netsecurity.ne.jp/article/2026/07/29/55810.html) | 24.0 | 20.0 | 43.0 |
| [Anthropicのミュトス、暗号アルゴリズムの新たな攻撃法を発見――耐量子署名「HAWK」の強度を半減](https://www.itmedia.co.jp/news/article/2607/29/2000000256/) | 24.0 | 20.0 | 43.0 |
| [NVIDIA「VIRTIO-Net」に脆弱性 - VM利用者によるコード実行のおそれ](https://www.security-next.com/187984) | 22.0 | 20.0 | 42.0 |
| [「Adobe Bridge」「Adobe Format Plugins」に脆弱性 - 修正版を公開](https://www.security-next.com/187979) | 22.0 | 20.0 | 42.0 |
| [分散型npmパッケージクラスターがAlibaba開発者を標的とするクロスプラットフォームRATを配布](https://socket.dev/blog/npm-rat-targets-alibaba) | 22.0 | 20.0 | 42.0 |
| [アップル、「iOS 26.6」をリリース--セキュリティ修正と「iOS 27」への準備](https://japan.zdnet.com/article/35251052/) | 21.0 | 20.0 | 42.0 |
| [ポスト量子暗号セキュリティへどう移行すればいいのか](https://ascii.jp/elem/000/004/422/4422285/?rss=) | 21.0 | 20.0 | 42.0 |
| [“120TB消失危機”を救ったBox。ゼネラルが挑むグローバルデータ統合の舞台裏](https://ascii.jp/elem/000/004/420/4420062/?rss=) | 21.0 | 20.0 | 42.0 |
| [象印マホービンの台湾連結子会社に不正アクセス、連結業績に与える影響は軽微](https://scan.netsecurity.ne.jp/article/2026/07/29/55809.html) | 21.0 | 20.0 | 42.0 |
| [メディア4u の SMS 送信システムへのサイバー攻撃、エンバーポイントの「SMSPubisher」にも影響](https://scan.netsecurity.ne.jp/article/2026/07/29/55808.html) | 21.0 | 20.0 | 42.0 |
| [9 月末でサービス終了 ～ 不正アクセス受けたデジタルギフトサービス](https://scan.netsecurity.ne.jp/article/2026/07/29/55807.html) | 21.0 | 20.0 | 42.0 |
| [「個人情報の保護に関する法律等の一部を改正する法律」公布](https://scan.netsecurity.ne.jp/article/2026/07/29/55805.html) | 21.0 | 20.0 | 42.0 |
| [家庭用 IoT 機器を悪用したサイバー攻撃、官民一体で対策推進](https://scan.netsecurity.ne.jp/article/2026/07/29/55804.html) | 21.0 | 20.0 | 42.0 |
| [PowerDNS Recursor に複数の脆弱性](https://scan.netsecurity.ne.jp/article/2026/07/29/55803.html) | 21.0 | 20.0 | 42.0 |
| [GMOサイバーセキュリティ byイエラエ、篠田佳奈氏を社外取締役に選任](https://scan.netsecurity.ne.jp/article/2026/07/29/55802.html) | 21.0 | 20.0 | 42.0 |
| [IoT 製品メーカー向けに「JC-STAR★1評価内製化支援コース」を新設、9 / 18 セミナー開催](https://scan.netsecurity.ne.jp/article/2026/07/29/55801.html) | 21.0 | 20.0 | 42.0 |
| [MFAなのに突破された？ 「Microsoft正規画面で認証したのに侵害された」理由](https://atmarkit.itmedia.co.jp/ait/articles/2607/29/news032.html) | 21.0 | 20.0 | 42.0 |
| [フィッシング92％減の裏でTeamsの通話攻撃が10倍に Microsoft分析](https://www.itmedia.co.jp/enterprise/articles/2607/27/news093.html) | 21.0 | 20.0 | 42.0 |
| [Weekly Report: 複数のElastic製品に脆弱性](https://www.jpcert.or.jp/wr/2026/wr260729.html) | 20.0 | 20.0 | 42.0 |
| [CISA ICS Advisory / ICS Medical Advisory（2026年07月28日）](https://jvn.jp/vu/JVNVU90008749/) | 20.0 | 20.0 | 42.0 |
| [みずほ銀行らが推進する「サプライチェーン途絶リスクマネジメント支援」に、トムソン・ロイターと日立製作所が新たに参画](https://internet.watch.impress.co.jp/docs/news/2128642.html) | 20.0 | 20.0 | 42.0 |
| [Ghost Credentialsがクラウドシステムを隠れたIDリスクにさらす](https://www.darkreading.com/cloud-security/non-human-identity-sprawl-creates-a-new-cloud-attack-path) | 20.0 | 20.0 | 42.0 |
| [ミネソタ州の水道システムに対する連携型サイバー攻撃の捜査](https://www.cybersecuritydive.com/news/authorities-investigating-a-coordinated-cyberattack-against-minnesota-water/826427/) | 20.0 | 20.0 | 42.0 |
| [CubePilotのドローンソフトウェア開発企業がDNSハイジャックで通信を傍受される](https://www.bleepingcomputer.com/news/security/cubepilot-drone-software-dev-hit-by-dns-hijacking-to-intercept-traffic/) | 20.0 | 20.0 | 42.0 |
| [数千のデータセンターコントローラーが乗っ取り可能な状態にある](https://www.darkreading.com/cyber-risk/flaw-exposes-data-centers-server-takeover) | 20.0 | 20.0 | 42.0 |
| [AnthropicがMythosを用いて暗号化アルゴリズムを検証した結果](https://cyberscoop.com/anthropic-claude-mythos-encryption-flaws-hawk-aes-pqc/) | 20.0 | 20.0 | 42.0 |

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
