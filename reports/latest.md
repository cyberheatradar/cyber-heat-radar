# 📡 サイレーダー 2026-07-17 11:00 JST

このレポートは、2026-07-17 05:00 JST〜2026-07-17 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 63
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 36

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [米CISA、「FortiSandbox」「SharePoint」の脆弱性悪用を警告](#topic-22941) | 33.0 | 20.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [ACR Stealer: Two observed intrusion chains amid increased threat activity](#topic-22943) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-22941"></a>

### 1. 米CISA、「FortiSandbox」「SharePoint」の脆弱性悪用を警告

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

米CISAは、Fortinetのマルウェア解析製品「FortiSandbox」とMicrosoftの「SharePoint」に関連する脆弱性について、悪用が確認されているとして注意を呼びかけました。
対象製品を利用している組織では、影響範囲の確認や対策状況の見直しが必要です。
脆弱性が実際に悪用されているとされるため、単なる未修正リスクではなく、早期対応の優先度が高い話題です。
広く使われる製品に関わるため、個別組織だけでなく多くの運用環境に影響し得ます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- FortiSandboxとSharePointの該当バージョンや構成を確認し、ベンダーの修正情報と照合する。
- 公開状況を点検し、不要な外部露出やアクセス権の過剰付与がないか見直す。
- 関連ログや監視アラートを確認し、異常なアクセスや改ざんの兆候がないか継続監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Fortinet | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [米CISA、「FortiSandbox」「SharePoint」の脆弱性悪用を警告](https://www.security-next.com/187509) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-22943"></a>

### 2. ACR Stealer: Two observed intrusion chains amid increased threat activity

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftの観測によると、2026年4月下旬から6月中旬にかけて、ACR Stealerの活動が顧客環境で増加していました。
報告では、ClickFixを用いた誘導を通じて、ブラウザーの認証情報やトークン、機密文書が狙われたとされています。
認証情報やセッショントークンが盗まれると、単一端末の感染にとどまらず、クラウドや社内サービスへの不正アクセスにつながるおそれがあります。
企業環境を対象にした事例であり、フィッシングやソーシャルエンジニアリング対策の重要性が改めて示されています。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ブラウザー保存情報やセッショントークンの保護・無効化手順を確認し、多要素認証の有効性を点検する。
- ClickFixのようなユーザー操作を促す誘導に対し、社内で注意喚起を行い、不審な操作要求を報告できる体制を整える。
- EDRやSIEMで、認証情報の不自然な利用や機密文書への異常なアクセスを早期検知できるよう監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |
| 製品 | Google Chrome | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| 製品 | Chromium | 言及あり | 0.80 | — |
| マルウェア | Latrodectus | 主題 | 0.80 | — |
| マルウェア | ZLib | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ACR Stealer: Two observed intrusion chains amid increased threat activity](https://www.microsoft.com/en-us/security/blog/2026/07/16/acr-stealer-two-observed-intrusion-chains-amid-increased-threat-activity/) | <nobr>内容確認・補足情報</nobr> |

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
| [オーミケンシへのランサムウェア攻撃、外部のクラウドストレージサービスへのデータ送信を確認](https://scan.netsecurity.ne.jp/article/2026/07/17/55728.html) | 29.0 | 30.0 | 42.0 |
| [Coca-Cola傘下のFairlifeでランサムウェア攻撃、米国の乳製品生産が停止](https://www.bleepingcomputer.com/news/security/coca-cola-says-fairlife-ransomware-attack-halts-us-dairy-production/) | 28.0 | 30.0 | 42.0 |
| [Anubis ransomware：知っておくべきこと](https://www.fortra.com/blog/anubis-ransomware) | 28.0 | 30.0 | 42.0 |
| [新たなClickLock macOSマルウェア、ユーザーをだましてログインパスワードを入力させる](https://www.bleepingcomputer.com/news/security/new-clicklock-macos-malware-traps-users-into-revealing-login-password/) | 28.0 | 20.0 | 42.0 |
| [Anthropic、AIを活用する若手人材とNPOを結ぶ支援プログラム開始](https://japan.zdnet.com/article/35250710/) | 26.0 | 20.0 | 42.0 |
| [OpenAIの新音声モデル「GPT-Live」を試してみた--スムーズな会話はほとんど人間のよう](https://japan.zdnet.com/article/35250442/) | 26.0 | 20.0 | 42.0 |
| [生成AIバブルの崩壊は「必然」 それでも気にする必要がない訳](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020600007/070700221/) | 26.0 | 20.0 | 42.0 |
| [コーディングエージェントは不要 現場がAI活用でアプリ開発者に](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/052100111/071300181/) | 26.0 | 20.0 | 42.0 |
| [AI BOM（AI Bill of Materials）](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020600009/070700227/) | 26.0 | 20.0 | 42.0 |
| [AI、自動化、そして攻撃：Unit 42の2026年グローバルインシデントレスポンスレポートを読み解く](https://unit42.paloaltonetworks.com/ai-incident-response-report/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、GPT-5.6がまれにファイルを削除する不具合を認める――「正直なミス」と説明](https://www.theregister.com/ai-and-ml/2026/07/16/openai-admits-gpt-56-occasionally-deletes-files-but-its-an-honest-mistake/5274008) | 25.0 | 20.0 | 42.0 |
| [Agentic AIは制御困難：適切なセキュリティ質問を投げかけよ](https://www.darkreading.com/cybersecurity-operations/agentic-ai-untamable-ask-the-right-security-questions) | 25.0 | 20.0 | 42.0 |
| [100ドル未満でオープンウェイトAIモデルを汚染する研究者](https://www.theregister.com/ai-and-ml/2026/07/16/researcher-poisons-open-weight-ai-model-for-under-100/5273880) | 25.0 | 20.0 | 42.0 |
| [Microsoft Defenderに脆弱性、Windows PCのディスク容量を枯渇させる攻撃手法を発見](https://news.mynavi.jp/techplus/article/20260717-4705047/) | 21.0 | 20.0 | 42.0 |
| [AIで巧妙化するフィッシング攻撃 企業に求められる「行動優先」のトレーニングとは](https://ascii.jp/elem/000/004/419/4419596/?rss=) | 21.0 | 20.0 | 42.0 |
| [攻撃するAIと防御するAI 日本企業のセキュリティ対策にいま何が必要か？](https://ascii.jp/elem/000/004/419/4419594/?rss=) | 21.0 | 20.0 | 42.0 |
| [欧州委員会、GoogleにAIアシスタントの相互運用と検索データ共有を命令──Googleは「安全性を損なう」と反発](https://www.itmedia.co.jp/news/articles/2607/17/news063.html) | 21.0 | 20.0 | 42.0 |
| [Microsoftでも発生した「機械のID」を狙う攻撃とは？ NHIのリスクをNECが解説](https://news.mynavi.jp/techplus/article/20260717-4708863/) | 21.0 | 20.0 | 42.0 |
| [2日間全科目休講 ～ 札幌国際大学のアカウントがフィッシングメール被害](https://scan.netsecurity.ne.jp/article/2026/07/17/55730.html) | 21.0 | 20.0 | 42.0 |
| [フラウ・インターナショナル業務委託先に不正アクセス、過去に問い合わせた顧客の個人情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/07/17/55729.html) | 21.0 | 20.0 | 42.0 |
| [エクセルファイルに個人情報が記載されたシートがあることに気づかず公開](https://scan.netsecurity.ne.jp/article/2026/07/17/55727.html) | 21.0 | 20.0 | 42.0 |
| [「QRでアクセスするので該当者しか閲覧できない」と思い込み ～ マラソンのボランティアの個人情報閲覧可能に](https://scan.netsecurity.ne.jp/article/2026/07/17/55726.html) | 21.0 | 20.0 | 42.0 |
| [2026年サイバー新法とSCS制度に対し企業法務が今すべき実務対応について解説](https://scan.netsecurity.ne.jp/article/2026/07/17/55725.html) | 21.0 | 20.0 | 42.0 |
| [マイクロソフトが 7 月のセキュリティ情報公開、悪用の事実を確認済みの脆弱性が 2 件](https://scan.netsecurity.ne.jp/article/2026/07/17/55724.html) | 21.0 | 20.0 | 42.0 |
| [HYPER SBI 2 のインストーラに DLL 読み込みに関する脆弱性](https://scan.netsecurity.ne.jp/article/2026/07/17/55723.html) | 21.0 | 20.0 | 42.0 |
| [スリーシェイクのエンジニア 4 名が翻訳を担当『セキュアAPI【リフロー型】 設計・構築・実装を貫く原則』7 / 15発売](https://scan.netsecurity.ne.jp/article/2026/07/17/55722.html) | 21.0 | 20.0 | 42.0 |
| [サイバー攻撃による事業停止を最小限に ～ 演習を交えて実効性を高める中小企業向け BCP 策定支援](https://scan.netsecurity.ne.jp/article/2026/07/17/55721.html) | 21.0 | 20.0 | 42.0 |
| [鉄道係員に対する暴力行為、飲酒有りが45.9％を占め 加害者年齢は60代以上が最多](https://scan.netsecurity.ne.jp/article/2026/07/17/55720.html) | 21.0 | 20.0 | 42.0 |
| [QRコードフィッシングが増加傾向に--身を守るために知っておくべきこと](https://japan.zdnet.com/article/35250661/) | 21.0 | 20.0 | 42.0 |
| [Entra IDの標準認証がパスキーに SMS認証が使えなくなるのはいつ？](https://www.itmedia.co.jp/enterprise/articles/2607/17/news019.html) | 21.0 | 20.0 | 42.0 |
| [「AI駆動型ワーム」の脅威 自律的に脆弱性を見つけて感染](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/052100113/070700190/) | 21.0 | 20.0 | 42.0 |
| [GMOの在宅勤務廃止は間違っていない？ ワサビのインシデントから考える企業防衛](https://atmarkit.itmedia.co.jp/ait/articles/2607/17/news039.html) | 21.0 | 20.0 | 42.0 |
| [トヨタの数年をかけたゼロトラスト改革、行く手を阻んだ最大の壁とは？](https://atmarkit.itmedia.co.jp/ait/articles/2607/17/news021.html) | 21.0 | 20.0 | 42.0 |
| [Microsoft、7月の月例更新で約570件を修正 悪用済みゼロデイ2件にまず対応を](https://www.itmedia.co.jp/enterprise/articles/2607/17/news042.html) | 21.0 | 20.0 | 42.0 |
| [ニチレイのサイバー攻撃被害、外食チェーンを直撃 KFC全店にも影響広がる](https://atmarkit.itmedia.co.jp/ait/articles/2607/17/news050.html) | 21.0 | 20.0 | 42.0 |
| [物理的にUSB Type-Cポートを塞ぎ、情報漏えいを防ぐポートロック製品、サンワサプライが発売](https://internet.watch.impress.co.jp/docs/news/2125822.html) | 20.0 | 20.0 | 42.0 |

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
