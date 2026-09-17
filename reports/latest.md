# 📡 サイレーダー 2026-09-18 05:00 JST

このレポートは、2026-09-17 17:00 JST〜2026-09-18 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 110
- [音声で扱う想定のトピック](#audio-topics): 8
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 77

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks](#topic-216) | 72.0 | 99.0 | 92.0 | 音声 | AI×Security枠 |
| 2 | [Cisco Secure Email Gateway SQL Injection Vulnerability](#topic-32497) | 52.0 | 74.0 | 67.0 | 音声 | 温度感上位枠 |
| 3 | [Unauthenticated attackers are bypassing Cisco ISE’s management interface (CVE-2026-76460)](#topic-32957) | 47.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 4 | [Druva expands identity resilience with ransomware detection](#topic-33251) | 33.0 | 30.0 | 42.0 | 音声 | AI×Security枠 |
| 5 | [Scammers leave AI fingerprints all over fake antivirus renewal page](#topic-33282) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 6 | [Hitachi Energy FACTS Control Platform (FCP)](#topic-33260) | 32.0 | 46.0 | 50.0 | 音声 | 温度感上位枠 |
| 7 | [PolinRider Spreads Through Compromised GitHub Accounts and Packagist](#topic-33214) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 8 | [LausivLoader analysis, or how to pass data between malware stages, (Thu, Sep 17th)](#topic-33217) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-216"></a>

### 1. CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 72.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 99.0 |
| <nobr>確⁠度</nobr> | 92.0 |

#### 概要

cPanel & WHM における CVE-2026-41940 は、認証を回避して管理権限に近い操作につながり得る問題として、実際の攻撃で悪用されたと報告されています。
公開情報では、ランサムウェア関連の活動やサーバー侵害の文脈で観測されており、検証コードやPoC言及も見られます。
認証バイパスは、外部からの侵入を大きく容易にし、ホスティング環境や管理対象サイト全体に影響が及ぶおそれがあります。
公開PoCや悪用情報がある場合、未対策環境は短期間で狙われやすくなるため、優先度が高い事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 12 sources。
- CISA KEV関連。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- cPanel & WHM の対象バージョンと公開状況を確認し、提供元の修正情報を反映する。
- 管理画面へのアクセス制御を再点検し、不要な公開やアカウントの棚卸しを行う。
- 侵害の兆候として、想定外のログイン、設定変更、ファイル改変、バックドア設置の有無を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-40473 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-41940 | 関連CVE | 1.00 | 候補あり（URL 11件以上） |
| 脆弱性 | CVE-2026-42208 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | cPanel | 言及あり | 0.80 | — |
| 製品 | WHM | 言及あり | 0.80 | — |
| 製品 | cPanel | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-41940](https://nvd.nist.gov/vuln/detail/CVE-2026-41940) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Ransomware incidents in Japan in the first half of 2026: Investigation of The Ge](https://blog.talosintelligence.com/ransomware-incidents-in-japan-in-the-first-half-of-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Large-Scale GitHub Actions Abuse Powers a Distributed cPanel and WHM Exploitatio](https://socket.dev/blog/github-actions-abuse-powers-cpanel-and-whm-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [What’s New in Rapid7 Products and Services: Q2 2026 in Review](https://www.rapid7.com/blog/post/pt-new-products-services-q2-2026-mdr) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Weekly Report: Apache Camelに複数の脆弱性](https://www.jpcert.or.jp/wr/2026/wr260513.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Stealthy hackers exploit cPanel flaw in active backdoor campaign (CVE-2026-41940](https://www.helpnetsecurity.com/2026/05/12/cpanel-vulnerability-exploited-backdoor-cve-2026-41940/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [cPanel CVE-2026-41940 Under Active Exploitation to Deploy Filemanager Backdoor](https://thehackernews.com/2026/05/cpanel-cve-2026-41940-under-active.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Week in review: cPanel vulnerability actively exploited, DigiCert breach, Linked](https://www.helpnetsecurity.com/2026/05/10/week-in-review-cpanel-vulnerability-actively-exploited-digicert-breach-linkedin-job-scams/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 採用あり（1件）。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-32497"></a>

### 2. Cisco Secure Email Gateway SQL Injection Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 52.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Cisco Secure Email Gateway に影響する CVE-2026-76461 は、メール処理に起因するSQLインジェクション脆弱性として公表されました。
公開情報では、認証不要のリモート攻撃で装置上の権限昇格や任意コマンド実行につながる可能性があり、Cisco は修正更新を案内しています。
メールセキュリティ機器は組織の受信経路に位置するため、影響が出ると広範囲のメール防御や境界防御に波及し得ます。
さらに、公開PoCや実際の悪用が示唆されているため、通常の脆弱性よりも優先度を高めて確認する必要があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Ciscoの案内に従い、影響を受ける版の有無を確認して速やかに更新を適用する。
- 公開されている侵害指標やログを確認し、既に不正利用の兆候がないか点検する。
- 外部公開されたメールゲートウェイは特に優先して棚卸しし、対象資産の把握と監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-76461 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-76461](https://nvd.nist.gov/vuln/detail/CVE-2026-76461) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Email Gateway SQL Injection Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-esa-inj-2bLVGmhX) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco email security boxes can be rooted by... an email](https://www.theregister.com/security/2026/09/15/cisco-email-security-boxes-can-be-rooted-by-an-email/5296604) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns customers of actively exploited zero-day in email gateways](https://cyberscoop.com/cisco-secure-email-gateway-zero-day-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-76461: Critical Cisco Secure Email Gateway Vulnerability Exploited in t](https://www.rapid7.com/blog/post/etr-cve-2026-76461-critical-cisco-secure-email-gateway-vulnerability-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco patches actively exploited email gateway zero-day (CVE-2026-76461)](https://www.helpnetsecurity.com/2026/09/15/cve-2026-76461-cisco-email-gateway-zero-day-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: Cisco Secure Email GatewayにおけるSQLインジェクションの脆弱性（CVE-2026-76461）に関する注意喚起  (公開](https://www.jpcert.or.jp/at/2026/at260027.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Email Gateway Flaw Exploited in the Wild, Enables Root Command Exec](https://thehackernews.com/2026/09/cisco-secure-email-gateway-flaw.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（2件）。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-32957"></a>

### 3. Unauthenticated attackers are bypassing Cisco ISE’s management interface (CVE-2026-76460)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 47.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Cisco Identity Services Engine（ISE）のAPIに認証回避の脆弱性（CVE-2026-76460）があり、未認証のリモート攻撃者が管理画面の認証を回避できる可能性があると案内されています。
Ciscoは修正版ソフトウェアを公開しており、現時点で有効な回避策は示されていません。
認証基盤やネットワークアクセス制御を担うISEが影響を受けるため、侵害時の影響範囲が広くなり得ます。
さらに、公開情報では実際の悪用が観測されている文脈があり、早期対応の重要性が高いと見られます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
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

- 影響を受けるISE/ISE-PICの稼働有無とバージョンを確認し、Ciscoの修正版適用可否を早急に判断する。
- 管理インターフェースへのアクセス制御や到達性を見直し、不要な公開を避ける。
- 認証回避の兆候や不審な管理操作がないか、監査ログとアラートを重点的に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-76460 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Identity Services Engine | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-76460](https://nvd.nist.gov/vuln/detail/CVE-2026-76460) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco drops another exploited zero-day, this time a perfect 10](https://www.theregister.com/security/2026/09/17/cisco-drops-another-exploited-zero-day-this-time-a-perfect-10/5297180) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-76460: A critical Cisco ISE authentication bypass under active exploita](https://www.bitsight.com/blog/critical-vulnerability-alert-cve-2026-76460-cisco-ise-authentication-bypass) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Unauthenticated attackers are bypassing Cisco ISE’s management interface (CVE-20](https://www.helpnetsecurity.com/2026/09/17/cisco-ise-vulnerability-exploited-cve-2026-76460/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Identity Services Engine Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ISE-ABP-VNSW7Tn5) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Warns of Active Exploitation of Critical ISE Flaw](https://www.infosecurity-magazine.com/news/cisco-active-exploitation-critical/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33251"></a>

### 4. Druva expands identity resilience with ransomware detection

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Druvaは、Identity Resilienceの機能拡張とあわせて、ランサムウェア検知機能の提供を発表しました。
行動ベースの分析と検証を組み合わせ、疑わしい挙動を証拠として整理し、影響の確認や復旧判断を支援する考え方が示されています。
ID基盤やバックアップ周辺での異常検知・影響確認は、侵害時の初動を左右しやすいため注目されています。
AIを使った判別支援は、正常動作と攻撃兆候の切り分けを早める可能性があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ID関連の異常検知が既存の監視・インシデント対応手順とどう連携するかを確認する。
- 検知結果を復旧判断に使う場合、誤検知時の運用手順や確認責任を明確にしておく。
- ランサムウェア対策として、検知だけでなくバックアップ整合性確認や復旧訓練との組み合わせを見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Druva expands identity resilience with ransomware detection](https://www.helpnetsecurity.com/2026/09/17/druva-identity-resilience-ransomware-detection/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33282"></a>

### 5. Scammers leave AI fingerprints all over fake antivirus renewal page

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Malwarebytesの調査で、AIの影響が疑われる、作り込みのよい偽のアンチウイルス更新ページが確認されたとされています。
対象はAvastを装ったもので、ベルギーの利用者を狙った表示内容だったとされていますが、AIの関与の程度など未確認の点もあります。
フィッシングや詐欺ページが、専門知識が乏しくても見た目の精度を上げやすくなっている可能性を示すため注目されています。
利用者だけでなく、正規製品を扱う企業にとってもブランド悪用対策の重要性が増します。

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

- 更新通知や請求画面を装うページは、見た目だけで判断せず正規ドメインや導線を確認する。
- ブランド名を騙る詐欺が増える前提で、顧客向け注意喚起や問い合わせ導線の整備を見直す。
- サポート窓口に寄せられる請求・更新系の問い合わせを監視し、偽ページの兆候を早期把握する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Scammers leave AI fingerprints all over fake antivirus renewal page](https://www.helpnetsecurity.com/2026/09/17/ai-antivirus-renewal-scam-fake-pages/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-33260"></a>

### 6. Hitachi Energy FACTS Control Platform (FCP)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 32.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 50.0 |

#### 概要

Hitachi EnergyのFACTS Control Platform（FCP）で、GWSコンポーネントを含む複数バージョンに複数の脆弱性が公表されました。
CVE-2024-4872では、認証済み攻撃者によるクエリ検証の不備が問題とされ、永続データへのコード注入につながる可能性が示されています。
影響は主に2020年以降に展開されたGWS付き環境が対象で、GWSを含まない導入は対象外とされています。
FCPは電力系を含む産業制御分野で使われるため、可用性や完全性への影響が広い範囲に及ぶ可能性があります。
特に認証済みユーザー前提の不備や、外部公開面に関わる問題が含まれている点は、運用上の確認優先度を高めます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- GWSコンポーネントの有無と、対象バージョン（3.4.0〜4.1.1の該当範囲）を棚卸しする。
- 公開ネットワークからの到達可否を確認し、制御系ネットワークの分離や露出最小化を再点検する。
- ベンダーの是正情報と推奨対策を確認し、認証情報の管理やアクセス権限の見直しを含めて対応する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2024-3980 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2024-3982 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2024-4872 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2024-7940 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2024-7941 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2024-4872](https://nvd.nist.gov/vuln/detail/CVE-2024-4872) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Hitachi Energy FACTS Control Platform (FCP)](https://www.cisa.gov/news-events/ics-advisories/icsa-26-260-03) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-33214"></a>

### 7. PolinRider Spreads Through Compromised GitHub Accounts and Packagist

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

PolinRiderに関する脅威情報として、侵害されたGitHubアカウントが悪用され、Packagist上のあるパッケージの開発版4件に不正なコードが混入したとされています。
対象パッケージは70万回超ダウンロードされており、依存関係を通じた供給網リスクが示唆されます。
開発者アカウントや配布基盤が侵害されると、正規の更新に見せかけて広く影響が及ぶ可能性があります。
特にパッケージ管理基盤を利用する組織では、依存ライブラリの検証と更新監視の重要性が改めて高まります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- GitHubやパッケージレジストリのアカウント保護を強化し、異常な変更や公開履歴の改変を監視する。
- 依存パッケージの更新時は、バージョン固定や整合性確認を行い、開発版や新規リリースの取り込みを慎重に判断する。
- 利用中のパッケージに不審な更新がないか棚卸しし、影響範囲を把握できるよう依存関係を可視化しておく。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [PolinRider Spreads Through Compromised GitHub Accounts and Packagist](https://socket.dev/blog/polinrider-github-packagist) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-33217"></a>

### 8. LausivLoader analysis, or how to pass data between malware stages, (Thu, Sep 17th)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

SANS Internet Storm Center は、8月末に確認されたマルスパムを起点とする事例として、LausivLoader に関する分析を公開しました。
内容は、見積依頼を装ったメールをきっかけに、マルウェアの各段階間でデータを受け渡す仕組みが論点になっているとされています。
メールを起点とする攻撃は業務環境に紛れ込みやすく、初動の見落としがその後の展開につながるおそれがあります。
マルウェアの段階間でのデータ受け渡しは検知や分析を難しくするため、挙動の把握が重要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 見積依頼や添付ファイルを装う不審メールについて、送信元・本文・添付の整合性を確認する。
- メールゲートウェイやEDRで、段階的に展開される不審な挙動や連鎖的な通信を監視する。
- 類似文面のマルスパムを受けた場合に備え、報告・隔離・初動対応の手順を再確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [LausivLoader analysis, or how to pass data between malware stages, (Thu, Sep 17t](https://isc.sans.edu/diary/rss/33348) | <nobr>内容確認・補足情報</nobr> |

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
| [中国製「RatHat」Androidマルウェア、AIを悪用して金融データを窃取](https://www.infosecurity-magazine.com/news/rathat-android-malware-ai-steal/) | 33.0 | 20.0 | 42.0 |
| [偽のAI取引エージェントが暗号資産ウォレットのパスワードを窃取](https://www.helpnetsecurity.com/2026/09/17/fake-ai-trading-agent-research/) | 33.0 | 20.0 | 42.0 |
| [サプライチェーンリスクの拡大で製造業へのランサムウェア攻撃が急増](https://www.securityweek.com/ransomware-attacks-on-manufacturers-surge-as-supply-chain-risk-grows/) | 28.0 | 30.0 | 42.0 |
| [MSSPが「何も起きなかった」ときに価値を証明する方法](https://any.run/cybersecurity-blog/how-mssps-prove-value/) | 28.0 | 30.0 | 42.0 |
| [中国のSalt Typhoonが新たな監視用マルウェアでラテンアメリカの組織にバックドアを設置](https://www.theregister.com/security/2026/09/17/chinas-salt-typhoon-backdoors-latin-american-orgs-with-new-snooping-malware/5297286) | 28.0 | 20.0 | 42.0 |
| [Brevoのサプライチェーン攻撃で顧客サイトにClickFixスクリプトが注入される](https://www.bleepingcomputer.com/news/security/brevo-supply-chain-attack-injected-clickfix-scripts-on-customer-sites/) | 28.0 | 20.0 | 42.0 |
| [当局が人気の長期稼働DDoS代行サービスのドメインを差し押さえ](https://cyberscoop.com/fbi-seizes-nightmarestresser-ddos-for-hire-domains/) | 28.0 | 20.0 | 42.0 |
| [改ざんされたトレント経由で複数国のユーザーを狙うMovieReaperの攻撃](https://securelist.com/moviereaper-malware-torrent-odyssey-solana/121344/) | 28.0 | 20.0 | 42.0 |
| [T-Mobileのリワードポイント失効を装うフィッシング詐欺](https://www.malwarebytes.com/blog/threat-intel/2026/09/t-mobile-rewards-points-expiry-texts-are-a-phishing-scam) | 28.0 | 20.0 | 42.0 |
| [中国系のFamousSparrowがラテンアメリカ全域にSparroWockyバックドアを展開](https://thehackernews.com/2026/09/china-aligned-famoussparrow-deploys.html) | 28.0 | 20.0 | 42.0 |
| [中国のハッカーが政府へのスパイ活動でSparroWockyマルウェアを使用](https://www.bleepingcomputer.com/news/security/chinese-hackers-use-sparrowocky-malware-in-govt-espionage-attacks/) | 28.0 | 20.0 | 42.0 |
| [AIによるハッキングの終末は避けられないものではない](https://cyberscoop.com/ai-agent-hacking-apocalypse-cybersecurity/) | 27.0 | 20.0 | 42.0 |
| [「AI slowdown」は気にすべきか](https://blog.talosintelligence.com/should-you-care-about-an-ai-slowdown/) | 27.0 | 20.0 | 42.0 |
| [iPhoneで撮影した写真がAI生成されていない「本物」だと証明する「Apple Reference Image」はどういう仕組みなのか？](https://gigazine.net/news/20260917-apple-reference-image/) | 27.0 | 20.0 | 42.0 |
| [東京ゲームショウ2026開幕、AI活用続々 3D制作や可観測性ツールなど](https://xtech.nikkei.com/atcl/nxt/column/18/03763/091700001/) | 26.0 | 20.0 | 42.0 |
| [デジタル相に古川俊治氏 AI戦略やサイバー安保も担当 外科医で弁護士、MBAも取得](https://www.itmedia.co.jp/news/article/2609/17/2000001594/) | 26.0 | 20.0 | 42.0 |
| [OpenAI、AIエージェントが無断で行動する追加事例を詳述](https://www.bleepingcomputer.com/news/security/openai-details-more-cases-of-ai-agents-taking-unauthorized-actions/) | 25.0 | 20.0 | 42.0 |
| [OpenAIのモデルが学習中にGitHubで漏えいしたAPIキーを検索していた件](https://www.securityweek.com/openai-says-its-models-hunted-github-for-leaked-api-keys-during-training/) | 25.0 | 20.0 | 42.0 |
| [AI脅威動向ダイジェスト：2026年7月～8月](https://research.checkpoint.com/2026/ai-threat-landscape-digest-july-august-2026/) | 25.0 | 20.0 | 42.0 |
| [Agent Intentを理解するAI検知エンジンの構築](https://www.wiz.io/blog/building-an-ai-detection-engine-for-agent-intent) | 25.0 | 20.0 | 42.0 |
| [最近のAI活用攻撃が示すアイデンティティセキュリティへの影響](https://www.bleepingcomputer.com/news/security/what-recent-ai-powered-attacks-mean-for-your-identity-security/) | 25.0 | 20.0 | 42.0 |
| [偽のChatGPT請求メールでOpenAIのパスワードを狙う攻撃](https://www.helpnetsecurity.com/2026/09/17/chatgpt-phishing-email-openai-password/) | 25.0 | 20.0 | 42.0 |
| [Comp AIがAIネイティブのコンプライアンスとセキュリティで3400万ドルを調達](https://www.securityweek.com/comp-ai-raises-34-million-for-ai-native-compliance-and-security/) | 25.0 | 20.0 | 42.0 |
| [Schneider Electric PowerChute Serial Shutdown の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-260-07) | 25.0 | 20.0 | 42.0 |
| [Schneider Electric NetBotz 5 750/755の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-260-05) | 25.0 | 20.0 | 42.0 |
| [Schneider Electric Modicon M340コントローラーおよび通信モジュール](https://www.cisa.gov/news-events/ics-advisories/icsa-26-260-04) | 25.0 | 20.0 | 42.0 |
| [Googleの新しいエージェントセキュリティシステムがツールの悪用、ループ、異常な挙動を検知](https://www.helpnetsecurity.com/2026/09/17/google-agent-anomaly-detection-audit-layer/) | 25.0 | 20.0 | 42.0 |
| [スペイン、初のAIエージェントによるハッキングを確認](https://www.itpro.com/security/cyber-attacks/spain-says-it-has-seen-first-ai-agent-hack) | 25.0 | 20.0 | 42.0 |
| [CISO向け：WebサイトのAgentic Pentesting実践ガイド](https://thehackernews.com/2026/09/cisos-expert-guide-to-agentic.html) | 25.0 | 20.0 | 42.0 |
| [OpenAI、隠れた失敗と不正なアップロードに関する6件のモデルインシデントを公表](https://thehackernews.com/2026/09/openai-reveals-six-model-incidents.html) | 25.0 | 20.0 | 42.0 |
| [OpenAIが新たに6件の不正AI事案を公表](https://www.itpro.com/technology/artificial-intelligence/openai-reveals-six-more-rogue-ai-incidents) | 25.0 | 20.0 | 42.0 |
| [スペイン、自治型AIエージェントを含む初のデータ侵害を報告](https://www.helpnetsecurity.com/2026/09/17/spain-ai-agent-data-breach/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントによる多段階データ窃取攻撃](https://www.infosecurity-magazine.com/news/ai-agent-carries-out-multistage/) | 25.0 | 20.0 | 42.0 |
| [CriticalなUnbound DNSSEC Validatorの欠陥により悪意あるDNSゾーン経由でRCEが可能に](https://thehackernews.com/2026/09/critical-unbound-dnssec-validator-flaw.html) | 24.0 | 46.0 | 50.0 |
| [Cisco、FMC・ISE・Nexus Dashboardに存在した多数の脆弱性を修正](https://www.securityweek.com/cisco-fixes-dozens-of-flaws-across-fmc-ise-and-nexus-dashboard/) | 24.0 | 38.0 | 42.0 |
| [BIND 9の更新で14件の脆弱性を修正、DNS-over-HTTPSで認証不要のクラッシュも含む](https://thehackernews.com/2026/09/bind-9-update-fixes-14-flaws-including.html) | 24.0 | 38.0 | 42.0 |
| [指針から実践へ：リスクを実質的に低減するセキュリティの基本原則](https://www.microsoft.com/en-us/security/blog/2026/09/17/from-guidance-to-action-security-fundamentals-that-materially-reduce-risk/) | 22.0 | 20.0 | 42.0 |
| [Microsoft Defenderの実例から学ぶメールセキュリティの改善策](https://www.microsoft.com/en-us/security/blog/2026/09/17/improving-email-security-outcomes-with-real-world-microsoft-defender-insights/) | 22.0 | 20.0 | 42.0 |
| [一部@cosme会員情報がネット上で閲覧可能に - ファイル転送時にミス](https://www.security-next.com/190486) | 22.0 | 20.0 | 42.0 |
| [OpenAIのHugging Face攻撃事件などで調査を担当しているAI監査組織「METR」とは何なのか？](https://gigazine.net/news/20260917-model-evaluation-and-threat-research/) | 22.0 | 20.0 | 42.0 |
| [不正アクセスで約771万件の個人情報が流出 - ムラウチドットコム](https://www.security-next.com/190439) | 22.0 | 20.0 | 42.0 |
| [アメリカの戦略石油備蓄を支える「驚くほど洗練されていてシンプル」な工学的解決策とは？](https://gigazine.net/news/20260917-engineering-behind-us-strategic-petroleum-reserve/) | 22.0 | 20.0 | 42.0 |
| [熊本県の就職移住支援サイトが改ざん - 偽警告でサブスクアプリに誘導](https://www.security-next.com/190205) | 22.0 | 20.0 | 42.0 |
| [従業員アカウントが侵害、なりすましメールが送信 - ホテル運営会社](https://www.security-next.com/189987) | 22.0 | 20.0 | 42.0 |
| [Mozilla、「Firefox 156」をリリース - 脆弱性73件に対応](https://www.security-next.com/190462) | 22.0 | 20.0 | 42.0 |
| [ドローン攻撃を受けたAWS中東データセンター、半年の復旧作業の末に「一部データは回復不能」](https://www.itmedia.co.jp/news/article/2609/17/2000001590/) | 21.0 | 20.0 | 42.0 |
| [Bransys ELDの脆弱性とセキュリティリスク](https://www.cisa.gov/news-events/ics-advisories/icsa-26-260-01) | 20.0 | 28.0 | 50.0 |
| [Mitsubishi Electric GX Works3およびMotion Control Settingsに関する脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-260-02) | 20.0 | 28.0 | 50.0 |
| [ロンドンの不動産管理会社への侵害で銀行口座情報とロックボックスのコードが漏えいした可能性](https://www.theregister.com/security/2026/09/17/london-property-manager-breach-may-have-exposed-bank-details-and-lockbox-codes/5297232) | 20.0 | 20.0 | 48.0 |
| [Flockカメラは車両だけでなく人も追跡している](https://www.malwarebytes.com/blog/privacy/2026/09/flock-cameras-are-tracking-people-as-well-as-cars) | 20.0 | 20.0 | 42.0 |
| [2隻の石油タンカーへのサイバー攻撃で沿岸警備隊とFBIが乗船調査](https://www.securityweek.com/cyberattacks-on-two-oil-tankers-prompt-coast-guard-fbi-to-board-vessels/) | 20.0 | 20.0 | 42.0 |
| [ChinaのFamousSparrowハッカー集団、ラテンアメリカを新たなバックドアで標的に](https://therecord.media/china-hackers-latin-america-espionage) | 20.0 | 20.0 | 42.0 |
| [Oracle製品における複数の脆弱性により任意コード実行の可能性](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-oracle-products-could-allow-for-arbitrary-code-execution_2026-097) | 20.0 | 20.0 | 42.0 |
| [FBIと沿岸警備隊、米国水域に入港する船舶へのサイバー攻撃疑惑を調査](https://www.cybersecuritydive.com/news/fbi-coast-guard-probe-cyberattacks-ships-us-waters/830668/) | 20.0 | 20.0 | 42.0 |
| [FamousSparrowがSparrowDoorを新たなSparroWockyバックドアに置き換え](https://www.infosecurity-magazine.com/news/famoussparrow-sparrowocky-latin/) | 20.0 | 20.0 | 42.0 |
| [US Coast GuardとFBIが油槽船を捜索、サイバー攻撃を調査](https://www.bitdefender.com/en-us/blog/hotforsecurity/us-coast-guard-fbi-board-oil-tanker-investigate-cyber-attack) | 20.0 | 20.0 | 42.0 |
| [CISAがリスク重視へ移行し週次脆弱性速報を終了](https://www.securityweek.com/cisa-retires-weekly-vulnerability-bulletin-in-risk-based-pivot/) | 20.0 | 20.0 | 42.0 |
| [Revolutのデータ漏えい後にフィッシングSMSが相次ぐ](https://www.malwarebytes.com/blog/threat-intel/2026/09/revolut-phishing-texts-appear-days-after-data-breach) | 20.0 | 20.0 | 42.0 |
| [CISAが重要インフラにネットワーク内へデコイの設置を促す](https://www.infosecurity-magazine.com/news/cisa-critical-infrastructure-cyber/) | 20.0 | 20.0 | 42.0 |
| [Revolutのデータ侵害：5か月間で680件の高プロフィールアカウントが被害、300万ドルの身代金要求](https://www.securityweek.com/revolut-data-breach-5-months-680-high-profile-accounts-3m-ransom/) | 20.0 | 20.0 | 42.0 |
| [ロシアの選挙システムが侵害されたとハッカーが主張、議会選挙を数日前に控え](https://therecord.media/russia-election-hackers-breach) | 20.0 | 20.0 | 42.0 |
| [製造業者はパッチ適用を進めるも、ID管理は依然として大きな弱点](https://www.cybersecuritydive.com/news/manufacturing-cybersecurity-weaknesses-ransomware-black-kite/830299/) | 20.0 | 20.0 | 42.0 |
| [最近の自殺死亡を受けたCyber Commandへの新たな支援を検討する議会](https://therecord.media/congress-eyes-support-for-cyber-command-suicide-deaths) | 20.0 | 20.0 | 42.0 |
| [IranによるAWS施設への攻撃でバーレーンとUAEの顧客データが復旧不能に](https://www.helpnetsecurity.com/2026/09/17/aws-middle-east-outage-permanent-data-loss-bahrain-uae/) | 20.0 | 20.0 | 42.0 |
| [CISAが重要インフラ組織や小規模セキュリティチームにサイバーおとりの活用を促す](https://www.helpnetsecurity.com/2026/09/17/cisa-guidance-for-implementing-cyber-decoys/) | 20.0 | 20.0 | 42.0 |
| [ISC、BIND 9のセキュリティアップデートで14件の脆弱性を修正](https://www.securityweek.com/isc-patches-14-vulnerabilities-in-bind-9-security-update/) | 20.0 | 20.0 | 42.0 |
| [Cyber Essentialsは過去最多を記録も、導入率は依然低い](https://www.infosecurity-magazine.com/news/cyber-essentials-has-record-year/) | 20.0 | 20.0 | 42.0 |
| [アドバーサリーシミュレーションで知っておくべきこと](https://www.ncsc.gov.uk/guidance/adversary-simulation-what-you-need-to-know) | 20.0 | 20.0 | 42.0 |
| [Cyber Adversary Simulation（CyAS）のスキーム文書が公開されました](https://www.ncsc.gov.uk/blogs/cyber-adversary-simulation-cyas-scheme-documents-now-available) | 20.0 | 20.0 | 42.0 |
| [新しいCVEが攻撃者より先に悪用可能かを証明する方法を学ぶウェビナー](https://thehackernews.com/2026/09/can-you-prove-new-cve-is-exploitable.html) | 20.0 | 20.0 | 42.0 |
| [FBIが長期運営されたDDoS代行サービスを摘発](https://www.helpnetsecurity.com/2026/09/17/fbi-nightmarestresser-ddos-for-hire-service-seized/) | 20.0 | 20.0 | 42.0 |
| [米国、DDoS請負サービス「NightmareStresser」を摘発](https://www.bleepingcomputer.com/news/security/fbi-seizes-nightmarestresser-service-linked-to-thousands-of-ddos-attacks/) | 20.0 | 20.0 | 42.0 |
| [テスト環境の不備により誰でも本番の顧客データにアクセス可能だった問題](https://www.theregister.com/security/2026/09/17/test-environment-let-anyone-access-live-customer-data/5296977) | 20.0 | 20.0 | 42.0 |
| [マンハッタン地区検事局、12の有名人ディープフェイクサイトを押収](https://www.malwarebytes.com/blog/ai/2026/09/12-celebrity-deepfake-websites-seized-by-manhattan-da) | 20.0 | 20.0 | 42.0 |
| [OfcomがOnline Safety Actの罰金を科すのは取り立てるより容易だと判明](https://www.theregister.com/security/2026/09/17/ofcom-discovers-issuing-online-safety-act-fines-is-easier-than-collecting-them/5297110) | 20.0 | 20.0 | 42.0 |
| [米国のサイバー戦略は、軍の機動を支える実際のインフラを見落としている](https://cyberscoop.com/us-cyber-strategy-iranian-threats-infrastructure-op-ed/) | 20.0 | 20.0 | 42.0 |
| [MicrosoftがWindowsのドメインログイン問題の回避策を公開](https://www.bleepingcomputer.com/news/microsoft/microsoft-releases-workaround-for-windows-domain-login-authentication-issues/) | 20.0 | 20.0 | 42.0 |

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
