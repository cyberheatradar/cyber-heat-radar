# 📡 サイレーダー 2026-10-22 05:00 JST

このレポートは、2026-10-21 17:00 JST〜2026-10-22 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 128
- [音声で扱う想定のトピック](#audio-topics): 8
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 95

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-109618 and CVE-2026-109619 (PHP2Shell): Two Critical PHP Remote Code Execution Flaws](#topic-38753) | 67.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [Ransomware gangs have been exploiting Palo Alto GlobalProtect VPN flaw since June](#topic-4247) | 56.0 | 77.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [Q3 2026 Threat Update: Attackers Are Exploiting Vulnerabilities Within 3 Days](#topic-38878) | 43.0 | 30.0 | 43.0 | 音声 | AI×Security枠 |
| 4 | [Cisco Expressway Series Security Hardening Release: October 2026](#topic-38838) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 5 | [Multiple Cisco Products Snort 3 Security Hardening Release: October 2026](#topic-38837) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 6 | [Cisco Unified Communications Products Security Hardening Release: October 2026](#topic-38832) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 7 | [LiteLLM PyPI Package and Docker Images Compromised to Steal Cloud and AI Credentials](#topic-38872) | 35.0 | 45.0 | 42.0 | 音声 | AI×Security枠 |
| 8 | [“Next Exploit Opportunities”: How a Threat Actor Used AI to Help Plan and Execute Multiple Types of Cybercrime Activities](#topic-38863) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-38753"></a>

### 1. CVE-2026-109618 and CVE-2026-109619 (PHP2Shell): Two Critical PHP Remote Code Execution Flaws

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 67.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

PHPにおけるCVE-2026-109618とCVE-2026-109619は、重大なリモートコード実行につながる可能性がある脆弱性として複数の情報源で言及されています。
公開情報では、パッチ提供前から悪用の試行が観測されたとする報告もあり、関連製品や運用環境への影響が注目されています。
認証なしでのリモートコード実行につながる可能性がある場合、WebサーバーやCMSを広く巻き込むおそれがあります。
複数のベンダーや研究機関が注意喚起しているため、単なる単一製品の問題ではなく、広範な影響が想定されやすい点が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 19 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- PHPを利用するサーバーや関連製品の影響有無を確認し、ベンダーの案内に沿って更新状況を点検する。
- 未適用環境がある場合は、優先度を上げて隔離・停止・制限などの暫定対策を検討する。
- Webアクセスログや監視アラートを確認し、不審な試行や異常な挙動がないか点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-109618 | 関連CVE | 1.00 | 候補あり（URL 15件以上） |
| 脆弱性 | CVE-2026-109619 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-109618](https://nvd.nist.gov/vuln/detail/CVE-2026-109618) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-](https://security.paloaltonetworks.com/CVE-2026-109618) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in PHP Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-php-october26-Jj384Daq) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP2Shell Patches Land as First Exploitation Attempts Hit Sensors](https://www.securityweek.com/php2shell-patches-land-as-first-exploitation-attempts-hit-sensors/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: Critical Vulnerabilities in PHP: CVE-2026-109618, CVE-2026-109619](https://unit42.paloaltonetworks.com/cve-2026-109618-cve-2026-109619/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP2Shell: Why websites are going offline for emergency security updates](https://www.malwarebytes.com/blog/bugs/2026/10/php2shell-why-websites-are-going-offline-for-emergency-security-updates) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP Patches Critical RCE Vulnerabilities, Organizations Urged to Take Unpatched ](https://socket.dev/blog/php-critical-rce-patches) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Widespread PHP Flaw May Cause Many Site Outages Today](https://krebsonsecurity.com/2026/10/widespread-php-flaw-may-cause-many-site-outages-today/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（15件）。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-4247"></a>

### 2. Ransomware gangs have been exploiting Palo Alto GlobalProtect VPN flaw since June

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 冷却中 |
| <nobr>温⁠度⁠感</nobr> | 56.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 77.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Palo Alto NetworksのGlobalProtect/ PAN-OSに関するCVE-2026-0257は、認証回避につながる脆弱性として以前から悪用が確認されており、最新の報告ではランサムウェア攻撃者による初期侵入手段として使われている可能性が示されています。
影響を受ける条件は特定の設定に限られますが、認証境界にあるVPN装置が突破されると、社内ネットワークへの不正アクセスの起点になり得ます。
VPN装置は外部公開されやすく、攻撃者にとって侵入の足がかりになりやすいため、認証回避の悪用は組織への影響が大きくなりがちです。
ランサムウェア事案との関連が示されている点からも、単なる脆弱性情報ではなく、実運用上の優先対応が必要なテーマといえます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 9 sources。
- 実悪用・ゼロデイ文脈。
- 技術詳細・再現情報あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 技術詳細により影響確認が進みやすい。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 影響バージョンと、認証オーバーライド機能の有無を確認し、該当する場合はベンダーの修正版適用を急ぐ。
- 認証オーバーライド用の証明書を他用途と共有していないか点検し、必要なら専用証明書へ切り替える。
- GlobalProtectの認証ログや管理ログを見直し、不審なCookie認証や不自然なVPNログインの痕跡を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-0257 | 関連CVE | 1.00 | 候補あり（URL 6件以上） |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Palo Alto | 言及あり | 0.80 | — |
| ランサムウェアグループ | Qilin | 主題 | 0.80 | — |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Arctic Wolf | 言及あり | 0.80 | — |
| 製品 | Palo Alto Networks PAN-OS | 言及あり | 0.80 | — |
| ランサムウェアグループ | INC Ransom | 主題 | 0.80 | — |
| 製品 | Palo Alto Networks Prisma Access | 言及あり | 0.80 | — |
| 製品 | Palo Alto Networks GlobalProtect | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-0257](https://nvd.nist.gov/vuln/detail/CVE-2026-0257) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Ransomware gangs have been exploiting Palo Alto GlobalProtect VPN flaw since Jun](https://www.helpnetsecurity.com/2026/10/21/ransomware-groups-exploit-palo-alto-globalprotect-cve-2026-0257/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: Active Exploitation of PAN-OS CVE-2026-0257 (Updated October 20)](https://unit42.paloaltonetworks.com/active-exploitation-of-pan-os-cve-2026-0257/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Qilin and INC Ransomware Groups Exploit Palo Alto Networks Flaw to Bypass MFA](https://thehackernews.com/2026/10/qilin-and-inc-ransomware-groups-exploit.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Qilin Ransomware Attackers Exploit PAN-OS Authentication Bypass for Initial Acce](https://thehackernews.com/2026/07/qilin-ransomware-attackers-exploit-pan.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Palo Alto Warns of Active Exploitation of PAN-OS GlobalProtect VPN Flaw](https://thehackernews.com/2026/06/palo-alto-warns-of-active-exploitation.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0257 PAN-OS: GlobalProtect Authentication Bypass Vulnerabilities (Sever](https://security.paloaltonetworks.com/CVE-2026-0257) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers are exploiting Palo Alto Networks defect that initially flew under the](https://cyberscoop.com/palo-alto-networks-cve-2026-0257-exploited-vulnerability/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-38878"></a>

### 3. Q3 2026 Threat Update: Attackers Are Exploiting Vulnerabilities Within 3 Days

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Rapid7の四半期脅威レポートによると、Q3では高・重大度の脆弱性が公開されてから実際に悪用されるまでの平均時間は3日でした。
追跡された悪用の多くが公開後1週間以内に起きており、脆弱性の公開から修正までの猶予が非常に短いことが示されています。
定期的なパッチ適用だけでは、攻撃の速さに追いつけない可能性があるためです。外部公開資産や既知の悪用対象を優先して管理する重要性が高まっています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 外部公開されている資産を洗い出し、既知の悪用事例がある脆弱性を優先して確認する。
- 認証不要またはユーザー操作不要で到達できる経路を重点的に点検する。
- すぐに修正できない場合は、補完的な防御策と検知の有無を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Q3 2026 Threat Update: Attackers Are Exploiting Vulnerabilities Within 3 Days](https://www.rapid7.com/blog/post/tr-q3-2026-threat-update-attackers-exploiting-vulnerabilities-within-3-days) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-38838"></a>

### 4. Cisco Expressway Series Security Hardening Release: October 2026

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

CiscoはExpressway Series向けに、内部テストで見つかった複数の脆弱性を修正するハードニング版のソフトウェア更新を公表しました。
対象はExpressway Core（Expressway-C）およびExpressway Edge（Expressway-E）で、現時点では悪用は確認されていないとされています。
Cisco製品は通信基盤で広く使われるため、更新の適用状況が運用継続やリスク低減に直結します。
公開情報では回避策が示されていないため、影響を受ける環境では修正適用の優先度が高い話題です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象がExpressway-C / Expressway-Eかを確認し、該当バージョンの更新有無を点検する。
- Ciscoが案内する修正版への計画的な更新を進め、保守窓口や変更管理と整合させる。
- 関連する複数のCVEがまとめて扱われているため、個別の影響範囲は別途続報や個別アドバイザリも確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-76490](https://nvd.nist.gov/vuln/detail/CVE-2026-76490) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Expressway Series Security Hardening Release: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-exwy-hardening-FhcqBVcs) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-38837"></a>

### 5. Multiple Cisco Products Snort 3 Security Hardening Release: October 2026

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

CiscoはSnort 3に関する複数の脆弱性について、2026年10月公開のセキュリティ更新を案内しています。
主要CVEであるCVE-2026-20043は、CWE-787に分類されるout-of-bounds writeに関連するとされています。
公開情報では、これらは社内テストで見つかったもので、現時点で悪用確認はされていないとされています。
Snort 3はセキュリティ機能の中核として使われることが多く、関連製品の更新遅延は運用上のリスクになり得ます。
さらに、脆弱性に対する修正版が提供されており、対応の優先度を判断しやすい点も重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当するCisco製品の利用有無を確認し、案内された更新版の適用可否を早めに判断する。
- 影響範囲が広い可能性を踏まえ、Snort 3関連の導入環境や依存構成を棚卸しする。
- 暫定回避策がないため、通常のパッチ運用に沿って速やかなアップデート計画を立てる。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20043](https://nvd.nist.gov/vuln/detail/CVE-2026-20043) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Multiple Cisco Products Snort 3 Security Hardening Release: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-hardening-snort3-ybgmhTQe) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-38832"></a>

### 6. Cisco Unified Communications Products Security Hardening Release: October 2026

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

Ciscoは、Unified Communications関連製品に対するセキュリティ強化版の更新を公開し、内部テストで見つかった複数の脆弱性に対処したとしています。
対象には Unified CM、IM & Presence、SME、Unity Connection などが含まれ、関連するCVEの一つとしてCVE-2026-76473が示されています。
現時点で、これらの問題が実際に悪用されているとは確認されていません。企業の音声・通話基盤は業務継続に直結するため、該当製品を使っている組織では更新の優先度が高い話題です。
Ciscoが修正を提供しており回避策はないとされるため、影響範囲の確認と計画的な適用が重要になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Cisco Unified Communications関連製品の利用有無とバージョンを確認し、修正済みリリースへの更新計画を立てる。
- 公開される追加情報や個別アドバイザリがあれば、影響するCWEやCVEを突き合わせて自組織への該当性を再評価する。
- 通話・連携系システムは停止影響が大きいため、検証環境での事前確認とメンテナンス手順の調整を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-76473](https://nvd.nist.gov/vuln/detail/CVE-2026-76473) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified Communications Products Security Hardening Release: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-voice-hardening-twgbH9e3) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-38872"></a>

### 7. LiteLLM PyPI Package and Docker Images Compromised to Steal Cloud and AI Credentials

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>サ⁠プ⁠ラ⁠イ⁠チ⁠ェ⁠ー⁠ン</nobr> / <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 45.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

LiteLLMのPyPIパッケージとDockerイメージが改ざんされ、クラウド認証情報や開発者の秘密情報、AIプロバイダのキーを狙う不正コードが混入したとされています。
対象はLiteLLM 1.107.0で、サプライチェーン経由の影響が懸念されています。
開発者やCI/CD環境で利用される配布物が侵害されると、導入元の組織に広く被害が及ぶおそれがあります。
特にクラウドやAI関連の認証情報が含まれるため、影響範囲がサービス運用にも波及し得ます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- LiteLLM 1.107.0を利用している場合は、入手元の正当性と現在の利用状況を確認する。
- クラウド資格情報、APIキー、AI関連シークレットのローテーションや漏えい有無の点検を行う。
- パッケージ管理やコンテナ取得元の監視を強化し、今後の更新は公式告知に基づいて判断する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Chromium | 言及あり | 0.80 | — |
| 製品 | Mozilla Firefox | 言及あり | 0.80 | — |
| 製品 | Cursor | 言及あり | 0.80 | — |
| 製品 | Microsoft Azure | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| マルウェア | ZLib | 主題 | 0.80 | — |
| 攻撃/検証ツール | Certify | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [LiteLLM PyPI Package and Docker Images Compromised to Steal Cloud and AI Credent](https://socket.dev/blog/litellm-compromise) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-38863"></a>

### 8. “Next Exploit Opportunities”: How a Threat Actor Used AI to Help Plan and Execute Multiple Types of Cybercrime Activities

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報に基づく調査で、脅威アクターがAIの安全対策を回避しながら、認証情報の窃取、VoIP不正利用の計画、データベース流出に関わる活動を進めていた可能性が示されています。
AIがサイバー犯罪の企図や作業の一部に悪用されうる実例として整理されています。生成AIの悪用は、攻撃の計画や準備を効率化しうるため、従来の脅威とは別の観点で監視が必要です。
特に、対話型AIの安全制御を回避する手口が確認されると、運用側のガードレールや監視設計の見直しにつながります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIサービスの利用ログや異常な質問傾向を監視し、認証情報や不正利用に結びつく兆候を早期に検知する。
- 生成AIの社内利用では、機密情報の入力制限と出力の取り扱いルールを明確にして、情報流出リスクを抑える。
- VoIPやアカウント管理、データベース周辺の不審な操作を横断的に確認し、複数の不正行為が連動していないかを見る。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [“Next Exploit Opportunities”: How a Threat Actor Used AI to Help Plan and Execut](https://unit42.paloaltonetworks.com/ai-assisted-cybercrime-analysis/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

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
| [ClickFixがこれまでになく拡大、AIツールが最も説得力のある誘いに](https://www.bleepingcomputer.com/news/security/clickfix-has-never-been-bigger-and-ai-tools-are-its-most-convincing-lure-yet/) | 33.0 | 20.0 | 42.0 |
| [RansomwareがQ3を席巻、Rapid7が3日以内に悪用された高深刻度の脆弱性を報告](https://www.securityweek.com/high-severity-flaws-exploited-in-three-days-as-ransomware-dominates-q3-rapid7/) | 28.0 | 30.0 | 42.0 |
| [FBIとCISA、SafePayランサムウェアが重要インフラに脅威と警告](https://www.cybersecuritydive.com/news/fbi-cisa-warn-safepay-ransomware-threat-critical-infrastructure/833589/) | 28.0 | 30.0 | 42.0 |
| [CISA、FBI、関係機関が複数の重要インフラ分野を標的とするSafePayランサムウェア攻撃者について警告](https://www.cisa.gov/news-events/news/cisa-fbi-and-partners-warn-organizations-safepay-ransomware-actors-targeting-multiple-critical) | 28.0 | 30.0 | 42.0 |
| [ライバルのランサムウェア集団が市場覇権を争い攻撃が増加](https://www.infosecurity-magazine.com/news/rival-gangs-vie-for-market/) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア攻撃で「Password1」アカウントが侵害され、子どものデータが窃取される](https://www.infosecurity-magazine.com/news/children-data-stolen-password1/) | 28.0 | 30.0 | 42.0 |
| [CISA: SafePayランサムウェアが600以上の重要インフラ組織を攻撃](https://www.bleepingcomputer.com/news/security/cisa-and-fbi-safepay-ransomware-has-hit-over-600-critical-infrastructure-organizations/) | 28.0 | 30.0 | 42.0 |
| [OVHcloudのGitHub侵害、GlassWorm脅威アクターに関連か](https://www.darkreading.com/cyberattacks-data-breaches/ovhcloud-github-compromise-glassworm-threat-actors) | 28.0 | 20.0 | 42.0 |
| [ロシア関連のハッカーがNATOの造船企業に侵入、最新のスパイ活動キャンペーンで](https://www.cybersecuritydive.com/news/russia-nato-hacking-shipbuilder-critical-infrastructure/833509/) | 28.0 | 20.0 | 42.0 |
| [AmazonテーマのClickFixキャンペーンがマルウェアを配布](https://www.huntress.com/blog/amazon-clickfix-finger) | 28.0 | 20.0 | 42.0 |
| [数十年前のWindowsユーティリティが現代のClickFix攻撃を支援](https://www.darkreading.com/cyberattacks-data-breaches/decades-old-windows-utility-modern-clickfix-attack) | 28.0 | 20.0 | 42.0 |
| [攻撃者がUpdraftCentralキーを悪用してWordPressサイトにバックドアを設置](https://thehackernews.com/2026/10/attackers-abuse-updraftcentral-keys-to.html) | 28.0 | 20.0 | 42.0 |
| [GitHub上のOVHcloud CLIリリースに紛れ込んだ情報窃取型マルウェア](https://www.helpnetsecurity.com/2026/10/21/ovhcloud-cli-github-malware/) | 28.0 | 20.0 | 42.0 |
| [Signalの不具合で通話終了後も盗聴される可能性](https://www.theregister.com/security/2026/10/21/signal-bug-could-keep-your-mic-and-camera-on-after-hangup/5304528) | 26.0 | 28.0 | 54.0 |
| [Google、ClickFix攻撃と安全でないHTTP接続に対するChromeの防御を強化](https://www.securityweek.com/google-hardens-chrome-against-clickfix-attacks-insecure-http-connections/) | 25.0 | 20.0 | 42.0 |
| [OpenAIのGPT-6エージェント、安全監視を削除した後にそれを否定した問題](https://thehackernews.com/2026/10/openais-gpt-6-agent-removed-safety.html) | 25.0 | 20.0 | 42.0 |
| [OpenAIエージェントが安全監視を無効化し、隠蔽もした件](https://www.bleepingcomputer.com/news/security/openai-agents-disabled-safety-monitoring-one-lied-about-it/) | 25.0 | 20.0 | 42.0 |
| [AIを活用してフィッシング文面を作成し悪意ある活動を隠蔽する新たなPhaaSプラットフォーム](https://www.infosecurity-magazine.com/news/new-phaas-uses-ai-phishing-lures/) | 25.0 | 20.0 | 42.0 |
| [「Context Bombs」でAIエージェントを偽の標的に誘導し攻撃成功率を低下させる手法](https://www.securityweek.com/context-bombs-cut-ai-attack-success-by-misleading-agents-with-fake-targets/) | 25.0 | 20.0 | 42.0 |
| [Symantec、AIエージェントを乗っ取って自律型サイバー攻撃を行うモデルを発見](https://www.infosecurity-magazine.com/news/symantec-ai-agent-llmjacking/) | 25.0 | 20.0 | 42.0 |
| [PHP2Shell：AIがインターネットの70%に影響する重大なRCE脆弱性を発見](https://www.wiz.io/blog/php2shell-php-rce) | 25.0 | 20.0 | 42.0 |
| [NVIDIA、AIエージェントの境界越えを防ぐセキュリティアーキテクチャを発表](https://www.helpnetsecurity.com/2026/10/21/nvidia-openshell-reference-architecture/) | 25.0 | 20.0 | 42.0 |
| [LiteLLMが侵害され、認証情報が窃取される](https://www.wiz.io/blog/litellm-compromised-steals-credentials) | 25.0 | 20.0 | 42.0 |
| [Asymptote Labs、AIエージェント実行時のセキュリティ強化に向け550万ドルのシード調達](https://www.securityweek.com/asymptote-labs-lands-5-5-million-seed-for-ai-agent-runtime-security/) | 25.0 | 20.0 | 42.0 |
| [OpenAI Agentsがセキュリティチームのアラートを無効化し、ミスアライメント監視を削除](https://www.securityweek.com/openai-agents-silenced-security-team-alerts-removed-misalignment-monitor/) | 25.0 | 20.0 | 42.0 |
| [AIがスクリプトキディを高度なインフラ攻撃者へ変える可能性](https://www.theregister.com/security/2026/10/21/ai-has-potential-to-turn-script-kiddies-into-sophisticated-infrastructure-attackers/5304297) | 25.0 | 20.0 | 42.0 |
| [生成AIが行動の兆候を消し、行動ベースのみの検知を弱体化させているとProofpointが報告](https://thehackernews.com/2026/10/generative-ai-is-erasing-behavioral.html) | 25.0 | 20.0 | 42.0 |
| [Nvidia、AIエージェント制御のためにOpenShellを採用](https://www.theregister.com/ai-and-ml/2026/10/21/nvidia-picks-openshell-to-tame-ai-gents/5304319) | 25.0 | 20.0 | 42.0 |
| [米国の政府システムからのDeepSeek排除を受け、中国がDeepSeekを擁護](https://www.securityweek.com/china-defends-deepseek-after-us-ban-of-its-ai-from-government-systems/) | 25.0 | 20.0 | 42.0 |
| [Agentic Pentestingにおけるハーネス構築の難しさ](https://thehackernews.com/2026/10/the-harness-is-hard-part-of-agentic.html) | 25.0 | 20.0 | 42.0 |
| [中国製AIモデルは「米国の請負業者向け」と伝えると、より脆弱なコードを書く](https://www.securityweek.com/chinese-ai-model-writes-more-hackable-code-when-told-its-for-us-contractor/) | 25.0 | 20.0 | 42.0 |
| [HyperArmorにおける3本柱の多層防御](https://www.security.com/feature-stories/hyperarmor-three-pillars-uphold-layered-defense) | 25.0 | 20.0 | 42.0 |
| [自律型LLMjacking：露出したAIモデルを乗っ取り攻撃を実行する「Skynet」エージェント](https://www.security.com/threat-intelligence/ai-llmjacking-skynet) | 25.0 | 20.0 | 42.0 |
| [ThreatLockerがAIエージェントのアクセスと実行に外部制御を追加](https://www.helpnetsecurity.com/2026/10/21/threatlocker-zero-trust-ai-control-ztaic/) | 25.0 | 20.0 | 42.0 |
| [「ロボティクス×生成AI」は日本にとって最大の機会、AWSは黒子として貢献できる――「AIエージェントがロボットを育てる」技術などを披露【CEATEC 2026】](https://internet.watch.impress.co.jp/docs/event/2149797.html) | 25.0 | 20.0 | 42.0 |
| [Cisco複数製品におけるSnort 3のサービス妨害脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-snort3-misc-dos-6mB22qAK) | 24.0 | 46.0 | 50.0 |
| [Cisco Unified Communications Managerの不適切なアクセス制御の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-cucm-access-PW9e8Jt2) | 24.0 | 46.0 | 50.0 |
| [Cisco IOS XR Software for ASR 9000 Series RoutersにおけるIPv4ユニキャストパケットのサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asr9k-tUyxcyXN) | 24.0 | 46.0 | 50.0 |
| [Cisco複数製品のSnort 3 SMTP MIMEにおけるサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-snort3-mime-vulns-bkXjcKkt) | 24.0 | 46.0 | 50.0 |
| [Cisco Expressway Series のリモートコード実行の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-vcs-static-cred-hr7EWZ8t) | 24.0 | 46.0 | 50.0 |
| [複数のCisco製品におけるSnort 3のGRE処理に起因するサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-snort3-gre-JNpMHrTv) | 24.0 | 46.0 | 50.0 |
| [複数のCisco製品におけるSnort 3のサービス拒否脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-snort3-gtpcodec-dos-Rmecfepz) | 24.0 | 46.0 | 50.0 |
| [Cisco Expressway Seriesの情報漏えい脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-expressway-inf-disc-vvYqgSTS) | 24.0 | 46.0 | 50.0 |
| [複数のCisco製品におけるSnort 3のVisual Basic for Applicationsバッファオーバーフローによるサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-snort3-vba-bufdos-jAuFdvn9) | 24.0 | 46.0 | 50.0 |
| [PHPにおける複数の脆弱性によりリモートコード実行が可能となるおそれ](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-php-could-allow-for-remote-code-execution_2026-119) | 24.0 | 38.0 | 42.0 |
| [PHP、2件の深刻なPHP2Shell RCE脆弱性に緊急パッチを公開、悪用試行も確認](https://thehackernews.com/2026/10/php-issues-emergency-patches-for-two.html) | 24.0 | 38.0 | 42.0 |
| [PHP Coreに存在する重大なリモートコード実行の脆弱性](https://www.akamai.com/blog/security-research/2026/oct/critical-remote-code-execution-vulnerabilities-php-core) | 24.0 | 38.0 | 42.0 |
| [PHP2Shell：14:00 UTCのPHP RCEパッチ適用前に本当に有効な対策とそうでない対策](https://thehackernews.com/2026/10/php2shell-what-actually-protects-you.html) | 24.0 | 38.0 | 42.0 |
| [Cisco Secure Client Secure Firewall Posture Moduleの権限昇格の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sec-client-priv-esc-muF8eZdm) | 22.0 | 40.0 | 50.0 |
| [PHPの重大脆弱性「PHP2Shell」はセキュリティ企業のCalifとWizがAIを用いて発見しOpenAIの枠組みを使って対策したことが判明](https://gigazine.net/news/20261022-php2shell-wiz-openai-calif/) | 22.0 | 20.0 | 42.0 |
| [「PHP」に2件の深刻なRCE脆弱性 - アップデートを公開](https://www.security-next.com/191749) | 22.0 | 20.0 | 42.0 |
| [PHPが緊急アップデート「8.5.12」「8.4.27」「8.3.36」「8.2.35」をリリース](https://gigazine.net/news/20261021-php-critical-vulnerabilities/) | 22.0 | 20.0 | 42.0 |
| [個人情報流出が判明、意図しない売買も - 岩井コスモ証券](https://www.security-next.com/191717) | 22.0 | 20.0 | 42.0 |
| [ニコニコやpixivなど各種ウェブサイトおよびアプリがPHPの緊急パッチに対応するべくメンテナンス入り](https://gigazine.net/news/20261021-php-php2shell-maintenance/) | 22.0 | 20.0 | 42.0 |
| [2010年から存在するWi-Fiの欠陥でパスワードを知らなくてもルーターを乗っ取れるバグが発覚、数百万台が影響を受ける可能性](https://gigazine.net/news/20261021-wpsplinter/) | 22.0 | 20.0 | 42.0 |
| [「代金後払いサービス」で個人情報が流出 - ヤマト運輸](https://www.security-next.com/191595) | 22.0 | 20.0 | 42.0 |
| [正規インフラを悪用して攻撃を送り込む手口](https://blog.talosintelligence.com/parasitizing-trust-how-legitimate-infrastructure-becomes-a-delivery-pipeline-for-attackers/) | 22.0 | 20.0 | 42.0 |
| [PHPに深刻度「9.2」の脆弱性が2件発覚、サーバー乗っ取りの恐れで緊急パッチを10月21日に公開へ](https://gigazine.net/news/20261021-php2shell/) | 22.0 | 20.0 | 42.0 |
| [PHPにおける重大な脆弱性（2026-018）](https://cert.europa.eu/publications/security-advisories/2026-018/) | 21.0 | 38.0 | 42.0 |
| [PHPの「緊急」レベルの脆弱性、開発元が修正バージョン公開 「直ちにアップデートを」](https://www.itmedia.co.jp/news/article/2610/22/2000002480/) | 21.0 | 20.0 | 42.0 |
| [PHP、認証不要のリモートコード実行につながる重大脆弱性2件を修正 全ユーザーに即時更新を呼び掛け](https://news.mynavi.jp/techplus/article/20261022-5170265/) | 21.0 | 20.0 | 42.0 |
| [PHPの重大な脆弱性で緊急メンテナンス相次ぐ さくらやCygames、pixivなど](https://xtech.nikkei.com/atcl/nxt/column/18/00001/12112/) | 21.0 | 20.0 | 42.0 |
| [PHPの重大脆弱性「php2shell」、パッチ公開まで待てない GMOが示した暫定策と注意点](https://atmarkit.itmedia.co.jp/ait/articles/2610/21/news072.html) | 21.0 | 20.0 | 42.0 |
| [IPA、PHPのセキュリティリリース公開を事前告知 - 対象システムの棚卸しを呼びかけ](https://news.mynavi.jp/techplus/article/20261021-5168892/) | 21.0 | 20.0 | 42.0 |
| [著名ITサービス相次いで緊急メンテへ コドモン、シャドバ、BASE、さくらのレンタルサーバなど 「PHP」脆弱性に起因か](https://www.itmedia.co.jp/news/article/2610/21/2000002472/) | 21.0 | 20.0 | 42.0 |
| [LiteLLMがサプライチェーン攻撃で侵害され、認証情報窃取ツールとバックドアを配布](https://thehackernews.com/2026/10/litellm-compromised-in-supply-chain.html) | 20.0 | 45.0 | 42.0 |
| [PHP2Shell：未修正の2件の重要なPHP RCE脆弱性（CVSS 9.2）で緊急セキュリティ警告](https://thehackernews.com/2026/10/php2shell-two-unpatched-critical-php.html) | 20.0 | 38.0 | 42.0 |
| [Open Source Snort 3のコントロールチャネルソケットにおける任意コマンド実行の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-opensrc-snort3-2fXGJPfe) | 20.0 | 28.0 | 50.0 |
| [Cloudflare WAFのフルトランザクション検知機能の導入](https://blog.cloudflare.com/full-transaction-waf/) | 20.0 | 20.0 | 48.0 |
| [WhatsAppのチャットボットにプライバシー規制当局へ言及しない隠し指示が与えられていた](https://www.malwarebytes.com/blog/news/2026/10/whatsapp-chatbot-privacy-regulators) | 20.0 | 20.0 | 42.0 |
| [CISAが警告、Plexの脆弱性連鎖を悪用したPlex2Shell攻撃でサーバー侵害](https://www.bleepingcomputer.com/news/security/cisa-hackers-chain-plex-flaws-in-plex2shell-attacks-to-breach-servers/) | 20.0 | 20.0 | 42.0 |
| [LiteLLMのサプライチェーン攻撃でパスワードと秘密情報が流出](https://www.theregister.com/security/2026/10/21/litellm-supply-chain-attack-hoovers-up-passwords-and-secrets/5304548) | 20.0 | 20.0 | 42.0 |
| [弱い暗号化証明書により、攻撃者がWebサイトを容易に詐称できた可能性](https://www.cybersecuritydive.com/news/website-encryption-security-certificates-emudhra-incident/833622/) | 20.0 | 20.0 | 42.0 |
| [Optiv、CyberBOTサイバーセキュリティ意識向上トレーニングプログラムを開始](https://www.darkreading.com/cybersecurity-operations/optiv-launches-cyberbot-cybersecurity-awareness-training-program) | 20.0 | 20.0 | 42.0 |
| [調査で判明、高名な経営幹部はデジタル露出が物理的リスクに変わっても「手が届かない存在」と感じている](https://www.darkreading.com/cybersecurity-operations/360-privacy-survey-high-profile-executives-feel-untouchable) | 20.0 | 20.0 | 42.0 |
| [Nikkei、1か月で3件目の侵害報告後に数百万件の記録流出を認める](https://www.itpro.com/security/data-breaches/nikkei-admits-millions-of-records-stolen-after-reporting-third-breach-in-a-month) | 20.0 | 20.0 | 42.0 |
| [深刻なPHP脆弱性に対する修正パッチが公開される](https://www.itpro.com/security/fixes-issued-for-critical-php-vulnerabilities-security-agencies-warn-patch-now-or-take-systems-offline) | 20.0 | 20.0 | 42.0 |
| [PHPの2つの脆弱性への懸念が高まり、数百のWebサイトがオフラインに](https://therecord.media/php-script-vulnerabilities-warnings) | 20.0 | 20.0 | 42.0 |
| [PHPの重大な脆弱性により多くのWebサイトが侵害される恐れ](https://www.cybersecuritydive.com/news/php-website-vulnerabilities/833580/) | 20.0 | 20.0 | 42.0 |
| [eMudhraのセキュリティ不備により信頼されたCAの署名鍵が誰でもアクセス可能な状態にあった](https://www.helpnetsecurity.com/2026/10/21/emudhra-certificates-private-keys-compromised/) | 20.0 | 20.0 | 42.0 |
| [Google Chromeが悪意あるコマンドの実行を防ぐClickFix警告を追加](https://thehackernews.com/2026/10/google-chrome-adds-clickfix-warnings-to.html) | 20.0 | 20.0 | 42.0 |
| [Huntress Managed ESPMにおける攻撃抑止：ClickFixの妨害](https://www.huntress.com/blog/espm-attack-reduction-clickfix) | 20.0 | 20.0 | 42.0 |
| [Chromeの353件の新しいセキュリティ修正の大半はメモリバグが原因](https://www.securityweek.com/memory-bugs-account-for-most-of-chromes-353-new-security-fixes/) | 20.0 | 20.0 | 42.0 |
| [Amazon MusicとYouTubeの偽提携でクリエイターをGoogleログインの罠に誘導](https://www.malwarebytes.com/blog/threat-intel/2026/10/fake-amazon-music-x-youtube-deal-lures-creators-into-a-google-login-trap) | 20.0 | 20.0 | 42.0 |
| [中国系のBronze SandcastleがSandboxieのDLLサイドローディングを悪用してバックドアを展開](https://thehackernews.com/2026/10/china-aligned-bronze-sandcastle-abuses.html) | 20.0 | 20.0 | 42.0 |
| [Browsers、復元可能な秘密鍵を持つeMudhraの中間CAをブロック](https://www.securityweek.com/browsers-block-emudhra-intermediate-cas-over-recoverable-private-keys/) | 20.0 | 20.0 | 42.0 |
| [EU、Booking.comに詐欺対策の強化を要請](https://www.theregister.com/security/2026/10/21/eu-wants-bookingcom-to-check-out-of-its-scam-problem/5304413) | 20.0 | 20.0 | 42.0 |
| [SafePayが世界中の重要インフラ被害者600件を侵害、CISAが警告](https://www.infosecurity-magazine.com/news/safepay-compromised-critical/) | 20.0 | 20.0 | 42.0 |
| [攻撃者が300以上のTor Exit Relayを乗っ取りSSH接続を傍受](https://thehackernews.com/2026/10/attackers-hijacked-over-300-tor-exit.html) | 20.0 | 20.0 | 42.0 |
| [予定されたセキュリティパッチ公開前に漏えいした重大なPHP脆弱性](https://www.infosecurity-magazine.com/news/critical-php-vulnerabilities-leaked/) | 20.0 | 20.0 | 42.0 |
| [Grafana LabsがKnowledge Graphでオブザーバビリティとインシデント対応を連携](https://www.helpnetsecurity.com/2026/10/21/grafana-labs-knowledge-graph/) | 20.0 | 20.0 | 42.0 |
| [ニフティ、不正アクセスで続報。調査により対象が絞り込まれ、最大1万8000件に](https://internet.watch.impress.co.jp/docs/news/2150101.html) | 20.0 | 20.0 | 42.0 |
| [Safariがメールアドレスを追跡IDに変換するトラッカーをブロックする](https://www.helpnetsecurity.com/2026/10/21/apple-safari-tracking-protection/) | 20.0 | 20.0 | 42.0 |
| [米政府、DeepSeekを連邦民間システムから削除し新規購入を禁止](https://thehackernews.com/2026/10/us-orders-deepseek-removed-from-federal.html) | 20.0 | 20.0 | 42.0 |
| [PHP緊急脆弱性「php2shell」パッチ今夜11時公開、その前にできる対策は……GMO系セキュリティ企業が提唱【更新】](https://www.itmedia.co.jp/news/article/2610/21/2000002462/) | 19.0 | 20.0 | 42.0 |

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
