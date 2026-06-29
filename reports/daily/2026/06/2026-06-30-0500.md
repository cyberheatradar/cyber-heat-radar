# 📡 サイレーダー 2026-06-30 05:00 JST

このレポートは、2026-06-29 17:00 JST〜2026-06-30 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 84
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 53

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Modernizing Global Vulnerability Standards For The Age Of AI](#topic-19940) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [29th June – Threat Intelligence Report](#topic-15753) | 43.0 | 58.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [JSP webshells being dropped on unpatched PTC Windchill instances](#topic-19909) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [US Federal Insurance Regulator Confirms Data Breach Via Oracle Flaw](#topic-19967) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [⚡ Weekly Recap: Linux Kernel Flaws, AI Malware Tricks, Turla Backdoor, Infostealers and More](#topic-19921) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 6 | [The Bear Necessities: A Look at the Drivers, Dynamics, and Applications of the Pro-Russia Influence Ecosystem](#topic-19927) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-19940"></a>

### 1. Modernizing Global Vulnerability Standards For The Age Of AI

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

AIによる脆弱性発見が高速化するなかで、既存のCVEやCVSS、NVD、KEV、EPSSといった脆弱性管理の仕組みが追いつかなくなりつつある、という問題提起です。
特に、単体の深刻度よりも「実際に到達可能か」「複数の脆弱性をつなげて悪用できるか」といった観点での優先順位付けが重要だとされています。
脆弱性の件数や発見速度がAIで大きく伸びると、守る側は評価・トリアージ・修正の負荷に直面します。
従来の指標だけでは実リスクを見誤るおそれがあるため、運用や調達、政策面を含めた見直しが注目されています。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- CVSSなどの数値だけでなく、自組織で到達可能か、既知の悪用や連鎖リスクがあるかを合わせて確認する。
- NVDやKEV、EPSSの更新遅延や限界を前提に、社内の優先順位付け基準を見直す。
- AIで見つかった脆弱性については、検証済みかどうか、再現性や影響範囲の情報が十分かを慎重に扱う。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Modernizing Global Vulnerability Standards For The Age Of AI](https://www.rapid7.com/blog/post/ai-modernizing-global-vulnerability-standards) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-15753"></a>

### 2. 29th June – Threat Intelligence Report

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Catalyst SD-WAN Managerに関する権限昇格の脆弱性CVE-2026-20245が、ゼロデイとして悪用された可能性が複数の情報源で報告されています。
Ciscoはこの脆弱性について、影響を受ける環境で有効な認証情報が必要とし、限定的な悪用事例を把握しているとしています。
ネットワーク機器の管理系コンポーネントが標的になると、侵害後の権限拡大や不正な管理操作につながるおそれがあります。
パッチ提供前の悪用観測があるため、該当環境では早急な状況確認が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- PoC/検証コード候補: 候補あり（該当CVE 3件 / URL 7件以上）。
- 直接PoCリンク: 掲載しません。
- 注意: 対象CVE・製品・バージョンとの一致確認が必要です。

#### 担当者向け確認ポイント

- CVE-2026-20245の影響範囲にCisco Catalyst SD-WAN Manager関連製品が含まれるか確認する。
- 管理者アカウントや認証情報の利用状況を見直し、不審なログインや権限変更の痕跡を確認する。
- Ciscoの公式勧告と更新情報を継続監視し、適用可能な緩和策や修正版が出たら速やかに対応する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20127 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20182 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20245 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-33017 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-34908 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-34909 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-34910 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-41947 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-41948 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-55255 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20245](https://nvd.nist.gov/vuln/detail/CVE-2026-20245) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [29th June – Threat Intelligence Report](https://research.checkpoint.com/2026/29th-june-threat-intelligence-report-2/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco SD-WAN Zero-Day Exploited Months Before Patching](https://www.securityweek.com/cisco-sd-wan-zero-day-exploited-months-before-patching/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Zero-Day CVE-2026-20245 Exploited to Gain Root Access](https://thehackernews.com/2026/06/cisco-catalyst-sd-wan-zero-day-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Mandiant reveals how Cisco SD-WAN zero-day attacks gained root access](https://www.bleepingcomputer.com/news/security/mandiant-reveals-how-cisco-sd-wan-zero-day-attacks-gained-root-access/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zero-Day Exploitation of Vulnerability (CVE-2026-20245) in Cisco Catalyst SD-WAN](https://cloud.google.com/blog/topics/threat-intelligence/zero-day-exploitation-cisco-catalyst-sd-wan-manager/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN V](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-privesc-4uxFrdzx) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco customers encounter another SD-WAN zero-day under attack](https://cyberscoop.com/cisco-sdwan-zero-day-vulnerability-exploited-cve202620245/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-19909"></a>

### 3. JSP webshells being dropped on unpatched PTC Windchill instances

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、PTCのWindchillおよびFlexPLMに関する脆弱性をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
PTCの注意喚起では、影響を受ける環境に対してJSP webshellが配置されていることを示す情報が更新されており、実際の悪用が疑われる状況です。
PLMソフトウェアは製品情報や設計情報を扱うことが多く、侵害されると業務影響が大きくなり得ます。
KEV入りしているため、単なる理論上の脆弱性ではなく、優先度を上げて対応すべき案件と見られます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Windchill / FlexPLMの該当バージョンを確認し、ベンダー修正の適用状況を点検する。
- PTCが公開している侵害指標や防御向け注意喚起を参照し、対象環境で整合する痕跡がないか確認する。
- 外部公開された管理画面や関連サービスの露出を見直し、暫定的にアクセス制限を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-12569 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [JSP webshells being dropped on unpatched PTC Windchill instances](https://www.helpnetsecurity.com/2026/06/29/ptc-windchill-cve-2026-12569-exploited/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-19967"></a>

### 4. US Federal Insurance Regulator Confirms Data Breach Via Oracle Flaw

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

米国の保険関連の標準設定団体NAICが、Oracle PeopleSoftの脆弱性を悪用された可能性のある侵害を確認したと報じられています。
現時点では、ゼロデイの悪用により同団体のITシステムへ不正アクセスがあったとされますが、被害の全容や影響範囲は限定的にしか分かっていません。
保険業界の中核に近い組織が影響を受けた可能性があり、同種の業務システムを使う組織にとっても関連性があります。
ゼロデイの悪用が示唆されるため、修正状況の確認や周辺システムの点検が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Oracle PeopleSoftの適用状況と関連ベンダー情報を確認し、保護策や修正の有無を点検する。
- 認証ログ、管理操作ログ、外部からの不審なアクセス痕跡を優先的に確認する。
- 影響が想定される場合は、関連アカウントの見直しと、機微情報へのアクセス制御を強化する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [US Federal Insurance Regulator Confirms Data Breach Via Oracle Flaw](https://www.infosecurity-magazine.com/news/us-insurance-regulator-confirms/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-19921"></a>

### 5. ⚡ Weekly Recap: Linux Kernel Flaws, AI Malware Tricks, Turla Backdoor, Infostealers and More

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

今週の脅威動向のまとめでは、Linuxカーネルの脆弱性、AIを悪用したマルウェアの手口、Turlaのバックドア、情報窃取型マルウェアなど複数の話題が取り上げられています。
個別の詳細はまだ整理途上でも、既知の脆弱性対応や初期侵入後の活動への備えが改めて重要だと示しています。
AI関連の話題だけでなく、従来型の脆弱性やマルウェアが並行して注目されており、守る側は複数の攻撃面を同時に見る必要があります。
特定の単発事案ではなく、運用上の見落としやパッチ遅延が被害につながりやすい点が注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Linux環境では、該当する脆弱性情報と保守適用状況を早めに確認する。
- AIを使った不審な文面・挙動があっても、従来の検知基盤やログ監視と突き合わせて判断する。
- 情報窃取型マルウェアやバックドアを想定し、認証情報の保護、権限の最小化、端末の異常通信監視を見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [⚡ Weekly Recap: Linux Kernel Flaws, AI Malware Tricks, Turla Backdoor, Infosteal](https://thehackernews.com/2026/06/weekly-recap-linux-kernel-flaws-ai.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-19927"></a>

### 6. The Bear Necessities: A Look at the Drivers, Dynamics, and Applications of the Pro-Russia Influence Ecosystem

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>A⁠I</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>サ⁠ー⁠ド⁠パ⁠ー⁠テ⁠ィ⁠リ⁠ス⁠ク</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、ロシア寄りの情報工作エコシステムは、ウクライナ戦争向けの動きから、より広い対外・国内向けの影響工作へ再び軸足を戻しつつあるとみられます。
記事は、生成AIの活用、ハクティビズム、偽装メディア、漏えい情報の拡散など、複数の手口が相互に結びついている点を指摘しています。
影響工作は単独のキャンペーンではなく、政府系・準政府系・第三者の活動が重なって拡張性と持続性を持つため、発見や切り分けが難しくなります。
選挙、国際イベント、地域紛争などに合わせて話題が切り替わる可能性があり、広報・脅威対応・レピュテーション管理の両面で注意が必要です。

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

- 生成AIを使った偽情報生成や下書き作成が増える前提で、社内外の情報の真偽確認プロセスを強化する。
- 選挙・国際情勢・大規模イベントに便乗した偽装メディアや漏えい主張に備え、一次情報と公式発表の確認導線を明確にする。
- DDoSや改ざん、情報漏えいを装う影響工作が同時に起きうるため、広報、SOC、法務の連携体制を事前に整える。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [The Bear Necessities: A Look at the Drivers, Dynamics, and Applications of the P](https://cloud.google.com/blog/topics/threat-intelligence/pro-russia-influence-ecosystem/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
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
| [VPN経由でサイバー攻撃、ランサム被害が発生 - D&M](https://www.security-next.com/186393) | 30.0 | 30.0 | 42.0 |
| [Mozillaが警告するAIコーディングエージェントにおける間接的プロンプトインジェクションのリスク](https://www.helpnetsecurity.com/2026/06/29/mozilla-warns-of-indirect-prompt-injection-risk-in-ai-coding-agents/) | 29.0 | 20.0 | 43.0 |
| [「Gentlemen」と名乗る攻撃者によるカスタムバックドアと進化する戦術](https://securelist.com/the-gentlemen-raas/120447/) | 28.0 | 30.0 | 42.0 |
| [Russian HackersによるJaguar Land Roverへの破壊的サイバー攻撃疑惑](https://www.infosecurity-magazine.com/news/russian-hackers-destructive-jaguar/) | 28.0 | 30.0 | 42.0 |
| [イラン、ロシア、中国が水道システムを妨害対象に](https://www.darkreading.com/ics-ot-security/iran-russia-china-target-water-systems-sabotage) | 28.0 | 20.0 | 42.0 |
| [Mistic：アクセスブローカー向けツールの進化を示す新たなマルウェア](https://blog.polyswarm.io/mistic-new-malware-may-signal-evolution-in-access-broker-tooling) | 28.0 | 20.0 | 42.0 |
| [米国、SignalやWhatsAppを標的としたロシアのサイバー攻撃キャンペーンに1,000万ドルの報奨金を提示](https://therecord.media/10million-reward-us-russian-hackers-unc4221-unc5792) | 28.0 | 20.0 | 42.0 |
| [Mustang Panda、インド政府機関への攻撃でZoho WorkDriveをコマンドチャネルに悪用](https://thehackernews.com/2026/06/mustang-panda-uses-zoho-workdrive-as.html) | 28.0 | 20.0 | 42.0 |
| [119個のEdge拡張機能が便利なツールを装い、実際にはマルウェアをダウンロードしていた](https://www.malwarebytes.com/blog/news/2026/06/119-edge-extensions-promised-useful-tools-instead-downloaded-malware) | 28.0 | 20.0 | 42.0 |
| [Telegramを利用したMillenium RATキャンペーンで6万台のデバイスが感染](https://www.infosecurity-magazine.com/news/millenium-rat-telegram-60000/) | 28.0 | 20.0 | 42.0 |
| [なぜ耐量子暗号は認証情報から始まるのか](https://thehackernews.com/2026/06/why-post-quantum-cryptography-starts.html) | 28.0 | 20.0 | 42.0 |
| [Gamaredon、Ukraineへの攻撃を新たなマルウェアとクラウドサービス悪用で拡大](https://thehackernews.com/2026/06/gamaredon-expands-ukraine-attacks-with.html) | 28.0 | 20.0 | 42.0 |
| [Microsoft、画像やフォントにマルウェアを隠した119件のEdge拡張機能を削除](https://thehackernews.com/2026/06/microsoft-removes-119-edge-extensions.html) | 28.0 | 20.0 | 42.0 |
| [神話から現実へ：2026年のペネトレーションテスト実態レポートが示すプログラム的防御の必要性](https://www.cybersecuritydive.com/spons/from-mythos-to-reality-why-the-2026-state-of-pentesting-report-proves-the/823726/) | 27.0 | 20.0 | 43.0 |
| [Chromium拡張機能がAI関連のブランディングを使ってブラウザ検索をリダイレクト](https://www.microsoft.com/en-us/security/blog/2026/06/29/chromium-extension-uses-airelated-branding-redirect-browser-search/) | 27.0 | 20.0 | 42.0 |
| [リコーとライズ・コンサルティング・グループが新会社、AI活用を伴走支援](https://xtech.nikkei.com/atcl/nxt/news/24/03278/) | 26.0 | 20.0 | 42.0 |
| [見た目は無害なリポジトリを悪用して開発者端末を乗っ取る新たなClaude Code攻撃を研究者が実証](https://www.securityweek.com/new-attack-abuses-claude-code-and-harmless-looking-repositories-to-hijack-developer-machines/) | 25.0 | 45.0 | 42.0 |
| [WordPressプラグイン・テーマの脆弱性最新情報 第31回 WordPress脆弱性16件、UpdraftPlus PremiumのRCEに注意【6月11日～6月17日】](https://news.mynavi.jp/techplus/article/wordpressvulnerability-31/) | 25.0 | 38.0 | 42.0 |
| [Claude Fable 5とAI活用型サードパーティリスクの新たな現実](https://www.bitsight.com/de/blog/claude-fable-5-und-die-neue-realitaet-von-ki-gestuetztem-drittparteirisiko) | 25.0 | 20.0 | 42.0 |
| [OpenAI、GPT-5.6 Solサイバーセキュリティモデルを公開し、早期アクセスを制限](https://www.infosecurity-magazine.com/news/openai-gpt-5-6-sol-limited-preview/) | 25.0 | 20.0 | 42.0 |
| [OpenAIが政府の要請を受けて新AIモデルの提供を自主的に制限](https://www.cybersecuritydive.com/news/openai-model-government-limit-request/823966/) | 25.0 | 20.0 | 42.0 |
| [Straiker、AIセキュリティプラットフォーム向けに6400万ドルを調達](https://www.securityweek.com/straiker-raises-64-million-for-ai-security-platform/) | 25.0 | 20.0 | 42.0 |
| [Agentic AIはアイデンティティに問題を抱えており、攻撃者はそれを知っている](https://www.bleepingcomputer.com/news/security/agentic-ai-has-an-identity-problem-and-attackers-know-it/) | 25.0 | 20.0 | 42.0 |
| [AIは脆弱性の発見に優れるが、人間の愚かさには勝てない](https://www.theregister.com/security/2026/06/29/ai-may-be-good-at-finding-security-vulnerabilities-but-it-cant-beat-human-stupidity/5263262) | 25.0 | 20.0 | 42.0 |
| [PrivacyHawk EnterpriseでシャドーITを発見し、第三者リスクを最小化する方法](https://www.helpnetsecurity.com/2026/06/29/privacyhawk-enterprise/) | 25.0 | 20.0 | 42.0 |
| [OpenAIとAnthropic、新AIモデルをトランプ承認済み顧客に限定しサイバーセキュリティ審査を実施](https://www.securityweek.com/openai-and-anthropic-limit-new-ai-models-to-trump-approved-customers-during-cybersecurity-review/) | 25.0 | 20.0 | 42.0 |
| [メルアカに不正アクセス、個人情報流出の可能性 - オークション事業者](https://www.security-next.com/186446) | 22.0 | 20.0 | 42.0 |
| [CISOsに本当に求められるポスト量子時代の大統領令対応](https://cyberscoop.com/post-quantum-cryptography-readiness-ciso-deadlines-op-ed/) | 20.0 | 20.0 | 48.0 |
| [悪意のあるPerplexity Chrome拡張機能が検索内容とアドレスバー入力を盗み見](https://thehackernews.com/2026/06/malicious-perplexity-chrome-extension.html) | 20.0 | 20.0 | 42.0 |
| [WhatsApp、電話番号を隠せるユーザー名機能を導入](https://www.bleepingcomputer.com/news/security/whatsapp-rolls-out-usernames-to-help-users-hide-their-phone-number/) | 20.0 | 20.0 | 42.0 |
| [最高裁、選挙日後に到着する郵便投票を承認](https://cyberscoop.com/supreme-court-rules-legal-mail-in-ballots-after-election-day/) | 20.0 | 20.0 | 42.0 |
| [Chatrie判決でテック企業のプライバシーに大きな追い風、最高裁が判断](https://cyberscoop.com/supreme-court-geofence-warrant-ruling-phone-privacy-chatrie/) | 20.0 | 20.0 | 42.0 |
| [Advisoryデータベースの内部と、脆弱性件数が記録を更新すると何が起こるか](https://github.blog/security/supply-chain-security/inside-the-advisory-database-and-what-happens-when-vulnerability-volume-breaks-records/) | 20.0 | 20.0 | 42.0 |
| [WhatsApp、電話番号のプライバシー強化に向けてユーザー名機能を段階的に展開](https://www.securityweek.com/whatsapp-rolling-out-username-feature-to-bolster-phone-number-privacy/) | 20.0 | 20.0 | 42.0 |
| [保険業界団体がOracle PeopleSoft侵害データの投稿を確認](https://www.cybersecuritydive.com/news/insurance-body-hackers-oracle-peoplesoft-breach-data/823978/) | 20.0 | 20.0 | 42.0 |
| [米国、WhatsAppとSignalの利用者を標的にするハッカーに1000万ドルの報奨金を提供](https://www.bleepingcomputer.com/news/security/us-offers-10-million-for-hackers-targeting-whatsapp-signal-users/) | 20.0 | 20.0 | 42.0 |
| [この賃金格差はプログラムされている（Lock and Code S07E13）](https://www.malwarebytes.com/blog/podcast/2026/06/this-pay-gap-is-programmed-lock-and-code-s07e13) | 20.0 | 20.0 | 42.0 |
| [攻撃に悪用されるOracle E-Businessの重大な脆弱性](https://www.bleepingcomputer.com/news/security/new-oracle-e-business-suite-flaw-now-exploited-in-attacks/) | 20.0 | 20.0 | 42.0 |
| [NAICがOracle PeopleSoft侵害の標的に](https://www.securityweek.com/insurance-regulators-group-naic-hit-in-oracle-peoplesoft-hack/) | 20.0 | 20.0 | 42.0 |
| [ウクライナ、サイバー犯罪グループから押収した暗号資産で戦時国債を購入へ](https://therecord.media/ukraine-uses-seized-crypto-cybercrime-for-war-bonds) | 20.0 | 20.0 | 42.0 |
| [ハイブリッドクラウドチームのための統合セキュリティ運用モデルによる可視性ギャップの解消](https://www.wiz.io/blog/sensor-wls-for-on-prem) | 20.0 | 20.0 | 42.0 |
| [23万6000件のDCloud Uni-Appサイトが暗号資産詐欺、フィッシング、ウォレットドレイナーに悪用される](https://thehackernews.com/2026/06/236000-dcloud-uni-app-sites-used-in.html) | 20.0 | 20.0 | 42.0 |
| [Amazon Q VS拡張機能の欠陥によりクラウド認証情報が窃取される](https://www.darkreading.com/cloud-security/amazon-q-vs-extension-flaw-leads-cloud-credential-theft) | 20.0 | 20.0 | 42.0 |
| [Web PKIの透明性と保証の向上：Mozillaルートストアポリシーv3.1](https://blog.mozilla.org/security/2026/06/29/improving-transparency-and-assurance-in-the-web-pki-mozilla-root-store-policy-v3-1/) | 20.0 | 20.0 | 42.0 |
| [ハッキンググループが交通ネットワークを標的に ネットワーク・レールがサイバー脅威の猛攻と対峙](https://www.itpro.com/security/cyber-attacks/hacking-groups-have-the-transport-network-firmly-in-their-sights-network-rail-is-battling-a-torrent-of-cyber-threats) | 20.0 | 20.0 | 42.0 |
| [米国当局がFIFAワールドカップの違法配信ドメイン数百件を差し押さえ](https://www.bleepingcomputer.com/news/security/us-seizes-hundreds-of-fifa-world-cup-illegal-streaming-domains/) | 20.0 | 20.0 | 42.0 |
| [DirtyCloneによるLinuxカーネルの脆弱性がroot権限奪取につながる](https://www.securityweek.com/dirtyclone-linux-kernel-vulnerability-leads-to-root-access/) | 20.0 | 20.0 | 42.0 |
| [Nissan、Oracle PeopleSoftへの侵入で給与記録とSSNが流出した可能性を公表](https://www.theregister.com/security/2026/06/29/nissan-says-oracle-peoplesoft-break-in-may-have-spilled-payroll-records-ssns/5263534) | 20.0 | 20.0 | 42.0 |
| [境界のない攻撃対象領域：公共部門のハイブリッド環境を守る](https://www.wiz.io/blog/wiz-xm-securing-public-sector-hybrid-environments) | 20.0 | 20.0 | 42.0 |
| [Red Agentの視点：航空会社のGraphQL APIにおけるBroken Object-Level Authorizationの悪用](https://www.wiz.io/blog/red-agent-pov-bola) | 20.0 | 20.0 | 42.0 |
| [米国、ロシアの国家関与ハッカーに1000万ドルの報奨金を提示、メッセージングアプリ攻撃は進化](https://www.securityweek.com/us-offers-10-million-bounty-for-russian-state-hackers-as-messaging-app-attacks-evolve/) | 20.0 | 20.0 | 42.0 |
| [GPT-5.6のサイバーセキュリティ性能が向上](https://www.helpnetsecurity.com/2026/06/29/openai-gpt-5-6-models-preview/) | 20.0 | 20.0 | 42.0 |
| [FBIが警告、ロシア諜報機関によるスピアフィッシング攻撃](https://www.infosecurity-magazine.com/news/fbi-alarm-russian-intelligence/) | 20.0 | 20.0 | 42.0 |

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
