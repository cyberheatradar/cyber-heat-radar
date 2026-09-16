# 📡 サイレーダー 2026-09-17 05:00 JST

このレポートは、2026-09-16 17:00 JST〜2026-09-17 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 138
- [音声で扱う想定のトピック](#audio-topics): 9
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 103

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Google Pixel owners urged to patch actively exploited modem flaw](#topic-32998) | 63.0 | 58.0 | 63.0 | 音声 | 温度感上位枠 |
| 2 | [Cisco Secure Firewall Management Center Software Authentication Bypass Vulnerability](#topic-24944) | 55.0 | 74.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [Acronis backup plugin flaw exploited in targeted attacks (CVE-2026-87886)](#topic-33023) | 50.0 | 58.0 | 59.0 | 音声 | 温度感上位枠 |
| 4 | [Cisco Secure Firewall Adaptive Security Appliance, Secure Firewall Threat Defense, and Secure Firewall Management Center Software Hardening Release: September 2026](#topic-32969) | 49.0 | 64.0 | 51.0 | 音声 | 温度感上位枠 |
| 5 | [Cisco Secure Firewall Management Center Software Static Credential Vulnerability](#topic-24943) | 45.0 | 64.0 | 66.0 | GitHub | 音声枠上限によりGitHubのみ |
| 6 | [Cisco Identity Services Engine Hardening Release: September 2026](#topic-32952) | 41.0 | 64.0 | 51.0 | 音声 | 温度感上位枠 |
| 7 | [Cisco Secure Firewall Adaptive Security Appliance and Secure Firewall Threat Defense Software Remote Access SSL VPN Denial of Service Vulnerability](#topic-27066) | 40.0 | 64.0 | 59.0 | 音声 | 温度感上位枠 |
| 8 | [Cisco Nexus Dashboard Software Security Hardening Release: September 2026](#topic-32960) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 9 | [EU Chief Warns of AI-Powered Hacking, Moves to Rein In Social Media](#topic-32983) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 10 | [Citrix adds AI-powered browser activity analysis to SecurAccess](#topic-33037) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-32998"></a>

### 1. Google Pixel owners urged to patch actively exploited modem flaw

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 63.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Googleは、Pixel端末のモデム関連の脆弱性CVE-2026-58704に対する修正を公開し、限定的な標的型攻撃で悪用されていたことが示されています。
複数の公開情報では、権限昇格につながる不備として扱われており、既知の悪用が確認された脆弱性として注意が必要です。
モバイル端末の基盤機能に関わる脆弱性のため、影響を受ける端末では攻撃者に不正な権限獲得の足がかりを与えるおそれがあります。
CISAの既知の悪用脆弱性カタログにも追加されており、優先度の高い対応対象と見なせます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象のPixel端末で最新の修正が適用されているか確認し、未適用なら速やかに更新する。
- 資産管理上、Pixel利用者やモバイル端末の更新状況を把握し、重要端末を優先して点検する。
- 同種のモバイル脆弱性は標的型攻撃で使われやすいため、端末更新の徹底と異常挙動の監視を継続する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-58704 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Apple iOS | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-58704](https://nvd.nist.gov/vuln/detail/CVE-2026-58704) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Pixel Modem Zero-Day Exploited in Targeted Attacks](https://www.securityweek.com/pixel-modem-zero-day-exploited-in-targeted-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/09/16/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google Patches Pixel Modem Flaw Amid Signs of Limited Targeted Exploitation](https://thehackernews.com/2026/09/google-patches-pixel-modem-flaw-amid.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google Pixel owners urged to patch actively exploited modem flaw](https://www.malwarebytes.com/blog/mobile/2026/09/google-pixel-owners-urged-to-patch-actively-exploited-modem-flaw) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-24944"></a>

### 2. Cisco Secure Firewall Management Center Software Authentication Bypass Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 55.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Secure Firewall Management Center（FMC）Software に認証回避の脆弱性（CVE-2026-20079）があり、未認証のリモート攻撃者が影響を受ける機器上でスクリプト実行につながる可能性があるとされています。
Cisco は修正版ソフトウェアを公開しており、公開管理インターフェースを持つ環境では特に注意が必要です。
FMC は複数の Cisco Secure Firewall 機器を集中管理するため、影響を受けると管理基盤としての重要性が高い点が注目されています。
公表情報では実際の悪用観測が示されており、優先度の高い対応対象と見られます。

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

- 該当する Cisco Secure Firewall Management Center のバージョンを確認し、ベンダー提供の修正版適用状況を点検する。
- FMC の管理インターフェースが外部公開されていないか確認し、公開範囲を最小化する。
- 管理系ログや不審な HTTP リクエスト、想定外のスクリプト実行の痕跡を確認し、関連製品全体の監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20079 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-20316 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Adaptive Security Appliance | 言及あり | 0.80 | — |
| 製品 | Cisco Firepower Threat Defense | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20079](https://nvd.nist.gov/vuln/detail/CVE-2026-20079) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Firewall Management Center Software Authentication Bypass Vulnerabi](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-onprem-fmc-authbypass-5JPp45V2) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [We've got one word for it, and it's usually the wrong one](https://blog.talosintelligence.com/weve-got-one-word-for-it-and-its-usually-the-wrong-one/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco FMC bugs exploited by nation-state and ransomware actors (CVE-2026-20079, ](https://www.helpnetsecurity.com/2026/09/10/cisco-fmc-exploited-cve-2026-20079-cve-2026-20316/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Organizations Warned of Cisco Secure FMC Exploitation](https://www.securityweek.com/organizations-warned-of-cisco-secure-fmc-exploitation/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco confirms CVE-2026-20079 Secure FMC flaw exploited in attacks](https://www.bleepingcomputer.com/news/security/cisco-confirms-cve-2026-20079-secure-fmc-flaw-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Active exploitation of Cisco Secure Firewall Management Center vulnerabilities](https://blog.talosintelligence.com/fmc-ongoing-exploitation/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-33023"></a>

### 3. Acronis backup plugin flaw exploited in targeted attacks (CVE-2026-87886)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 50.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

Acronisは、cPanelおよびWHM向けのBackupプラグインに存在する脆弱性CVE-2026-87886が、限定的かつ標的型の攻撃で悪用されたと警告しています。
公開情報では、この問題は不適切なファイル権限に起因するローカル権限昇格の脆弱性とされ、CVSS 7.8の高い深刻度が付与されています。
バックアップ関連コンポーネントは運用上の重要度が高く、侵害されると権限拡大や管理環境への影響につながるおそれがあります。
すでに実際の悪用が示されているため、該当環境では通常の脆弱性管理よりも優先度を上げて確認する必要があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Acronis Backup plugin for cPanel/WHMの該当バージョンを棚卸しし、ベンダー案内に沿って速やかに更新・緩和策を適用する。
- cPanel/WHMサーバーで不審なローカル操作や権限昇格の兆候、関連する監査ログを確認する。
- バックアップ管理系プラグインや権限設定を定期点検し、不要な権限付与や古い構成が残っていないか見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-87886 | 関連CVE | 1.00 | 未確認 |
| ベンダー | cPanel | 言及あり | 0.80 | — |
| 製品 | cPanel | 言及あり | 0.80 | — |
| 製品 | WHM | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-87886](https://nvd.nist.gov/vuln/detail/CVE-2026-87886) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Acronis cPanel Backup Plugin Vulnerability Exploited in Targeted Attacks](https://thehackernews.com/2026/09/acronis-cpanel-backup-plugin.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Acronis Patches Exploited Vulnerability in cPanel Backup Plugin](https://www.securityweek.com/acronis-patches-exploited-vulnerability-in-cpanel-backup-plugin/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Acronis backup plugin flaw exploited in targeted attacks (CVE-2026-87886)](https://www.helpnetsecurity.com/2026/09/16/acronis-backup-plugin-vulnerability-exploited-cve-2026-87886/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32969"></a>

### 4. Cisco Secure Firewall Adaptive Security Appliance, Secure Firewall Threat Defense, and Secure Firewall Management Center Software Hardening Release: September 2026

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 49.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

Ciscoは、Secure Firewall ASA/FTD/FMC向けのハードニング更新を公開し、内部調査で見つかった複数の脆弱性に対処したと案内しています。
対象には複数のCVEが含まれ、少なくとも一部は実際の悪用が確認されているとされています。
ファイアウォールや管理センターは境界防御の中核にあたるため、影響がある場合は優先度高く確認が必要です。公開情報では回避策は示されておらず、更新適用が主な対処になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象製品（ASA / FTD / FMC）と導入バージョンを確認し、該当パッチの適用状況を点検する。
- 管理系インターフェースや外部公開面の露出を確認し、不要な公開やアクセス許可がないか見直す。
- 更新前後で機器ログや認証ログを確認し、異常なアクセスや設定変更の痕跡がないか監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20329](https://nvd.nist.gov/vuln/detail/CVE-2026-20329) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Firewall Adaptive Security Appliance, Secure Firewall Threat Defens](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-hardening-asaftdfmc-uvpPROhN) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32952"></a>

### 5. Cisco Identity Services Engine Hardening Release: September 2026

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

Ciscoは、Identity Services Engine（ISE）およびISE-PIC向けに、内部検証で見つかった複数の脆弱性を修正するハードニング版の更新を公開しました。
対象の1件にはCVE-2026-20130が割り当てられており、少なくとも1件については悪用が確認されていると案内されています。
ISEは認証やアクセス制御の中核に関わる製品であり、影響が出るとネットワーク全体の防御に波及し得ます。
Ciscoは修正更新を案内しており、現時点で回避策はないため、適用の優先度が高い事案です。

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

- ISEおよびISE-PICの利用有無を確認し、該当版かどうかを早急に棚卸しする。
- Ciscoが提供する修正更新の適用可否を確認し、優先的にパッチ計画へ組み込む。
- 認証・アクセス制御の異常や不審な管理操作がないか、関連ログを重点的に点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Identity Services Engine | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20130](https://nvd.nist.gov/vuln/detail/CVE-2026-20130) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Identity Services Engine Hardening Release: September 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-hardening-ise-XU5EwX5T) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-27066"></a>

### 6. Cisco Secure Firewall Adaptive Security Appliance and Secure Firewall Threat Defense Software Remote Access SSL VPN Denial of Service Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 40.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

Cisco Secure Firewall ASAおよびFTDのRemote Access SSL VPNサービスに、未認証の遠隔攻撃者によって装置を予期せず再起動させ、サービス拒否（DoS）状態を引き起こしうる脆弱性が報告されています。
CVE-2026-20349として管理されており、Ciscoは修正済みソフトウェア更新を公開しています。
VPN公開機能に関わるため、外部から到達可能な構成では業務影響が出やすく、ファイアウォールの可用性低下に直結する可能性があります。
さらに、公開情報では悪用観測が示されているため、優先度を上げて対応を検討すべき事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
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

- 影響を受けるASA/FTDのバージョンと、Remote Access SSL VPNの利用有無を確認する。
- Ciscoの修正版ソフトウェア適用を優先し、保守手順と再起動影響を踏まえて更新計画を立てる。
- 外部公開VPN装置の再起動・異常終了の監視を強化し、関連するインシデント兆候を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20349 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Adaptive Security Appliance | 言及あり | 0.80 | — |
| 製品 | Cisco Firepower Threat Defense | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20349](https://nvd.nist.gov/vuln/detail/CVE-2026-20349) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Firewall Adaptive Security Appliance and Secure Firewall Threat Def](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-vpn-dos-dzv4mQFF) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco fixes vulnerability exploited to DoS its firewalls (CVE-2026-20349)](https://www.helpnetsecurity.com/2026/08/13/cve-2026-20349-cisco-firewalls-dos/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Patches Firewall Zero-Day Exploited for DoS Attacks](https://www.securityweek.com/cisco-patches-firewall-zero-day-exploited-for-dos-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32960"></a>

### 7. Cisco Nexus Dashboard Software Security Hardening Release: September 2026

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

Cisco Nexus Dashboard向けのソフトウェア強化版リリースで、複数の内部テストで見つかった脆弱性が修正されています。
Ciscoによると、これらの問題は現時点で実際の悪用は確認されておらず、回避策はなく更新適用が必要です。
CVEが付与されており、重要度も高いとされているため、Nexus Dashboardを利用する組織では優先的な確認対象になります。
影響範囲の整理とパッチ適用の判断を早めに進める材料です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Nexus Dashboardの該当バージョンが更新対象かを確認し、ベンダーの修正版適用を優先する。
- 回避策がないため、恒久対策はアップデート中心で検討する。
- 複数のCVEがまとめて扱われているため、個別CVEだけでなく関連する修正全体を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20322](https://nvd.nist.gov/vuln/detail/CVE-2026-20322) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Nexus Dashboard Software Security Hardening Release: September 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-hardening-ndw1-psFvnrg) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32983"></a>

### 8. EU Chief Warns of AI-Powered Hacking, Moves to Rein In Social Media

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

欧州委員長のウルズラ・フォン・デア・ライエン氏が、先進的なAIによってハッキングがこれまでにない規模で拡大しうると警鐘を鳴らしました。
あわせて、子どもへのSNSの影響を抑えるための新たな保護策をEUが検討していることも伝えられています。
AIの高度化は、攻撃の自動化や大量化を通じて脅威の見え方を変える可能性があり、政策面でも関心が高まっています。
SNSと子どもの保護をめぐる規制強化の動きは、テック企業や運用現場にも影響し得ます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIを悪用した攻撃の“量”と“速度”が増える前提で、検知・対応の自動化や監視体制を見直す。
- SNS関連の安全対策や年齢保護の規制動向を追い、利用者向け設定や社内ガイドラインに反映する。
- AI生成のフィッシングやなりすましを想定し、本人確認や承認フローを再点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [EU Chief Warns of AI-Powered Hacking, Moves to Rein In Social Media](https://www.securityweek.com/eu-chief-warns-of-ai-powered-hacking-moves-to-rein-in-social-media/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33037"></a>

### 9. Citrix adds AI-powered browser activity analysis to SecurAccess

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Citrixは、Chrome Enterpriseと組み合わせたSecurAccess向けに、ブラウザー上の操作を記録・分析できるAI機能「Citrix Session Insights」を発表しました。
利用者だけでなく自律型エージェントのブラウザー活動も対象に、視覚的なセッション証跡やリスク分析、推奨事項を提供するとされています。
ブラウザーが業務とAI活用の共通基盤になりつつある中、操作の可視化と監査性を高める取り組みとして注目されます。インシデント調査や説明責任の確保に役立つ可能性があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ブラウザー上の機密操作やAIエージェントの利用が、監査・証跡の対象になる前提で運用設計を見直す。
- 記録対象、保存期間、アクセス権限、個人情報や機密情報の取り扱いを明確にする。
- AIによる分析結果は補助情報として扱い、最終判断は既存のログや業務文脈と突き合わせて行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Citrix | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Citrix adds AI-powered browser activity analysis to SecurAccess](https://www.helpnetsecurity.com/2026/09/16/citrix-session-insights-capability/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-24943"></a>

### 1. Cisco Secure Firewall Management Center Software Static Credential Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Secure Firewall Management Center（FMC）SoftwareのWebインターフェースに、静的な低権限アカウントの認証情報に起因する脆弱性（CVE-2026-20316）が公表されました。
影響を受ける環境では、認証されていないリモート攻撃者がログインに成功し、機微情報にアクセスできる可能性があるとされています。
CISAの既知悪用脆弱性カタログへの掲載や、実際に悪用されたという文脈があるため、単なる理論上の問題ではなく、優先度の高い対応対象として扱う必要があります。
FMCはネットワーク機器の集中管理基盤であり、影響が広がると管理情報の保護や運用継続性に関わります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Ciscoが提供する修正済みソフトウェアの適用状況を確認し、該当バージョンを速やかに更新する。
- FMC管理インターフェースの公開状況を見直し、インターネットから直接到達できない構成を維持する。
- 管理系ログや不審なログインの痕跡を点検し、想定外のアクセスがないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20316 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20316](https://nvd.nist.gov/vuln/detail/CVE-2026-20316) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Firewall Management Center Software Static Credential Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-fmc-static-cred-BET3Cjh) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco FMC static credentials exploited by attackers (CVE-2026-20316)](https://www.helpnetsecurity.com/2026/07/30/cisco-fmc-cve-2026-20316-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure FMC Zero-Day Exploited in the Wild](https://www.securityweek.com/cisco-secure-fmc-zero-day-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco FMC Zero-Day Actively Exploited, Static Credentials Could Expose Sensitive](https://thehackernews.com/2026/07/cisco-fmc-zero-day-actively-exploited.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of FMC static credential flaw exploited in zero-day attacks](https://www.bleepingcomputer.com/news/security/cisco-warns-of-fmc-static-credential-flaw-exploited-in-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [ハッカーがCiscoメールゲートウェイのゼロデイ脆弱性を悪用](https://www.cybersecuritydive.com/news/hackers-exploit-zero-day-cisco-email-gateway/830553/) | 37.0 | 38.0 | 43.0 |
| [ScreenConnectの致命的な脆弱性が現在攻撃で悪用中](https://www.bleepingcomputer.com/news/security/cisa-warns-of-hackers-exploiting-critical-screenconnect-flaw/) | 37.0 | 38.0 | 43.0 |
| [TP-Linkカメラのゼロデイ脆弱性が盗聴を可能にする](https://www.infosecurity-magazine.com/news/zeroday-tplink-cameras/) | 37.0 | 38.0 | 43.0 |
| [3つの脅威グループがバックドア、ランサムウェア、ワイパーでロシア企業を標的にしている](https://thehackernews.com/2026/09/three-threat-groups-target-russian.html) | 36.0 | 30.0 | 42.0 |
| [Cisco Secure Firewall Adaptive Security ApplianceおよびSecure Firewall Threat Defense SoftwareのSSL VPNサービス拒否脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftdvirtual-dos-MuenGnYR) | 32.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Adaptive Security ApplianceおよびSecure Firewall Threat Defense SoftwareのIKEv2証明書認証におけるサービス拒否脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-ikev2cert-dos-uWyc2xtv) | 32.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Adaptive Security ApplianceおよびSecure Firewall Threat Defense SoftwareのObject Group Access Control Listバイパス脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ftd-acl-bypass-8p6vFvw) | 32.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Adaptive Security ApplianceおよびSecure Firewall Threat Defense SoftwareのEIGRPサービス拒否脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-eigrp-dos-GOhNejSj) | 32.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Threat Defense Software Snort 2のSSL/TLSサービス妨害の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ftd-snort2-ssldos-Mw7WYX9c) | 32.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Management CenterおよびSecure Firewall Threat Defense Softwareのsftunnel脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-fmcftd-sftun-multivulns-WGVHOrN3) | 32.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Adaptive Security ApplianceおよびSecure Firewall Threat Defense Softwareのログ機能におけるサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asa-ftd-logging-dos-ZXXNesfN) | 32.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Adaptive Security ApplianceおよびSecure Firewall Threat Defense SoftwareのDTLSサービス拒否脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-dtls-dos-Kp57HkyO) | 32.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Adaptive Security ApplianceおよびSecure Firewall Threat Defense SoftwareのTCP DNSサービス拒否脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-tcpdns-dos-p6dUnjr5) | 32.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Management Center Software の Java デシリアライズによるリモートコード実行脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-fmc-javarce-y2NypXwk) | 32.0 | 46.0 | 50.0 |
| [Cisco Secure Firewall Threat Defense SoftwareのTLS 1.3サービス拒否脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ftd-tls1.3-dos-dLxwFWgF) | 32.0 | 46.0 | 50.0 |
| [Parallels Desktopの脆弱性により、Mac上の任意のローカルユーザーがroot権限を取得可能に（CVE-2026-90894）](https://www.helpnetsecurity.com/2026/09/16/parallels-desktop-cve-2026-90894-parashells-vulnerability/) | 30.0 | 28.0 | 50.0 |
| [ランサムウェア攻撃の真のコスト：BCDRの有無で見る違い](https://www.bleepingcomputer.com/news/security/the-true-cost-of-a-ransomware-attack-with-and-without-bcdr/) | 28.0 | 30.0 | 42.0 |
| [Cisco Secure Firewall Management Center Softwareの脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-fmc-mulivulns-4PsnFwvx) | 28.0 | 28.0 | 50.0 |
| [Cisco Secure Firewall Management Center SoftwareのsftunnelにおけるRoot権限の任意コード実行の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-fmc-sftunn-codex-c3O4Jft2) | 28.0 | 28.0 | 50.0 |
| [NightEagleがロシア企業を標的にする](https://securelist.com/tr/nighteagle-apt-ghostcontainer-and-tunneling/121323/) | 28.0 | 28.0 | 50.0 |
| [イランのハッカーがCHOSEN BRICKデータ窃取マルウェアで反体制派やジャーナリストを監視](https://www.helpnetsecurity.com/2026/09/16/iranian-hackers-chosen-brick-malware-dissidents-journalists/) | 28.0 | 20.0 | 48.0 |
| [マルウェアがブラウザのチェックを回避してChromeとEdgeの拡張機能を強制インストール](https://www.bleepingcomputer.com/news/security/malware-bypasses-browser-checks-to-force-install-chrome-edge-extensions/) | 28.0 | 20.0 | 42.0 |
| [PHP WebshellキャンペーンがWordPressを狙う重大なWooCommerceプラグインの脆弱性](https://www.infosecurity-magazine.com/news/woocommerce-wholesale-lead-capture/) | 28.0 | 20.0 | 42.0 |
| [米英蘭の当局、イランの監視型マルウェア「Chosen Brick」を公開](https://www.securityweek.com/us-uk-dutch-agencies-expose-iranian-chosen-brick-surveillance-malware/) | 28.0 | 20.0 | 42.0 |
| [サイバーデコイを活用した検知と対応の強化](https://www.cisa.gov/resources-tools/resources/using-cyber-decoys-strengthen-detection-and-response) | 28.0 | 20.0 | 42.0 |
| [N0va Phishkitが米国とEUの企業を標的に：IDセキュリティに新たな課題](https://thehackernews.com/2026/09/n0va-phishkit-targets-us-and-eu.html) | 28.0 | 20.0 | 42.0 |
| [Atomic macOS (AMOS) Stealerの活動](https://unit42.paloaltonetworks.com/atomic-macos-amos-stealer-activity/) | 28.0 | 20.0 | 42.0 |
| [NCSCと同盟国がイランのスパイウェア キャンペーンを警告](https://www.infosecurity-magazine.com/news/ncsc-allies-warn-iranian-chosen/) | 28.0 | 20.0 | 42.0 |
| [AI時代の脆弱性に備える、パッチ不能な対象の保護](https://blog.talosintelligence.com/securing-the-unpatchable-in-an-age-of-ai-driven-vulnerabilities/) | 27.0 | 20.0 | 42.0 |
| [iPhoneの画像生成AIがアップデートされたので使ってみた、無料で使えるが品質はかなり低め](https://gigazine.net/news/20260916-image-playground-ios-27/) | 27.0 | 20.0 | 42.0 |
| [AIが「同僚AI」を密告するための専用ホットラインが本当に開設される](https://gigazine.net/news/20260916-ai-contact-hotline/) | 27.0 | 20.0 | 42.0 |
| [生成AI活用は過半数に達するもルール浸透は15％止まり](https://japan.zdnet.com/article/35252697/) | 26.0 | 20.0 | 42.0 |
| [“ほったらかしAI動画編集”を「DaVinci Resolve」で試す これが今のベストチョイスかも](https://www.itmedia.co.jp/news/article/2609/16/2000001551/) | 26.0 | 20.0 | 42.0 |
| [AIコーディングアシスタントのセッションを乗っ取り、約100のリポジトリにShai-Huludを拡散](https://thehackernews.com/2026/09/attacker-hijacks-ai-coding-assistant.html) | 25.0 | 45.0 | 42.0 |
| [暴走したAIエージェントが5万ドルのクラウド請求を発生させた](https://www.helpnetsecurity.com/2026/09/16/google-mandiant-enterprise-ai-security-risks-report/) | 25.0 | 45.0 | 42.0 |
| [スペインのデータ機関がAI活用のデータ侵害を初確認](https://www.bleepingcomputer.com/news/security/spains-data-agency-gets-first-report-of-ai-powered-data-breach/) | 25.0 | 20.0 | 42.0 |
| [スペインで初のAIを用いたデータ窃取攻撃の疑いを報告](https://www.bleepingcomputer.com/news/security/spain-reports-first-alleged-ai-powered-data-theft-attack/) | 25.0 | 20.0 | 42.0 |
| [BragJack攻撃によりブラウザのAgentic AIを逆用可能にする](https://www.darkreading.com/endpoint-security/bragjack-browser-agentic-ai) | 25.0 | 20.0 | 42.0 |
| [スペイン規制当局に初めて報告されたAgentic AIによるデータ漏えい](https://www.securityweek.com/first-agentic-ai-data-breach-reported-to-spanish-regulator/) | 25.0 | 20.0 | 42.0 |
| [1つの拡張機能がChrome、Comet、Edge、Opera Neon、ClaudeのAIアシスタントを乗っ取る可能性がある](https://thehackernews.com/2026/09/one-extension-could-hijack-ai.html) | 25.0 | 20.0 | 42.0 |
| [TreasuryのScott Bessent氏、AIラボへの免責は認めないと発言](https://fedscoop.com/treasury-scott-bessent-ai-labs-liability-exemptions/) | 25.0 | 20.0 | 42.0 |
| [AIUC、企業向けAIエージェント認証のため4,000万ドルを調達](https://www.securityweek.com/aiuc-raises-40-million-to-certify-enterprise-ai-agents/) | 25.0 | 20.0 | 42.0 |
| [Microsoft、classic OutlookでCopilotボタンがまだ表示されないと発表](https://www.bleepingcomputer.com/news/microsoft/microsoft-shares-workaround-for-missing-outlook-copilot-buttons/) | 25.0 | 20.0 | 42.0 |
| [スペインで初めて確認されたAI支援サイバー攻撃](https://www.theregister.com/cyber-crime/2026/09/16/spain-gets-its-first-taste-of-ai-aided-cyber-attack/5296844) | 25.0 | 20.0 | 42.0 |
| [自己改善型AIは減速すべきとフォン・デア・ライエン氏がEU議会に警告](https://www.helpnetsecurity.com/2026/09/16/eu-ursula-von-der-leyen-ai/) | 25.0 | 20.0 | 42.0 |
| [Hackuity、AI搭載の脆弱性管理向けに1900万ドルを調達](https://www.securityweek.com/hackuity-raises-19-million-for-ai-powered-vulnerability-management/) | 25.0 | 20.0 | 42.0 |
| [Cohesity、AIエージェントと管理データ向けの復旧機能を追加](https://www.helpnetsecurity.com/2026/09/16/cohesity-agent-resilience-capability/) | 25.0 | 20.0 | 42.0 |
| [Rubrik MCPがAIエージェントにセキュリティインテリジェンスへの制御されたアクセスを提供](https://www.helpnetsecurity.com/2026/09/16/rubrik-mcp/) | 25.0 | 20.0 | 42.0 |
| [Nozomi Compassが産業向けチームのOT資産と脆弱性管理を支援](https://www.helpnetsecurity.com/2026/09/16/nozomi-networks-compass/) | 25.0 | 20.0 | 42.0 |
| [Hugging Face上で不正なOpenAI Agentの活動を追跡する](https://www.sentinelone.com/labs/agents-at-large-tracing-illicit-openai-agent-activity-on-hugging-face/) | 25.0 | 20.0 | 42.0 |
| [AIが詐欺師のために巧妙なアンチウイルス更新ページの作成を支援](https://www.malwarebytes.com/blog/threat-intel/2026/09/ai-helps-scammers-build-convincing-antivirus-renewal-pages) | 25.0 | 20.0 | 42.0 |
| [Cisco Identity Services Engineの認証回避脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ISE-ABP-VNSW7Tn5) | 24.0 | 46.0 | 50.0 |
| [Cisco Identity Services Engineの認証回避脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-multiauth-bypass-sgD2HbL4) | 24.0 | 46.0 | 50.0 |
| [Cisco Identity Services Engineの脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-multi-hrP9jQSQ) | 24.0 | 46.0 | 50.0 |
| [Cisco Identity Services Engineの802.1Xセッションハイジャックおよび情報漏えいの脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-multi-vuln-kWLeNnRD) | 24.0 | 46.0 | 50.0 |
| [Cisco Identity Services Engine の認証済みリモートコード実行および API の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-mult-vul-ymSsTLCc) | 24.0 | 46.0 | 50.0 |
| [Cisco Identity Services Engineのリモートコード実行の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-rce-se7bYU57) | 24.0 | 46.0 | 50.0 |
| [Cisco ThousandEyes Virtual Applianceの認証済みWebインターフェースにおけるコマンドインジェクション脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-teva-os-command-W4GAO6jp) | 24.0 | 46.0 | 50.0 |
| [Cisco Identity Services EngineのRADIUSによるサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-RADIUS-dos-wR3hYPMw) | 24.0 | 46.0 | 50.0 |
| [Cisco Identity Services Engineのクロスサイトスクリプティング脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-xss-Uz9VWRQ) | 24.0 | 46.0 | 50.0 |
| [Cisco Identity Services Engineのコマンドインジェクションの脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-cmd-inj-e2CuZCYZ) | 24.0 | 46.0 | 50.0 |
| [AttackersがIssabel Frameworkの脆弱性を悪用し、認証なしでOSコマンドを実行可能にする問題](https://thehackernews.com/2026/09/attackers-exploit-issabel-framework.html) | 24.0 | 46.0 | 50.0 |
| [認証不要のRCE脆弱性により20万件超のWordPressサイトが乗っ取りの危機](https://www.securityweek.com/unauthenticated-rce-flaws-could-expose-200000-wordpress-sites-to-takeover/) | 24.0 | 38.0 | 42.0 |
| [Cisco Identity Services Engineの情報漏えい脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-inf-disc-LFWvcCu) | 22.0 | 36.0 | 50.0 |
| [ロート製薬の不正アクセス、顧客との通話音声データが流出の可能性](https://www.security-next.com/190377) | 22.0 | 20.0 | 42.0 |
| [クリエイティブ業界向け求人サービス「CINRA JOB」に不正アクセス](https://www.security-next.com/189866) | 22.0 | 20.0 | 42.0 |
| [元従業員が顧客情報を持ち出し、拾得者の連絡で判明 - プルデンシャル生命](https://www.security-next.com/190321) | 22.0 | 20.0 | 42.0 |
| [Apple、「macOS Golden Gate 27」を公開 - 脆弱性210件に対処](https://www.security-next.com/190401) | 22.0 | 20.0 | 42.0 |
| [フィッシング攻撃の報告数は減少 - 悪用URLは増加傾向](https://www.security-next.com/189537) | 22.0 | 20.0 | 42.0 |
| [WSO2の脆弱性を悪用する攻撃に対する企業向け警告](https://www.securityweek.com/enterprises-warned-of-attacks-exploiting-wso2-vulnerability/) | 21.0 | 28.0 | 54.0 |
| [Salesforceで大規模障害 「夕方以降に落ちるなんて」阿鼻叫喚 PayPayのフォームにも影響](https://www.itmedia.co.jp/news/article/2609/16/2000001562/) | 21.0 | 20.0 | 42.0 |
| [Gyazoに不正アクセス ユーザー情報約2362万件、画像メタデータ約4.9億件が流出](https://www.itmedia.co.jp/news/article/2609/16/2000001560/) | 21.0 | 20.0 | 42.0 |
| [Cisco BroadWorks CommPilot Application Softwareの認可バイパス脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-auth-bypass-broadwor-57m9dmm5) | 20.0 | 28.0 | 50.0 |
| [Cisco Identity Services Engineの認可バイパス脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-auth-bypass-1-MxcTNgwx) | 20.0 | 28.0 | 50.0 |
| [Cisco Identity Services EngineのSQLインジェクション脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-sql-inj-3QTKR947) | 20.0 | 28.0 | 50.0 |
| [Cisco Identity Services Engineの複数のパストラバーサル脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-multi-traversal-WDTgYCdn) | 20.0 | 28.0 | 50.0 |
| [Cisco Identity Services EngineのSQLおよびHQLインジェクション脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-multisql-inject-JnHK54Rq) | 20.0 | 28.0 | 50.0 |
| [米国行きの外国籍船舶に対するCyberattack調査で沿岸警備隊とFBIが立ち入り調査](https://cyberscoop.com/coast-guard-fbi-investigate-tanker-cyberattacks/) | 20.0 | 20.0 | 48.0 |
| [海上保安当局とFBIが「外国のサイバー攻撃者」による攻撃後にタンカーへ乗船](https://therecord.media/oil-tanker-cyberattack-coast-guard-fbi) | 20.0 | 20.0 | 42.0 |
| [下院、地方警察に詐欺対策ツールを提供する法案を可決](https://therecord.media/house-passes-bill-to-equip-local-law-enforcement-scams) | 20.0 | 20.0 | 42.0 |
| [Data Broker Radaris、プライバシー争いでドメインを失う](https://krebsonsecurity.com/2026/09/data-broker-radaris-loses-domains-in-privacy-fight/) | 20.0 | 20.0 | 42.0 |
| [厳しい技術環境を乗り越えてドラゴンに立ち向かう方法](https://www.darkreading.com/cybersecurity-careers/finding-hope-brutal-job-market) | 20.0 | 20.0 | 42.0 |
| [Salesforce、英国でのAgentforce推進に向けフォワードデプロイドエンジニアを増強](https://www.itpro.com/security/salesforce-doubles-down-on-forward-deployed-engineers-in-uk-agentforce-push) | 20.0 | 20.0 | 42.0 |
| [Google Pixelスマートフォンがゼロクリック攻撃で侵害される問題](https://www.theregister.com/security/2026/09/16/google-pixel-phones-pwned-in-zero-click-attacks/5296936) | 20.0 | 20.0 | 42.0 |
| [International Meteor OrganizationのWebサイトがサイバー攻撃で重大な打撃を受ける](https://therecord.media/international-meteor-organization-cyberattack) | 20.0 | 20.0 | 42.0 |
| [CISA、分野別ではなく汎用インフラセキュリティ専門家の採用を検討](https://www.cybersecuritydive.com/news/cisa-critical-infrastructure-experts-hiring-ai-election-security/830550/) | 20.0 | 20.0 | 42.0 |
| [CISAとNISTがクラウドのIDトークンを保護するためのガイダンスを発行](https://www.infosecurity-magazine.com/news/cisa-nist-cloud-identity-token/) | 20.0 | 20.0 | 42.0 |
| [Parallels Desktopの脆弱性で非管理者のMacユーザーがroot権限を取得可能、ただしIntel Macは修正を適用不可](https://thehackernews.com/2026/09/parallels-desktop-flaw-lets-non-admin.html) | 20.0 | 20.0 | 42.0 |
| [EU chiefが求めるサイバー攻撃と破壊工作への共同対応](https://therecord.media/eu-chief-wants-joint-response-to-cyberattacks) | 20.0 | 20.0 | 42.0 |
| [Gyazoに不正アクセス 情報漏えい](https://news.yahoo.co.jp/pickup/6595526?source=rss) | 20.0 | 20.0 | 42.0 |
| [CISAの新ガイダンス、重要インフラの悪意あるサイバー活動の検知・監視・阻止を支援](https://www.cisa.gov/news-events/news/new-cisa-guidance-helps-critical-infrastructure-detect-observe-and-impede-malicious-cyber-activity) | 20.0 | 20.0 | 42.0 |
| [英国の中小企業はサイバー攻撃に最も脆弱](https://www.itpro.com/security/uk-smbs-are-the-most-vulnerable-to-cyber-attacks) | 20.0 | 20.0 | 42.0 |
| [Threat Intelligence だけでは悪用のギャップは埋められない](https://thehackernews.com/2026/09/threat-intelligence-alone-wont-close.html) | 20.0 | 20.0 | 42.0 |
| [サイバー攻撃による組織の平均被害額は52,000ドル](https://www.infosecurity-magazine.com/news/cyberattacks-cost-organizations/) | 20.0 | 20.0 | 42.0 |
| [Premier Medical Groupのデータ侵害で28万人に影響](https://www.securityweek.com/280000-impacted-by-premier-medical-group-data-breach/) | 20.0 | 20.0 | 42.0 |
| [法務省、裁判所職員によるSouthport被害者ファイル閲覧を受け謝罪](https://www.theregister.com/security/2026/09/16/ministry-of-justice-apologizes-after-court-staff-accessed-southport-victims-files/5296808) | 20.0 | 20.0 | 42.0 |
| [CenterPoint Energy、ハッキングフォーラムでの主張を受けデータ侵害を確認](https://www.helpnetsecurity.com/2026/09/16/centerpoint-energy-data-breach-hacker-claims/) | 20.0 | 20.0 | 42.0 |
| [Chrome、Firefoxの更新で115件の脆弱性を修正](https://www.securityweek.com/chrome-firefox-updates-patch-115-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [画像共有サービス「Gyazo」に不正アクセス、ユーザー情報約2362万件・画像メタデータ約4.9億件が漏えい](https://internet.watch.impress.co.jp/docs/news/2141538.html) | 20.0 | 20.0 | 42.0 |
| [静かな環境に潜む機密データ](https://www.security.com/product-insights/sensitive-data-thrives-quiet-environment) | 20.0 | 20.0 | 42.0 |
| [ムラウチドットコム、不正アクセスにより約771万件の個人情報漏えい](https://internet.watch.impress.co.jp/docs/news/2141530.html) | 20.0 | 20.0 | 42.0 |
| [主要なサイバーセキュリティベンダーがMITRE評価の変更を受けて新たな英国のテストプログラムへ移行](https://www.infosecurity-magazine.com/news/cyber-vendors-mitre-uk-testing/) | 20.0 | 20.0 | 42.0 |
| [Oracle、2026年9月のセキュリティ更新で800件超の脆弱性を修正](https://www.securityweek.com/oracle-patches-800-vulnerabilities-in-september-2026-security-update/) | 20.0 | 20.0 | 42.0 |

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
