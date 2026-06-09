# 📡 サイレーダー 2026-06-10 05:00 JST

このレポートは、2026-06-09 17:00 JST〜2026-06-10 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 98
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 3
- [低温だが記録しておくトピック](#low-record-topics): 63

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Microsoft 2026年6月 Patch Tuesday 関連まとめ](#topic-15857) | 64.0 | 69.0 | 58.0 | 音声 | 温度感上位枠 |
| 2 | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN Validator Authenticated Privilege Escalation Vulnerability](#topic-4945) | 63.0 | 84.0 | 67.0 | 音声 | 温度感上位枠 |
| 3 | [Check Point VPN Zero-Day Exploited in Qilin Ransomware Attacks](#topic-16271) | 49.0 | 66.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Google Releases Patch for Chrome Vulnerability Exploited in the Wild](#topic-16168) | 48.0 | 46.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 5 | [Check Point warns of zero-day flaw targeted by ransomware affiliate](#topic-16226) | 45.0 | 48.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [Check Point Warns Critical Auth Bypass Bug Exploited in the Wild](#topic-16274) | 45.0 | 48.0 | 43.0 | 音声 | 温度感上位枠 |
| 7 | [CVE-2026-42271: CISA KEV catalog addition](#topic-16161) | 42.0 | 64.0 | 55.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 8 | [Will AI Kill the Bug Bounty Industry?](#topic-16260) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 9 | [Cisco customers encounter another SD-WAN zero-day under attack](#topic-15753) | 30.0 | 58.0 | 59.0 | GitHub | 音声枠上限によりGitHubのみ |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-15857"></a>

### 1. Microsoft 2026年6月 Patch Tuesday 関連まとめ

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>A⁠I</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 64.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 69.0 |
| <nobr>確⁠度</nobr> | 58.0 |

#### 概要

Microsoftの2026年6月Patch Tuesdayでは、複数の脆弱性修正が公開され、公開前に知られていたものも含まれていると報じられています。
関連報道では、合計200件超の修正や、深刻度の高い脆弱性、ゼロデイ文脈が取り上げられています。
対象範囲が広く、業務で使われるWindowsや関連製品への影響確認と更新対応が必要になりやすい点が注目されています。
公開済み情報に基づく悪用文脈もあるため、優先度をつけた適用判断が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 実悪用・ゼロデイ文脈。
- 技術詳細・再現情報あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 中。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 技術詳細により影響確認が進みやすい。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 技術詳細・悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 技術詳細、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 該当するMicrosoft製品・エディションを棚卸しし、修正対象かどうかを確認する。
- 優先度の高い更新を先行適用し、検証後に段階的に展開する。
- 関連する監視や検知ルールを見直し、異常兆候がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-44799 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-48563 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-42992 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-41091 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-45657 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-47291 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-44815 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-45585 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-50507 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-49160 | 主要CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft Patches 200 Vulnerabilities](https://www.securityweek.com/microsoft-patches-200-vulnerabilities/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft releases Windows 10 KB5094127 extended security update](https://www.bleepingcomputer.com/news/microsoft/microsoft-releases-windows-10-kb5094127-extended-security-update/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [The June 2026 Security Update Review](https://www.thezdi.com/blog/2026/6/9/the-june-2026-security-update-review) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft June 2026 Patch Tuesday fixes 3 zero-day, 200 flaws](https://www.bleepingcomputer.com/news/microsoft/microsoft-june-2026-patch-tuesday-fixes-3-zero-day-200-flaws/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft June 2026 Patch Tuesday, (Tue, Jun 9th)](https://isc.sans.edu/diary/rss/33064) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Week in review: Cisco SD-WAN 0-day exploited, Patch Tuesday forecast](https://www.helpnetsecurity.com/2026/06/07/week-in-review-cisco-sd-wan-0-day-exploited-june-2026-patch-tuesday-forecast/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 未確認。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 中。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 技術詳細・悪用観測あり。

---

<a id="topic-4945"></a>

### 2. Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN Validator Authenticated Privilege Escalation Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 63.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 84.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

CiscoのCatalyst SD-WAN Controller、Catalyst SD-WAN Manager、Catalyst SD-WAN Validatorに、認証済みのローカル攻撃者がroot権限で任意のコマンドを実行できる脆弱性が公表されました。
CVE-2026-20182として追跡されており、限定的な悪用が確認されているとされています。
SD-WANの制御・管理基盤に関わるため、影響範囲が広くなりやすい点が注目されています。公開PoCの言及もあり、未対応環境では早期の修正適用が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 9 sources。
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

- 該当するCatalyst SD-WAN製品のバージョンと公開済み修正版の適用状況を確認する。
- 管理系インターフェースへのアクセス権限を見直し、不要なローカル利用者やアカウントを減らす。
- 関連製品の監査ログを確認し、不審なファイル操作や権限昇格の兆候がないか点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20182 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20182](https://nvd.nist.gov/vuln/detail/CVE-2026-20182) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN V](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-privesc-4uxFrdzx) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Metasploit Wrap Up 05/22/2026](https://www.rapid7.com/blog/post/pt-metasploit-wrap-up-05-22-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco zero-day under ongoing attack by persistent threat group](https://cyberscoop.com/cisco-sd-wan-zero-day-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco patches another actively exploited SD-WAN zero-day (CVE-2026-20182)](https://www.helpnetsecurity.com/2026/05/15/cisco-sd-wan-zero-day-cve-2026-20182/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Patches Another SD-WAN Zero-Day, the Sixth Exploited in 2026](https://www.securityweek.com/cisco-patches-another-sd-wan-zero-day-the-sixth-exploited-in-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds Cisco SD-WAN CVE-2026-20182 to KEV After Admin Access Exploits](https://thehackernews.com/2026/05/cisa-adds-cisco-sd-wan-cve-2026-20182.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of new critical SD-WAN flaw exploited in zero-day attacks](https://www.bleepingcomputer.com/news/security/cisco-warns-of-new-critical-sd-wan-flaw-exploited-in-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・低信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 中。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。

---

<a id="topic-16271"></a>

### 3. Check Point VPN Zero-Day Exploited in Qilin Ransomware Attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 49.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 66.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Check PointのVPN製品に関するゼロデイの認証回避脆弱性が、Qilinランサムウェア攻撃で悪用されたと報じられています。
報告内容によれば、この問題により正しいパスワードなしでVPN接続が成立する可能性があるとされています。
VPNは社内ネットワークへの入口になりやすく、認証回避の脆弱性は侵入の起点として重大です。
ランサムウェアの文脈での悪用が示されているため、境界防御だけでなく早急な影響確認が重要になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 対象となるCheck Point VPN環境の利用有無を確認し、ベンダーの修正情報や注意喚起を点検する。
- VPN認証や接続ログを確認し、不審な接続や普段と異なる挙動がないかを洗い出す。
- 侵入経路になり得るため、認証情報の見直しや多要素認証、監視強化を優先する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ransomware_group | Qilin | 主題 | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Check Point VPN Zero-Day Exploited in Qilin Ransomware Attacks](https://www.securityweek.com/check-point-vpn-zero-day-exploited-in-qilin-ransomware-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・低信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-16226"></a>

### 4. Check Point warns of zero-day flaw targeted by ransomware affiliate

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Check Pointは、自社のVPN展開に関するゼロデイ脆弱性が、5月上旬以降に悪用されていると警告しています。
現時点の材料では、ランサムウェア関連の攻撃者による標的化が示されていますが、影響範囲の詳細は限定的です。
VPNは外部公開されやすく、侵入の起点になりやすいため、認証基盤やリモートアクセス環境の安全性に直結します。
ゼロデイでの悪用が示唆される場合、通常のパッチ適用待ちでは間に合わない可能性があるため注意が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 対象製品・構成が該当するかを確認し、ベンダーの注意喚起や更新情報を継続監視する。
- VPN機器の認証ログ、管理ログ、設定変更履歴を点検し、不審な接続や異常な挙動がないか確認する。
- 可能であれば外部公開面の制限、MFAの有効化、不要な管理機能の露出抑止など、暫定的なリスク低減策を優先する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Check Point warns of zero-day flaw targeted by ransomware affiliate](https://www.cybersecuritydive.com/news/check-point-zero-day-ransomware/822372/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 未確認。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-16274"></a>

### 5. Check Point Warns Critical Auth Bypass Bug Exploited in the Wild

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Check Pointは、自社のRemote Access VPNおよびMobile Access製品に関わる重大な認証回避の脆弱性について、実際に悪用されたと警告しています。
材料では、ランサムウェアグループのQilinがこの脆弱性の悪用に関与したとされています。
認証回避は、正規の認証を経ずに侵入されるおそれがあるため、リモートアクセス基盤にとって影響が大きい領域です。
しかも実際の悪用が示されているため、対象製品を運用している組織は早急な確認が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 対象製品の利用有無とバージョンを確認し、ベンダーの案内に沿って優先対応する。
- VPNやリモートアクセス経由の認証・接続ログを点検し、通常と異なる挙動がないか確認する。
- 外部公開しているリモートアクセス経路の露出を見直し、必要に応じて制限や追加の防御策を適用する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ransomware_group | Qilin | 主題 | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Check Point Warns Critical Auth Bypass Bug Exploited in the Wild](https://www.infosecurity-magazine.com/news/check-point-critical-auth-bypass/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 未確認。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-16260"></a>

### 6. Will AI Kill the Bug Bounty Industry?

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

AnthropicのMythosに関する話題として、AIが脆弱性発見の速度を大きく引き上げ、バグバウンティや攻撃的セキュリティの在り方に影響を与える可能性が取り上げられています。
現時点では、脆弱性を見つけること自体の難しさよりも、その後の検証や優先順位付け、対応の方が重要になるという問題意識が示されています。
AIによる脆弱性発見の高速化は、発見件数の増加だけでなく、報告の精査や修正の運用負荷を押し上げる可能性があります。
バグバウンティ運営やセキュリティチームは、従来の前提が変わることを見据えて、プロセスの見直しが必要になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI支援の検出結果を前提に、トリアージと再現確認の体制を見直す。
- バグバウンティ運営では、報告品質のばらつきや重複対応を想定した運用を整える。
- 脆弱性対応のSLAや優先度付けを、発見速度の上昇に合わせて再評価する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Will AI Kill the Bug Bounty Industry?](https://www.securityweek.com/will-ai-kill-the-bug-bounty-industry/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-16168"></a>

### 1. Google Releases Patch for Chrome Vulnerability Exploited in the Wild

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 48.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

GoogleはChromeの脆弱性CVE-2026-11645を修正する更新を公開しました。
複数の報道では、この問題は実際に悪用されていたとされ、ChromeのV8エンジンにおける範囲外アクセスに関係する高リスクの欠陥と説明されています。
広く使われるブラウザの脆弱性であり、悪用が確認されている点から、更新の適用遅れがそのままリスクにつながります。
Chrome利用者の端末だけでなく、業務でブラウザ依存のサービスを使う組織にとっても影響が及びやすい話題です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Chromeを最新の修正版へ速やかに更新する。自動更新の反映状況も確認する。
- Windows、macOS、Linuxなど利用環境ごとに対象バージョンを点検し、更新漏れ端末を洗い出す。
- ブラウザ経由の不審な挙動や端末の異常がないか確認し、必要に応じて検疫・再起動・再配布の手順を用意する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-11645 | 主要CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-11645](https://nvd.nist.gov/vuln/detail/CVE-2026-11645) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Chrome's zero-day Whac-A-Mole continues with fifth exploited bug of the year](https://www.theregister.com/security/2026/06/09/chromes-zero-day-whac-a-mole-continues-with-fifth-exploited-bug-of-the-year/5252689) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Chrome V8 Zero-Day CVE-2026-11645 Exploited in the Wild - Patch Now](https://thehackernews.com/2026/06/chrome-v8-zero-day-cve-2026-11645.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google patches Chrome zero-day exploited in the wild (CVE-2026-11645)](https://www.helpnetsecurity.com/2026/06/09/google-chrome-zero-day-cve-2026-11645/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Update Chrome: Google patches actively exploited vulnerability and 73 others](https://www.malwarebytes.com/blog/bugs/2026/06/update-chrome-google-patches-actively-exploited-vulnerability-and-73-others) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google Releases Patch for Chrome Vulnerability Exploited in the Wild](https://www.infosecurity-magazine.com/news/google-patch-chrome-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google Patches 5th Chrome Zero-Day Exploited in 2026](https://www.securityweek.com/google-patches-5th-chrome-zero-day-exploited-in-2026/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-16161"></a>

### 2. CVE-2026-42271: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>A⁠I</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 42.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

CVE-2026-42271: CISA KEV catalog addition に関する脆弱性情報です。
では英語本文の全文翻訳は行わず、参照リンク、関連する対象、スコア根拠を中心に整理しています。詳細はベンダー公式情報、公的機関情報、NVD等を確認してください。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 自組織で対象製品・関連資産を利用しているか確認する。
- ベンダー公式情報または公的機関情報を優先確認する。
- 対象バージョンか確認する。
- 修正版・緩和策の適用状況を確認する。
- インターネット露出の有無を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-42271 | 主要CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-42271](https://nvd.nist.gov/vuln/detail/CVE-2026-42271) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [LiteLLM vulnerability under active attack, CISA warns (CVE-2026-42271)](https://www.helpnetsecurity.com/2026/06/09/litellm-vulnerability-under-active-attack-cisa-warns-cve-2026-42271/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [LiteLLM Flaw CVE-2026-42271 Exploited in the Wild, Chains to Unauthenticated RCE](https://thehackernews.com/2026/06/litellm-flaw-cve-2026-42271-exploited.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-15753"></a>

### 3. Cisco customers encounter another SD-WAN zero-day under attack

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

Cisco customers encounter another SD-WAN zero-day under attack に関する脆弱性情報です。
では英語本文の全文翻訳は行わず、参照リンク、関連する対象、スコア根拠を中心に整理しています。詳細はベンダー公式情報、公的機関情報、NVD等を確認してください。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 自組織で対象製品・関連資産を利用しているか確認する。
- ベンダー公式情報または公的機関情報を優先確認する。
- 対象バージョンか確認する。
- 修正版・緩和策の適用状況を確認する。
- インターネット露出の有無を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20245 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20245](https://nvd.nist.gov/vuln/detail/CVE-2026-20245) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco customers encounter another SD-WAN zero-day under attack](https://cyberscoop.com/cisco-sdwan-zero-day-vulnerability-exploited-cve202620245/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Manager CVE-2026-20245 Flaw Actively Exploited – No Patch ](https://thehackernews.com/2026/06/cisco-catalyst-sd-wan-manager-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco SD-WAN 0-day exploited, no patch available (CVE-2026-20245)](https://www.helpnetsecurity.com/2026/06/05/cisco-sd-wan-cve-2026-20245-0-day-exploited/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [CISA、Check Point VPNのゼロデイ悪用バグに3日以内の修正を要求](https://www.bleepingcomputer.com/news/security/cisa-orders-feds-to-patch-check-point-flaw-exploited-by-ransomware-gangs/) | 45.0 | 48.0 | 43.0 |
| [Mythos PreviewはN-day脆弱性を数時間で悪用可能にする](https://www.helpnetsecurity.com/2026/06/09/anthropic-mythos-preview-n-day-exploits-firefox-windows/) | 37.0 | 38.0 | 43.0 |
| [Hades PyPI攻撃：19件のパッケージが改ざんされBun認証情報窃取ツールを自動実行](https://thehackernews.com/2026/06/hades-pypi-attack-19-packages-poisoned.html) | 28.0 | 45.0 | 42.0 |
| [QilinによるNHS侵害で被害拡大、Essex trustが記録盗難を確認](https://www.theregister.com/cyber-crime/2026/06/09/qilin-nhs-breach-tally-grows-as-essex-trust-confirms-stolen-records/5252663) | 28.0 | 30.0 | 42.0 |
| [GitHubがパスワード窃取マルウェアを拡散するMicrosoftのリポジトリを無効化](https://www.bleepingcomputer.com/news/security/github-disables-microsoft-repos-pushing-password-stealing-malware/) | 28.0 | 20.0 | 42.0 |
| [調査におけるAI活動の再構築](https://www.microsoft.com/en-us/security/blog/2026/06/09/reconstructing-ai-activity-investigations/) | 27.0 | 20.0 | 42.0 |
| [XBOWがAnthropicのMythos Previewを攻撃セキュリティ用途でテスト](https://www.bleepingcomputer.com/news/security/xbow-tests-anthropics-mythos-preview-for-offensive-security/) | 27.0 | 20.0 | 42.0 |
| [Rapid7がAnthropicのProject Glasswingにアクセスし、サイバーセキュリティ向け最先端AIを探求](https://www.rapid7.com/blog/post/ai-rapid7-accesses-anthropics-project-glasswing-exploring-frontier-artificial-cybersecurity-intelligence) | 27.0 | 20.0 | 42.0 |
| [サイバー攻撃性能が高すぎるAI「Claude Mythos Preview」は公開済みの脆弱性「N-day」から数時間で攻撃を開発できるため「N-dayからN-hourに常識が変わる」とAnthropicが指摘](https://gigazine.net/news/20260609-anthropics-mythos-exploit/) | 27.0 | 20.0 | 42.0 |
| [ローカルのオープンウェイトモデルのみで動作する自己増殖型AIワームを研究者が構築](https://thehackernews.com/2026/06/researchers-build-self-replicating-ai.html) | 27.0 | 20.0 | 42.0 |
| [ワークスがAI型ERPとサービス事業を強化、SAPのリプレース需要を狙う](https://xtech.nikkei.com/atcl/nxt/column/18/00001/11811/) | 26.0 | 20.0 | 42.0 |
| [東京エレクトロン デバイス、製造向けにエッジAI実装の支援制度を立ち上げ](https://japan.zdnet.com/article/35248672/) | 26.0 | 20.0 | 42.0 |
| [Metaがオフサイトの業務データをフィードとAIのパーソナライズに利用へ](https://thehackernews.com/2026/06/meta-to-use-off-site-business-data-for.html) | 25.0 | 20.0 | 42.0 |
| [Anthropic、Cybersecurityガードレールを備えたMythos-class AI「Claude Fable 5」を発表](https://www.securityweek.com/anthropic-launches-claude-fable-5-mythos-class-ai-with-cybersecurity-guardrails/) | 25.0 | 20.0 | 42.0 |
| [Anthropicの新モデル「Mythos on a leash」](https://cyberscoop.com/anthropic-claude-fable-5-release-mythos-guardrails/) | 25.0 | 20.0 | 42.0 |
| [OpenSSLがAIで発見された高危険度脆弱性を修正](https://www.securityweek.com/openssl-patches-high-severity-vulnerability-found-with-ai/) | 25.0 | 20.0 | 42.0 |
| [AppleのiOS 27、侵害されたパスワードをワンタップで変更するエージェント機能を搭載へ](https://www.theregister.com/personal-tech/2026/06/09/apples-ios-27-goes-all-agentic-on-compromised-passwords/5252957) | 25.0 | 20.0 | 42.0 |
| [AI脅威への備え 第2の柱：パッチ適用と対応の迅速化](https://www.wiz.io/blog/ai-threat-readiness-pillar-2) | 25.0 | 20.0 | 42.0 |
| [Claude Mythos、Nデイ脆弱性を数時間で悪用可能にする迅速なExploit生成](https://www.securityweek.com/claude-mythos-turns-n-days-into-n-hours-with-rapid-exploit-creation/) | 25.0 | 20.0 | 42.0 |
| [AIコーディング導入率は97%に達するも、ガバナンス整備は遅れがち](https://www.infosecurity-magazine.com/news/ai-coding-adoption-governance-lags/) | 25.0 | 20.0 | 42.0 |
| [IT業界、知的財産を狙う中国とAI活用のサイバー犯罪者から脅威増大](https://www.cybersecuritydive.com/news/china-cyberattacks-it-sector-crowdstrike-report/822366/) | 25.0 | 20.0 | 42.0 |
| [Elastic、KubernetesとオブザーバビリティツールにAI駆動のインシデント調査機能を提供](https://www.helpnetsecurity.com/2026/06/09/elastic-observability-agentic-kubernetes-investigation-workflow/) | 25.0 | 20.0 | 42.0 |
| [Filigran、AIエージェントでCTEMを自動化するXTM Oneを発表](https://www.helpnetsecurity.com/2026/06/09/filigran-xtm-one/) | 25.0 | 20.0 | 42.0 |
| [Rockwell Automation、SecureOT SuiteにAI搭載のセキュリティツールを追加](https://www.helpnetsecurity.com/2026/06/09/rockwell-automation-secureot-expansion/) | 25.0 | 20.0 | 42.0 |
| [AI構築アプリを守る暗号学的不可視化を用いた新プラットフォーム](https://www.securityweek.com/new-platform-uses-cryptographic-invisibility-to-protect-ai-built-applications/) | 25.0 | 20.0 | 42.0 |
| [Schneider Electric EcoStruxure Panel Serverの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-160-03) | 25.0 | 20.0 | 42.0 |
| [Schneider Electric Modicon Network Managed Switches の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-160-01) | 25.0 | 20.0 | 42.0 |
| [Frontier AIを見直す前に、すでに機能しているものを測定する](https://www.bitsight.com/blog/frontier-ai-security-measure-what-is-working) | 25.0 | 20.0 | 42.0 |
| [Veeam Backup & ReplicationのRCE脆弱性によりドメインユーザーがリモートコードを実行可能に](https://thehackernews.com/2026/06/veeam-backup-replication-rce-flaw-lets.html) | 24.0 | 46.0 | 50.0 |
| [Veeamの新たな脆弱性でバックアップサーバーがRCE攻撃にさらされる](https://www.bleepingcomputer.com/news/security/new-veeam-vulnerability-exposes-backup-servers-to-rce-attacks/) | 24.0 | 38.0 | 42.0 |
| [phpBBの重大な欠陥により、1回のリクエストで任意のアカウントを乗っ取り可能に](https://www.infosecurity-magazine.com/news/phpbb-authentication-bypass/) | 24.0 | 38.0 | 42.0 |
| [賛助会員向けの情報提供メールで誤送信 - 宮崎県産業振興機構](https://www.security-next.com/185420) | 22.0 | 20.0 | 42.0 |
| [九電子会社が紛失した記憶媒体、暗号化やパスワード保護なしと判明 施錠も徹底されず](https://www.itmedia.co.jp/news/articles/2606/09/news132.html) | 21.0 | 20.0 | 42.0 |
| [企業の口座を狙うボイスフィッシングが巧妙化 日本サイバー犯罪対策センターが注意喚起](https://www.itmedia.co.jp/news/articles/2606/09/news130.html) | 21.0 | 20.0 | 42.0 |
| [三菱UFJ、PPAP廃止計画「以前からあった」 今になって実施の経緯は](https://www.itmedia.co.jp/news/articles/2606/09/news129.html) | 21.0 | 20.0 | 42.0 |
| [九州電力送配電、最大1090万件の顧客情報漏洩か データを保存したSSD紛失](https://xtech.nikkei.com/atcl/nxt/news/24/03260/) | 21.0 | 20.0 | 42.0 |
| [100件超のNPM・PyPIパッケージが新たなShai-Huludサプライチェーン攻撃の標的に](https://www.securityweek.com/over-100-npm-pypi-packages-hit-in-new-shai-hulud-supply-chain-attacks/) | 20.0 | 40.0 | 42.0 |
| [Siemens KACO Blueplanetインバータの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-160-02) | 20.0 | 28.0 | 50.0 |
| [SAP NetWeaverおよびCommerce Cloudの重大な脆弱性修正](https://www.bleepingcomputer.com/news/security/sap-fixes-critical-flaws-in-netweaver-and-commerce-cloud/) | 20.0 | 20.0 | 42.0 |
| [CISAがサイバー脆弱性とリスクの評価方法を転換へ、Andersen氏が語る](https://therecord.media/cisa-to-transform-how-it-assesses-cyber-vulns-risks) | 20.0 | 20.0 | 42.0 |
| [Adobeが123件の脆弱性を修正](https://www.securityweek.com/adobe-patches-123-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [攻撃キットのオープンソース化でMiasmaがGitHubに出現](https://www.theregister.com/cyber-crime/2026/06/09/miasma-supply-chain-attack-toolkit-goes-public-on-github/5253074) | 20.0 | 20.0 | 42.0 |
| [Microsoft、Miasma調査継続の中で一部GitHubリポジトリを復旧し、他はオフライン維持](https://thehackernews.com/2026/06/microsoft-restores-some-github-repos.html) | 20.0 | 20.0 | 42.0 |
| [CISAが連邦政府と民間向けのリスクと脆弱性の優先順位付けを見直し](https://cyberscoop.com/cisa-cyber-risk-prioritization-vulnerability-directive/) | 20.0 | 20.0 | 42.0 |
| [CISOsへの圧力が高まる中、75％の企業が脆弱なコードを導入していることが判明](https://www.infosecurity-magazine.com/news/firms-deploy-vulnerable-code/) | 20.0 | 20.0 | 42.0 |
| [フランス政府のメッセージングプラットフォームがアカウント乗っ取りで侵害される](https://www.helpnetsecurity.com/2026/06/09/tchap-french-government-secure-messaging-platform-breach/) | 20.0 | 20.0 | 42.0 |
| [Metaの顔認識コードがスマートグラスへの新たな懸念を呼ぶ](https://www.malwarebytes.com/blog/privacy/2026/06/metas-face-recognition-code-raises-new-concerns-about-smart-glasses) | 20.0 | 20.0 | 42.0 |
| [ハッカーが女性を装いロシア兵士を偵察するロマンス詐欺](https://therecord.media/hackers-pose-as-women-seeking-romance-russian-military) | 20.0 | 20.0 | 42.0 |
| [詐欺師はMetaを好む、Lloyds Bankによると](https://www.malwarebytes.com/blog/scams/2026/06/scammers-love-meta-according-to-lloyds-bank) | 20.0 | 20.0 | 42.0 |
| [ポスト量子暗号の到来とDNSの対応課題](https://www.akamai.com/blog/security/2026/jun/post-quantum-cryptography-coming-dns-not-ready) | 20.0 | 20.0 | 42.0 |
| [Signal、英政府の端末画像スキャン計画は「私たち全員を危険にさらす」](https://www.theregister.com/security/2026/06/09/signal-uks-child-nude-block-threat-wont-protect-children/5252761) | 20.0 | 20.0 | 42.0 |
| [SAP NetWeaverとCommerceの重大な脆弱性に対する修正パッチを公開](https://www.securityweek.com/sap-patches-critical-netweaver-commerce-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [CISA、2026年大統領杯サイバーセキュリティ競技大会の優勝者を発表](https://www.cisa.gov/news-events/news/cisa-announces-winners-2026-presidents-cup-cybersecurity-competition) | 20.0 | 20.0 | 42.0 |
| [最新ネットワークに潜む見えにくいセキュリティリスク：ツール間の連携作業](https://thehackernews.com/2026/06/the-hidden-security-risk-in-modern.html) | 20.0 | 20.0 | 42.0 |
| [France、アカウント乗っ取り後に政府メッセージングプラットフォームの侵害を調査](https://www.theregister.com/security/2026/06/09/france-probes-compromise-of-gov-messaging-platform-after-account-hijack/5252717) | 20.0 | 20.0 | 42.0 |
| [Apple Intelligenceが弱いパスワードをユーザー介入なしで置き換え可能に](https://www.helpnetsecurity.com/2026/06/09/apple-intelligence-automated-passwords-security-updates/) | 20.0 | 20.0 | 42.0 |
| [フランス政府のメッセージングサービスがアカウント乗っ取り攻撃で侵害される](https://www.bleepingcomputer.com/news/security/french-govt-messaging-service-breached-in-account-hijacking-attack/) | 20.0 | 20.0 | 42.0 |
| [UMass Bostonにおける5万人のユーザー保護：ANY.RUNがインシデント予防を推進する方法](https://any.run/cybersecurity-blog/umass-boston-success-story/) | 20.0 | 20.0 | 42.0 |
| [Apple、保護者がブロック・承認・制限できる範囲を拡大](https://www.helpnetsecurity.com/2026/06/09/apple-child-safety-features-and-parental-controls-update/) | 20.0 | 20.0 | 42.0 |
| [新たなFROST攻撃でWebサイトがSSDのタイミングから開いたサイトやアプリを追跡可能に](https://thehackernews.com/2026/06/new-frost-attack-lets-websites-track.html) | 20.0 | 20.0 | 42.0 |
| [北海道医療センター・北海道がんセンターで、患者の個人情報を含むHDDが外部に流通。廃棄処理業者が破砕せず](https://internet.watch.impress.co.jp/docs/news/2115720.html) | 20.0 | 20.0 | 42.0 |
| [Infosecurity Europe：JLRのCISOがサイバー攻撃後に対面でのパスワードリセットを義務付けた理由](https://www.infosecurity-magazine.com/news/jlr-cyberattack-ciso-inperson/) | 20.0 | 20.0 | 42.0 |
| [WhatsApp、NSO Group関連のスピアフィッシング攻撃を発見](https://www.infosecurity-magazine.com/news/whatsapp-nso-group-spearphishing/) | 20.0 | 20.0 | 42.0 |

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
