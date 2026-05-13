# 📡 サイレーダー 2026-05-14 05:00 JST 試作版

このレポートは、2026-05-13 17:00 JST〜2026-05-14 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 142
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 6
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [Microsoft 2026年5月 Patch Tuesday 関連まとめ](#topic-3472) | 76.0 | 56.0 | 58.0 | GitHub | 直近掲載済み・再掲抑制 |
| 2 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 74.0 | 82.0 | 81.0 | GitHub | 直近掲載済み・再掲抑制 |
| 3 | [Microsoft Patches Critical Zero-Click Outlook Vulnerability Threatening Enterprises](#topic-3625) | 52.0 | 64.0 | 57.0 | 音声 | 温度感上位枠 |
| 4 | [When IT Support Calls: Dissecting a ModeloRAT Campaign from Teams to Domain Compromise](#topic-4269) | 40.0 | 35.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](#topic-31) | 36.0 | 30.0 | 42.0 | GitHub | 直近掲載済み・再掲抑制 |
| 6 | [Canvas owner reaches ‘agreement’ with threat actors after data breach](#topic-4189) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 7 | [Pwn2Own Berlin 2026: The Full Schedule](#topic-4237) | 35.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 8 | [Weaponized AI: The new frontier of fraud and identity spoofing](#topic-4232) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 9 | [ランサム被害で個人情報流出の可能性 - エネサンスHD](#topic-4118) | 30.0 | 30.0 | 42.0 | GitHub | audio_slots_filled_or_ranked_below_selected_topics |
| 10 | [Threats Making WAVs - Incident Response to a Cryptomining Attack](#topic-29) | 30.0 | 20.0 | 42.0 | GitHub | 直近掲載済み・再掲抑制 |
| 11 | [人気ノートアプリ「Obsidian」がプラグイン審査を刷新、マルウェア検査や安全性表示を導入へ](#topic-4219) | 30.0 | 20.0 | 42.0 | GitHub | audio_slots_filled_or_ranked_below_selected_topics |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-3625"></a>

### 1. Microsoft Patches Critical Zero-Click Outlook Vulnerability Threatening Enterprises

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>RCE</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 52.0 |
| <nobr>実務影響</nobr> | 64.0 |
| <nobr>確度</nobr> | 57.0 |

#### 概要

Microsoftは2026年5月の月例更新で多数の脆弱性修正を公開し、その中にCVE-2026-40361を含むMicrosoft Word関連の深刻な脆弱性が含まれています。
公開情報では、未認証の攻撃者によるコード実行につながる可能性が示されており、Outlook/Office利用環境では優先的な確認が必要とされています。
Office製品は企業利用が広く、影響範囲が大きくなりやすいため、文書の取り扱いを起点にしたリスクとして注目されています。
ゼロクリック系として報じられている点もあり、利用者の操作を前提にしない脅威として警戒されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Microsoftの更新情報を確認し、該当するOffice/Wordの修正適用状況を優先的に点検する。
- メールや文書の受け渡しが多い環境では、関連製品の保護機能や隔離設定、添付ファイル検査の運用を見直す。
- 同系統のMicrosoft Office脆弱性が併せて修正されている可能性があるため、単一CVEではなく月例パッチ全体で影響を確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-40361 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40364 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-40361](https://nvd.nist.gov/vuln/detail/CVE-2026-40361) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches Critical Zero-Click Outlook Vulnerability Threatening Enterpri](https://securityweek.com/microsoft-patches-critical-zero-click-outlook-vulnerability-threatening-enterprises) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft May 2026 Patch Tuesday: Many fixes, but no zero-days](https://helpnetsecurity.com/2026/05/12/microsoft-may-2026-patch-tuesday) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-40361 Microsoft Word Remote Code Execution Vulnerability](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-40361) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 継続。

---

<a id="topic-4269"></a>

### 2. When IT Support Calls: Dissecting a ModeloRAT Campaign from Teams to Domain Compromise

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>TTP</nobr> / <nobr>Windows</nobr> / <nobr>IoC</nobr> / <nobr>ボットネット</nobr> / <nobr>権限昇格</nobr> / <nobr>CVE</nobr> / <nobr>脅威アクター</nobr> / <nobr>脆弱性</nobr> / <nobr>マルウェア</nobr> / <nobr>防御・運用</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 40.0 |
| <nobr>実務影響</nobr> | 35.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Rapid7は、偽の「IT Support」を装ったMicrosoft Teamsのメッセージを起点に、マルウェア配布、権限昇格、認証情報の窃取、横展開へ進んだ侵害事例を分析しました。
攻撃にはPythonベースのModeloRAT系の挙動が見られ、既知のWindows脆弱性（CVE-2023-36036）も悪用されたとされています。
コラボレーションツールを起点に、端末侵害からID基盤のリスクへ短時間で拡大しうることを示しています。
既知の脆弱性、正規ツール、ソーシャルエンジニアリングが組み合わさると、従来の境界防御だけでは見逃されやすくなります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 技術詳細により影響確認が進みやすい。
- 権限昇格系。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 技術詳細・再現情報あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 技術詳細、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Teamsなど外部チャット経由のなりすまし連絡を前提に、外部アクセス設定と監視を見直す。
- PowerShell、Python、rundll32、WebDAV など正規機能を使った不審な連鎖を検知できるようにする。
- CVE-2023-36036を含む既知脆弱性の適用状況と、認証情報窃取後の横展開・RDP/WinRM利用を重点的に確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2023-36036 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2021-31969 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Active Directory | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [When IT Support Calls: Dissecting a ModeloRAT Campaign from Teams to Domain Comp](https://rapid7.com/blog/post/tr-it-support-dissecting-modelorat-campaign-microsoft-teams-compromise) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 技術詳細・再現情報あり。
- 継続観測: 初出。

---

<a id="topic-4189"></a>

### 3. Canvas owner reaches ‘agreement’ with threat actors after data breach

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脅威アクター</nobr> / <nobr>ランサムウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Canvas owner reaches ‘agreement’ with threat actors after data breach に関する脅威・攻撃キャンペーン系の話題です。
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
| <nobr>出典</nobr> | [Canvas owner reaches ‘agreement’ with threat actors after data breach](https://cybersecuritydive.com/news/canvas-agreement-threat-actors--ransomware/820084) | <nobr>内容確認・補足情報</nobr> |

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

<a id="topic-4237"></a>

### 4. Pwn2Own Berlin 2026: The Full Schedule

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>Linux</nobr> / <nobr>Windows</nobr> / <nobr>AI</nobr> / <nobr>クラウド</nobr> / <nobr>RCE</nobr> / <nobr>DDoS</nobr> / <nobr>iOS</nobr> / <nobr>AIエージェント</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 35.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Pwn2Own Berlin 2026: The Full Schedule に関するAI×Securityの話題です。
AIの利用目的、扱うデータ、権限、外部接続、監査、ベンダー管理など、実務上の確認観点を中心に整理しています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

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

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| ベンダー | Palo Alto | 言及あり | 0.80 |
| ベンダー | VMware | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Pwn2Own Berlin 2026: The Full Schedule](https://thezdi.com/blog/2026/5/13/pwn2own-berlin-2026-the-full-schedule) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-4232"></a>

### 5. Weaponized AI: The new frontier of fraud and identity spoofing

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Weaponized AI: The new frontier of fraud and identity spoofing に関するAI×Securityの話題です。
AIの利用目的、扱うデータ、権限、外部接続、監査、ベンダー管理など、実務上の確認観点を中心に整理しています。

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
| <nobr>出典</nobr> | [Weaponized AI: The new frontier of fraud and identity spoofing](https://cyberscoop.com/ai-generated-fraud-identity-spoofing-defense-strategy) | <nobr>内容確認・補足情報</nobr> |

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

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-3472"></a>

### 1. Microsoft 2026年5月 Patch Tuesday 関連まとめ

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>Windows</nobr> / <nobr>RCE</nobr> / <nobr>クラウド</nobr> / <nobr>DDoS</nobr> / <nobr>AI</nobr> / <nobr>政策・規制</nobr> / <nobr>防御・運用</nobr> / <nobr>Android</nobr> |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 76.0 |
| <nobr>実務影響</nobr> | 56.0 |
| <nobr>確度</nobr> | 58.0 |

#### 概要

Microsoftの2026年5月のPatch Tuesdayでは、120件超のCVE修正が公開され、複数の重大な脆弱性が含まれています。
公開情報では、今回は既知の積極的な悪用や公表済みゼロデイは確認されていない一方、Microsoft Word関連の複数のリモートコード実行脆弱性など、優先度を上げて対応すべき項目があるとされています。
修正件数が多く、影響範囲も広いため、通常の月例更新としては見逃せない内容です。
特に文書処理系やリモートコード実行に関わる脆弱性は、利用環境によっては実害につながりやすいため注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 14 sources。
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

- Microsoft Wordなど、利用頻度の高い製品の修正を優先的に適用する。
- 社内で影響を受ける製品・機能を棚卸しし、段階的にパッチ適用計画を確認する。
- 今回ゼロデイは確認されていないが、公開情報の更新や追加報告がないか継続監視する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-40364 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40361 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-41096 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-41089 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-42898 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40415 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-35435 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-35428 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-42826 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-32207 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft, Palo Alto Networks Find Many Vulnerabilities by Using AI on Their Own](https://securityweek.com/microsoft-palo-alto-networks-find-many-vulnerabilities-by-using-ai-on-their-own-code) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft's MDASH AI System Finds 16 Windows Flaws Fixed in Patch Tuesday](https://thehackernews.com/2026/05/microsofts-mdash-ai-system-finds-16.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [May 2026 Patch Tuesday: no zero-days but plenty to fix](https://malwarebytes.com/blog/news/2026/05/may-2026-patch-tuesday-no-zero-days-but-plenty-to-fix) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Chipmaker Patch Tuesday: Intel and AMD Patch 70 Vulnerabilities](https://securityweek.com/chipmaker-patch-tuesday-intel-and-amd-patch-70-vulnerabilities) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Fixes 17 Critical Flaws in May Patch Tuesday](https://infosecurity-magazine.com/news/microsoft-17-critical-flaws-may) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ICS Patch Tuesday: New Security Advisories From Siemens, Schneider, CISA](https://securityweek.com/ics-patch-tuesday-new-security-advisories-from-siemens-schneider-cisa) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Patch Tuesday - May 2026](https://rapid7.com/blog/post/em-patch-tuesday-may-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Defense at AI speed: Microsoft’s new multi-model agentic security system tops le](https://microsoft.com/en-us/security/blog/2026/05/12/defense-at-ai-speed-microsofts-new-multi-model-agentic-security-system-finds-16-new-vulnerabilities) | <nobr>内容確認・補足情報</nobr> |

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

CVE-2025-60710は、Microsoft WindowsのTaskhost関連の処理に起因するローカル権限昇格の脆弱性として整理されています。
公開情報ではCISAのKnown Exploited Vulnerabilitiesにも含まれており、悪用済みとして優先的な対応が必要な対象とされています。
権限昇格は、低権限で侵入された端末でも管理者権限獲得につながるため、被害拡大の起点になりやすい点が重要です。
公開PoCの存在が示されているため、影響範囲の確認と早期の緩和策適用が注目されます。

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

- Microsoftの修正情報や適用可能な更新を確認し、対象端末へ優先的に適用する。
- Windows端末で不審な権限昇格やTaskhost関連の異常な挙動がないか、監視・ログ確認を強化する。
- CVE-2025-60710の影響を受ける資産を棚卸しし、特に管理権限のない利用端末を優先して点検する。

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

Akamai Security Intelligenceは、MySQLサーバーを標的とするランサムウェアのキャンペーンを確認したと伝えています。
攻撃者は二重恐喝の手口を用い、データの公開をちらつかせて被害者に圧力をかけているとされています。
MySQLは多くのシステムの基盤になるため、侵害が発生すると業務影響が広がりやすい点が注意されます。
公開された情報に基づく脅威インテリジェンスとして、運用側の監視や備えの見直しに役立ちます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- MySQLの認証情報管理、外部公開状況、不要な到達経路を改めて確認する。
- バックアップの整合性と復旧手順を点検し、実際に復旧できるかを検証する。
- データ流出を前提に、ログ監視・アラート・インシデント対応手順を見直す。

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

<a id="topic-4118"></a>

### 4. ランサム被害で個人情報流出の可能性 - エネサンスHD

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

液化石油ガスの輸入、販売を手がけるエネサンスホールディングスは、ランサムウェアを用いたサイバー攻撃を受けた問題で、顧客の個人情報が流出した可能性があることを明らかにした。

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
| <nobr>出典</nobr> | [ランサム被害で個人情報流出の可能性 - エネサンスHD](https://security-next.com/184352) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
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

<a id="topic-4219"></a>

### 6. 人気ノートアプリ「Obsidian」がプラグイン審査を刷新、マルウェア検査や安全性表示を導入へ

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>マルウェア</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Markdown形式のノートをローカルファイルとして扱えるノートアプリ「Obsidian」が、プラグインとテーマの配布基盤を刷新し、新たに「Obsidian Community」というコミュニティサイトと開発者向けのレビューシステムを立ち上げました。
続きを読む...

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 発行元・一次情報を確認する。
- 自組織の業務・システム・委託先への関係有無を確認する。
- 追加情報や続報が出ていないか確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [人気ノートアプリ「Obsidian」がプラグイン審査を刷新、マルウェア検査や安全性表示を導入へ](https://gigazine.net/news/20260513-obsidian-plugin-future) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり・低信頼。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [The Gentlemenを装った攻撃に関する注意喚起](https://research.checkpoint.com/2026/thus-spoke-the-gentlemen) | 29.0 | 38.0 | 50.0 |
| [Unifi Accessにおけるリモートコード実行の脆弱性（CVE-2025-52665）](https://catchify.sa/post/cve-2025-52665-rce-in-unifi-os-25-000) | 28.0 | 46.0 | 50.0 |
| [CVE-2026-0263：PAN-OSのIKEv2処理におけるリモートコード実行の脆弱性（重要度：高）](https://security.paloaltonetworks.com/CVE-2026-0263) | 28.0 | 46.0 | 50.0 |
| [CVE-2026-0264: PAN-OSのDNS ProxyおよびDNS Serverにおけるヒープベースのバッファオーバーフローにより未認証のリモートコード実行が可能に](https://security.paloaltonetworks.com/CVE-2026-0264) | 28.0 | 46.0 | 50.0 |
| [CVE-2026-0257 PAN-OSのGlobalProtect認証バイパスの脆弱性（重要度: MEDIUM）](https://security.paloaltonetworks.com/CVE-2026-0257) | 28.0 | 46.0 | 50.0 |
| [CVE-2026-0265 PAN-OSのCAS有効時における認証回避の脆弱性](https://security.paloaltonetworks.com/CVE-2026-0265) | 28.0 | 46.0 | 50.0 |
| [CVE-2026-0261 PAN-OSの認証済み管理者向けコマンドインジェクション脆弱性（重大度: 中）](https://security.paloaltonetworks.com/CVE-2026-0261) | 28.0 | 46.0 | 50.0 |
| [Netskopeにおけるクロステナント認証バイパスの脆弱性](https://blog.amberwolf.com/blog/2025/august/advisory---netskope-cross-tenant-authentication-bypass) | 28.0 | 38.0 | 42.0 |
| [MicrosoftがDNSとNetlogonのRCE脆弱性を含む138件の脆弱性を修正](https://thehackernews.com/2026/05/microsoft-patches-138-vulnerabilities.html) | 28.0 | 38.0 | 42.0 |
| [Foxconn、北米の工場がサイバー攻撃を受けたことを確認](https://securityweek.com/foxconn-confirms-north-american-factories-hit-by-cyberattack) | 28.0 | 30.0 | 42.0 |
| [Foxconn、北米の一部施設を対象としたサイバー攻撃を確認](https://cybersecuritydive.com/news/foxconn-confirms-cyberattack-affecting-some-north-american-facilities/820120) | 28.0 | 30.0 | 42.0 |
| [Canvas Owner、ランサムウェア攻撃後にサイバー犯罪者と合意に達する](https://infosecurity-magazine.com/news/canvas-cybercriminals-agreement) | 28.0 | 30.0 | 42.0 |
| [Nitrogenランサムウェア集団が主張したFoxconnへのサイバー攻撃、Foxconnが確認](https://bleepingcomputer.com/news/security/electronics-giant-foxconn-confirms-cyberattack-on-north-american-factories) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア被害でCISOの半数超が身代金支払いを検討](https://infosecurity-magazine.com/news/ransomware-over-half-cisos-would) | 28.0 | 30.0 | 42.0 |
| [Oracle of Delphiが認証情報を盗む](https://akamai.com/blog/security/the-oracle-of-delphi-steal-your-credentials) | 28.0 | 20.0 | 42.0 |
| [Nansh0uキャンペーン―攻撃者の武器庫がさらに強化](https://akamai.com/blog/security/the-nansh0u-campaign-hackers-arsenal-grows-stronger) | 28.0 | 20.0 | 42.0 |
| [Signal、フィッシング攻撃に対応する新しいアプリ内セキュリティ警告を導入](https://helpnetsecurity.com/2026/05/13/signal-phishing-social-engineering-protections) | 28.0 | 20.0 | 42.0 |
| [中国のAPTグループ「FamousSparrow」が南コーカサスのエネルギー企業に潜伏](https://darkreading.com/cyberattacks-data-breaches/china-famoussparrow-apt-south-caucasus-energy-firm) | 28.0 | 20.0 | 42.0 |
| [アゼルバイジャンのエネルギー企業がMicrosoft Exchangeの脆弱性悪用を繰り返し受ける](https://thehackernews.com/2026/05/azerbaijani-energy-firm-hit-by-repeated.html) | 28.0 | 20.0 | 42.0 |
| [LatAm Vibe Hackersがその場でカスタムハッキングツールを生成](https://darkreading.com/cloud-security/ai-agents-generate-custom-hacking-tools) | 28.0 | 20.0 | 42.0 |
| [GemStufferが150以上のRubyGemsを悪用して英国の地方議会ポータルから収集したデータを流出](https://thehackernews.com/2026/05/gemstuffer-abuses-150-rubygems-to.html) | 28.0 | 20.0 | 42.0 |
| [Geminiがスマホを“自動操縦” Google、Android向けAIエージェント「Gemini Intelligence」発表](https://itmedia.co.jp/news/articles/2605/13/news136.html) | 26.0 | 20.0 | 42.0 |
| [MicrosoftがAI活用のセキュリティーシステム、Windowsの脆弱性16件を発見](https://xtech.nikkei.com/atcl/nxt/news/24/03229) | 26.0 | 20.0 | 42.0 |
| [AI inside、国内データセンター事業者との「Sovereign Grid」を開始](https://japan.zdnet.com/article/35247467) | 26.0 | 20.0 | 42.0 |

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
