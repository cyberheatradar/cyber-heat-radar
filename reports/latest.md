# 📡 サイレーダー 2026-05-16 05:00 JST 試作版

このレポートは、2026-05-15 17:00 JST〜2026-05-16 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 104
- [音声で扱う想定のトピック](#audio-topics): 4
- [GitHubのみ掲載想定のトピック](#github-only-topics): 3
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cisco patches another actively exploited SD-WAN zero-day (CVE-2026-20182)](#topic-4945) | 83.0 | 84.0 | 67.0 | GitHub | 直近掲載済み・再掲抑制 |
| 2 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 54.0 | 82.0 | 81.0 | GitHub | 直近掲載済み・再掲抑制 |
| 3 | [Microsoft warns of Exchange zero-day flaw exploited in attacks](#topic-5579) | 48.0 | 44.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Unpatched Microsoft Exchange Server vulnerability exploited (CVE-2026-42897)](#topic-5098) | 46.0 | 52.0 | 65.0 | GitHub | 直近掲載済み・再掲抑制 |
| 5 | [Funnel Builder WordPress plugin bug exploited to steal credit cards](#topic-5528) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [Cisco zero-day under ongoing attack by persistent threat group](#topic-5542) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 7 | [Microsoft Reports Severe Zero-Day Flaw in On-Prem Exchange Servers](#topic-5554) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-5579"></a>

### 1. Microsoft warns of Exchange zero-day flaw exploited in attacks

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>脅威アクター</nobr> / <nobr>ゼロデイ</nobr> / <nobr>Windows</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 48.0 |
| <nobr>実務影響</nobr> | 44.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Microsoftは、Exchange Serverに存在する高深刻度の脆弱性について、攻撃で悪用されているとして緩和策を公表しました。
対象はOutlook on the webの利用者で、XSSに関連する形で任意コード実行につながるおそれがあるとされています。
ゼロデイとして悪用が確認されている点から、修正や緩和が遅れると影響が広がる可能性があります。
Exchangeは組織内で広く使われるため、メール基盤への影響が業務全体に及びやすいことも注目点です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。
- XSS系。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Exchange ServerとOutlook on the webの利用有無を確認し、Microsoftの案内に沿って緩和策や更新状況を点検する。
- 外部公開しているExchange関連の機能やアクセス経路について、不要な露出がないか確認する。
- 管理者向けの監視では、認証やWebアクセスの異常、想定外の挙動がないかを重点的に確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft warns of Exchange zero-day flaw exploited in attacks](https://bleepingcomputer.com/news/microsoft/microsoft-warns-of-exchange-zero-day-flaw-exploited-in-attacks) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 初出。

---

<a id="topic-5528"></a>

### 2. Funnel Builder WordPress plugin bug exploited to steal credit cards

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

WordPress向けプラグイン「Funnel Builder」に関する脆弱性が、WooCommerceのチェックアウト画面に不正なJavaScriptを注入する目的で悪用されていると報じられています。
これにより、決済情報の窃取につながるおそれがあるとされています。ECサイトの決済画面が改ざんされると、利用者のクレジットカード情報が漏えいするリスクがあります。
WordPressやWooCommerceを使う事業者にとって、プラグインの脆弱性管理が直接的な事業影響につながる事案です。

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

- Funnel Builderプラグインの利用有無とバージョンを確認し、更新版の適用可否を早急に点検する。
- WooCommerceのチェックアウト画面や関連スクリプトに不審な変更がないか、ファイル改ざんと管理者アカウントの異常を確認する。
- 決済ページを持つサイトでは、WAFや改ざん検知、支払い時の異常通信監視を強化する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Funnel Builder WordPress plugin bug exploited to steal credit cards](https://bleepingcomputer.com/news/security/funnel-builder-wordpress-plugin-bug-exploited-to-steal-credit-cards) | <nobr>内容確認・補足情報</nobr> |

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

<a id="topic-5542"></a>

### 3. Cisco zero-day under ongoing attack by persistent threat group

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>ゼロデイ</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Cisco zero-day under ongoing attack by persistent threat group に関する脆弱性情報です。
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

- CISA KEVに追加された各CVEを確認する。
- 自組織で対象製品を利用しているCVEが含まれるか確認する。
- 個別CVEごとのRequired Action、緩和策、期限を確認する。
- 音声や即時対応では、RCE、認証バイパス、広範な製品影響があるCVEを優先する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20182 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20122 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20128 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20133 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20127 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Cisco zero-day under ongoing attack by persistent threat group](https://cyberscoop.com/cisco-sd-wan-zero-day-exploited) | <nobr>内容確認・補足情報</nobr> |

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

<a id="topic-5554"></a>

### 4. Microsoft Reports Severe Zero-Day Flaw in On-Prem Exchange Servers

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ゼロデイ</nobr> / <nobr>Windows</nobr> / <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Microsoft Reports Severe Zero-Day Flaw in On-Prem Exchange Servers に関する脆弱性情報です。
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

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft Reports Severe Zero-Day Flaw in On-Prem Exchange Servers](https://infosecurity-magazine.com/news/microsoft-zeroday-exchange-servers) | <nobr>内容確認・補足情報</nobr> |

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

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-4945"></a>

### 1. Cisco patches another actively exploited SD-WAN zero-day (CVE-2026-20182)

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>ゼロデイ</nobr> / <nobr>認証バイパス</nobr> / <nobr>KEV</nobr> / <nobr>防御・運用</nobr> / <nobr>国家支援</nobr> / <nobr>脅威アクター</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>IoC</nobr> |
| <nobr>温度状態</nobr> | 高温 |
| <nobr>温度感</nobr> | 83.0 |
| <nobr>実務影響</nobr> | 84.0 |
| <nobr>確度</nobr> | 67.0 |

#### 概要

Ciscoは、Catalyst SD-WAN ControllerおよびSD-WAN Managerに影響する認証バイパス脆弱性CVE-2026-20182への修正を公開しました。
公開情報では、この問題は限定的なゼロデイ攻撃で悪用されたとされ、深刻度はCVSS 10.0とされています。
SD-WANは企業ネットワークの中核に置かれることが多く、管理系コンポーネントの認証不備は影響範囲が広くなりやすいです。
CISAのKEV掲載対象にもなっており、優先度の高い対応が必要と見られます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 中。
- 現在の熱量に合わせた冷却補正。

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

- Ciscoの修正情報を確認し、対象製品・対象バージョンの更新適用状況を速やかに点検する。
- SD-WAN Controller／Managerへの管理アクセス権限や到達経路を見直し、不要な露出を抑える。
- 関連ログを確認し、不審な管理操作や設定変更の兆候がないかを監視する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20182 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20133 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20128 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20122 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20127 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20182](https://nvd.nist.gov/vuln/detail/CVE-2026-20182) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Cisco patches another actively exploited SD-WAN zero-day (CVE-2026-20182)](https://helpnetsecurity.com/2026/05/15/cisco-sd-wan-zero-day-cve-2026-20182) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Patches Another SD-WAN Zero-Day, the Sixth Exploited in 2026](https://securityweek.com/cisco-patches-another-sd-wan-zero-day-the-sixth-exploited-in-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds Cisco SD-WAN CVE-2026-20182 to KEV After Admin Access Exploits](https://thehackernews.com/2026/05/cisa-adds-cisco-sd-wan-cve-2026-20182.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of new critical SD-WAN flaw exploited in zero-day attacks](https://bleepingcomputer.com/news/security/cisco-warns-of-new-critical-sd-wan-flaw-exploited-in-zero-day-attacks) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller Auth Bypass Actively Exploited to Gain Admin Ac](https://thehackernews.com/2026/05/cisco-catalyst-sd-wan-controller-auth.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Ongoing exploitation of Cisco Catalyst SD-WAN vulnerabilities](https://blog.talosintelligence.com/sd-wan-ongoing-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>公的・一次情報</nobr> | [Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-rpa2-v69WY2SW) | <nobr>内容確認・補足情報</nobr> |

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

<a id="topic-12"></a>

### 2. Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).

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

CVE-2025-60710は、Microsoft WindowsのTaskhost関連のタスク処理に起因するローカル権限昇格の脆弱性とされています。
CISAのKnown Exploited Vulnerabilitiesに含まれており、公開PoCや検証コードの存在が示唆されています。
権限昇格の脆弱性は、攻撃者が端末内でより高い権限を得る足がかりになり得るため、影響が広がりやすい点が重要です。
既知悪用リストに載っていることから、優先度を上げて確認すべき対象です。

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

- 対象Windows環境でCVE-2025-60710の影響有無を確認し、利用中の構成や更新状況を点検する。
- Microsoftの修正情報やCISA KEVの更新を確認し、適用可能な緩和策・更新を優先する。
- 端末内で不審な権限昇格の兆候やTaskhost関連の異常挙動がないか、監視・ログ確認を強化する。

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

<a id="topic-5098"></a>

### 3. Unpatched Microsoft Exchange Server vulnerability exploited (CVE-2026-42897)

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>Windows</nobr> / <nobr>KEV</nobr> / <nobr>ゼロデイ</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 46.0 |
| <nobr>実務影響</nobr> | 52.0 |
| <nobr>確度</nobr> | 65.0 |

#### 概要

Microsoft Exchange Serverの脆弱性CVE-2026-42897について、実際の悪用が観測されたとして注意喚起が出ています。
影響を受けるのはオンプレミス版Exchange Serverで、Exchange Onlineは対象外とされています。
CISAの既知悪用脆弱性カタログにも追加されており、放置すると組織内メール基盤への影響が広がるおそれがあります。
Microsoftは恒久修正までの間、暫定的な緩和策を案内しています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- XSS系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 対象がオンプレミス版Exchange Serverかを確認し、該当バージョンの有無を棚卸しする。
- Microsoftが案内する緩和策を適用し、恒久修正の提供状況を継続監視する。
- Exchange関連の不審な認証・表示不整合・メール起点の異常挙動がないか、監視とログ確認を強化する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-42897 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-42897](https://nvd.nist.gov/vuln/detail/CVE-2026-42897) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Warns of Exchange Server Zero-Day Exploited in the Wild](https://securityweek.com/microsoft-warns-of-exchange-server-zero-day-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://cisa.gov/news-events/alerts/2026/05/15/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Unpatched Microsoft Exchange Server vulnerability exploited (CVE-2026-42897)](https://helpnetsecurity.com/2026/05/15/exchange-server-cve-2026-42897-exploited) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [On-Prem Microsoft Exchange Server CVE-2026-42897 Exploited via Crafted Email](https://thehackernews.com/2026/05/on-prem-microsoft-exchange-server-cve.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-42897 Microsoft Exchange Server Spoofing Vulnerability](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-42897) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 継続。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [CVE-2026-42010 GnuTLSにおけるユーザー名のヌル文字を悪用した認証バイパス](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-42010) | 28.0 | 46.0 | 38.0 |
| [人気のnode-ipc npmパッケージが侵害され、認証情報を窃取](https://bleepingcomputer.com/news/security/popular-node-ipc-npm-package-compromised-to-steal-credentials) | 28.0 | 45.0 | 42.0 |
| [攻撃者がCisco Catalyst SD-WAN Controllerの重大な脆弱性を悪用](https://cybersecuritydive.com/news/attackers-exploit-critical-flaw-in-cisco-catalyst-sd-wan-controller/820368) | 28.0 | 38.0 | 42.0 |
| [CISAがCisco SD-WANシステムの悪用済み脆弱性に対する修正を日曜までに全連邦機関へ指示](https://therecord.media/cisa-orders-all-federal-agencies-to-patch-cisco-sd-wan-bug) | 28.0 | 38.0 | 42.0 |
| [American Lending Centerのデータ侵害で12万3000人に影響](https://securityweek.com/american-lending-center-data-breach-affects-123000-individuals) | 28.0 | 30.0 | 42.0 |
| [SHADOW-EARTH-053がレガシーなExchange脆弱性を悪用しアジア太平洋地域の政府機関を標的に攻撃](https://blog.polyswarm.io/shadow-earth-053-uses-legacy-exchange-exploitation-to-target-asia-pacific-governments) | 28.0 | 20.0 | 42.0 |
| [TurlaがKazuarバックドアをモジュール型P2Pボットネットに改変し、持続的アクセスを確保](https://thehackernews.com/2026/05/turla-turns-kazuar-backdoor-into.html) | 28.0 | 20.0 | 42.0 |
| [BlackFile：Vishingによる恐喝オペレーションの実態](https://cloud.google.com/blog/topics/threat-intelligence/blackfile-vishing-extortion-operation) | 28.0 | 20.0 | 42.0 |
| [攻撃者がJDownloaderのインストーラー配布をマルウェアに差し替えた問題](https://malwarebytes.com/blog/news/2026/05/attackers-replaced-jdownloader-installer-downloads-with-malware) | 28.0 | 20.0 | 42.0 |
| [自社ツールを45日間監視して見えてくる本当の攻撃対象領域](https://thehackernews.com/2026/05/what-45-days-of-watching-your-own-tools.html) | 28.0 | 20.0 | 42.0 |
| [OpenAIがTanStackのサプライチェーン攻撃の標的に](https://securityweek.com/openai-hit-by-tanstack-supply-chain-attack) | 25.0 | 45.0 | 42.0 |
| [OpenClawの4件の脆弱性によりデータ窃取、権限昇格、永続化が可能に](https://thehackernews.com/2026/05/four-openclaw-flaws-enable-data-theft.html) | 25.0 | 32.0 | 42.0 |
| [MSPはAI主導のサイバー脅威に対抗するためAIを必要としている、Guardzが指摘](https://cybersecuritydive.com/news/msps-need-ai-to-fight-ai-fueled-cyberthreats-guardz/820371) | 25.0 | 20.0 | 42.0 |
| [Big Techとカナダの暗号化法案、Ciscoの無料AIセキュリティ仕様、Audiアプリの脆弱性](https://securityweek.com/in-other-news-big-tech-vs-canada-encryption-bill-ciscos-free-ai-security-spec-audi-app-flaws) | 25.0 | 20.0 | 42.0 |
| [エージェント型AIを導入する前に慎重に検討すること](https://ncsc.gov.uk/blogs/thinking-carefully-before-adopting-agentic-ai) | 25.0 | 20.0 | 42.0 |
| [Akamai、LayerXを2億500万ドルで買収へ](https://helpnetsecurity.com/2026/05/15/akamai-layerx-acquisition) | 25.0 | 20.0 | 42.0 |
| [TanStackのサプライチェーン攻撃がOpenAI従業員2人の端末に影響、macOSアップデートを強制](https://thehackernews.com/2026/05/tanstack-supply-chain-attack-hits-two.html) | 25.0 | 20.0 | 42.0 |
| [Pwn2Own 2日目にMicrosoft ExchangeとWindows 11がハッキングされる](https://bleepingcomputer.com/news/security/pwn2own-day-two-hackers-demo-microsoft-exchange-windows-11-red-had-enterprise-linux-zero-days) | 22.0 | 20.0 | 43.0 |
| [Metasploitの最新まとめ 2026年5月15日](https://rapid7.com/blog/post/pt-metasploit-wrap-up-05-15-2026) | 22.0 | 20.0 | 42.0 |
| [マチ★アソビ Vol.30会場まとめ、「アミコドームステージ」が初登場で「旧みずほ銀行徳島支店」内覧会も](https://gigazine.net/news/20260516-place-machiasobi30) | 22.0 | 20.0 | 42.0 |
| [米当局、「Cisco SD-WAN」の脆弱性悪用で緊急対応を要請](https://security-next.com/184506) | 22.0 | 20.0 | 42.0 |
| [MITの学長が資金調達と人材育成に関する危機的状況を説明、「率直に言ってこれは国家にとって損失だ」と話す](https://gigazine.net/news/20260515-mit-message-funding-talent-pipeline) | 22.0 | 20.0 | 42.0 |
| [ファミマで服を買う、出張で忘れ物しても24時間営業で丈夫な服を買えて超便利](https://gigazine.net/news/20260515-familymart-conveniencewear-machiasobi30) | 22.0 | 20.0 | 42.0 |
| [自動車メーカーによる個人情報の追跡から逃れるべく自力でモデムとGPSを取り外す](https://gigazine.net/news/20260515-removing-modem-gps-from-car) | 22.0 | 20.0 | 42.0 |

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
