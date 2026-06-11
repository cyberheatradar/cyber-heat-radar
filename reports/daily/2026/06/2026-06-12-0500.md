# 📡 サイレーダー 2026-06-12 05:00 JST

このレポートは、2026-06-11 17:00 JST〜2026-06-12 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 97
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 65

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN Validator Authenticated Privilege Escalation Vulnerability](#topic-4945) | 63.0 | 84.0 | 67.0 | 音声 | 温度感上位枠 |
| 2 | [CVE-2026-10520: CISA KEV catalog addition](#topic-16465) | 62.0 | 74.0 | 64.0 | 音声 | 温度感上位枠 |
| 3 | [Oracle Addresses PeopleSoft Vulnerability Amid Reports of Zero-Day Attacks](#topic-16788) | 52.0 | 64.0 | 59.0 | 音声 | 温度感上位枠 |
| 4 | [Oracle PeopleSoft servers under attack, Oracle pushes out-of-band security alert](#topic-16831) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [Criminal AI-as-a-Service in 2026: How the Underground Market Is Operationalizing Cybercrime](#topic-16826) | 41.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [ThreatsDay Bulletin: Worm Code Leaked, AI Agent Phished, Claude Code Patch + 28 New Stories](#topic-16821) | 33.0 | 45.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [Cybercriminals Use Fake AI Guides and Dev Tools to Spread AsyncRAT Malware](#topic-16814) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-4945"></a>

### 1. Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN Validator Authenticated Privilege Escalation Vulnerability

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

Ciscoは、Catalyst SD-WAN Controller、Catalyst SD-WAN Manager、Catalyst SD-WAN Validatorに存在する権限昇格の脆弱性に対する修正を公表しました。
CVE-2026-20182として追跡されており、認証済みのローカル攻撃者が細工されたファイルを用いてroot権限で任意のコマンドを実行できる可能性があるとされています。
SD-WANの管理系コンポーネントに関わる脆弱性のため、影響を受けると広範なネットワーク運用基盤に波及するおそれがあります。
加えて、限定的な実悪用が示唆されているため、早期の適用判断が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 9 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 観測あり・信頼度: 中。
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

- 影響を受けるCatalyst SD-WAN製品のバージョンと構成を確認し、Ciscoの修正情報に沿って更新を進める。
- 管理系インターフェースへの認証済みアクセスを前提にしたリスクとして、不要なアカウントや権限を見直す。
- 関連する管理操作や不審なファイル取り込みの痕跡を確認し、想定外のCLI実行や高権限操作がないか監視する。

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

- SNS反応: 観測あり・信頼度: 低。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 観測あり・信頼度: 低。
- 技術者コミュニティ反応: 観測あり・信頼度: 中。
- 開発者コミュニティ反応: 観測あり・信頼度: 中。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。

---

<a id="topic-16465"></a>

### 2. CVE-2026-10520: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 62.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 64.0 |

#### 概要

CISAは、Ivanti Sentryに存在するCVE-2026-10520をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
公表情報では、この脆弱性はOSコマンドインジェクションに関係し、Ivantiは既に修正を案内しています。
KEV掲載は、実際に悪用された証拠があることを示すため、優先度の高い対応が必要になります。
公開情報では技術詳細や検証コードへの言及もあり、未対応環境ではリスクが高まる可能性があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 観測あり・信頼度: 中。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

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

- Ivanti Sentryの該当バージョンを利用しているか確認し、ベンダーの修正適用状況を点検する。
- KEV追加対象として、脆弱性管理の優先順位を上げて早期対応する。
- 外部公開された技術情報の影響を前提に、関連ログや異常な挙動の監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-10520 | 主要CVE | 1.00 |
| ベンダー | Ivanti | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-10520](https://nvd.nist.gov/vuln/detail/CVE-2026-10520) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/06/11/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Ivanti Sentry flaw allows root-level remote code execution (CVE-2026-10](https://www.helpnetsecurity.com/2026/06/10/ivanti-sentry-cve-2026-10520-cve-2026-10523/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Ivanti tells Sentry customers to patch now as critical bugs hit 10.0 and 9.9](https://www.theregister.com/patches/2026/06/10/ivanti-urges-sentry-users-to-patch-two-critical-bugs/5253428) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-10520, CVE-2026-10523 - Multiple critical vulnerabilities affecting Iva](https://www.rapid7.com/blog/post/etr-cve-2026-10520-cve-2026-10523-multiple-critical-vulnerabilities-affecting-ivanti-sentry) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 観測あり・信頼度: 低。
- 技術者コミュニティ反応: 観測あり・信頼度: 中。
- 開発者コミュニティ反応: 観測あり・信頼度: 中。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。

---

<a id="topic-16788"></a>

### 3. Oracle Addresses PeopleSoft Vulnerability Amid Reports of Zero-Day Attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 52.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

OracleはPeopleSoft Suiteに関する脆弱性CVE-2026-35273への対応を公表しており、複数の報道ではこの問題がゼロデイとして悪用された可能性が取り上げられています。
現時点では、Oracleが被害規模や攻撃の詳細をすべて確認したとまでは言えませんが、認証不要のリモートコード実行につながるとされる点から、影響は大きいとみられます。
PeopleSoftは業務基盤として利用されることがあるため、該当環境では優先度の高い確認対象になります。
悪用観測が報じられている脆弱性は、公開情報だけでも迅速な緩和対応が求められます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。

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

- PeopleSoftの利用有無と対象バージョンを確認し、Oracleの案内に沿って緩和策や更新状況を点検する。
- 外部公開されている管理画面や関連サービスの露出を見直し、不要な公開を避ける。
- 認証関連の異常、予期しないプロセス起動、設定変更やデータアクセスの兆候がないか監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-35273 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-35273](https://nvd.nist.gov/vuln/detail/CVE-2026-35273) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Oracle mitigates PeopleSoft zero-day exploited in data theft attacks](https://www.bleepingcomputer.com/news/security/oracle-mitigates-peoplesoft-zero-day-exploited-in-data-theft-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShinyHunters claims it hacked 100 orgs by exploiting an Oracle PeopleSoft 0-day](https://www.theregister.com/cyber-crime/2026/06/11/shinyhunters-claims-oracle-peoplesoft-0-day-hit-100-orgs/5254443) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Oracle Addresses PeopleSoft Vulnerability Amid Reports of Zero-Day Attacks](https://www.securityweek.com/oracle-addresses-peoplesoft-vulnerability-amid-reports-of-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 観測あり・信頼度: 低。
- 技術者コミュニティ反応: 観測あり・信頼度: 中。
- 開発者コミュニティ反応: 観測あり・信頼度: 中。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-16831"></a>

### 4. Oracle PeopleSoft servers under attack, Oracle pushes out-of-band security alert

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Oracle PeopleSoft PeopleToolsに関する脆弱性CVE-2026-35273について、実際の悪用が観測されていると伝えられています。
Oracleはこの件について、通常の更新とは別にセキュリティ警告を出しています。
影響範囲はPeopleSoft PeopleToolsの8.61および8.62が中心とされ、未サポート版にも影響する可能性が示されています。
認証なしで外部から悪用される可能性があり、深刻な侵害につながるおそれがあるためです。
業務システムで使われる製品であることから、対応の遅れが運用影響に直結しやすい点も注目されています。

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

- Oracleのセキュリティ告知と修正情報を確認し、対象バージョンの有無を早急に棚卸しする。
- 公開インターフェースや関連サービスの露出状況を点検し、不要な公開を避ける。
- 監視ログでPeopleSoft関連の異常なアクセスや挙動を確認し、必要に応じてインシデント対応を準備する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-35273 | 主要CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Oracle PeopleSoft servers under attack, Oracle pushes out-of-band security alert](https://www.helpnetsecurity.com/2026/06/11/oracle-peoplesoft-under-attack-cve-2026-35273/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 観測あり・信頼度: 低。
- 技術者コミュニティ反応: 観測あり・信頼度: 中。
- 開発者コミュニティ反応: 観測あり・信頼度: 中。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-16826"></a>

### 5. Criminal AI-as-a-Service in 2026: How the Underground Market Is Operationalizing Cybercrime

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

2026年時点の地下市場では、犯罪向け生成AIは「自律的に攻撃するAI」よりも、フィッシング文面作成、標的分析、偽造文書作成、翻訳、データ整理などを効率化する作業支援層として浸透しているとされています。
市場はTelegram系ボットやラッパー、盗用されたAIアカウントやAPIキーなどを含む形で商業化が進んでいますが、実態は不安定で、誇大広告や短命なサービスも多いと見られます。
攻撃者の技能や手間を下げ、より多くの人が高度に見える詐欺やソーシャルエンジニアリングを実行しやすくなる点が注目されています。
さらに、企業が利用するAIアカウントやAPIキー自体が新たな攻撃面になるため、従来のマルウェア対策だけでは不十分になりつつあります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI関連アカウント、APIキー、接続先、アップロードファイルの権限とログを棚卸しし、最小権限で管理する。
- フィッシング対策は文面の巧拙よりも、送信元検証、業務プロセスの異常、取引確認などの制御を重視する。
- 高リスク業務では、多要素認証や強い承認フロー、送金・権限変更のアウトオブバンド確認を標準化する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Criminal AI-as-a-Service in 2026: How the Underground Market Is Operationalizing](https://www.rapid7.com/blog/post/tr-criminal-ai-underground-market-operationalizing-cybercrime-2026) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 観測あり・信頼度: 低。
- 技術者コミュニティ反応: 観測あり・信頼度: 中。
- 開発者コミュニティ反応: 観測あり・信頼度: 中。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-16821"></a>

### 6. ThreatsDay Bulletin: Worm Code Leaked, AI Agent Phished, Claude Code Patch + 28 New Stories

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>サ⁠プ⁠ラ⁠イ⁠チ⁠ェ⁠ー⁠ン</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 45.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報では、サプライチェーン攻撃に関係しうるコードや、AIエージェントが認証情報を漏らす可能性を示す研究が話題になっています。
あわせて、Claude Codeに関するパッチ情報も含まれており、AI活用環境と開発基盤の両方で注意が必要な状況がうかがえます。
AI関連機能の導入が進むほど、エージェントの挙動や権限設定の不備が情報漏えいにつながるリスクがあります。
さらに、開発者向けのサプライチェーン経由の脅威は、個別端末だけでなくCI/CDや依存関係全体に影響し得ます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIエージェントに与える権限と接続先を最小化し、機密情報へのアクセスを必要最小限に制限する。
- 依存パッケージや外部コードの取り込み手順を再点検し、署名・レビュー・固定バージョン運用を徹底する。
- Claude Codeを含むAI開発ツールは、パッチや更新情報を確認し、利用中の構成に影響がないか検証する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ai_model_or_project | Claude | 主題 | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ThreatsDay Bulletin: Worm Code Leaked, AI Agent Phished, Claude Code Patch + 28 ](https://thehackernews.com/2026/06/threatsday-bulletin-worm-code-leaked-ai.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 観測あり・信頼度: 低。
- 技術者コミュニティ反応: 観測あり・信頼度: 中。
- 開発者コミュニティ反応: 観測あり・信頼度: 中。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-16814"></a>

### 7. Cybercriminals Use Fake AI Guides and Dev Tools to Spread AsyncRAT Malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、サイバー犯罪者が偽のAIガイドや開発ツールを装った誘導を使い、最終的にAsyncRATを配布する多段階の手口が観測されています。
コードや構成の一部にAI支援を示唆する痕跡がある可能性も指摘されていますが、詳細は確認情報に基づいて慎重に見る必要があります。
AI関連の偽情報や開発者向け資料を悪用する手口は、利用者の警戒を下げやすく、通常のフィッシングよりも見抜きにくい点が問題です。
感染後にリモート操作を可能にするマルウェアが配布されるため、エンドポイント防御とユーザー教育の両面で注意が必要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIツールや開発支援資料を装う配布物は、信頼できる提供元かを確認し、入手経路を厳格に管理する。
- 不審な添付ファイル、圧縮ファイル、インストーラ、スクリプトの実行を抑止し、端末側で多段階の実行痕跡を監視する。
- AsyncRAT系の不審な通信や永続化の兆候を想定し、EDRやネットワーク監視で早期検知できるようルールを見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Cybercriminals Use Fake AI Guides and Dev Tools to Spread AsyncRAT Malware](https://www.infosecurity-magazine.com/news/fake-ai-guides-dev-tools-spread/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 観測あり・信頼度: 低。
- 技術者コミュニティ反応: 観測あり・信頼度: 中。
- 開発者コミュニティ反応: 観測あり・信頼度: 中。
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
| [‘GreatXML’のゼロデイ攻撃でBitLockerを回避](https://www.securityweek.com/greatxml-zero-day-exploit-bypasses-bitlocker/) | 39.0 | 38.0 | 43.0 |
| [ProofpointがEuropol EC3の諮問グループに参加し、サイバー犯罪対策で官民連携を強化](https://www.proofpoint.com/us/blog/corporate-news/proofpoint-joins-europol-ec3-agis) | 36.0 | 30.0 | 42.0 |
| [Microsoftの最悪の「Nightmare」がBitLockerバイパスのゼロデイを解き放つ](https://www.theregister.com/security/2026/06/11/nightmare-eclipse-drops-claimed-bitlocker-bypass-for-microsoft-windows/5254371) | 35.0 | 38.0 | 42.0 |
| [AIブームに便乗したソーシャルエンジニアリング攻撃の増加、Anthropic・OpenAI・DeepSeekを餌に悪用](https://www.itpro.com/security/cyber-attacks/hackers-are-capitalizing-on-ai-hype-to-ramp-up-social-engineering-attacks-and-theyre-using-big-brands-like-anthropic-openai-and-deepseek-as-bait-to-lure-victims) | 33.0 | 20.0 | 42.0 |
| [10人中9人が本物とAI生成コンテンツを見分けられなくなっている](https://www.helpnetsecurity.com/2026/06/11/ai-scams-deepfakes-survey/) | 33.0 | 20.0 | 42.0 |
| [ジョーシス、ランサムウェアの脅威を防ぐAI駆動の新機能を発表](https://japan.zdnet.com/article/35248805/) | 31.0 | 38.0 | 42.0 |
| [The Gentlemenランサムウェアが478件の被害を主張、ワームのように拡散可能](https://thehackernews.com/2026/06/the-gentlemen-ransomware-claims-478.html) | 28.0 | 30.0 | 42.0 |
| [当局が「AudiA6」ランサムウェアの暗号資産洗浄サービスを摘発](https://www.bleepingcomputer.com/news/legal/authorities-dismantle-audia6-ransomware-crypto-laundering-service/) | 28.0 | 30.0 | 42.0 |
| [データ窃取がランサムウェア要求を支配し、恐喝のみの攻撃が増加](https://www.infosecurity-magazine.com/news/extortion-only-attacks-surge/) | 28.0 | 30.0 | 42.0 |
| [Void Blizzardによるスパイ活動キャンペーンに関連してロシア人国民が起訴される](https://cyberscoop.com/russian-national-charged-void-blizzard-cyber-espionage/) | 28.0 | 20.0 | 48.0 |
| [中国関連の拡張ボットネットが米国の重要インフラと軍事資産を狙っているとして専門家が警鐘](https://www.itpro.com/security/security-experts-sound-alarm-over-expanded-china-linked-botnet-used-to-target-us-critical-infrastructure-and-military-assets) | 28.0 | 20.0 | 42.0 |
| [Void Blizzardに関連するハッカー、サイバー諜報キャンペーンで起訴される](https://therecord.media/hacker-linked-to-void-blizzard-faces-charges) | 28.0 | 20.0 | 42.0 |
| [TikTokやInstagram Reelsで広がる偽Spotify Premiumチュートリアルによるマルウェア拡散](https://www.helpnetsecurity.com/2026/06/11/vidar-infostealer-tiktok-instagram-reels-malware-campaigns/) | 28.0 | 20.0 | 42.0 |
| [OnyxC2 Stealerが月額250ドルで企業級の窃取機能を提供](https://www.securityweek.com/onyxc2-stealer-offers-cybercriminals-enterprise-grade-theft-for-250-a-month/) | 28.0 | 20.0 | 42.0 |
| [Siemens、Desigo CCのファイルがセキュリティエンジンにマルウェアとして検出されると発表](https://www.securityweek.com/siemens-says-desigo-cc-files-flagged-as-malware-by-security-engines/) | 28.0 | 20.0 | 42.0 |
| [OceanLotusがFireAnt攻撃でSPECTRALVIPERを用いてベトナムの投資家を標的に](https://thehackernews.com/2026/06/oceanlotus-hits-vietnam-investors-with.html) | 28.0 | 20.0 | 42.0 |
| [「Interop Tokyo 2026」が開催中 - 「AI」関連ソリューションも充実](https://www.security-next.com/185762) | 27.0 | 20.0 | 42.0 |
| [Brickcom Camerasの脆弱性に関する情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-162-03) | 26.0 | 46.0 | 50.0 |
| [AIに買い物を任せる時代へ VisaとOpenAIが提携──“代理決済”を上限設定などで安全に](https://www.itmedia.co.jp/news/articles/2606/11/news126.html) | 26.0 | 20.0 | 42.0 |
| [NECとAnthropic、三井住友FGなど金融8社と協業 金融業界のAI実装拡大へ](https://xtech.nikkei.com/atcl/nxt/news/24/03264/) | 26.0 | 20.0 | 42.0 |
| [積水化学工業の基幹システム刷新、AI活用に向けた業務の標準化とデータ整備](https://xtech.nikkei.com/atcl/nxt/column/18/03585/061100020/) | 26.0 | 20.0 | 42.0 |
| [OpenClaw AIエージェントをだましてコード実行と機密情報漏えいを引き起こす新たな攻撃](https://thehackernews.com/2026/06/new-attacks-trick-openclaw-ai-agent.html) | 25.0 | 20.0 | 42.0 |
| [Google、AI Overviewsの虚偽表示で責任を問われると裁判所が判断](https://www.malwarebytes.com/blog/ai/2026/06/google-can-be-liable-for-false-ai-overviews-court-rules) | 25.0 | 20.0 | 42.0 |
| [CISAが連邦機関に「より賢くパッチを適用する」よう指示](https://www.helpnetsecurity.com/2026/06/11/cisa-risk-based-vulnerability-management-government/) | 25.0 | 20.0 | 42.0 |
| [企業がAIなどの重要トピックに対するセキュリティ教育予算を拡大](https://www.cybersecuritydive.com/news/cybersecurity-training-budget-increases-ai-skills/822640/) | 25.0 | 20.0 | 42.0 |
| [AI主導の脅威がMSPセキュリティスタックの限界を露呈している理由](https://www.bleepingcomputer.com/news/security/why-ai-driven-threats-are-exposing-the-limits-of-msp-security-stacks/) | 25.0 | 20.0 | 42.0 |
| [新たなサイバー脅威への対策トレーニング時間を確保できないセキュリティチームの実態](https://www.infosecurity-magazine.com/news/cybersecurity-training-time/) | 25.0 | 20.0 | 42.0 |
| [AIが脆弱性管理を変えたためCISOがBASに予算を移す理由](https://thehackernews.com/2026/06/ai-broke-vulnerability-management-thats.html) | 25.0 | 20.0 | 42.0 |
| [AIエージェントのサプライチェーンにおける整合性検証](https://unit42.paloaltonetworks.com/ai-agent-supply-chain-risks/) | 25.0 | 20.0 | 42.0 |
| [サーバーの保護を強化する方法](https://www.security.com/product-insights/locking-down-server) | 25.0 | 20.0 | 42.0 |
| [AIコーディングエージェントを乗っ取る新たな「Agentjacking」攻撃](https://www.infosecurity-magazine.com/news/agentjacking-attacks-hijack-ai/) | 25.0 | 20.0 | 42.0 |
| [Check Point、MSP向けプラットフォームをAIガバナンスと統合セキュリティバンドルで拡張](https://www.helpnetsecurity.com/2026/06/11/check-point-msp-platform-expansion/) | 25.0 | 20.0 | 42.0 |
| [SQLiからRCEへ――LangGraphのCheckpointerを悪用する手法](https://research.checkpoint.com/2026/from-sqli-to-rce-exploiting-langgraphs-checkpointer/) | 24.0 | 46.0 | 50.0 |
| [HackersがLangflowの脆弱性を悪用しリモートコード実行を実施](https://www.securityweek.com/hackers-exploit-langflow-vulnerability-for-remote-code-execution/) | 24.0 | 38.0 | 42.0 |
| [サイトが改ざん被害、外部へ誘導 - アイサンテクノロジー](https://www.security-next.com/185010) | 22.0 | 20.0 | 42.0 |
| [防災士向け研修会の案内メールで送信ミス - 本巣市](https://www.security-next.com/185744) | 22.0 | 20.0 | 42.0 |
| [Naxclow IoT Platformの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-162-02) | 20.0 | 28.0 | 50.0 |
| [YarboのAndroid/iOSモバイルアプリケーションおよびクラウドインフラストラクチャ](https://www.cisa.gov/news-events/ics-advisories/icsa-26-162-01) | 20.0 | 28.0 | 50.0 |
| [開示から24時間後に悪用されたIvantiの最大深刻度の脆弱性](https://www.darkreading.com/vulnerabilities-threats/max-severity-ivanti-sentry-flaw-exploited-24-hours) | 20.0 | 20.0 | 42.0 |
| [GreatXMLの新たなエクスプロイトがRecovery PartitionのXMLファイルを通じてWindows BitLockerを回避](https://thehackernews.com/2026/06/new-greatxml-exploit-bypasses-windows.html) | 20.0 | 20.0 | 42.0 |
| [Cyber Forceは上院の国防政策ロードマップに含まれず](https://therecord.media/cyber-force-not-included-senate-defense-roadmap) | 20.0 | 20.0 | 42.0 |
| [VRChat、Maine州司法長官室の偽の侵害通知に言及](https://www.theregister.com/security/2026/06/11/24m-vrchat-users-data-accessed-following-cloud-breach/5254246) | 20.0 | 20.0 | 42.0 |
| [Secret scanningの信頼性向上：大規模環境での誤検知削減](https://github.blog/security/making-secret-scanning-more-trustworthy-reducing-false-positives-at-scale/) | 20.0 | 20.0 | 42.0 |
| [英国の高校がサイバー攻撃を受け生徒を帰宅させる](https://therecord.media/british-school-sends-students-home-cyberattack) | 20.0 | 20.0 | 42.0 |
| [CISAが脆弱性の深刻度ではなくリスクに基づく修正を各機関に指示](https://www.infosecurity-magazine.com/news/cisa-orders-agencies-to-patch-by/) | 20.0 | 20.0 | 42.0 |
| [FIFA World Cupが大規模な犯罪・ハクティビストのサイバー脅威に直面する見込み](https://www.cybersecuritydive.com/news/fifa-world-cup-criminal-hacktivist-cyber-threat/822638/) | 20.0 | 20.0 | 42.0 |
| [OTでは、運用担当者が注意を払っていればセグメンテーションは有効です](https://www.darkreading.com/cybersecurity-operations/segmentation-works-for-ot-if-operators-are-paying-attention) | 20.0 | 20.0 | 42.0 |
| [Proxmox Mail Gateway 9.1リリース、隔離とバックアップの暗号化を変更](https://www.helpnetsecurity.com/2026/06/11/proxmox-mail-gateway-9-1-released/) | 20.0 | 20.0 | 42.0 |
| [University of Nottinghamがサイバーインシデントを確認、Shiny Huntersグループがデータ窃取を主張](https://therecord.media/university-of-nottingham-cyber-incident-shiny-hunters) | 20.0 | 20.0 | 42.0 |
| [アラート疲れが独自のセキュリティ脅威になりつつある](https://www.securityweek.com/alert-fatigue-is-becoming-a-security-threat-of-its-own/) | 20.0 | 20.0 | 42.0 |
| [Cybersecurity Stars Awards 2026、95部門の受賞者を発表](https://thehackernews.com/2026/06/cybersecurity-stars-awards-2026-winners.html) | 20.0 | 20.0 | 42.0 |
| [CISAが連邦機関にリスクに基づくセキュリティパッチの優先適用を指示](https://www.securityweek.com/cisa-directs-federal-agencies-to-prioritize-security-patches-based-on-risk/) | 20.0 | 20.0 | 42.0 |
| [LABScon25再演｜基調講演：サイバー生態学への歩み](https://www.sentinelone.com/labs/labscon25-replay-keynote-steps-to-an-ecology-of-cyber/) | 20.0 | 20.0 | 42.0 |
| [Coupang、韓国で過去最高の4億900万ドルのデータ侵害罰金を科される](https://www.bleepingcomputer.com/news/security/south-korea-hits-coupang-with-record-409-million-fine-over-data-breach/) | 20.0 | 20.0 | 42.0 |
| [CISAが政府機関に対し、悪用確認済みの重大な脆弱性を3日以内に修正するよう通知](https://www.bleepingcomputer.com/news/security/cisa-tells-govt-agencies-to-patch-critical-exploited-flaws-in-3-days/) | 20.0 | 20.0 | 42.0 |
| [VRChatユーザー240万人分のデータが流出](https://www.malwarebytes.com/blog/data-breaches/2026/06/data-of-2-4-million-vrchat-users-stolen) | 20.0 | 20.0 | 42.0 |
| [Interpol、Phishing-as-a-Serviceプラットフォーム「SniperDz」を摘発](https://www.infosecurity-magazine.com/news/interpol-dismantles-sniperdz/) | 20.0 | 20.0 | 42.0 |
| [FBIが中国による米国労働者の標的化と勧誘に使われた13のWebサイトを差し押さえ](https://www.securityweek.com/fbi-seizes-13-websites-that-officials-say-were-used-by-china-to-target-and-recruit-us-workers/) | 20.0 | 20.0 | 42.0 |
| [英国、子ども向けスマートフォンにヌード画像のブロックを9月までに義務化](https://www.malwarebytes.com/blog/family-and-parenting/2026/06/childrens-phones-must-block-nude-images-by-september-uk-says) | 20.0 | 20.0 | 42.0 |
| [SplunkとPalo Alto Networksが深刻な脆弱性を修正](https://www.securityweek.com/splunk-palo-alto-networks-patch-severe-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [FBI、中国の情報収集活動に関連する13のウェブサイトを差し押さえ](https://www.helpnetsecurity.com/2026/06/11/fake-consulting-websites-target-us-security-clearance-holders-china/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、Windows Server 2025のBitLocker回復不具合を修正](https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-bitlocker-recovery-bug-on-windows-server-2025/) | 20.0 | 20.0 | 42.0 |
| [Infosecurity EuropeからCONFidence、C1b3rWallまで：2026年にセキュリティチームが優先すること](https://any.run/cybersecurity-blog/europe-cybersecurity-conferences-2026/) | 20.0 | 20.0 | 42.0 |
| [University of Nottingham、ハッカーによるデータ流出後に侵害を確認](https://www.securityweek.com/university-of-nottingham-confirms-breach-after-hackers-leak-data/) | 20.0 | 20.0 | 42.0 |
| [IDnow、規制対象企業のKYCから継続的な信頼へ移行を支援するTrust Platformを発表](https://www.helpnetsecurity.com/2026/06/11/idnow-launches-trust-platform-to-help-regulated-firms-move-from-kyc-to-continuous-trust/) | 20.0 | 20.0 | 42.0 |

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
