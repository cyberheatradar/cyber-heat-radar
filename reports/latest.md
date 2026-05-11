# 📡 サイレーダー 2026-05-12 05:00 JST 試作版

このレポートは、2026-05-11 05:00 JST〜2026-05-12 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 490
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 6
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks](#topic-216) | 100.0 | 99.0 | 92.0 | 音声 | 温度感上位枠 |
| 2 | [CVE-2026-31431: Copy Fail Linux kernel local privilege escalation](#topic-107) | 100.0 | 95.0 | 92.0 | 音声 | 温度感上位枠 |
| 3 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 74.0 | 82.0 | 81.0 | 音声 | 温度感上位枠 |
| 4 | [ランサムウェア交渉役・関係者に実刑判決](#topic-3001) | 45.0 | 45.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [「BerriAI LiteLLM」にSQLi脆弱性 - 認証情報漏洩のおそれ、悪用も](#topic-2412) | 43.0 | 46.0 | 43.0 | GitHub | - |
| 6 | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](#topic-31) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 7 | [Apache HTTP Server 2.4における複数の脆弱性に対するアップデート（2026年5月）](#topic-394) | 35.0 | 46.0 | 54.0 | GitHub | - |
| 8 | [Hackers Used AI to Develop First Known Zero-Day 2FA Bypass for Mass Exploitation](#topic-2989) | 35.0 | 20.0 | 43.0 | 音声 | AI×Security枠 |
| 9 | [Hackers Observed Using AI to Develop Zero-Day for the First Time](#topic-3011) | 35.0 | 20.0 | 43.0 | 音声 | AI×Security枠 |
| 10 | [Final Countdown: Last Chance to Join the Rapid7 Global Cybersecurity Summit](#topic-3015) | 33.0 | 20.0 | 42.0 | GitHub | - |
| 11 | [次世代reCAPTCHAがAIによる突破対策のため「Google Play開発者サービス」を必須にしてパズルではなくQRコードスキャンを要求](#topic-2403) | 31.0 | 20.0 | 42.0 | GitHub | - |
| 12 | [Threats Making WAVs - Incident Response to a Cryptomining Attack](#topic-29) | 30.0 | 20.0 | 42.0 | GitHub | - |
| 13 | [Why we use CAPTCHAs, (Mon, May 11th)](#topic-2998) | 30.0 | 20.0 | 42.0 | GitHub | - |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-216"></a>

### 1. CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>KEV</nobr> / <nobr>認証バイパス</nobr> / <nobr>防御・運用</nobr> / <nobr>政策・規制</nobr> / <nobr>脅威レポート</nobr> / <nobr>PoC</nobr> / <nobr>ボットネット</nobr> / <nobr>マルウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 高温 |
| <nobr>温度感</nobr> | 100.0 |
| <nobr>実務影響</nobr> | 99.0 |
| <nobr>確度</nobr> | 92.0 |

#### 概要

CVE-2026-41940は、cPanel & WHMおよびWP2（WordPress Squared）に影響する認証バイパスの脆弱性として、実際の悪用が確認されているとされています。
公開情報では、ランサムウェア攻撃やバックドア設置に関連した事例が報告されており、CISAのKEVカタログにも追加されています。
管理用コントロールパネルが影響を受けるため、侵害されるとサーバー運用全体に広く波及するおそれがあります。
公開PoCの言及もあり、未対応環境では悪用可能性が高い点が注目されています。

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

- cPanel & WHM / WP2の利用有無を確認し、該当環境は優先的に修正状況を点検する。
- 認証回避を前提とした不審な管理者操作や、ファイル配置・永続化の兆候を監視する。
- 外部公開された管理画面の露出を見直し、アクセス制御や多要素認証などの防御を確認する。

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
| <nobr>出典</nobr> | [cPanel CVE-2026-41940 Under Active Exploitation to Deploy Filemanager Backdoor](https://thehackernews.com/2026/05/cpanel-cve-2026-41940-under-active.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Week in review: cPanel vulnerability actively exploited, DigiCert breach, Linked](https://helpnetsecurity.com/2026/05/10/week-in-review-cpanel-vulnerability-actively-exploited-digicert-breach-linkedin-job-scams) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [4th May – Threat Intelligence Report](https://research.checkpoint.com/2026/4th-may-threat-intelligence-report) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [South-East Asian Military Entities Targeted via cPanel (CVE-2026-41940)](https://ctrlaltintel.com/research/SEA-CPanel) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Vulnerability Alert: CVE-2026-41940 in cPanel, WHM, and WP Squared](https://bitsight.com/blog/critical-vulnerability-alert-cve-2026-41940-cPanel-WHM-WPSquared) | <nobr>内容確認・補足情報</nobr> |

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

<a id="topic-107"></a>

### 2. CVE-2026-31431: Copy Fail Linux kernel local privilege escalation

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>Linux</nobr> / <nobr>脆弱性</nobr> / <nobr>権限昇格</nobr> / <nobr>CVE</nobr> / <nobr>TTP</nobr> / <nobr>ゼロデイ</nobr> / <nobr>防御・運用</nobr> / <nobr>AI</nobr> / <nobr>PoC</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 高温 |
| <nobr>温度感</nobr> | 100.0 |
| <nobr>実務影響</nobr> | 95.0 |
| <nobr>確度</nobr> | 92.0 |

#### 概要

Linux kernelのローカル権限昇格脆弱性として、CVE-2026-31431（Copy Fail）が注目されています。
公開情報では、影響範囲が広く、悪用やPoCの言及もあるため、既存環境への影響確認が必要とみられています。
ローカル権限昇格は、侵入後に管理者権限へ拡大される足がかりになりやすく、被害の深刻化につながります。
Linuxカーネルは利用範囲が広いため、対象システムの把握と優先対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 22 sources。
- CISA KEV関連。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 技術者コミュニティ反応: 強。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- 権限昇格系。
- 実務影響100は特別条件が揃う場合に限定するため、上限補正を適用。

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

- 影響を受けるLinuxカーネルのバージョンや配布物を確認し、ベンダーの修正状況を点検する。
- サーバーや重要端末で、不要なローカルアカウントや権限の見直しを行い、侵入後の権限昇格リスクを下げる。
- 監視・検知の観点では、通常と異なる権限取得やカーネル周辺の異常な挙動を重点的に確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-31431 | 主要CVE | 1.00 |
| ベンダー | Linux | 影響ベンダー | 1.00 |
| 脆弱性 | CVE-2026-43284 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-43500 | 主要CVE | 1.00 |
| 製品 | Kernel | 影響製品 | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-31431](https://nvd.nist.gov/vuln/detail/CVE-2026-31431) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | ['Dirty Frag' Exploit Poised to Blow Up on Enterprise Linux Distros](https://darkreading.com/vulnerabilities-threats/dirty-frag-exploit-blow-up-enterprise-linux-distros) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Linux developers weigh emergency “killswitch” for vulnerable kernel functions](https://helpnetsecurity.com/2026/05/11/linux-kernel-emergency-killswitch) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Dirty Frag: Linux kernel hit by second major security flaw in two weeks](https://therecord.media/dirty-frag-linux-kernel-hit-by-second-major-bug) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [New ‘Dirty Frag’ Linux Vulnerability Possibly Exploited in Attacks](https://securityweek.com/new-dirty-frag-linux-vulnerability-possibly-exploited-in-attacks) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Another Universal Linux Local Privilege Escalation (LPE) Vulnerability: Dirty Fr](https://isc.sans.edu/diary/rss/32968) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Linux Kernel Dirty Frag LPE Exploit Enables Root Access Across Major Distributio](https://thehackernews.com/2026/05/linux-kernel-dirty-frag-lpe-exploit.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Unplug your way to better code](https://blog.talosintelligence.com/unplug-your-way-to-better-code) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: あり。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 強。
- 技術者コミュニティ反応: 強。
- 開発者コミュニティ反応: 中。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。
- 継続観測: 継続。

---

<a id="topic-12"></a>

### 3. Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).

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

CVE-2025-60710は、Microsoft WindowsのTaskhost関連タスクにおけるローカル権限昇格の脆弱性とされています。
CISAのKnown Exploited Vulnerabilitiesに掲載されており、公開PoCや検証コードの言及も確認されています。
権限昇格の脆弱性は、端末内での被害拡大や管理者権限の取得につながるため、優先度が高い領域です。
さらに、KEV掲載と公開PoCの存在は、実環境での悪用リスクを意識した対応が必要であることを示します。

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

- Microsoftの更新情報とCISA KEV掲載状況を確認し、該当端末への適用優先度を上げる。
- Windows端末で不審なローカル権限昇格の兆候や、Taskhost関連の異常挙動を点検する。
- 影響範囲の棚卸しを行い、管理者権限を持つ端末・重要端末を優先して対策状況を確認する。

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

<a id="topic-3001"></a>

### 4. ランサムウェア交渉役・関係者に実刑判決

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>脅威アクター</nobr> / <nobr>脆弱性</nobr> / <nobr>マルウェア</nobr> / <nobr>TTP</nobr> / <nobr>サプライチェーン</nobr> / <nobr>防御・運用</nobr> / <nobr>Android</nobr> / <nobr>政策・規制</nobr> / <nobr>攻撃キャンペーン</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 45.0 |
| <nobr>実務影響</nobr> | 45.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Google Threat Intelligence Group（GTIG）は、生成AIを悪用する攻撃活動が研究段階から実運用へ進みつつあると報告しました。
脅威アクターは脆弱性調査、回避、認証回避、情報収集、さらにはサプライチェーン経由の侵害まで、攻撃の各段階でAIを取り入れているとしています。
AIは攻撃の効率化や自動化を後押しする一方、AI関連基盤や開発・CI/CD周辺への影響も広げます。
特にサプライチェーン侵害や認証回避のような事案は、単一組織にとどまらず下流の利用者にも波及し得る点が注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- ランサムウェア文脈。
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI連携機能、依存パッケージ、CI/CD、APIキー管理など“周辺層”の監視と棚卸しを強化する。
- 不審なアカウント作成・API利用増加・連携先の急な変更など、AIサービスの不自然な利用兆候を確認する。
- 認証強化や権限最小化に加え、サードパーティ製スキル／プラグイン／拡張の導入審査を見直す。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [GTIG AI Threat Tracker: Adversaries Leverage AI for Vulnerability Exploitation, ](https://cloud.google.com/blog/topics/threat-intelligence/ai-vulnerability-exploitation-initial-access) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 初出。

---

<a id="topic-31"></a>

### 5. PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers

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

<a id="topic-2989"></a>

### 6. Hackers Used AI to Develop First Known Zero-Day 2FA Bypass for Mass Exploitation

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脅威アクター</nobr> / <nobr>AI</nobr> / <nobr>ゼロデイ</nobr> / <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | AI×Security枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 35.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Hackers Used AI to Develop First Known Zero-Day 2FA Bypass for Mass Exploitation に関する脆弱性情報です。
では英語本文の全文翻訳は行わず、参照リンク、関連する対象、スコア根拠を中心に整理しています。詳細はベンダー公式情報、公的機関情報、NVD等を確認してください。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- AIが扱うデータ分類と機密度を確認する。
- AIツールやエージェントに与えている権限・外部接続範囲を確認する。
- 入力データが学習・保存・第三者提供に使われる条件を確認する。
- 監査ログ、承認フロー、利用者管理が定義されているか確認する。
- プラグイン、MCP、外部ツール連携の許可範囲を確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Hackers Used AI to Develop First Known Zero-Day 2FA Bypass for Mass Exploitation](https://thehackernews.com/2026/05/hackers-used-ai-to-develop-first-known.html) | <nobr>内容確認・補足情報</nobr> |

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

<a id="topic-3011"></a>

### 7. Hackers Observed Using AI to Develop Zero-Day for the First Time

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ゼロデイ</nobr> / <nobr>AI</nobr> / <nobr>攻撃キャンペーン</nobr> |
| <nobr>分類理由</nobr> | AI×Security枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 35.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Hackers Observed Using AI to Develop Zero-Day for the First Time に関する脆弱性情報です。
では英語本文の全文翻訳は行わず、参照リンク、関連する対象、スコア根拠を中心に整理しています。詳細はベンダー公式情報、公的機関情報、NVD等を確認してください。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 攻撃者がAIを使っている工程と、既存の検知・教育で補足できる範囲を確認する。
- フィッシング、マルウェア、詐欺テンプレート、認証情報窃取の観点で検知ロジックを確認する。
- SOC/CSIRTで共有すべきIoC、TTP、注意喚起文面があるか確認する。
- 利用者向け注意喚起や訓練内容を更新する必要があるか確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Hackers Observed Using AI to Develop Zero-Day for the First Time](https://infosecurity-magazine.com/news/hackers-using-ai-zero-day-first) | <nobr>内容確認・補足情報</nobr> |

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

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-2412"></a>

### 1. 「BerriAI LiteLLM」にSQLi脆弱性 - 認証情報漏洩のおそれ、悪用も

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>AI</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 43.0 |
| <nobr>実務影響</nobr> | 46.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

米当局は、LLMサービス向けプロキシである「BerriAI LiteLLM」の脆弱性が悪用されているとして注意喚起を行った。データベース内の情報が読み取られるおそれがある。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- 情報漏えい系。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [「BerriAI LiteLLM」にSQLi脆弱性 - 認証情報漏洩のおそれ、悪用も](https://security-next.com/184241) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 未評価。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 初出。

---

<a id="topic-394"></a>

### 2. Apache HTTP Server 2.4における複数の脆弱性に対するアップデート（2026年5月）

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>RCE</nobr> / <nobr>権限昇格</nobr> / <nobr>DDoS</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 35.0 |
| <nobr>実務影響</nobr> | 46.0 |
| <nobr>確度</nobr> | 54.0 |

#### 概要

Apache HTTP Server 2.4における複数の脆弱性に対するアップデート（2026年5月） に関する脆弱性情報です。
では英語本文の全文翻訳は行わず、参照リンク、関連する対象、スコア根拠を中心に整理しています。詳細はベンダー公式情報、公的機関情報、NVD等を確認してください。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-23918 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-24072 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-28780 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-29168 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-29169 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-33006 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-33007 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-33523 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-33857 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-34032 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-23918](https://nvd.nist.gov/vuln/detail/CVE-2026-23918) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>公的・一次情報</nobr> | [Apache HTTP Server 2.4における複数の脆弱性に対するアップデート（2026年5月）](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015084.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Apache HTTP/2 Flaw (CVE-2026-23918) Enables DoS and Potential RCE](https://thehackernews.com/2026/05/critical-apache-http2-flaw-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: あり。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 弱。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 継続。

---

<a id="topic-3015"></a>

### 3. Final Countdown: Last Chance to Join the Rapid7 Global Cybersecurity Summit

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>CISO・組織運営</nobr> / <nobr>防御・運用</nobr> / <nobr>AI</nobr> / <nobr>TTP</nobr> / <nobr>脅威レポート</nobr> / <nobr>脆弱性</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Final Countdown: Last Chance to Join the Rapid7 Global Cybersecurity Summit は、AIを攻撃者側の自動化・詐欺・マルウェア・フィッシングに利用する話題です。
攻撃手口、標的、検知観点、利用者教育やSOC監視への反映要否を確認する価値があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Final Countdown: Last Chance to Join the Rapid7 Global Cybersecurity Summit](https://rapid7.com/blog/post/it-last-chance-rapid7-global-cybersecurity-summit) | <nobr>内容確認・補足情報</nobr> |

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

<a id="topic-2403"></a>

### 4. 次世代reCAPTCHAがAIによる突破対策のため「Google Play開発者サービス」を必須にしてパズルではなくQRコードスキャンを要求

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>Android</nobr> / <nobr>AI</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 31.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Googleが不正なアクセスを防ぐための仕組みとして導入している「reCAPTCHA」で、AIによる突破を防ぎ人間のユーザーだけを通すためのふるいとして、Android端末では「『Google Play開発者サービス』がインストールされていること」を必須要件としたことがわかりました。
不審なアクティビティと判断された場合に人間であることを証明する方法も「パズルを解く」ではなく「QRコードをスキャンする」に改められています。続きを読む...

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [次世代reCAPTCHAがAIによる突破対策のため「Google Play開発者サービス」を必須にしてパズルではなくQRコードスキャンを要求](https://gigazine.net/news/20260511-google-new-recaptcha-needs-google-play-services) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 弱。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-29"></a>

### 5. Threats Making WAVs - Incident Response to a Cryptomining Attack

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

<a id="topic-2998"></a>

### 6. Why we use CAPTCHAs, (Mon, May 11th)

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | - |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Why we use CAPTCHAs, (Mon, May 11th) に関する脅威・攻撃キャンペーン系の話題です。
攻撃者、標的、TTP、IoC、悪用技術、検知観点を中心に確認する価値があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Why we use CAPTCHAs, (Mon, May 11th)](https://isc.sans.edu/diary/rss/32974) | <nobr>内容確認・補足情報</nobr> |

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
| [いま見直す「ランサムウェア対策の基本」--ZDNETセキュリティセミナー開催](https://japan.zdnet.com/article/35247109) | 29.0 | 30.0 | 42.0 |
| [山一電機 フィリピン子会社にランサムウェア攻撃](https://scan.netsecurity.ne.jp/article/2026/05/11/55233.html) | 29.0 | 30.0 | 42.0 |
| [東山産業へのランサムウェア攻撃、データの公開を確認](https://scan.netsecurity.ne.jp/article/2026/05/11/55232.html) | 29.0 | 30.0 | 42.0 |
| [ファイルが暗号化されておりランサムウェアである可能性が高い ～ オーミケンシへのサイバー攻撃によるシステム障害](https://scan.netsecurity.ne.jp/article/2026/05/11/55231.html) | 29.0 | 30.0 | 42.0 |
| [UniFi Accessにおけるリモートコード実行の脆弱性（CVE-2025-52665）](https://catchify.sa/post/cve-2025-52665-rce-in-unifi-os-25-000) | 28.0 | 46.0 | 50.0 |
| [CVE-2026-42258 net-imapにおける未検証のSymbol入力によるコマンドインジェクション](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-42258) | 28.0 | 46.0 | 38.0 |
| [CVE-2026-42257: net-imapにおける複数コマンドの「raw」引数を介したコマンドインジェクション](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-42257) | 28.0 | 46.0 | 38.0 |
| [Netskopeにおけるクロステナント認証バイパスのセキュリティ問題](https://blog.amberwolf.com/blog/2025/august/advisory---netskope-cross-tenant-authentication-bypass) | 28.0 | 38.0 | 42.0 |
| [英国の水道会社でハッカーが約2年間も潜伏、規制当局が確認](https://therecord.media/uk-water-company-had-hackers-lurking-for-years) | 28.0 | 30.0 | 42.0 |
| [ランサムウェアの現状 ― 2026年第1四半期](https://research.checkpoint.com/2026/the-state-of-ransomware-q1-2026) | 28.0 | 30.0 | 42.0 |
| [Oracle of Delphiが認証情報を窃取する](https://akamai.com/blog/security/the-oracle-of-delphi-steal-your-credentials) | 28.0 | 20.0 | 42.0 |
| [Nansh0uキャンペーン―ハッカーの武器庫がさらに強化](https://akamai.com/blog/security/the-nansh0u-campaign-hackers-arsenal-grows-stronger) | 28.0 | 20.0 | 42.0 |
| [DAEMON Toolsのバックドアが標的型の後続マルウェア攻撃を可能にする](https://blog.polyswarm.io/daemon-tools-backdoor-enables-targeted-follow-on-malware-operations) | 28.0 | 20.0 | 42.0 |
| [Second Canvasのデータ侵害で学校や大学に大きな混乱](https://cybersecuritydive.com/news/a-2nd-canvas-data-breach-causes-major-disruptions-for-schools-colleges/819784) | 28.0 | 20.0 | 42.0 |
| [航空関連企業を狙うサイバー諜報グループ、地図データを窃取](https://darkreading.com/vulnerabilities-threats/cyber-espionage-group-aviation-firms-steal-map-data) | 28.0 | 20.0 | 42.0 |
| [米国人2人が偽従業員向けノートPC農場への関与で有罪判決](https://itpro.com/security/two-us-nationals-sentenced-for-role-in-prolific-fake-worker-laptop-farms) | 28.0 | 20.0 | 42.0 |
| [ShinyHuntersがCanvasの恐喝を学校ごとのランサム攻撃へ拡大](https://infosecurity-magazine.com/news/shinyhunters-escalates-canvas) | 28.0 | 20.0 | 42.0 |
| [TrickMo Androidバンカーが秘匿通信にTONブロックチェーンを採用](https://bleepingcomputer.com/news/security/trickmo-android-banker-adopts-ton-blockchain-for-covert-comms) | 28.0 | 20.0 | 42.0 |
| [5年以上にわたるフィッシングキャンペーンで500以上の組織が被害](https://securityweek.com/over-500-organizations-hit-in-years-long-phishing-campaign) | 28.0 | 20.0 | 42.0 |
| [Electerm projectのElectermにおける複数の脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-014913.html) | 28.0 | 20.0 | 42.0 |
| [Palo Alto NetworksのPAN-OSにおける境界外書き込みに関する脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-014858.html) | 28.0 | 20.0 | 42.0 |
| [スマートフォンアプリ「くら寿司 公式アプリ」における証明書検証不備の脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-000067.html) | 27.0 | 31.0 | 51.0 |
| [libXpmにおける境界外読み取りの脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-000070.html) | 27.0 | 31.0 | 51.0 |
| [LinuxのLinux Kernelにおける境界外書き込みに関する脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-014806.html) | 27.0 | 23.0 | 43.0 |

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
