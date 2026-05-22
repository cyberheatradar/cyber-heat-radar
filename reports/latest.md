# 📡 サイレーダー 2026-05-23 05:00 JST

このレポートは、2026-05-22 17:00 JST〜2026-05-23 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 97
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-9082: CISA KEV catalog addition](#topic-8272) | 47.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 2 | [CISA’s new KEV nomination form opens reporting to vendors and researchers](#topic-8595) | 38.0 | 38.0 | 51.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [$20 per zero-day is already the WordPress plugin reality](#topic-9273) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Trend Micro warns of Apex One zero-day exploited in the wild](#topic-9274) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [CVE-2025-20333: Cisco ASA/FTD persistence mechanism update](#topic-203) | 33.0 | 46.0 | 62.0 | 音声 | 温度感上位枠 |
| 6 | [Fake Gemini and Claude Code Sites Spread Infostealers Through SEO Poisoning](#topic-9288) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-8272"></a>

### 1. CVE-2026-9082: CISA KEV catalog addition

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>KEV</nobr> / <nobr>RCE</nobr> / <nobr>権限昇格</nobr> / <nobr>TTP</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 47.0 |
| <nobr>実務影響</nobr> | 64.0 |
| <nobr>確度</nobr> | 63.0 |

#### 概要

CISAは、Drupal Coreの脆弱性CVE-2026-9082をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
公開情報では、Drupalはすでにこの脆弱性に対する悪用の試みを確認しており、影響範囲は認証なしでの情報漏えい、権限昇格、リモートコード実行につながる可能性があるとされています。
KEV追加は、実際に悪用が確認された脆弱性として優先対応が求められることを意味します。
Drupalを利用する組織では、Webサイトや関連サービスの被害防止のため、修正適用の優先度が高い案件です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 情報漏えい系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Drupal Coreの該当修正版が適用済みかを確認し、未適用なら早急に対応する。
- 公開中のDrupalサイトで不審な挙動や改ざん、情報流出の兆候がないか点検する。
- KEV対象として、資産棚卸しと脆弱性管理の優先順位を上げる。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-9082 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-9082](https://nvd.nist.gov/vuln/detail/CVE-2026-9082) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Drupal Vulnerability in Hacker Crosshairs Shortly After Disclosure](https://www.securityweek.com/drupal-vulnerability-in-hacker-crosshairs-shortly-after-disclosure/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/05/22/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Drupal Patches Highly Critical Vulnerability Exposing Websites to Hacking](https://www.securityweek.com/drupal-patches-highly-critical-vulnerability-exposing-websites-to-hacking/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-9082: Mitigating a Critical SQL Injection Vulnerability in Drupal](https://www.akamai.com/blog/security-research/2026/may/cve-2026-9082-mitigating-critical-sql-injection-drupal) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Highly Critical Drupal Core Flaw Exposes PostgreSQL Sites to RCE Attacks](https://thehackernews.com/2026/05/highly-critical-drupal-core-flaw.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-9273"></a>

### 2. $20 per zero-day is already the WordPress plugin reality

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>ゼロデイ</nobr> / <nobr>AIエージェント</nobr> / <nobr>脆弱性</nobr> / <nobr>MCP</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

WordPressプラグインを対象に、AIを使った脆弱性発見の取り組みが紹介されました。
研究者らは短期間で構築したパイプラインにより、静的解析と動的検証を組み合わせて実際の不具合を見つけられる可能性を示したとされています。
AIが脆弱性調査の効率をどこまで高められるかは、攻撃面の拡大と防御側の検証能力の両面で注目されています。
WordPressは利用範囲が広いため、プラグインの品質管理や検証体制への関心が高まる話題です。

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

- WordPressプラグインの更新状況と、未修正の既知脆弱性がないかを継続確認する。
- AI支援の検出結果は過信せず、再現性と誤検知の切り分けを前提に評価する。
- プラグイン導入時は提供元の保守状況、更新頻度、権限設定を見直す。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [$20 per zero-day is already the WordPress plugin reality](https://www.helpnetsecurity.com/2026/05/22/ai-wordpress-plugin-vulnerabilities/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-9274"></a>

### 3. Trend Micro warns of Apex One zero-day exploited in the wild

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ゼロデイ</nobr> / <nobr>KEV</nobr> / <nobr>Windows</nobr> / <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Trend Microは、Apex Oneに存在するゼロデイ脆弱性について注意喚起し、Windowsを狙った攻撃で悪用が確認されているとしています。
現時点では、詳細な影響範囲や攻撃の広がりについては公開情報の範囲で慎重に見る必要があります。
ゼロデイで実際の悪用が確認されている点は、修正前の製品利用者に直接的なリスクがあるため注目されています。
エンドポイント防御製品に関わる問題であり、対応の遅れが被害拡大につながる可能性があります。

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

- Apex Oneの利用有無を確認し、ベンダーの案内に従って更新や緩和策を早急に適用する。
- 管理対象端末で不審な挙動や未承認の操作痕跡がないかを点検する。
- 関連するログや検知ルールを見直し、同種の攻撃兆候を監視できる状態にしておく。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Trend Micro warns of Apex One zero-day exploited in the wild](https://www.bleepingcomputer.com/news/security/trend-micro-warns-of-apex-one-zero-day-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-203"></a>

### 4. CVE-2025-20333: Cisco ASA/FTD persistence mechanism update

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>TTP</nobr> / <nobr>防御・運用</nobr> / <nobr>RCE</nobr> / <nobr>ランサムウェア</nobr> / <nobr>脅威アクター</nobr> / <nobr>Linux</nobr> / <nobr>ゼロデイ</nobr> / <nobr>フィッシング</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 46.0 |
| <nobr>確度</nobr> | 62.0 |

#### 概要

CISAとCiscoは、Cisco Secure Firewall ASA/FTD製品に関連する脆弱性対応の更新を公表し、攻撃者が修正後も残る持続化の仕組みを確認したとしています。
初期侵入は、修正前に存在したCVE-2025-20333およびCVE-2025-20362の悪用から始まった可能性が示されています。
境界機器に関わる侵害は、組織内ネットワーク全体への影響につながるおそれがあるため注目されています。
修正適用後も残り得る持続化の可能性が示されたことで、単純なアップデートだけでは安心できない点が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 中。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Cisco ASA/FTDおよび関連プラットフォームで、修正済みリリースへの更新状況と適用漏れがないか確認する。
- 侵害の有無を、設定変更や不審な管理動作だけでなく、ベンダーや公的機関の案内に沿って点検する。
- 境界機器の監視を強化し、異常な認証・VPN利用・管理アクセスの兆候を継続的に確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-20333 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-20333](https://nvd.nist.gov/vuln/detail/CVE-2025-20333) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [From edge appliance to enterprise compromise: Multi-stage Linux intrusion via F5](https://www.microsoft.com/en-us/security/blog/2026/05/22/from-edge-appliance-to-enterprise-compromise-multi-stage-linux-intrusion-via-f5-and-confluence/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>公的・一次情報</nobr> | [Continued Evolution of Persistence Mechanism Against Cisco Secure Firewall Adapt](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-persist-CISAED25-03) | <nobr>内容確認・補足情報</nobr> |
| <nobr>公的・一次情報</nobr> | [Weekly Report: JPCERT/CCが「Cisco ASAおよびFTDにおける複数の脆弱性（CVE-2025-20333、CVE-2025-2036](https://www.jpcert.or.jp/wr/2026/wr260430.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>公的・一次情報</nobr> | [注意喚起: Cisco ASAおよびFTDにおける複数の脆弱性（CVE-2025-20333、CVE-2025-20362）に関する注意喚起  (更新)](https://www.jpcert.or.jp/at/2025/at250021.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [It pays to be a forever student](https://blog.talosintelligence.com/it-pays-to-be-a-forever-student/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [UAT-4356's Targeting of Cisco Firepower Devices](https://blog.talosintelligence.com/uat-4356-firestarter/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [IR Trends Q1 2026: Phishing reemerges as top initial access vector, as attacks t](https://blog.talosintelligence.com/ir-trends-q1-2026/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: あり。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 中。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-9288"></a>

### 5. Fake Gemini and Claude Code Sites Spread Infostealers Through SEO Poisoning

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>マルウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

検索エンジン最適化を悪用して、GeminiやClaude Codeを装う偽サイトへ誘導し、情報窃取型マルウェアを配布するキャンペーンが報告されています。
公開情報では、盗まれる対象にはコラボレーション系の認証情報や暗号資産ウォレットなど、幅広いデータが含まれるとされています。
生成AI関連サービスを装う偽サイトは、利用者の警戒心を下げやすく、正規サイトと見分けにくい点が問題です。
認証情報やウォレット情報が含まれるため、個人被害だけでなく、業務環境への侵害や二次被害にもつながるおそれがあります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 検索経由で配布される偽サイトやスポンサーリンクを前提に、正規ドメイン確認を徹底する。
- コラボレーションツールやAIサービスの認証情報、セッション情報の保護を見直す。
- 情報窃取型マルウェアを想定し、端末側のEDR監視や不審なダウンロード検知を強化する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ai_model_or_project | Claude | 主題 | 0.80 |
| ai_model_or_project | Gemini | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Fake Gemini and Claude Code Sites Spread Infostealers Through SEO Poisoning](https://www.infosecurity-magazine.com/news/gemini-claude-infostealers-seo/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-8595"></a>

### 1. CISA’s new KEV nomination form opens reporting to vendors and researchers

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>KEV</nobr> / <nobr>脆弱性</nobr> / <nobr>CVE</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 38.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 51.0 |

#### 概要

CISAは、既知の悪用が確認された脆弱性を公開リストに載せるための新しいノミネーションフォームを公開し、ベンダーや研究者が報告しやすくしました。
あわせて、KEVカタログには複数の脆弱性が追加されており、Microsoft Defender関連の問題も含まれています。
公的な優先順位付けの対象に入る脆弱性が増え、組織側は修正や監視の優先度を見直す必要があります。
外部からの報告経路が整備されたことで、悪用が確認された脆弱性がより早く可視化される可能性があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- KEVカタログへの追加有無を定期確認し、該当製品の修正状況を把握する。
- Microsoft Defenderを含む対象製品は、ベンダー情報と資産棚卸しを突き合わせて影響範囲を確認する。
- 外部公開情報だけで判断せず、検知ログや脅威インテリジェンスと合わせて優先度を決める。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-34291 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [CISA’s new KEV nomination form opens reporting to vendors and researchers](https://www.helpnetsecurity.com/2026/05/22/cisa-kev-nomination-form/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds Exploited Langflow and Trend Micro Apex One Vulnerabilities to KEV](https://thehackernews.com/2026/05/cisa-adds-exploited-langflow-and-trend.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Defender vulnerabilities are being exploited in the wild](https://www.malwarebytes.com/blog/bugs/2026/05/microsoft-defender-vulnerabilities-are-being-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [25のランサムウェアグループに利用されていたVPN、国際共同摘発で初めて摘発](https://thehackernews.com/2026/05/first-vpn-dismantled-in-global-takedown.html) | 28.0 | 30.0 | 42.0 |
| [Verizon DBIR: 医療業界が増加するソーシャルエンジニアリング攻撃を撃退](https://www.darkreading.com/cyber-risk/verizon-dbir-healthcare-fends-off-increased-social-engineering-attacks) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア関連の法執行・司法措置](https://www.securityweek.com/first-vpn-cybercrime-service-disrupted-administrator-arrested/) | 28.0 | 30.0 | 42.0 |
| [Microsoft 365ユーザーを標的にしたMFAを回避する新たなフィッシング脅威](https://www.helpnetsecurity.com/2026/05/22/kali365-microsoft-365-phishing-fbi-warning/) | 28.0 | 20.0 | 48.0 |
| [オランダ、サイバー攻撃を助長したホスティング会社の800台のサーバーを押収](https://www.bleepingcomputer.com/news/security/netherlands-seizes-800-servers-of-hosting-firm-enabling-cyberattacks/) | 28.0 | 20.0 | 42.0 |
| [Kazuarがバックドアから堅牢なスパイ活動エコシステムへ進化](https://blog.polyswarm.io/kazuar-evolves-from-backdoor-to-resilient-espionage-ecosystem) | 28.0 | 20.0 | 42.0 |
| [GhostwriterがPrometheusフィッシングマルウェアでウクライナ政府機関を標的にする](https://thehackernews.com/2026/05/ghostwriter-targets-ukraine-government.html) | 28.0 | 20.0 | 42.0 |
| [Fast and Furious: イラン紛争中のNimbus Manticoreの活動](https://research.checkpoint.com/2026/fast-and-furious-nimbus-manticore-operations-during-the-iranian-conflict/) | 28.0 | 20.0 | 42.0 |
| [Canadian man arrested, charged for running KimWolf DDoSボットネット](https://therecord.media/canadian-man-arrested-charged-running-kimwolf-botnet) | 28.0 | 20.0 | 42.0 |
| [イランのAPTグループScreening Serpensによる2026年のスパイ活動キャンペーンの追跡](https://unit42.paloaltonetworks.com/tracking-iran-apt-screening-serpens/) | 28.0 | 20.0 | 42.0 |
| [Kimwolfボットネットを運用したカナダ人が逮捕される](https://www.securityweek.com/canadian-man-arrested-for-operating-kimwolf-botnet/) | 28.0 | 20.0 | 42.0 |
| [Megalodon、悪意あるCI/CDワークフローで5,561件のGitHubリポジトリを標的に攻撃](https://thehackernews.com/2026/05/megalodon-github-attack-targets-5561.html) | 28.0 | 20.0 | 42.0 |
| [DDoS請負サービス運営に関与した疑いでKimWolfボットネット管理者を逮捕](https://www.helpnetsecurity.com/2026/05/22/kimwolf-ddos-botnet-administrator-arrested/) | 28.0 | 20.0 | 42.0 |
| [ROADtoolsと国家レベルの戦術が織りなすクラウド上の意図的な道筋](https://unit42.paloaltonetworks.com/roadtools-cloud-attacks/) | 28.0 | 20.0 | 42.0 |
| [米国とカナダ、Kimwolfボットネットの管理者とみられる人物を逮捕・起訴](https://www.bleepingcomputer.com/news/security/us-and-canada-arrest-and-charge-suspected-kimwolf-botnet-admin/) | 28.0 | 20.0 | 42.0 |
| [カナダでDDoS代行攻撃の運営者Kimwolfボットネット管理者を逮捕](https://thehackernews.com/2026/05/kimwolf-ddos-botnet-operator-arrested.html) | 28.0 | 20.0 | 42.0 |
| [Microsoft Securityの成功事例：St. Luke’sとManpowerGroupはいかにAI基盤を守っているか](https://www.microsoft.com/en-us/security/blog/2026/05/22/microsoft-security-success-stories-how-st-lukes-and-manpowergroup-are-securing-ai-foundations/) | 27.0 | 20.0 | 42.0 |
| [AIシステムを過信せず恐れすぎずに守るために 第2回：攻撃対象領域とチェックポイントフロー](https://blog.nviso.eu/2026/05/22/securing-ai-systems-without-overconfidence-or-fear-part-2-attack-surfaces-and-the-checkpoint-flow/) | 27.0 | 20.0 | 42.0 |
| [ハードウェアなしで脆弱なドライバを悪用可能にするBYOVDの視点](https://thehackernews.com/2026/05/making-vulnerable-drivers-exploitable.html) | 25.0 | 23.0 | 43.0 |
| [Kore.ai、企業向けマルチエージェントシステムのためのAIネイティブ・プラットフォームを発表](https://www.helpnetsecurity.com/2026/05/22/kore-ai-unveils-ai-native-platform-for-enterprise-multiagent-systems/) | 25.0 | 20.0 | 42.0 |
| [Versa、AIエージェントとMCPワークフローにゼロトラスト原則を拡張](https://www.helpnetsecurity.com/2026/05/22/versa-extends-zero-trust-principles-to-ai-agents-and-mcp-workflows/) | 25.0 | 20.0 | 42.0 |
| [GitLab 19.0にAIワークフロー、シークレット管理、セルフホスト型モデル対応を追加](https://www.helpnetsecurity.com/2026/05/22/gitlab-19-0-adds-ai-workflows-secrets-management-and-self-hosted-model-support/) | 25.0 | 20.0 | 42.0 |
| [Proton Pass、AIエージェント向けの監視付き認証情報共有機能を追加](https://www.helpnetsecurity.com/2026/05/22/proton-pass-adds-monitored-credential-sharing-for-ai-agents/) | 25.0 | 20.0 | 42.0 |
| [Microsoft、Forrester Wave™ の Workforce Identity Security Platforms でリーダーに認定](https://www.microsoft.com/en-us/security/blog/2026/05/22/microsoft-recognized-as-a-leader-in-the-forrester-wave-for-workforce-identity-security-platforms/) | 22.0 | 20.0 | 42.0 |

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
