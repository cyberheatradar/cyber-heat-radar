# 📡 サイレーダー 2026-07-22 11:00 JST

このレポートは、2026-07-22 05:00 JST〜2026-07-22 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 59
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 32

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Critical SharePoint RCE flaw exploited to steal machine keys](#topic-23476) | 39.0 | 56.0 | 56.0 | 音声 | 温度感上位枠 |
| 2 | [Ransomware Is Accelerating, But It's Not Because of AI](#topic-23631) | 33.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-23476"></a>

### 1. Critical SharePoint RCE flaw exploited to steal machine keys

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 56.0 |

#### 概要

Microsoft SharePoint の脆弱性 CVE-2026-50522 が、公開後に悪用されている可能性が報じられています。
報道によれば、この問題は不正なデシリアライズに起因する重大な RCE 脆弱性で、機械鍵の窃取や、修正後も継続的なアクセスにつながるおそれがあるとされています。
SharePoint は企業内の重要な情報基盤として使われることが多く、影響範囲が広がりやすい点が注目されています。
公開 PoC の存在が示唆されているため、実運用環境では早期の対応と侵害有無の確認が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 公開PoC・検証コード言及あり。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当する SharePoint Server の更新適用状況を確認し、未適用の環境は優先的にパッチを適用する。
- 機械鍵や関連する秘密情報の保護状況を点検し、必要に応じてローテーションを検討する。
- 外部からの不審なアクセス、異常な認証、設定変更や Web シェル等の痕跡がないかログを確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-50522 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | watchTowr | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| 製品 | Microsoft Office | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-50522](https://nvd.nist.gov/vuln/detail/CVE-2026-50522) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Critical SharePoint RCE flaw exploited to steal machine keys](https://www.bleepingcomputer.com/news/security/critical-sharepoint-rce-flaw-exploited-to-steal-machine-keys/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical SharePoint RCE CVE-2026-50522 Under Active Exploitation After Public Po](https://thehackernews.com/2026/07/critical-sharepoint-rce-cve-2026-50522.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-23631"></a>

### 2. Ransomware Is Accelerating, But It's Not Because of AI

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

ランサムウェアの被害拡大が続いていますが、その背景はAIの活用というより、攻撃者側の分散化や新規参入、そして防御が手薄な組織への攻撃拡大にあるとされています。
研究者は、ランサムウェアのエコシステムが細分化し、攻撃の広がり方が変化している点を指摘しています。
AIが原因とみなすと対策の焦点を外すおそれがあるため、実際の変化要因を見極めることが重要です。特に防御が十分でない組織は、従来型の脅威管理と基本対策の見直しが必要になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ランサムウェアの増加要因をAIだけに結びつけず、攻撃者の動向や標的の変化を継続監視する。
- 防御が手薄になりやすい部門・子会社・委託先を含め、バックアップ、権限管理、復旧手順を点検する。
- インシデント対応計画を更新し、侵入検知から隔離・復旧までの実運用を定期的に確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Ransomware Is Accelerating, But It's Not Because of AI](https://www.darkreading.com/cyberattacks-data-breaches/ransomware-is-accelerating-not-ai) | <nobr>内容確認・補足情報</nobr> |

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
| [AIを悪用した攻撃、どう対抗する？ EDR導入の“次”にやるべきこと](https://www.itmedia.co.jp/enterprise/articles/2607/22/news025.html) | 29.0 | 30.0 | 42.0 |
| [FakeGitキャンペーン、7,600件のGitHubリポジトリを悪用してSmartLoaderマルウェアを拡散](https://www.bleepingcomputer.com/news/security/fakegit-campaign-uses-7-600-github-repos-to-push-smartloader-malware/) | 28.0 | 20.0 | 42.0 |
| [AnthropicがAIモデル「Claude」のトレーニングに海賊版書籍を使った件で作家グループと和解するも一部の著者は和解を拒否](https://gigazine.net/news/20260722-anthropics-settlement-book-piracy-ai/) | 27.0 | 20.0 | 42.0 |
| [ジャック・ドーシー氏率いるBlock、AI協働プラットフォーム「Buzz」公開 SlackやGitHub依存からの脱却目指し](https://www.itmedia.co.jp/news/articles/2607/22/news058.html) | 26.0 | 20.0 | 42.0 |
| [最低賃金実現に並ぶ歴史的改革か ～ オーストラリア首相が AI 企業に消費する以上の発電とコンテンツ盗用停止を突きつける](https://scan.netsecurity.ne.jp/article/2026/07/22/55753.html) | 26.0 | 20.0 | 42.0 |
| [Hugging Face侵害のAIエージェントはOpenAIのモデル──社内のサイバー能力評価中に「GPT-5.6 Sol」などが暴走し本番DBに侵入](https://www.itmedia.co.jp/news/articles/2607/22/news056.html) | 26.0 | 20.0 | 42.0 |
| [AI戦略にも違い 基盤構築とデータ分散](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/071300561/071300003/) | 26.0 | 20.0 | 42.0 |
| [「Claude」が認証情報にアクセスせずにログイン可能に--1Passwordの新たな「エージェンティック・モード」](https://japan.zdnet.com/article/35250732/) | 26.0 | 20.0 | 42.0 |
| [OpenAI、モデルテストがHugging Faceのハックの背景にあったと発表](https://cyberscoop.com/openai-chatgpt-hugging-face-cyberattack-data-poisoning/) | 25.0 | 20.0 | 42.0 |
| [Ciscoのオープンウェイト型バグバスターがGoogleとOpenAIに挑む](https://www.theregister.com/security/2026/07/21/ciscos-open-weight-bug-busters-take-on-google-and-openai/5275817) | 25.0 | 20.0 | 42.0 |
| [「WordPress」「Langflow」の脆弱性悪用に警戒を - 米当局が注意喚起](https://www.security-next.com/187654) | 22.0 | 20.0 | 42.0 |
| [大手会計事務所のアーンスト・アンド・ヤング、顧客の税務情報流出を公表](https://japan.zdnet.com/article/35250839/) | 21.0 | 20.0 | 42.0 |
| [お客を「成功」させるのが自分の仕事 ～ 日本プルーフポイント 代表取締役社長 野村健インタビュー](https://scan.netsecurity.ne.jp/article/2026/07/22/55752.html) | 21.0 | 20.0 | 42.0 |
| [TwoFive、事例から学ぶ Microsoft 365 の設定管理・脅威検知ウェビナーを7月30日に開催](https://scan.netsecurity.ne.jp/article/2026/07/22/55751.html) | 21.0 | 20.0 | 42.0 |
| [佐川急便「スマートクラブ」でシステム不具合、配達予定通知メールの一部で本来と異なる顧客情報を表示](https://scan.netsecurity.ne.jp/article/2026/07/22/55750.html) | 21.0 | 20.0 | 42.0 |
| [中学校教員がSDカード紛失、飲食後 深夜屋外で約50分間眠り込む](https://scan.netsecurity.ne.jp/article/2026/07/22/55749.html) | 21.0 | 20.0 | 42.0 |
| [石川コンピュータ・センターが不正アクセスの最終報を発表、他サービスへの影響はなく漏えい件数も変更なし](https://scan.netsecurity.ne.jp/article/2026/07/22/55748.html) | 21.0 | 20.0 | 42.0 |
| [銚子市で入札不正行為、2名が起訴され免職に](https://scan.netsecurity.ne.jp/article/2026/07/22/55747.html) | 21.0 | 20.0 | 42.0 |
| [ピックルボールワン ウェブサイトにプラグインの脆弱性を悪用した不正アクセス](https://scan.netsecurity.ne.jp/article/2026/07/22/55746.html) | 21.0 | 20.0 | 42.0 |
| [HENNGE One、次世代コラボレーションツール「Lark」と SSO 連携](https://scan.netsecurity.ne.jp/article/2026/07/22/55745.html) | 21.0 | 20.0 | 42.0 |
| [「GMOサイバー攻撃ネットde診断 ASM」にサイバーリスク保険とインシデント初動対応（最大3日分）を標準付帯](https://scan.netsecurity.ne.jp/article/2026/07/22/55744.html) | 21.0 | 20.0 | 42.0 |
| [SGLang に Pickle のデシリアライゼーションに関する脆弱性](https://scan.netsecurity.ne.jp/article/2026/07/22/55743.html) | 21.0 | 20.0 | 42.0 |
| [一部の HTTP/2 サーバにフロー制御に起因したサービス拒否（DoS）の脆弱性](https://scan.netsecurity.ne.jp/article/2026/07/22/55742.html) | 21.0 | 20.0 | 42.0 |
| [Windows DNS に複数の脆弱性](https://scan.netsecurity.ne.jp/article/2026/07/22/55741.html) | 21.0 | 20.0 | 42.0 |
| [わずか11バイトでメモリを圧迫 OpenSSLを狙う新DoS攻撃、その意外な仕組み](https://atmarkit.itmedia.co.jp/ait/articles/2607/22/news042.html) | 21.0 | 20.0 | 42.0 |
| [「AIは破壊的な技術」「防御は基本に立ち返る時」--チェック・ポイントのCEO](https://japan.zdnet.com/article/35250683/) | 21.0 | 20.0 | 42.0 |
| [WordPress本体に重大脆弱性、運営元が異例の強制更新 専門家が語る“本当の危険”](https://atmarkit.itmedia.co.jp/ait/articles/2607/22/news037.html) | 21.0 | 20.0 | 42.0 |
| [CISA ICS Advisory / ICS Medical Advisory（2026年07月21日）](https://jvn.jp/vu/JVNVU98832565/) | 20.0 | 20.0 | 42.0 |
| [Kratosフィッシング・プラットフォームを摘発、開発者を逮捕](https://www.bleepingcomputer.com/news/security/police-dismantle-kratos-phishing-platform-arrest-developer/) | 20.0 | 20.0 | 42.0 |
| [モデルは私たちが求めたとおりに実行した](https://cloudsecurityalliance.org/articles/the-model-did-exactly-what-we-asked) | 20.0 | 20.0 | 42.0 |
| [DTSとグランセキュノロジー、法人向けセキュリティサービス高度化のためASRM「Mitokude」を軸に協業 7月23日開催の「保険EXPO 2026」に出展](https://internet.watch.impress.co.jp/docs/news/2126700.html) | 20.0 | 20.0 | 42.0 |
| [LLMを使った脆弱性の発見と優先順位付けは容易ではない](https://www.darkreading.com/application-security/finding-and-prioritizing-vulnerabilities-no-easy-task) | 20.0 | 20.0 | 42.0 |

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
