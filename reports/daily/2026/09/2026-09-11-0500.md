# 📡 サイレーダー 2026-09-11 05:00 JST

このレポートは、2026-09-10 17:00 JST〜2026-09-11 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 99
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 2
- [低温だが記録しておくトピック](#low-record-topics): 64

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Organizations Warned of Cisco Secure FMC Exploitation](#topic-24944) | 55.0 | 74.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [CISA: WatchGuard RCE flaw now exploited in ransomware attacks](#topic-32073) | 49.0 | 66.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [New 'BlueMoon' kit exploited Windows and Chrome zero-day flaws](#topic-32019) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [CISA Flags Exploited Cisco, Citrix, Fortinet Flaws, Sets Sept. 12 Federal Patch Deadline](#topic-32052) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [MantaxOtax Android Malware Combines Ransomware With Spyware](#topic-32034) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [Critical NetScaler Vulnerability Exploited in Attacks](#topic-28317) | 35.0 | 64.0 | 55.0 | GitHub | 音声枠上限によりGitHubのみ |
| 7 | [Protecting organizations from AI-assisted executive impersonation and invoice fraud](#topic-32000) | 35.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 8 | [Detect and disrupt AI-themed attacks with Microsoft Defender](#topic-32005) | 35.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 9 | [Update Chrome now to protect against an actively exploited vulnerability](#topic-31864) | 33.0 | 46.0 | 55.0 | GitHub | 音声枠上限によりGitHubのみ |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-24944"></a>

### 1. Organizations Warned of Cisco Secure FMC Exploitation

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 55.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Secure Firewall Management Center（FMC）に関する深刻な脆弱性（CVE-2026-20079）について、実際に悪用されている可能性があるとして注意喚起が出ています。
認証回避につながるおそれがあり、影響を受けた環境では管理対象機器の運用やネットワーク防御に大きな影響が出る可能性があります。
FMCは複数のCiscoファイアウォール機器を一元管理する基盤のため、侵害されると影響範囲が広くなり得ます。
ベンダーが修正を案内しており、優先度を上げて確認・更新すべき事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- FMCの公開状況と外部から到達可能かを確認し、影響を受ける構成かを把握する。
- Ciscoが提供する修正済みソフトウェアへの更新可否を早急に確認する。
- FMCの管理系アクセスログや不審な認証回避の痕跡を点検し、異常があれば調査を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20079 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-20316 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Adaptive Security Appliance | 言及あり | 0.80 | — |
| 製品 | Cisco Firepower Threat Defense | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20079](https://nvd.nist.gov/vuln/detail/CVE-2026-20079) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [We've got one word for it, and it's usually the wrong one](https://blog.talosintelligence.com/weve-got-one-word-for-it-and-its-usually-the-wrong-one/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco FMC bugs exploited by nation-state and ransomware actors (CVE-2026-20079, ](https://www.helpnetsecurity.com/2026/09/10/cisco-fmc-exploited-cve-2026-20079-cve-2026-20316/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Organizations Warned of Cisco Secure FMC Exploitation](https://www.securityweek.com/organizations-warned-of-cisco-secure-fmc-exploitation/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco confirms CVE-2026-20079 Secure FMC flaw exploited in attacks](https://www.bleepingcomputer.com/news/security/cisco-confirms-cve-2026-20079-secure-fmc-flaw-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Active exploitation of Cisco Secure Firewall Management Center vulnerabilities](https://blog.talosintelligence.com/fmc-ongoing-exploitation/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Firewall Management Center Software Authentication Bypass Vulnerabi](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-onprem-fmc-authbypass-5JPp45V2) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-32073"></a>

### 2. CISA: WatchGuard RCE flaw now exploited in ransomware attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 49.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 66.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、WatchGuard Fireboxの重大な脆弱性がランサムウェア攻撃でも悪用されていることを確認したとされています。
以前から「実際に悪用されている」として注意喚起されていた脆弱性で、今回あらためて攻撃者側の利用が示された形です。
境界防御機器の脆弱性は、社内ネットワークへの侵入口になり得るため影響が大きいです。
ランサムウェアとの関連が示されているため、該当機器の防御状況確認や緊急対応の優先度が高まります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象機器のバージョンとパッチ適用状況を確認し、該当する場合は速やかに更新する。
- 外部公開されている管理機能や不要なサービスの露出を点検する。
- 侵害の兆候を前提に、ログ確認と関連アカウント・設定の監査を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-14733 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA: WatchGuard RCE flaw now exploited in ransomware attacks](https://www.bleepingcomputer.com/news/security/cisa-watchguard-rce-flaw-now-exploited-in-ransomware-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32019"></a>

### 3. New 'BlueMoon' kit exploited Windows and Chrome zero-day flaws

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>Exploit Kit</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

複数のサイバースパイ活動グループが、「BlueMoon」と呼ばれるエクスプロイトキットを用い、Microsoft WindowsとGoogle Chromeのゼロデイ脆弱性を悪用していたと報じられています。
現時点の材料では、具体的なCVE番号や影響範囲の詳細は示されていません。ゼロデイの悪用は、修正前の環境が狙われるため、被害の広がりや対応の難しさが大きくなります。
WindowsとChromeという利用者の多い製品が関係している点でも、注目度が高い話題です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- WindowsとChromeの更新適用状況を改めて確認し、最新パッチを優先して適用する。
- 侵入の兆候を前提に、端末・ブラウザ周辺の監視とログ確認を強化する。
- 特に標的型攻撃を想定し、権限管理や多要素認証など基本対策の徹底を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Microsoft Windows | 言及あり | 0.80 | — |
| 製品 | Google Chrome | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New 'BlueMoon' kit exploited Windows and Chrome zero-day flaws](https://www.bleepingcomputer.com/news/security/new-bluemoon-kit-exploited-windows-and-chrome-zero-day-flaws/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32052"></a>

### 4. CISA Flags Exploited Cisco, Citrix, Fortinet Flaws, Sets Sept. 12 Federal Patch Deadline

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、Cisco、Citrix、Fortinetに関連する3件の脆弱性をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
これにより、米連邦民間行政機関（FCEB）は2026年9月12日までに修正対応を行う必要があります。
KEVへの追加は、実際に悪用が確認された、またはその可能性が高い脆弱性として優先度が上がることを意味します。
対象製品を利用する組織では、通常の脆弱性管理よりも早い確認と対応が求められます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 自組織でCisco、Citrix、Fortinet製品の利用有無を確認し、該当バージョンを棚卸しする。
- ベンダーの修正情報と影響範囲を確認し、優先度を上げて適用計画を立てる。
- 公開情報だけで判断せず、ログや監視結果で不審な兆候がないか点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Fortinet | 言及あり | 0.80 | — |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Flags Exploited Cisco, Citrix, Fortinet Flaws, Sets Sept. 12 Federal Patch ](https://thehackernews.com/2026/09/cisa-flags-exploited-cisco-citrix.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32034"></a>

### 5. MantaxOtax Android Malware Combines Ransomware With Spyware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠n⁠d⁠r⁠o⁠i⁠d</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

MantaxOtaxと呼ばれるAndroid向けマルウェアが、ランサムウェア的な脅迫とスパイウェア的な情報窃取機能を併せ持つ事例として報告されています。
現時点では公開情報ベースの初報であり、被害範囲や実際の広がりは断定できません。1つのAndroidマルウェアが、端末の利用妨害と情報収集を同時に狙う点が注目されています。
モバイル端末が業務利用される環境では、情報漏えいと可用性低下の両面で影響が出る可能性があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Android端末の導入元やインストール経路を再確認し、非公式配布や不審な権限要求への注意を徹底する。
- 端末管理の観点で、モバイル向けEDRやMDMの検知・隔離設定、アプリ許可制御を見直す。
- 端末内の機密情報保護とバックアップの整備を確認し、万一のロックや情報流出に備える。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [MantaxOtax Android Malware Combines Ransomware With Spyware](https://www.infosecurity-magazine.com/news/mantaxotax-android-malware/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32000"></a>

### 6. Protecting organizations from AI-assisted executive impersonation and invoice fraud

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftは、AIを活用したビジネスメール詐欺（BEC）の一例として、経営層を装ったなりすましと偽の請求書を組み合わせ、財務部門を狙ってACH送金を不正に誘導するキャンペーンを取り上げています。
AIの利用により、見た目や文面の説得力が増し、従来型の詐欺よりも見分けにくくなる点が懸念されます。
財務・経理の承認フローを狙うため、被害が直接的な金銭損失につながりやすい点が重要です。
AIによるなりすましは、メールの真正性判断や社内確認だけでは防ぎにくくなっており、業務プロセス側の対策が求められます。

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

- 経理・財務向けに、送金依頼の本人確認をメール単独に依存しない手順へ見直す。
- 経営層や取引先を装う不自然な請求・支払変更依頼について、承認前の二重確認を徹底する。
- Microsoft DefenderやMicrosoft 365、Exchangeなどの保護機能で、なりすましや不審なメールの検知・警告設定を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |
| 製品 | Exchange | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Protecting organizations from AI-assisted executive impersonation and invoice fr](https://www.microsoft.com/en-us/security/blog/2026/09/10/protecting-organizations-ai-assisted-executive-impersonation-invoice-fraud/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-32005"></a>

### 7. Detect and disrupt AI-themed attacks with Microsoft Defender

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftは、AIを題材にしたフィッシング、マルウェア、多段階攻撃に対して、Microsoft Defenderが検知・妨害に役立つとする内容を公開しました。
材料ではVidarなどのマルウェア名やMicrosoft Teams、Microsoft 365、DeepSeekといった関連語が見られますが、具体的な攻撃手口の詳細までは示されていません。
AI関連の話題を悪用した攻撃は、利用者の関心を引きやすく、通常の業務環境にも紛れ込みやすいため注意が必要です。
防御側にとっては、メール・チャット・エンドポイントをまたぐ検知と連携が重要であることを改めて示す内容です。

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

- Microsoft Defenderで、フィッシング・マルウェア・多段階攻撃の検知連携が適切に働くか確認する。
- Microsoft TeamsやMicrosoft 365上の不審な誘導、添付ファイル、リンクの監視を強化する。
- AI関連の話題を装うメッセージは業務連絡と見分けにくいため、利用者向け注意喚起を継続する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | DeepSeek | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |
| 製品 | Microsoft Teams | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |
| マルウェア | Vidar | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Detect and disrupt AI-themed attacks with Microsoft Defender](https://www.microsoft.com/en-us/security/blog/2026/09/10/detect-and-disrupt-ai-themed-attacks-with-microsoft-defender/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-28317"></a>

### 1. Critical NetScaler Vulnerability Exploited in Attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

Citrix NetScaler ADCとNetScaler Gatewayに、認証を回避される恐れのある重大な脆弱性CVE-2026-19490が報告されています。
公開情報では、影響を受ける製品の一部は修正済みバージョンが案内されており、関連する構成を持つ環境では早急な確認と更新が推奨されています。
NetScalerは企業の境界付近で使われることが多く、影響を受けると認証基盤やリモートアクセス経路に直接関わる可能性があります。
認証回避系の脆弱性は優先度が高く、実運用では迅速なパッチ適用と影響範囲の確認が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 影響対象のNetScaler ADC / Gatewayのバージョンを確認し、修正済み版への更新を急ぐ。
- SAML認証やVPN/認証vServerの構成がある場合は、該当CVEの影響有無を重点的に点検する。
- インターネット公開面にある機器として、ログ監視と不審な認証挙動の確認を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-19490 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-19490](https://nvd.nist.gov/vuln/detail/CVE-2026-19490) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Critical NetScaler Vulnerability Exploited in Attacks](https://www.securityweek.com/critical-netscaler-vulnerability-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-19490: Critical Vulnerability Affecting Citrix NetScaler ADC and NetSca](https://www.rapid7.com/blog/post/etr-cve-2026-19490-critical-vulnerability-affecting-citrix-netscaler-adc-and-netscaler-gateway) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-31864"></a>

### 2. Update Chrome now to protect against an actively exploited vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

GoogleはChromeの更新版を公開し、合計230件の脆弱性を修正しました。
その中には、V8に存在するCVE-2026-87491が含まれており、公開情報では実際の悪用が観測されているとされています。
ブラウザは利用者数が多く、修正遅れがそのまま被害につながりやすいため、優先度の高い更新対象です。特に実悪用が示唆される脆弱性は、組織内の端末管理や更新適用の速さが問われます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Chromeの更新状況を確認し、管理下端末へ早急に適用する。
- 自動更新が無効・停滞している端末がないか点検する。
- ブラウザ経由の不審な挙動がないか、関連ログやEDRの検知状況を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-87491 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Google Chrome | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-87491](https://nvd.nist.gov/vuln/detail/CVE-2026-87491) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Update Chrome now to protect against an actively exploited vulnerability](https://www.malwarebytes.com/blog/bugs/2026/09/update-chrome-now-to-protect-against-an-actively-exploited-vulnerability) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Chrome V8 Zero-Day Exploited in the Wild Enables Code Execution Inside Sandbox](https://thehackernews.com/2026/09/chrome-v8-zero-day-exploited-in-wild.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [AIを活用した攻撃がPaperCutの脆弱性を悪用し395組織を侵害](https://www.bleepingcomputer.com/news/security/ai-powered-attack-exploited-papercut-flaws-to-hack-395-organizations/) | 33.0 | 20.0 | 42.0 |
| [システムがランサム被害、一部業務を停止 - インキメーカー](https://www.security-next.com/189674) | 30.0 | 30.0 | 42.0 |
| [ANY.RUN、G2のマルウェア分析ランキングでリーダー評価を獲得](https://any.run/cybersecurity-blog/g2-leader-fall-2026/) | 30.0 | 20.0 | 42.0 |
| [チャットAIのClaudeに「カートに追加するボタンを青色にして」とウェブデザインの変更を依頼すると堂々巡りで全く完成しない様子を再現した「Opusfived」](https://gigazine.net/news/20260910-opusfived/) | 29.0 | 20.0 | 42.0 |
| [金融セクターの脅威動向2026：資金の流れを追う](https://www.intel471.com/blog/follow-the-money-the-financial-sectors-threat-landscape-in-2026) | 28.0 | 30.0 | 42.0 |
| [Cisco FMCの脆弱性がランサムウェア組織や国家支援型ハッカーに悪用される](https://www.bleepingcomputer.com/news/security/cisco-fmc-flaws-exploited-by-ransomware-gang-state-sponsored-hackers/) | 28.0 | 30.0 | 42.0 |
| [攻撃者が従業員の個人用電話に連絡してMicrosoft 365アカウントに侵入](https://www.helpnetsecurity.com/2026/09/10/microsoft-365-social-engineering-personal-phones/) | 28.0 | 20.0 | 42.0 |
| [FBIが初のサイバー戦略を公開、脅威アクターの妨害に注力](https://www.infosecurity-magazine.com/news/fbi-cyber-strategy-disrupting/) | 28.0 | 20.0 | 42.0 |
| [GigabudがAndroidのワークプロファイルを作成し、銀行アプリのマルウェア検知を回避](https://thehackernews.com/2026/09/gigabud-creates-android-work-profiles.html) | 28.0 | 20.0 | 42.0 |
| [AdaptHealthのデータ侵害で410万人に影響](https://www.securityweek.com/4-1-million-impacted-by-adapthealth-data-breach/) | 28.0 | 20.0 | 42.0 |
| [偽のGTA 6ダウンロードでマルウェア入りバンドルを配布、発売を待ちきれないゲーマーを狙う](https://www.helpnetsecurity.com/2026/09/10/fake-gta-6-downloads-malware-ransomware/) | 28.0 | 20.0 | 42.0 |
| [Apple、最も必要とする人向けの写真検証機能を開発中](https://www.helpnetsecurity.com/2026/09/10/apple-reference-image-iphone-18-pro/) | 28.0 | 20.0 | 42.0 |
| [OpenAIのAIエージェントによるハッキング事件で他にも最低10件のサイトが侵害されていたことが判明](https://gigazine.net/news/20260910-openai-agent-hacking-incident-another-sites/) | 27.0 | 20.0 | 42.0 |
| [「AI社員」活用、NECは無人部署・DeNAには17体 南場社長「けなげ」と太鼓判](https://www.itmedia.co.jp/news/article/2609/10/2000001380/) | 26.0 | 20.0 | 42.0 |
| [PaperCut攻撃者はHundreds of AI agentsを使い395以上の組織を標的に、制御不能になるものもあった](https://www.theregister.com/security/2026/09/10/hundreds-of-ai-agents-helped-papercut-attacker-hit-395-orgs-and-some-went-off-script/5295650) | 25.0 | 20.0 | 42.0 |
| [Cyber Command、情報機関のベテランをAI責任者に起用](https://therecord.media/cyber-command-ai-leader-ronzelle-green) | 25.0 | 20.0 | 42.0 |
| [脅威グループがAIでサイバー攻撃能力を強化](https://www.cybersecuritydive.com/news/threat-groups-enhance-cyberattack-capabilities-ai/830055/) | 25.0 | 20.0 | 42.0 |
| [Akamai Web Security Analytics向けAIアシスタントの紹介](https://www.akamai.com/blog/security/2026/sep/introducing-ai-assistant-web-security-analytics) | 25.0 | 20.0 | 42.0 |
| [Anthropicの研究者がAI開発の危険性を警告して辞任](https://www.securityweek.com/anthropic-researcher-resigns-with-warning-about-the-dangers-of-ai-development/) | 25.0 | 20.0 | 42.0 |
| [PuzzleMask: 平文の文章を悪用した隠密AI攻撃ベクトル](https://research.checkpoint.com/2026/puzzlemask-abusing-plain-prose-as-a-covert-ai-attack-vector/) | 25.0 | 20.0 | 42.0 |
| [CISA、インサイダー脅威ガイドを更新し新たな緩和策を追加](https://www.infosecurity-magazine.com/news/cisa-updates-insider-threat-guide/) | 25.0 | 20.0 | 42.0 |
| [AIは今後10年以内に人類を滅ぼすのか？](https://www.malwarebytes.com/blog/ai/2026/09/will-ai-kill-us-all-within-the-next-decade) | 25.0 | 20.0 | 42.0 |
| [拡大したスキャンで4件目の不正Claudeサイバー事案を確認](https://www.securityweek.com/widened-scan-turns-up-fourth-rogue-claude-cyber-incident/) | 25.0 | 20.0 | 42.0 |
| [PaperCut攻撃者が数百のAIエージェントを使い440件超のインスタンスを侵害](https://thehackernews.com/2026/09/papercut-attacker-uses-hundreds-of-ai.html) | 25.0 | 20.0 | 42.0 |
| [Scytale、AI搭載のTPRMツールでベンダーリスク管理を拡充](https://www.helpnetsecurity.com/2026/09/10/scytale-ai-third-party-risk-management-capabilities/) | 25.0 | 20.0 | 42.0 |
| [OpenAIとAnthropicが、暴走したAIエージェントの被害が当初より深刻だったと認める](https://www.itpro.com/security/openai-and-anthropic-admit-rogue-ai-agents-did-more-than-first-thought) | 25.0 | 20.0 | 42.0 |
| [Anthropicが明かした新たなサイバーセキュリティインシデント](https://www.infosecurity-magazine.com/news/anthropic-another-cybersecurity/) | 25.0 | 20.0 | 42.0 |
| [AVEVA Pipeline Integrity Monitorの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-253-01) | 24.0 | 46.0 | 50.0 |
| [Check Pointが認証不要のRCEを可能にする9.8評価のVPN証明書2件の脆弱性を公開](https://thehackernews.com/2026/09/check-point-discloses-two-98-rated-vpn.html) | 24.0 | 38.0 | 42.0 |
| [Check Point製品における重大な脆弱性（2026-012）](https://cert.europa.eu/publications/security-advisories/2026-012/) | 24.0 | 38.0 | 42.0 |
| [Nightmare-Eclipseが再び「ShieldCrash」Windows Exploitで攻撃](https://www.darkreading.com/vulnerabilities-threats/nightmare-eclipse-strikes-again-shieldcrash-windows-exploit) | 22.0 | 20.0 | 43.0 |
| [採用管理プラットフォームに不正アクセス - きちりHD子会社](https://www.security-next.com/190132) | 22.0 | 20.0 | 42.0 |
| [学生の個人情報含むバックアップHDDが所在不明 - 秋田高専](https://www.security-next.com/189482) | 22.0 | 20.0 | 42.0 |
| [「Citrix Workspace app for Windows」に2件の脆弱性](https://www.security-next.com/190113) | 22.0 | 20.0 | 42.0 |
| [さくらインターネット、不正アクセス調査が完了 - 会員情報136万アカウントに閲覧・取得の可能性](https://news.mynavi.jp/techplus/article/20260910-4946867/) | 21.0 | 20.0 | 42.0 |
| [Android利用者要注意、不正アプリへ誘導するフィッシング - 「ポイントプレゼント」装う](https://news.mynavi.jp/techplus/article/20260910-4945569/) | 21.0 | 20.0 | 42.0 |
| [日本はコンプライアンス先行、サイバー防御のレジリエンスに課題--Arctic Wolf調査](https://japan.zdnet.com/article/35252497/) | 21.0 | 20.0 | 42.0 |
| [Orthanc DICOM Serverの脆弱性](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-253-02) | 20.0 | 28.0 | 50.0 |
| [NextGen Healthcare Mirth Connectの脆弱性情報](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-253-01) | 20.0 | 28.0 | 50.0 |
| [Surfshark VPNが内部テスト用およびプロキシサーバーへの侵入を公表](https://www.bleepingcomputer.com/news/security/surfshark-vpn-says-hackers-breached-internal-testing-proxy-servers/) | 20.0 | 20.0 | 42.0 |
| [Microsoft ExcelのKB5002914更新で一部ユーザーのコピー＆ペーストが動作しない問題](https://www.bleepingcomputer.com/news/microsoft/microsoft-excel-kb5002914-update-breaks-copy-and-paste-for-some-users/) | 20.0 | 20.0 | 42.0 |
| [IDScanが侵害を確認、ハッカーが1億5300万件の運転免許証スキャンを販売へ](https://therecord.media/idscan-data-breach-notice-drivers-licenses) | 20.0 | 20.0 | 42.0 |
| [ThreatsDay: 200件のAndroid脆弱性、ブラウザ内で完結するフィッシング、11.9万件の詐欺ショップほか23件の話題](https://thehackernews.com/2026/09/threatsday-200-android-flaws-browser.html) | 20.0 | 20.0 | 42.0 |
| [Ivanti製品における複数の脆弱性により任意コード実行が可能となるおそれ](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-ivanti-products-could-allow-for-arbitrary-code-execution_2026-093) | 20.0 | 20.0 | 42.0 |
| [サイバーセキュリティ分野のM&A総括：2026年8月に発表された33件の取引](https://www.securityweek.com/cybersecurity-ma-roundup-33-deals-announced-in-august-2026/) | 20.0 | 20.0 | 42.0 |
| [Androidでpasskeysがパスワードマネージャー間を移行可能に](https://www.helpnetsecurity.com/2026/09/10/google-android-password-manager-transfer/) | 20.0 | 20.0 | 42.0 |
| [BlueMoon exploit kitがChromeとWindowsの脆弱性を悪用する攻撃に転用](https://www.malwarebytes.com/blog/bugs/2026/09/bluemoon-exploit-kit-turns-chrome-and-windows-flaws-into-attacks) | 20.0 | 20.0 | 42.0 |
| [IDScan、1億5300万件の運転免許証窃取に関連する侵害を確認](https://www.bleepingcomputer.com/news/security/idscan-confirms-breach-tied-to-153-million-stolen-drivers-licenses/) | 20.0 | 20.0 | 42.0 |
| [Hacker Conversations: Vinnie Liu、パフォーマーからリングマスターへ](https://www.securityweek.com/hacker-conversations-vinnie-liu-performer-turned-ringmaster/) | 20.0 | 20.0 | 42.0 |
| [ホワイトハウス、テキサス州の水分野サイバーセキュリティ連携を全国の青写真と位置付け](https://www.cybersecuritydive.com/news/water-cybersecurity-white-house-oncd-texas-partnership-cairncross/830029/) | 20.0 | 20.0 | 42.0 |
| [CISA、数百件の重要な欠員補充が目前に](https://www.cybersecuritydive.com/news/cisa-hiring-circia-anchor-nick-andersen/829980/) | 20.0 | 20.0 | 42.0 |
| [四半期にわたる全アラート分析で判明した4大脅威](https://www.bleepingcomputer.com/news/security/the-top-4-threats-we-found-by-investigating-every-alert-for-a-quarter/) | 20.0 | 20.0 | 42.0 |
| [政府はイノベーションとセキュリティの競争で「時間を買っている」と米国家サイバー担当高官が発言](https://cyberscoop.com/national-cyber-director-ai-cybersecurity-threats/) | 20.0 | 20.0 | 42.0 |
| [Anne Hathawayを名乗る人物が2億4500万ドル相当の暗号資産窃取グループを主導し、ナイトクラブや時計、高級車に散財](https://www.bitdefender.com/en-us/blog/hotforsecurity/anne-hathaway-245-million-crypto-theft-nightclubs-watches-luxury-cars) | 20.0 | 20.0 | 42.0 |
| [Russian e-commerce大手Wildberries、DDoS攻撃で出品者への支払いが遅延](https://therecord.media/russian-e-commerce-giant-wildberries-says-payments-disrupted) | 20.0 | 20.0 | 42.0 |
| [ShinyHuntersによるMcKessonへの攻撃で640万人分の情報が流出](https://www.theregister.com/security/2026/09/10/shinyhunters-expose-64m-in-attack-on-medical-supplier-mckesson/5295550) | 20.0 | 20.0 | 42.0 |
| [1.1.1.1がポスト量子DNSSECをサポート、全2,420バイトに対応](https://blog.cloudflare.com/post-quantum-dnssec-1111/) | 20.0 | 20.0 | 42.0 |
| [英国、National Cyber Forceの新司令官を任命](https://therecord.media/uk-appoints-new-commander-of-national-cyber-force) | 20.0 | 20.0 | 42.0 |
| [Wiz、GovRAMP High認証を取得](https://www.wiz.io/blog/wiz-govramp-high) | 20.0 | 20.0 | 42.0 |
| [「被害者のブラウザ内にのみ存在するフィッシングページ」に関する警告をサイバー研究者が発出](https://www.itpro.com/security/phishing/cyber-researchers-issue-warning-over-phishing-pages-that-exist-only-inside-the-victims-browser) | 20.0 | 20.0 | 42.0 |
| [WordPressが危険なプラグインリリースを防ぐ自動セキュリティチェックを導入](https://www.helpnetsecurity.com/2026/09/10/wordpress-automated-plugin-security-review/) | 20.0 | 20.0 | 42.0 |
| [SPIFFE/SPIREにおける侵害後のID悪用の実態](https://unit42.paloaltonetworks.com/kubernetes-spiffe-spire-identity-spoofing/) | 20.0 | 20.0 | 42.0 |
| [MITRE ATT&CK T1047における検知のギャップ](https://www.security.com/expert-perspectives/detection-gap-mitre-attck-t1047) | 20.0 | 20.0 | 42.0 |
| [Instagramアカウントを停止させた著作権詐欺師が金銭を要求](https://www.malwarebytes.com/blog/scams/2026/09/copyright-scammers-get-instagram-accounts-suspended-and-demand-payment) | 20.0 | 20.0 | 42.0 |

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
