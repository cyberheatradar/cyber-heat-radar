# 📡 サイレーダー 2026-05-11 11:00 JST 試作版

このレポートは、2026-05-10 11:00 JST〜2026-05-11 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 130
- [音声で扱う想定のトピック](#audio-topics): 0
- [GitHubのみ掲載想定のトピック](#github-only-topics): 5
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>音声掲載理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks](#topic-216) | 100.0 | 99.0 | 92.0 | GitHub | - |
| 2 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 74.0 | 82.0 | 81.0 | GitHub | - |
| 3 | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](#topic-31) | 36.0 | 30.0 | 42.0 | GitHub | - |
| 4 | [Hackers abuse Google ads, Claude.ai chats to push Mac malware](#topic-2177) | 34.0 | 20.0 | 42.0 | GitHub | - |
| 5 | [Threats Making WAVs - Incident Response to a Cryptomining Attack](#topic-29) | 30.0 | 20.0 | 42.0 | GitHub | - |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

今回は音声で扱う想定のトピックはありません。

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

CVE-2026-41940は、WebProsのcPanel & WHMおよびWP Squaredに存在する認証回避の脆弱性として公表され、CISAのKEV Catalogにも追加されています。
公開情報では、実際の悪用が確認されており、ランサムウェア攻撃との関連も示されています。
cPanel/WHMはホスティング運用の中核に関わるため、侵害されると広範囲に影響が及ぶおそれがあります。公開PoCの言及もあるため、未対策環境では迅速な確認と対応が重要です。

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

- cPanel & WHM / WP Squaredの該当バージョンを確認し、ベンダーの修正版・回避策があれば直ちに適用する。
- インターネット公開された管理画面や関連サービスのアクセス制御、認証ログ、異常な管理操作の有無を点検する。
- KEV掲載脆弱性として優先度を上げ、他の管理系製品や同一基盤上の不審な変更・永続化の兆候もあわせて確認する。

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

<a id="topic-12"></a>

### 2. Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>Windows</nobr> / <nobr>権限昇格</nobr> / <nobr>TTP</nobr> / <nobr>脆弱性</nobr> / <nobr>KEV</nobr> |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 74.0 |
| <nobr>実務影響</nobr> | 82.0 |
| <nobr>確度</nobr> | 81.0 |

#### 概要

CVE-2025-60710は、Microsoft WindowsのTaskhost関連の処理におけるローカル権限昇格の脆弱性として扱われています。
CISAのKnown Exploited Vulnerabilitiesにも掲載されており、公開PoCの言及もあるため、実務上は優先確認対象と考えられます。
権限昇格の脆弱性は、最初の侵入後に被害を拡大させる足がかりになりやすい点が重要です。さらに、KEV掲載は実際の悪用リスクを示す材料として、対応優先度を上げる根拠になります。

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

- 対象Windows環境でCVE-2025-60710の影響有無を確認し、ベンダーの修正情報や回避策を確認する。
- Taskhost関連の異常な実行や権限変化、予定外のタスク操作がないか監視する。
- 公開PoCの存在を踏まえ、該当端末の優先度を上げてパッチ適用と検出ルールの見直しを進める。

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

### 3. PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>防御・運用</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

AkamaiのSecurity Intelligenceによると、Guardicore LabsはMySQLサーバーを標的とするランサムウェア関連のキャンペーンを確認しました。
攻撃者は二重脅迫の手法を用い、データ公開をちらつかせて被害組織に圧力をかけているとされています。
MySQLは多くの業務システムやアプリケーションの基盤で使われるため、侵害されると広範囲の業務停止や情報漏えいにつながるおそれがあります。
ランサムウェアは暗号化だけでなくデータ流出も組み合わせることがあり、復旧と対外対応の負担が大きくなります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- MySQLサーバーの公開範囲、認証設定、パッチ適用状況を点検する。
- バックアップが実際に復元できるかを定期的に確認し、重要データの保全体制を見直す。
- 不審な認証試行や設定変更、データ転送の兆候を監視し、インシデント対応手順を再確認する。

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
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>マルウェア</nobr> / <nobr>攻撃キャンペーン</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 34.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

攻撃者がGoogle広告とClaude.aiの共有チャットを悪用し、Mac向けマルウェアへ誘導するキャンペーンが報告されています。
検索結果上では正規のサービスに見える導線が使われるため、利用者が不審な手順や配布物に気づきにくい点が特徴です。
正規サービスや広告枠を経由するため、見た目の信頼性に惑わされやすく、エンドユーザーの初動を誤らせるリスクがあります。
AIサービスの共有機能や検索広告が攻撃の足場として使われうる点は、運用・教育の両面で注意が必要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 検索広告経由のダウンロード導線をそのまま信頼せず、配布元ドメインと入手経路を確認する。
- AIチャットの共有リンクや外部に公開された手順書を経由した不審な案内に注意し、社内では正規のインストール手順を明示する。
- Mac端末でも不審なプロファイル、権限要求、未知のインストーラに警戒し、検知・教育を見直す。

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
| [Security: Netskopeのクロステナント認証バイパス](https://blog.amberwolf.com/blog/2025/august/advisory---netskope-cross-tenant-authentication-bypass) | 28.0 | 38.0 | 42.0 |
| [Oracle of Delphi が認証情報を窃取する](https://akamai.com/blog/security/the-oracle-of-delphi-steal-your-credentials) | 28.0 | 20.0 | 42.0 |
| [Nansh0uキャンペーン：ハッカーの攻撃手法がさらに強化される](https://akamai.com/blog/security/the-nansh0u-campaign-hackers-arsenal-grows-stronger) | 28.0 | 20.0 | 42.0 |
| [AI生成画像の背景を透明化するのに役立つ画像背景削除ツール「Rembg」](https://gigazine.net/news/20260510-rembg) | 27.0 | 20.0 | 42.0 |
| [クリエイターの創造力を拡張、コロプラが作った「世界初」の生成AIゲーム](https://xtech.nikkei.com/atcl/nxt/column/18/03076/050700025) | 26.0 | 20.0 | 42.0 |
| [LINEヤフーのAIエージェント「Agent i」、日本での強みを生かせるか](https://xtech.nikkei.com/atcl/nxt/column/18/00086/00402) | 26.0 | 20.0 | 42.0 |
| [AIエージェント開発は「正解」なのか、日経BPのAI・データラボ所長が解説](https://xtech.nikkei.com/atcl/nxt/column/18/03585/050800002) | 26.0 | 20.0 | 42.0 |
| [Googleの廉価版スマホ「Google Pixel 10a」のベンチマークスコアやバッテリー持続時間を検証してみたよレビュー](https://gigazine.net/news/20260510-google-pixel-10a-benchmark-battery) | 25.0 | 20.0 | 43.0 |
| [OpenAI Sora 2のセキュリティ分析：マルチモーダルLLMを駆動するシステムプロンプトの解明](https://mindgard.ai/resources/openai-sora-system-prompts) | 25.0 | 20.0 | 42.0 |
| [必見：Geminiをハッキングする多層的アプローチ](https://buganizer.cc/hacking-gemini-a-multi-layered-approach-md) | 25.0 | 20.0 | 42.0 |
| [YARA-X 1.16.0のリリース](https://isc.sans.edu/diary/rss/32970) | 25.0 | 20.0 | 42.0 |
| [あなたのパスワードは何分耐えられる？ 解析速度上昇で「8文字パスワード」はほぼ無力に](https://itmedia.co.jp/enterprise/articles/2605/11/news036.html) | 24.0 | 20.0 | 43.0 |
| [「Linuxカーネル」の暗号通信処理にLoP脆弱性「Dirty Frag」](https://security-next.com/184228) | 24.0 | 20.0 | 42.0 |
| [Citrix NetScalerのメモリリークと反射型XSS（CVE-2025-12101）](https://bit.ly/48bPzCO) | 23.0 | 34.0 | 50.0 |
| [CVE-2026-39826 html/template の Escaper 回避により XSS が発生する脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-39826) | 23.0 | 34.0 | 38.0 |
| [CVE-2026-39823: html/templateのmeta content URLエスケープ回避によるXSS脆弱性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-39823) | 23.0 | 34.0 | 38.0 |
| [MixMaster MMORPGのリバースエンジニアリングに関するセキュリティ情報](https://3r4y.github.io/posts/mixmasterreverseengineering) | 22.0 | 20.0 | 42.0 |

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
