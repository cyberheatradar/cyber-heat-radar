# 📡 サイレーダー 2026-06-17 05:00 JST

このレポートは、2026-06-16 17:00 JST〜2026-06-17 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 98
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 67

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability](#topic-4945) | 63.0 | 84.0 | 67.0 | 音声 | 温度感上位枠 |
| 2 | [Cisco discloses second exploited SD-WAN vulnerability in two weeks (CVE-2026-20262)](#topic-17402) | 43.0 | 46.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [CISA warns of another cPanel plugin flaw exploited in attacks](#topic-17677) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 4 | ['Lorem Ipsum' Malware Pivots to ClickFix Delivery](#topic-17623) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Cybercriminals mask malicious communications through Microsoft Teams relays](#topic-17631) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [TekStream launches Proactive Cyber Defense to counter AI-driven threats](#topic-17635) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-4945"></a>

### 1. Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 63.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 84.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Ciscoは、Catalyst SD-WAN Controllerおよび関連コンポーネントにおける認証回避の脆弱性「CVE-2026-20182」への修正を公開しました。
複数の公開情報では、限定的な標的型攻撃で悪用された可能性や、ゼロデイとして扱われている状況が示されています。
認証回避は、侵入の足がかりとして悪用された場合に管理基盤全体へ影響が及ぶおそれがあり、CVSS 10.0とされる点でも重く見られています。
SD-WANは通信経路の制御に関わるため、影響範囲が広がりやすいことから、運用側の迅速な対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 9 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
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

- Ciscoの修正状況を確認し、対象製品・対象バージョンが残っていないか優先的に棚卸しする。
- ベンダーが示す確認手順やIOC関連の案内があれば、管理面の異常や不審な接続痕跡を点検する。
- SD-WAN管理系は外部公開やアクセス経路を最小化し、修正適用まで監視を強める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20182 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20182](https://nvd.nist.gov/vuln/detail/CVE-2026-20182) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-rpa2-v69WY2SW) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN V](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-privesc-4uxFrdzx) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Metasploit Wrap Up 05/22/2026](https://www.rapid7.com/blog/post/pt-metasploit-wrap-up-05-22-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco zero-day under ongoing attack by persistent threat group](https://cyberscoop.com/cisco-sd-wan-zero-day-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco patches another actively exploited SD-WAN zero-day (CVE-2026-20182)](https://www.helpnetsecurity.com/2026/05/15/cisco-sd-wan-zero-day-cve-2026-20182/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Patches Another SD-WAN Zero-Day, the Sixth Exploited in 2026](https://www.securityweek.com/cisco-patches-another-sd-wan-zero-day-the-sixth-exploited-in-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds Cisco SD-WAN CVE-2026-20182 to KEV After Admin Access Exploits](https://thehackernews.com/2026/05/cisa-adds-cisco-sd-wan-cve-2026-20182.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 要確認候補あり。

---

<a id="topic-17402"></a>

### 2. Cisco discloses second exploited SD-WAN vulnerability in two weeks (CVE-2026-20262)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Ciscoは、Catalyst SD-WAN Manager（旧SD-WAN vManage）の脆弱性CVE-2026-20262に対する修正を公開しました。
公開情報では、この問題は認証済みの攻撃者による不正なファイル作成・上書きにつながる可能性があり、実際に悪用が観測されたとされています。
SD-WAN管理基盤はネットワーク運用の中枢に当たるため、侵害されると影響範囲が大きくなり得ます。
しかも短期間でCisco製SD-WAN関連の悪用事例が続いており、管理系機器の優先的な点検が求められます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
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

- Ciscoの該当セキュリティアドバイザリを確認し、対象バージョンの更新状況を点検する。
- Catalyst SD-WAN Managerの管理アクセス権限を見直し、不要なアカウントや過剰権限がないか確認する。
- 管理系機器の監査ログを確認し、不審なファイル操作やAPI呼び出しの痕跡がないか点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20262 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20262](https://nvd.nist.gov/vuln/detail/CVE-2026-20262) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco discloses second exploited SD-WAN vulnerability in two weeks (CVE-2026-202](https://www.helpnetsecurity.com/2026/06/16/cisco-sd-wan-cve-2026-20262-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Patches Another SD-WAN Zero-Day Exploited in Attacks](https://www.securityweek.com/cisco-patches-another-sd-wan-zero-day-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Releases Security Updates for Actively Exploited SD-WAN Manager Flaw](https://thehackernews.com/2026/06/cisco-releases-security-updates-for.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Manager Arbitrary File Write Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-arbfw-c2rZvQ) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco fixes SD-WAN vManage flaw exploited in zero-day attacks](https://www.bleepingcomputer.com/news/security/cisco-fixes-sd-wan-vmanage-flaw-exploited-in-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 要確認候補あり。

---

<a id="topic-17677"></a>

### 3. CISA warns of another cPanel plugin flaw exploited in attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

CISAは、LiteSpeedのcPanel向けユーザーエンドプラグインに存在するCVE-2026-54420について、攻撃で悪用されているとして注意喚起しました。
米政府機関には短期間での対策が求められており、cPanel関連環境を運用する組織も影響範囲の確認が必要です。
公的機関が実際の悪用を前提に警告しているため、単なる脆弱性情報よりも緊急性が高い話題です。管理対象のサーバーやホスティング環境に該当する場合、迅速な対応が求められます。

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

- cPanelおよびLiteSpeed関連コンポーネントの利用有無を確認し、該当バージョンや適用状況を点検する。
- ベンダーや公的機関の案内に従い、修正パッチや緩和策の適用状況を早急に確認する。
- 外部公開している管理画面や関連サービスについて、監視強化と不審な挙動の確認を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-54420 | 主要CVE | 1.00 |
| ベンダー | cPanel | 言及あり | 0.80 |
| 製品 | cPanel | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-54420](https://nvd.nist.gov/vuln/detail/CVE-2026-54420) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA warns of another cPanel plugin flaw exploited in attacks](https://www.bleepingcomputer.com/news/security/cisa-warns-of-another-actively-exploited-cpanel-plugin-flaw/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17623"></a>

### 4. 'Lorem Ipsum' Malware Pivots to ClickFix Delivery

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

「Lorem Ipsum」と呼ばれるマルウェアの配布手口が、ClickFixを用いる形に変化していると分析されています。
公開情報では、侵害されたWordPressサイトが使われており、この活動はランサムウェア／データ恐喝グループのVice Societyとの関連が示唆されています。
正規サイトの改ざんや侵害済みWebサイトを経由するため、利用者や組織側で気づきにくい点が注意点です。
ランサムウェア文脈の脅威として、初期侵入の経路や偽装の手口が変化している可能性があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- WordPressサイトや関連Web資産の改ざん有無、不要な挙動の監視を強化する。
- 不審な誘導や認証・確認を促す画面が出た場合は、安易に操作せずユーザー報告経路へ回す。
- ランサムウェア関連の兆候として、周辺のログ・エンドポイント・Webアクセスの相関確認を行う。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | ['Lorem Ipsum' Malware Pivots to ClickFix Delivery](https://www.darkreading.com/cyberattacks-data-breaches/lorem-ipsum-malware-clickfix-delivery) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17631"></a>

### 5. Cybercriminals mask malicious communications through Microsoft Teams relays

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Symantecの観測によると、DragonForce系の侵入事例で、カスタムマルウェア「Backdoor.Turn」を使い、Microsoft Teamsの中継基盤を経由してコマンド＆コントロール通信を隠していたとされています。
DragonForceはランサムウェア・アズ・ア・サービス型のグループとされ、今回の件は正規の業務通信基盤が悪用される可能性を示すものです。
正規サービスを悪用して通信を紛れ込ませる手口は、検知や遮断を難しくするため注目されます。特にランサムウェア関連の侵入では、初期侵入後の内部通信の監視・可視化が重要になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Microsoft Teamsなど正規クラウドサービス由来の通信でも、通常と異なる認証・接続パターンがないか確認する。
- エンドポイントとクラウド側のログを突き合わせ、通信の宛先やタイミングに不自然な点がないか監視する。
- ランサムウェア対策として、権限分離、MFA、EDRの検知ルール見直しを継続する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Cybercriminals mask malicious communications through Microsoft Teams relays](https://www.helpnetsecurity.com/2026/06/16/dragonforce-microsoft-teams-malware-backdoor-turn/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17635"></a>

### 6. TekStream launches Proactive Cyber Defense to counter AI-driven threats

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

TekStreamは、同社のサイバー防御インテリジェンス基盤「Cosmos」を活用した新サービス「TekStream Proactive Cyber Defense」を発表しました。
背景には、AIで加速する攻撃や自律的な攻撃能力の拡大、運用の複雑化とセキュリティ環境の分断があるとされています。
AIを前提にした攻撃が現実的なリスクとして意識される中、検知だけでなく予防や継続的な防御支援を打ち出す動きとして注目されます。
自動化された攻撃や変化の速い脅威に対し、運用面でどう備えるかを考える材料になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI関連の脅威は、従来の検知中心の運用だけでは追いつかない可能性があるため、監視・対応プロセスの見直しが必要です。
- セキュリティ製品やサービスの統合状況を確認し、分断された環境での可視性低下や対応遅延を減らす設計が重要です。
- 新しいサービス導入時は、提供範囲、検知・対応の責任分界、既存運用との連携方法を事前に確認するとよいでしょう。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [TekStream launches Proactive Cyber Defense to counter AI-driven threats](https://www.helpnetsecurity.com/2026/06/16/tekstream-launches-proactive-cyber-defense-to-counter-ai-driven-threats/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

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
| [ランサムウェアグループがMicrosoft Teamsの中継を悪用して悪意ある通信を隠蔽](https://www.bleepingcomputer.com/news/security/ransomware-gang-abuses-microsoft-teams-relays-to-hide-malicious-traffic/) | 36.0 | 30.0 | 42.0 |
| [Rockwell Automation FLEX I/O EtherNet/IPアダプタの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-167-05) | 32.0 | 46.0 | 50.0 |
| [攻撃者がFortinet FortiSandboxの3件の脆弱性を悪用、うち1件は先週修正済み](https://www.theregister.com/security/2026/06/16/three-critical-fortinet-sandbox-bugs-splattered-by-unknown-attackers/5256461) | 31.0 | 28.0 | 58.0 |
| [ランサムウェア被害が発生、営業活動は継続 - 食創](https://www.security-next.com/185737) | 30.0 | 30.0 | 42.0 |
| [DragonForceランサムウェアがMicrosoft Teamsを悪用し大手企業への攻撃に潜伏](https://www.infosecurity-magazine.com/news/dragonforce-ransomware-hidden/) | 28.0 | 30.0 | 42.0 |
| [Steam Workshopを悪用してWallpaper Engineアプリ経由でマルウェアを拡散](https://www.bleepingcomputer.com/news/security/steam-workshop-abused-to-spread-malware-via-wallpaper-engine-app/) | 28.0 | 20.0 | 42.0 |
| [ClickFixキャンペーン、新たなローダーと偽アップデート誘導でマルウェア配信を拡大](https://thehackernews.com/2026/06/clickfix-campaigns-expand-malware.html) | 28.0 | 20.0 | 42.0 |
| [Rokarolla Androidトロイの木馬、完全な端末制御と永続化へ進化](https://www.darkreading.com/endpoint-security/rokarolla-android-trojan) | 28.0 | 20.0 | 42.0 |
| [Sharing is Caring: SMB Secret Scanning with Sulla](https://www.praetorian.com/blog/sharing-is-caring-smb-secret-scanning-with-sulla/) | 28.0 | 20.0 | 42.0 |
| [CrooksがTeamsを悪用して新たな方法で連携、C2通信を隠蔽](https://www.theregister.com/cyber-crime/2026/06/16/crooks-found-a-new-way-to-collaborate-using-teams-by-hiding-command-and-control-traffic/5256296) | 28.0 | 20.0 | 42.0 |
| [GhostTree攻撃、再帰的なWindowsジャンクションを悪用してマルウェアを隠蔽](https://www.bleepingcomputer.com/news/security/ghosttree-attack-abused-recursive-windows-junctions-to-hide-malware/) | 28.0 | 20.0 | 42.0 |
| [新たなRokarolla Androidマルウェア、PINやSMSコード、暗号資産ウォレットの資金を窃取](https://thehackernews.com/2026/06/new-rokarolla-android-malware-steals.html) | 28.0 | 20.0 | 42.0 |
| [Microsoft Teamsの中継を悪用して身を隠すDragonForce攻撃者](https://www.security.com/threat-intelligence/dragonforce-msteams-backdoor) | 28.0 | 20.0 | 42.0 |
| [Steam Workshopで数十件の悪意ある壁紙を確認、ゲーマーのアカウントが危険に](https://securelist.com/dozens-of-malicious-wallpapers-found-on-steam-workshop/120186/) | 28.0 | 20.0 | 42.0 |
| [政府機関を標的にしたSprySOCKS LinuxマルウェアのWindows版](https://www.bleepingcomputer.com/news/security/windows-version-of-sprysocks-linux-malware-used-to-attack-govt-orgs/) | 28.0 | 20.0 | 42.0 |
| [偽のMicrosoftアラートを使って北朝鮮系のNarwhalRATマルウェアを展開](https://thehackernews.com/2026/06/fake-microsoft-alerts-used-to-deploy.html) | 28.0 | 20.0 | 42.0 |
| [Microsoftが「Cowork」を提供開始、従量課金で 低コストのAIモデルも展開](https://xtech.nikkei.com/atcl/nxt/column/18/00001/11831/) | 26.0 | 20.0 | 42.0 |
| [デジタル相、停止中のミュトス級AIについて「今あるもので最大限」 3メガバンクなども同様](https://www.itmedia.co.jp/news/articles/2606/16/news124.html) | 26.0 | 20.0 | 42.0 |
| [AIモデルの「成分表」をどう設計するか](https://cyberscoop.com/ai-bill-of-materials-policy-roadmap/) | 25.0 | 20.0 | 42.0 |
| [AI導入の進展はインシデント発生頻度と相関し、ガバナンスの必要性を浮き彫りにする](https://www.cybersecuritydive.com/news/ai-cybersecurity-incidents-governance-jamf/823026/) | 25.0 | 20.0 | 42.0 |
| [AIとサイバーセキュリティ――知りたいけれど聞けなかったすべて](https://www.securityweek.com/ai-and-cybersecurity-everything-you-wanted-to-know-but-were-afraid-to-ask/) | 25.0 | 20.0 | 42.0 |
| [AppViewXがAIエージェントとポスト量子環境に機械IDセキュリティを拡張](https://www.helpnetsecurity.com/2026/06/16/appviewx-agent-identity-security/) | 25.0 | 20.0 | 42.0 |
| [Teleport、LLM ProxyとDelegated Identityを追加しAIエージェントの操作とアクセスを保護](https://www.helpnetsecurity.com/2026/06/16/llm-proxy-and-delegated-identity/) | 25.0 | 20.0 | 42.0 |
| [Radware AI Xploit Shield、新たに特定されたアプリケーションおよびAPIの脆弱性に仮想パッチを提供](https://www.helpnetsecurity.com/2026/06/16/radware-ai-xploit-shield-delivers-virtual-patching-for-newly-identified-application-and-api-flaws/) | 25.0 | 20.0 | 42.0 |
| [Chainguard、JPMorgan、BNYがAI脅威からオープンソースを保護するために連携](https://www.infosecurity-magazine.com/news/chainguard-bny-open-source-athena/) | 25.0 | 20.0 | 42.0 |
| [Cybersecurity幹部らがTrump政権にAnthropicのAIモデル規制緩和を要請](https://www.securityweek.com/cybersecurity-executives-urge-the-trump-administration-to-ease-restrictions-on-anthropic-ai-models/) | 25.0 | 20.0 | 42.0 |
| [Pickle in the Middle ― Vertex AIのモデルアップロードを乗っ取るクロステナントRCE](https://unit42.paloaltonetworks.com/hijacking-vertex-ai-model/) | 25.0 | 20.0 | 42.0 |
| [SimpleHelp RMMの脆弱性により管理対象エンドポイントへの完全アクセスが可能に（CVE-2026-48558）](https://www.helpnetsecurity.com/2026/06/16/simplehelp-rmm-cve-2026-48558/) | 24.0 | 46.0 | 50.0 |
| [Rockwell Automation CompactLogixの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-167-04) | 24.0 | 46.0 | 50.0 |
| [フィッシング報告が23％増 - 約9割が独自ドメイン名を利用](https://www.security-next.com/184893) | 22.0 | 20.0 | 42.0 |
| [机の中に生徒資料を置き忘れ、複数生徒が閲覧 - 大阪府](https://www.security-next.com/185413) | 22.0 | 20.0 | 42.0 |
| [申込者向けのイベント案内メールで誤送信 - 田村市](https://www.security-next.com/185940) | 22.0 | 20.0 | 42.0 |
| [OSSのcurlが異例の「夏休み」を宣言、7月中は脆弱性報告を受け付けず開発者の負担軽減へ](https://gigazine.net/news/20260616-curl-summer-of-bliss/) | 22.0 | 20.0 | 42.0 |
| [SBGとOpenAI、AIで脆弱性診断「Patching as a Service」提供 まずは日本の重要インフラ向けに](https://www.itmedia.co.jp/news/articles/2606/16/news115.html) | 21.0 | 20.0 | 42.0 |
| [Rockwell Automation FactoryTalk Analytics PavilionXの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-167-01) | 20.0 | 28.0 | 50.0 |
| [Rockwell Automation Logix 5370および5570コントローラにCIP経由のサービス拒否の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-167-03) | 20.0 | 28.0 | 50.0 |
| [Rockwell Automation RSLinxの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-167-02) | 20.0 | 28.0 | 50.0 |
| [India、医学試験の不正懸念でTelegramを一時的に遮断](https://therecord.media/india-blocks-telegram-over-cheating-fears) | 20.0 | 20.0 | 42.0 |
| [iRhythm、ハッキングでデータ窃取を確認](https://www.securityweek.com/irhythm-confirms-data-stolen-in-hack/) | 20.0 | 20.0 | 42.0 |
| [英国、SNSアカウント作成時にIDまたは顔スキャンを義務化へ](https://www.bleepingcomputer.com/news/security/uk-to-require-id-or-face-scan-before-you-can-make-social-media-accounts/) | 20.0 | 20.0 | 42.0 |
| [SprySOCKSバックドアがLinuxからWindowsへ拡大](https://www.infosecurity-magazine.com/news/sprysocks-backdoor-windows/) | 20.0 | 20.0 | 42.0 |
| [Hacker Conversations: Isira Adithya、倫理的ハッカーの進化](https://www.securityweek.com/hacker-conversations-isira-adithya-the-evolution-of-an-ethical-hacker/) | 20.0 | 20.0 | 42.0 |
| [FTC、2025年に過去最高の35億ドル被害となったなりすまし詐欺に警鐘](https://www.bleepingcomputer.com/news/security/ftc-warns-of-record-35-billion-losses-to-imposter-scams-in-2025/) | 20.0 | 20.0 | 42.0 |
| [Magnitude、1,000万ドルの資金調達でステルスモードから登場](https://www.securityweek.com/magnitude-emerges-from-stealth-mode-with-10-million-in-funding/) | 20.0 | 20.0 | 42.0 |
| [Rokarolla Trojan、銀行詐欺と端末監視を組み合わせる](https://www.infosecurity-magazine.com/news/rokarolla-android-banking-trojan/) | 20.0 | 20.0 | 42.0 |
| [「無料のワールドカップ配信」サイトは、サッカーではなく詐欺を配信している](https://www.malwarebytes.com/blog/threat-intel/2026/06/free-world-cup-stream-sites-are-serving-scams-not-football) | 20.0 | 20.0 | 42.0 |
| [Endpoint Security新興企業Entがステルスを脱し1億ドルのシード調達を実施](https://www.securityweek.com/endpoint-security-startup-ent-emerges-from-stealth-with-100-million-seed-round/) | 20.0 | 20.0 | 42.0 |
| [心臓病患者の医療データが盗まれ、身代金要求の対象に](https://www.malwarebytes.com/blog/news/2026/06/cardiac-patients-medical-data-stolen-and-held-to-ransom) | 20.0 | 20.0 | 42.0 |
| [Goldilock Secure、Frameとの新たな提携でアイルランドのチャネル展開を拡大](https://www.itpro.com/security/goldilock-secure-expands-irish-channel-presence-through-new-frame-partnership) | 20.0 | 20.0 | 42.0 |
| [サイバー犯罪グループがNovo Nordiskへのハッキングを主張](https://www.securityweek.com/cybercrime-group-claims-novo-nordisk-hack/) | 20.0 | 20.0 | 42.0 |
| [CISOは自社アプリケーションを信頼できるのか？ TrustCloudが目指す質問票の置き換え](https://www.securityweek.com/can-cisos-trust-their-applications-trustcloud-wants-to-replace-the-questionnaire/) | 20.0 | 20.0 | 42.0 |
| [セキュリティ専門家の3分の2以上がサイバー攻撃の難易度が高まっていると回答](https://www.infosecurity-magazine.com/news/security-pros-cyber-cyber-harder/) | 20.0 | 20.0 | 42.0 |
| [Cal Water、イラン系ハッカーによる主張を調査](https://www.securityweek.com/cal-water-investigating-iranian-hackers-claims/) | 20.0 | 20.0 | 42.0 |
| [心拍モニター製造会社のセキュリティに不備、データ窃取犯が急所を狙う](https://www.theregister.com/cyber-crime/2026/06/16/cardiac-monitor-makers-security-skips-a-beat-as-data-thieves-go-for-the-jugular/5256038) | 20.0 | 20.0 | 42.0 |
| [ホワイトハウスがNSSのサイバーセキュリティ強化に向けたメモを発出](https://www.securityweek.com/white-house-issues-memo-to-bolster-nss-cybersecurity/) | 20.0 | 20.0 | 42.0 |
| [調査：インシデントの94%に匿名化インフラが関与、チームは依然として後手に回っている](https://thehackernews.com/2026/06/survey-94-of-incidents-involve.html) | 20.0 | 20.0 | 42.0 |
| [Wiz Exposure Management Dashboard: CTEMのコマンドセンター](https://www.wiz.io/blog/exposure-management-dashboard) | 20.0 | 20.0 | 42.0 |
| [Atomic Archのサプライチェーン攻撃、AURパッケージ1,500件に影響](https://www.securityweek.com/atomic-arch-supply-chain-attack-hits-1500-aur-packages/) | 20.0 | 20.0 | 42.0 |
| [有名女性を描いたディープフェイク投稿サイトが当局により閉鎖される](https://www.malwarebytes.com/blog/ai/2026/06/deepfake-posting-sites-depicting-famous-women-taken-down-by-feds) | 20.0 | 20.0 | 42.0 |
| [URL分析の新標準：ブラウザ内データ検査でフィッシングの死角をなくす](https://any.run/cybersecurity-blog/in-browser-data-inspection/) | 20.0 | 20.0 | 42.0 |
| [仮想通貨詐欺師が宅配業者を送り込み、被害者宅で現金を回収している](https://www.helpnetsecurity.com/2026/06/16/crypto-scammers-couriers-cash-pickups-fbi-warning/) | 20.0 | 20.0 | 42.0 |
| [China関連のSprySOCKSバックドア、ドライバベースのステルスでWindowsへ拡大](https://thehackernews.com/2026/06/china-linked-sprysocks-backdoor-expands.html) | 20.0 | 20.0 | 42.0 |
| [Tech Coalitionの「Athena」が公開前のOSS脆弱性を狙う動き](https://www.securityweek.com/tech-coalition-athena-targets-oss-vulnerabilities-ahead-of-disclosure/) | 20.0 | 20.0 | 42.0 |
| [ソフトウェアサプライチェーンは透明性の試練を迎えている](https://www.helpnetsecurity.com/2026/06/16/enisa-software-supply-chain-transparency/) | 20.0 | 20.0 | 42.0 |
| [Fortinet FortiSandboxの重大な脆弱性が攻撃で悪用中](https://www.bleepingcomputer.com/news/security/critical-fortinet-fortisandbox-flaws-now-exploited-in-attacks/) | 20.0 | 20.0 | 42.0 |
| [夏の旅行計画に便乗する偽旅行サイトが急増しています](https://www.helpnetsecurity.com/2026/06/16/hospitality-travel-organizations-cyberattacks/) | 20.0 | 20.0 | 42.0 |
| [FBIが警告、宅配便による現金受け取りが暗号資産詐欺を助長](https://www.infosecurity-magazine.com/news/fbi-warns-courier-cash-pickups/) | 20.0 | 20.0 | 42.0 |

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
