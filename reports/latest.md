# 📡 サイレーダー 2026-05-13 07:02 JST 試作版

このレポートは、2026-05-12 19:01 JST〜2026-05-13 07:01 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 254
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 10
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks](#topic-216) | 100.0 | 99.0 | 92.0 | GitHub | fatigue_or_recently_covered |
| 2 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 74.0 | 82.0 | 81.0 | 音声 | 温度感上位枠 |
| 3 | [Microsoft 2026年5月 Patch Tuesday 関連まとめ](#topic-3472) | 74.0 | 56.0 | 58.0 | GitHub | fatigue_or_recently_covered |
| 4 | [Multiple Vulnerabilities in Fortinet Products Could Allow for Remote Code Execution](#topic-3622) | 61.0 | 66.0 | 43.0 | GitHub | fatigue_or_recently_covered |
| 5 | [Adobe Patches 52 Vulnerabilities in 10 Products](#topic-3486) | 37.0 | 38.0 | 43.0 | GitHub | fatigue_or_recently_covered |
| 6 | [ABB Automation Builder Gateway for Windows](#topic-3527) | 36.0 | 46.0 | 50.0 | GitHub | fatigue_or_recently_covered |
| 7 | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](#topic-31) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 8 | [How Rapid7 is bringing Cyber GRC closer to security operations](#topic-3512) | 35.0 | 30.0 | 43.0 | GitHub | fatigue_or_recently_covered |
| 9 | [What is Cyber GRC? How Rapid7 is bringing compliance closer to security operations](#topic-3517) | 35.0 | 30.0 | 43.0 | GitHub | fatigue_or_recently_covered |
| 10 | [TanStack, Mistral AI, UiPath Hit in Fresh Supply Chain Attack](#topic-3549) | 33.0 | 20.0 | 42.0 | GitHub | fatigue_or_recently_covered |
| 11 | [ランサム攻撃でシステム障害、一部業務に影響 - 医薬品卸](#topic-3513) | 30.0 | 30.0 | 42.0 | GitHub | fatigue_or_recently_covered |
| 12 | [Threats Making WAVs - Incident Response to a Cryptomining Attack](#topic-29) | 30.0 | 20.0 | 42.0 | GitHub | fatigue_or_recently_covered |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-12"></a>

### 1. Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>Windows</nobr> / <nobr>権限昇格</nobr> / <nobr>TTP</nobr> / <nobr>脆弱性</nobr> / <nobr>KEV</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 74.0 |
| <nobr>実務影響</nobr> | 82.0 |
| <nobr>確度</nobr> | 81.0 |

#### 概要

CVE-2025-60710は、Microsoft WindowsのTaskhost関連の処理におけるローカル権限昇格の脆弱性とされています。
CISAのKnown Exploited Vulnerabilitiesに含まれており、公開PoCや検証コードの言及もあるため、実運用環境での優先確認対象とみられます。
権限昇格は、初期侵入後に管理者権限へ到達される足がかりになり得るため、影響が大きい類型です。加えて、既知悪用リストに掲載されている点は、放置した場合のリスクを高めます。

#### CISA KEV詳細

- **CVE**: CVE-2025-60710
- **Vendor / Project**: Microsoft
- **Product**: Windows
- **Vulnerability Name**: Microsoft Windows Link Following Vulnerability
- **Date Added**: 2026-04-13
- **Due Date**: 2026-04-27
- **Known Ransomware Use**: Unknown

**Required Action**

> Apply mitigations per vendor instructions, follow applicable BOD 22-01 guidance for cloud services, or discontinue use of the product if mitigations are unavailable.

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- CISA KEV関連。
- 公開PoC・検証コード言及あり。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 公開PoCにより再現・悪用可能性が上がる。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 公開PoC・検証コード言及あり。
- 公開PoC/Exploitコード: 確認あり。
- 直接PoCリンク: 掲載しません。
- 確認方針: NVD、ベンダー公式、公的機関、信頼できる技術分析を優先し、GitHub等のコードは防御・検証目的で別途確認します。

#### 担当者向け確認ポイント

- 対象Windows環境での該当CVEの修正状況を確認し、未適用なら優先的に対処する。
- Taskhost関連の異常な挙動や、不審なローカル権限変化の監視を強化する。
- 公開PoCの存在を前提に、関連システムの露出と権限分離の見直しを行う。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-60710 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 影響ベンダー | 1.00 |
| 製品 | Windows | 影響製品 | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-60710](https://nvd.nist.gov/vuln/detail/CVE-2025-60710) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>公的機関</nobr> | [CISA KEV: CVE-2025-60710](https://www.cisa.gov/known-exploited-vulnerabilities-catalog?field_cve=CVE-2025-60710) | <nobr>KEV掲載内容、Date Added、Due Date、Required Action</nobr> |
| <nobr>公的機関データ</nobr> | [CISA KEV JSON](https://www.cisa.gov/sites/default/files/feeds/known_exploited_vulnerabilities.json) | <nobr>CISA公式の機械可読データ。CVE IDで検索して確認</nobr> |
| <nobr>出典</nobr> | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](https://github.com/Wh04m1001/CVE-2025-60710) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。
- 継続観測: 継続。

---

<a id="topic-31"></a>

### 2. PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>防御・運用</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers に関する脅威・攻撃キャンペーン系の話題です。
攻撃者、標的、TTP、IoC、悪用技術、検知観点を中心に確認する価値があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 標的OS、仮想化基盤、暗号化対象、バックアップ影響を確認する。
- 初期侵入、横展開、認証情報窃取、永続化のTTPを確認する。
- EDR/SIEMで検知すべきIoCや振る舞いを確認する。
- ESXi、vCenter、バックアップ基盤、特権アカウントの保護状況を確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](https://akamai.com/blog/security/please-read-me-opportunistic-ransomware-devastating-mysql-servers) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 未評価。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-216"></a>

### 1. CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>KEV</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>マルウェア</nobr> / <nobr>認証バイパス</nobr> / <nobr>脅威レポート</nobr> / <nobr>ボットネット</nobr> / <nobr>ランサムウェア</nobr> / <nobr>脅威アクター</nobr> |
| <nobr>温度状態</nobr> | 高温 |
| <nobr>温度感</nobr> | 100.0 |
| <nobr>実務影響</nobr> | 99.0 |
| <nobr>確度</nobr> | 92.0 |

#### 概要

cPanel & WHMに影響する認証回避の脆弱性CVE-2026-41940が、実際の攻撃で悪用されていると複数の公開情報で報告されています。
関連報道では、ランサムウェア文脈やバックドア展開につながる事例、さらに一部地域の組織やホスティング事業者を狙った動きが示されています。
管理系の認証を迂回されると、対象サーバーの設定やデータ、配下サイトに広く影響が及ぶおそれがあります。
公開PoCの言及もあり、対応の遅れが被害拡大につながりやすい点が注目されています。

#### CISA KEV詳細

- **CVE**: CVE-2026-41940
- **Vendor / Project**: WebPros
- **Product**: cPanel & WHM and WP2 (WordPress Squared)
- **Vulnerability Name**: WebPros cPanel & WHM and WP2 (WordPress Squared) Missing Authentication for Critical Function Vulnerability
- **Date Added**: 2026-04-30
- **Due Date**: 2026-05-03
- **Known Ransomware Use**: Known

**Required Action**

> Apply mitigations per vendor instructions, follow applicable BOD 22-01 guidance for cloud services, or discontinue use of the product if mitigations are unavailable.

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
- CISA KEV関連。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

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

#### 攻撃・悪用観測シグナル

- シグナル種別: 公開PoC・検証コード言及あり。
- 公開PoC/Exploitコード: 確認あり。
- 直接PoCリンク: 掲載しません。
- 確認方針: NVD、ベンダー公式、公的機関、信頼できる技術分析を優先し、GitHub等のコードは防御・検証目的で別途確認します。

#### 担当者向け確認ポイント

- cPanel & WHMおよび関連製品の利用有無を確認し、ベンダー案内に沿って緊急対応を進める。
- 管理画面への不審なログインや設定変更、ファイル追加などの痕跡を点検する。
- ホスティング基盤や周辺システムを含め、認証情報の再点検と監視強化を行う。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-41940 | 主要CVE | 1.00 |
| ベンダー | WebPros | 影響ベンダー | 1.00 |
| 製品 | cPanel & WHM and WP2 (WordPress Squared) | 影響製品 | 1.00 |
| 脆弱性 | CVE-2026-26268 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-42208 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2023-1389 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-41940](https://nvd.nist.gov/vuln/detail/CVE-2026-41940) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>公的機関</nobr> | [CISA KEV: CVE-2026-41940](https://www.cisa.gov/known-exploited-vulnerabilities-catalog?field_cve=CVE-2026-41940) | <nobr>KEV掲載内容、Date Added、Due Date、Required Action</nobr> |
| <nobr>公的機関データ</nobr> | [CISA KEV JSON](https://www.cisa.gov/sites/default/files/feeds/known_exploited_vulnerabilities.json) | <nobr>CISA公式の機械可読データ。CVE IDで検索して確認</nobr> |
| <nobr>出典</nobr> | [Stealthy hackers exploit cPanel flaw in active backdoor campaign (CVE-2026-41940](https://helpnetsecurity.com/2026/05/12/cpanel-vulnerability-exploited-backdoor-cve-2026-41940) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [cPanel CVE-2026-41940 Under Active Exploitation to Deploy Filemanager Backdoor](https://thehackernews.com/2026/05/cpanel-cve-2026-41940-under-active.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Week in review: cPanel vulnerability actively exploited, DigiCert breach, Linked](https://helpnetsecurity.com/2026/05/10/week-in-review-cpanel-vulnerability-actively-exploited-digicert-breach-linkedin-job-scams) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [4th May – Threat Intelligence Report](https://research.checkpoint.com/2026/4th-may-threat-intelligence-report) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [South-East Asian Military Entities Targeted via cPanel (CVE-2026-41940)](https://ctrlaltintel.com/research/SEA-CPanel) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 弱。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。
- 継続観測: 継続。

---

<a id="topic-3472"></a>

### 2. Microsoft 2026年5月 Patch Tuesday 関連まとめ

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>RCE</nobr> / <nobr>Windows</nobr> / <nobr>クラウド</nobr> / <nobr>DDoS</nobr> / <nobr>AI</nobr> / <nobr>Android</nobr> / <nobr>脅威アクター</nobr> / <nobr>IoC</nobr> |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 74.0 |
| <nobr>実務影響</nobr> | 56.0 |
| <nobr>確度</nobr> | 58.0 |

#### 概要

Microsoftの2026年5月のPatch Tuesdayでは、120件超のCVE修正が公開されました。
現時点で公に悪用が確認されたものやゼロデイは含まれていないとされていますが、Microsoft Wordの複数の深刻なRCE脆弱性を含め、優先度の高い修正が複数あります。
件数が多く、影響範囲も広いため、通常の月次更新より計画的な対応が求められます。
特に文書ファイル経由での侵入リスクがあるため、エンドポイントやメール経由の受け口を持つ環境では注意が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 7 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 中。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Microsoft Word関連の深刻なRCE修正を優先して適用する。
- 通常の月次パッチ運用に加え、影響の大きい製品群の適用状況を早めに確認する。
- Windows 10の拡張セキュリティ更新対象を含む端末では、該当する更新が確実に入っているか点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-28943 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40364 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40397 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40398 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-41096 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-41089 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-42898 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40415 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-35435 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-35428 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [It's Patch Tuesday for Microsoft and Not a Zero-Day In Sight](https://darkreading.com/application-security/patch-tuesday-microsoft-zero-day-sight) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft addresses 137 vulnerabilities in May’s Patch Tuesday, including 13 rat](https://cyberscoop.com/microsoft-patch-tuesday-may-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patch Tuesday for May 2026 — Snort rules and prominent vulnerabilities](https://blog.talosintelligence.com/microsoft-patch-tuesday-may-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft May 2026 Patch Tuesday: Many fixes, but no zero-days](https://helpnetsecurity.com/2026/05/12/microsoft-may-2026-patch-tuesday) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft releases Windows 10 KB5087544 extended security update](https://bleepingcomputer.com/news/microsoft/microsoft-releases-windows-10-kb5087544-extended-security-update) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [The May 2026 Security Update Review](https://thezdi.com/blog/2026/5/12/the-may-2026-security-update-review) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft May 2026 Patch Tuesday, (Tue, May 12th)](https://isc.sans.edu/diary/rss/32980) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft May 2026 Patch Tuesday fixes 120 flaws, no zero-days](https://bleepingcomputer.com/news/microsoft/microsoft-may-2026-patch-tuesday-fixes-120-flaws-no-zero-days) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 中。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 継続。

---

<a id="topic-3622"></a>

### 3. Multiple Vulnerabilities in Fortinet Products Could Allow for Remote Code Execution

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>RCE</nobr> / <nobr>脆弱性</nobr> / <nobr>防御・運用</nobr> / <nobr>ゼロデイ</nobr> / <nobr>ランサムウェア</nobr> / <nobr>マルウェア</nobr> / <nobr>クラウド</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 61.0 |
| <nobr>実務影響</nobr> | 66.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Fortinet製品に複数の脆弱性が見つかっており、最も深刻なものではリモートコード実行につながる可能性があるとされています。
対象にはFortiAuthenticatorやFortiSandboxが含まれており、悪用された場合はシステム上で任意の操作が行われるおそれがあります。
認証や脅威検知に関わる製品が影響を受ける可能性があるため、組織の境界防御や運用基盤に直接関係します。悪用が確認されている文脈もあり、優先度を上げて確認すべき話題です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Fortinet製品の利用有無と対象バージョンを確認し、ベンダー案内に沿って更新・緩和策の適用状況を点検する。
- FortiAuthenticatorなど認証基盤に関わる製品は影響範囲が広くなりやすいため、管理権限の見直しと監視強化を行う。
- 関連製品のログや異常な管理操作、予期しないプロセス起動など、侵害の兆候がないかを確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Fortinet | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Multiple Vulnerabilities in Fortinet Products Could Allow for Remote Code Execut](https://cisecurity.org/advisory/multiple-vulnerabilities-in-fortinet-products-could-allow-for-remote-code-execution_2026-049) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 未評価。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 初出。

---

<a id="topic-3486"></a>

### 4. Adobe Patches 52 Vulnerabilities in 10 Products

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>RCE</nobr> / <nobr>KEV</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Adobe Patches 52 Vulnerabilities in 10 Products に関する脆弱性情報です。
では英語本文の全文翻訳は行わず、参照リンク、関連する対象、スコア根拠を中心に整理しています。詳細はベンダー公式情報、公的機関情報、NVD等を確認してください。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 自組織で対象製品・関連資産を利用しているか確認する。
- ベンダー公式情報または公的機関情報を優先確認する。
- 対象バージョンか確認する。
- 修正版・緩和策の適用状況を確認する。
- インターネット露出の有無を確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Adobe Patches 52 Vulnerabilities in 10 Products](https://securityweek.com/adobe-patches-52-vulnerabilities-in-10-products) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 未評価。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 初出。

---

<a id="topic-3527"></a>

### 5. ABB Automation Builder Gateway for Windows

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>防御・運用</nobr> / <nobr>Windows</nobr> / <nobr>政策・規制</nobr> / <nobr>TTP</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 46.0 |
| <nobr>確度</nobr> | 50.0 |

#### 概要

ABB Automation Builder Gateway for Windows に関する脆弱性情報です。
では英語本文の全文翻訳は行わず、参照リンク、関連する対象、スコア根拠を中心に整理しています。詳細はベンダー公式情報、公的機関情報、NVD等を確認してください。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 自組織で対象製品・関連資産を利用しているか確認する。
- ベンダー公式情報または公的機関情報を優先確認する。
- 対象バージョンか確認する。
- 修正版・緩和策の適用状況を確認する。
- インターネット露出の有無を確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2024-41975 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2024-41975](https://nvd.nist.gov/vuln/detail/CVE-2024-41975) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [ABB Automation Builder Gateway for Windows](https://cisa.gov/news-events/ics-advisories/icsa-26-132-04) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-3512"></a>

### 6. How Rapid7 is bringing Cyber GRC closer to security operations

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>政策・規制</nobr> / <nobr>防御・運用</nobr> / <nobr>CISO・組織運営</nobr> / <nobr>サプライチェーン</nobr> / <nobr>脆弱性</nobr> / <nobr>AI</nobr> / <nobr>KEV</nobr> / <nobr>AIエージェント</nobr> / <nobr>TTP</nobr> / <nobr>脅威レポート</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 35.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

How Rapid7 is bringing Cyber GRC closer to security operations は、AIを攻撃者側の自動化・詐欺・マルウェア・フィッシングに利用する話題です。
攻撃手口、標的、検知観点、利用者教育やSOC監視への反映要否を確認する価値があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 攻撃者がAIを使っている工程と、既存の検知・教育で補足できる範囲を確認する。
- フィッシング、マルウェア、詐欺テンプレート、認証情報窃取の観点で検知ロジックを確認する。
- SOC/CSIRTで共有すべきIoC、TTP、注意喚起文面があるか確認する。
- 利用者向け注意喚起や訓練内容を更新する必要があるか確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [How Rapid7 is bringing Cyber GRC closer to security operations](https://rapid7.com/blog/post/cds-rapid7-cyber-grc-secops-compliance) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 初出。

---

<a id="topic-3517"></a>

### 7. What is Cyber GRC? How Rapid7 is bringing compliance closer to security operations

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>政策・規制</nobr> / <nobr>防御・運用</nobr> / <nobr>CISO・組織運営</nobr> / <nobr>サプライチェーン</nobr> / <nobr>脆弱性</nobr> / <nobr>AI</nobr> / <nobr>KEV</nobr> / <nobr>AIエージェント</nobr> / <nobr>TTP</nobr> / <nobr>脅威レポート</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 35.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

What is Cyber GRC? How Rapid7 is bringing compliance closer to security operations は、AIを攻撃者側の自動化・詐欺・マルウェア・フィッシングに利用する話題です。
攻撃手口、標的、検知観点、利用者教育やSOC監視への反映要否を確認する価値があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 攻撃者がAIを使っている工程と、既存の検知・教育で補足できる範囲を確認する。
- フィッシング、マルウェア、詐欺テンプレート、認証情報窃取の観点で検知ロジックを確認する。
- SOC/CSIRTで共有すべきIoC、TTP、注意喚起文面があるか確認する。
- 利用者向け注意喚起や訓練内容を更新する必要があるか確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [What is Cyber GRC? How Rapid7 is bringing compliance closer to security operatio](https://rapid7.com/blog/post/so-cyber-grc-how-rapid7-brings-compliance-to-security-operations) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 初出。

---

<a id="topic-3549"></a>

### 8. TanStack, Mistral AI, UiPath Hit in Fresh Supply Chain Attack

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>サプライチェーン</nobr> / <nobr>AI</nobr> / <nobr>攻撃キャンペーン</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

TanStack, Mistral AI, UiPath Hit in Fresh Supply Chain Attack は、ソフトウェアサプライチェーンを悪用した攻撃・侵害キャンペーン系の話題です。
影響するパッケージ、依存関係、開発環境、CI/CD、配布経路、認証情報や保守者アカウントの悪用有無を中心に確認する価値があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 影響するパッケージ、製品、依存関係を確認する。
- SBOM、lockfile、CI/CD、開発者端末への影響を確認する。
- 配布元、署名、ハッシュ、更新履歴の妥当性を確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ai_model_or_project | Mistral | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [TanStack, Mistral AI, UiPath Hit in Fresh Supply Chain Attack](https://securityweek.com/tanstack-mistral-ai-uipath-hit-in-fresh-supply-chain-attack) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-3513"></a>

### 9. ランサム攻撃でシステム障害、一部業務に影響 - 医薬品卸

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | - |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

医薬品や医療機器の卸売り事業を手がけるマルタケは、サイバー攻撃によりシステム障害が発生し、一部事業に影響が生じていることを明らかにした。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 標的OS、仮想化基盤、暗号化対象、バックアップ影響を確認する。
- 初期侵入、横展開、認証情報窃取、永続化のTTPを確認する。
- EDR/SIEMで検知すべきIoCや振る舞いを確認する。
- ESXi、vCenter、バックアップ基盤、特権アカウントの保護状況を確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [ランサム攻撃でシステム障害、一部業務に影響 - 医薬品卸](https://security-next.com/184285) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 未評価。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-29"></a>

### 10. Threats Making WAVs - Incident Response to a Cryptomining Attack

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>防御・運用</nobr> / <nobr>マルウェア</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Threats Making WAVs - Incident Response to a Cryptomining Attack に関するインシデント・侵害報道系の話題です。
影響範囲、原因、復旧状況、利用者影響、追加公表の有無を中心に確認する価値があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 被害組織、影響範囲、利用者影響を確認する。
- 原因、侵入経路、復旧状況、追加公表の有無を確認する。
- 自組織で類似構成・類似委託先・類似サービス利用がないか確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Threats Making WAVs - Incident Response to a Cryptomining Attack](https://akamai.com/blog/security/threats-making-wavs-incident-reponse-cryptomining-attack) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 未評価。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [サードパーティ侵害を通じたステルス侵入の調査](https://microsoft.com/en-us/security/blog/2026/05/12/undermining-the-trust-boundary-investigating-a-stealthy-intrusion-through-third-party-compromise) | 30.0 | 20.0 | 42.0 |
| [UniFi Accessにおけるリモートコード実行の脆弱性（CVE-2025-52665）](https://catchify.sa/post/cve-2025-52665-rce-in-unifi-os-25-000) | 28.0 | 46.0 | 50.0 |
| [ABB AC500 V3 の Cryptographic Message Syntax におけるスタックバッファオーバーフロー](https://cisa.gov/news-events/ics-advisories/icsa-26-132-05) | 28.0 | 46.0 | 50.0 |
| [ABB AC500 V3の複数の脆弱性](https://cisa.gov/news-events/ics-advisories/icsa-26-132-03) | 28.0 | 46.0 | 50.0 |
| [CVE-2026-40358: Microsoft Officeのリモートコード実行の脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-40358) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-35422 Windows TCP/IP Driverのセキュリティ機能バイパス脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-35422) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-42898 Microsoft Dynamics 365 On-Premisesのリモートコード実行脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-42898) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-33112 Microsoft SharePoint Serverのリモートコード実行脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-33112) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-42893 Microsoft Outlook for iOSの改ざん脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-42893) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-40368 Microsoft SharePoint Serverのリモートコード実行の脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-40368) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-40359 Microsoft Excelのリモートコード実行脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-40359) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-40415 Windows TCP/IP リモートコード実行の脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-40415) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-35439 Microsoft SharePoint Server のリモートコード実行の脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-35439) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-40367 Microsoft Wordのリモートコード実行の脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-40367) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-35421 Windows GDIのリモートコード実行の脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-35421) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-34332 Windows Kernel-Mode Driverのリモートコード実行脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-34332) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-42831 Microsoft Officeのリモートコード実行脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-42831) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-40366 Microsoft Wordのリモートコード実行の脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-40366) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-40380 Windows Volume Manager Extension Driverのリモートコード実行脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-40380) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-33110 Microsoft SharePoint Serverのリモートコード実行脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-33110) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-34329 Microsoft Message Queuing (MSMQ) のリモートコード実行脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-34329) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-40362 Microsoft Excel リモートコード実行の脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-40362) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-41094 Microsoft Data Formulatorのリモートコード実行の脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-41094) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-42833 Microsoft Dynamics 365 On-Premises のリモートコード実行の脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-42833) | 28.0 | 46.0 | 38.0 |

---

## 📊 スコアの見方

| <nobr>指標</nobr> | 意味 |
|---|---|
| <nobr>温度状態</nobr> | 話題のライフサイクルを示す補助ラベルです。例: 低温、継続監視、温度上昇中、高温、冷却中。 |
| <nobr>温度感</nobr> | 話題として今どれだけ注目・拡散・更新されているかを示します。 |
| <nobr>実務影響</nobr> | 対象組織・担当者にとって、対応優先度や被害可能性がどれだけ大きいかを示します。 |
| <nobr>確度</nobr> | 公的機関、ベンダー公式、複数ソース、CVE/KEV、一次資料などにより、情報をどれだけ確認できているかを示します。事件報道系は、複数報道があっても司法文書・当局発表などの一次資料が弱い場合、脆弱性KEV系より低く出ることがあります。 |

スコアは、公開情報から抽出した特徴量と事前定義した重み付けに基づく参考指標です。詳しい算出方針は [スコアリング方針](../docs/scoring.md) を参照してください。

## 🔒 公開しない内部情報について

サイレーダーでは、温度感の補助シグナルとして、公的機関・ベンダー公式・信頼できる報道機関・技術者コミュニティ・国内外の公開反応などを利用します。

これらのシグナルは、一次情報、報道波及、技術者反応、開発者反応、PoC・悪用観測などに分けて評価します。

ただし、ランキング操作、スパム的誘導、監視回避を防ぐため、個別の監視対象、取得手段、検索条件、評価対象サービス名、内部的な重み付けやしきい値は公開しません。

また、公開反応の多さだけで掲載順位を決めることはありません。重要度の判定では、ベンダー公式情報、公的機関、一次資料、信頼できる技術分析、実務影響を優先します。

## ⚠️ 注意事項

このレポートは、収集・観測できた公開情報をもとにした参考情報です。完全性、正確性、即時性を保証するものではありません。

重要な判断を行う場合は、必ずベンダー公式情報、公的機関、一次情報を確認してください。

サイレーダーは、広告・スポンサー・企業関係に基づいて掲載順位や温度感スコアを変更しません。
