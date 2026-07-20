# 📡 サイレーダー 2026-07-21 05:00 JST

このレポートは、2026-07-20 17:00 JST〜2026-07-21 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 83
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 49

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [SonicWall Zero-Days Exploited to Deliver Custom Malware for Weeks Before Patch](#topic-22364) | 52.0 | 74.0 | 67.0 | 音声 | 温度感上位枠 |
| 2 | [ServiceNow pre-auth RCE exploited in the wild (CVE-2026-6875)](#topic-23291) | 41.0 | 64.0 | 51.0 | 音声 | 温度感上位枠 |
| 3 | [JadePuffer Returns With Ransomware Designed to Wipe AI Models](#topic-23296) | 41.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [New 7-Zip Vulnerability Could Let Crafted XZ Archives Run Code During Extraction](#topic-23331) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 5 | [Researchers trace SonicWall SMA1000 exploitation to late June](#topic-23283) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [⚡ Weekly Recap: WordPress RCE, SonicWall 0-Days, AI Service Attacks, SharePoint 0-Day and More](#topic-23302) | 35.0 | 20.0 | 43.0 | 音声 | AI×Security枠 |
| 7 | [From a Single Alert to 1,000 Files: Inside an Exposed WebDAV Malware Delivery Lab](#topic-23305) | 35.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 8 | [Exploitation in the Wild of wp2shell](#topic-23164) | 32.0 | 56.0 | 60.0 | GitHub | 音声枠上限によりGitHubのみ |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-22364"></a>

### 1. SonicWall Zero-Days Exploited to Deliver Custom Malware for Weeks Before Patch

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 52.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

SonicWallのSecure Mobile Access（SMA）1000シリーズに影響する2件の脆弱性、CVE-2026-15409とCVE-2026-15410が、実際の攻撃で悪用されていたと報じられています。
関係各社は修正版の適用と、侵害の痕跡がないかの確認を呼びかけています。リモートアクセス機器が対象のため、侵害されると社内ネットワークへの入口になり得ます。
公開情報では悪用の事実や検証コードの言及もあり、早期対応の優先度が高い案件です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
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

- SMA 1000シリーズの利用有無を確認し、該当する場合は修正版の適用を急ぐ。
- ベンダーが示す侵害痕跡や不審な設定変更・接続履歴を点検する。
- 痕跡が見つかった場合は、認証情報やTOTPの再設定を含む復旧手順を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-15409 | 関連CVE | 1.00 | 候補あり（URL 4件以上） |
| 脆弱性 | CVE-2026-15410 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | SonicWall | 言及あり | 0.80 | — |
| 製品 | SonicWall SMA | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-15409](https://nvd.nist.gov/vuln/detail/CVE-2026-15409) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [SonicWall Zero-Days Exploited to Deliver Custom Malware for Weeks Before Patch](https://www.securityweek.com/sonicwall-zero-days-exploited-to-deliver-custom-malware-for-weeks-before-patch/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Rapid7 MDR Team Discovers New SonicWall SMA1000 Zero Days being Actively Exploit](https://www.rapid7.com/blog/post/etr-rapid7-mdr-team-discovers-new-sonicwall-sma1000-zero-days-being-actively-exploited-cve-2026-15409-cve-2026-15410) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Two SonicWall SMA 1000 Zero-Days Exploited, One Could Enable Admin Commands](https://thehackernews.com/2026/07/two-sonicwall-sma-1000-zero-days.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall Issues Urgent SMA Patch Warning for Two Zero-Day Exploits](https://www.securityweek.com/sonicwall-issues-urgent-sma-patch-warning-for-two-zero-day-exploits/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall warns of SMA1000 flaws exploited in zero-day attacks, patch now](https://www.bleepingcomputer.com/news/security/sonicwall-warns-of-sma1000-flaws-exploited-in-zero-day-attacks-patch-now/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall SMA appliances targeted in zero-day attacks (CVE-2026-15409, CVE-2026-](https://www.helpnetsecurity.com/2026/07/14/sonicwall-sma-attacks-via-cve-2026-15409-cve-2026-15410/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-23291"></a>

### 2. ServiceNow pre-auth RCE exploited in the wild (CVE-2026-6875)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

ServiceNow AI Platformの脆弱性CVE-2026-6875について、実際の悪用が始まっているとする脅威情報が出ています。
公開情報では、未認証で任意コード実行につながる可能性がある重大なプリオーセンティケーション脆弱性として説明されています。
ServiceNowは業務自動化の基盤として広く使われるため、影響範囲が大きくなりやすい点が注目されます。
認証前に悪用されうる脆弱性は、外部からの侵入リスクが高く、優先度の高い対応が必要になりやすいです。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ServiceNow AI Platformを利用している環境では、ベンダーの修正情報と適用状況を早急に確認する。
- 外部公開されたインスタンスや関連アクセス経路について、想定外の到達性がないか見直す。
- 不審なリクエストや管理系の異常動作、想定外のコード実行の兆候を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-6875 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-6875](https://nvd.nist.gov/vuln/detail/CVE-2026-6875) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [ServiceNow pre-auth RCE exploited in the wild (CVE-2026-6875)](https://www.helpnetsecurity.com/2026/07/20/servicenow-cve-2026-6875-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical ServiceNow code execution flaw now exploited in attacks](https://www.bleepingcomputer.com/news/security/critical-servicenow-code-execution-flaw-now-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23296"></a>

### 3. JadePuffer Returns With Ransomware Designed to Wipe AI Models

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

JadePufferとされる脅威活動に関連して、AIモデルの成果物を破壊することを意図したランサムウェアが使われたと報じられています。
対象はAIモデルそのものや関連ファイルで、一般的な身代金要求型の被害にとどまらず、復旧に必要な資産の損壊が懸念されます。
AI導入が進む組織では、学習済みモデルや推論用資産の損失が業務停止や再構築コストの増大につながるためです。
従来のデータ暗号化対策に加え、AI資産の保全と復旧計画を見直す必要があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 学習済みモデル、重み、設定ファイル、関連メタデータを重要資産としてバックアップと復旧手順を確認する。
- AI開発・運用環境のアクセス権限を見直し、不要な書き込み権限や共有領域の露出を減らす。
- ランサムウェア対策として、端末・サーバー監視、オフライン保管を含むバックアップ、復旧訓練をAI環境でも適用する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [JadePuffer Returns With Ransomware Designed to Wipe AI Models](https://www.infosecurity-magazine.com/news/jadepuffer-ai-model-ransomware/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23331"></a>

### 4. New 7-Zip Vulnerability Could Let Crafted XZ Archives Run Code During Extraction

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

7-Zipに関する脆弱性CVE-2026-14266が報告され、細工されたXZアーカイブを展開した際にコード実行につながる可能性があるとされています。
説明されている内容では、XZチャンクデータの処理に起因するヒープベースのバッファオーバーフローで、7-Zip 26.02で修正が提供済みとされています。
圧縮ファイルの展開は日常的な操作のため、影響範囲が広くなりやすい点が注目されます。既知の悪用情報があるとされているため、利用環境の更新状況を確認する必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 7-Zipを利用している端末やサーバーで、26.02以降への更新状況を確認する。
- XZ形式のアーカイブを扱う業務フローがある場合は、受領元の確認や不審ファイルの取り扱いを改めて見直す。
- 脆弱性情報の更新を追い、同種の圧縮ファイル処理を行う周辺ツールにも影響がないか点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-14266 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Trend Micro | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-14266](https://nvd.nist.gov/vuln/detail/CVE-2026-14266) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [New 7-Zip Vulnerability Could Let Crafted XZ Archives Run Code During Extraction](https://thehackernews.com/2026/07/new-7-zip-vulnerability-could-let.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23283"></a>

### 5. Researchers trace SonicWall SMA1000 exploitation to late June

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者は、SonicWallのSMA1000が6月下旬ごろから悪用された可能性を指摘しています。
複数の脅威アクターが関与しているとされ、その中にはINC Ransomも含まれています。境界防御機器が悪用されると、組織内ネットワークへの侵入口になり得るため注意が必要です。
ランサムウェア文脈での事案であり、初動対応や資産管理の重要性が改めて示されています。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SonicWall SMA1000の利用有無を確認し、最新のベンダー情報や修正状況を点検する。
- 境界機器の認証・管理ログを確認し、不審なアクセスや設定変更がないかを監視する。
- ランサムウェア対策として、重要データのバックアップと復旧手順を再確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ランサムウェアグループ | INC Ransom | 主題 | 0.80 | — |
| ベンダー | SonicWall | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Researchers trace SonicWall SMA1000 exploitation to late June](https://www.cybersecuritydive.com/news/researchers-sonicwall-sma1000-exploitation-june/825654/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23302"></a>

### 6. ⚡ Weekly Recap: WordPress RCE, SonicWall 0-Days, AI Service Attacks, SharePoint 0-Day and More

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>R⁠C⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

今週は、WordPress、SonicWall、Microsoft SharePoint に関する脆弱性や、AIサービスを狙う攻撃がまとめて取り上げられました。
公開情報では、コード実行や認証回避、セキュリティ機能の無効化につながる可能性がある話題が含まれており、既に悪用が観測されたものもあるとされています。
複数の主要製品が同時に話題になっており、運用現場では優先度付けと対応の見直しが必要になりやすい状況です。
特に、既に悪用観測がある項目は、通知待ちではなく保護状況の確認を急ぐ価値があります。

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

- WordPress、SonicWall、SharePoint の関連製品について、最新パッチ適用状況と公開範囲を確認する。
- AI関連サービスでは、入力検証や権限設定、外部連携の見直しを行い、想定外の操作につながる経路がないか点検する。
- 脆弱性情報だけでなく、実際の悪用観測の有無を踏まえて監視・優先順位を調整する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | SonicWall | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| 製品 | WordPress | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [⚡ Weekly Recap: WordPress RCE, SonicWall 0-Days, AI Service Attacks, SharePoint ](https://thehackernews.com/2026/07/weekly-recap-wordpress-rce-sonicwall-0.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-23305"></a>

### 7. From a Single Alert to 1,000 Files: Inside an Exposed WebDAV Malware Delivery Lab

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>A⁠I</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Rapid7は、公開状態だったWebDAV系の配信インフラを調査し、1,000件超の資料やペイロード、ルアー素材が置かれたマルウェア配信・検証環境を確認したと報告しました。
そこには、WebDAV経由の実行方法やファイル名偽装、ClickFix型の誘導ページなど、複数の配信手法を試した形跡が含まれていたとされています。
単発のマルウェア配布ではなく、攻撃者が配信手順を体系的に検証・改良していた可能性がうかがえる点が注目されています。
防御側にとっては、個別サンプルだけでなく、WebDAVや偽装ファイル、誘導ページを含む配信経路全体を監視する重要性を示します。

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

- WebDAV経由のファイル取得や不審な .url / .lnk / .scr などの起動に注意し、関連するログと端末テレメトリを横断確認する。
- Microsoft Windows の既知のワーキングディレクトリ悪用やファイル名偽装に関する対策状況を点検し、未適用の修正がないか確認する。
- ユーザー向けには、文書ダウンロードやエラー表示を装うページからのコマンド実行やファイル開封を避けるよう周知する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-24054 | 関連CVE | 1.00 | 候補あり（URL 14件以上） |
| 脆弱性 | CVE-2025-33053 | 関連CVE | 1.00 | 候補あり（URL 6件以上） |
| 脆弱性 | CVE-2026-21513 | 関連CVE | 1.00 | 未確認 |
| 脅威アクター | Stealth Falcon | 主題 | 0.80 | — |
| 脅威アクター | Sandworm Team | 主題 | 0.80 | — |
| ベンダー | Check Point | 言及あり | 0.80 | — |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | cPanel | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [From a Single Alert to 1,000 Files: Inside an Exposed WebDAV Malware Delivery La](https://www.rapid7.com/blog/post/tr-exposed-webdav-malware-delivery-lab-analysis) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-23164"></a>

### 1. Exploitation in the Wild of wp2shell

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>A⁠I</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 32.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 60.0 |

#### 概要

WordPress Coreの脆弱性「CVE-2026-63030（wp2shell）」について、複数のセキュリティ研究者・企業が実際の悪用を観測したと報じています。
対象はWordPressの特定バージョンで、未認証でのリモートコード実行につながる可能性があるため、影響を受ける環境では早急な更新が求められます。
WordPressは広く使われているため、コアの脆弱性は多数の公開サイトに波及しやすい点が注目されています。
さらに、実運用環境での悪用が示唆されているため、単なる将来リスクではなく直近の対応課題として扱う必要があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 公開PoC・検証コード言及あり。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 影響を受けるWordPressのバージョンを確認し、修正版への更新を優先する。
- 公開Webサイトでは、更新後も改ざんや不審なファイル配置、Webシェルの痕跡がないか点検する。
- WAFや監視ルールを見直し、WordPress関連の異常なアクセスや実行挙動を継続的に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-60137 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-63030 | 関連CVE | 1.00 | 候補あり（URL 21件以上） |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| 製品 | WordPress | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-63030](https://nvd.nist.gov/vuln/detail/CVE-2026-63030) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [WordPress Exploitation Underway (CVE-2026-63030), (Mon, Jul 20th)](https://isc.sans.edu/diary/rss/33168) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Exploitation in the Wild of wp2shell](https://www.wiz.io/blog/wp2shell-cve-2026-63030-cve-2026-60137) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-63030: wp2shell a Critical Remote Code Execution Vulnerability in WordP](https://www.rapid7.com/blog/post/etr-cve-2026-63030-wp2shell-a-critical-remote-code-execution-vulnerability-in-wordpress-core) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [WebDAVマルウェアキャンペーンの背後にあるAI支援フィッシングツールキットを露呈した公開サーバー](https://thehackernews.com/2026/07/exposed-server-reveals-ai-assisted.html) | 33.0 | 20.0 | 42.0 |
| [ロシア語話者のハッカーがGoogle Gemini CLIを使い歯科医院の8台のPCからなるボットネットを制御](https://thehackernews.com/2026/07/russian-speaking-hacker-uses-google.html) | 33.0 | 20.0 | 42.0 |
| [映画公開直後に浮上したOdysseyの海賊版詐欺サイト](https://www.helpnetsecurity.com/2026/07/20/odyssey-movie-piracy-scams-malware/) | 28.0 | 20.0 | 42.0 |
| [CrashStealer：ネイティブmacOSマルウェアがもたらす脅威の高度化](https://blog.polyswarm.io/crashstealer-how-native-macos-malware-is-raising-the-bar) | 28.0 | 20.0 | 42.0 |
| [HollowGraphマルウェアがMicrosoft Graphを悪用してステルス性の高いC2通信を実現](https://www.bleepingcomputer.com/news/security/new-hollowgraph-malware-uses-microsoft-graph-for-stealthy-c2-comms/) | 28.0 | 20.0 | 42.0 |
| [HOLLOWGRAPHマルウェアがMicrosoft 365のカレンダーをスパイ活動の通信経路に転用](https://www.helpnetsecurity.com/2026/07/20/hollowgraph-malware-microsoft-365-calendar/) | 28.0 | 20.0 | 42.0 |
| [映画公開から数時間で現れるOdysseyの海賊版詐欺](https://www.malwarebytes.com/blog/threat-intel/2026/07/the-odyssey-piracy-scams-appear-within-hours-of-the-movies-release) | 28.0 | 20.0 | 42.0 |
| [Microsoft 365カレンダーがHOLLOWGRAPHキャンペーンでスパイ用の受け渡しボックスに利用される](https://www.theregister.com/security/2026/07/20/microsoft-365-calendars-become-spy-drop-boxes-in-hollowgraph-campaign/5274982) | 28.0 | 20.0 | 42.0 |
| [HollowGraphマルウェアがMicrosoft 365イベントを悪用し、C2と窃取ファイルを2050年の日付で隠蔽](https://thehackernews.com/2026/07/hollowgraph-malware-hides-c2-and-stolen.html) | 28.0 | 20.0 | 42.0 |
| [HollowGraphマルウェアがMicrosoft 365カレンダーを乗っ取り、密かにC2通信を行う手口](https://www.infosecurity-magazine.com/news/hollowgraph-microsoft-calendars/) | 28.0 | 20.0 | 42.0 |
| [偽ゲームがRenPy Loader、MSBuild、EtherHidingを用いて情報窃取型マルウェアを拡散](https://www.malwarebytes.com/blog/threat-intel/2026/07/fake-games-spread-stealers-with-renpy-loader-msbuild-and-etherhiding) | 28.0 | 20.0 | 42.0 |
| [CISOがAIリスクへの対応で厳しい状況に直面](https://www.darkreading.com/cybersecurity-operations/cisos-feel-heat-ai-risk) | 25.0 | 20.0 | 42.0 |
| [Commerce省AI標準室責任者、就任3カ月で退任](https://cyberscoop.com/director-of-commerce-ai-standards-office-out-after-three-months/) | 25.0 | 20.0 | 42.0 |
| [Neo、1億ドルを調達しエンタープライズAIソフトウェアの制御と保護へ](https://www.securityweek.com/neo-emerges-from-stealth-with-100m-to-control-and-secure-enterprise-ai-software/) | 25.0 | 20.0 | 42.0 |
| [AIモデルを遮断しても、それが生み出すサイバー脅威は止められない](https://cyberscoop.com/why-blocking-ai-models-wont-stop-cyber-threats-op-ed/) | 25.0 | 20.0 | 42.0 |
| [セキュリティ責任者のためのAI SOC評価ガイド](https://www.bleepingcomputer.com/news/security/an-ai-soc-evaluation-guide-for-security-leaders/) | 25.0 | 20.0 | 42.0 |
| [ResearchersがOpenAIのGPTを用いてWordPressのエクスプロイトを構築](https://www.infosecurity-magazine.com/news/researchers-wordpress-exploit/) | 25.0 | 20.0 | 42.0 |
| [Hugging Face、自律型AIエージェントによるネットワーク侵害を警告](https://www.bleepingcomputer.com/news/security/hugging-face-breach-autonomous-ai-agent-system-internal-datasets-credentials/) | 25.0 | 20.0 | 42.0 |
| [自律型AIエージェントによるHugging Face侵害](https://www.helpnetsecurity.com/2026/07/20/hugging-face-breached-by-autonomous-ai-agent/) | 25.0 | 20.0 | 42.0 |
| [Capital OneがAI搭載の脆弱性検出ツール「VulnHunter」をオープンソース化](https://www.securityweek.com/capital-one-open-sources-ai-powered-vulnhunter-security-tool/) | 25.0 | 20.0 | 42.0 |
| [Hugging Faceが自律型AI攻撃で侵害される](https://www.securityweek.com/hugging-face-hacked-in-autonomous-ai-attack/) | 25.0 | 20.0 | 42.0 |
| [AIインフラの秘密の問題：MCPのセキュリティはシークレット管理から始まる](https://www.cybersecuritydive.com/spons/the-secret-problem-in-ai-infrastructure-why-mcp-security-starts-with-secre/825210/) | 25.0 | 20.0 | 42.0 |
| [WordPress Coreの脆弱性チェーンによりリモートコード実行が可能に](https://www.cisecurity.org/advisory/a-vulnerability-chain-in-wordpress-core-could-allow-for-remote-code-execution_2026-070) | 24.0 | 38.0 | 42.0 |
| [7月20日版 脅威インテリジェンスレポート](https://research.checkpoint.com/2026/20th-july-threat-intelligence-report/) | 20.0 | 28.0 | 50.0 |
| [Frontier LLMではHugging Faceへの悪意あるエージェントの攻撃を防げなかった](https://www.theregister.com/cyber-crime/2026/07/20/frontier-llms-couldnt-help-hugging-face-fight-off-evil-agents/5275168) | 20.0 | 20.0 | 42.0 |
| [攻撃者がBECフィッシングで回避手法を組み合わせる手口](https://www.darkreading.com/endpoint-security/attackers-combo-evasion-tactics-bec-phishing) | 20.0 | 20.0 | 42.0 |
| [インド、流出したとされる原子力発電所の文書は安全上のリスクなしと発表](https://therecord.media/india-nuclear-plant-kudankulam-world-leaks-documents) | 20.0 | 20.0 | 42.0 |
| [韓国の外交官研修システムに9か月間侵入していたハッカーたち](https://therecord.media/south-korea-cyberattack-foreign-ministry) | 20.0 | 20.0 | 42.0 |
| [Cruciferra CrypterがProcess Ghostingを悪用して検知を回避](https://www.infosecurity-magazine.com/news/cruciferra-crypter-process-ghosting/) | 20.0 | 20.0 | 42.0 |
| [Paidworkの漏えいで2300万ユーザーの機密データが流出](https://www.helpnetsecurity.com/2026/07/20/paidwork-data-breach-23-million-users/) | 20.0 | 20.0 | 42.0 |
| [サイバー攻撃で停止した不動産登記システム、ルーマニアが復旧を急ぐ](https://therecord.media/romania-cyberattack-land-registry) | 20.0 | 20.0 | 42.0 |
| [医療大手Abbott、恐喝 দাবいの中で2件のサイバーインシデントを調査](https://www.malwarebytes.com/blog/data-breaches/2026/07/healthcare-giant-abbott-probes-two-cyber-incidents-amid-extortion-claims) | 20.0 | 20.0 | 42.0 |
| [大手病院向けソフトウェアベンダーから顧客データが窃取される](https://www.cybersecuritydive.com/news/craneware-health-care-data-breach/825643/) | 20.0 | 20.0 | 42.0 |
| [Cybersecurityでイベントを「平穏無事」に保つ方法](https://www.darkreading.com/cyber-risk/cybersecurity-keeps-events-uneventful) | 20.0 | 20.0 | 42.0 |
| [LOTL攻撃に今すぐ備える3つの対策](https://www.security.com/product-insights/three-ways-defend-against-lotl-attacks-now) | 20.0 | 20.0 | 42.0 |
| [Italy、WINDTREに対し2件のデータ侵害の背後にあるセキュリティ不備で170万ユーロの罰金を科す](https://www.helpnetsecurity.com/2026/07/20/italy-windtre-1-7-million-fine/) | 20.0 | 20.0 | 42.0 |
| [Health tech firm Craneware、サイバー攻撃で顧客・従業員データの大規模流出を認める](https://www.itpro.com/security/data-breaches/health-tech-firm-craneware-admits-significant-volume-of-customer-and-employee-data-exposed-in-cyber-attack) | 20.0 | 20.0 | 42.0 |
| [OpenSSLが「HollowByte」DoS脆弱性を静かに修正](https://www.securityweek.com/openssl-silently-fixes-hollowbyte-dos-vulnerability/) | 20.0 | 20.0 | 42.0 |
| [ロシア情報機関がNATO諸国とウクライナの軍事物流を監視するためIPカメラをハッキング](https://thehackernews.com/2026/07/russian-intelligence-hacks-ip-cameras.html) | 20.0 | 20.0 | 42.0 |
| [重大な侵害を追跡する新しいインデックス、損失は集計せず](https://www.securityweek.com/new-index-tracks-material-breaches-and-refuses-to-add-up-the-losses/) | 20.0 | 20.0 | 42.0 |
| [セキュリティプログラムを壊したのはMythosではない、露出期間かもしれない](https://thehackernews.com/2026/07/mythos-didnt-break-your-security.html) | 20.0 | 20.0 | 42.0 |
| [Ernst & Youngのデータ侵害で個人情報・金融情報が流出](https://www.securityweek.com/ernst-young-data-breach-affects-personal-financial-information/) | 20.0 | 20.0 | 42.0 |
| [2,000以上の米国病院にソフトウェアを提供する企業でハッカーが従業員と顧客のデータを窃取](https://therecord.media/software-provider-for-us-hospitals-customer-data-breach) | 20.0 | 20.0 | 42.0 |
| [Windows KB5121767のOOB更新で一部のDell PCのシャットダウン問題を修正](https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-windows-bug-causing-some-dell-pcs-to-shut-down/) | 20.0 | 20.0 | 42.0 |
| [警察幹部、TfLへのハッキングを受けサイバー犯罪リスク命令の導入を要請](https://www.infosecurity-magazine.com/news/police-chiefs-tfl-cybercrime-risk/) | 20.0 | 20.0 | 42.0 |
| [想像以上に広いあなたの攻撃対象領域](https://www.cybersecuritydive.com/spons/your-attack-surface-is-bigger-than-you-think/825160/) | 20.0 | 20.0 | 42.0 |
| [エージェント型エンドポイントセキュリティがIDEベースのサプライチェーン攻撃を阻止する方法](https://www.cybersecuritydive.com/spons/how-agentic-endpoint-security-shuts-down-ide-based-supply-chain-attacks/825550/) | 20.0 | 20.0 | 42.0 |
| [Windows 10の移行遅れがセキュリティ問題化している](https://www.helpnetsecurity.com/2026/07/20/windows-10-support-risks-report/) | 20.0 | 20.0 | 42.0 |
| [Chrome 150更新で深刻なメモリ安全性の不具合を修正](https://www.securityweek.com/chrome-150-update-patches-severe-memory-safety-bugs/) | 20.0 | 20.0 | 42.0 |

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
