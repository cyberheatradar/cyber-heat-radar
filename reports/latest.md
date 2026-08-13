# 📡 サイレーダー 2026-08-14 05:00 JST

このレポートは、2026-08-13 17:00 JST〜2026-08-14 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 86
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 56

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Attackers exploit critical SharePoint flaw after PoC goes public (CVE-2026-55040)](#topic-27420) | 42.0 | 56.0 | 56.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [Microsoft patches LegacyHive Windows zero-day vulnerability](#topic-27465) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Nightmare Eclipse Drops Windows Zero-Day Exploit ‘ShieldBreak’](#topic-27556) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [ANDRITZ HIPASE-250 and 250 SCALA](#topic-27507) | 32.0 | 46.0 | 50.0 | 音声 | 温度感上位枠 |
| 5 | [Hitachi Energy APM Edge Product](#topic-1916) | 30.0 | 50.0 | 67.0 | 音声 | 温度感上位枠 |
| 6 | [VPN機器経由でランサム被害、メアド変更など対策実施 - 丸高興業](#topic-27546) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-27465"></a>

### 1. Microsoft patches LegacyHive Windows zero-day vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Microsoftは、Windowsのゼロデイ脆弱性「LegacyHive」に対する修正パッチを公開したとされています。
材料上は、7月のPatch Tuesday後に明らかになった事案で、悪用観測がある文脈として扱われています。
ゼロデイかつ悪用情報があるとされるため、対応の遅れが影響拡大につながるおそれがあります。Windows環境を広く運用する組織では、優先度を上げて評価すべき話題です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象Windows環境で、該当する修正プログラムの適用状況を確認する。
- 資産台帳と脆弱性管理を突き合わせ、未適用端末を優先的に洗い出す。
- 関連する監視ログや異常挙動を点検し、必要に応じて追加の防御策を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-62832 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft patches LegacyHive Windows zero-day vulnerability](https://www.bleepingcomputer.com/news/microsoft/microsoft-patches-legacyhive-windows-zero-day-vulnerability/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-27556"></a>

### 2. Nightmare Eclipse Drops Windows Zero-Day Exploit ‘ShieldBreak’

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Windows向けのゼロデイ脆弱性に関する公開情報が伝えられており、当該エクスプロイトは高い権限を得られる可能性があるとされています。
現時点では詳細な悪用条件や影響範囲は限定的な情報にとどまり、一次情報に基づく確認が必要です。
権限昇格につながる脆弱性は、端末内での防御を回避して被害を拡大させるおそれがあるため注目されます。ゼロデイとされる場合、修正公開前後の運用判断が特に重要になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Windows端末の修正状況を確認し、関連する更新プログラムを優先適用する。
- EDRや監査ログで不審な権限昇格やシェル起動の兆候がないか確認する。
- 特権アカウントの利用を最小化し、管理者権限の分離を徹底する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-50656 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Nightmare Eclipse Drops Windows Zero-Day Exploit ‘ShieldBreak’](https://www.securityweek.com/nightmare-eclipse-drops-windows-zero-day-exploit-shieldbreak/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-27507"></a>

### 3. ANDRITZ HIPASE-250 and 250 SCALA

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 32.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 50.0 |

#### 概要

CISAは、ANDRITZの産業制御向け製品「HIPASE-250」と「250 SCALA」に複数の脆弱性があると公表しました。
影響を受けるのは両製品の7.20以下で、認証不備やハードコードされた認証情報、復元可能な形式でのパスワード保存に関する問題が含まれます。
認証なしで機器情報や設定にアクセスできる可能性があり、監査ログの抑制やワークステーションへの不正アクセスにつながるおそれがあります。
エネルギー分野で使われる制御機器に関するため、運用影響の観点でも確認が必要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象バージョンが7.20以下に該当しないか確認する。
- 公開範囲やネットワーク分離、認証設定を見直す。
- ベンダー修正版への更新可否を早急に評価する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-65309 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-65310 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-65311 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-65313 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-65309](https://nvd.nist.gov/vuln/detail/CVE-2026-65309) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [ANDRITZ HIPASE-250 and 250 SCALA](https://www.cisa.gov/news-events/ics-advisories/icsa-26-225-05) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-1916"></a>

### 4. Hitachi Energy APM Edge Product

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>M⁠C⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 50.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Hitachi Energy APM Edge Productに関する公開情報では、Dirty Fragと呼ばれるLinuxの権限昇格脆弱性の影響が整理されており、対象バージョンはAPM Edge 6.10以下とされています。
公開資料では、影響を受ける状況では機密性・完全性・可用性に影響しうると説明されています。
公開PoCや検証コードの言及があり、初期侵入後の権限昇格リスクとして実務上の優先度が高いと見られます。
対象製品を使う環境では、既存侵害の拡大や管理者権限奪取につながる可能性があるため注意が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
- 公開PoC・検証コード言及あり。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 公開PoCにより再現・悪用可能性が上がる。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- APM Edge 6.10以下を利用しているかを確認し、ベンダーの修正・緩和策の適用状況を点検する。
- Linuxホスト上の不審な権限昇格の兆候や、低権限アカウントからの異常な挙動を監視する。
- 公開PoCの存在を踏まえ、関連システムの露出を最小化し、初期侵入対策とインシデント対応手順を再確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Citrix | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-43284](https://nvd.nist.gov/vuln/detail/CVE-2026-43284) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Hitachi Energy APM Edge Product](https://www.cisa.gov/news-events/ics-advisories/icsa-26-225-04) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Linux Kernel vulnerability Dirty Frag](https://fortiguard.fortinet.com/psirt/FG-IR-26-144) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Metasploit Wrap Up 05/29/2026](https://www.rapid7.com/blog/post/pt-metasploit-wrap-up-05-29-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [New ‘Dirty Frag’ Linux Vulnerability Possibly Exploited in Attacks](https://www.securityweek.com/new-dirty-frag-linux-vulnerability-possibly-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Active attack: Dirty Frag Linux vulnerability expands post-compromise risk](https://www.microsoft.com/en-us/security/blog/2026/05/08/active-attack-dirty-frag-linux-vulnerability-expands-post-compromise-risk/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Dirty Frag: Unpatched Linux vulnerability delivers root access](https://www.helpnetsecurity.com/2026/05/08/dirty-frag-linux-vulnerability-cve-2026-43284-cve-2026-43500/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-27546"></a>

### 5. VPN機器経由でランサム被害、メアド変更など対策実施 - 丸高興業

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

丸高興業は、サーバがランサムウェア攻撃を受けた件について公表し、顧客の個人情報が流出した可能性があるとしています。
あわせて、メアド変更などの対策を進めていることが示されています。VPN機器を起点とする侵入が疑われる事案として、外部接続機器の管理や認証強化の重要性が改めて注目されます。
個人情報の流出可能性があるため、顧客対応や影響範囲の確認も実務上の焦点になります。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- VPN機器やリモート接続経路の設定、認証、ログ管理を再点検する。
- ランサムウェア被害時の初動として、影響範囲の特定と重要データの保全を優先する。
- 個人情報の流出可能性がある場合に備え、通知・問い合わせ対応の手順を確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [VPN機器経由でランサム被害、メアド変更など対策実施 - 丸高興業](https://www.security-next.com/188142) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-27420"></a>

### 1. Attackers exploit critical SharePoint flaw after PoC goes public (CVE-2026-55040)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 42.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 56.0 |

#### 概要

Microsoft SharePointの脆弱性CVE-2026-55040について、公開されたPoCコードをきっかけに実際の悪用が始まったと複数ソースで伝えられています。
この問題は認証の不備に起因する重要なセキュリティ機能のバイパスとされ、Microsoftは2026年7月の更新で修正済みです。
認証回避につながる脆弱性は、情報漏えいやデータ改ざんなどの被害に直結しやすく、公開PoC後は悪用のハードルが下がります。
SharePointを利用する組織では、修正済みであっても適用状況と露出範囲の確認が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SharePointの該当パッチ適用状況を確認し、未適用環境がないか洗い出す。
- 外部公開されたSharePoint関連エンドポイントや認証まわりの異常ログを重点的に監視する。
- 脆弱性情報の更新に合わせて、影響対象の資産一覧と優先順位を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-55040 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-55040](https://nvd.nist.gov/vuln/detail/CVE-2026-55040) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Attackers exploit critical SharePoint flaw after PoC goes public (CVE-2026-55040](https://www.helpnetsecurity.com/2026/08/13/microsoft-sharepoint-cve-2026-55040-poc-exploit/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit SharePoint Authentication Bypass After Public PoC Release](https://thehackernews.com/2026/08/attackers-exploit-sharepoint.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [重大なVMware vCenterのRCE脆弱性が悪用され逆SSHアクセスを許す問題](https://www.bleepingcomputer.com/news/security/critical-vmware-vcenter-rce-flaw-exploited-for-reverse-ssh-access/) | 28.0 | 46.0 | 54.0 |
| [Microsoftが約束しなかったバックアップ](https://www.theregister.com/security/2026/08/13/sponsored-the-backup-microsoft-never-promised-you/5284957) | 28.0 | 30.0 | 42.0 |
| [Ransomwareの現状 Q2 2026](https://research.checkpoint.com/2026/the-state-of-ransomware-q2-2026/) | 28.0 | 30.0 | 42.0 |
| [Akiraのアフィリエイト、EDR回避を試みた後にランサムウェアをクラッシュさせる](https://www.infosecurity-magazine.com/news/akira-affiliate-crashes-ransomware/) | 28.0 | 30.0 | 42.0 |
| [新たなAndroidマルウェア、犯罪者が銀行カードをリアルタイムで悪用可能に](https://www.malwarebytes.com/blog/mobile/2026/08/new-android-malware-lets-criminals-use-your-bank-card-in-real-time) | 28.0 | 20.0 | 48.0 |
| [Miraiの新亜種が悪名高いボットネットコードにステルス機能を追加](https://therecord.media/new-mirai-variant-adds-stealth-to-botnet-code) | 28.0 | 20.0 | 42.0 |
| [GitHub PAT侵害の調査方法：複数組織を標的としたキャンペーンから得た教訓](https://www.wiz.io/blog/investigating-github-pat-compromise) | 28.0 | 20.0 | 42.0 |
| [ホワイトハウス、米国の民間企業による国外犯罪ネットワークへのハッキングを承認](https://www.helpnetsecurity.com/2026/08/13/usa-private-companies-offensive-cyber-operations/) | 28.0 | 20.0 | 42.0 |
| [モデル自体がマルウェア――4つのAgentic侵入が防御側に示すこと](https://www.sentinelone.com/labs/the-model-is-the-malware-what-four-agentic-intrusions-tell-defenders/) | 28.0 | 20.0 | 42.0 |
| [Jewelbug：APTグループがスパイ活動と暗号資産詐欺を並行して実施](https://www.security.com/threat-intelligence/jewelbug-crypto-fraud-espionage) | 28.0 | 20.0 | 42.0 |
| [「Jewelbug」APT、国家スパイ活動と暗号資産窃取を両立](https://www.darkreading.com/threat-intelligence/jewelbug-apt-state-espionage-cryptocurrency-theft) | 28.0 | 20.0 | 42.0 |
| [Armored Likhoがサイバー諜報ツールキットを拡張](https://securelist.com/armored-likho-still-toolkit/121033/) | 28.0 | 20.0 | 42.0 |
| [AIモデルに子ども向けの動物物語を作らせると女性キャラをほぼ完全に排除してしまう](https://gigazine.net/news/20260813-ai-erase-female-characters-kids-stories/) | 27.0 | 20.0 | 42.0 |
| [AIウォーターマーク除去ツールがネット上に氾濫、ほとんど効果を証明できず](https://www.bleepingcomputer.com/news/security/ai-watermark-removers-flood-the-web-almost-none-can-prove-they-work/) | 25.0 | 20.0 | 42.0 |
| [AIの「中堅層」がハッキング能力を大幅に向上させた](https://cyberscoop.com/mid-tier-ai-models-hacking-threat/) | 25.0 | 20.0 | 42.0 |
| [50のオープンソースプロジェクトから学んだAI時代のセキュリティ](https://github.blog/open-source/maintainers/what-50-open-source-projects-taught-us-about-security-in-the-ai-era/) | 25.0 | 20.0 | 42.0 |
| [地下フォーラムで販売されるAI搭載ハッキングツールを研究者が発見](https://www.cybersecuritydive.com/news/ai-hacking-tools-sale-underground-forums/827807/) | 25.0 | 20.0 | 42.0 |
| [誰がAIのコードを検証するのか：オープンソース取り込みが直面する規模の課題](https://www.bleepingcomputer.com/news/security/who-vets-ais-code-the-scale-challenge-facing-open-source-ingestion/) | 25.0 | 20.0 | 42.0 |
| [DataGroutで企業のAI利用、ガバナンス、LLMコストを管理する方法](https://www.helpnetsecurity.com/2026/08/13/selecthub-datagrout-llm-inference-optimization/) | 25.0 | 20.0 | 42.0 |
| [A10 Networksが企業向けAIを保護・管理するAI Gatewayを発表](https://www.helpnetsecurity.com/2026/08/13/a10-networks-introduces-ai-gateway-to-secure-and-manage-enterprise-ai/) | 25.0 | 20.0 | 42.0 |
| [Searchlight Cyberが露出情報と脅威インテリジェンスを統合した新PTEMプラットフォームを発表](https://www.helpnetsecurity.com/2026/08/13/searchlight-cyber-preemptive-threat-exposure-management-ptem-platform/) | 25.0 | 20.0 | 42.0 |
| [Siemens Siveillance Videoの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-225-09) | 24.0 | 46.0 | 50.0 |
| [Haiwell IoT Cloud HMI Gatewayの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-225-02) | 24.0 | 46.0 | 50.0 |
| [WordPress 7.0.4、リモートコード実行の脆弱性を修正](https://www.securityweek.com/wordpress-7-0-4-patches-remote-code-execution-vulnerability/) | 24.0 | 38.0 | 42.0 |
| [Curiouser and Curiouser](https://blog.talosintelligence.com/curiouser-and-curiouser/) | 22.0 | 20.0 | 48.0 |
| [JWRフィッシングフレームワークの解析](https://blog.talosintelligence.com/dissecting-the-jwr-phishing-framework/) | 22.0 | 20.0 | 48.0 |
| [AI会議録サービス「tl;dv」で18万件超の会議メタデータにアクセス可能だったと研究者が報告、会社側は「別々の2つの脆弱性」と説明](https://gigazine.net/news/20260813-tldv-data-hack/) | 22.0 | 20.0 | 42.0 |
| [情報共有用のクラウドストレージに不正アクセス - 扶桑電通](https://www.security-next.com/187742) | 22.0 | 20.0 | 42.0 |
| [Johnson Controls Metasysの脆弱性とセキュリティ動向](https://www.cisa.gov/news-events/ics-advisories/icsa-26-225-14) | 21.0 | 34.0 | 50.0 |
| [Adobe Commerceのバグが公開直後に標的化](https://www.securityweek.com/adobe-commerce-bug-targeted-immediately-after-disclosure/) | 21.0 | 28.0 | 54.0 |
| [露出したAWSアクセスキーに関連する1500以上の英国慈善団体へのデータ侵害](https://www.infosecurity-magazine.com/news/exposed-aws-key-data-charities/) | 21.0 | 20.0 | 43.0 |
| [AVEVA Enterprise SCADAの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-225-01) | 20.0 | 28.0 | 50.0 |
| [Flow Neuroscience FL-100の脆弱性](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-225-01) | 20.0 | 28.0 | 50.0 |
| [Johnson Controls Inc. Airwall の脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-225-03) | 20.0 | 28.0 | 50.0 |
| [ハッカーが暗号資産詐欺を進める中で政府のWebメールに侵入](https://www.bleepingcomputer.com/news/security/hackers-breach-govt-webmail-while-running-parallel-crypto-fraud/) | 20.0 | 20.0 | 42.0 |
| [Trezorが約1万4000人の顧客に影響するデータ侵害を公表](https://www.bleepingcomputer.com/news/security/trezor-discloses-data-breach-affecting-nearly-14-000-customers/) | 20.0 | 20.0 | 42.0 |
| [米国政府、民間企業による犯罪組織へのハッキングを容認](https://www.cybersecuritydive.com/news/us-private-companies-gangs-cyberattacks-offensive-operations/827805/) | 20.0 | 20.0 | 42.0 |
| [Trump氏が民間サイバー企業にハッキング反撃のライセンスを与えようとしている](https://www.theregister.com/security/2026/08/13/trump-wants-to-grant-private-cyber-firms-a-license-to-hack-back/5287420) | 20.0 | 20.0 | 42.0 |
| [Google Cloud、初の主要な耐量子セキュリティマイルストーンを2027年に目標設定](https://www.infosecurity-magazine.com/news/google-cloud-post-quantum-roadmap/) | 20.0 | 20.0 | 42.0 |
| [2026年7月に発表されたサイバーセキュリティM&Aの動向：21件の買収・合併発表](https://www.securityweek.com/cybersecurity-ma-roundup-21-deals-announced-in-july-2026/) | 20.0 | 20.0 | 42.0 |
| [vCenterの脆弱性、公開からわずか5日で悪用される](https://www.infosecurity-magazine.com/news/vcenter-cve-2026-59310-exploited/) | 20.0 | 20.0 | 42.0 |
| [ソフトウェアサプライチェーンにおける個人リポジトリの保護と盲点の解消](https://www.wiz.io/blog/securing-personal-repositories) | 20.0 | 20.0 | 42.0 |
| [White Houseがセキュリティ企業を攻撃的なハックバック作戦に動員](https://www.bleepingcomputer.com/news/security/white-house-taps-security-firms-for-offensive-hack-back-operations/) | 20.0 | 20.0 | 42.0 |
| [Trump、サイバー企業を犯罪者への攻勢に動員](https://therecord.media/trump-cyber-crime-offensive) | 20.0 | 20.0 | 42.0 |
| [Tech FLAMEを絶やさずに：Trailblazer Suzanne Wheeler](https://www.akamai.com/blog/culture/2026/aug/keep-your-tech-flame-alive-trailblazer-suzanne-wheeler) | 20.0 | 20.0 | 42.0 |
| [ドイツ、諜報機関にハッキングと妨害工作の権限付与へ](https://therecord.media/germany-spy-agency-powers) | 20.0 | 20.0 | 42.0 |
| [Trump、民間企業の攻撃的サイバー作戦参加を承認](https://www.infosecurity-magazine.com/news/trump-private-offensive-cyber/) | 20.0 | 20.0 | 42.0 |
| [BitLocker PINがデータとデバイスを保護する仕組み](https://www.ncsc.gov.uk/blogs/how-bitlocker-pins-help-protect-your-data-and-devices) | 20.0 | 20.0 | 42.0 |
| [Trump、攻撃的ハッキング作戦のメモで民間部門に協力を求める](https://cyberscoop.com/trump-memo-private-sector-offensive-hacking/) | 20.0 | 20.0 | 42.0 |
| [ベンチャー企業Team8、追加で3億6500万ドルを調達](https://www.securityweek.com/venture-firm-team8-secures-additional-365-million/) | 20.0 | 20.0 | 42.0 |
| [JavaScript内でAWSキーが露出しBeaconの慈善団体データ流出につながった可能性](https://www.theregister.com/security/2026/08/13/aws-key-exposed-in-javascript-may-have-lit-way-to-beacons-charity-data/5287303) | 20.0 | 20.0 | 42.0 |
| [FortiWebとFortiManagerの認証不備を修正するFortinetのパッチ公開](https://www.securityweek.com/fortinet-patches-authentication-flaws-in-fortiweb-and-fortimanager/) | 20.0 | 20.0 | 42.0 |
| [LiteLLMのサプライチェーン攻撃後に153GBの盗まれた認証情報が流出](https://www.helpnetsecurity.com/2026/08/13/litellm-breach-stolen-credentials-leak/) | 20.0 | 20.0 | 42.0 |
| [今年のLiteLLMのサプライチェーン攻撃は史上最大規模の可能性がある](https://www.itpro.com/security/cyber-attacks/the-litellm-supply-chain-attack-this-year-could-be-the-biggest-ever) | 20.0 | 20.0 | 42.0 |
| [Meta、TikTok、Google、Snapを相手取った3,000件の青少年安全訴訟](https://www.malwarebytes.com/blog/privacy/2026/08/parents-take-on-meta-tiktok-google-and-snap-in-3000-youth-safety-lawsuits) | 20.0 | 20.0 | 42.0 |
| [ホワイトハウス、外国サイバー犯罪組織への対策でセキュリティ企業を動員](https://www.securityweek.com/white-house-mobilizes-security-firms-for-operations-against-foreign-cybercrime-gangs/) | 20.0 | 20.0 | 42.0 |

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
