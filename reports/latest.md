# 📡 サイレーダー 2026-06-02 05:00 JST

このレポートは、2026-06-01 17:00 JST〜2026-06-02 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 98
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 61

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-0826: Critical unauthenticated stack buffer overflow in HP Poly VVX and Trio VoIP Phones (FIXED)](#topic-13423) | 48.0 | 74.0 | 52.0 | 音声 | 温度感上位枠 |
| 2 | [Hackers are exploiting Palo Alto GlobalProtect VPN authentication bypass (CVE-2026-0257)](#topic-4247) | 48.0 | 67.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [Critical WP Maps Pro Flaw Actively Exploited to Create Admin Accounts](#topic-13474) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Windows Netlogon RCE exploited, domain controllers at risk (CVE-2026-41089)](#topic-3744) | 37.0 | 64.0 | 65.0 | 音声 | 温度感上位枠 |
| 5 | [CVE-2024-21182: CISA KEV catalog addition](#topic-13437) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 6 | [Iranian Threat Actor Nimbus Manticore Expands Wartime Cyber Operations with AI-Assisted Malware and SEO Poisoning](#topic-13389) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [CVE-2026-0826: How an Old Bug Can Feed AI-Powered Impersonation](#topic-13424) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-13423"></a>

### 1. CVE-2026-0826: Critical unauthenticated stack buffer overflow in HP Poly VVX and Trio VoIP Phones (FIXED)

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>RCE</nobr> / <nobr>政策・規制</nobr> / <nobr>防御・運用</nobr> / <nobr>ゼロデイ</nobr> / <nobr>権限昇格</nobr> / <nobr>Linux</nobr> / <nobr>PoC</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 48.0 |
| <nobr>実務影響</nobr> | 74.0 |
| <nobr>確度</nobr> | 52.0 |

#### 概要

HP PolyのVVXシリーズおよびTrio IP Conferenceシリーズの一部機種に、認証不要のスタックバッファオーバーフロー脆弱性CVE-2026-0826が公表されました。
条件がそろうと遠隔からコード実行につながる可能性があるとされ、ベンダーは修正版ファームウェアの適用と、不要な環境ではICE接続機能を無効にするよう案内しています。
音声通話用端末は社内ネットワークの入口や会議システムに置かれることが多く、影響を受けると端末乗っ取りや横展開の起点になり得ます。
公開PoCや検証コードの言及があるため、対応の遅れがリスクに直結しやすい点も注目されています。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 公開PoC・検証コード言及あり。
- 公開PoC/Exploitコード: 確認あり。
- 直接PoCリンク: 掲載しません。
- 確認方針: NVD、ベンダー公式、公的機関、信頼できる技術分析を優先し、GitHub等のコードは防御・検証目的で別途確認します。

#### 担当者向け確認ポイント

- 対象機種と現在のファームウェア版を確認し、ベンダー案内の修正版へ更新する。
- 不要な場合はICE接続機能を無効化し、利用環境での有効化状況を点検する。
- VoIP端末の管理セグメントやSIP関連通信を監視し、想定外の挙動や再起動の増加がないか確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-0826 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-0826](https://nvd.nist.gov/vuln/detail/CVE-2026-0826) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0826: Critical unauthenticated stack buffer overflow in HP Poly VVX and](https://www.rapid7.com/blog/post/ve-cve-2026-0826-critical-unauthenticated-stack-buffer-overflow-hp-poly-vvx-trio-voip-phones-fixed) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。

---

<a id="topic-4247"></a>

### 2. Hackers are exploiting Palo Alto GlobalProtect VPN authentication bypass (CVE-2026-0257)

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>IoC</nobr> / <nobr>認証バイパス</nobr> / <nobr>KEV</nobr> / <nobr>防御・運用</nobr> / <nobr>脅威アクター</nobr> / <nobr>Windows</nobr> / <nobr>Linux</nobr> / <nobr>政策・規制</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 冷却中 |
| <nobr>温度感</nobr> | 48.0 |
| <nobr>実務影響</nobr> | 67.0 |
| <nobr>確度</nobr> | 66.0 |

#### 概要

Palo Alto NetworksのPAN-OSおよびPrisma Accessに存在する認証バイパスの脆弱性CVE-2026-0257について、実際の悪用が確認されたと複数の報道・分析で伝えられています。
条件に合う構成では、GlobalProtectのVPN接続が不正に成立する可能性があるとされていますが、被害の広がりや内部侵入の有無は環境によって異なります。
インターネット公開のVPN機器で認証を回避されると、社内ネットワークへの入口を直接与えかねないため、影響は小さくありません。
CISAの既知悪用脆弱性カタログにも追加されており、修正適用と設定確認が急がれる案件です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 7 sources。
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
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 技術詳細、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 対象バージョンかどうかを確認し、ベンダー提供の修正済み版へ速やかに更新する。
- GlobalProtectのauthentication override機能の有効化有無と、証明書の使い回しがないかを点検する。
- 認証ログを確認し、不審なCookie認証や見覚えのないホスト名・送信元IPの痕跡がないかを調べる。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-0257 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |
| ベンダー | Palo Alto | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-0257](https://nvd.nist.gov/vuln/detail/CVE-2026-0257) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Recent Palo Alto Networks Vulnerability Exploited for Weeks](https://www.securityweek.com/recent-palo-alto-networks-vulnerability-exploited-for-weeks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers are exploiting Palo Alto GlobalProtect VPN authentication bypass (CVE-20](https://www.helpnetsecurity.com/2026/06/01/hackers-are-exploiting-palo-alto-globalprotect-vpn-authentication-bypass-cve-2026-0257/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Palo Alto GlobalProtect VPN auth bypass flaw now exploited in attacks](https://www.bleepingcomputer.com/news/security/palo-alto-globalprotect-vpn-auth-bypass-flaw-now-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PAN-OS GlobalProtect Authentication Bypass (CVE-2026-0257) Under Active Exploita](https://thehackernews.com/2026/05/pan-os-globalprotect-authentication.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Rapid7 Observed Exploitation of PAN-OS GlobalProtect Authentication Bypass Vulne](https://www.rapid7.com/blog/post/etr-rapid7-observed-exploitation-of-pan-os-globalprotect-authentication-bypass-vulnerability-cve-2026-0257) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/05/29/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0257 PAN-OS: GlobalProtect Authentication Bypass Vulnerabilities (Sever](https://security.paloaltonetworks.com/CVE-2026-0257) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 技術詳細・悪用観測あり。

---

<a id="topic-13474"></a>

### 3. Critical WP Maps Pro Flaw Actively Exploited to Create Admin Accounts

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>脅威アクター</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 45.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

WordPressプラグイン「WP Maps Pro」に影響する重大な脆弱性について、悪用が観測されていると報じられています。
影響を受けるサイトでは、不正な管理者アカウントが作成されるおそれがあるとされています。管理者権限の奪取につながる可能性があるため、サイト改ざんや追加侵害の起点になり得ます。
WordPressサイトの運用者にとっては、公開直後から対策状況の確認が重要です。

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
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- WP Maps Proの利用有無を確認し、ベンダー提供の修正・対策情報を確認する。
- 不審な管理者アカウントや権限変更の有無を点検する。
- WordPress本体・プラグインの更新、不要な管理者権限の整理を優先する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Critical WP Maps Pro Flaw Actively Exploited to Create Admin Accounts](https://thehackernews.com/2026/06/critical-wp-maps-pro-flaw-actively.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-3744"></a>

### 4. Windows Netlogon RCE exploited, domain controllers at risk (CVE-2026-41089)

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>Windows</nobr> / <nobr>RCE</nobr> / <nobr>クラウド</nobr> / <nobr>DDoS</nobr> / <nobr>政策・規制</nobr> / <nobr>AI</nobr> / <nobr>IoC</nobr> / <nobr>Android</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 再燃 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 64.0 |
| <nobr>確度</nobr> | 65.0 |

#### 概要

Windows Netlogon に存在する CVE-2026-41089 は、ネットワーク経由でのリモートコード実行につながる脆弱性とされ、複数の公開情報で悪用観測が示されています。
特にドメインコントローラーが関わる環境では影響が大きく、優先的な対応が求められています。
認証基盤に関わる Netlogon の脆弱性は、ドメイン全体への影響に直結しやすいためです。
公開情報では実際の悪用が示唆されており、通常の高リスク脆弱性よりも早い確認と対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
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
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- ドメインコントローラーを含む Windows 環境で、関連パッチの適用状況を優先確認する。
- 外部から到達可能なサーバーや認証系サービスのログを見直し、不審な接続や異常な失敗を確認する。
- 資産影響が大きい場合は、脆弱性管理だけでなく検知・隔離・復旧手順を事前に点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-41089 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-41089](https://nvd.nist.gov/vuln/detail/CVE-2026-41089) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Critical Windows Netlogon Vulnerability in Attackers’ Crosshairs](https://www.securityweek.com/critical-windows-netlogon-vulnerability-in-attackers-crosshairs/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Windows Netlogon RCE exploited, domain controllers at risk (CVE-2026-41089)](https://www.helpnetsecurity.com/2026/06/01/windows-netlogon-rce-exploited-cve-2026-41089/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Patch Tuesday - May 2026](https://www.rapid7.com/blog/post/em-patch-tuesday-may-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Patch Tuesday, May 2026 Edition](https://krebsonsecurity.com/2026/05/patch-tuesday-may-2026-edition/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-41089 Windows Netlogon Remote Code Execution Vulnerability](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-41089) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-13437"></a>

### 5. CVE-2024-21182: CISA KEV catalog addition

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>KEV</nobr> / <nobr>CVE</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 46.0 |
| <nobr>確度</nobr> | 51.0 |

#### 概要

CISAは、Oracle WebLogic Serverに関連するCVE-2024-21182をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
公的な説明では、実際の悪用が確認されたことを根拠としており、対象製品を利用する組織では早急な確認が必要です。
KEVへの追加は、少なくとも一部環境で悪用が観測されていることを示すため、優先度の高い対応対象になります。
特に公開系のWebLogic環境を持つ組織では、影響範囲の把握と修正対応の遅れがリスクにつながります。

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
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Oracle WebLogic Serverの利用有無を確認し、該当バージョンや構成を棚卸しする。
- ベンダー情報とCISA KEVの情報を突き合わせ、該当環境があれば修正適用や緩和策を優先する。
- 外部公開された管理面や関連サービスの監視を強め、異常な挙動や侵入兆候がないか点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2024-21182 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2024-21182](https://nvd.nist.gov/vuln/detail/CVE-2024-21182) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/06/01/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-13389"></a>

### 6. Iranian Threat Actor Nimbus Manticore Expands Wartime Cyber Operations with AI-Assisted Malware and SEO Poisoning

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脅威アクター</nobr> / <nobr>地政学・サイバー紛争</nobr> / <nobr>マルウェア</nobr> / <nobr>TTP</nobr> / <nobr>通信基盤</nobr> / <nobr>国家支援</nobr> / <nobr>防御・運用</nobr> / <nobr>AI</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>フィッシング</nobr> |
| <nobr>分類理由</nobr> | AI×Security枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Nimbus Manticoreと呼ばれる脅威アクターが、AI支援型マルウェアやSEOポイズニングを含む新たな配布・潜伏手法を伴うサイバー活動を拡大したと報告されています。
航空、防衛、通信、ソフトウェア開発、政府関連など複数分野を対象に、フィッシングや改ざんされたインストーラ、永続化を狙う手法が使われたとされています。
戦時下の地政学的緊張と結びついた活動として、複数地域・複数業種にまたがる影響が想定されるため注目されます。
AIの利用や正規の業務活動に紛れ込む手口は、従来の検知や利用者教育だけでは見逃しやすく、組織側の対策見直しにつながります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ソフトウェア配布経路や更新プロセスの真正性確認を強化する。
- フィッシング、検索経由の誘導、正規ツールを装う配布物への警戒を高める。
- 永続化や不審なスケジュール実行、アプリ連携の異常を監視対象に含める。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Iranian Threat Actor Nimbus Manticore Expands Wartime Cyber Operations with AI-A](https://blog.polyswarm.io/iranian-threat-actor-nimbus-manticore-expands-wartime-cyber-operations-with-ai-assisted-malware-and-seo-poisoning) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-13424"></a>

### 7. CVE-2026-0826: How an Old Bug Can Feed AI-Powered Impersonation

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>AI</nobr> / <nobr>CVE</nobr> / <nobr>防御・運用</nobr> / <nobr>RCE</nobr> / <nobr>脅威アクター</nobr> / <nobr>フィッシング</nobr> / <nobr>国家支援</nobr> / <nobr>権限昇格</nobr> / <nobr>TTP</nobr> |
| <nobr>分類理由</nobr> | AI×Security枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Rapid7によると、HP Polyの複数のVoIP端末に、認証不要で悪用されうる重大なスタックベースのバッファオーバーフロー脆弱性CVE-2026-0826が確認されました。
影響を受ける機器は業務上の通話基盤として使われることが多く、端末への侵害が内部通信の盗聴やなりすまし関連のリスクにつながる可能性が指摘されています。
電話機や会議室の音声端末は見落とされやすい一方で、機密会話が集まる場所でもあります。
音声データがAIを使ったなりすましや詐欺に悪用されうる点からも、単なる端末障害にとどまらない影響が注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 影響を受けるHP Poly端末の有無を確認し、ベンダーの案内に従って修正や回避策を適用する。
- VoIP端末を“専用機器”ではなくネットワーク上の資産として扱い、管理対象・棚卸し対象に含める。
- 会議室や役員室など重要会話の場にある音声機器の配置と権限を見直し、不要な露出を減らす。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-0826 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [CVE-2026-0826: How an Old Bug Can Feed AI-Powered Impersonation](https://www.rapid7.com/blog/post/ve-cve-2026-0826-how-an-old-bug-can-feed-ai-powered-impersonation) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
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
| [Microsoft、ゼロデイ報告への反発を受けセキュリティ研究者を追及しない方針を表明](https://therecord.media/microsoft-says-it-will-not-pursue-security-researchers-disclosure) | 37.0 | 38.0 | 43.0 |
| [OpenAI Codexの認証トークンがcodexui-androidのnpmサプライチェーン攻撃で窃取される](https://thehackernews.com/2026/06/openai-codex-authentication-tokens.html) | 33.0 | 45.0 | 42.0 |
| [強固なガバナンスがなければ、企業はAI時代に信用格付けリスクを抱える](https://www.cybersecuritydive.com/news/ai-cyberattacks-credit-ratings-sp-analysis/821599/) | 33.0 | 20.0 | 42.0 |
| [Secure Code Warriorが開発者トレーニングをAI利用とコードリスクに結び付ける](https://www.helpnetsecurity.com/2026/06/01/secure-code-warrior-adaptive-learning-capability/) | 33.0 | 20.0 | 42.0 |
| [選挙への脅威は投票機ではなく選挙運動システムに集中している](https://cyberscoop.com/2026-election-cyber-threats-campaign-systems/) | 33.0 | 20.0 | 42.0 |
| [AttackersがChatGPTを狙うフィッシングキャンペーンで共有コンテンツを悪用](https://www.infosecurity-magazine.com/news/attackers-shared-content-chatgpt/) | 33.0 | 20.0 | 42.0 |
| [深刻なWindows NetlogonのRCE脆弱性、現在攻撃で悪用中](https://www.bleepingcomputer.com/news/microsoft/critical-windows-netlogon-remote-code-execution-flaw-now-exploited-in-attacks/) | 32.0 | 38.0 | 42.0 |
| [Miasmaのサプライチェーン攻撃、Red Hatのnpmパッケージを侵害し認証情報窃取ワームを展開](https://thehackernews.com/2026/06/miasma-supply-chain-attack-compromises.html) | 28.0 | 45.0 | 42.0 |
| [RedHatのnpmパッケージを標的としたサプライチェーン攻撃「Miasma」](https://www.wiz.io/blog/miasma-supply-chain-attack-targeting-redhat-npm-packages) | 28.0 | 30.0 | 42.0 |
| [オランダ警察が1700万台規模のボットネットを解体](https://www.securityweek.com/dutch-police-dismantle-massive-17-million-device-botnet/) | 28.0 | 20.0 | 42.0 |
| [WordPressマルウェアキャンペーンがSteamプロフィールにペイロードを隠す](https://www.bleepingcomputer.com/news/security/wordpress-malware-campaign-hides-payloads-in-steam-profiles/) | 28.0 | 20.0 | 42.0 |
| [Macからパスワード、アカウント、暗号資産を盗む偽BlueWallet](https://www.malwarebytes.com/blog/threat-intel/2026/06/fake-bluewallet-steals-passwords-accounts-and-crypto-from-macs) | 28.0 | 20.0 | 42.0 |
| [中国系攻撃グループの攻撃が活発化、Dragon Weaveがチェコと台湾を標的に](https://thehackernews.com/2026/06/china-aligned-groups-ramp-up-attacks.html) | 28.0 | 20.0 | 42.0 |
| [Horizon3.ai、脆弱性修正の優先順位付けと検証を行うRapid Responseを発表](https://www.helpnetsecurity.com/2026/06/01/horizon3-ai-rapid-response/) | 27.0 | 20.0 | 43.0 |
| [Flowiseの深刻な脆弱性により攻撃者がサーバーを完全制御可能に](https://www.infosecurity-magazine.com/news/flowise-mcp-rce-poc/) | 26.0 | 38.0 | 42.0 |
| [NVIDIA、AIエージェント向けPC半導体「RTX Spark」発表 Microsoftと連携](https://xtech.nikkei.com/atcl/nxt/news/24/03249/) | 26.0 | 20.0 | 42.0 |
| [ハッカーがMetaのAIサポートボットを悪用してInstagramアカウントを乗っ取る](https://krebsonsecurity.com/2026/06/hackers-used-metas-ai-support-bot-to-seize-instagram-accounts/) | 25.0 | 20.0 | 42.0 |
| [OpenAIが最も高性能なAIモデルの利用者により強力な認証を要求](https://www.helpnetsecurity.com/2026/06/01/yubico-openai-passkeys-requirements/) | 25.0 | 20.0 | 42.0 |
| [NetworkLensがネットワーク管理トラフィックに潜む脅威を検知できるよう拡張](https://www.helpnetsecurity.com/2026/06/01/netquest-networklens-dataset-portfolio/) | 25.0 | 20.0 | 42.0 |
| [週刊まとめ：新たなLinux脆弱性、PAN-OSの悪用、AI搭載攻撃、OAuthフィッシングなど](https://thehackernews.com/2026/06/weekly-recap-new-linux-flaw-pan-os.html) | 25.0 | 20.0 | 42.0 |
| [Insightが露出管理、パッチ運用、XDRを統合した単一サービスを提供](https://www.helpnetsecurity.com/2026/06/01/insight-managed-exposure-defense/) | 25.0 | 20.0 | 42.0 |
| [depthfirstが悪意ある依存関係に対するインストール前保護を追加](https://www.helpnetsecurity.com/2026/06/01/depthfirst-dependency-firewall/) | 25.0 | 20.0 | 42.0 |
| [PathSolutionsがNetOpsチーム向けにオンプレミスAIトラブルシューティングを提供](https://www.helpnetsecurity.com/2026/06/01/pathsolutions-totalview-ai/) | 25.0 | 20.0 | 42.0 |
| [Cato、エージェント型脅威研究で脆弱性保護時間を45分に短縮](https://www.helpnetsecurity.com/2026/06/01/cato-networks-agentic-threat-research/) | 25.0 | 20.0 | 42.0 |
| [Microsoft Entra Agent IDにおける不審なAIワークフローの調査：エージェントのユーザーアカウント](https://redcanary.com/blog/threat-detection/entra-id-ai-workflows-teams/) | 25.0 | 20.0 | 42.0 |
| [Hylandプラットフォームの革新、AIガバナンス、コンテキスト、エージェント監視に注力](https://www.helpnetsecurity.com/2026/06/01/hyland-platform-innovations/) | 25.0 | 20.0 | 42.0 |
| [Webinar明日開催：ネットワークインシデント対応におけるアラートから解決まで](https://www.bleepingcomputer.com/news/security/webinar-tomorrow-from-alert-to-resolution-in-network-incident-response/) | 25.0 | 20.0 | 42.0 |
| [戦場AI導入を進める米国防総省に軍指導者が慎重論](https://www.securityweek.com/as-the-pentagon-pushes-for-battlefield-ai-some-military-leaders-urge-caution/) | 25.0 | 20.0 | 42.0 |
| [Infosecurity Europe：AI SOCでもSOCアナリストは依然必要、セキュリティベンダーが指摘](https://www.infosecurity-magazine.com/news/ai-soc-still-need-analysts/) | 25.0 | 20.0 | 42.0 |
| [AI活用企業のためのデータセキュリティベストプラクティス4選](https://www.cybersecuritydive.com/spons/top-4-data-security-best-practices-for-the-ai-enabled-enterprise/820564/) | 25.0 | 20.0 | 42.0 |
| [NVIDIA、物理AIエージェント向けツール群を大規模にオープンソース化](https://www.helpnetsecurity.com/2026/06/01/nvidia-open-source-physical-ai-skills/) | 25.0 | 20.0 | 42.0 |
| [WP Maps Proの脆弱性を悪用したWordPressサイト乗っ取り攻撃](https://www.securityweek.com/wp-maps-pro-vulnerability-exploited-to-take-over-wordpress-sites/) | 24.0 | 46.0 | 50.0 |
| [元職員が個人情報を掲示板投稿、システム設定に不備も - 津田塾大](https://www.security-next.com/184944) | 22.0 | 20.0 | 42.0 |
| [個人情報含む文書を外部サイトに掲載、職員を処分 - 郡山広域消防](https://www.security-next.com/184749) | 22.0 | 20.0 | 42.0 |
| [19年前のLinuxカーネル脆弱性によりシステムがroot権限を取得される可能性](https://www.securityweek.com/19-year-old-linux-kernel-vulnerability-exposes-systems-to-root-access/) | 22.0 | 20.0 | 42.0 |
| [公開講座を案内する一斉メールで送信ミス - 東北学院大](https://www.security-next.com/185187) | 22.0 | 20.0 | 42.0 |
| [エフサス製サーバ管理ソフト「ServerView Agents for Windows」に複数脆弱性](https://www.security-next.com/185229) | 22.0 | 20.0 | 42.0 |
| [「JCB社員がインスタに社内資料を載せている」Xで画像拡散 同社「事実関係を調査中」](https://www.itmedia.co.jp/news/articles/2606/01/news120.html) | 21.0 | 20.0 | 42.0 |
| [コンテナの危機：コンテナ脱出からサプライチェーン攻撃まで](https://securelist.com/container-attack-vectors/120010/) | 20.0 | 45.0 | 42.0 |
| [Red Canary CFPトラッカー：2026年5月](https://redcanary.com/blog/news-events/red-canary-cfp-tracker-june-2026/) | 20.0 | 20.0 | 42.0 |
| [NSA、主要サイバーセキュリティ職の新任リーダーを選出](https://therecord.media/nsa-selects-new-leads-for-cyber-posts) | 20.0 | 20.0 | 42.0 |
| [Dashlaneパスワードマネージャーのユーザーがブルートフォース攻撃でロックアウトされる](https://www.bleepingcomputer.com/news/security/dashlane-password-manager-users-locked-out-by-brute-force-attacks/) | 20.0 | 20.0 | 42.0 |
| [USPSが郵便投票の変更を進める中、裁判所がトランプ氏の選挙命令を審理](https://cyberscoop.com/usps-mail-in-ballot-restrictions-trump-order/) | 20.0 | 20.0 | 42.0 |
| [Meta、ワールドカップ開幕前に詐欺対策を強化](https://www.helpnetsecurity.com/2026/06/01/meta-fifa-world-cup-scams/) | 20.0 | 20.0 | 42.0 |
| [Wiz API SPMで重大なAPI攻撃経路を排除する](https://www.wiz.io/blog/introducing-wiz-api-spm) | 20.0 | 20.0 | 42.0 |
| [CISA、Palo Alto Networksのファイアウォールの重大な脆弱性をKEVに追加、同社と研究者が悪用を警告](https://www.cybersecuritydive.com/news/palo-alto-networks-firewall-flaw-exploitation-cisa-kev/821598/) | 20.0 | 20.0 | 42.0 |
| [6月1日脅威インテリジェンスレポート](https://research.checkpoint.com/2026/1st-june-threat-intelligence-report/) | 20.0 | 20.0 | 42.0 |
| [Palo Altoの認証バイパス脆弱性が再び悪用中、今すぐ修正を](https://www.darkreading.com/threat-intelligence/patch-palo-alto-auth-bypass-bug-exploit) | 20.0 | 20.0 | 42.0 |
| [時間との競争：脆弱性アラートの迅速化が重要な理由](https://www.bleepingcomputer.com/news/security/race-against-time-why-faster-vulnerability-alerts-matter/) | 20.0 | 20.0 | 42.0 |
| [Brute-force攻撃によりDashlaneアカウントがロックアウト発生](https://www.helpnetsecurity.com/2026/06/01/dashlane-brute-force-attack-user-accounts/) | 20.0 | 20.0 | 42.0 |
| [Infosecurity Europe：CISOが大手スーパーマーケットへの大規模サイバー攻撃への対応を試す机上演習](https://www.infosecurity-magazine.com/news/infosecurity-europe-semperis/) | 20.0 | 20.0 | 42.0 |
| [Microsoft Defender Vulnerability Managementでより賢い露出スコアを実現](https://www.helpnetsecurity.com/2026/06/01/microsoft-defender-exposure-score-update/) | 20.0 | 20.0 | 42.0 |
| [Dragos、xIoTセキュリティ企業Phosphorusを買収](https://www.securityweek.com/dragos-acquires-xiot-security-firm-phosphorus/) | 20.0 | 20.0 | 42.0 |
| [NISTによるNational Vulnerability Databaseの管理失敗](https://www.helpnetsecurity.com/2026/06/01/nist-nvd-management-problems/) | 20.0 | 20.0 | 42.0 |
| [Security Growth Platform：MSPがvCISOツールを超えて進む理由](https://thehackernews.com/2026/06/the-security-growth-platform-why-msps.html) | 20.0 | 20.0 | 42.0 |
| [データセキュリティが注目を集める時代に](https://www.security.com/product-insights/data-security-moment) | 20.0 | 20.0 | 42.0 |
| [FSB系GamaredonがWindowsのデータストリームにワームを隠蔽](https://www.infosecurity-magazine.com/news/gamaredon-worm-ntfs-data-streams/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、Windowsセキュリティ更新プログラム KB5089549 のインストール問題を修正](https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-kb5089549-windows-security-update-install-issues/) | 20.0 | 20.0 | 42.0 |
| [DragosがPhosphorusを買収し拡張運用技術の保護を強化](https://www.helpnetsecurity.com/2026/06/01/dragos-phosphorus-acquisition/) | 20.0 | 20.0 | 42.0 |
| [Canvaが2億6000万人超のユーザー規模へ成長しながらセキュリティと生産性を高めた方法](https://www.cybersecuritydive.com/spons/how-canva-scaled-to-260m-users-while-elevating-security-and-productivity/821203/) | 20.0 | 20.0 | 42.0 |
| [あなたのスマホにクリーンアップが必要です](https://www.malwarebytes.com/blog/mobile/2026/06/your-phone-called-it-needs-a-cleanup) | 20.0 | 20.0 | 42.0 |

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
