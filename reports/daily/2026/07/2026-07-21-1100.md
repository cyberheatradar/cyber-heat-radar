# 📡 サイレーダー 2026-07-21 11:00 JST

このレポートは、2026-07-21 05:00 JST〜2026-07-21 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 60
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 30

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [SonicWall SMA1000 flaws exploited as zero-days to push custom malware](#topic-23373) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [JadePuffer agentic attacks now target AI model data with ransomware](#topic-23404) | 41.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | ['WP2Shell' Opens Millions of WordPress Sites to Remote Takeover](#topic-23189) | 37.0 | 64.0 | 59.0 | 音声 | 温度感上位枠 |
| 4 | [Unpacking “Cruciferra”: An Analysis of a Sophisticated Crypter Service](#topic-23407) | 32.0 | 32.0 | 48.0 | 音声 | 温度感上位枠 |
| 5 | [樋口商会子会社の会計情報漏えい、取引先から「ランサムウェア感染に起因するとみられる情報漏えいの可能性がある」旨の連絡](#topic-23356) | 31.0 | 38.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-23373"></a>

### 1. SonicWall SMA1000 flaws exploited as zero-days to push custom malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

SonicWallのSMA1000製品に関する2件の脆弱性が、公開前からゼロデイ攻撃に悪用されていたと報じられています。
攻撃者は脆弱なVPN機器にカスタムマルウェアを導入していた可能性があり、対象環境では早急な確認が必要です。
VPN装置は社内ネットワークへの入口になりやすく、侵害されると認証情報や内部通信に影響が及ぶおそれがあります。
公開済みの脆弱性が実際に悪用されていた点から、パッチ適用だけでなく侵害有無の点検も重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SonicWall SMA1000を利用している場合は、該当脆弱性に対するベンダー案内と修正状況を確認する。
- VPN機器のログや設定変更、未知のファイル・プロセスなど、侵害痕跡の有無を点検する。
- 外部公開しているリモートアクセス機器は、優先度を上げて更新・隔離・監視を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-15409 | 関連CVE | 1.00 | 候補あり（URL 4件以上） |
| 脆弱性 | CVE-2026-15410 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | SonicWall | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [SonicWall SMA1000 flaws exploited as zero-days to push custom malware](https://www.bleepingcomputer.com/news/security/sonicwall-sma1000-flaws-exploited-as-zero-days-to-push-custom-malware/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23404"></a>

### 2. JadePuffer agentic attacks now target AI model data with ransomware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

JadePufferと呼ばれる自律型AIエージェントに関する脅威情報として、AI資産を狙うランサムウェアの動きが報告されています。
報告では、学習データセット、ベクトルデータベース、モデルのチェックポイントなど、AI運用に関わるデータが対象になり得るとされています。
AIシステムの被害は、業務停止だけでなくモデル再構築や学習資産の再整備にも影響しやすく、復旧コストが大きくなりがちです。
従来のファイル暗号化対策に加え、AI特有の重要資産を保護する視点が必要になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 学習データ、ベクトルDB、モデル成果物などのバックアップと復旧手順を、通常の業務データとは別に点検する。
- AI基盤へのアクセス権限を見直し、重要資産の保管場所と変更履歴を把握しておく。
- 異常な暗号化や大量変更を早期検知できる監視を、AI関連ストレージや推論基盤にも適用する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [JadePuffer agentic attacks now target AI model data with ransomware](https://www.bleepingcomputer.com/news/security/jadepuffer-agentic-attacks-now-target-ai-model-data-with-ransomware/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23189"></a>

### 3. 'WP2Shell' Opens Millions of WordPress Sites to Remote Takeover

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

WordPressの新たな脆弱性群をめぐり、CVE-2026-60137とCVE-2026-63030が公開後まもなく実環境で悪用されていると複数の報道で伝えられています。
関連するWordPress 7.0.2のセキュリティ更新では、深刻度の高い問題が修正対象とされています。
WordPressは利用規模が大きく、影響を受けるサイト数が多くなりやすいため、公開直後の悪用報告は注意が必要です。
特に認証回避やRCEにつながる可能性があるとされるため、対応の遅れが被害拡大につながり得ます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
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

- WordPressの対象バージョンを確認し、該当する場合は速やかに修正版へ更新する。
- WAFや監視でWordPress関連の異常なリクエストや管理操作の兆候を重点確認する。
- 公開済みの脆弱性情報を踏まえ、関連プラグインや運用経路も含めて影響範囲を再点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-60137 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-63030 | 関連CVE | 1.00 | 候補あり（URL 21件以上） |
| 製品 | WordPress | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-60137](https://nvd.nist.gov/vuln/detail/CVE-2026-60137) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | ['WP2Shell' Opens Millions of WordPress Sites to Remote Takeover](https://www.darkreading.com/cyberattacks-data-breaches/wp2shell-millions-wordpress-sites-remote-takeover) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [WP2Shell WordPress Vulnerabilities Exploited in the Wild](https://www.securityweek.com/wp2shell-wordpress-vulnerabilities-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Two new high severity WordPress vulnerabilities, patch immediately!](https://www.helpnetsecurity.com/2026/07/18/wordpress-vulnerabilities-wp2shell-cve-2026-60137-cve-2026-60137/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23407"></a>

### 4. Unpacking “Cruciferra”: An Analysis of a Sophisticated Crypter Service

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>国⁠家⁠支⁠援</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 32.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 32.0 |
| <nobr>確⁠度</nobr> | 48.0 |

#### 概要

Proofpointは、複数の異なるサイバー犯罪グループで利用されている難読化サービス「Cruciferra」を分析し、さまざまなRATやインフォスティーラーの配布に使われていると報告しました。
Cruciferraは防御回避や解析妨害の仕組みを多数備え、サンプルの差分も大きいため、検知や追跡が難しくなる点が特徴です。
攻撃基盤として共通利用されるため、特定のマルウェア1種ではなく、複数のキャンペーンにまたがって被害拡大につながる可能性があります。
メール経由の配布が多く、標的組織の業種も幅広いため、メール防御と端末防御の両面で警戒が必要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 権限昇格系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 不審なZIP、VHD、LNK、DLLサイドローディングを伴う添付・リンクの受信状況を確認し、メール経由の初期侵入対策を強化する。
- EDRやAVの無効化・回避を狙う挙動、権限昇格や永続化の兆候、通知設定やレジストリ変更の監視を見直す。
- 既知のRAT/インフォスティーラー配布キャンペーンと関連するIOCや不審ドメイン、未知の実行ファイルの振る舞いを継続的に照合する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Proofpoint | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |
| マルウェア | Snake Keylogger | 主題 | 0.80 | — |
| マルウェア | Agent Tesla | 主題 | 0.80 | — |
| マルウェア | AsyncRAT | 主題 | 0.80 | — |
| マルウェア | FormBook | 主題 | 0.80 | — |
| マルウェア | Remcos | 主題 | 0.80 | — |
| マルウェア | DCRat | 主題 | 0.80 | — |
| マルウェア | XWorm | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Unpacking “Cruciferra”: An Analysis of a Sophisticated Crypter Service](https://www.proofpoint.com/us/blog/threat-insight/unpacking-cruciferra-analysis-sophisticated-crypter-service) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-23356"></a>

### 5. 樋口商会子会社の会計情報漏えい、取引先から「ランサムウェア感染に起因するとみられる情報漏えいの可能性がある」旨の連絡

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 31.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

樋口商会の子会社に関して、会計情報の漏えいがあった可能性があると、取引先から「ランサムウェア感染に起因するとみられる情報漏えいの可能性がある」旨の連絡があったとされています。
現時点では、漏えいの範囲や原因の詳細は公表情報だけでは断定できません。
会計情報は取引先管理や内部統制に直結するため、漏えいの有無や範囲によっては関係先への影響が大きくなり得ます。
ランサムウェア文脈での情報漏えいの可能性は、復旧対応だけでなく、情報管理や対外説明の見直しも求められる点で注目されます。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- 情報漏えい系。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 漏えいの対象情報、件数、関係先の範囲を早期に確認し、事実関係を整理する。
- 取引先からの通知や問い合わせに備え、連絡窓口と説明文の整合性を確認する。
- 同種事案を踏まえ、バックアップ、アクセス管理、ログ確認などの初動対応を点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [樋口商会子会社の会計情報漏えい、取引先から「ランサムウェア感染に起因するとみられる情報漏えいの可能性がある」旨の連絡](https://scan.netsecurity.ne.jp/article/2026/07/21/55739.html) | <nobr>内容確認・補足情報</nobr> |

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
| [AIがHugging Faceにサイバー攻撃--攻撃を検知して分析したのもAI](https://japan.zdnet.com/article/35250781/) | 26.0 | 20.0 | 42.0 |
| [Okta Japan、企業における AI ツールの利用実態調査「Okta Enterprise AI Index」発表](https://scan.netsecurity.ne.jp/article/2026/07/21/55736.html) | 26.0 | 20.0 | 42.0 |
| [「Claude Cowork」にコーディング以外の7つのタスクを任せてみた--その結果、「欠かせない存在」に](https://japan.zdnet.com/article/35250608/) | 26.0 | 20.0 | 42.0 |
| [Cursor、Codex、Gemini CLI、Antigravityでサンドボックスエスケープの問題が発生](https://www.bleepingcomputer.com/news/security/cursor-codex-gemini-cli-antigravity-hit-by-sandbox-escapes/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントだけ追う企業は危ない？ガートナー流「次に投資すべき技術」の見極め方](https://www.sbbit.jp/article/cont1/186051?ref=rss) | 25.0 | 20.0 | 42.0 |
| [Microsoft、Windowsの脆弱性発見にAIを本格導入 ゼロデイ攻撃を防ぐ新体制へ](https://news.mynavi.jp/techplus/article/20260721-4695088/) | 24.0 | 20.0 | 43.0 |
| [JavaScript ライブラリ「Forge」に複数の署名検証不備の脆弱性](https://scan.netsecurity.ne.jp/article/2026/07/21/55733.html) | 24.0 | 20.0 | 43.0 |
| [Node.<wbr>js向け解凍ライブラリにDoS脆弱性 - ディスク枯渇のおそれ](https://www.security-next.com/187585) | 22.0 | 20.0 | 42.0 |
| [先週注目された記事（2026年7月12日〜2026年7月18日）](https://www.security-next.com/187578) | 22.0 | 20.0 | 42.0 |
| [Chromeにアップデート - 「クリティカル」など脆弱性7件を解消](https://www.security-next.com/187576) | 22.0 | 20.0 | 42.0 |
| [音楽ストリーミングサービスが普及した時代に「音楽海賊版の失われた喜び」をアーティストが語る](https://gigazine.net/news/20260721-music-piracy/) | 22.0 | 20.0 | 42.0 |
| [攻撃者がWordPressの重大な脆弱性を悪用し、さまざまな不正行為を実行](https://www.theregister.com/security/2026/07/20/attackers-pummel-critical-wordpress-vuln-to-create-all-sorts-of-mischief/5275265) | 22.0 | 20.0 | 42.0 |
| [WordPressプラグイン・テーマの脆弱性最新情報 第32回 WordPress脆弱性18件、LatePointの決済悪用に注意【7月2日～7月8日】](https://news.mynavi.jp/techplus/article/wordpressvulnerability-32/) | 21.0 | 20.0 | 42.0 |
| [パルマー・ラッキー氏のAnduril、軍用自律飛行VTOL機「Thunder」を公開](https://www.itmedia.co.jp/news/articles/2607/21/news052.html) | 21.0 | 20.0 | 42.0 |
| [患者の氏名・住所情報を利用し別の医療機関の開業案内を郵送](https://scan.netsecurity.ne.jp/article/2026/07/21/55740.html) | 21.0 | 20.0 | 42.0 |
| [システムから送信される「受領完了」メールに 22 名の個人情報記載](https://scan.netsecurity.ne.jp/article/2026/07/21/55738.html) | 21.0 | 20.0 | 42.0 |
| [愛知県農業共済組合のメールアドレスに不正アクセス、大量の迷惑メール発信](https://scan.netsecurity.ne.jp/article/2026/07/21/55737.html) | 21.0 | 20.0 | 42.0 |
| [Apache Tomcat に複数の脆弱性](https://scan.netsecurity.ne.jp/article/2026/07/21/55735.html) | 21.0 | 20.0 | 42.0 |
| [Tera Term の TTSSH2 プラグインに複数の脆弱性](https://scan.netsecurity.ne.jp/article/2026/07/21/55734.html) | 21.0 | 20.0 | 42.0 |
| [サプライチェーン対策と同じでは守れない？ グループ会社に必要なセキュリティガバナンスとは](https://scan.netsecurity.ne.jp/article/2026/07/21/55732.html) | 21.0 | 20.0 | 42.0 |
| [ニチレイへのサイバー攻撃はなぜ起きた？ 「たまたま選ばれる」被害の構造](https://www.itmedia.co.jp/enterprise/articles/2607/21/news028.html) | 21.0 | 20.0 | 42.0 |
| [九州電力送配電、顧客情報1354万件漏洩の恐れ データ保存用のSSD紛失](https://xtech.nikkei.com/atcl/nxt/column/18/01157/071400165/) | 21.0 | 20.0 | 42.0 |
| [顧客情報1354万件漏洩の恐れ SSD紛失、例外運用のリスク露呈](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020600011/071300211/) | 21.0 | 20.0 | 42.0 |
| [脆弱性報告を受け付けない企業は危うい？ CISAら5機関が共同指針](https://atmarkit.itmedia.co.jp/ait/articles/2607/21/news027.html) | 21.0 | 20.0 | 42.0 |
| [IPA、DX・AI活用のセキュリティリスクに備える「東北サイバーセキュリティシンポジウム2026」を仙台で11月に開催](https://internet.watch.impress.co.jp/docs/news/2126191.html) | 20.0 | 20.0 | 42.0 |
| [Estée Lauder、Oracle E-Businessの脆弱性によるデータ侵害を公表](https://www.bleepingcomputer.com/news/security/est-e-lauder-discloses-data-breach-via-oracle-e-business-flaw/) | 20.0 | 20.0 | 42.0 |
| [Off-chain攻撃でOstiumから2,370万ドル相当の暗号資産が盗まれる](https://www.bleepingcomputer.com/news/security/hackers-steal-237-million-in-crypto-from-ostium-in-off-chain-attack/) | 20.0 | 20.0 | 42.0 |
| [佐川急便、「スマートクラブ」で約7万人の個人情報漏えい。サイバー攻撃ではなくシステム不具合が原因](https://internet.watch.impress.co.jp/docs/news/2126372.html) | 20.0 | 20.0 | 42.0 |
| [LLMを活用した脆弱性対処：Ivantiの自動化推進の内幕](https://www.darkreading.com/cybersecurity-operations/remediating-vulnerabilities-llms-ivanti-automation) | 20.0 | 20.0 | 42.0 |
| [SNS上でFBIを装う詐欺師、犯罪被害者を狙う](https://www.theregister.com/security/2026/07/20/scammers-impersonate-fbi-on-social-media-prey-on-crime-victims/5275224) | 20.0 | 20.0 | 42.0 |

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
