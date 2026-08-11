# 📡 サイレーダー 2026-08-12 05:00 JST

このレポートは、2026-08-11 17:00 JST〜2026-08-12 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 97
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 67

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Microsoft 2026年8月 Patch Tuesday 関連まとめ](#topic-26601) | 56.0 | 66.0 | 57.0 | 音声 | 温度感上位枠 |
| 2 | [CISA: Microsoft SharePoint flaw now exploited in ransomware attacks](#topic-27104) | 49.0 | 66.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Shattering the Dream – When a Job Offer Becomes a Zero-Day Attack](#topic-27063) | 45.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 4 | [Cisco Secure Firewall Management Center Software Static Credential Vulnerability](#topic-24943) | 37.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 5 | [Rapid7 Analysis: Microsoft SharePoint JWT Token Authentication Bypass (CVE-2026-55040)](#topic-27098) | 35.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-26601"></a>

### 1. Microsoft 2026年8月 Patch Tuesday 関連まとめ

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>A⁠I</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 56.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 66.0 |
| <nobr>確⁠度</nobr> | 57.0 |

#### 概要

Microsoftの2026年8月のPatch Tuesdayでは、400件超の脆弱性修正が案内され、ゼロデイとして扱われる事案も含まれていました。
公開情報では、少なくとも一部の脆弱性は実際の悪用が確認されているとされていますが、個別の影響範囲や深刻度は製品ごとに異なります。
広範なWindows関連製品や周辺コンポーネントに修正が入るため、組織全体の更新計画に影響します。
実悪用が報告されている脆弱性が含まれる可能性があるため、通常の月例更新より優先度を高めて確認されやすい話題です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象製品の更新適用状況を早急に確認し、未適用端末・サーバーを洗い出す。
- 公開済みの悪用情報やゼロデイ該当の有無を確認し、優先順位を見直す。
- 影響を受ける可能性がある重要システムは、適用前後の動作確認とロールバック手順を準備する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-50522 | 関連CVE | 1.00 | 候補あり（URL 5件以上） |
| 製品 | Microsoft Windows | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [August 2026 Patch Tuesday: Microsoft Fixes 421 CVEs, One Exploited Zero-Day](https://www.securityweek.com/august-2026-patch-tuesday-microsoft-fixes-421-cves-one-exploited-zero-day/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft August 2026 Patch Tuesday fixes 400 flaws, 3 zero-days](https://www.bleepingcomputer.com/news/microsoft/microsoft-august-2026-patch-tuesday-fixes-400-flaws-3-zero-days/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [The August 2026 Security Update Review](https://www.thezdi.com/blog/2026/8/11/the-august-2026-security-update-review) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patch Tuesday August 2026, (Tue, Aug 11th)](https://isc.sans.edu/diary/rss/33236) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-27104"></a>

### 2. CISA: Microsoft SharePoint flaw now exploited in ransomware attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 49.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 66.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、Microsoft SharePointの高深刻度なリモートコード実行脆弱性が、ランサムウェア攻撃で悪用され始めていると確認しました。
この脆弱性は早い段階から実際の悪用が疑われており、攻撃対象としてのリスクが高い状況です。
業務利用の多いSharePointに関わるため、単一の脆弱性でも広い範囲に影響が及ぶ可能性があります。
ランサムウェア文脈での悪用が確認されている点から、侵入後の被害拡大や業務停止につながるおそれがあります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Microsoftの案内やCISA情報を確認し、該当バージョンの修正適用状況を点検する。
- SharePoint関連の公開範囲、不要な外部公開、認証やアクセス制御の設定を見直す。
- 関連ログを確認し、不審な実行や不自然なアクセスの有無を早めに点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-45659 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA: Microsoft SharePoint flaw now exploited in ransomware attacks](https://www.bleepingcomputer.com/news/security/cisa-microsoft-sharepoint-flaw-now-exploited-in-ransomware-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-27063"></a>

### 3. Shattering the Dream – When a Job Offer Becomes a Zero-Day Attack

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

Check Point Researchは、2026年初頭以降に観測した「Operation Dream Job」キャンペーンの新しい波について報告しました。
報告では、防衛分野、特に航空宇宙・航空関連企業が主な標的となり、CVE-2026-68820に関連するゼロデイ文脈の悪用が示されています。
防衛・航空宇宙のような機微な分野が狙われている点から、情報窃取や侵入の影響が大きくなりやすい事案です。
ゼロデイ文脈での悪用が示されているため、パッチ可用性だけに頼れず、検知と封じ込めの準備が重要になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- CVE-2026-68820に関連する製品・利用状況を確認し、影響範囲を把握する。
- 不審なPDFや外部共有ファイルの取り扱いを見直し、隔離環境での開封や検査を徹底する。
- 標的型攻撃を想定して、EDR/メール/プロキシの検知ルールとインシデント対応手順を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-49113 | 関連CVE | 1.00 | 候補あり（URL 27件以上） |
| 脆弱性 | CVE-2026-68820 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-68820](https://nvd.nist.gov/vuln/detail/CVE-2026-68820) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Shattering the Dream – When a Job Offer Becomes a Zero-Day Attack](https://research.checkpoint.com/2026/shattering-the-dream-when-a-job-offer-becomes-a-zero-day-attack/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-24943"></a>

### 4. Cisco Secure Firewall Management Center Software Static Credential Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Cisco Secure Firewall Management Center（FMC）SoftwareのWebインターフェースに、低権限アカウントの静的認証情報が含まれる脆弱性（CVE-2026-20316）が報告されています。
Ciscoによると、未認証のリモート攻撃者が影響を受ける機器にログインし、機微情報へアクセスできる可能性があります。
管理用製品の認証まわりの不備は、侵入後の情報閲覧や他の脆弱性と組み合わさった権限拡大につながるおそれがあります。
Ciscoは更新プログラムを公開しており、対処の優先度が高い事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- FMC管理インターフェースが外部公開されていないか確認し、公開範囲を最小化する。
- Ciscoが提供する修正済みソフトウェアへ速やかに更新する。
- FMCへの不審なログインや設定変更の有無を点検し、関連ログを確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20316 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20316](https://nvd.nist.gov/vuln/detail/CVE-2026-20316) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Firewall Management Center Software Static Credential Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-fmc-static-cred-BET3Cjh) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco FMC static credentials exploited by attackers (CVE-2026-20316)](https://www.helpnetsecurity.com/2026/07/30/cisco-fmc-cve-2026-20316-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure FMC Zero-Day Exploited in the Wild](https://www.securityweek.com/cisco-secure-fmc-zero-day-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of FMC static credential flaw exploited in zero-day attacks](https://www.bleepingcomputer.com/news/security/cisco-warns-of-fmc-static-credential-flaw-exploited-in-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-27098"></a>

### 5. Rapid7 Analysis: Microsoft SharePoint JWT Token Authentication Bypass (CVE-2026-55040)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>Exploit Kit</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Rapid7は、Microsoft SharePointの認証回避脆弱性「CVE-2026-55040」について技術分析を公開しました。
説明では、JWTトークンの検証処理に複数の問題があり、条件がそろうと未認証の攻撃者がSharePoint上でユーザーとして扱われる可能性があるとされています。
認証をすり抜けられる性質の脆弱性は、公開サービスだけでなく社内ポータルでも影響が広がりやすく、権限のある利用者として操作されるおそれがあります。
SharePointは業務利用が多いため、認証基盤への影響として注目されています。

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

- Microsoftの修正情報と適用状況を確認し、対象バージョンのSharePoint Serverが残っていないか点検する。
- SharePointへの外部アクセスや認証関連のログを確認し、不審なBearerトークン利用や異常な管理操作の兆候を監視する。
- 影響が疑われる場合は、管理者権限の再点検と関連する資格情報・セッションの見直しを行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| ベンダー | F5 | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| 製品 | Microsoft Azure | 言及あり | 0.80 | — |
| 製品 | Active Directory | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Rapid7 Analysis: Microsoft SharePoint JWT Token Authentication Bypass (CVE-2026-](https://www.rapid7.com/blog/post/ra-microsoft-sharepoint-jwt-token-authentication-bypass-cve-2026-55040) | <nobr>内容確認・補足情報</nobr> |

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
| [Cisco Secure Firewall Adaptive Security ApplianceおよびSecure Firewall Threat Defense SoftwareのリモートアクセスSSL VPNにおけるサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-vpn-dos-dzv4mQFF) | 32.0 | 46.0 | 50.0 |
| [Mira Hormone MonitorとMira Android Appに関する脆弱性情報](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-223-01) | 32.0 | 46.0 | 50.0 |
| [ランサムウェアグループがサイバー攻撃の余波の中で病院のFacebookページを乗っ取る](https://therecord.media/ransomware-group-hijacks-hospital-facebook-amid-cyberattack-response) | 28.0 | 30.0 | 42.0 |
| [DeadLockランサムウェア、Polygon Smart Contractsを使って恐喝インフラの妨害を困難にする](https://thehackernews.com/2026/08/deadlock-ransomware-uses-polygon-smart.html) | 28.0 | 30.0 | 42.0 |
| [Gunraランサムウェア集団への警告、世界的に攻撃が増加](https://www.itpro.com/security/ransomware/warning-issued-over-gunra-ransomware-gang-as-attacks-ramp-up-globally) | 28.0 | 30.0 | 42.0 |
| [米国と韓国、政府機関を標的とするGunraランサムウェアについて警告](https://www.bleepingcomputer.com/news/security/us-warns-of-gunra-ransomware-attacks-against-government-critical-infrastructure/) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア攻撃グループは制御システムにアクセスしなくても産業生産を妨害できる](https://www.helpnetsecurity.com/2026/08/11/industrial-ransomware-attacks-q2-2026/) | 28.0 | 30.0 | 42.0 |
| [GunraランサムウェアがFortinetとSchneider Electricの脆弱性を悪用してネットワークに侵入](https://thehackernews.com/2026/08/gunra-ransomware-exploits-fortinet-and.html) | 28.0 | 30.0 | 42.0 |
| [Head Mare APTが未修正のTrueConfサーバーの脆弱性を悪用し、ビデオ会議参加者にPhantomCoreとPhantomGraphを配布](https://securelist.com/tr/head-mare-targets-trueconf-server-with-phantomcore/120988/) | 28.0 | 20.0 | 48.0 |
| [Sandworm関連のUAC-0145が偽の面接を使ってコマンド実行可能なVPNを配布](https://thehackernews.com/2026/08/sandworm-linked-uac-0145-uses-fake-job.html) | 28.0 | 20.0 | 42.0 |
| [Adobe、ColdFusionとCampaign Classicの重大な脆弱性に対する即時修正を呼びかけ](https://www.securityweek.com/adobe-urges-immediate-patching-of-critical-coldfusion-campaign-classic-flaws/) | 28.0 | 20.0 | 42.0 |
| [Former BlackFile関連アフィリエイトによるプライベート・エクイティ企業を標的とした恐喝キャンペーン](https://www.cybersecuritydive.com/news/former-blackfile-extortion-campaign-private-equity/827574/) | 28.0 | 20.0 | 42.0 |
| [Ciscoが警告する、公開エクスプロイトが存在するClamAVの高危険度脆弱性](https://www.bleepingcomputer.com/news/security/cisco-warns-of-high-severity-clamav-flaws-with-public-exploits/) | 28.0 | 20.0 | 42.0 |
| [Kimwolf v7：Kimwolfボットネットの進化](https://unit42.paloaltonetworks.com/kimwolf-v7-botnet-malware/) | 28.0 | 20.0 | 42.0 |
| [OpenAIがサイバー能力の「重大なしきい値」を超えたとしてAstra AIモデルの開発を一時停止、Hugging Faceを侵害したものとは別と判明](https://www.itpro.com/security/openai-has-paused-work-on-its-astra-ai-model-after-it-passed-a-critical-threshold-in-cyber-capability-but-its-not-the-one-that-breached-hugging-face) | 27.0 | 20.0 | 43.0 |
| [OpenAIが脆弱性開発向けの安全対策を緩和したGPT-5.6-Cyberを発表](https://thehackernews.com/2026/08/openai-launches-gpt-56-cyber-with.html) | 27.0 | 20.0 | 43.0 |
| [Frontier AIの登場で脆弱性修正競争がさらに難しくなった](https://www.security.com/expert-perspectives/frontier-ai-just-made-race-patch-vulns-much-harder) | 27.0 | 20.0 | 43.0 |
| [CVE-2026-63520: Microsoft SharePointのリモートコード実行（修正済み）](https://www.rapid7.com/blog/post/etr-cve-2026-63520-microsoft-sharepoint-remote-code-execution-fixed) | 27.0 | 20.0 | 42.0 |
| [CVE Program、AI時代の脆弱性急増に備え自動化とグローバル化を推進](https://www.cybersecuritydive.com/news/cve-program-ai-black-hat-def-con/827477/) | 27.0 | 20.0 | 42.0 |
| [研究者が明らかにしたAI支援のSharePoint攻撃チェーン、認証不要のRCEに到達](https://thehackernews.com/2026/08/researchers-disclose-ai-assisted.html) | 25.0 | 20.0 | 42.0 |
| [NIST、AI時代に向けて脆弱性データベースを大幅刷新へ](https://cyberscoop.com/nist-national-vulnerability-database-ai-overhaul/) | 25.0 | 20.0 | 42.0 |
| [AIガバナンスのギャップはリーダーシップの問題であり、待っていても埋まらない](https://www.securityweek.com/the-ai-governance-gap-is-a-leadership-problem-waiting-wont-close-it/) | 25.0 | 20.0 | 42.0 |
| [曖昧なタスク、完全なアクセス：AIへの委任がセキュリティリスクになるとき](https://www.bleepingcomputer.com/news/security/vague-task-total-access-when-ai-delegation-becomes-a-security-risk/) | 25.0 | 20.0 | 42.0 |
| [若者はAIを好む一方で信頼を失いつつある関係性の揺らぎ](https://www.malwarebytes.com/blog/ai/2026/08/love-hate-relationship-the-ai-affair-young-people-love-ai-but-its-breaking-their-trust) | 25.0 | 20.0 | 42.0 |
| [Corma、防御用サイバーセキュリティAIモデルのために6000万ドルを調達](https://www.securityweek.com/corma-raises-60-million-for-defensive-cybersecurity-ai-model/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、GPT 5.6 Cyberと併せて二層型セキュリティアクセスプログラムを開始](https://www.infosecurity-magazine.com/news/openai-daybreak-blue-red-gpt-cyber/) | 25.0 | 20.0 | 42.0 |
| [AIチャットを盗む拡張機能がChromeウェブストアに再登場し、悪意ある活動を再開](https://www.securityweek.com/extension-banned-for-stealing-ai-chats-returns-to-chrome-store-resumes-malicious-activities/) | 25.0 | 20.0 | 42.0 |
| [悪意あるMCPサーバーが指示を分割し、AIコーディングエージェントに機密情報を流出させる](https://thehackernews.com/2026/08/malicious-mcp-servers-can-split.html) | 25.0 | 20.0 | 42.0 |
| [OpenAIが新たなサイバーセキュリティモデルGPT-5.6-Cyberを発表](https://www.securityweek.com/openai-unveils-new-cybersecurity-model-gpt-5-6-cyber/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、セキュリティ懸念でAstraモデルの一部開発を一時停止](https://www.infosecurity-magazine.com/news/openai-pauses-development-astra/) | 25.0 | 20.0 | 42.0 |
| [Pulsetto Vagus神経刺激装置](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-223-02) | 20.0 | 28.0 | 50.0 |
| [悪意あるSIMでスマホを停止させ、ファイルを盗み、5Gを2Gに引き戻すことが可能に](https://www.theregister.com/security/2026/08/11/malicious-sims-can-shut-down-phones-steal-files-and-drag-5g-back-to-2g/5285482) | 20.0 | 28.0 | 50.0 |
| [DEF CON後のラスベガス発便で発生した機内Wi‑FiなりすましをDeltaが調査](https://cyberscoop.com/delta-flight-rogue-wifi-investigation-def-con-las-vegas/) | 20.0 | 20.0 | 48.0 |
| [Deepfakeの不具合で疑われるデジタル証明書詐欺師が露見](https://www.theregister.com/security/2026/08/11/deepfake-hiccup-unmasks-suspected-digital-certificate-fraudster/5285934) | 20.0 | 20.0 | 48.0 |
| [Project CAV3RNの続報：Google Apps ScriptをC2リレーに、DNSベースでC2チャネルを選択](https://securelist.com/project-cav3rn-continues/120991/) | 20.0 | 20.0 | 48.0 |
| [DEF CON参加者を乗せた航空便に対するWi-Fiデオーソ攻撃をDeltaが調査](https://www.bleepingcomputer.com/news/security/delta-probes-wi-fi-deauth-attack-on-flight-carrying-def-con-attendees/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、Windows 10向けKB5120249拡張セキュリティ更新を公開](https://www.bleepingcomputer.com/news/microsoft/windows-10-kb5120249-cumulative-update-released-with-fixes/) | 20.0 | 20.0 | 42.0 |
| [Valve、Steamハードウェア購入者に偽配送詐欺への警戒を呼びかけ](https://www.malwarebytes.com/blog/data-breaches/2026/08/valve-warns-steam-hardware-buyers-expect-fake-delivery-scams) | 20.0 | 20.0 | 42.0 |
| [DEF CONの参加者がDelta機内Wi-Fiの乗っ取りを試みた疑い](https://www.theregister.com/security/2026/08/11/def-con-dingus-suspected-of-trying-to-take-over-delta-in-flight-wi-fi/5286331) | 20.0 | 20.0 | 42.0 |
| [SNSプラットフォームがドローン工場の採用ゲームを取り締まり開始](https://www.malwarebytes.com/blog/news/2026/08/social-media-platforms-crack-down-on-drone-factory-recruiting-game) | 20.0 | 20.0 | 42.0 |
| [Wesco、ExfilSquadによるデータ窃取主張を受けセキュリティインシデントを確認](https://www.bleepingcomputer.com/news/security/wesco-confirms-security-incident-after-exfilsquad-claims-data-theft/) | 20.0 | 20.0 | 42.0 |
| [Zoomのゼロクリックコード実行脆弱性を修正](https://www.securityweek.com/zoom-patches-zero-click-code-execution-vulnerability/) | 20.0 | 20.0 | 42.0 |
| [物流大手Cevaへのサイバー攻撃で欧州の小売業者とSteam利用者に影響](https://therecord.media/ceva-logistics-cyberattack-bol-steam-debijenkorf-ace-tate) | 20.0 | 20.0 | 42.0 |
| [二つの戦争とワールドカップが出版社への大規模DDoS攻撃を招く](https://www.theregister.com/security/2026/08/11/two-wars-and-a-world-cup-lead-to-epic-ddos-attacks-on-publishers/5286278) | 20.0 | 20.0 | 42.0 |
| [英国の製造業者にサイバー脅威の増加に備えたレジリエンス強化を促す](https://www.itpro.com/security/cyber-attacks/uk-manufacturers-urged-to-bolster-resilience-as-cyber-threats-surge) | 20.0 | 20.0 | 42.0 |
| [6つのnpmパッケージがEthereumウォレットからC2アドレスを読み取る](https://www.infosecurity-magazine.com/news/npm-packages-ethereum-wallet-c2/) | 20.0 | 20.0 | 42.0 |
| [Cursorのセキュリティバグにより、信頼確認前にリポジトリがコマンドを実行可能だった](https://www.infosecurity-magazine.com/news/cursor-security-bug-command/) | 20.0 | 20.0 | 42.0 |
| [SAPが修正した重大なコードインジェクションとメモリ破損の脆弱性](https://www.securityweek.com/sap-patches-critical-code-injection-memory-corruption-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [米国の水道システム、新たな上院法案と「Water Watch Center」でサイバー対策を強化](https://www.securityweek.com/us-water-systems-get-cyber-boost-from-new-senate-bill-and-water-watch-center/) | 20.0 | 20.0 | 42.0 |
| [FBIが警告、オンラインアカウントを狙う性的加害者による интимな画像の収集・悪用](https://www.malwarebytes.com/blog/news/2026/08/sexual-predators-targeting-online-accounts-for-intimate-images-fbi-warns) | 20.0 | 20.0 | 42.0 |
| [Mozilla、露出を受けてFirefoxリリース用のGPG署名鍵を更新](https://www.bleepingcomputer.com/news/security/mozilla-updates-gpg-key-for-signing-firefox-thunderbird-releases-after-exposure/) | 20.0 | 20.0 | 42.0 |
| [Arctera、証拠ベースのコンプライアンスワークフロー向けUnified Platformを強化](https://www.helpnetsecurity.com/2026/08/11/arctera-unified-platform-new-capabilities/) | 20.0 | 20.0 | 42.0 |
| [1Tbps超のDDoS攻撃が第2四半期に5倍増加](https://www.bleepingcomputer.com/news/security/ddos-attacks-over-1-tbps-surged-fivefold-in-the-second-quarter/) | 20.0 | 20.0 | 42.0 |
| [4州の地方自治体、サイバー攻撃でサービス停止の被害](https://therecord.media/cyberattacks-ransomware-local-governments) | 20.0 | 20.0 | 42.0 |
| [Citrix、Platform Flexを拡張し可観測性と安全な開発者向けサービスを追加](https://www.helpnetsecurity.com/2026/08/11/citrix-platform-flex-new-services/) | 20.0 | 20.0 | 42.0 |
| [悪意あるSIMでスマートフォンを乗っ取り、ファイルを窃取して2Gに固定する手口](https://www.helpnetsecurity.com/2026/08/11/malicious-sim-cards-hijack-phones-ev-chargers/) | 20.0 | 20.0 | 42.0 |
| [悪意あるSIMカードがセルラーIoTデバイス背後のモデム内で攻撃者コードを実行可能にする](https://thehackernews.com/2026/08/a-malicious-sim-card-can-run-attacker.html) | 20.0 | 20.0 | 42.0 |
| [NCSCのSecure connectivity principlesに追加された水道分野の事例](https://www.ncsc.gov.uk/blogs/water-sector-example-added-to-the-ncscs-secure-connectivity-principles) | 20.0 | 20.0 | 42.0 |
| [カリフォルニア州スイサンシティ、米地方自治体への攻撃急増の中でサイバーインシデントに対応](https://www.infosecurity-magazine.com/news/suisan-cyber-incident-government/) | 20.0 | 20.0 | 42.0 |
| [Mozilla、GitHubに暗号化されていないコピーが公開された後にFirefoxの署名鍵を失効](https://www.theregister.com/security/2026/08/11/mozilla-revokes-firefox-signing-key-after-unencrypted-copy-lands-in-github/5285908) | 20.0 | 20.0 | 42.0 |
| [研究者が偽の暗号資産スタートアップを立ち上げ、北朝鮮関与が疑われるIT技術者3人を採用](https://thehackernews.com/2026/08/researchers-built-fake-crypto-startup.html) | 20.0 | 20.0 | 42.0 |
| [物流大手Cevaでデータ侵害、欧州顧客に影響](https://www.infosecurity-magazine.com/news/logistics-ceva-data-breach/) | 20.0 | 20.0 | 42.0 |
| [物流企業のサプライチェーン侵害がValveなどの顧客に影響](https://www.itpro.com/security/data-breaches/logistics-firm-supply-chain-breach-hits-valve-and-other-customers) | 20.0 | 20.0 | 42.0 |
| [Hacker Conversations: Marcus Hutchinsとグレーゾーンからの更生への道](https://www.securityweek.com/hacker-conversations-marcus-hutchins/) | 20.0 | 20.0 | 42.0 |
| [ssh-agentのローカル限定鍵を保護する方法とOpenSSH 10.5での変更点](https://www.helpnetsecurity.com/2026/08/11/openssh-10-5-ssh-agent-flaw/) | 20.0 | 20.0 | 42.0 |
| [偽のTikTok Shopに注意：資金をだまし取る手口](https://www.malwarebytes.com/blog/scams/2026/08/watch-out-for-fake-tiktok-shops-trying-to-steal-your-money) | 20.0 | 20.0 | 42.0 |
| [人気サイトを装って無料アプリを配布し、PCを乗っ取る手口](https://www.malwarebytes.com/blog/threat-intel/2026/08/fake-popular-sites-offer-a-free-app-instead-take-over-pcs) | 20.0 | 20.0 | 42.0 |

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
