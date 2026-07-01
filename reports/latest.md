# 📡 サイレーダー 2026-07-02 05:00 JST

このレポートは、2026-07-01 17:00 JST〜2026-07-02 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 92
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 61

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cisco Unified Communications Manager Server-Side Request Forgery Vulnerability](#topic-14652) | 55.0 | 96.0 | 91.0 | 音声 | 温度感上位枠 |
| 2 | [Researchers spot exploitation of another critical Oracle defect](#topic-20074) | 45.0 | 56.0 | 60.0 | 音声 | 温度感上位枠 |
| 3 | [Microsoft 2026年6月 Patch Tuesday 関連まとめ](#topic-15857) | 44.0 | 48.0 | 57.0 | 音声 | 温度感上位枠 |
| 4 | [22nd June – Threat Intelligence Report](#topic-15753) | 43.0 | 58.0 | 66.0 | 音声 | 温度感上位枠 |
| 5 | [AI-Generated Browser Ransomware Abuses Chromium API on Windows and Android](#topic-20398) | 41.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [Browser-Only Ransomware: From LLM Hallucinations to a Practical Attack Technique](#topic-20427) | 36.0 | 30.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-14652"></a>

### 1. Cisco Unified Communications Manager Server-Side Request Forgery Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 55.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 96.0 |
| <nobr>確⁠度</nobr> | 91.0 |

#### 概要

Cisco Unified Communications Manager（Unified CM）および Unified CM SME に、認証不要のリモート攻撃者が SSRF を引き起こせる脆弱性（CVE-2026-20230）が公表されています。
条件がそろうと、基盤OS上へのファイル書き込みを通じて権限昇格につながる可能性があり、複数の情報源で悪用観測が伝えられています。
音声・通話基盤として広く使われる製品への影響が想定され、業務停止や横展開の起点になり得るため注目されています。
Ciscoは修正更新を案内しており、緊急度の高い対応対象として扱うべき事案です。

#### CISA KEV詳細

- **CVE**: CVE-2026-20230
- **Vendor / Project**: Cisco
- **Product**: Unified Communications Manager
- **Vulnerability Name**: Cisco Unified Communications Manager Server-Side Request Forgery (SSRF) Vulnerability
- **Date Added**: 2026-06-25
- **Due Date**: 2026-06-28
- **Known Ransomware Use**: Unknown

**Required Action**

> Apply mitigations in accordance with vendor instructions, ensuring compliance with CISA’s BOD 26-04 Prioritizing Security Updates Based on Risk (see URL in Notes) guidance and CISA’s “Forensics Triage Requirements” (see URL in Notes). Follow applicable BOD 26-04 guidance for cloud services or discontinue use of the product if mitigations are unavailable. Stakeholders are responsible for evaluating each asset's internet exposure and ensuring adherence to BOD 26-04 patching guidelines.

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 7 sources。
- CISA KEV関連。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- PoC/Exploit候補: 候補あり（該当CVE 2件 / URL 6件以上）。

#### 担当者向け確認ポイント

- Ciscoの修正更新の適用状況を確認し、対象バージョンを洗い出す。
- WebDialer の有効化有無を確認し、不要なら設定見直しを検討する。
- 関連システムのログを点検し、異常なHTTP要求や不審なファイル生成の兆候がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20230 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20245 | 関連CVE | 1.00 |
| ベンダー | Cisco | 影響ベンダー | 1.00 |
| 製品 | Unified Communications Manager | 影響製品 | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20230](https://nvd.nist.gov/vuln/detail/CVE-2026-20230) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>公的機関</nobr> | [CISA KEV: CVE-2026-20230](https://www.cisa.gov/known-exploited-vulnerabilities-catalog?field_cve=CVE-2026-20230) | <nobr>KEV掲載内容、Date Added、Due Date、Required Action</nobr> |
| <nobr>公的機関データ</nobr> | [CISA KEV JSON](https://www.cisa.gov/sites/default/files/feeds/known_exploited_vulnerabilities.json) | <nobr>CISA公式の機械可読データ。CVE IDで検索して確認</nobr> |
| <nobr>出典</nobr> | [Cisco Unified Communications Manager Server-Side Request Forgery Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-cucm-ssrf-cXPnHcW) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [The hits keep on coming for Cisco vulnerabilities](https://www.theregister.com/security/2026/06/24/the-hits-keep-on-coming-for-cisco-vulnerabilities/5261797) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified CM flaw actively exploited to drop webshells (CVE-2026-20230)](https://www.helpnetsecurity.com/2026/06/24/cisco-unified-cm-flaw-exploited-to-drop-webshells-cve-2026-20230/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified CM Flaw Exploited After PoC Reveals File-Write Path to Root](https://thehackernews.com/2026/06/cisco-unified-cm-flaw-exploited-after.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers Exploiting Cisco Unified CM Vulnerability](https://www.securityweek.com/hackers-exploiting-cisco-unified-cm-vulnerability/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-20074"></a>

### 2. Researchers spot exploitation of another critical Oracle defect

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 60.0 |

#### 概要

Oracle E-Business Suite の Payments に関する重大な脆弱性「CVE-2026-46817」が、実環境で悪用されていると複数の情報源が伝えています。
内容としては権限管理や認証に関わる不備とされ、影響を受ける環境では不正な操作や乗っ取りにつながるおそれがあります。
基幹業務で使われる Oracle E-Business Suite が対象で、影響範囲が大きくなりやすい点が注目されています。
さらに、公開 PoC や悪用の兆候が示されているため、対策の遅れが被害拡大につながる懸念があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- 公開PoC/Exploitコード: 記事中で言及あり。
- PoC/Exploit候補: 候補あり（該当CVE 1件 / URL 2件以上）。

#### 担当者向け確認ポイント

- Oracle の公式情報を確認し、CVE-2026-46817 に対応する修正プログラムの適用状況を点検する。
- Oracle E-Business Suite の外部公開面や関連ログを確認し、不審な認証・権限変更の兆候を監視する。
- 影響を受ける可能性のあるシステムについて、暫定的なアクセス制御や緊急対応手順を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-46817 | 関連CVE | 1.00 |
| ransomware_group | Clop | 主題 | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-46817](https://nvd.nist.gov/vuln/detail/CVE-2026-46817) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Researchers spot exploitation of another critical Oracle defect](https://cyberscoop.com/oracle-ebs-critical-vulnerability-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Oracle E-Business Suite Payments flaw under attack (CVE-2026-46817)](https://www.helpnetsecurity.com/2026/06/30/oracle-payments-cve-2026-46817-exploitation/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Oracle E-Business Suite Flaw CVE-2026-46817 Actively Exploited in the Wild](https://thehackernews.com/2026/06/oracle-e-business-suite-flaw-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-15857"></a>

### 3. Microsoft 2026年6月 Patch Tuesday 関連まとめ

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>i⁠O⁠S</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>A⁠I</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 44.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 57.0 |

#### 概要

Microsoftの2026年6月 Patch Tuesdayでは、過去最多規模とされる多数の脆弱性修正がまとめて公開され、複数のゼロデイや公開済みの問題が含まれたと報じられています。
関連報道では、すでに攻撃事例やPoCの存在が指摘されたものもあり、優先的な対応が求められる状況です。
広範囲の製品に影響しうる修正が一度に出ているため、未対応環境ではリスクが残りやすい点が重要です。
特に、悪用可能性や実際の攻撃文脈がある項目は、通常の定期更新よりも早い確認が必要になります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 14 sources。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- PoC/Exploit候補: 候補あり（該当CVE 10件 / URL 19件以上）。

#### 担当者向け確認ポイント

- 影響を受けるWindows/関連製品の適用状況を確認し、優先度を付けて早期に更新する。
- ゼロデイや公開済み問題に該当する修正があるかを確認し、露出の高い端末を先行対応する。
- 更新後は、異常な権限昇格や不審なプロセス生成などの兆候を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-10263 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-10879 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-11463 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-26142 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-28979 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-32193 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-33113 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-33825 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-33828 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-34335 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [The June 2026 Apple Security Update Review](https://www.thezdi.com/blog/2026/6/30/the-june-2026-apple-security-update-review) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft ships largest Patch Tuesday on record, with one bug under active attac](https://therecord.media/microsoft-ships-largest-patch-tuesday-on-record) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft’s biggest-ever Patch Tuesday fixes 206 bugs, including 3 zero-days](https://www.malwarebytes.com/blog/bugs/2026/06/microsofts-biggest-ever-patch-tuesday-fixes-206-bugs-including-3-zero-days) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Record Microsoft Patch Tuesday, fresh zero-day](https://www.helpnetsecurity.com/2026/06/10/microsoft-patch-tuesday-rogueplanet/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Fixes 200 CVEs in June Patch Tuesday](https://www.infosecurity-magazine.com/news/microsoft-fixes-200-cves-in-june/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-15753"></a>

### 4. 22nd June – Threat Intelligence Report

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Catalyst SD-WAN ManagerにおけるCVE-2026-20245が、修正前から悪用されていたゼロデイ脆弱性として報告されています。
公開情報によれば、攻撃者は有効な認証情報を得るか、関連する別の脆弱性を悪用して必要な権限を取得したうえで、権限昇格につなげた可能性があります。
ネットワーク基盤や運用管理系の製品が影響を受けるため、侵害時の影響が大きくなりやすい点が注目されています。
さらに、パッチ提供前の悪用が確認されているため、既存環境では通常の脆弱性対応より広い観点での点検が必要です。

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

- PoC/Exploit候補: 候補あり（該当CVE 6件 / URL 10件以上）。

#### 担当者向け確認ポイント

- Ciscoの案内と関連アドバイザリを確認し、影響対象の有無を早急に洗い出す。
- 管理系アカウントの認証情報保護を強化し、不審なログインや権限変更の痕跡を確認する。
- 関連する既知脆弱性を含め、SD-WAN管理面の監査・ログ確認・アクセス制御を優先する。

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
| <nobr>出典</nobr> | [22nd June – Threat Intelligence Report](https://research.checkpoint.com/2026/22nd-june-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [29th June – Threat Intelligence Report](https://research.checkpoint.com/2026/29th-june-threat-intelligence-report-2/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco SD-WAN Zero-Day Exploited Months Before Patching](https://www.securityweek.com/cisco-sd-wan-zero-day-exploited-months-before-patching/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Zero-Day CVE-2026-20245 Exploited to Gain Root Access](https://thehackernews.com/2026/06/cisco-catalyst-sd-wan-zero-day-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Mandiant reveals how Cisco SD-WAN zero-day attacks gained root access](https://www.bleepingcomputer.com/news/security/mandiant-reveals-how-cisco-sd-wan-zero-day-attacks-gained-root-access/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zero-Day Exploitation of Vulnerability (CVE-2026-20245) in Cisco Catalyst SD-WAN](https://cloud.google.com/blog/topics/threat-intelligence/zero-day-exploitation-cisco-catalyst-sd-wan-manager/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN V](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-privesc-4uxFrdzx) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-20398"></a>

### 5. AI-Generated Browser Ransomware Abuses Chromium API on Windows and Android

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠n⁠d⁠r⁠o⁠i⁠d</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者は、DeepSeekが生成に関与したとされるマルウェアの成果物について、ブラウザ内の実際の機能を悪用してランサムウェア的な挙動につながる新しい攻撃経路が確認されたと報告しています。
現時点で示されているのは、WindowsとAndroidの両方でブラウザ内に収まる形の挙動が見られるという点です。
AIが攻撃コードやその発想形成に関与しうることを示す事例として、AI×セキュリティの観点で注目されています。
ブラウザという身近な実行環境が悪用される可能性があるため、端末OSだけでなくブラウザ側の対策も意識する必要があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ブラウザ経由の不審な挙動を前提に、EDRやブラウザ管理の監視観点を見直す。
- WindowsとAndroidの両環境で、ブラウザ更新や関連ポリシーが適切に適用されているか確認する。
- AI生成物を含むコード・スクリプトの取り扱いに関するレビュー手順を整備する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [AI-Generated Browser Ransomware Abuses Chromium API on Windows and Android](https://thehackernews.com/2026/07/ai-generated-browser-ransomware-abuses.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20427"></a>

### 6. Browser-Only Ransomware: From LLM Hallucinations to a Practical Attack Technique

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Check Point Researchは、LLMの出力に含まれる“幻覚”のような挙動をきっかけに、ブラウザだけで成立するランサムウェアの攻撃手法を論じています。
現時点の材料からは、実際の大規模被害や広範な悪用の確認までは読み取れませんが、AIの誤生成が攻撃研究に転用されうる点が示されています。
ブラウザ内で完結する脅威は、端末や環境によっては従来の対策の前提を崩す可能性があります。また、生成AIの出力品質や安全性が、攻撃手法の発想や検証に影響しうる点も注目されます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 生成AIを業務利用する環境では、出力内容をそのまま実装・運用に反映しない運用確認を徹底する。
- ブラウザ起点の不審な挙動に備え、Webフィルタリングや端末側の挙動監視を見直す。
- ランサムウェア対策として、バックアップの分離保管と復旧手順の定期確認を継続する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Browser-Only Ransomware: From LLM Hallucinations to a Practical Attack Technique](https://research.checkpoint.com/2026/browser-only-ransomware-from-llm-hallucinations-to-a-practical-attack-technique/) | <nobr>内容確認・補足情報</nobr> |

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
| [Adobe、ColdFusionとCampaign Classicの7件のCVSS 10.0の脆弱性を修正](https://thehackernews.com/2026/07/adobe-patches-7-cvss-100-flaws-in.html) | 30.0 | 32.0 | 42.0 |
| [ランサムウェアの潜伏時間が被害拡大を招く、侵入後に長期間潜伏する攻撃とデータ窃取の実態](https://www.itpro.com/security/every-hour-ransomware-goes-undetected-drastically-increases-its-potential-blast-radius-hackers-are-breaching-networks-and-laying-low-for-longer-and-nearly-half-of-firms-dont-realize-until-data-is-stolen) | 28.0 | 30.0 | 42.0 |
| [SEO汚染されたソフトウェアサイトがScreenConnectを悪用してAsyncRATを配布](https://thehackernews.com/2026/07/seo-poisoned-software-sites-abuse.html) | 28.0 | 20.0 | 42.0 |
| [VEIL#DROPマルウェアチェーンがBloggerプラットフォームを悪用してPureLogs Stealerを配布](https://thehackernews.com/2026/07/veildrop-malware-chain-uses-blogger.html) | 28.0 | 20.0 | 42.0 |
| [HackersがMicrosoft 365アカウントを標的にした8100万件のログイン試行](https://www.bleepingcomputer.com/news/security/hackers-target-microsoft-365-accounts-with-81-million-login-attempts/) | 28.0 | 20.0 | 42.0 |
| [Ousaban Banking Trojanが偽PDFを使ってイベリアの銀行利用者を標的にする](https://thehackernews.com/2026/07/ousaban-banking-trojan-targets-iberian.html) | 28.0 | 20.0 | 42.0 |
| [Fileless MalwareがGoogle Blogspotを悪用してメモリ上にInfostealerを展開](https://www.infosecurity-magazine.com/news/veil-drop-blogspot-purelog-stealer/) | 28.0 | 20.0 | 42.0 |
| [Adobe、ColdFusionとCampaign Classicの深刻な脆弱性を修正](https://www.securityweek.com/adobe-patches-critical-coldfusion-campaign-classic-vulnerabilities/) | 28.0 | 20.0 | 42.0 |
| [ScreenConnectをフリーウェアに偽装した大規模キャンペーンの内幕](https://securelist.com/tr/the-soc-files-screenconnect-campaign-with-asyncrat/120472/) | 28.0 | 20.0 | 42.0 |
| [BioShocking：AIエージェントを「ゲーム」で操る行為がもはや遊びではない理由](https://www.malwarebytes.com/blog/ai/2026/07/bioshocking-when-gaming-ai-agents-is-no-longer-a-game) | 27.0 | 20.0 | 42.0 |
| [Claude Codeがユーザーの接続経路を「日付の書式を変更する」という手法で記録していたとの指摘、「2026-06-30」「2026/06/30」といった書式の違いで見分ける仕組み](https://gigazine.net/news/20260701-claude-code-prompt-steganography/) | 27.0 | 20.0 | 42.0 |
| [Microsoft Teamsに会議への無許可AIボットをブロックする新しい制御を追加](https://www.securityweek.com/microsoft-adds-new-teams-controls-to-block-unauthorized-ai-bots-from-meetings/) | 25.0 | 20.0 | 42.0 |
| [Red teamerがClaude Desktopを二重スパイ化して悪事を実行させた件](https://www.theregister.com/security/2026/07/01/red-teamers-turned-claude-desktop-into-a-double-agent-to-do-their-evil-bidding/5264692) | 25.0 | 20.0 | 42.0 |
| [SOCにおけるAIに関する5つの誤解、セキュリティチームが見直すべきこと](https://www.rapid7.com/blog/post/ai-rethinking-5-soc-myths) | 25.0 | 20.0 | 42.0 |
| [Phantom Squatting：AI駆動で新たに浮上するサプライチェーン脅威](https://www.darkreading.com/endpoint-security/phantom-squatting-ai-driven-supply-chain-threat) | 25.0 | 20.0 | 42.0 |
| [Anthropic、政府承認を得てFableとMythosを再開](https://www.cybersecuritydive.com/news/anthropic-ai-mythos-fable-reenable/824214/) | 25.0 | 20.0 | 42.0 |
| [米国、AnthropicのMythosとFableに対する輸出規制を解除](https://cyberscoop.com/us-lifting-export-control-restrictions-anthropic-mythos-fable/) | 25.0 | 20.0 | 42.0 |
| [米国、Anthropicの先端サイバーセキュリティAIモデルへの輸出規制を解除](https://therecord.media/us-lifts-export-controls-anthropic-cyber-models) | 25.0 | 20.0 | 42.0 |
| [AI推論がクラウドを圧迫している](https://www.akamai.com/blog/ai/2026/jun/ai-inference-swallowing-the-cloud) | 25.0 | 20.0 | 42.0 |
| [Netziloが主要プラットフォーム横断でAIエージェント向け実行時ガバナンスを追加](https://www.helpnetsecurity.com/2026/07/01/netzilo-adds-runtime-governance-for-ai-agents-across-major-platforms/) | 25.0 | 20.0 | 42.0 |
| [AnthropicのFable 5とMythos 5が新たなセキュリティガードレールとともに再登場](https://www.infosecurity-magazine.com/news/anthropic-fable-mythos-back/) | 25.0 | 20.0 | 42.0 |
| [Frontier AI：企業がセキュリティベンダーに必ず尋ねるべき6つの質問](https://www.securityweek.com/frontier-ai-six-questions-every-enterprise-should-ask-security-vendors/) | 25.0 | 20.0 | 42.0 |
| [ChatGPTが研究者を驚かせる過激な暴力画像を生成](https://www.malwarebytes.com/blog/ai/2026/07/chatgpt-produced-graphic-violent-images-that-shocked-researchers) | 25.0 | 20.0 | 42.0 |
| [Claude Sonnet 5は危険なサイバー利用に対する安全対策を備える](https://www.helpnetsecurity.com/2026/07/01/anthropic-claude-sonnet-5/) | 25.0 | 20.0 | 42.0 |
| [Cisco Catalyst Centerの任意ファイル読み取り脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-catc-file-read-wLH2vf8X) | 24.0 | 46.0 | 50.0 |
| [Progress Kemp LoadMasterの認証前RCE脆弱性、実際の悪用試行を確認](https://thehackernews.com/2026/07/latest-progress-kemp-loadmaster-pre.html) | 24.0 | 46.0 | 50.0 |
| [CitrixがNetScalerの脆弱性を修正、新たな「HTTP/2 Bomb」攻撃も含む](https://www.securityweek.com/citrix-patches-netscaler-vulnerabilities-including-new-http-2-bomb-attack/) | 22.0 | 28.0 | 42.0 |
| [耐量子暗号対応への道 第2回: 移行プレイブック](https://blog.nviso.eu/2026/07/01/the-road-to-post-quantum-readiness-part-2-of-2-the-migration-playbook/) | 22.0 | 20.0 | 48.0 |
| [Microsoft、クラウドとアプリケーション実行時セキュリティのFrost Radarでリーダーに選出](https://www.microsoft.com/en-us/security/blog/2026/07/01/microsoft-named-a-leader-in-the-frost-radar-for-cloud-and-application-runtime-security/) | 22.0 | 20.0 | 42.0 |
| [サポート詐欺でPC遠隔操作、情報流出を調査 - 東北文化学園大](https://www.security-next.com/186648) | 22.0 | 20.0 | 42.0 |
| [システムの登録ユーザー情報、ユーザー間で閲覧可能に - コマツ](https://www.security-next.com/186504) | 22.0 | 20.0 | 42.0 |
| [児童情報を全認定こども園にメール誤送信 - 八王子市](https://www.security-next.com/186577) | 22.0 | 20.0 | 42.0 |
| [Martin Lee: Arcticを駆け抜ける（脅威の全体像）](https://blog.talosintelligence.com/martin-lee-running-through-the-arctic-and-the-threat-landscape/) | 22.0 | 20.0 | 42.0 |
| [ARToken: Microsoft 365を狙うEvilTokensアフィリエイトパネルの内部](https://blog.talosintelligence.com/artoken-inside-an-eviltokens-affiliate-panel-targeting-microsoft-365/) | 22.0 | 20.0 | 42.0 |
| [「Apache Tomcat」に複数脆弱性 - 「クリティカル」との評価も](https://www.security-next.com/186655) | 22.0 | 20.0 | 42.0 |
| [Cisco製品に影響するClamAVの脆弱性：2026年7月](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-clamav-88cFYyxR) | 20.0 | 28.0 | 50.0 |
| [Cursorの深刻な脆弱性により、プロンプトインジェクションでサンドボックスを回避しコマンド実行が可能に](https://thehackernews.com/2026/07/critical-cursor-flaws-could-let-prompt.html) | 20.0 | 28.0 | 50.0 |
| [Chromeに再び大型アップデート、382件のセキュリティバグを修正](https://www.malwarebytes.com/blog/bugs/2026/07/chrome-needs-another-whopper-update-to-fix-382-security-fixes) | 20.0 | 28.0 | 50.0 |
| [DHS、情報共有プラットフォームHSINへの侵入を確認](https://www.bleepingcomputer.com/news/security/dhs-confirms-hackers-breached-hsin-info-sharing-platform/) | 20.0 | 20.0 | 42.0 |
| [今週GitHubメンテナーが有効化すべき6つのセキュリティ設定](https://github.blog/security/6-security-settings-every-github-maintainer-should-enable-this-week/) | 20.0 | 20.0 | 42.0 |
| [Oracle E-Business Suiteの重大な脆弱性が差し迫った脅威にさらされる](https://www.cybersecuritydive.com/news/critical-flaw-oracle-e-business-suite-threat/824230/) | 20.0 | 20.0 | 42.0 |
| [OpenCTIでCriminal IPを活用してインジケーターをインテリジェンスに変換する方法](https://www.bleepingcomputer.com/news/security/turning-indicators-into-intelligence-in-opencti-with-criminal-ip/) | 20.0 | 20.0 | 42.0 |
| [Cyber Brief 26-07 - 2026年6月](https://cert.europa.eu/publications/threat-intelligence/cb26-07/) | 20.0 | 20.0 | 42.0 |
| [ブラジルのバンキングトロージャンOusabanがスペインとポルトガルを標的にした](https://www.infosecurity-magazine.com/news/ousaban-banking-trojan-spain/) | 20.0 | 20.0 | 42.0 |
| [日本の保険会社、ビール会社、製造業者、通信事業者がサイバー侵害を公表](https://therecord.media/japan-cyber-breaches-aflac-sapporo-nidec-kddi) | 20.0 | 20.0 | 42.0 |
| [Threat Intelとデジタルセキュリティで安全なイベントを実現する方法](https://www.darkreading.com/threat-intelligence/safe-events-threat-intel-digital-security) | 20.0 | 20.0 | 42.0 |
| [900件超のOracle E-Businessインスタンスが継続的な攻撃にさらされる](https://www.bleepingcomputer.com/news/security/over-900-oracle-e-business-instances-exposed-to-ongoing-attacks/) | 20.0 | 20.0 | 42.0 |
| [Dawnguard、セキュアなクラウドアーキテクチャを自動化するプラットフォームを発表](https://www.helpnetsecurity.com/2026/07/01/dawnguard-security-architecture-automation-platform/) | 20.0 | 20.0 | 42.0 |
| [リリースノート：ブラウザ内データ検査、Torq連携、1,100件超の脅威カバレッジ更新](https://any.run/cybersecurity-blog/release-notes-june-2026/) | 20.0 | 20.0 | 42.0 |
| [2026年サイバーセキュリティ評価：認識とレジリエンスのギャップ](https://thehackernews.com/2026/07/2026-cybersecurity-assessment-gap.html) | 20.0 | 20.0 | 42.0 |
| [Intruder、リソースの限られたIT・セキュリティチーム向けに無料のセキュリティプランを提供](https://www.helpnetsecurity.com/2026/07/01/intruder-offers-free-security-plan-for-lean-it-and-security-teams/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、耐量子暗号への移行を2029年へ前倒し](https://thehackernews.com/2026/07/microsoft-accelerates-post-quantum.html) | 20.0 | 20.0 | 42.0 |
| [ARTokenのフィッシングパネルがMicrosoft 365アカウントを標的にする](https://www.helpnetsecurity.com/2026/07/01/artoken-phishing-panel-microsoft-365-accounts/) | 20.0 | 20.0 | 42.0 |
| [Microsoftが量子耐性対応の取り組みを加速、新たなタイムラインを発表](https://www.infosecurity-magazine.com/news/microsoft-accelerates-quantumsafe/) | 20.0 | 20.0 | 42.0 |
| [BEC as a Serviceに見せかけたこのフィッシングキット](https://cyberscoop.com/artoken-bec-platform-cisco-talos/) | 20.0 | 20.0 | 42.0 |
| [AV-TEST、Symantec Endpoint Security Completeに満点評価](https://www.security.com/feature-stories/av-test-symantec-endpoint-security-complete) | 20.0 | 20.0 | 42.0 |
| [詐欺被害者への証拠開示を怠ったとしてAmazonに225万ドルの罰金](https://www.bleepingcomputer.com/news/security/amazon-fined-225m-for-withholding-evidence-from-fraud-victims/) | 20.0 | 20.0 | 42.0 |
| [Apple、iOS・macOS・Safariの多数の脆弱性を修正](https://www.securityweek.com/apple-patches-dozens-of-vulnerabilities-across-ios-macos-and-safari/) | 20.0 | 20.0 | 42.0 |
| [保険大手Aflac、数百万人に影響するデータ侵害を公表](https://www.infosecurity-magazine.com/news/insurance-giant-aflac-data-breach/) | 20.0 | 20.0 | 42.0 |
| [Dawnguard、セキュリティアーキテクチャ自動化プラットフォームの開発資金として630万ドルを調達](https://www.securityweek.com/dawnguard-raises-6-3-million-for-security-architecture-automation-platform/) | 20.0 | 20.0 | 42.0 |
| [Claude Fable 5とAI支援による第三者リスクの新たな現実](https://www.bitsight.com/de/blog/claude-fable-5-und-die-neue-realitaet-von-ki-gestuetztem-drittparteirisiko) | 10.0 | 20.0 | 42.0 |

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
