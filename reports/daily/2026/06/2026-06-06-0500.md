# 📡 サイレーダー 2026-06-06 05:00 JST

このレポートは、2026-06-05 17:00 JST〜2026-06-06 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 71
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 39

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cisco Catalyst SD-WAN Manager Authenticated Privilege Escalation Vulnerability](#topic-4945) | 63.0 | 84.0 | 67.0 | 音声 | 温度感上位枠 |
| 2 | [Threat Brief: Active Exploitation of PAN-OS CVE-2026-0257](#topic-4247) | 48.0 | 67.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [Cisco warns zero-day flaw in SD-WAN is being exploited](#topic-15697) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Cisco SD-WAN 0-day exploited, no patch available (CVE-2026-20245)](#topic-15753) | 39.0 | 58.0 | 51.0 | 音声 | 温度感上位枠 |
| 5 | [CVE-2026-28318: CISA KEV catalog addition](#topic-15718) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 6 | [In Other News: Anthropic Maps AI Threats, Unpatched Comodo Flaw, Palantir Chief Eyed for CISA](#topic-15710) | 33.0 | 30.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [Adaptive, Agentic AI Worms Loom as Next Enterprise Threat](#topic-15702) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-4945"></a>

### 1. Cisco Catalyst SD-WAN Manager Authenticated Privilege Escalation Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 63.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 84.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Cisco Catalyst SD-WAN Manager／Controllerに関する脆弱性CVE-2026-20182が報告され、Ciscoは修正アップデートを公開しています。
公開情報では、限定的な標的型攻撃での悪用や公開PoCの言及があり、認証回避や権限昇格につながる可能性があるとされています。
SD-WANの管理・制御面に関わるため、影響を受けるとネットワーク全体の運用に波及するおそれがあります。
さらに、既に悪用文脈や検証コードの言及があることから、早期対応の優先度が高い事案です。

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

- 影響を受けるCisco Catalyst SD-WAN Controller／Managerのバージョンを確認し、ベンダーの修正済み版へ速やかに更新する。
- 管理プレーンへの到達経路を見直し、不要な公開やアクセス許可を絞る。
- 異常な管理操作や想定外のファイル操作、権限変更の痕跡がないか監査ログを確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20182 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20245 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-41940 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2023-7101 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-31431 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20133 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20128 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20122 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20127 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-24479 | 主要CVE | 1.00 |

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

<a id="topic-4247"></a>

### 2. Threat Brief: Active Exploitation of PAN-OS CVE-2026-0257

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 48.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 67.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Palo Alto NetworksのPAN-OS/Prisma Accessに影響するCVE-2026-0257について、公開後まもなく実際の悪用が観測されたと報告されています。
条件を満たす構成では、GlobalProtectの認証をすり抜けてVPN接続が成立する可能性があるとされ、影響範囲のある環境では緊急の対応が推奨されています。
境界装置の認証バイパスは、外部から社内ネットワークへの侵入起点になり得るため注目されています。
現時点で横展開の兆候は確認されていない一方、認証突破そのもののリスクが高く、優先度の高い対処対象です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 9 sources。
- 実悪用・ゼロデイ文脈。
- 技術詳細・再現情報あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 技術詳細により影響確認が進みやすい。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 技術詳細・悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 技術詳細、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- PAN-OS/Prisma Accessで該当バージョンかつGlobalProtectの認証オーバーライド機能を使っているかを確認する。
- ベンダー案内に従い、修正版への更新を優先し、必要に応じて認証オーバーライド機能の無効化や専用証明書の再設定を検討する。
- GlobalProtectの認証ログやVPN接続履歴を点検し、不審なCookie認証や見慣れない送信元からの試行がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-0257 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |
| ベンダー | Palo Alto | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-0257](https://nvd.nist.gov/vuln/detail/CVE-2026-0257) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: Active Exploitation of PAN-OS CVE-2026-0257](https://unit42.paloaltonetworks.com/active-exploitation-of-pan-os-cve-2026-0257/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0257 PAN-OS: GlobalProtect Authentication Bypass Vulnerabilities (Sever](https://security.paloaltonetworks.com/CVE-2026-0257) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers are exploiting Palo Alto Networks defect that initially flew under the](https://cyberscoop.com/palo-alto-networks-cve-2026-0257-exploited-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Recent Palo Alto Networks Vulnerability Exploited for Weeks](https://www.securityweek.com/recent-palo-alto-networks-vulnerability-exploited-for-weeks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers are exploiting Palo Alto GlobalProtect VPN authentication bypass (CVE-20](https://www.helpnetsecurity.com/2026/06/01/hackers-are-exploiting-palo-alto-globalprotect-vpn-authentication-bypass-cve-2026-0257/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Palo Alto GlobalProtect VPN auth bypass flaw now exploited in attacks](https://www.bleepingcomputer.com/news/security/palo-alto-globalprotect-vpn-auth-bypass-flaw-now-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PAN-OS GlobalProtect Authentication Bypass (CVE-2026-0257) Under Active Exploita](https://thehackernews.com/2026/05/pan-os-globalprotect-authentication.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・低信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 技術詳細・悪用観測あり。

---

<a id="topic-15697"></a>

### 3. Cisco warns zero-day flaw in SD-WAN is being exploited

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Ciscoは、SD-WAN製品に存在するゼロデイ脆弱性について、すでに悪用が確認されていると注意喚起しました。
現時点では修正パッチが提供されていないとされ、影響を受ける環境ではコマンドインジェクションにつながる可能性があるとされています。
ゼロデイで実際の悪用が示されているため、公開直後から優先度の高い対応が必要になりやすい事案です。
ネットワーク機器は影響範囲が広く、侵害されると組織内への横展開や設定改ざんにつながるおそれがあります。

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

- Ciscoの告知と更新情報を確認し、影響製品・バージョンの該当有無を点検する。
- 暫定的に露出を減らせる設定やアクセス制御がないか確認し、不要な外部公開を避ける。
- 関連機器のログや管理操作履歴を確認し、不審なコマンド実行や設定変更の兆候を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Cisco warns zero-day flaw in SD-WAN is being exploited](https://www.cybersecuritydive.com/news/cisco-zero-day-flaw-sd-wan-exploited/822138/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・低信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-15753"></a>

### 4. Cisco SD-WAN 0-day exploited, no patch available (CVE-2026-20245)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

Cisco Catalyst SD-WAN Managerにおいて、権限昇格につながる脆弱性CVE-2026-20245が悪用されていると報じられています。
現時点ではCiscoから修正パッチは公開されておらず、同社は限定的な悪用事例を把握しているとしています。
SD-WAN管理基盤はネットワーク運用の中枢に当たるため、侵害されると広範な影響につながる可能性があります。
既知の脆弱性や有効な資格情報を起点に権限が上がる構図のため、周辺の関連脆弱性も含めた確認が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Ciscoの案内を確認し、該当製品の影響範囲と緩和策の有無を早急に点検する。
- 管理者権限やnetadmin権限の利用状況を見直し、不要なアカウントや認証情報のリスクを確認する。
- CVE-2026-20182、CVE-2026-20127を含む関連脆弱性の適用状況もあわせて棚卸しする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20245 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20182 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20127 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20245](https://nvd.nist.gov/vuln/detail/CVE-2026-20245) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco SD-WAN 0-day exploited, no patch available (CVE-2026-20245)](https://www.helpnetsecurity.com/2026/06/05/cisco-sd-wan-cve-2026-20245-0-day-exploited/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-15718"></a>

### 5. CVE-2026-28318: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

CISAは、実際の悪用が確認されたとして、SolarWinds Serv-Uに関するCVE-2026-28318をKnown Exploited Vulnerabilities（KEV）Catalogに追加しました。
対象の脆弱性は「Uncontrolled Resource Consumption（制御されていないリソース消費）」とされており、公開情報上は活発な悪用の証拠に基づく追加です。
KEV Catalogへの追加は、脆弱性がすでに攻撃対象になっている可能性が高いことを示します。運用上は、影響有無の確認と優先度の高い対応が必要になりやすい点が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- SolarWinds Serv-Uの利用有無を確認し、該当バージョンや影響範囲を早急に棚卸しする。
- 脆弱性管理の優先順位を見直し、修正適用や緩和策の実施を前倒しで検討する。
- 関連製品のログや監視を確認し、異常な負荷や不審な挙動がないかを点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-28318 | 主要CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-28318](https://nvd.nist.gov/vuln/detail/CVE-2026-28318) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/06/05/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・低信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-15710"></a>

### 6. In Other News: Anthropic Maps AI Threats, Unpatched Comodo Flaw, Palantir Chief Eyed for CISA

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

AnthropicがAIに関する脅威を整理・可視化する取り組みが取り上げられました。
あわせて、未修正のComodo関連の脆弱性や、ランサムウェア分析など複数のセキュリティ話題が並んでいます。
AIの安全性評価は、生成AIの導入拡大とともに実務上の関心が高まっています。加えて、未修正脆弱性やランサムウェア動向は、日々の防御優先度の見直しにつながります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI機能の利用範囲とリスク評価を定期的に見直す。
- 未修正ソフトウェアや関連製品の更新状況を確認し、適用漏れを減らす。
- ランサムウェア関連の最新動向を踏まえ、検知・バックアップ・復旧手順を再点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ai_model_or_project | Anthropic | 主題 | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [In Other News: Anthropic Maps AI Threats, Unpatched Comodo Flaw, Palantir Chief ](https://www.securityweek.com/in-other-news-anthropic-maps-ai-threats-unpatched-comodo-flaw-palantir-chief-eyed-for-cisa/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・低信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-15702"></a>

### 7. Adaptive, Agentic AI Worms Loom as Next Enterprise Threat

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者らが、環境に適応しながら脆弱性を探す「AIワーム」が次の企業向け脅威になり得ると警鐘を鳴らしています。
現時点では将来のリスクに関する見立てであり、具体的な発生事例が確認されたという内容ではありません。
AIが自律的に振る舞う前提が強まるほど、従来のマルウェア対策だけでは捉えにくい挙動が増える可能性があります。
生成AIの業務利用が広がる中で、セキュリティ運用やガバナンスの見直しにつながるため注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIを組み込んだ業務フローやエージェント連携の権限設定を点検し、不要な権限を最小化する。
- 外部サービス連携や自動実行の監視を強化し、想定外の挙動を検知できる運用にする。
- AI関連のリスクを既存の脅威モデリングに含め、従来型マルウェア対策とのギャップを洗い出す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Adaptive, Agentic AI Worms Loom as Next Enterprise Threat](https://www.darkreading.com/cyber-risk/adaptive-agentic-ai-worms-enterprise-cyber-threat) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 未確認。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

今回はGitHubのみ掲載の注目トピックはありません。

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [米国法律事務所を標的とした継続的な攻撃キャンペーン](https://cloud.google.com/blog/topics/threat-intelligence/targeted-campaign-us-law-firms/) | 36.0 | 30.0 | 48.0 |
| [流出した未来：小児医療データの長期的な犯罪価値](https://blog.polyswarm.io/stolen-futures-the-long-term-criminal-value-of-pediatric-healthcare-data) | 36.0 | 30.0 | 42.0 |
| [HackersがCriticalなEverest Forms Pro WordPressプラグインの脆弱性を悪用しサイトを乗っ取り](https://thehackernews.com/2026/06/hackers-exploit-critical-everest-forms.html) | 32.0 | 46.0 | 50.0 |
| [ANY.RUNがG2 Summer 2026 Awardsでトップベンダーに選出される](https://any.run/cybersecurity-blog/g2-summer-awards-2026/) | 30.0 | 20.0 | 42.0 |
| [IronWormと新たなMiasmaワーム亜種がnpmを標的としたサプライチェーン攻撃](https://thehackernews.com/2026/06/ironworm-and-new-miasma-worm-variant.html) | 28.0 | 40.0 | 42.0 |
| [中国のAPTが侵害ネットワークへのアクセス維持に新たなマルウェアを展開](https://www.bleepingcomputer.com/news/security/chinese-apt-deploys-new-malware-to-keep-access-to-hacked-networks/) | 28.0 | 20.0 | 42.0 |
| [AndroidスパイウェアAsinが偽ニュース、PDF、戦況マップアプリを通じてアラビア語ユーザーを標的にする](https://thehackernews.com/2026/06/android-spyware-asin-targets-arabic.html) | 28.0 | 20.0 | 42.0 |
| [攻撃者が一部のDashlaneユーザーアカウントから暗号化されたパスワード保管庫を入手した件](https://www.helpnetsecurity.com/2026/06/05/dashlane-brute-force-attack-vaults-customer-accounts/) | 28.0 | 20.0 | 42.0 |
| [NCSCが組織にサプライチェーンセキュリティ対策の強化を要請](https://www.itpro.com/security/ncsc-urges-organizations-to-shore-up-supply-chain-security-practices) | 28.0 | 20.0 | 42.0 |
| [エージェント時代のCI/CDを守る：Claude Code GitHub Action事例](https://www.microsoft.com/en-us/security/blog/2026/06/05/securing-ci-cd-in-agentic-world-claude-code-github-action-case/) | 27.0 | 20.0 | 42.0 |
| [米下院の新AI法案、フロンティアモデル監督とオープンソース向けセキュリティ助成金を含む](https://www.cybersecuritydive.com/news/house-ai-bill-regulation-cisa-nist-open-source/822131/) | 25.0 | 20.0 | 42.0 |
| [EUが米中サプライヤーへの依存を減らすための技術主権パッケージを発表](https://therecord.media/eu-unveils-tech-sovereignty-package-cut-reliance-us-china) | 25.0 | 20.0 | 42.0 |
| [Trump政権のAI命令、フロンティアモデルの自発的テストを要請](https://www.darkreading.com/cybersecurity-operations/trump-ai-order-seeks-voluntary-frontier-model-testing) | 25.0 | 20.0 | 42.0 |
| [Infosecurity Europeに学ぶLloydsのエージェント型AIセキュリティ実践ガイド](https://www.infosecurity-magazine.com/news/lloyds-agentic-ai-security-playbook/) | 25.0 | 20.0 | 42.0 |
| [SOCの10%しかAIから優れた価値を得ていないと回答、次の波に求められるものとは](https://thehackernews.com/2026/06/only-10-of-socs-say-theyre-getting.html) | 25.0 | 20.0 | 42.0 |
| [Infosecurity EuropeでOWASPがAgentic AIセキュリティ成熟度フレームワークを発表](https://www.infosecurity-magazine.com/news/owasp-agentic-ai-security-maturity/) | 25.0 | 20.0 | 42.0 |
| [新たなTrump AIサイバーセキュリティ大統領令に対する業界の反応と意見](https://www.securityweek.com/industry-reactions-to-new-trump-ai-cybersecurity-executive-order-feedback-friday/) | 25.0 | 20.0 | 42.0 |
| [Infosecurity Europe：AIコーディングツールにはエージェント型開発時代に向けた組み込みセキュリティが必要](https://www.infosecurity-magazine.com/news/ai-coding-tools-security-agentic/) | 25.0 | 20.0 | 42.0 |
| [AIは脅威か、ツールか、あるいはその両方か](https://www.malwarebytes.com/blog/ai/2026/06/ai-threat-tool-or-both) | 25.0 | 20.0 | 42.0 |
| [AIが低スキルのハッカーによる高度なサイバー攻撃を支援している](https://www.helpnetsecurity.com/2026/06/05/anthropic-ai-cyber-activity-analysis/) | 25.0 | 20.0 | 42.0 |
| [送信メールの添付ファイル保管サーバが侵害 - 石川のSIer](https://www.security-next.com/184676) | 22.0 | 20.0 | 42.0 |
| [サーバに不正アクセス、侵害経路や影響を調査 - ソディック](https://www.security-next.com/185106) | 22.0 | 20.0 | 42.0 |
| [卒業生宛の「進路だより」でメール誤送信 - 新潟県](https://www.security-next.com/185455) | 22.0 | 20.0 | 42.0 |
| [家庭用PCでも数秒でサーバを“落とせる”、HTTP/2の脆弱性をCodexが発見 さくらインターネットも対策](https://www.itmedia.co.jp/news/articles/2606/05/news119.html) | 21.0 | 20.0 | 42.0 |
| [キューバでVisa・Mastercardが利用停止に 在キューバ日本国大使館「現金の持参を」 渡航者に注意喚起](https://www.itmedia.co.jp/news/articles/2606/05/news116.html) | 21.0 | 20.0 | 42.0 |
| [CISAが警告、SolarWinds Serv-Uの脆弱性を悪用してサーバーをクラッシュさせる攻撃が発生](https://www.bleepingcomputer.com/news/security/cisa-hackers-now-exploit-solarwinds-serv-u-flaw-to-crash-servers/) | 20.0 | 20.0 | 42.0 |
| [ダークウェブのNemesis Market出品者、薬物販売で26年の実刑判決](https://www.bleepingcomputer.com/news/security/dark-web-nemesis-market-vendor-gets-26-years-for-selling-drugs/) | 20.0 | 20.0 | 42.0 |
| [LinkedInの採用メッセージに潜む中国諜報活動、FBIとMI5が警告](https://www.bitdefender.com/en-us/blog/hotforsecurity/linkedin-recruiter-chinese-intelligence-fbi-mi5) | 20.0 | 20.0 | 42.0 |
| [OWASP Incubator Projectが開発者の脆弱な依存関係を数秒で発見・修正できるよう支援](https://www.securityweek.com/owasp-incubator-project-helps-developers-find-and-fix-vulnerable-dependencies-in-seconds/) | 20.0 | 20.0 | 42.0 |
| [900台超の米国ガソリンスタンドのタンクゲージシステムが攻撃にさらされる](https://www.bleepingcomputer.com/news/security/over-900-us-gas-station-tank-gauge-systems-exposed-to-attacks/) | 20.0 | 20.0 | 42.0 |
| [Nightmare Eclipseインシデントが示す研究者とベンダーの対立はなくならないかもしれない](https://cyberscoop.com/microsoft-coordinated-vulnerability-disclosure-debacle/) | 20.0 | 20.0 | 42.0 |
| [2026年DBIRが示す、攻撃はブラウザ内で進行しているという現実](https://www.bleepingcomputer.com/news/security/what-2026-dbir-confirms-attacks-are-living-in-the-browser/) | 20.0 | 20.0 | 42.0 |
| [Cisco製品の脆弱性によりサーバーサイドリクエストフォージェリが可能になる恐れ](https://www.cisecurity.org/advisory/a-vulnerability-in-cisco-products-could-allow-for-server-side-request-forgery_2026-053) | 20.0 | 20.0 | 42.0 |
| [新たな脅威クラスターOP-512がMicrosoft IISサーバーを標的にカスタムWebシェルフレームワークを使用](https://thehackernews.com/2026/06/new-threat-cluster-op-512-targets.html) | 20.0 | 20.0 | 42.0 |
| [DentaQuestの情報漏えい、260万人に影響](https://www.securityweek.com/hackers-leak-dentaquest-information-impacting-2-6-million/) | 20.0 | 20.0 | 42.0 |
| [Chrome 149で429件の脆弱性を修正](https://www.securityweek.com/chrome-149-patches-429-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [Let’s Encryptが大規模Web向けの耐量子証明書実現に向けて取り組む](https://www.helpnetsecurity.com/2026/06/05/lets-encrypt-mcts-web-post-quantum-authentication/) | 20.0 | 20.0 | 42.0 |
| [Dashlane、攻撃者による暗号化されたユーザー保管庫のダウンロードを明らかにする](https://www.itpro.com/security/dashlane-lifts-the-lid-on-attack-that-saw-hackers-downloaded-encrypted-user-vaults) | 20.0 | 20.0 | 42.0 |
| [Five Eyes：中国のスパイが偽の求人を使って政府・軍関係者を標的に](https://www.securityweek.com/five-eyes-chinese-spies-target-government-military-staff-with-fake-job-opportunities/) | 20.0 | 20.0 | 42.0 |

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
