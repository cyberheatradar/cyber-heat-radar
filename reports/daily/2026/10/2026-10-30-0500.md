# 📡 サイレーダー 2026-10-30 05:00 JST

このレポートは、2026-10-29 17:00 JST〜2026-10-30 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 99
- [音声で扱う想定のトピック](#audio-topics): 9
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 65

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Chinese Hackers Quietly Used Low-Severity ESXi Logging Flaw as Zero-Day](#topic-40319) | 51.0 | 46.0 | 59.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [Cisco Patches Actively Exploited ASA and FTD VPN Flaw That Can Crash Firewalls](#topic-40437) | 49.0 | 64.0 | 51.0 | 音声 | 温度感上位枠 |
| 3 | [Hackers exploit Cisco SD-WAN flaw to deploy custom KeyDrift malware](#topic-17617) | 47.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 4 | [Have an older iPhone or iPad? Apple has a security update for you](#topic-34785) | 43.0 | 56.0 | 67.0 | 音声 | 温度感上位枠 |
| 5 | [Tracking AI adoption in North Korean threat actor tradecraft](#topic-40377) | 35.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 6 | [Exploitation attempts against recently patched Oracle EBS flaw have begun (CVE-2026-101767)](#topic-40192) | 33.0 | 46.0 | 58.0 | 音声 | 温度感上位枠 |
| 7 | [Fake ChatGPT and Claude Apps Abuse Signed Executables to Deploy Crypto Miners](#topic-40381) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 8 | [Yoba malware hides in fake desktop versions of ChatGPT and Claude](#topic-40387) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 9 | [IR trends Q3 2026: Actors impersonate IT help desks in vishing attacks as ransomware activity increases](#topic-40399) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 10 | [New Cisco firewall zero-day exploited to crash SSL VPN devices](#topic-40432) | 30.0 | 20.0 | 43.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-40437"></a>

### 1. Cisco Patches Actively Exploited ASA and FTD VPN Flaw That Can Crash Firewalls

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 49.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

Ciscoは、Secure Firewall ASA SoftwareとFTD Softwareに存在する高深刻度の脆弱性CVE-2026-76418に対する修正パッチを公開しました。
同社によると、この問題はすでに実環境で悪用が確認されており、未認証のリモート攻撃者によってファイアウォールの停止や障害を引き起こされるおそれがあります。
VPNや境界防御に使われる製品への影響が示されており、可用性への影響が大きい点が注目されています。
実際の悪用が確認されているとされるため、放置すると業務通信の保護と継続性の両面でリスクが高まります。

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

- Cisco ASA/FTDの対象バージョンを確認し、提供済みの修正を速やかに適用する。
- インターネット公開されているVPN終端装置を優先的に点検し、異常な再起動や応答停止の有無を監視する。
- 公式アドバイザリに基づき、影響範囲と回避策の有無を確認しつつ、ログ保全とインシデント対応手順を準備する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-76418 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Adaptive Security Appliance | 言及あり | 0.80 | — |
| 製品 | Cisco Firepower Threat Defense | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-76418](https://nvd.nist.gov/vuln/detail/CVE-2026-76418) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Patches Actively Exploited ASA and FTD VPN Flaw That Can Crash Firewalls](https://thehackernews.com/2026/10/cisco-patches-actively-exploited-asa.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit Second Cisco Firewall VPN Zero-Day Since August](https://www.securityweek.com/attackers-exploit-second-cisco-firewall-vpn-zero-day-since-august/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-17617"></a>

### 2. Hackers exploit Cisco SD-WAN flaw to deploy custom KeyDrift malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 47.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Catalyst SD-WANの脆弱性CVE-2026-20127について、認証回避を伴う深刻な問題として注意喚起が出ています。
公開情報では、この脆弱性が実際の攻撃に悪用され、カスタムマルウェアの展開につながったと報じられています。
SD-WANの制御基盤が侵害されると、ネットワーク設定の変更や広範な影響につながるおそれがあります。
ベンダーの修正が提供されている一方、悪用観測があるため、通常の重要脆弱性よりも優先度を高く見て対応する必要があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
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

- Ciscoの修正済みバージョン適用状況を確認し、影響製品の露出を最小化する。
- 管理系インターフェースや関連ログを点検し、不審な認証成功や設定変更の痕跡がないか確認する。
- SD-WAN管理プレーンへのアクセス制御を再点検し、必要最小限の到達性に絞る。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20127 | 関連CVE | 1.00 | 候補あり（URL 6件以上） |
| 脆弱性 | CVE-2026-20245 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Catalyst SD-WAN Manager | 言及あり | 0.80 | — |
| 脅威アクター | Volt Typhoon | 主題 | 0.80 | — |
| 製品 | OpenSSL | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20127](https://nvd.nist.gov/vuln/detail/CVE-2026-20127) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Hackers exploit Cisco SD-WAN flaw to deploy custom KeyDrift malware](https://www.bleepingcomputer.com/news/security/hackers-exploit-cisco-sd-wan-flaw-to-deploy-custom-keydrift-malware/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-rpa-EHchtZk) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Inside KeyDrift: Analyzing historical UAT-11473 activity on Cisco SD-WAN](https://blog.talosintelligence.com/uat-11473-keydrift/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Malicious hackers exploit Cisco zero-day for highest access level at communicati](https://cyberscoop.com/cisco-sd-wan-zero-day-exploit-communications-provider/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco adds another SD-WAN box to max-severity bug advisory](https://www.theregister.com/security/2026/06/17/cisco-adds-another-sd-wan-box-to-max-severity-bug-advisory/5257621) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco SD-WAN Zero-Day Exploitation Tied to Volt Typhoon’s ‘Silent Train’ Network](https://www.securityweek.com/cisco-sd-wan-zero-day-exploitation-tied-to-volt-typhoons-silent-train-network/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-34785"></a>

### 3. Have an older iPhone or iPad? Apple has a security update for you

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>i⁠O⁠S</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Appleは、古いiPhoneやiPadを対象にセキュリティ修正を含む更新を公開しました。
対象のCVE-2026-86950はCoreGraphicsに関する問題とされ、悪用された可能性がある脆弱性として複数の情報源で扱われています。
旧世代の端末は最新系と更新経路が異なることがあり、修正の適用漏れが起きやすいため注目されます。公開PoCの言及もあるため、既知の脆弱性として放置せず、影響範囲の確認が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- iPhone/iPadの対象世代とOS枝分かれを確認し、該当端末には提供済みの修正を適用する。
- 利用者向けに不審なファイルの取り扱いに注意喚起し、特に受信した文書や添付の扱いを見直す。
- 組織内のApple端末で更新状況を点検し、古い端末が残っていないか棚卸しする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-86950 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Apple | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Apple iOS | 言及あり | 0.80 | — |
| ベンダー | Meta | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-86950](https://nvd.nist.gov/vuln/detail/CVE-2026-86950) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Have an older iPhone or iPad? Apple has a security update for you](https://www.malwarebytes.com/blog/bugs/2026/10/have-an-older-iphone-or-ipad-apple-has-a-security-update-for-you) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Backports Fix for Exploited CoreGraphics Flaw to Older iPhones and iPads](https://thehackernews.com/2026/10/apple-backports-fix-for-exploited.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple CoreGraphics PoC Emerges as WhatsApp PDF Checks Hint at Possible Delivery ](https://thehackernews.com/2026/10/apple-coregraphics-poc-emerges-as.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Patches CoreGraphics Zero Day Exploited in Attacks](https://www.infosecurity-magazine.com/news/apple-patches-coregraphics-zero/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Zero-Day Vulnerability Weaponized in Targeted Attacks](https://www.darkreading.com/cyberattacks-data-breaches/apple-zero-day-vulnerability-weaponized-targeted-attacks) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple patches CoreGraphics zero-day already exploited in targeted attacks](https://www.theregister.com/security/2026/09/29/apple-patches-coregraphics-zero-day-already-exploited-in-targeted-attacks/5299721) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Update your iPhone, iPad, or Mac: Flaw could run attackers’ code](https://www.malwarebytes.com/blog/bugs/2026/09/update-your-iphone-ipad-or-mac-flaw-could-run-attackers-code) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-40377"></a>

### 4. Tracking AI adoption in North Korean threat actor tradecraft

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftは、北朝鮮系とされる脅威アクターがAIの利用を広げており、その活用度合いにはばらつきがあると報告しました。
対象としてAPT38、Lazarus Group、Kimsuky、Andarielが挙げられており、攻撃活動の一部でAIを取り入れる動きが示されています。
脅威アクターによるAI活用は、攻撃の効率化や作業の高速化につながる可能性があるため注目されています。
AIが攻撃チェーンに組み込まれる傾向を把握しておくことは、防御側の監視や対策の優先度判断に役立ちます。

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

- AIを使った不審な文面生成や偽装活動を前提に、メール・チャット・認証ログの異常を確認する。
- 北朝鮮系脅威グループに関連する戦術・手口・標的の変化を継続監視し、既存の検知ルールを見直す。
- Microsoft 365、Entra ID、Teams など主要な業務基盤で、なりすましや不審なアクセスの検知設定を再点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脅威アクター | APT38 | 主題 | 0.80 | — |
| 脅威アクター | Lazarus Group | 主題 | 0.80 | — |
| 脅威アクター | Kimsuky | 主題 | 0.80 | — |
| 脅威アクター | Andariel | 主題 | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Adobe | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |
| 製品 | Microsoft Entra ID | 言及あり | 0.80 | — |
| 製品 | Microsoft Teams | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Tracking AI adoption in North Korean threat actor tradecraft](https://www.microsoft.com/en-us/security/blog/2026/10/29/tracking-ai-adoption-in-north-korean-threat-actor-tradecraft/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-40192"></a>

### 5. Exploitation attempts against recently patched Oracle EBS flaw have begun (CVE-2026-101767)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 58.0 |

#### 概要

Oracle E-Business Suiteの脆弱性CVE-2026-101767について、公開後まもなく探索的な攻撃試行が始まったと複数の情報源が伝えています。
対象は認証不備に関連する重大な脆弱性とされ、CVSS 9.8と評価されていますが、実際の悪用被害の広がりについては現時点で断定できません。
基幹業務で使われることの多いOracle EBSが対象であり、パッチ適用の遅れがそのままリスクにつながりやすい点が注目されています。
公開直後から攻撃対象になりうるため、早期対応の重要性が高い事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Oracle EBSの該当パッチ適用状況を確認し、未適用環境を優先して是正する。
- 外部公開しているEBS関連サービスについて、想定外のアクセスや異常なリクエストの監視を強化する。
- 脆弱性の影響範囲を確認し、認証情報の見直しや関連ログの点検を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-101767 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Oracle | 言及あり | 0.80 | — |
| 製品 | Oracle E-Business Suite | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-101767](https://nvd.nist.gov/vuln/detail/CVE-2026-101767) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Exploitation attempts against recently patched Oracle EBS flaw have begun (CVE-2](https://www.helpnetsecurity.com/2026/10/29/oracle-e-business-suite-cve-2026-101767-exploitation/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers Target Critical Oracle E-Business Suite RCE Flaw Days After Security Pat](https://thehackernews.com/2026/10/hackers-target-critical-oracle-e.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers Start Probing Fresh Oracle EBS Vulnerability](https://www.securityweek.com/hackers-start-probing-fresh-oracle-ebs-vulnerability/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-40381"></a>

### 6. Fake ChatGPT and Claude Apps Abuse Signed Executables to Deploy Crypto Miners

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

偽のChatGPTやClaudeのデスクトップアプリを装った不正な配布物を通じて、暗号資産マイナーや悪意あるローダーが展開されていると報告されています。
公開情報では、GitHub上の偽プロジェクトや署名済み実行ファイルの悪用が関与しているとされますが、詳細な手口は記事内情報に基づく範囲で扱う必要があります。
人気のAIツール名を悪用するため、利用者が正規アプリと誤認しやすく、感染リスクが高まります。
組織としては、ソフトウェア入手経路の管理や実行ファイルの信頼性確認の重要性が改めて示されています。

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

- AI関連ツールを装う配布物について、公式配布元以外からの入手を避ける運用を徹底する。
- 署名済み実行ファイルでも無条件に信頼せず、入手元・ハッシュ・配布実績などを合わせて確認する。
- エンドポイントで不審なプロセス起動や暗号資産マイニングに関連する挙動を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Anthropic | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | ChatGPT | 主題 | 0.80 | — |
| AIモデル/プロジェクト | Claude | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Fake ChatGPT and Claude Apps Abuse Signed Executables to Deploy Crypto Miners](https://thehackernews.com/2026/10/fake-chatgpt-and-claude-apps-abuse.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-40387"></a>

### 7. Yoba malware hides in fake desktop versions of ChatGPT and Claude

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Check Pointによると、ChatGPTやClaudeのデスクトップ版を装った偽のGitHubプロジェクトが、最終的に暗号資産マイナーへつながるマルウェア配布に使われていたとされています。
キャンペーンは「Yoba」と呼ばれ、複数の偽アプリ名を使って利用者を誘導していた可能性があります。
生成AI関連の人気サービス名を悪用した偽配布は、利用者の警戒心を下げやすく、業務端末への侵入や不要な負荷発生につながるおそれがあります。
開発者や一般利用者が信頼しやすい公開リポジトリ経由でも、配布物の確認が必要であることを示す事例です。

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

- GitHub上の配布物は、発行元・リリース内容・署名やハッシュの整合性を確認してから導入する。
- ChatGPTやClaudeなどを名乗る非公式デスクトップアプリは、社内端末での実行可否を慎重に扱う。
- 不審な圧縮ファイルや新規導入アプリの実行後は、端末のCPU高負荷や不審なプロセス、ネットワーク通信を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Check Point | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | ChatGPT | 主題 | 0.80 | — |
| AIモデル/プロジェクト | Claude | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Yoba malware hides in fake desktop versions of ChatGPT and Claude](https://www.helpnetsecurity.com/2026/10/29/fake-chatgpt-claude-apps-github-yoba-malware-cryptominer/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-40399"></a>

### 8. IR trends Q3 2026: Actors impersonate IT help desks in vishing attacks as ransomware activity increases

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Cisco TalosのQ3 2026インシデント傾向では、フィッシングが引き続き主要な初期侵入手口であり、ランサムウェアおよびその前段階の事案の割合が増加したとされています。
特に、ITヘルプデスクを装う音声詐欺（vishing）が確認され、対象業種としては金融と行政機関が上位に並びました。
初期侵入の中心が継続してフィッシングにある一方で、ランサムウェア関連の比重が増している点が重要です。
実務上は、認証情報の窃取や正規サポートを装う連絡への対策が、被害抑止の鍵になりやすいことを示しています。

#### 温度感の理由

##### 温度感
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ITヘルプデスクを名乗る電話・チャット・メールに対して、本人確認手順を厳格化する。
- MFAの有効化だけでなく、初期侵入後の横展開や権限昇格を前提に、特権アカウント管理と監視を見直す。
- ランサムウェア前段の兆候を想定し、バックアップの分離保管と復旧手順の定期検証を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ランサムウェアグループ | Interlock | 主題 | 0.80 | — |
| ランサムウェアグループ | The Gentlemen | 主題 | 0.80 | — |
| ランサムウェアグループ | Rhysida | 主題 | 0.80 | — |
| ランサムウェアグループ | Conti | 主題 | 0.80 | — |
| ランサムウェアグループ | Qilin | 主題 | 0.80 | — |
| 脅威アクター | Salt Typhoon | 主題 | 0.80 | — |
| ベンダー | Anthropic | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [IR trends Q3 2026: Actors impersonate IT help desks in vishing attacks as ransom](https://blog.talosintelligence.com/ir-trends-q3-2026/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-40432"></a>

### 9. New Cisco firewall zero-day exploited to crash SSL VPN devices

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Ciscoは、ASAおよびFTDソフトウェアに存在するゼロデイ脆弱性に対する更新を公開し、攻撃者が脆弱なファイアウォール機器をリモートでクラッシュさせていると案内しました。
現時点では、対象はSSL VPN機能を持つ機器へのサービス妨害が中心とみられますが、被害状況や影響範囲は環境によって異なる可能性があります。
境界防御機器が停止すると、VPN接続やネットワークの可用性に直接影響し、業務停止につながりやすいためです。
しかも悪用が観測されているため、通常の脆弱性公表よりも早い対応が求められます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 検知、監視、SOC/CSIRT運用、環境への適用可否を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Cisco ASA/FTDの該当バージョンを使っているかを確認し、ベンダーの修正版適用を優先する。
- SSL VPNを含む外部公開インターフェースの監視を強化し、再起動・異常終了・接続断の兆候を点検する。
- パッチ適用までの間は、不要な公開範囲の縮小やアクセス制御の見直しなど、影響を抑える暫定対策を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-76418 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Adaptive Security Appliance | 言及あり | 0.80 | — |
| 製品 | Cisco Firepower Threat Defense | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New Cisco firewall zero-day exploited to crash SSL VPN devices](https://www.bleepingcomputer.com/news/security/cisco-warns-of-firewall-zero-day-exploited-to-crash-ssl-vpn-devices/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-40319"></a>

### 1. Chinese Hackers Quietly Used Low-Severity ESXi Logging Flaw as Zero-Day

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 51.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

CVE-2026-41709は、BroadcomのVMware ESXi/ESXに影響するログ記録の不備で、悪用されると一部の操作が監査ログに残りにくくなるとされています。
公開情報によれば、China-nexusの脅威アクターによる実際の悪用が確認され、CISAのKEVカタログにも追加されました。
仮に深刻度が比較的低く見えても、監査証跡を弱める欠陥は侵害の発見や追跡を難しくするため、運用上の影響が大きくなり得ます。
特に仮想化基盤は多くのシステムの土台になるため、優先的な確認対象になります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- VMware ESXi/ESXの該当バージョンと修正状況を確認し、パッチ適用を優先する。
- 管理者権限を持つアカウントの利用状況や不審な操作の有無を点検し、監査ログの収集・保全を強化する。
- 仮想化基盤への管理アクセスを最小化し、MFAやアクセス制御、管理ネットワークの分離を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-41709 | 関連CVE | 1.00 | 未確認 |
| ベンダー | CrowdStrike | 言及あり | 0.80 | — |
| ベンダー | Broadcom | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Linux kernel | 言及あり | 0.80 | — |
| 製品 | VMware ESXi | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-41709](https://nvd.nist.gov/vuln/detail/CVE-2026-41709) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Chinese hackers used VMware ESX zero-day; PHP2Shell and Fragnesia chained to roo](https://www.helpnetsecurity.com/2026/10/29/php2shell-fragnesia-vmware-esx-zero-day/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Chinese Hackers Quietly Used Low-Severity ESXi Logging Flaw as Zero-Day](https://www.securityweek.com/chinese-hackers-quietly-used-low-severity-esxi-logging-flaw-as-zero-day/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [China-Linked Hackers Exploited VMware ESX Zero-Day to Reduce Audit Trail Visibil](https://thehackernews.com/2026/10/china-linked-hackers-exploited-vmware.html) | <nobr>内容確認・補足情報</nobr> |

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
| [米国選挙の安全性とは？投票機のリスクと拡大するAIの脅威](https://www.securityweek.com/how-secure-are-us-elections-voting-machine-risks-and-the-growing-threat-of-ai/) | 33.0 | 20.0 | 42.0 |
| [NIK C2マルウェアが被害者のOpenAIキーをAIクエリに悪用可能](https://www.infosecurity-magazine.com/news/nik-c2-malware-victims-openai-keys/) | 33.0 | 20.0 | 42.0 |
| [「EDR無効化」「暗号化はしない」 2026年のランサムウェアに起きた変化](https://atmarkit.itmedia.co.jp/ait/articles/2610/29/news019.html) | 29.0 | 30.0 | 42.0 |
| [BYODサイバー攻撃でUniversity of New Mexicoの救急車が迂回し授業が中止に](https://www.fortra.com/blog/byod-cyberattack-diverts-ambulances-and-cancels-classes-university-new-mexico-health-center) | 28.0 | 30.0 | 42.0 |
| [Chrome拡張機能13.4百万件が検索を乗っ取りしていることが判明](https://www.bleepingcomputer.com/news/security/chrome-extensions-with-134-million-installs-caught-hijacking-searches/) | 28.0 | 20.0 | 42.0 |
| [Volt Typhoonが変化し続ける「Silent Train」中継ネットワークを通じて企業の制御プレーンを標的化](https://www.helpnetsecurity.com/2026/10/29/volt-typhoon-silent-train-relay-network/) | 28.0 | 20.0 | 42.0 |
| [Cloudflare DDoS脅威レポート 2026年第3四半期：より多くのスウォーム、より少ない巨大攻撃](https://blog.cloudflare.com/ddos-threat-report-2026-q3/) | 28.0 | 20.0 | 42.0 |
| [AttackersがGitHub Issuesを悪用し、1時間足らずで61の公開リポジトリを標的にしたサプライチェーン攻撃](https://www.theregister.com/security/2026/10/29/attackers-turn-github-issues-into-supply-chain-campaign-against-61-public-repos-in-less-than-an-hour/5306153) | 28.0 | 20.0 | 42.0 |
| [MR ROBOT Malware-as-a-Serviceがインドの銀行顧客を標的にする](https://www.infosecurity-magazine.com/news/robot-malware-indian-bank-customers/) | 28.0 | 20.0 | 42.0 |
| [HackersがCisco SD-WANの脆弱性を悪用し、暗号鍵を窃取するマルウェアを仕込んだ](https://thehackernews.com/2026/10/hackers-exploited-cisco-sd-wan-flaw-to.html) | 28.0 | 20.0 | 42.0 |
| [Unknown APTがNetamLoaderを用いてアジアの政府向けにカスタマイズされたWindows 10 OSを攻撃](https://securelist.com/netamloader/121676/) | 28.0 | 20.0 | 42.0 |
| [OpenCodeユーザーが無料AIの抜け穴を報告した後に激しい反発を受ける](https://socket.dev/blog/opencode-free-usage-bypass) | 27.0 | 20.0 | 42.0 |
| [NIK C2：新たなAI対応コマンド＆コントロールフレームワーク](https://blog.talosintelligence.com/nik-c2-new-ai-enabled-framework/) | 27.0 | 20.0 | 42.0 |
| [AIのコード解析を妨害するために「天安門事件」「台湾独立」「水道水に毒物混入」などのフレーズを大量に混入させる手法が発見される](https://gigazine.net/news/20261029-anti-ai-words-in-script/) | 25.0 | 20.0 | 43.0 |
| [Claudeモデルが主要ブラウザとOS向けのエクスプロイトを作成](https://www.darkreading.com/application-security/claude-model-exploits-major-browsers-oses) | 25.0 | 20.0 | 42.0 |
| [JPMorgan ChaseとGoldman Sachsが示すAI計画におけるセキュリティ強化の重要性](https://www.cybersecuritydive.com/news/jpmorgan-chase-goldman-sachs-AI-security/873171/) | 25.0 | 20.0 | 42.0 |
| [Google、Gemini 4 Carbonモデルの強力なサイバーセキュリティ機能をアピール](https://www.securityweek.com/google-says-gemini-4-carbon-leads-in-finding-exploiting-and-fixing-vulnerabilities/) | 25.0 | 20.0 | 42.0 |
| [Agentic攻撃の台頭：その実態と今後の展望](https://www.wiz.io/blog/the-rise-of-agentic-attacks-what-they-look-like-and-where-theyre-headed) | 25.0 | 20.0 | 42.0 |
| [Cisco、無害な手順に潜むAIエージェント攻撃を検知するQuarryをオープンソース化](https://www.securityweek.com/cisco-open-sources-quarry-to-catch-ai-agent-attacks-hidden-in-harmless-steps/) | 25.0 | 20.0 | 42.0 |
| [VS Code、Cursor、Copilot、Codex、Claude Desktop内蔵ブラウザの脆弱性を研究者が解明](https://www.helpnetsecurity.com/2026/10/29/research-ai-assistant-browser-vulnerabilities/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントはすでにブラウザー内で動作している3つの方法](https://www.bleepingcomputer.com/news/security/3-ways-ai-agents-already-operate-in-your-browser/) | 25.0 | 20.0 | 42.0 |
| [GoogleのGemini 4 Carbonが脆弱性の発見・悪用・修正ベンチマークで首位に立つ](https://thehackernews.com/2026/10/googles-gemini-4-carbon-leads.html) | 25.0 | 20.0 | 42.0 |
| [Threat Operatorの台頭：AIがセキュリティ運用とキャリアをどう再定義するか](https://thehackernews.com/2026/10/the-rise-of-threat-operator-how-ai-will.html) | 25.0 | 20.0 | 42.0 |
| [公開Giteeリポジトリで26,400件の有効なクラウド・AI認証情報が露出していた件](https://thehackernews.com/2026/10/26400-valid-cloud-and-ai-credentials.html) | 25.0 | 20.0 | 42.0 |
| [Shadowy AI RelayがOpenAI CodexとClaude Codeのサンドボックスを無効化](https://www.darkreading.com/threat-intelligence/ai-relay-service-openai-codex-claude-code-sandboxes) | 25.0 | 20.0 | 42.0 |
| [Sandboxが「Danger-Full-Access」に反転：不正なAIリレーが組織にリスクをもたらす](https://www.security.com/threat-intelligence/openai-claude-unauthorized-relays) | 25.0 | 20.0 | 42.0 |
| [Hitachi Energy TRO600シリーズ製品](https://www.cisa.gov/news-events/ics-advisories/icsa-26-302-02) | 24.0 | 46.0 | 50.0 |
| [Hitachi Energy CoreTec製品の脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-302-03) | 24.0 | 46.0 | 50.0 |
| [CISA、PHP2Shell攻撃で悪用されるFragnesiaのLinux脆弱性に警告](https://www.bleepingcomputer.com/news/security/cisa-warns-of-fragnesia-linux-flaw-chained-in-php2shell-attacks/) | 22.0 | 32.0 | 42.0 |
| [Adobe、Veeam、Juniper Networksが重大な脆弱性を修正](https://www.securityweek.com/adobe-veeam-juniper-networks-patch-critical-vulnerabilities/) | 22.0 | 32.0 | 42.0 |
| [IDC MarketScape、2026年世界の企業向けモダンエンドポイントセキュリティベンダー評価でMicrosoftをリーダーに選出](https://www.microsoft.com/en-us/security/blog/2026/10/29/idc-marketscape-names-microsoft-a-leader-in-the-2026-worldwide-modern-endpoint-security-for-enterprises-vendor-assessment/) | 22.0 | 20.0 | 42.0 |
| [従業員の個人情報が流出した可能性 - ドトールコーヒー](https://www.security-next.com/192077) | 22.0 | 20.0 | 42.0 |
| [不正アクセスで電子ギフトが不正発行 - ギフティ](https://www.security-next.com/191987) | 22.0 | 20.0 | 42.0 |
| [会員サイトやアプリにPWリスト攻撃 - 富士急ハイランド](https://www.security-next.com/192167) | 22.0 | 20.0 | 42.0 |
| [PHPの脆弱性悪用で日本含む4カ国のサーバ25台が侵害か、JPCERT/CCが追加警告](https://news.mynavi.jp/techplus/article/20261029-5217835/) | 21.0 | 20.0 | 42.0 |
| [不正アクセスによる漏えい人数、半年余りでのべ2億6000万人に 日本人口の2倍超](https://www.itmedia.co.jp/news/article/2610/29/2000002730/) | 21.0 | 20.0 | 42.0 |
| [楽天カード、本人認証をワンタイムパスワードに統一 27年2月から順次](https://www.itmedia.co.jp/news/article/2610/29/2000002729/) | 21.0 | 20.0 | 42.0 |
| [Linux KernelのTCP脆弱性、CVSS 9.8でUbuntuやRed Hatなどに影響](https://thehackernews.com/2026/10/linux-kernel-tcp-flaw-with-98-cvss.html) | 20.0 | 28.0 | 50.0 |
| [悪意のあるFirefox拡張機能が人気の暗号資産ウォレットを装う](https://www.malwarebytes.com/blog/news/2026/10/malicious-firefox-extensions-impersonate-popular-crypto-wallets) | 20.0 | 20.0 | 48.0 |
| [リスクが個人的なものになったとき：がんの診断からセキュリティリーダーが学べること](https://www.securityweek.com/when-risk-becomes-personal-what-security-leaders-can-learn-from-a-cancer-diagnosis/) | 20.0 | 20.0 | 42.0 |
| [連邦破産裁判所契約業者、サイバー侵入でデータ流出はなかったと説明](https://therecord.media/us-bankruptcy-courts-it-contractor-says-no-data-stolen-cyberattack) | 20.0 | 20.0 | 42.0 |
| [ホワイトボードで4つの質問を使った脅威モデリング](https://www.darkreading.com/cyber-risk/threat-modeling-4-simple-questions) | 20.0 | 20.0 | 42.0 |
| [ベルギー税務当局、サイバー攻撃を確認しサービスを停止](https://www.theregister.com/security/2026/10/29/belgiums-tax-agency-confirms-cyberattack-pulls-services-offline/5306409) | 20.0 | 20.0 | 42.0 |
| [Microsoft、最近のWindows更新で発生したRemote Desktopの接続障害を修正](https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-remote-desktop-failures-caused-by-recent-windows-updates/) | 20.0 | 20.0 | 42.0 |
| [CRESTが呼びかける金融サイバー防御のエコシステム全体での強化](https://www.infosecurity-magazine.com/news/crest-financial-cyber-resilience/) | 20.0 | 20.0 | 42.0 |
| [申告期限前にBelgiumの税務サービスを妨害したサイバー攻撃](https://therecord.media/cyberattack-disrupts-belgian-tax-services-before-deadline) | 20.0 | 20.0 | 42.0 |
| [University of New Mexico、病院システムを復旧し、ハッカーへの接触を控えるよう呼びかけ](https://therecord.media/new-mexico-cyberattack-hospital) | 20.0 | 20.0 | 42.0 |
| [BAE、破産裁判所を狙ったインシデントでデータ流出はなしと発表](https://www.securityweek.com/bae-says-no-data-extracted-in-incident-hitting-bankruptcy-courts/) | 20.0 | 20.0 | 42.0 |
| [41,000件超のDHS職員記録がオンラインで流出](https://www.securityweek.com/over-41000-dhs-employee-records-leaked-online/) | 20.0 | 20.0 | 42.0 |
| [GoogleがGemini 4 Carbonでセキュリティ脆弱性の発見と修正を強化](https://www.helpnetsecurity.com/2026/10/29/google-gemini-4-carbon-model/) | 20.0 | 20.0 | 42.0 |
| [英国の16歳未満向けSNS禁止に備えた年齢確認候補、成人の一部にも本人確認が必要に](https://www.theregister.com/security/2026/10/29/shortlist-of-age-checks-for-the-uks-under-16-social-media-ban-is-out-some-adults-will-need-verifying/5306282) | 20.0 | 20.0 | 42.0 |
| [Ubuntu Core Desktopが再登場、Canonicalの不変型デフォルトデスクトップ構想](https://www.helpnetsecurity.com/2026/10/29/canonical-ubuntu-core-desktop/) | 20.0 | 20.0 | 42.0 |
| [攻撃者は顧客をハッキングしているのではなく、あなたを装っている](https://www.akamai.com/blog/security/2026/oct/attackers-hacking-your-customers-impersonating-you) | 20.0 | 20.0 | 42.0 |
| [Telegram Androidの脆弱性により、ユーザーが音声通話に応答するとコードが実行される可能性](https://thehackernews.com/2026/10/telegram-android-flaw-lets-attackers.html) | 20.0 | 20.0 | 42.0 |
| [オンライン詐欺の件数が倍増し、フィッシングを上回る](https://www.infosecurity-magazine.com/news/online-scam-volumes-double/) | 20.0 | 20.0 | 42.0 |
| [Sonyの日本ISP So-netから260万件の記録を窃取したハッカーたち](https://www.securityweek.com/hackers-steal-2-6-million-records-from-sonys-japanese-isp-so-net/) | 20.0 | 20.0 | 42.0 |
| [ICO、家庭内暴力の情報漏えいを受けてStaffordshire Policeを厳重注意](https://www.infosecurity-magazine.com/news/ico-reprimand-staffordshire-police/) | 20.0 | 20.0 | 42.0 |
| [GitHub、インストール前に悪意のあるパッケージをブロックするnpm Firewallを公開](https://thehackernews.com/2026/10/github-launches-npm-firewall-to-block.html) | 20.0 | 20.0 | 42.0 |
| [量子リスクの高まりを受けて見直しが迫られる公開鍵基盤](https://www.itpro.com/security/encryption/security-leaders-brace-for-an-overhaul-of-public-key-infrastructure-as-quantum-risks-rise) | 20.0 | 20.0 | 42.0 |
| [ハクティビストがDHS職員4万1000人分の記録を流出、潜入中のICE捜査官が判明](https://www.helpnetsecurity.com/2026/10/29/icepick-dhs-leak-ice-undercover-agents/) | 20.0 | 20.0 | 42.0 |
| [NISTが連邦政府の耐量子計算期限に対応するためのガイダンスを公開](https://www.infosecurity-magazine.com/news/nist-guidance-post-quantum/) | 20.0 | 20.0 | 42.0 |
| [管理者がパスワードにF-wordを入れて、ハッカーに自分が本当に1337であることを示した](https://www.theregister.com/security/2026/10/29/admin-dropped-the-f-bomb-in-a-password-to-show-hackers-who-was-really-1337/5306139) | 20.0 | 20.0 | 42.0 |
| [HHSへの提出でiRhythmのデータ侵害件数が820万人に拡大](https://www.securityweek.com/hhs-filing-puts-irhythm-data-breach-toll-at-8-2-million/) | 20.0 | 20.0 | 42.0 |
| [「グッドスマイルカンパニー公式ショップ」、決済ページの改ざんでクレジットカード情報を含む個人情報が漏えいの可能性](https://internet.watch.impress.co.jp/docs/news/2152332.html) | 20.0 | 20.0 | 42.0 |
| [グッスマ、顧客の2800人のカード番号全16桁＋セキュリティコードなど流出か 下4桁は40万枚分](https://www.itmedia.co.jp/news/article/2610/29/2000002716/) | 16.0 | 20.0 | 42.0 |

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
