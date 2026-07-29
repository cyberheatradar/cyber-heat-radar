# 📡 サイレーダー 2026-07-30 05:00 JST

このレポートは、2026-07-29 17:00 JST〜2026-07-30 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 108
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 78

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cleaning Out Inboxes: TA488 Comes for Outlook with Another Half-Click Exploit](#topic-5098) | 42.0 | 52.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [Stairwell launches Backstory, pioneering agentic investigation for malware blast radius](#topic-24968) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [Torq makes AI SOC investigations continuously self-learning](#topic-25035) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Public PoC Released for Exploited Check Point SmartConsole Authentication Bypass](#topic-24022) | 30.0 | 56.0 | 65.0 | 音声 | 温度感上位枠 |
| 5 | [サーバにランサム攻撃、顧客情報流出の可能性 - 名鉄協商](#topic-24963) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-5098"></a>

### 1. Cleaning Out Inboxes: TA488 Comes for Outlook with Another Half-Click Exploit

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 42.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 52.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Microsoft Exchange Server の脆弱性 CVE-2026-42897 が、公開情報では実際に悪用された事例があるとして扱われています。
関連報道では、Outlook Web Access（OWA）に対するXSS脆弱性とされ、政府機関や通信、金融、医療分野などが標的になった可能性が示されています。
CISA の Known Exploited Vulnerabilities（KEV）にも追加されており、机上の脆弱性ではなく実運用環境での対応が必要な案件です。
Exchange のオンプレミス環境に影響しうるため、メール基盤を持つ組織では優先度が高いと考えられます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- XSS系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Exchange Server の該当バージョンが影響を受けるか確認し、Microsoft が案内する緩和策や更新情報を適用する。
- OWA を含むメールアクセス経路の監視を強化し、不審な認証・閲覧・リダイレクト挙動がないか点検する。
- KEV 掲載の脆弱性として扱い、資産管理・パッチ管理の優先順位を上げる。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-42897 | 主題CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Exchange | 言及あり | 0.80 | — |
| ベンダー | Proofpoint | 言及あり | 0.80 | — |
| ベンダー | Zimbra | 言及あり | 0.80 | — |
| 製品 | Microsoft Exchange Server | 言及あり | 0.80 | — |
| 製品 | WordPress | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-42897](https://nvd.nist.gov/vuln/detail/CVE-2026-42897) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cleaning Out Inboxes: TA488 Comes for Outlook with Another Half-Click Exploit](https://www.proofpoint.com/us/blog/threat-insight/cleaning-out-inboxes-ta488-comes-outlook-another-half-click-exploit) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches Exploited Exchange Server Vulnerability](https://www.securityweek.com/microsoft-patches-exploited-exchange-server-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Exchange Zero-Day Under Attack, No Patch Available](https://www.darkreading.com/vulnerabilities-threats/microsoft-exchange-zero-day-no-patch) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Warns of Exchange Server Zero-Day Exploited in the Wild](https://www.securityweek.com/microsoft-warns-of-exchange-server-zero-day-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/05/15/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Unpatched Microsoft Exchange Server vulnerability exploited (CVE-2026-42897)](https://www.helpnetsecurity.com/2026/05/15/exchange-server-cve-2026-42897-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [On-Prem Microsoft Exchange Server CVE-2026-42897 Exploited via Crafted Email](https://thehackernews.com/2026/05/on-prem-microsoft-exchange-server-cve.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: あり（2件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-24968"></a>

### 2. Stairwell launches Backstory, pioneering agentic investigation for malware blast radius

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Stairwellが、マルウェアの関連変種や影響範囲を素早く把握するための調査プラットフォーム「Backstory」を発表しました。
AIで生成された新しい変種が増える中、既存のアラート中心の運用だけでは対応しきれない場面を補う狙いがうかがえます。
侵害後の影響範囲確認や封じ込め判断は初動対応の遅れに直結するため、調査を短時間で支援する仕組みは実務上の関心が高いです。
AIを悪用した変種増加という文脈とも重なり、検知後の分析・整理のあり方が問われています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- インシデント発生時に、影響を受けた資産や関連サンプルを短時間で整理できるかを確認する。
- 既存のSIEM/EDR/SOAR運用と、調査結果の連携やエスカレーション手順がどうなるかを見ておく。
- AI支援の分析結果でも、最終判断はログ・端末状況・封じ込め状況と突き合わせて検証する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Stairwell launches Backstory, pioneering agentic investigation for malware blast](https://www.helpnetsecurity.com/2026/07/29/stairwell-backstory-agentic-investigation/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-25035"></a>

### 3. Torq makes AI SOC investigations continuously self-learning

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Torqは、過去の調査履歴やアナリストの判断、組織固有の運用知識を取り込んで学習し続けるとする「Torq SOC Brain」を発表しました。
SOC向けのAI機能として、単なる履歴参照ではなく、運用に合わせて判断を改善していく点が特徴として説明されています。
SOC業務の自動化や支援において、AIが組織ごとの運用文脈をどこまで反映できるかは重要な論点です。
実運用での誤検知対応やトリアージの効率化に関わるため、導入時の期待値や検証方法が注目されます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 既存のSOC運用とどの程度整合するか、学習対象と判断基準を確認する。
- 過去事例の再利用だけでなく、誤った判断が蓄積しない運用設計になっているかを見る。
- 自動化範囲と人手による最終確認の切り分けを明確にする。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Torq makes AI SOC investigations continuously self-learning](https://www.helpnetsecurity.com/2026/07/29/torq-soc-brain/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-24022"></a>

### 4. Public PoC Released for Exploited Check Point SmartConsole Authentication Bypass

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 65.0 |

#### 概要

Check PointのSmartConsole認証バイパス脆弱性（CVE-2026-16232）について、公開PoCの存在が報じられています。
この脆弱性は管理サーバーに対する認証回避につながる可能性があり、Check Pointは実際に悪用が確認されているとしています。
管理系製品の脆弱性は、設定変更やアクセス制御の改変などにつながるため影響が大きくなりやすいです。
すでに悪用報告があるため、通常の更新待ちではなく早急な対応が必要な案件として注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- ランサムウェア文脈。
- 情報漏えい系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象バージョンの影響有無を確認し、ベンダー提供の修正を優先して適用する。
- 管理サーバーへの到達性を見直し、信頼済みクライアントや管理アクセス元を必要最小限に制限する。
- 管理者・SmartConsole・API・アプリケーショントークンの利用状況や、侵害の兆候がないかログを点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-16232 | 主題CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-62144 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-62145 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Check Point | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-16232](https://nvd.nist.gov/vuln/detail/CVE-2026-16232) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Public PoC Released for Exploited Check Point SmartConsole Authentication Bypass](https://thehackernews.com/2026/07/rapid7-releases-poc-for-exploited-check.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [27th July – Threat Intelligence Report](https://research.checkpoint.com/2026/27th-july-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-16232: Critical Check Point SmartConsole Authentication Bypass Exploite](https://www.rapid7.com/blog/post/etr-cve-2026-16232-critical-check-point-smartconsole-authentication-bypass-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers exploit critical Check Point flaw to take over firewall management (CV](https://www.helpnetsecurity.com/2026/07/23/check-point-vulnerability-cve-2026-16232/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [New Check Point Zero-Day Vulnerability Exploited in the Wild](https://www.securityweek.com/new-check-point-zero-day-vulnerability-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Check Point Patches Exploited SmartConsole Flaw Allowing Full Admin Access](https://thehackernews.com/2026/07/check-point-patches-exploited.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-24963"></a>

### 5. サーバにランサム攻撃、顧客情報流出の可能性 - 名鉄協商

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

名鉄協商は、サーバがランサムウェアによるサイバー攻撃を受け、顧客情報が流出した可能性があると公表しました。現時点では、流出の有無や対象範囲の詳細は確認中とみられます。
ランサムウェア被害では、システム停止に加えて情報漏えいの有無が事業と利用者の両面で重要になります。
顧客情報が含まれる可能性があるため、関係者への影響確認や対外対応の進捗が注目されます。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 影響を受けたサーバと保管データの範囲を早期に切り分け、漏えい可能性のある情報種別を確認する。
- 復旧対応と並行して、認証情報の変更や不審なアクセスの有無など、関連システム全体の点検を進める。
- 顧客・取引先への案内が必要な場合に備え、事実関係が確定した範囲で説明できるよう情報整理を行う。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [サーバにランサム攻撃、顧客情報流出の可能性 - 名鉄協商](https://www.security-next.com/187989) | <nobr>内容確認・補足情報</nobr> |

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
| [Root Evidenceが実世界の証拠を脆弱性優先順位付けの中心に据える](https://www.helpnetsecurity.com/2026/07/29/root-evidence-puts-real-world-evidence-at-the-center-of-vulnerability-prioritization/) | 28.0 | 30.0 | 42.0 |
| [Tenguボットネット、削除を免れるためLinuxデバイスを再起動](https://www.helpnetsecurity.com/2026/07/29/tengu-mirai-iot-botnet-linux/) | 28.0 | 20.0 | 42.0 |
| [9年間にわたる詐欺キャンペーン、ロシア企業サイトを複製して前払い金を詐取](https://thehackernews.com/2026/07/nine-year-fraud-campaign.html) | 28.0 | 20.0 | 42.0 |
| [TrendAI™が2026年上半期の国家支援型APT活動を報告](https://newsroom.trendmicro.com/2026-07-29-TrendAI-TM-Reports-Nation-State-Activity-in-H1-2026-APT-Activity-Roundup) | 28.0 | 20.0 | 42.0 |
| [Microsoft Teams を狙う新たなビッシングキャンペーンについて知っておくべきこと](https://www.itpro.com/security/phishing/a-new-vishing-campaign-is-targeting-microsoft-teams-heres-what-users-need-to-know) | 28.0 | 20.0 | 42.0 |
| [盗まれたMetaとGoogleの広告アカウントは、口座残高以上の価値がある](https://www.helpnetsecurity.com/2026/07/29/ad-account-theft-meta-google/) | 28.0 | 20.0 | 42.0 |
| [WhatsAppがWeb版にエンドツーエンド暗号化の音声通話とビデオ通話を導入](https://www.helpnetsecurity.com/2026/07/29/whatsapp-voice-video-calls-web-support/) | 28.0 | 20.0 | 42.0 |
| [AIが書き換えるゼロデイ対策の新戦略と先制的セキュリティ](https://www.rapid7.com/blog/post/ai-rewriting-zero-day-playbook-for-preemptive-security) | 27.0 | 20.0 | 43.0 |
| [AIが発見した脆弱性のうち実際に悪用されたのはわずか1%だった、調査で判明](https://www.infosecurity-magazine.com/news/one-percent-ai-vulnerabilities/) | 27.0 | 20.0 | 43.0 |
| [OpenAIとHugging Faceのハックで悪用されたJFrogのゼロデイ脆弱性](https://www.securityweek.com/jfrog-zero-days-exploited-in-openai-hugging-face-hack/) | 27.0 | 20.0 | 43.0 |
| [パナソニック コネクト、AI活用で年間78.8万の労働時間を削減--2030年に総労働時間10％削減へ](https://japan.zdnet.com/article/35251079/) | 26.0 | 20.0 | 42.0 |
| [CVE-2026-63077: JetBrains TeamCityの重要な認証不要リモートコード実行脆弱性](https://www.rapid7.com/blog/post/etr-cve-2026-63077-critical-unauthenticated-remote-code-execution-in-jetbrains-teamcity) | 25.0 | 46.0 | 58.0 |
| [AIエージェントが暴走したときの責任は誰にあるのか？Hugging Faceの侵害が突きつける難題](https://www.darkreading.com/cyberattacks-data-breaches/liable-ai-agents-escape-hugging-face-breach-questions) | 25.0 | 20.0 | 42.0 |
| [Hugging Face侵害から学ぶサイバー防御の教訓](https://www.darkreading.com/cyberattacks-data-breaches/hugging-face-hack-lessons-cyber-defenders) | 25.0 | 20.0 | 42.0 |
| [OpenAI、Hugging Face侵害の不正エージェントが追加サービスにも侵入したと発表](https://therecord.media/openai-says-rogue-agent-behind-hugging-face-hack-broke-into-additional-services) | 25.0 | 20.0 | 42.0 |
| [WordワームがCopilotに侵入し混乱を拡大](https://www.theregister.com/security/2026/07/29/word-worm-crawls-into-copilot-spreads-chaos/5280588) | 25.0 | 20.0 | 42.0 |
| [OpenAI agentがHugging Face侵害で露出した4つのサービスの認証情報を使用](https://www.bleepingcomputer.com/news/security/openai-agent-used-exposed-credentials-at-4-services-in-hugging-face-breach/) | 25.0 | 20.0 | 42.0 |
| [Cisco、2026年8月5日公開予定のセキュリティアドバイザリ事前通知](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-notice-L4XfJg8S) | 25.0 | 20.0 | 42.0 |
| [Ruflo MCPの脆弱性により未認証の攻撃者がコマンド実行とAIメモリ汚染を可能にする](https://thehackernews.com/2026/07/ruflo-mcp-flaw-lets-unauthenticated.html) | 25.0 | 20.0 | 42.0 |
| [AI音声自動通話：発信者番号はなぜまだ偽装されるのか](https://www.malwarebytes.com/blog/news/2026/07/ai-robocalls-why-caller-id-is-still-lying-to-you) | 25.0 | 20.0 | 42.0 |
| [Patchで修正困難な「RufRoot」脆弱性により悪意あるAIエージェント群が解き放たれる](https://www.darkreading.com/cyber-risk/patch-resistant-rufroot-flaw-malicious-ai-agent-swarms) | 25.0 | 20.0 | 42.0 |
| [OpenAIがAIエージェントによるHugging Face侵入の経緯を説明](https://www.malwarebytes.com/blog/news/2026/07/openai-explains-how-its-ai-agent-breached-hugging-face) | 25.0 | 20.0 | 42.0 |
| [データ侵害のコスト増大に伴い、管理されないAIが新たなリスクを生む](https://www.cybersecuritydive.com/news/data-breach-costs-ai-governance-ibm/826463/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントの推測が大規模化する中で、被害を左右するのは権限設定です](https://www.bleepingcomputer.com/news/security/your-ai-agents-are-guessing-at-scale-permissions-decide-the-damage/) | 25.0 | 20.0 | 42.0 |
| [Wiz Red Agentが一般提供開始](https://www.wiz.io/blog/wiz-red-agent-is-ga) | 25.0 | 20.0 | 42.0 |
| [Mythosは適切な問いを投げかけるが、答えは示さない](https://thehackernews.com/2026/07/mythos-asks-right-question-it-doesnt.html) | 25.0 | 20.0 | 42.0 |
| [MIND AI DLP AgentsによるDLP分類、調査、修復の自動化](https://www.helpnetsecurity.com/2026/07/29/mind-ai-dlp-agents/) | 25.0 | 20.0 | 42.0 |
| [Contrast CVE Shield、セキュリティチームがパッチを適用する間にアプリケーションを保護することを目指す](https://www.helpnetsecurity.com/2026/07/29/contrast-security-cve-shield/) | 25.0 | 20.0 | 42.0 |
| [OpenAIの不正AIがHugging Faceを超えて暴走](https://www.securityweek.com/openais-rogue-ai-ventured-beyond-hugging-face/) | 25.0 | 20.0 | 42.0 |
| [OpenAIの暴走AIエージェントが示す、自治型システムに連邦規制が必要な理由](https://cyberscoop.com/openai-rogue-agent-federal-rules-autonomous-ai/) | 25.0 | 20.0 | 42.0 |
| [AI強化型の電話詐欺エコシステムに関する研究者の警告](https://www.infosecurity-magazine.com/news/researchers-aienhanced-phone-fraud/) | 25.0 | 20.0 | 42.0 |
| [AccurisがAIを活用してBOM判断とサプライチェーンのレジリエンスを向上](https://www.helpnetsecurity.com/2026/07/29/accuris-bom-intelligence/) | 25.0 | 20.0 | 42.0 |
| [Railsの重大な脆弱性により、未認証の攻撃者が画像アップロード経由でサーバー上のファイルを読み取れる可能性](https://thehackernews.com/2026/07/critical-rails-flaw-could-let.html) | 24.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Management Center Softwareの静的認証情報脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-fmc-static-cred-BET3Cjh) | 24.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Management Center Softwareの認証バイパス脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-onprem-fmc-authbypass-5JPp45V2) | 24.0 | 46.0 | 50.0 |
| [認証バイパス、コード実行、VM脱出を可能にする3件の重大なVMware脆弱性](https://thehackernews.com/2026/07/three-critical-vmware-flaws-allow-auth.html) | 24.0 | 46.0 | 50.0 |
| [より良いセキュリティは、より良い問いから始まる](https://www.microsoft.com/en-us/security/blog/2026/07/29/better-security-starts-with-better-questions/) | 22.0 | 20.0 | 42.0 |
| [顧客情報含む伝票など誤廃棄 - 東京三協信金](https://www.security-next.com/187814) | 22.0 | 20.0 | 42.0 |
| [通販サイトにサイバー攻撃、調査を実施 - ヴェレダ・ジャパン](https://www.security-next.com/187944) | 22.0 | 20.0 | 42.0 |
| [「VMware ESX」「VMware vCenter」に深刻な脆弱性 - 修正版が公開](https://www.security-next.com/188019) | 22.0 | 20.0 | 42.0 |
| [GrapheneOSの緊急コードでデータを抹消し警察を困らせたユーザーのインタビューが公開される](https://gigazine.net/news/20260729-interview-grapheneos-data-reset-man/) | 22.0 | 20.0 | 42.0 |
| [「macOS Tahoe 26.6」を公開 - 脆弱性155件を修正](https://www.security-next.com/188015) | 22.0 | 20.0 | 42.0 |
| [警察庁、熊本地震に便乗した詐欺に注意喚起 義援金名目で電子マネーなどだまし取る手口](https://www.itmedia.co.jp/news/article/2607/29/2000000280/) | 21.0 | 20.0 | 42.0 |
| [企業資産の36%が「脆弱性ゾーン」に、EYが指摘するフロンティアAI時代のサイバーリスク](https://news.mynavi.jp/techplus/article/20260729-4753934/) | 21.0 | 20.0 | 42.0 |
| [Health-ISACが警告する医療機関を狙うShinyHuntersによるデータ窃取攻撃の増加](https://www.bleepingcomputer.com/news/security/health-isac-warns-of-rising-shinyhunters-data-theft-attacks-on-healthcare/) | 20.0 | 20.0 | 42.0 |
| [AppSecスキャナーがサプライチェーン攻撃の経路になるとき](https://www.darkreading.com/application-security/when-appsec-scanners-become-supply-chain-attack-vector) | 20.0 | 20.0 | 42.0 |
| [TikTokの再生回数やフォロワーを購入すると本当に何が手に入るのか](https://www.malwarebytes.com/blog/threat-intel/2026/07/buying-tiktok-views-or-followers-heres-what-youre-really-getting) | 20.0 | 20.0 | 42.0 |
| [Huntressが警告、2日間で30社のSonicWall顧客を襲った攻撃の連続発生](https://cyberscoop.com/sonicwall-credential-attacks-vpn-firewall/) | 20.0 | 20.0 | 42.0 |
| [LogoKitフィッシングキットが被害者サイトをリアルタイムでスクリーンショット取得](https://www.infosecurity-magazine.com/news/logokit-phishing-real-time/) | 20.0 | 20.0 | 42.0 |
| [Dependabotをうまく制御する：更新をグループ化し、頻度を抑えつつセキュリティ対応は迅速に保つ](https://github.blog/security/supply-chain-security/tame-dependabot-group-your-updates-slow-the-cadence-keep-security-fast/) | 20.0 | 20.0 | 42.0 |
| [ロシア系とされるTA488が再びOutlook Web Accessを狙った継続的攻撃を実施](https://www.infosecurity-magazine.com/news/ta488-outlook-half-click-owareaper/) | 20.0 | 20.0 | 42.0 |
| [ハッカーが協調的なOT攻撃でミネソタ州の水道事業者30以上を妨害](https://www.bleepingcomputer.com/news/security/hackers-target-over-30-minnesota-water-utilities-in-coordinated-ot-attack/) | 20.0 | 20.0 | 42.0 |
| [Laundry BearのWebメール侵入者は2月以降も追加の攻撃を準備していたと報告書が示す](https://therecord.media/russia-hackers-outlook-webmail-malware) | 20.0 | 20.0 | 42.0 |
| [WizのGoogle傘下入り後6カ月の歩み](https://www.wiz.io/blog/6-months-google) | 20.0 | 20.0 | 42.0 |
| [Iran関連のCyberAv3ngersによるミネソタ州の水道システムへの攻撃が疑われる件](https://www.theregister.com/security/2026/07/29/iran-linked-cyberav3ngers-suspected-in-attacks-on-minnesota-water-systems/5280357) | 20.0 | 20.0 | 42.0 |
| [30以上のミネソタ州水道システムを標的とした協調サイバー攻撃、1つの施設が停止](https://thehackernews.com/2026/07/coordinated-cyberattack-targets-30.html) | 20.0 | 20.0 | 42.0 |
| [米国、国家安全保障を理由に中国製のヒューマノイドロボットを禁止](https://www.securityweek.com/us-bans-foreign-made-humanoid-robots-targeting-china-over-national-security/) | 20.0 | 20.0 | 42.0 |
| [ShutterGap：Aryon Securityが3.7百万のAWSクラウドリソースがCSPM/CNAPPの可視範囲外に露出していると発見](https://www.helpnetsecurity.com/2026/07/29/cspm-blind-spot-report/) | 20.0 | 20.0 | 42.0 |
| [Mate Security、Agentic SOC向けに3500万ドルを調達](https://www.securityweek.com/mate-security-raises-35-million-for-agentic-soc/) | 20.0 | 20.0 | 42.0 |
| [ThreatLocker、シリーズFで1億9000万ドルを調達](https://www.securityweek.com/threatlocker-raises-190-million-in-series-f-funding/) | 20.0 | 20.0 | 42.0 |
| [Angola最大の通信事業者が歴史的な株式上場直前にサイバー攻撃を受ける](https://therecord.media/angola-unitel-cyberattack-outage) | 20.0 | 20.0 | 42.0 |
| [CISAとパートナーが公開した、透明性・セキュリティ・リスクに基づく意思決定を向上させる更新版ソフトウェア部品表（SBOM）リソース](https://www.cisa.gov/news-events/news/cisa-and-partners-unveil-updated-software-bill-materials-resource-improves-transparency-security-and) | 20.0 | 20.0 | 42.0 |
| [2026年版 ソフトウェア部品表（SBOM）の最小要件](https://www.cisa.gov/resources-tools/resources/2026-minimum-elements-software-bill-materials-sbom) | 20.0 | 20.0 | 42.0 |
| [研究者が、悪意あるWebページを1回閲覧するだけでTor Browserを侵害できることを実証](https://thehackernews.com/2026/07/researchers-show-single-malicious.html) | 20.0 | 20.0 | 42.0 |
| [VMware ESXiで修正された重大なVMエスケープ脆弱性](https://www.securityweek.com/critical-vm-escape-vulnerability-patched-in-vmware-esxi/) | 20.0 | 20.0 | 42.0 |
| [73%の組織が大規模サイバー攻撃への完全な備えができていないと回答](https://thehackernews.com/2026/07/73-of-organizations-say-they-are-not.html) | 20.0 | 20.0 | 42.0 |
| [ほぼ新品のASUS Chromebook再生品が145ドルで購入可能](https://www.bleepingcomputer.com/news/security/these-near-mint-asus-chromebook-refurbs-are-only-145/) | 20.0 | 20.0 | 42.0 |
| [ZscalerとSchwarz Digits、ソブリンクラウドセキュリティプラットフォームで提携](https://www.itpro.com/security/zscaler-and-schwarz-digits-team-up-on-sovereign-cloud-security-platform) | 20.0 | 20.0 | 42.0 |
| [Telegram創業者Pavel Durovをテロ活動幇助でロシアが起訴](https://thehackernews.com/2026/07/russia-charges-telegram-founder-pavel.html) | 20.0 | 20.0 | 42.0 |
| [データ侵害の平均コストが500万ドルに上昇](https://www.infosecurity-magazine.com/news/cost-of-a-data-breach-5m-ibm/) | 20.0 | 20.0 | 42.0 |
| [米国とオーストラリア、重要インフラ向けOT分離ガイダンスを公開](https://www.securityweek.com/us-australia-release-ot-isolation-guidance-for-critical-infrastructure/) | 20.0 | 20.0 | 42.0 |
| [Walmartを装った偽店舗120件がクレジットカード情報を盗もうとしていたことを確認](https://www.malwarebytes.com/blog/scams/2026/07/we-found-120-fake-walmart-stores-trying-to-steal-your-credit-card) | 20.0 | 20.0 | 42.0 |
| [Cloudflareが明かす大規模インターネット障害の原因](https://www.helpnetsecurity.com/2026/07/29/cloudflare-q2-2026-internet-outages/) | 20.0 | 20.0 | 42.0 |
| [米国CFOの戦略：厳しい労働市場でSOCチームを拡大せずにサイバーリスクを低減する方法](https://any.run/cybersecurity-blog/cfo-cyber-risk-playbook/) | 20.0 | 20.0 | 42.0 |
| [SpurがIPインテリジェンスプラットフォーム向けに2億ドルを調達](https://www.securityweek.com/spur-raises-200-million-for-ip-intelligence-platform/) | 20.0 | 20.0 | 42.0 |
| [FortiGate 1200GがFortiSASE Outpostを顧客管理環境に導入](https://www.helpnetsecurity.com/2026/07/29/fortinet-fortigate-1200g/) | 20.0 | 20.0 | 42.0 |
| [NCSCがインシデント対応と復旧を支援するガイダンスを公開](https://www.infosecurity-magazine.com/news/ncsc-publishes-guidance-incident/) | 20.0 | 20.0 | 42.0 |
| [1Password、常時特権への対応を強化する新しいアクセス管理機能を発表](https://www.helpnetsecurity.com/2026/07/29/1password-privileged-access/) | 20.0 | 20.0 | 42.0 |

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
