# 📡 サイレーダー 2026-05-15 08:01 JST 試作版

このレポートは、2026-05-14 20:00 JST〜2026-05-15 08:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 122
- [音声で扱う想定のトピック](#audio-topics): 0
- [GitHubのみ掲載想定のトピック](#github-only-topics): 10
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-20182: CISA KEV catalog addition](#topic-4945) | 93.0 | 84.0 | 67.0 | GitHub | 直近掲載済み・再掲抑制 |
| 2 | [CVE-2026-0265: CISA KEV catalog addition](#topic-4257) | 62.0 | 74.0 | 56.0 | GitHub | 直近掲載済み・再掲抑制 |
| 3 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 54.0 | 82.0 | 81.0 | GitHub | 直近掲載済み・再掲抑制 |
| 4 | [Maximum Severity Cisco SD-WAN Bug Exploited in the Wild](#topic-5050) | 45.0 | 38.0 | 43.0 | GitHub | 直近掲載済み・再掲抑制 |
| 5 | [PraisonAI CVE-2026-44338 Auth Bypass Targeted Within Hours of Disclosure](#topic-4997) | 36.0 | 46.0 | 50.0 | GitHub | 直近掲載済み・再掲抑制 |
| 6 | [Fragnesia: New Linux kernel LPE bug was spawned by Dirty Frag patch (CVE-2026-46300)](#topic-4581) | 36.0 | 40.0 | 62.0 | GitHub | 直近掲載済み・再掲抑制 |
| 7 | [LATAM Under Siege: Agent Tesla’s 18-Month Credential Theft Campaign Against Chilean Enterprises](#topic-4995) | 36.0 | 30.0 | 42.0 | GitHub | 直近掲載済み・再掲抑制 |
| 8 | [OpenAI asks macOS users to update after TanStack npm supply chain attack](#topic-5049) | 33.0 | 30.0 | 42.0 | GitHub | 直近掲載済み・再掲抑制 |
| 9 | [Cofense adds AI-powered campaign detection to stop phishing attacks](#topic-4974) | 33.0 | 20.0 | 42.0 | GitHub | 直近掲載済み・再掲抑制 |
| 10 | [Kazuar: Anatomy of a nation-state botnet](#topic-4956) | 30.0 | 20.0 | 42.0 | GitHub | 直近掲載済み・再掲抑制 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

今回は音声で扱う想定のトピックはありません。

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-4945"></a>

### 1. CVE-2026-20182: CISA KEV catalog addition

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>認証バイパス</nobr> / <nobr>KEV</nobr> / <nobr>政策・規制</nobr> / <nobr>防御・運用</nobr> / <nobr>IoC</nobr> / <nobr>PoC</nobr> / <nobr>ゼロデイ</nobr> / <nobr>国家支援</nobr> |
| <nobr>温度状態</nobr> | 高温 |
| <nobr>温度感</nobr> | 93.0 |
| <nobr>実務影響</nobr> | 84.0 |
| <nobr>確度</nobr> | 67.0 |

#### 概要

Cisco Catalyst SD-WAN Controllerに存在する認証バイパス脆弱性CVE-2026-20182が、CISAのKEVカタログに追加されました。
公開情報では、限定的ではあるものの実際の悪用が確認されているとされ、管理権限の取得につながる可能性が指摘されています。
KEV掲載は、実環境での悪用可能性が高く、優先対応が必要な脆弱性であることを示します。ネットワーク制御系製品への影響のため、侵害時の波及範囲が大きくなり得ます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 中。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 公開PoC・検証コード言及あり。
- 公開PoC/Exploitコード: 確認あり。
- 直接PoCリンク: 掲載しません。
- 確認方針: NVD、ベンダー公式、公的機関、信頼できる技術分析を優先し、GitHub等のコードは防御・検証目的で別途確認します。

#### 担当者向け確認ポイント

- Ciscoの案内に沿って、対象製品とバージョンを確認し、修正版への更新を優先する。
- 管理系コンポーネントへの不審なアクセスや設定変更、認証関連の異常を監視する。
- 関連するインシデントがないか、管理権限の棚卸しとログ確認を急ぐ。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20182 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20182](https://nvd.nist.gov/vuln/detail/CVE-2026-20182) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of new critical SD-WAN flaw exploited in zero-day attacks](https://bleepingcomputer.com/news/security/cisco-warns-of-new-critical-sd-wan-flaw-exploited-in-zero-day-attacks) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller Auth Bypass Actively Exploited to Gain Admin Ac](https://thehackernews.com/2026/05/cisco-catalyst-sd-wan-controller-auth.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Ongoing exploitation of Cisco Catalyst SD-WAN vulnerabilities](https://blog.talosintelligence.com/sd-wan-ongoing-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [The Dark Side of Efficiency: When Network Controllers Become "God Mode" for Atta](https://rapid7.com/blog/post/tr-efficiencys-dark-side-network-controllers-in-god-mode-attackers-sd-wan) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-20182: Critical authentication bypass in Cisco Catalyst SD-WAN Controll](https://rapid7.com/blog/post/ve-cve-2026-20182-critical-authentication-bypass-cisco-catalyst-sd-wan-controller-fixed) | <nobr>内容確認・補足情報</nobr> |
| <nobr>公的・一次情報</nobr> | [Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-rpa2-v69WY2SW) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://cisa.gov/news-events/alerts/2026/05/14/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 中。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。
- 継続観測: 継続。

---

<a id="topic-4257"></a>

### 2. CVE-2026-0265: CISA KEV catalog addition

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>KEV</nobr> / <nobr>認証バイパス</nobr> / <nobr>防御・運用</nobr> / <nobr>脅威アクター</nobr> / <nobr>政策・規制</nobr> / <nobr>PoC</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 62.0 |
| <nobr>実務影響</nobr> | 74.0 |
| <nobr>確度</nobr> | 56.0 |

#### 概要

Palo Alto NetworksのPAN-OSに関するCVE-2026-0265について、CISAのKEVカタログへの追加が話題になっています。
CAS（Cloud Authentication Service）が有効でログインインターフェースに関連付けられている構成では、認証バイパスにつながる可能性があるとされています。
KEVへの追加は、実際の攻撃リスクが高いと判断された脆弱性として運用優先度が上がることを意味します。
対象製品がファイアウォールや管理基盤であるため、影響範囲の確認と迅速な更新が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 公開PoC・検証コード言及あり。
- 公開PoC/Exploitコード: 確認あり。
- 直接PoCリンク: 掲載しません。
- 確認方針: NVD、ベンダー公式、公的機関、信頼できる技術分析を優先し、GitHub等のコードは防御・検証目的で別途確認します。

#### 担当者向け確認ポイント

- CASが有効なPAN-OS環境か、対象のログインインターフェースに紐づいていないかを確認する。
- 影響を受ける版かどうかを整理し、可能なら修正版へ優先的に更新する。
- 一時的な回避策よりも、ベンダーの修正適用を優先し、管理系アクセスの露出を見直す。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-0265 | 主要CVE | 1.00 |
| ベンダー | Palo Alto | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-0265](https://nvd.nist.gov/vuln/detail/CVE-2026-0265) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0265: Authentication Bypass in Palo Alto Networks PAN-OS](https://rapid7.com/blog/post/etr-cve-2026-0265-authentication-bypass-in-palo-alto-networks-pan-os) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0265 PAN-OS: Authentication Bypass with Cloud Authentication Service (C](https://security.paloaltonetworks.com/CVE-2026-0265) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。
- 継続観測: 継続。

---

<a id="topic-12"></a>

### 3. Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>Windows</nobr> / <nobr>権限昇格</nobr> / <nobr>TTP</nobr> / <nobr>脆弱性</nobr> / <nobr>KEV</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 54.0 |
| <nobr>実務影響</nobr> | 82.0 |
| <nobr>確度</nobr> | 81.0 |

#### 概要

CVE-2025-60710は、Microsoft WindowsのTaskhost関連タスクにおけるローカル権限昇格の脆弱性とされています。
CISAのKnown Exploited Vulnerabilitiesに掲載されており、公開PoCや検証コードに言及があるため、確認の優先度は高いとみられます。
権限昇格の脆弱性は、侵入後に被害を拡大させる足がかりになりやすく、端末の管理権限奪取につながるおそれがあります。
さらに、KEV掲載と公開PoCの存在示唆により、実運用環境での対応が急がれます。

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
- 現在の熱量に合わせた冷却補正。

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

- Windows環境で該当CVEの影響有無を確認し、ベンダーの修正情報や推奨対策を優先して適用する。
- 権限の高いアカウントやタスク関連の挙動を監視し、想定外の権限昇格や不審なプロセス実行を点検する。
- 端末侵害後の横展開を防ぐため、最小権限と管理者権限の分離を改めて確認する。

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

<a id="topic-5050"></a>

### 4. Maximum Severity Cisco SD-WAN Bug Exploited in the Wild

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>KEV</nobr> / <nobr>脅威アクター</nobr> / <nobr>CVE</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 45.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Maximum Severity Cisco SD-WAN Bug Exploited in the Wild に関する脅威・攻撃キャンペーン系の話題です。
攻撃者、標的、TTP、IoC、悪用技術、検知観点を中心に確認する価値があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 攻撃者、標的業種、対象地域を確認する。
- 公開されたTTP、IoC、検知ロジックを確認する。
- 自組織のログ・EDR・SIEMで検知可能か確認する。
- 初期侵入経路、横展開、永続化、情報窃取の有無を確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Maximum Severity Cisco SD-WAN Bug Exploited in the Wild](https://darkreading.com/vulnerabilities-threats/maximum-severity-cisco-sd-wan-bug-exploited) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 初出。

---

<a id="topic-4997"></a>

### 5. PraisonAI CVE-2026-44338 Auth Bypass Targeted Within Hours of Disclosure

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>脅威アクター</nobr> / <nobr>認証バイパス</nobr> / <nobr>政策・規制</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 46.0 |
| <nobr>確度</nobr> | 50.0 |

#### 概要

PraisonAI CVE-2026-44338 Auth Bypass Targeted Within Hours of Disclosure に関する脆弱性情報です。
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
| 脆弱性 | CVE-2026-44338 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-44338](https://nvd.nist.gov/vuln/detail/CVE-2026-44338) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [PraisonAI CVE-2026-44338 Auth Bypass Targeted Within Hours of Disclosure](https://thehackernews.com/2026/05/praisonai-cve-2026-44338-auth-bypass.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-4581"></a>

### 6. Fragnesia: New Linux kernel LPE bug was spawned by Dirty Frag patch (CVE-2026-46300)

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>権限昇格</nobr> / <nobr>Linux</nobr> / <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>TTP</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 40.0 |
| <nobr>確度</nobr> | 62.0 |

#### 概要

Fragnesia: New Linux kernel LPE bug was spawned by Dirty Frag patch (CVE-2026-46300) に関する脆弱性情報です。
では英語本文の全文翻訳は行わず、参照リンク、関連する対象、スコア根拠を中心に整理しています。詳細はベンダー公式情報、公的機関情報、NVD等を確認してください。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 権限昇格系。

##### 確度
- 複数ソース確認。
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
| 脆弱性 | CVE-2026-46300 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-43284 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-46300](https://nvd.nist.gov/vuln/detail/CVE-2026-46300) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Fragnesia: New Linux kernel LPE bug was spawned by Dirty Frag patch (CVE-2026-46](https://helpnetsecurity.com/2026/05/14/fragnesia-cve-2026-46300-linux-lpe-vulnerability) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [New Linux Kernel Vulnerability Fragnesia Allows Root Privilege Escalation](https://securityweek.com/new-linux-kernel-vulnerability-fragnesia-allows-root-privilege-escalation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [New Fragnesia Linux flaw lets attackers gain root privileges](https://bleepingcomputer.com/news/security/new-fragnesia-linux-flaw-lets-attackers-gain-root-privileges) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [New Fragnesia Linux Kernel LPE Grants Root Access via Page Cache Corruption](https://thehackernews.com/2026/05/new-fragnesia-linux-kernel-lpe-grants.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 継続。

---

<a id="topic-4995"></a>

### 7. LATAM Under Siege: Agent Tesla’s 18-Month Credential Theft Campaign Against Chilean Enterprises

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>攻撃キャンペーン</nobr> / <nobr>マルウェア</nobr> / <nobr>ランサムウェア</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

LATAM Under Siege: Agent Tesla’s 18-Month Credential Theft Campaign Against Chilean Enterprises に関する脅威・攻撃キャンペーン系の話題です。
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

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| ベンダー | VMware | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [LATAM Under Siege: Agent Tesla’s 18-Month Credential Theft Campaign Against Chil](https://any.run/cybersecurity-blog/agent-tesla-latam-enterprise) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-5049"></a>

### 8. OpenAI asks macOS users to update after TanStack npm supply chain attack

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>サプライチェーン</nobr> / <nobr>AI</nobr> / <nobr>攻撃キャンペーン</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

OpenAI asks macOS users to update after TanStack npm supply chain attack は、ソフトウェアサプライチェーンを悪用した攻撃・侵害キャンペーン系の話題です。
影響するパッケージ、依存関係、開発環境、CI/CD、配布経路、認証情報や保守者アカウントの悪用有無を中心に確認する価値があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 影響するパッケージ、製品、依存関係を確認する。
- SBOM、lockfile、CI/CD、開発者端末への影響を確認する。
- 配布元、署名、ハッシュ、更新履歴の妥当性を確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ai_model_or_project | OpenAI | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [OpenAI asks macOS users to update after TanStack npm supply chain attack](https://therecord.media/openai-asks-macos-users-to-update-tanstack-npm) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-4974"></a>

### 9. Cofense adds AI-powered campaign detection to stop phishing attacks

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>フィッシング</nobr> / <nobr>防御・運用</nobr> / <nobr>攻撃キャンペーン</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Cofense adds AI-powered campaign detection to stop phishing attacks は、防御側でAIを活用するセキュリティ運用・検知・対応強化に関する話題です。
AIが扱うデータ、検知対象、判断支援の範囲、誤検知・過検知、監査ログ、既存SOC/CSIRT運用との接続を確認する価値があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIが扱うデータ分類と機密度を確認する。
- AIツールやエージェントに与えている権限・外部接続範囲を確認する。
- 入力データが学習・保存・第三者提供に使われる条件を確認する。
- 監査ログ、承認フロー、利用者管理が定義されているか確認する。
- プラグイン、MCP、外部ツール連携の許可範囲を確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Cofense  adds AI-powered campaign detection to stop phishing attacks](https://helpnetsecurity.com/2026/05/14/cofense-phishing-defense-platform-updates) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-4956"></a>

### 10. Kazuar: Anatomy of a nation-state botnet

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>国家支援</nobr> / <nobr>ボットネット</nobr> / <nobr>マルウェア</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Kazuar: Anatomy of a nation-state botnet に関する脅威・攻撃キャンペーン系の話題です。
攻撃者、標的、TTP、IoC、悪用技術、検知観点を中心に確認する価値があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 攻撃者、標的業種、対象地域を確認する。
- 公開されたTTP、IoC、検知ロジックを確認する。
- 自組織のログ・EDR・SIEMで検知可能か確認する。
- 初期侵入経路、横展開、永続化、情報窃取の有無を確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Kazuar: Anatomy of a nation-state botnet](https://microsoft.com/en-us/security/blog/2026/05/14/kazuar-anatomy-of-a-nation-state-botnet) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [Siemens SIPROTEC 5の脆弱性](https://cisa.gov/news-events/ics-advisories/icsa-26-134-13) | 28.0 | 46.0 | 50.0 |
| [Universal Robots Polyscope 5の脆弱性とセキュリティ対策](https://cisa.gov/news-events/ics-advisories/icsa-26-134-17) | 28.0 | 46.0 | 50.0 |
| [HackersがBurst Statistics WordPressプラグインの認証バイパス脆弱性を悪用](https://bleepingcomputer.com/news/security/hackers-exploit-auth-bypass-flaw-in-burst-statistics-wordpress-plugin) | 28.0 | 38.0 | 42.0 |
| [NGINXの18年前の脆弱性によりDoS、潜在的なRCEが可能に](https://bleepingcomputer.com/news/security/18-year-old-nginx-vulnerability-allows-dos-potential-rce) | 28.0 | 38.0 | 42.0 |
| [セキュアな接続と強固なバックアップでランサムウェア被害の早期復旧を支援するサービス、KDDIアイレットが提供開始](https://internet.watch.impress.co.jp/docs/news/2108724.html) | 28.0 | 30.0 | 42.0 |
| [West Pharmaceutical、ランサムウェア攻撃後に業務復旧を開始](https://cybersecuritydive.com/news/west-pharmaceutical-restoring-operations-ransomware-attack/820250) | 28.0 | 30.0 | 42.0 |
| [Foxconn、北米工場がサイバー攻撃を受けたと確認](https://cyberscoop.com/foxconn-cyberattack-disrupts-north-america-factories) | 28.0 | 30.0 | 42.0 |
| [Foxconn攻撃が浮き彫りにした製造業のサイバー危機](https://darkreading.com/cyberattacks-data-breaches/foxconn-attack-manufacturing-cyber-crisis) | 28.0 | 30.0 | 42.0 |
| [FrostyNeighbor APTがポーランドとウクライナの政府機関を標的に慎重に攻撃](https://darkreading.com/cyberattacks-data-breaches/frostyneighbor-apt-govt-orgs-poland-ukraine) | 28.0 | 20.0 | 42.0 |
| [Mustang Pandaが関与するアジア太平洋諜報キャンペーンで更新版FDMTPバックドアを使用](https://infosecurity-magazine.com/news/mustang-panda-fdmtp-backdoor-apj) | 28.0 | 20.0 | 42.0 |
| [中国系APTが標的を拡大し、最近のキャンペーンでバックドアを更新](https://securityweek.com/chinese-apts-expand-targets-update-backdoors-in-recent-campaigns) | 28.0 | 20.0 | 42.0 |
| [KimsukyがPebbleDashベースのツールで組織を標的にする](https://securelist.com/kimsuky-appleseed-pebbledash-campaigns/119785) | 28.0 | 20.0 | 42.0 |
| [大量のパッチ適用の時期が来る](https://blog.talosintelligence.com/the-time-of-much-patching-is-coming) | 27.0 | 20.0 | 42.0 |
| [自律型AIエージェントのための多層防御](https://microsoft.com/en-us/security/blog/2026/05/14/defense-in-depth-autonomous-ai-agents) | 27.0 | 20.0 | 42.0 |
| [設定ミスが脆弱性になるとき：AIアプリにおける悪用可能な誤設定](https://microsoft.com/en-us/security/blog/2026/05/14/configuration-becomes-vulnerability-exploitable-misconfigurations-ai-apps) | 27.0 | 20.0 | 42.0 |
| [AnthropicやOpenAIがFDE新会社、PEファンドと組む怖い理由](https://xtech.nikkei.com/atcl/nxt/column/18/00692/051400188) | 26.0 | 20.0 | 42.0 |
| [「AI導入による人員削減」はむしろ業績を悪化させる？　4月のAI注目論文](https://xtech.nikkei.com/atcl/nxt/column/18/02801/051300035) | 26.0 | 20.0 | 42.0 |
| [Claude Code生みの親は「コードを一行も自分で書いていない」――情シスはどう受け止めるべき？](https://techtarget.itmedia.co.jp/tt/news/2605/15/news12.html) | 26.0 | 20.0 | 42.0 |
| [AppleがiOS 26.5公開 カーネルやWebKitなど多数の脆弱性を修正、早期更新を](https://itmedia.co.jp/enterprise/articles/2605/15/news042.html) | 25.0 | 28.0 | 42.0 |
| [ペンタゴンのサイバー担当者、先進AIを「革命的な戦争」と呼ぶ](https://cyberscoop.com/pentagon-cyber-ai-revolutionary-warfare-mythos) | 25.0 | 20.0 | 42.0 |
| [ホワイトハウスのサイバー担当者、AI時代におけるIDセキュリティの重要性を強調](https://cyberscoop.com/white-house-federal-identity-security-ai-risks) | 25.0 | 20.0 | 42.0 |
| [OpenAIがTanStackのサプライチェーン攻撃におけるセキュリティ侵害を確認](https://bleepingcomputer.com/news/security/openai-confirms-security-breach-in-tanstack-supply-chain-attack) | 25.0 | 20.0 | 42.0 |
| [ThreatsDay Bulletin: PAN-OS RCE、Mythos cURLの脆弱性、AIトークナイザー攻撃、その他10件以上のニュース](https://thehackernews.com/2026/05/threatsday-bulletin-pan-os-rce-mythos.html) | 25.0 | 20.0 | 42.0 |
| [Frontier AIモデルによるセキュリティ脆弱性の迅速な発見](https://cybersecuritydive.com/news/frontier-ai-rapid-discovery-security-vulnerabilities/820258) | 25.0 | 20.0 | 42.0 |

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
