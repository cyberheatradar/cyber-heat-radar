# 📡 サイレーダー 2026-05-11 17:00 JST 試作版

このレポートは、2026-05-10 17:00 JST〜2026-05-11 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 367
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 2
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>音声掲載理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks](#topic-216) | 100.0 | 99.0 | 92.0 | GitHub | - |
| 2 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 74.0 | 82.0 | 81.0 | 音声 | 温度感上位枠 |
| 3 | [「BerriAI LiteLLM」にSQLi脆弱性 - 認証情報漏洩のおそれ、悪用も](#topic-2412) | 43.0 | 46.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](#topic-31) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Hackers abuse Google ads, Claude.ai chats to push Mac malware](#topic-2177) | 34.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [Threats Making WAVs - Incident Response to a Cryptomining Attack](#topic-29) | 30.0 | 20.0 | 42.0 | GitHub | - |
| 7 | [次世代reCAPTCHAがAIによる突破対策のため「Google Play開発者サービス」を必須にしてパズルではなくQRコードスキャンを要求](#topic-2403) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

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
| <nobr>音声掲載理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 74.0 |
| <nobr>実務影響</nobr> | 82.0 |
| <nobr>確度</nobr> | 81.0 |

#### 概要

CVE-2025-60710は、Microsoft WindowsのTaskhost関連の処理に起因するローカル権限昇格の脆弱性として報告されています。
CISAのKnown Exploited Vulnerabilitiesに関連情報があり、公開PoCや検証コードの言及も見られるため、優先的な確認対象とされています。
権限昇格の脆弱性は、侵入後に端末内で攻撃者の権限を大きく広げるおそれがあるため、運用上の影響が大きくなりやすいです。
公開PoCの存在は、再現や悪用のハードルを下げる要因として注意が必要です。

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

- Windows端末で該当CVEへの対策状況を確認し、ベンダー案内に沿って更新を適用すること。
- 管理者権限の付与状況や不要な高権限アカウントを見直し、権限昇格の影響範囲を抑えること。
- 端末監視で不審なタスク実行や権限変更の兆候を確認し、関連イベントを重点的に追跡すること。

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

<a id="topic-2412"></a>

### 2. 「BerriAI LiteLLM」にSQLi脆弱性 - 認証情報漏洩のおそれ、悪用も

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>AI</nobr> |
| <nobr>音声掲載理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 43.0 |
| <nobr>実務影響</nobr> | 46.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

LLMサービス向けプロキシ「BerriAI LiteLLM」にSQLインジェクションの脆弱性が報告され、米当局が悪用を踏まえた注意喚起を行っています。
データベース内の情報が読み取られるおそれがあり、認証情報の漏えいにつながる可能性があるとされています。
LLM基盤や周辺コンポーネントは、利用データや認証情報を集約しやすいため、ひとたび漏えいが起きると影響範囲が大きくなり得ます。
すでに悪用が示唆されているため、早期の確認と対策が重要です。

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

#### 担当者向け確認ポイント

- LiteLLMの利用有無と導入形態を確認し、影響対象のインスタンスを特定する。
- 認証情報や接続先情報を含むデータベース関連の保護状況を点検し、必要に応じてアクセス制御や監査を強化する。
- 提供元の修正版情報や注意喚起を確認し、更新適用と周辺ログの点検を進める。

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

<a id="topic-31"></a>

### 3. PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>防御・運用</nobr> |
| <nobr>音声掲載理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Guardicore Labs による公開情報では、MySQL サーバーを狙うランサムウェアのキャンペーンが確認されています。
攻撃者はデータの公開をちらつかせる二重脅迫の手口を用い、被害組織に圧力をかけているとされています。
MySQL は業務システムの基盤として広く使われるため、侵害されると業務停止や情報漏えいの影響が大きくなり得ます。
ランサムウェアと二重脅迫の組み合わせは、復旧だけでなく情報管理面でも対応負荷を高めます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- MySQL の公開設定、認証強度、不要な外部到達性を点検する。
- バックアップの分離保管と復元手順の定期確認を行い、復旧可能性を検証する。
- データベース周辺の監視を強化し、異常な接続やデータ流出の兆候を早期に把握する。

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

<a id="topic-2177"></a>

### 4. Hackers abuse Google ads, Claude.ai chats to push Mac malware

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>マルウェア</nobr> / <nobr>攻撃キャンペーン</nobr> |
| <nobr>音声掲載理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 34.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Hackers abuse Google ads, Claude.ai chats to push Mac malware は、AIを攻撃者側の自動化・詐欺・マルウェア・フィッシングに利用する話題です。
攻撃手口、標的、検知観点、利用者教育やSOC監視への反映要否を確認する価値があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 攻撃者がAIを使っている工程と、既存の検知・教育で補足できる範囲を確認する。
- フィッシング、マルウェア、詐欺テンプレート、認証情報窃取の観点で検知ロジックを確認する。
- SOC/CSIRTで共有すべきIoC、TTP、注意喚起文面があるか確認する。
- 利用者向け注意喚起や訓練内容を更新する必要があるか確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ai_model_or_project | Claude | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Hackers abuse Google ads, Claude.ai chats to push Mac malware](https://bleepingcomputer.com/news/security/hackers-abuse-google-ads-claudeai-chats-to-push-mac-malware) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 弱。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-2403"></a>

### 5. 次世代reCAPTCHAがAIによる突破対策のため「Google Play開発者サービス」を必須にしてパズルではなくQRコードスキャンを要求

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>Android</nobr> / <nobr>AI</nobr> |
| <nobr>音声掲載理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
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

#### 担当者向け確認ポイント

- 攻撃者、標的業種、対象地域を確認する。
- 公開されたTTP、IoC、検知ロジックを確認する。
- 自組織のログ・EDR・SIEMで検知可能か確認する。
- 初期侵入経路、横展開、永続化、情報窃取の有無を確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [次世代reCAPTCHAがAIによる突破対策のため「Google Play開発者サービス」を必須にしてパズルではなくQRコードスキャンを要求](https://gigazine.net/news/20260511-google-new-recaptcha-needs-google-play-services) | <nobr>内容確認・補足情報</nobr> |

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

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-216"></a>

### 1. CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>KEV</nobr> / <nobr>認証バイパス</nobr> / <nobr>防御・運用</nobr> / <nobr>政策・規制</nobr> / <nobr>脅威レポート</nobr> / <nobr>PoC</nobr> / <nobr>ボットネット</nobr> / <nobr>ゼロデイ</nobr> |
| <nobr>温度状態</nobr> | 高温 |
| <nobr>温度感</nobr> | 100.0 |
| <nobr>実務影響</nobr> | 99.0 |
| <nobr>確度</nobr> | 92.0 |

#### 概要

CVE-2026-41940は、WebProsのcPanel & WHMおよびWP2（WordPress Squared）に関連する認証回避の脆弱性で、CISAのKEVカタログに追加されています。
公開情報では、実際の悪用が確認されており、ランサムウェア攻撃や標的型の侵害文脈でも言及されています。
管理系コントロールパネルへの不正アクセスにつながる可能性があるため、影響は大きいと見られます。
公開PoCの言及もあり、未対策環境では短期間で悪用リスクが高まりやすい点が注目されています。

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
- 複数ソースで確認: 7 sources。
- CISA KEV関連。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
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

- cPanel & WHM / WP2の利用有無を確認し、ベンダーの修正情報と適用状況を点検する。
- 外部公開された管理画面や関連サービスのアクセス制御を見直し、不要な露出を減らす。
- 認証回避や管理者権限の不審な操作、設定変更、ログイン痕跡を重点的に監視する。

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
| <nobr>出典</nobr> | [Week in review: cPanel vulnerability actively exploited, DigiCert breach, Linked](https://helpnetsecurity.com/2026/05/10/week-in-review-cpanel-vulnerability-actively-exploited-digicert-breach-linkedin-job-scams) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [4th May – Threat Intelligence Report](https://research.checkpoint.com/2026/4th-may-threat-intelligence-report) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [South-East Asian Military Entities Targeted via cPanel (CVE-2026-41940)](https://ctrlaltintel.com/research/SEA-CPanel) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Vulnerability Alert: CVE-2026-41940 in cPanel, WHM, and WP Squared](https://bitsight.com/blog/critical-vulnerability-alert-cve-2026-41940-cPanel-WHM-WPSquared) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://cisa.gov/news-events/alerts/2026/04/30/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

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

<a id="topic-29"></a>

### 2. Threats Making WAVs - Incident Response to a Cryptomining Attack

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
| [Ollamaの境界外読み取り脆弱性によりリモートでプロセスメモリが漏えいする問題](https://thehackernews.com/2026/05/ollama-out-of-bounds-read-vulnerability.html) | 28.0 | 46.0 | 50.0 |
| [CVE-2026-44656: Vimの「path」補完によるOSコマンドインジェクション](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-44656) | 28.0 | 46.0 | 38.0 |
| [Netskopeにおけるクロステナント認証バイパスの脆弱性](https://blog.amberwolf.com/blog/2025/august/advisory---netskope-cross-tenant-authentication-bypass) | 28.0 | 38.0 | 42.0 |
| [Oracle of Delphiが認証情報を窃取する](https://akamai.com/blog/security/the-oracle-of-delphi-steal-your-credentials) | 28.0 | 20.0 | 42.0 |
| [Nansh0uキャンペーン：ハッカーの武器庫がさらに強化](https://akamai.com/blog/security/the-nansh0u-campaign-hackers-arsenal-grows-stronger) | 28.0 | 20.0 | 42.0 |
| [5年以上にわたるフィッシングキャンペーンで500以上の組織が被害](https://securityweek.com/over-500-organizations-hit-in-years-long-phishing-campaign) | 28.0 | 20.0 | 42.0 |
| [Electerm projectのElectermにおける複数の脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-014913.html) | 28.0 | 20.0 | 42.0 |
| [Palo Alto NetworksのPAN-OSにおける境界外書き込みに関する脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-014858.html) | 28.0 | 20.0 | 42.0 |
| [LinuxのLinux Kernelにおける境界外書き込みに関する脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-014806.html) | 27.0 | 23.0 | 43.0 |
| [デジタルコンテンツや生成AIのアーカイブを保存する非営利財団「インターネットアーカイブ・スイス」設立](https://gigazine.net/news/20260511-internet-archive-switzerland) | 27.0 | 20.0 | 42.0 |
| [ヒンドゥー教・シーク教・モルモン教などの指導者とAnthropicやOpenAIなどのAI企業が会合、AIモデルに倫理と道徳を組み込む方法に関する原則を策定へ](https://gigazine.net/news/20260511-ai-and-religion-faith-ai-covenant) | 27.0 | 20.0 | 42.0 |
| [Mervin Praison (MervinPraison)のPraisonAIにおける複数の脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-014907.html) | 27.0 | 20.0 | 42.0 |
| [sandboxie-plusのSandboxieにおけるスタックベースのバッファオーバーフローの脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-014792.html) | 27.0 | 20.0 | 42.0 |
| [MUFG、購買や決済などのAIエージェントを開発--戦略パートナーにグーグル](https://japan.zdnet.com/article/35247279) | 26.0 | 20.0 | 42.0 |
| [MUFGがGoogleと戦略的提携 リテール総合金融、AIでSMBCより「先行」狙う](https://xtech.nikkei.com/atcl/nxt/column/18/00001/11718) | 26.0 | 20.0 | 42.0 |
| [ソニーが打ち出した「AIによる成長」と“ただし書き”の中身 26年度経営方針説明会](https://itmedia.co.jp/news/articles/2605/11/news089.html) | 26.0 | 20.0 | 42.0 |
| [“ChatGPT以後”に公開のWebサイト、35％がAI生成に？ 米スタンフォード大などが調査 広まる「不自然に明るい文章」](https://itmedia.co.jp/news/articles/2605/11/news027.html) | 26.0 | 20.0 | 42.0 |
| [AIエージェント開発は「正解」なのか、日経BPのAI・データラボ所長が解説](https://xtech.nikkei.com/atcl/nxt/column/18/03585/050800002) | 26.0 | 20.0 | 42.0 |
| [LINEヤフーのAIエージェント「Agent i」、日本での強みを生かせるか](https://xtech.nikkei.com/atcl/nxt/column/18/00086/00402) | 26.0 | 20.0 | 42.0 |

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
