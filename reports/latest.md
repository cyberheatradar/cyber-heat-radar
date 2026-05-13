# 📡 サイレーダー 2026-05-13 09:23 JST 試作版

このレポートは、2026-05-13 03:22 JST〜2026-05-13 09:22 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 106
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 3
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [PAN-OSに深刻な脆弱性「CVE-2026-0300」発覚 root権限奪取の恐れ](#topic-345) | 100.0 | 96.0 | 91.0 | GitHub | 直近掲載済み・再掲抑制 |
| 2 | [Microsoft 2026年5月 Patch Tuesday 関連まとめ](#topic-3472) | 76.0 | 56.0 | 58.0 | GitHub | 直近掲載済み・再掲抑制 |
| 3 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 74.0 | 82.0 | 81.0 | 音声 | 温度感上位枠 |
| 4 | [Multiple Vulnerabilities in Fortinet Products Could Allow for Remote Code Execution](#topic-3622) | 61.0 | 66.0 | 43.0 | GitHub | 直近掲載済み・再掲抑制 |
| 5 | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](#topic-31) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [Threats Making WAVs - Incident Response to a Cryptomining Attack](#topic-29) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

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

CVE-2025-60710は、Microsoft WindowsのTaskhost関連で発生するローカル権限昇格の脆弱性として報告されています。
公開情報では、CISAのKnown Exploited Vulnerabilitiesに含まれており、実際に悪用されている脆弱性として優先対応が必要とされています。
権限昇格につながる脆弱性は、侵入後の被害拡大や管理者権限の奪取に直結しやすいため注意が必要です。
さらに公開PoCの存在が示されているため、影響範囲の確認と対策の優先度が上がります。

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

- 対象のWindows環境でCVE-2025-60710の修正状況を確認し、未適用なら速やかに更新を検討する。
- 権限昇格の兆候がないか、Taskhost関連の不審な挙動や管理者権限取得の痕跡を点検する。
- CISA KEV掲載のため、通常の脆弱性対応より優先度を上げて資産棚卸しと影響評価を行う。

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

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
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

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-29"></a>

### 3. Threats Making WAVs - Incident Response to a Cryptomining Attack

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>防御・運用</nobr> / <nobr>マルウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
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

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-345"></a>

### 1. PAN-OSに深刻な脆弱性「CVE-2026-0300」発覚 root権限奪取の恐れ

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>KEV</nobr> / <nobr>RCE</nobr> / <nobr>ゼロデイ</nobr> / <nobr>国家支援</nobr> / <nobr>防御・運用</nobr> / <nobr>脅威アクター</nobr> / <nobr>IoC</nobr> / <nobr>政策・規制</nobr> |
| <nobr>温度状態</nobr> | 高温 |
| <nobr>温度感</nobr> | 100.0 |
| <nobr>実務影響</nobr> | 96.0 |
| <nobr>確度</nobr> | 91.0 |

#### 概要

Palo Alto NetworksのPAN-OSに、認証不要でリモートコード実行につながる可能性がある重大な脆弱性「CVE-2026-0300」が公表されました。
対象はPA-SeriesとVM-Seriesの一部で、User-ID Authentication Portalが有効な構成で影響を受けるとされています。
ベンダーは実際の悪用を確認しており、CISAのKEVにも追加されています。
ファイアウォール製品は社内外の境界に置かれることが多く、侵害されると影響が広範囲に及ぶおそれがあります。
しかも本件は既に悪用が観測されているため、対応の優先度が高い脆弱性といえます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 10 sources。
- CISA KEV関連。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 自組織のPAN-OS機器でUser-ID Authentication Portalが有効かどうかを確認する。
- 修正版の提供状況を確認し、適用可能になり次第すぐ更新計画を進める。
- 当面はベンダー推奨の回避策に従い、ポータルへのアクセスを信頼できる範囲に制限するか、不要なら無効化する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-0300 | 主要CVE | 1.00 |
| ベンダー | Palo Alto Networks | 影響ベンダー | 1.00 |
| 製品 | PAN-OS | 影響製品 | 1.00 |
| ベンダー | Palo Alto | 言及あり | 0.80 |
| 製品 | Active Directory | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-0300](https://nvd.nist.gov/vuln/detail/CVE-2026-0300) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [PAN-OSに深刻な脆弱性「CVE-2026-0300」発覚　root権限奪取の恐れ](https://atmarkit.itmedia.co.jp/ait/articles/2605/13/news034.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PAN-OS RCE Exploit Under Active Use Enabling Root Access and Espionage](https://thehackernews.com/2026/05/pan-os-rce-exploit-under-active-use.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [State-sponsored hackers likely behind zero-day attacks on Palo Alto firewalls](https://helpnetsecurity.com/2026/05/07/state-sponsored-hackers-zero-day-attacks-palo-alto-firewalls) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0300 PAN-OS: Unauthenticated user initiated Buffer Overflow Vulnerabili](https://security.paloaltonetworks.com/CVE-2026-0300) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: Exploitation of PAN-OS Captive Portal Zero-Day for Unauthenticated](https://unit42.paloaltonetworks.com/captive-portal-zero-day) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [A critical Palo Alto PAN-OS zero-day is being exploited in the wild](https://cyberscoop.com/palo-alto-networks-pan-os-firewall-zero-day-vulnerability-exploited) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Buffer Overflow in Palo Alto Networks PAN-OS User-ID Authentication Por](https://rapid7.com/blog/post/etr-critical-buffer-overflow-in-palo-alto-networks-pan-os-user-id-authentication-portal-cve-2026-0300) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 弱。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 継続。

---

<a id="topic-3472"></a>

### 2. Microsoft 2026年5月 Patch Tuesday 関連まとめ

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>RCE</nobr> / <nobr>Windows</nobr> / <nobr>クラウド</nobr> / <nobr>AI</nobr> / <nobr>DDoS</nobr> / <nobr>Android</nobr> / <nobr>脅威アクター</nobr> / <nobr>防御・運用</nobr> |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 76.0 |
| <nobr>実務影響</nobr> | 56.0 |
| <nobr>確度</nobr> | 58.0 |

#### 概要

Microsoftの2026年5月のPatch Tuesdayでは、120件超のCVE修正が公開されました。
現時点で広く確認されたゼロデイや公表済みの悪用はないとされますが、Microsoft Wordに関する複数の重要なRCE脆弱性など、優先度を上げて対応したい項目が含まれています。
件数が多いだけでなく、業務利用の多い製品に深刻度の高い脆弱性が含まれるため、修正の遅れがリスクにつながります。
ゼロデイが見当たらない場合でも、公開後の悪用に備えた通常より速い対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 9 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 強。

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

- Word関連を含む重要度の高い更新を優先し、影響範囲の大きい端末から適用する。
- 通常の月次更新として扱わず、検証後すみやかに展開できるよう社内の適用手順を前倒しで確認する。
- 資産管理と脆弱性管理の観点で、未適用端末や更新失敗端末が残っていないかを重点的に点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-40399 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40364 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40401 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-33096 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40361 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-41096 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-41089 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-42898 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40415 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-35435 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Defense at AI speed: Microsoft’s new multi-model agentic security system tops le](https://microsoft.com/en-us/security/blog/2026/05/12/defense-at-ai-speed-microsofts-new-multi-model-agentic-security-system-finds-16-new-vulnerabilities) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Patch Tuesday, May 2026 Edition](https://krebsonsecurity.com/2026/05/patch-tuesday-may-2026-edition) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [It's Patch Tuesday for Microsoft and Not a Zero-Day In Sight](https://darkreading.com/application-security/patch-tuesday-microsoft-zero-day-sight) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft addresses 137 vulnerabilities in May’s Patch Tuesday, including 13 rat](https://cyberscoop.com/microsoft-patch-tuesday-may-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patch Tuesday for May 2026 — Snort rules and prominent vulnerabilities](https://blog.talosintelligence.com/microsoft-patch-tuesday-may-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft May 2026 Patch Tuesday: Many fixes, but no zero-days](https://helpnetsecurity.com/2026/05/12/microsoft-may-2026-patch-tuesday) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft releases Windows 10 KB5087544 extended security update](https://bleepingcomputer.com/news/microsoft/microsoft-releases-windows-10-kb5087544-extended-security-update) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [The May 2026 Security Update Review](https://thezdi.com/blog/2026/5/12/the-may-2026-security-update-review) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 強。
- 開発者コミュニティ反応: 反応あり。
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

Fortinet製品に複数の脆弱性が見つかり、最も深刻なものではリモートコード実行につながる可能性があるとされています。
対象にはFortiAuthenticatorやFortiSandboxが含まれており、影響が出た場合は権限の範囲に応じて不正な操作や設定変更などのリスクが生じます。
認証や脅威検知に関わる製品が含まれるため、侵害時の影響が大きくなり得ます。公開情報では悪用の文脈も示されているため、優先的な確認対象になっています。

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

- Fortinet製品の利用有無と該当バージョンを確認し、ベンダー情報に基づいて修正の要否を判断する。
- FortiAuthenticatorやFortiSandboxなど、外部から到達し得る管理系サービスの露出状況を見直す。
- 権限の強い管理アカウントの利用状況を点検し、侵害時の影響を抑えるためアクセス制御を再確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Fortinet | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Multiple Vulnerabilities in Fortinet Products Could Allow for Remote Code Execut](https://cisecurity.org/advisory/multiple-vulnerabilities-in-fortinet-products-could-allow-for-remote-code-execution_2026-049) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 初出。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [AI製のゼロデイ攻撃が出現 Googleが報告した高度化する脆弱性探索と自律型攻撃の脅威](https://itmedia.co.jp/enterprise/articles/2605/13/news041.html) | 29.0 | 20.0 | 42.0 |
| [UniFi Access におけるリモートコード実行（CVE-2025-52665）](https://catchify.sa/post/cve-2025-52665-rce-in-unifi-os-25-000) | 28.0 | 46.0 | 50.0 |
| [Netskopeにおけるクロステナント認証バイパス脆弱性](https://blog.amberwolf.com/blog/2025/august/advisory---netskope-cross-tenant-authentication-bypass) | 28.0 | 38.0 | 42.0 |
| [Fortinet、FortiSandboxとFortiAuthenticatorのクリティカルなRCE脆弱性を警告](https://bleepingcomputer.com/news/security/fortinet-warns-of-critical-rce-flaws-in-fortisandbox-and-fortiauthenticator) | 28.0 | 38.0 | 42.0 |
| [Mini Shai-Huludマルウェアが大規模なサプライチェーン攻撃で数百件のオープンソースパッケージを侵害](https://cyberscoop.com/mini-shai-hulud-supply-chain-malware-attack) | 28.0 | 30.0 | 42.0 |
| [West Pharmaceutical、ランサムウェア攻撃で業務に影響と警告](https://therecord.media/west-pharmaceutical-warns-of-ransomware-attack-impacting-operations) | 28.0 | 30.0 | 42.0 |
| [Nansh0uキャンペーン ― ハッカーの武器庫がさらに強化される](https://akamai.com/blog/security/the-nansh0u-campaign-hackers-arsenal-grows-stronger) | 28.0 | 20.0 | 42.0 |
| [Oracle of Delphi が認証情報を窃取する](https://akamai.com/blog/security/the-oracle-of-delphi-steal-your-credentials) | 28.0 | 20.0 | 42.0 |
| [米政府、Canvasへの大規模サイバー攻撃に関するInstructureの証言を求める](https://bleepingcomputer.com/news/security/us-govt-seeks-instructure-testimony-on-massive-canvas-cyberattack) | 28.0 | 20.0 | 42.0 |
| [Claude拡張機能に深刻な脆弱性 無権限でAI操作を乗っ取り可能](https://atmarkit.itmedia.co.jp/ait/articles/2605/13/news037.html) | 28.0 | 20.0 | 42.0 |
| [AI支援による合成攻撃ログ生成で検知エンジニアリングを加速する](https://microsoft.com/en-us/security/blog/2026/05/12/accelerating-detection-engineering-using-ai-assisted-synthetic-attack-logs-generation) | 27.0 | 20.0 | 42.0 |
| [大山鳴動 深刻度「低」脆弱性 1 匹 ～ cURL開発者「脆弱性発見 AI Mythos は宣伝目的の茶番」](https://scan.netsecurity.ne.jp/article/2026/05/13/55258.html) | 26.0 | 20.0 | 42.0 |
| [GMOサイバーセキュリティ byイエラエ「AIエージェントペネトレーションテスト」の提供](https://scan.netsecurity.ne.jp/article/2026/05/13/55249.html) | 26.0 | 20.0 | 42.0 |
| [スリーシェイク「AI-Ready に関する実態調査」を発表](https://scan.netsecurity.ne.jp/article/2026/05/13/55248.html) | 26.0 | 20.0 | 42.0 |
| [AIを活用した思考の可視化と共有化―属人知を組織知に転換する7つのステップ](https://japan.zdnet.com/article/35247317) | 26.0 | 20.0 | 42.0 |
| [東芝、AIの異常検知の根拠を説明する技術　波形データで分かりやすく](https://xtech.nikkei.com/atcl/nxt/news/24/03218) | 26.0 | 20.0 | 42.0 |
| [OpenAI Sora 2のセキュリティ：マルチモーダルLLMを駆動するシステムプロンプトの解明](https://mindgard.ai/resources/openai-sora-system-prompts) | 25.0 | 20.0 | 42.0 |
| [必見：Geminiをハッキングする—多層的アプローチ](https://buganizer.cc/hacking-gemini-a-multi-layered-approach-md) | 25.0 | 20.0 | 42.0 |
| [主要世界経済国がAIの「構成要素リスト」の主要項目を明確化](https://cyberscoop.com/g7-cisa-ai-sbom-security-guidance) | 25.0 | 20.0 | 42.0 |
| [訓練なし、検証なし、責任者不明 サイバーBCPの危うい実態](https://atmarkit.itmedia.co.jp/ait/articles/2605/13/news053.html) | 24.0 | 20.0 | 43.0 |
| [テスト自動化ツールのオーティファイ、品質検証サービスに乗り出す理由](https://japan.zdnet.com/article/35247210) | 24.0 | 20.0 | 43.0 |
| [Citrix NetScaler のメモリリークおよび反射型XSS（CVE-2025-12101）](https://bit.ly/48bPzCO) | 23.0 | 34.0 | 50.0 |
| [MixMaster MMORPGのリバースエンジニアリングによるセキュリティ分析](https://3r4y.github.io/posts/mixmasterreverseengineering) | 22.0 | 20.0 | 42.0 |
| [Mozilla、「Firefox 150.0.3」を公開 - 脆弱性5件を修正](https://security-next.com/184338) | 22.0 | 20.0 | 42.0 |

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
