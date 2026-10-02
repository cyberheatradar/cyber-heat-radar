# 📡 サイレーダー 2026-10-03 05:00 JST

このレポートは、2026-10-02 17:00 JST〜2026-10-03 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 80
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 49

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Exploited Fortinet FortiMail Zero-Day Calls for Urgent Action](#topic-35559) | 52.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [Kiteworks & Citrix Incidents Show Challenges of Zero-Day Response](#topic-35643) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Two Zero-Days Exploited in Attack on Dutch Institute for Vulnerability Disclosure](#topic-35705) | 37.0 | 38.0 | 43.0 | 音声 | AI×Security枠 |
| 4 | [Defending against AI-fueled cyberattacks requires focus on identity, data governance, Microsoft says](#topic-35647) | 33.0 | 30.0 | 42.0 | 音声 | AI×Security枠 |
| 5 | [SMTP is the key: BPFDoor and AVERAT hitting the network edge](#topic-35671) | 33.0 | 23.0 | 49.0 | 音声 | 温度感上位枠 |
| 6 | [Microsoft: AI Cuts Post-Compromise Attack Time to Minutes](#topic-35660) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-35559"></a>

### 1. Exploited Fortinet FortiMail Zero-Day Calls for Urgent Action

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 52.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Fortinetは、メールセキュリティ製品FortiMailに存在する重大な脆弱性CVE-2026-104286について注意喚起しており、ゼロデイとして悪用されているとされています。
報告では、認可されていないコード実行や任意のファイル書き込みにつながる可能性が示されており、対策の適用が急がれています。
インターネットに接続された境界製品での悪用が示唆されており、影響範囲が広がるおそれがあります。
CISAの既知悪用脆弱性リストへの掲載報道もあり、優先度の高い対応対象として見られています。

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

- FortiMailの対象バージョンと公開済みの回避策・修正情報を確認し、速やかに適用する。
- 当該製品の管理画面やログを点検し、不審なアクセスや設定変更、想定外のファイル生成の有無を確認する。
- 外部公開している管理インターフェースがあれば露出を最小化し、必要に応じてアクセス制御を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-104286 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Fortinet | 言及あり | 0.80 | — |
| 製品 | Fortinet FortiGate | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-104286](https://nvd.nist.gov/vuln/detail/CVE-2026-104286) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Fortinet sounds the alarm over actively exploited FortiMail zero-day](https://www.theregister.com/security/2026/10/02/fortinet-sounds-the-alarm-over-actively-exploited-fortimail-zero-day/5300803) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical FortiMail zero-day exploited in the wild (CVE-2026-104286)](https://www.helpnetsecurity.com/2026/10/02/fortinet-fortimail-vulnerability-cve-2026-104286/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Exploited Fortinet FortiMail Zero-Day Calls for Urgent Action](https://www.securityweek.com/exploited-fortinet-fortimail-zero-day-calls-for-urgent-action/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical FortiMail Zero-Day Flaw Exploited in Attacks Allows Unauthenticated Arb](https://thehackernews.com/2026/10/critical-fortimail-zero-day-flaw.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Fortinet warns of critical FortiMail flaw exploited in zero-day attacks](https://www.bleepingcomputer.com/news/security/fortinet-warns-of-critical-fortimail-flaw-exploited-in-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [A Vulnerability in Fortinet FortiMail Could Allow for Arbitrary Code Execution](https://www.cisecurity.org/advisory/a-vulnerability-in-fortinet-fortimail-could-allow-for-arbitrary-code-execution_2026-108) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Fortinet warns that critical flaw in FortiMail is facing exploitation](https://www.cybersecuritydive.com/news/fortinet-critical-flaw-fortimail-exploitation/832017/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35643"></a>

### 2. Kiteworks & Citrix Incidents Show Challenges of Zero-Day Response

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

KiteworksとCitrixをめぐる事例が、ゼロデイ脆弱性への対応の難しさを示しています。
片方は顧客に対して一時的な停止を求め、もう一方は報告された攻撃への言及がないまま修正パッチを公開したとされています。
ゼロデイ対応では、被害抑止のための迅速な運用判断と、利用者への適切な情報提供の両立が求められます。
対応の遅れや情報不足は、管理者側の判断を難しくし、影響範囲の把握にも支障を与えます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象製品の緊急告知やパッチ情報を継続的に確認し、必要なら一時停止や回避策を速やかに検討する。
- 資産棚卸しを行い、該当製品の利用有無と影響範囲を把握しておく。
- ベンダー通知の有無にかかわらず、侵害の兆候を前提にログ確認と監視強化を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Citrix | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Kiteworks & Citrix Incidents Show Challenges of Zero-Day Response](https://www.darkreading.com/cybersecurity-operations/kiteworks-citrix-incidents-challenges-zero-day-response) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35705"></a>

### 3. Two Zero-Days Exploited in Attack on Dutch Institute for Vulnerability Disclosure

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

オランダの脆弱性開示機関への攻撃で、2件のゼロデイ脆弱性が悪用されたとされています。
公開情報では、攻撃にはZammadに関する脆弱性が関わっていたとされますが、詳細な手口や影響範囲の確定情報は限定的です。
ゼロデイの悪用が含まれるため、同種製品を利用する組織では早期の影響確認と対応が重要です。
脆弱性開示を担う組織自体が標的になった点も、サプライチェーンや関連業務への波及を考える上で注目されます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Zammadを利用している場合は、ベンダー情報と修正版の有無を確認する。
- 外部公開されているサポート窓口や問い合わせ基盤の設定、アクセス制御を点検する。
- 関連ログを確認し、不審な操作や未説明の通信がないかを洗い出す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Two Zero-Days Exploited in Attack on Dutch Institute for Vulnerability Disclosur](https://www.infosecurity-magazine.com/news/zerodays-dutch-institute/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35647"></a>

### 4. Defending against AI-fueled cyberattacks requires focus on identity, data governance, Microsoft says

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftの最新レポートでは、AIの普及に伴って脅威活動のあり方が変化しており、特にランサムウェアの一部が自動化される可能性が示されています。
防御の重点としては、ID管理とデータガバナンスの強化が挙げられています。AIの活用は攻撃側の効率化にもつながるため、従来の対策だけでは不十分になる可能性があります。
特に認証情報や重要データの管理は、被害の広がりを抑えるうえで実務上の重要度が高い分野です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ID管理の見直し: 多要素認証や特権管理、アカウントの棚卸しを継続する。
- データガバナンスの確認: 機密データの所在、アクセス権限、持ち出し経路を把握する。
- AI前提の脅威モデル更新: フィッシングやランサムウェアの自動化を念頭に、検知・教育・復旧手順を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Defending against AI-fueled cyberattacks requires focus on identity, data govern](https://www.cybersecuritydive.com/news/ai-cyberattacks-automation-identity-data-microsoft-report/832020/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35671"></a>

### 5. SMTP is the key: BPFDoor and AVERAT hitting the network edge

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>通⁠信⁠基⁠盤</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 23.0 |
| <nobr>確⁠度</nobr> | 49.0 |

#### 概要

Rapid7は、Linux向けのBPFDoor系サンプルやRekoobe系バックドア、そしてAVERATと呼ぶインプラントを含む一連の活動を分析し、通信事業者やネットワーク境界機器を狙った事例としてまとめました。
いずれもSMTPのような通常業務の通信に紛れ込む設計が見られ、韓国や台湾の環境で観測されたサンプルでは、対象環境に合わせた偽装やファイルレスに近い挙動が確認されています。
ネットワークの境界に置かれた機器は、外向き通信や中継機能を持つため、侵害されると検知しづらい踏み台になりやすい点が問題です。
特にSMTPや正規のプロセス名を悪用した隠蔽は、通常の監視では見落とされやすく、運用上の注意が必要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 技術詳細により影響確認が進みやすい。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- port 25 への不自然な送信元プロセスや、メール系でない機器からのSMTP通信を確認する。
- Linuxホストで raw socket や BPF フィルタの利用、削除済み実行ファイルの痕跡を監視する。
- 境界機器・NAS・DVRなどの管理面を見直し、未使用のVPN/PPTPや不要な外部公開を棚卸しする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Oracle | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| 製品 | Apache HTTP Server | 言及あり | 0.80 | — |
| 製品 | Ivanti Policy Secure | 言及あり | 0.80 | — |
| マルウェア | BPFdoor | 主題 | 0.80 | — |
| 攻撃/検証ツール | Responder | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [SMTP is the key: BPFDoor and AVERAT hitting the network edge](https://www.rapid7.com/blog/post/tr-smtp-is-the-key-bpfdoor-averat-hitting-the-network-edge) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-35660"></a>

### 6. Microsoft: AI Cuts Post-Compromise Attack Time to Minutes

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftは、攻撃者がAIを使って侵入後の攻撃をより速く、より大規模に進めていると警告しています。
これにより、防御側が対応するまでの時間が短くなり、事後対応の難しさが増しているとされています。
AIの活用によって、攻撃の実行速度や規模が従来より高まる可能性が示されており、検知や封じ込めの遅れが被害拡大につながりやすくなります。
防御側は、侵入後の初動対応をより短時間で行える体制が求められます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 侵入検知後の初動対応手順を見直し、調査・隔離・認証情報の保護を迅速に行える体制を確認する。
- ログ監視やアラート運用を再点検し、短時間で進む不審な横展開や権限昇格の兆候を見逃しにくくする。
- 多要素認証、特権アカウント管理、セッション保護などの基本対策を改めて徹底する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft: AI Cuts Post-Compromise Attack Time to Minutes](https://www.infosecurity-magazine.com/news/microsoft-ai-attack-time-minutes/) | <nobr>内容確認・補足情報</nobr> |

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
| [AIが攻撃者に先手を与えているとMicrosoftが警告](https://www.helpnetsecurity.com/2026/10/02/ai-cybersecurity-threats-microsoft-report/) | 33.0 | 20.0 | 42.0 |
| [中国のスパイがホワイトハウスやAnthropic関係者を装い、AI政策専門家を狙ってフィッシング攻撃](https://www.helpnetsecurity.com/2026/10/02/china-aligned-ta419-phishing-ai-policy-experts/) | 33.0 | 20.0 | 42.0 |
| [Warlock ransomwareによる水道・通信事業者へのSharePoint侵害攻撃](https://www.bleepingcomputer.com/news/security/warlock-ransomware-breach-sharepoint-in-water-telecom-operator-attacks/) | 28.0 | 30.0 | 42.0 |
| [ミシシッピ州の市長、ランサムウェア被害で市がシステム停止と発表](https://therecord.media/vicksburg-mississippi-government-ransomware-attack) | 28.0 | 30.0 | 42.0 |
| [ポルトガル語・スペイン語圏の重要インフラを狙った「Warlock」ランサムウェア攻撃](https://therecord.media/warlock-ransomware-used-in-critical-infrastructure-attacks) | 28.0 | 30.0 | 42.0 |
| [16歳の少年、KillSecランサムウェアグループの主導者として逮捕される](https://www.itpro.com/security/ransomware/16-year-old-boy-arrested-for-masterminding-killsec-ransomware-group) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア関連の法執行・司法措置](https://www.infosecurity-magazine.com/news/police-target-killsec-ransomware/) | 28.0 | 30.0 | 42.0 |
| [AntinoバックドアがOutlookとOneDriveをC2に悪用した中国関連のスパイ活動キャンペーン](https://thehackernews.com/2026/10/antino-backdoor-uses-outlook-and.html) | 28.0 | 20.0 | 42.0 |
| [Android 17の高度な保護機能が検証済みアクセシビリティツールに対してアクセシビリティサービスを制限する](https://thehackernews.com/2026/10/android-17-advanced-protection-locks.html) | 28.0 | 20.0 | 42.0 |
| [agentic AIによるハッキングが提起する法的課題](https://cyberscoop.com/ai-agent-hacks-legal-liability-cfaa/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、100以上の組織に「ミスアラインされたモデル」が侵入を試みた可能性を警告](https://www.theregister.com/security/2026/10/02/openai-alerts-100-orgs-that-its-misaligned-models-attempted-to-break-in-or-worse/5300891) | 25.0 | 20.0 | 42.0 |
| [GitLab、セルフホスト型サーバーでコマンド実行を許すAI Gatewayの重大な脆弱性を修正](https://thehackernews.com/2026/10/gitlab-patches-critical-self-hosted-ai.html) | 25.0 | 20.0 | 42.0 |
| [GitLabのAI Gatewayサービスにおける重要なRCE脆弱性を警告](https://www.bleepingcomputer.com/news/security/gitlab-warns-of-critical-rce-vulnerability-in-ai-gateway-service/) | 25.0 | 20.0 | 42.0 |
| [2027年のAI説明責任時代に組織は備えていますか](https://www.darkreading.com/cybersecurity-operations/is-your-organization-ready-for-2027-s-ai-accountability-era-) | 25.0 | 20.0 | 42.0 |
| [「Rogue」なAIにセキュリティ障害の責任を負わせるのは公平か](https://www.darkreading.com/insider-threats/blame-rogue-ai-security-failures) | 25.0 | 20.0 | 42.0 |
| [OpenAIの自律AIエージェント巡る問題でカリフォルニア州が召喚状発行](https://www.theregister.com/ai-and-ml/2026/10/02/openais-wandering-ai-agents-earn-it-a-california-subpoena/5300850) | 25.0 | 20.0 | 42.0 |
| [その他のニュース：1万5000ドルのiCloudなりすまし脆弱性、AIポリシー専門家がフィッシング被害、広告ブロッカーがAIチャットを監視](https://www.securityweek.com/in-other-news-15k-icloud-spoofing-bugs-ai-policy-experts-phished-adblocker-spies-on-ai-chats/) | 25.0 | 20.0 | 42.0 |
| [アカウント悪用を調査するための新しいダッシュボード](https://blog.cloudflare.com/account-abuse-protection-dashboard/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、機密情報の取り扱い不備で安全性研究者3名と契約終了](https://thehackernews.com/2026/10/openai-parts-ways-with-three-safety.html) | 25.0 | 20.0 | 42.0 |
| [中国のハッカーが著名なAI関係者を装って認証情報を窃取](https://www.itpro.com/security/cyber-crime/chinese-hackers-impersonate-leading-ai-figures-to-harvest-credentials) | 25.0 | 20.0 | 42.0 |
| [AIエージェントが米国およびカナダの政府サイトを標的にSQLインジェクションを実行](https://www.securityweek.com/ai-agents-aimed-sql-injection-at-us-and-canadian-government-sites/) | 25.0 | 20.0 | 42.0 |
| [Dell CSMの脆弱性によりKubernetesノードで認証不要の管理者アクセスとroot権限取得が可能に](https://thehackernews.com/2026/10/dell-csm-flaws-enable-unauthenticated.html) | 24.0 | 46.0 | 50.0 |
| [SWIFT BankingおよびGovernment MiddlewareでRCEが可能に](https://www.darkreading.com/cybersecurity-operations/swift-banking-govt-middleware-rce) | 24.0 | 38.0 | 42.0 |
| [AIでOTセキュリティ運用を自動化、NTTドコモビジネスとPKTが新システムを開発](https://news.mynavi.jp/techplus/article/20261002-5063094/) | 24.0 | 20.0 | 43.0 |
| [本人確認書類の画像流出、対象アカウントは約160万件 - タイムズカー](https://www.security-next.com/190989) | 22.0 | 20.0 | 42.0 |
| [荷物問合サービスが侵害、個人情報流出の可能性 - 佐川急便](https://www.security-next.com/190952) | 22.0 | 20.0 | 42.0 |
| [研究用原子炉利用者の身分証明書などが外部流出 - 原子力機構](https://www.security-next.com/190957) | 22.0 | 20.0 | 42.0 |
| [ヤマト運輸、「クロネコ代金後払いサービス」への不正アクセスで続報 利用者など一部個人情報が漏えいか](https://www.itmedia.co.jp/news/article/2610/02/2000001979/) | 21.0 | 20.0 | 42.0 |
| [日本エネルギー経済研究所、不正アクセスの続報 パスポート情報13件の漏えい確認](https://www.itmedia.co.jp/news/article/2610/02/2000001976/) | 21.0 | 20.0 | 42.0 |
| [サイリーグHDら、AIでサイバー攻撃時の初動対応を支援する新サービスを発表](https://japan.zdnet.com/article/35253195/) | 21.0 | 20.0 | 42.0 |
| [Protected Quick Tunnels：次の開発プロジェクト向けの簡単なアカウント不要認証](https://blog.cloudflare.com/protected-quick-tunnels/) | 20.0 | 20.0 | 48.0 |
| [Frontline Educationの侵害で学校区職員データが流出](https://www.bleepingcomputer.com/news/security/frontline-education-data-breach-impacts-school-district-employees/) | 20.0 | 20.0 | 42.0 |
| [Lunex、BYOVDを悪用してセキュリティ監視を無効化し、永続的な情報窃取マルウェアを展開](https://blog.polyswarm.io/lunex-uses-byovd-to-disable-security-monitoring-and-deploy-persistent-stealer) | 20.0 | 20.0 | 42.0 |
| [米国、ATMハッキング取り締まりでTren de Araguaメンバーに制裁](https://www.bleepingcomputer.com/news/security/us-sanctions-tren-de-aragua-members-in-atm-jackpotting-crackdown/) | 20.0 | 20.0 | 42.0 |
| [Cyber Brief 26-10 - 2026年9月版](https://cert.europa.eu/publications/threat-intelligence/cb26-10/) | 20.0 | 20.0 | 42.0 |
| [第一ライフG 従業員情報漏えいか](https://news.yahoo.co.jp/pickup/6597333?source=rss) | 20.0 | 20.0 | 42.0 |
| [EDRの盲点：ブラウザ攻撃がエンドポイントテレメトリを回避する3つの手法](https://www.bleepingcomputer.com/news/security/the-edr-blind-spot-3-ways-browser-attacks-evade-endpoint-telemetry/) | 20.0 | 20.0 | 42.0 |
| [脆弱性バックログはオーナーシップの問題である](https://www.darkreading.com/cybersecurity-operations/vulnerability-backlogs-ownership-problem) | 20.0 | 20.0 | 42.0 |
| [情報漏えい相次ぐ「異様」と識者](https://news.yahoo.co.jp/pickup/6597326?source=rss) | 20.0 | 20.0 | 42.0 |
| [macOSユーザーを狙う偽ZoomインストーラーによるCloudSyncDバックドア配布](https://www.securityweek.com/macos-users-targeted-by-fake-zoom-installer-carrying-cloudsyncd-backdoor/) | 20.0 | 20.0 | 42.0 |
| [悪意あるLinuxインプラントがアジアのメールセキュリティ製品を装う](https://www.darkreading.com/threat-intelligence/malicious-linux-implants-mimic-asian-mail-security) | 20.0 | 20.0 | 42.0 |
| [Dell、CSMの最大深刻度の脆弱性を早急に修正するよう管理者に呼びかけ](https://www.bleepingcomputer.com/news/security/new-max-severity-dell-csm-flaws-give-hackers-admin-privileges/) | 20.0 | 20.0 | 42.0 |
| [Crypto ScammersがMicrosoftの公式Xアカウントを乗っ取り](https://www.securityweek.com/crypto-scammers-hijack-microsofts-official-x-account/) | 20.0 | 20.0 | 42.0 |
| [CISOが取締役会の3つの難しい質問に答えられない理由と、その改善方法](https://thehackernews.com/2026/10/why-cisos-struggle-to-answer-boards.html) | 20.0 | 20.0 | 42.0 |
| [まれな措置で、イランの国家関与ハッカー容疑者が米国に身柄引き渡し](https://www.securityweek.com/in-rare-move-iranian-hacker-accused-of-working-for-irgc-extradited-to-us/) | 20.0 | 20.0 | 42.0 |
| [ヤマト運輸「クロネコ代金後払いサービス」、不正アクセスで情報漏えいの可能性](https://internet.watch.impress.co.jp/docs/news/2145352.html) | 20.0 | 20.0 | 42.0 |
| [佐川急便「お荷物問い合わせサービス」不正アクセスにより情報流出の可能性、ウェブの荷物問い合わせなどを停止中](https://internet.watch.impress.co.jp/docs/news/2145343.html) | 20.0 | 20.0 | 42.0 |
| [Warlockが重要インフラ攻撃でSharePointの悪用を拡大](https://www.securityweek.com/warlock-expands-sharepoint-exploitation-in-critical-infrastructure-attacks/) | 20.0 | 20.0 | 42.0 |
| [MicrosoftのXアカウントが仮想通貨のポンプ・アンド・ダンプ詐欺に悪用される](https://www.bleepingcomputer.com/news/security/microsofts-x-account-hacked-in-crypto-token-pump-and-dump-scheme/) | 20.0 | 20.0 | 42.0 |

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
