# 📡 サイレーダー 2026-06-09 05:00 JST

このレポートは、2026-06-08 17:00 JST〜2026-06-09 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 89
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 55

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Qilin ransomware affiliate exploited Check Point VPN zero-day (CVE-2026-50751)](#topic-15996) | 73.0 | 74.0 | 63.0 | 音声 | 温度感上位枠 |
| 2 | [Cisco Catalyst SD-WAN Manager Authenticated Privilege Escalation Vulnerability](#topic-4945) | 63.0 | 84.0 | 67.0 | 音声 | 温度感上位枠 |
| 3 | [Check Point links VPN zero-day attacks to Qilin ransomware gang](#topic-16031) | 45.0 | 48.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [⚡ Weekly Recap: Instagram Account Hacks, Android Zero-Day, GitHub Worm and More](#topic-16029) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [Gogs patches critical zero-day enabling remote code execution](#topic-16003) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [AI brands as bait: How threat actors are using the AI hype in social engineering](#topic-16006) | 35.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [Don't Fear the Repo: UNK_DeadDrop Phishing Campaign Targets Developers to Steal Cryptocurrency](#topic-16013) | 35.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 8 | [8th June – Threat Intelligence Report](#topic-13941) | 33.0 | 46.0 | 63.0 | GitHub | 音声枠上限によりGitHubのみ |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-15996"></a>

### 1. Qilin ransomware affiliate exploited Check Point VPN zero-day (CVE-2026-50751)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 73.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Check PointのVPN製品において、CVE-2026-50751として追跡される認証回避の脆弱性が公表され、実際に悪用が観測されていると報じられています。
報道では、Qilinランサムウェアの関連アフィリエイトが関与している可能性も示されていますが、現時点では確認できる範囲の情報に基づき注意喚起が必要な状況です。
VPNは社内ネットワークへの入口になりやすく、認証回避が成立すると侵入の前提が崩れるため影響が大きくなります。
ランサムウェア文脈での悪用が示唆されている点から、単なる脆弱性情報ではなく、実運用上の緊急対応が求められる案件です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Check Pointの該当製品と設定条件に自組織が該当するかを確認し、ベンダーの修正版・回避策を優先して適用する。
- VPN経由の不審な認証成功や未承認の接続、異常な管理操作の有無をログで点検する。
- 外部公開されているリモートアクセス経路について、必要最小限の露出に絞り、監視とアラートを強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-50751 | 主要CVE | 1.00 |
| 製品 | Exchange | 言及あり | 0.80 |
| ransomware_group | Qilin | 主題 | 0.80 |
| 製品 | Connect Secure | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-50751](https://nvd.nist.gov/vuln/detail/CVE-2026-50751) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Ransomware crims got a month-long head start on Check Point VPN 0-day that now h](https://www.theregister.com/cyber-crime/2026/06/08/attackers-had-month-long-head-start-on-patched-check-point-vpn-zero-day/5252438) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Check Point VPN Zero-Day Exploited in the Wild (CVE-2026-50751)](https://www.rapid7.com/blog/post/etr-critical-check-point-vpn-zero-day-exploited-in-the-wild-cve-2026-50751) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Check Point VPN Flaw Exploited to Bypass Passwords in IKEv1 Setups](https://thehackernews.com/2026/06/critical-check-point-vpn-flaw-exploited.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Qilin ransomware affiliate exploited Check Point VPN zero-day (CVE-2026-50751)](https://www.helpnetsecurity.com/2026/06/08/check-point-cve-2026-50751-qilin-ransomware/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-4945"></a>

### 2. Cisco Catalyst SD-WAN Manager Authenticated Privilege Escalation Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 63.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 84.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Cisco Catalyst SD-WAN Managerに、認証済みのローカル攻撃者が細工したファイルを使ってroot権限で任意コマンドを実行できる脆弱性があり、Ciscoは修正版を公開しています。
CVE-2026-20182として追跡されており、限定的な悪用やゼロデイ文脈、公開PoCの言及も確認されています。
SD-WANの管理系コンポーネントに影響するため、侵害されると広範なネットワーク制御に波及するおそれがあります。
既に悪用や検証コードの情報があるため、影響環境では早期の対応が重要です。

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

- Ciscoの修正版適用状況を確認し、対象製品・対象バージョンが残っていないか洗い出す。
- SD-WAN Managerへの管理者アクセス権限を見直し、不要な認証済みユーザーや運用アカウントを整理する。
- 管理系操作や不審なファイルアップロード、root相当のコマンド実行痕跡がないかログを点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20182 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20182](https://nvd.nist.gov/vuln/detail/CVE-2026-20182) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Manager Authenticated Privilege Escalation Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-privesc-4uxFrdzx) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Metasploit Wrap Up 05/22/2026](https://www.rapid7.com/blog/post/pt-metasploit-wrap-up-05-22-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco zero-day under ongoing attack by persistent threat group](https://cyberscoop.com/cisco-sd-wan-zero-day-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco patches another actively exploited SD-WAN zero-day (CVE-2026-20182)](https://www.helpnetsecurity.com/2026/05/15/cisco-sd-wan-zero-day-cve-2026-20182/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Patches Another SD-WAN Zero-Day, the Sixth Exploited in 2026](https://www.securityweek.com/cisco-patches-another-sd-wan-zero-day-the-sixth-exploited-in-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds Cisco SD-WAN CVE-2026-20182 to KEV After Admin Access Exploits](https://thehackernews.com/2026/05/cisa-adds-cisco-sd-wan-cve-2026-20182.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of new critical SD-WAN flaw exploited in zero-day attacks](https://www.bleepingcomputer.com/news/security/cisco-warns-of-new-critical-sd-wan-flaw-exploited-in-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 中。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。

---

<a id="topic-16031"></a>

### 3. Check Point links VPN zero-day attacks to Qilin ransomware gang

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Check Pointは、Remote Access VPNおよびMobile Accessの環境に影響する重大な脆弱性を修正するセキュリティ更新を公開し、この欠陥がゼロデイ攻撃で悪用されていたとしています。
公開情報では、この攻撃がランサムウェア集団Qilinと結び付けられていますが、詳細な攻撃経路や被害範囲は材料内では限定的です。
VPN製品は社内ネットワークへの入口になりやすく、ゼロデイ悪用が確認されると影響が広がりやすい点が注目されます。
ランサムウェア集団との関連が示されているため、認証基盤やリモート接続環境の緊急点検が重要になります。

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

- Check Pointの更新適用状況を確認し、該当するRemote Access VPN／Mobile Access環境を優先的に点検する。
- 外部公開されているVPN装置の管理インターフェースやアクセス制御を見直し、不要な露出を減らす。
- 認証ログやVPN接続ログを確認し、不審なアクセスや設定変更の兆候がないか監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ransomware_group | Qilin | 主題 | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Check Point links VPN zero-day attacks to Qilin ransomware gang](https://www.bleepingcomputer.com/news/security/check-point-links-vpn-zero-day-attacks-to-qilin-ransomware-gang/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-16029"></a>

### 4. ⚡ Weekly Recap: Instagram Account Hacks, Android Zero-Day, GitHub Worm and More

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>A⁠n⁠d⁠r⁠o⁠i⁠d</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

先週は、Instagramアカウントの不正アクセス、Androidのゼロデイ、GitHub上で広がるワームなど、複数のセキュリティ事案がまとめて取り上げられました。
加えて、悪意あるパッケージやAI関連の不具合、長期間にわたるメール監視のような動きも示されており、攻撃者が複数の手口を使い分けている状況がうかがえます。
個別の脆弱性だけでなく、実際の悪用や侵害の文脈が含まれているため、端末・アカウント・開発基盤のいずれも影響を受けうる点が重要です。
特に、基本的な運用ミスや認証情報管理の弱さが被害拡大につながる可能性があります。

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
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- アカウント保護を見直し、強固な認証と不審なログイン検知を優先する。
- Android端末と開発環境の更新状況を確認し、既知の脆弱性への対応を急ぐ。
- 依存パッケージ、ボット、トークンなどの秘密情報管理を点検し、漏えい前提の監視を強化する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [⚡ Weekly Recap: Instagram Account Hacks, Android Zero-Day, GitHub Worm and More](https://thehackernews.com/2026/06/weekly-recap-instagram-account-hacks.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・低信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-16003"></a>

### 5. Gogs patches critical zero-day enabling remote code execution

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Gogsで、リモートコード実行につながる重大なゼロデイ脆弱性が修正されたとされています。
インターネット公開されたインスタンスが影響を受ける可能性があり、条件によってはリポジトリへの不正アクセスにつながるおそれがあります。
ソースコード管理基盤が影響を受けると、機密情報や開発資産の漏えい、改ざん、横展開の起点になり得ます。
ゼロデイとして扱われているため、公開運用中の環境では優先的な確認と更新が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Gogsを外部公開している環境は、修正版の適用状況を早急に確認する。
- 管理者権限やリポジトリ権限の見直し、不要な公開範囲の縮小を検討する。
- 不審なアクセスやリポジトリ操作の痕跡がないか、ログを点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Gogs patches critical zero-day enabling remote code execution](https://www.bleepingcomputer.com/news/security/gogs-patches-critical-zero-day-enabling-remote-code-execution/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-16006"></a>

### 6. AI brands as bait: How threat actors are using the AI hype in social engineering

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoft Security Blogは、脅威アクターがAIそのものへの関心や話題性を、ソーシャルエンジニアリングの誘引として利用していると伝えています。
AIを悪用した攻撃の高度化だけでなく、AIブランドや関連用語が「信頼できそう」に見える材料として使われる点が示唆されています。
AI関連サービスや製品を扱う組織では、正規の案内やサポートを装う偽情報と見分けにくくなるため、注意が必要です。
技術的な脆弱性だけでなく、話題性を利用した騙しの手口が増えると、利用者教育と確認手順の重要性が高まります。

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

- AI関連の名義や案内を受け取った際は、送信元・ドメイン・依頼内容を通常以上に厳しく確認する。
- 社内向けには、AIツール導入やサポートを装う連絡に対する確認フローを明確にしておく。
- メール、チャット、SNS経由の問い合わせで、認証情報やアクセス許可を求める場合は特に警戒する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [AI brands as bait: How threat actors are using the AI hype in social engineering](https://www.microsoft.com/en-us/security/blog/2026/06/08/ai-brands-as-bait-how-threat-actors-are-using-the-ai-hype-in-social-engineering/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・低信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-16013"></a>

### 7. Don't Fear the Repo: UNK_DeadDrop Phishing Campaign Targets Developers to Steal Cryptocurrency

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>I⁠o⁠C</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>A⁠I</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Proofpointは、開発者向けの採用案内やコードレビュー依頼を装ったフィッシングで、暗号資産関連の認証情報やウォレット情報を狙う攻撃キャンペーンを確認したと報告しました。
攻撃では、GitHub上の不正なリポジトリやVS Code系の仕組みが悪用された可能性があり、macOS、Linux、Windowsをまたいで動作するマルウェアが使われたとされています。
開発者の通常業務に見える流れを利用するため、警戒されにくく、組織のソースコード管理やウォレット保護に直接影響し得ます。
暗号資産や開発環境に関わる認証情報の流出は、金銭被害や二次侵害につながるおそれがあります。

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

- 採用・レビュー依頼を装うメールや、外部リポジトリの取り扱いに対する確認手順を見直す。
- IDEでのフォルダ自動実行や拡張機能の導入が許可されている範囲を点検し、不要な自動実行を抑える。
- 開発端末でウォレット拡張、ブラウザ資格情報、Keychain/Keyring などへのアクセスを最小化し、異常な拡張機能やプロセスを監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Don't Fear the Repo: UNK_DeadDrop Phishing Campaign Targets Developers to Steal ](https://www.proofpoint.com/us/blog/threat-insight/dont-fear-repo-unkdeaddrop-phishing-campaign-targets-developers-steal) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-13941"></a>

### 1. 8th June – Threat Intelligence Report

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠n⁠d⁠r⁠o⁠i⁠d</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

8th June – Threat Intelligence Report に関する脆弱性情報です。
では英語本文の全文翻訳は行わず、参照リンク、関連する対象、スコア根拠を中心に整理しています。詳細はベンダー公式情報、公的機関情報、NVD等を確認してください。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
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

- 自組織で対象製品・関連資産を利用しているか確認する。
- ベンダー公式情報または公的機関情報を優先確認する。
- 対象バージョンか確認する。
- 修正版・緩和策の適用状況を確認する。
- インターネット露出の有無を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-48595 | 主要CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-48595](https://nvd.nist.gov/vuln/detail/CVE-2025-48595) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [8th June – Threat Intelligence Report](https://research.checkpoint.com/2026/8th-june-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google June 2026 Android Update Patches 124 Flaws, One Actively Exploited](https://thehackernews.com/2026/06/google-june-2026-android-update-patches.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Android Update Patches Exploited Zero-Day, 123 Other Vulnerabilities](https://www.securityweek.com/android-update-patches-exploited-zero-day-123-other-vulnerabilities/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google fixes actively exploited Android vulnerability (CVE-2025-48595)](https://www.helpnetsecurity.com/2026/06/02/android-vulnerability-exploited-cve-2025-48595/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 反応あり・低信頼。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Everest Formsの脆弱性を悪用したWordPressサイトへの侵入](https://www.securityweek.com/everest-forms-vulnerability-exploited-to-hack-wordpress-sites/) | 37.0 | 38.0 | 43.0 |
| [AIフィッシングがSOCsを圧迫するアラート急増：Tier 1の負荷をどう減らすか](https://thehackernews.com/2026/06/ai-phishing-is-crushing-socs-with-alert.html) | 33.0 | 20.0 | 42.0 |
| [TeamPCPのサプライチェーンキャンペーン：2026-06-07時点の活動状況](https://isc.sans.edu/diary/rss/33060) | 30.0 | 20.0 | 42.0 |
| [ランサムウェア攻撃でイリノイ州の高校が早めの夏休みに](https://www.theregister.com/cyber-crime/2026/06/08/ransomware-attack-shuts-illinois-high-school-until-wednesday/5252322) | 28.0 | 30.0 | 42.0 |
| [Silent Ransom Groupが攻撃でDNS Fast Fluxを使用](https://www.securityweek.com/silent-ransom-group-uses-dns-fast-flux-in-attacks/) | 28.0 | 30.0 | 42.0 |
| [WhatsAppが新たなNSOスパイウェアのフィッシング攻撃を阻止した件](https://www.bleepingcomputer.com/news/security/whatsapp-says-it-disrupted-new-nso-spyware-phishing-attacks/) | 28.0 | 20.0 | 42.0 |
| [Minecraft ModからMalware-as-a-Serviceへ：Weedhackエコシステムの実態](https://blog.polyswarm.io/from-minecraft-mods-to-malware-as-a-service-inside-the-weedhack-ecosystem) | 28.0 | 20.0 | 42.0 |
| [Meta、NSO Groupがスパイウェア差し止め命令に違反したとして裁判所侮辱申立てを提出](https://cyberscoop.com/meta-contempt-complaint-nso-group-spyware/) | 28.0 | 20.0 | 42.0 |
| [PyPIを狙う「Hades」キャンペーン、新たな「Shai-Hulud」の手口を採用](https://www.darkreading.com/application-security/hades-campaign-pypi-shai-hulud) | 28.0 | 20.0 | 42.0 |
| [Cloudflareの脅威インジケーターをリアルタイムWAFルールに変換する方法](https://blog.cloudflare.com/realtime-threat-intel-waf-rules/) | 28.0 | 20.0 | 42.0 |
| [海賊版PCゲームがパスワード窃取マルウェアを配布](https://www.malwarebytes.com/blog/threat-intel/2026/06/pirated-pc-games-are-delivering-password-stealing-malware) | 28.0 | 20.0 | 42.0 |
| [VerdantBambooがLinuxアプライアンスにBRICKSTORMのBSD版を展開](https://thehackernews.com/2026/06/verdantbamboo-deploys-bsd-variant-of.html) | 28.0 | 20.0 | 42.0 |
| [Appleの画像生成AIが大幅強化されて高品質生成や画像編集が可能に](https://gigazine.net/news/20260609-apple-wwdc26-image-generation/) | 27.0 | 20.0 | 42.0 |
| [SiriとApple Intelligenceが統合した「Siri AI」発表、SiriやSafariやパスワードでGoogle Geminiベースの新生Apple Intelligenceを駆使できる](https://gigazine.net/news/20260609-apple-wwdc26-apple-intelligence/) | 27.0 | 20.0 | 42.0 |
| [「AIが私のソフトウェアエンジニアとしてのキャリアを侵食しておりどうすればいいか分からない」という投稿が大きな反響を呼ぶ](https://gigazine.net/news/20260608-llms-eroding-career/) | 27.0 | 20.0 | 42.0 |
| [Siri、ようやく全面刷新へ Appleが「Siri AI」発表 会話能力向上、今風のAIアシスタントに](https://www.itmedia.co.jp/news/articles/2606/09/news063.html) | 26.0 | 20.0 | 42.0 |
| [パナソニックエナジー、28年度に売上高2兆円目指す AIデータセンター向けに主力転換](https://www.itmedia.co.jp/news/articles/2606/08/news131.html) | 26.0 | 20.0 | 42.0 |
| [Microsoft Entra Agent IDにおける疑わしいAIワークフローの調査：Assistive agents](https://redcanary.com/blog/threat-detection/entra-id-ai-workflows-assistive-agents/) | 25.0 | 20.0 | 42.0 |
| [FBIが警告、AI悪用詐欺で米国人が約9億ドルの被害](https://www.malwarebytes.com/blog/scams/2026/06/americans-lost-nearly-900-million-to-ai-powered-scams-fbi-says) | 25.0 | 20.0 | 42.0 |
| [企業はAIによるなりすまし攻撃の加速に備えられていない](https://www.cybersecuritydive.com/news/ai-executive-impersonation-outtake-survey/822235/) | 25.0 | 20.0 | 42.0 |
| [Wazuh Cloudでセキュリティ運用の複雑さを軽減する方法](https://www.bleepingcomputer.com/news/security/reducing-security-operations-complexity-with-wazuh-cloud/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、ChatGPTのアカウントセキュリティ制御を発表](https://www.infosecurity-magazine.com/news/chatgpt-lockdown-mode-active/) | 25.0 | 20.0 | 42.0 |
| [ハッカーがMetaのAIサポートシステムを悪用し2万件超のInstagramアカウントを乗っ取り](https://www.helpnetsecurity.com/2026/06/08/instagram-ai-support-vulnerability-account-takeovers/) | 25.0 | 20.0 | 42.0 |
| [New Relic、AI支援ソフトウェア開発への可観測性を拡大](https://www.helpnetsecurity.com/2026/06/08/new-relic-ai-coding-observability/) | 25.0 | 20.0 | 42.0 |
| [Infosecurity EuropeでOWASP研究者が警告、プロンプトインジェクションは未解決のまま](https://www.infosecurity-magazine.com/news/infosec-europe-prompt-injection/) | 25.0 | 20.0 | 42.0 |
| [AIセキュリティ競争に必要なのは過度な規制ではなく説明責任](https://cyberscoop.com/ai-security-regulation-accountability-op-ed/) | 25.0 | 20.0 | 42.0 |
| [OpenAIがChatGPTのアカウントセキュリティ機能を展開開始](https://www.securityweek.com/openai-rolling-out-chatgpt-account-security-controls/) | 25.0 | 20.0 | 42.0 |
| [サイバー攻撃でシステム障害、原因や影響を調査 - 建材補修会社](https://www.security-next.com/185269) | 22.0 | 20.0 | 42.0 |
| [複数取引サイトとの確認メールで誤送信 - 北陸電力](https://www.security-next.com/185512) | 22.0 | 20.0 | 42.0 |
| [小学校で児童情報含む書類を紛失、確認作業中に - 名古屋市](https://www.security-next.com/185189) | 22.0 | 20.0 | 42.0 |
| [サイバー攻撃に8割の企業が「丸裸」 穴だらけの環境をどう守る？](https://atmarkit.itmedia.co.jp/ait/articles/2606/07/news010.html) | 21.0 | 20.0 | 42.0 |
| [GitHubが70件超のMicrosoftリポジトリを削除、疑わしいワーム感染でCI/CDパイプラインに障害](https://www.theregister.com/security/2026/06/08/github-nukes-70-microsoft-repos-amid-suspected-worm-attack/5252169) | 20.0 | 45.0 | 42.0 |
| [イランが停戦に署名してもハッカーは止まらなかった](https://www.darkreading.com/cyberattacks-data-breaches/iran-signed-ceasefire-hackers) | 20.0 | 20.0 | 42.0 |
| [Meta、裁判所命令後もNSO GroupがWhatsAppユーザーを標的にしていると主張](https://www.helpnetsecurity.com/2026/06/08/meta-whatsapp-nso-group-phishing-campaign/) | 20.0 | 20.0 | 42.0 |
| [Security Raises 3700万ドルを調達、自律型オフェンシブ・セキュリティ・プラットフォームを展開](https://www.securityweek.com/a-security-raises-37-million-for-autonomous-offensive-security-platform/) | 20.0 | 20.0 | 42.0 |
| [MetaがNSO Groupの新たなWhatsAppフィッシング攻撃を阻止、侮辱命令を申請](https://thehackernews.com/2026/06/meta-blocks-nso-groups-new-whatsapp.html) | 20.0 | 20.0 | 42.0 |
| [WhatsApp、NSOが裁判所命令に違反して標的型フィッシング攻撃でユーザーを標的にしたと発表](https://therecord.media/whatsapp-says-nso-targeted-users-with-attacks-against-court-order) | 20.0 | 20.0 | 42.0 |
| [Microsoft Defender for EndpointのEDR更新配信方法がWindowsで変更される](https://www.helpnetsecurity.com/2026/06/08/microsoft-defender-for-endpoint-edr-updates/) | 20.0 | 20.0 | 42.0 |
| [世界的混乱の中で高まる脅威](https://www.security.com/expert-perspectives/threats-rise-global-unrest) | 20.0 | 20.0 | 42.0 |
| [認証なしで攻撃者がroot権限を取得できるUniFi OSの重大なバグ](https://www.bleepingcomputer.com/news/security/critical-unifi-os-bug-lets-hackers-gain-root-without-authentication/) | 20.0 | 20.0 | 42.0 |
| [サイバー保険の契約者が引受審査と保険金請求で厳しい審査に直面](https://www.cybersecuritydive.com/news/cyber-insurance-policyholders-facing-heavier-scrutiny-underwriting-claims/822089/) | 20.0 | 20.0 | 42.0 |
| [全員がVibe Codingをしているのに、セキュリティチームには誰も伝えていなかった](https://www.securityweek.com/everybody-is-vibe-coding-but-nobody-told-the-security-team/) | 20.0 | 20.0 | 42.0 |
| [北朝鮮のハッカーが偽のコーディング課題を使って暗号資産を窃取](https://www.infosecurity-magazine.com/news/north-korean-hackers-developers/) | 20.0 | 20.0 | 42.0 |
| [WhatsApp、NSOのハッキング禁止命令違反を受けてスパイウェア企業を摘発](https://www.securityweek.com/whatsapp-catches-spyware-firm-nso-defying-no-hacking-court-order/) | 20.0 | 20.0 | 42.0 |
| [サイバーセキュリティM&A総括：2026年5月に発表された26件の取引](https://www.securityweek.com/cybersecurity-ma-roundup-26-deals-announced-in-may-2026/) | 20.0 | 20.0 | 42.0 |
| [Metaが再びNSO Groupを標的に、WhatsAppへの攻撃疑惑で追及](https://www.theregister.com/security/2026/06/08/nso-group-back-in-metas-crosshairs-after-alleged-whatsapp-targeting/5252105) | 20.0 | 20.0 | 42.0 |
| [RidgeBot 7.0によるActive Directory攻撃シミュレーションの自動化によるセキュリティ検証](https://www.helpnetsecurity.com/2026/06/08/ridge-security-ridgebot-7-0/) | 20.0 | 20.0 | 42.0 |
| [Lansing Community Collegeのデータ漏えいで17万4000人に影響](https://www.securityweek.com/174000-impacted-by-lansing-community-college-data-breach/) | 20.0 | 20.0 | 42.0 |
| [ConnectSecure Patch 360によるMSP向けパッチのテストと展開の管理](https://www.helpnetsecurity.com/2026/06/08/connectsecure-patch-360/) | 20.0 | 20.0 | 42.0 |
| [Oxford University、就職支援プラットフォームへの不正アクセス後にデータ漏えいを公表](https://www.bleepingcomputer.com/news/security/oxford-university-discloses-data-breach-after-careerconnect-platform-hack/) | 20.0 | 20.0 | 42.0 |
| [九州電力送配電、最大1090万件の個人情報漏えいのおそれ、バックアップ媒体が所在不明に](https://internet.watch.impress.co.jp/docs/news/2115399.html) | 20.0 | 20.0 | 42.0 |
| [Samsung、One UI 9ベータでGalaxyスマートフォンのセキュリティを強化](https://www.helpnetsecurity.com/2026/06/08/samsung-lockdown-mode-power-menu/) | 20.0 | 20.0 | 42.0 |
| [オープンソースコミュニティの3分の2がCyber Resilience Actを認識していない](https://www.infosecurity-magazine.com/news/open-source-unaware-cyber/) | 20.0 | 20.0 | 42.0 |
| [新たなリスク方程式：なぜエンドポイントセキュリティは経営上の必須課題なのか](https://www.cybersecuritydive.com/spons/the-new-risk-equation-why-endpoint-security-is-a-financial-imperative/821449/) | 20.0 | 20.0 | 42.0 |
| [Infosecurity Europe：DSITが数千の英国組織をサイバー脆弱性から守る方法](https://www.infosecurity-magazine.com/news/infosecurity-europe-dsit-cyber/) | 20.0 | 20.0 | 42.0 |

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
