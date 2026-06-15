# 📡 サイレーダー 2026-06-16 05:00 JST

このレポートは、2026-06-15 17:00 JST〜2026-06-16 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 99
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 69

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [15th June – Threat Intelligence Report](#topic-16788) | 48.0 | 67.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [Cisco Catalyst SD-WAN Manager Arbitrary File Write Vulnerability](#topic-17402) | 43.0 | 46.0 | 55.0 | 音声 | 温度感上位枠 |
| 3 | [⚡ Weekly Recap: Chrome 0-Day, UniFi Exploits, macOS Stealers, VPN Flaw and More](#topic-17435) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Public and Private Medical Community Targeted by China-Nexus Threat Actor Pursuing Artificial Intelligence, Cyber, Medical, and National Defense Research](#topic-17432) | 37.0 | 20.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [China-nexus group linked to multiyear campaign targeting US, Canadian medical research](#topic-17420) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-16788"></a>

### 1. 15th June – Threat Intelligence Report

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 冷却中 |
| <nobr>温⁠度⁠感</nobr> | 48.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 67.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Oracle PeopleSoft Enterprise PeopleToolsの脆弱性CVE-2026-35273について、外部では実際の悪用が確認されていると報じられており、CISAのKEVカタログにも追加されています。
影響は未認証でのリモートコード実行につながる可能性があるとされ、大学などへの侵害・データ窃取キャンペーンとの関連が指摘されています。
認証なしで悪用され得る重大な脆弱性であり、公開後すぐに攻撃対象になった可能性がある点が重要です。対象製品を利用している組織では、資産把握と修正適用の優先度が高い事案です。

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

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 技術詳細・悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 技術詳細、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Oracle PeopleSoft Enterprise PeopleToolsの利用有無を確認し、該当バージョンを特定する。
- Oracleの修正情報とCISA KEV掲載状況を踏まえ、影響を受ける環境は優先的に対処する。
- 外部公開面の監視、認証不要の異常アクセス、設定変更や不審なコード実行の痕跡を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-35273 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |
| ベンダー | Microsoft | 言及あり | 0.80 |
| ransomware_group | Clop | 主題 | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-35273](https://nvd.nist.gov/vuln/detail/CVE-2026-35273) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [15th June – Threat Intelligence Report](https://research.checkpoint.com/2026/15th-june-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShinyHunters is actively extorting universities after exploiting an unpatched Or](https://cyberscoop.com/oracle-peoplesoft-zero-day-vulnerability-shinyhunters-extortion/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Active Exploitation of Oracle PeopleSoft Zero-Day (CVE-2026-35273)](https://www.rapid7.com/blog/post/etr-active-exploitation-of-oracle-peoplesoft-zero-day-cve-2026-35273) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/06/12/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google Confirms Exploitation of Oracle PeopleSoft Zero-Day by ShinyHunters](https://www.securityweek.com/google-confirms-exploitation-of-oracle-peoplesoft-zero-day-by-shinyhunters/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShinyHunters Exploits Oracle PeopleSoft Zero-Day (CVE-2026-35273) to Breach Univ](https://thehackernews.com/2026/06/shinyhunters-exploits-oracle-peoplesoft.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Oracle mitigates PeopleSoft zero-day exploited in data theft attacks](https://www.bleepingcomputer.com/news/security/oracle-mitigates-peoplesoft-zero-day-exploited-in-data-theft-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補あり。

---

<a id="topic-17402"></a>

### 2. Cisco Catalyst SD-WAN Manager Arbitrary File Write Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

Ciscoは、Catalyst SD-WAN Manager（旧SD-WAN vManage）の脆弱性 CVE-2026-20262 に対する修正を公開しました。
公開情報によると、この問題は認証済みのリモート攻撃者に任意のファイル作成・上書きを許す可能性があり、実際の攻撃で悪用されたとされています。
ネットワーク管理系の製品でファイル書き込みにつながる脆弱性は、設定改ざんや権限昇格など深刻な影響に発展し得ます。
すでに悪用情報があるため、該当環境では通常より優先度を上げて確認すべき事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。

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

- Ciscoの修正提供状況と、該当バージョンの利用有無を確認する。
- 管理画面や関連APIへの認証ログ・不審なリクエストの有無を点検する。
- 適用可能な更新を早急に適用し、影響範囲の大きい管理系システムは優先して監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20262 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20262](https://nvd.nist.gov/vuln/detail/CVE-2026-20262) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco fixes SD-WAN vManage flaw exploited in zero-day attacks](https://www.bleepingcomputer.com/news/security/cisco-fixes-sd-wan-vmanage-flaw-exploited-in-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Manager Arbitrary File Write Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-arbfw-c2rZvQ) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17435"></a>

### 3. ⚡ Weekly Recap: Chrome 0-Day, UniFi Exploits, macOS Stealers, VPN Flaw and More

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

今週のサイバーセキュリティ動向をまとめた記事で、Chromeのゼロデイ、UniFi関連の脆弱性、macOS向けの情報窃取型マルウェア、VPNの不備など、複数の話題が取り上げられています。
公開情報ベースでは、既知の問題や古い仕組みの放置が引き続き攻撃の起点になり得るという流れが示されています。
単発の個別事案というより、広く使われる製品や見落とされがちな運用部分が継続的に狙われている点が重要です。パッチ適用だけでなく、不要な機能や古い認証経路の見直しも求められます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- ChromeやVPNなど、外部公開面にある製品の更新状況と緊急パッチ情報を確認する。
- UniFiやmacOS端末など、利用中の製品群に関連する既知の脆弱性・検知情報を棚卸しする。
- 不要な旧機能や未使用のログイン経路、放置されたソフトウェアが残っていないか点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [⚡ Weekly Recap: Chrome 0-Day, UniFi Exploits, macOS Stealers, VPN Flaw and More](https://thehackernews.com/2026/06/weekly-recap-chrome-0-day-unifi.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17432"></a>

### 4. Public and Private Medical Community Targeted by China-Nexus Threat Actor Pursuing Artificial Intelligence, Cyber, Medical, and National Defense Research

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>国⁠家⁠支⁠援</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Google Threat Intelligence Group（GTIG）は、UNC6508とされる中国関連の脅威アクターが、北米の医療・学術・軍関連研究機関を狙ったキャンペーンを観測したと公表しました。
外部公開Webアプリケーションの悪用、独自マルウェアの投入、正規の管理機能を使った情報流出が含まれ、医療研究や防衛研究など幅広い情報収集が意図されていた可能性が示されています。
医療研究機関は患者情報だけでなく、先端技術や国家安全保障に関わる研究データも扱うため、被害の影響が広がりやすい点が重要です。
さらに、正規機能を悪用した流出は検知しづらく、一般的な侵入対策だけでは見落としが起きやすいことが注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- REDCapなど外部公開している研究系アプリケーションは、最新化と不要な旧版の削除を徹底する。
- 管理者アカウントにはフィッシング耐性のある多要素認証を適用し、資格情報の使い回しを避ける。
- 監査ログやDLP、内容監査ルールの変更を監視し、正規機能を使った不審な転送・共有の兆候を確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Public and Private Medical Community Targeted by China-Nexus Threat Actor Pursui](https://cloud.google.com/blog/topics/threat-intelligence/prc-targets-us-medical-research/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17420"></a>

### 5. China-nexus group linked to multiyear campaign targeting US, Canadian medical research

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Googleの報告を受け、米国とカナダの医療研究を狙った長期的なスパイ活動に、China-nexusのグループが関与していると伝えられています。
標的にはウイルス関連、AI、軍事関連の情報が含まれていたとされます。医療研究は機微な知的財産や公衆衛生に関わるため、情報流出の影響が大きくなり得ます。
AIや軍事情報も対象に含まれている点から、単一分野ではなく広範な機密情報収集の一環として注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 研究機関や共同研究先を含め、機微情報の保管場所とアクセス権限を再点検する。
- 長期潜伏を想定し、通常業務に紛れる不審な認証・通信・権限昇格の兆候を継続監視する。
- 医療・研究部門では、アカウント保護、多要素認証、端末管理、ログ保全を優先して強化する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [China-nexus group linked to multiyear campaign targeting US, Canadian medical re](https://www.cybersecuritydive.com/news/china-nexus-multiyear-hacking-us-canadian-medical-research/822912/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
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
| [北朝鮮のハッカーが開発者向けツールをマルウェア配信チャネルとして悪用](https://thehackernews.com/2026/06/north-korean-hackers-are-turning.html) | 28.0 | 45.0 | 42.0 |
| [Miasmaが侵害されたCI/CDインフラを通じてソフトウェアサプライチェーン攻撃を拡大](https://blog.polyswarm.io/miasma-expands-software-supply-chain-attacks-through-compromised-ci/cd-infrastructure) | 28.0 | 45.0 | 42.0 |
| [AnubisによるAdriatic港へのサイバー攻撃で高まる海事セキュリティリスクへの警戒](https://www.infosecurity-magazine.com/news/anubis-ransomware-adriatic-port/) | 28.0 | 30.0 | 42.0 |
| [オーストラリア第2位の砂糖生産者の製糖工場がランサムウェア攻撃で停止](https://www.securityweek.com/ransomware-attack-shuts-down-mills-of-australias-second-largest-sugar-producer/) | 28.0 | 30.0 | 42.0 |
| [Contiランサムウェアに関与したウクライナ国籍の男が有罪を認める](https://www.helpnetsecurity.com/2026/06/15/conti-ransomware-member-pleads-guilty/) | 28.0 | 30.0 | 42.0 |
| [米国でContiランサムウェア関連の罪を認めたウクライナ人男性](https://www.securityweek.com/ukrainian-man-pleads-guilty-in-us-to-conti-ransomware-charges/) | 28.0 | 30.0 | 42.0 |
| [中国系ハッカーがREDCapサーバーを通じて北米の研究機関に侵入](https://www.helpnetsecurity.com/2026/06/15/chinese-hackers-redcap-medical-research-institutions-breach/) | 28.0 | 20.0 | 42.0 |
| [セキュリティプログラムはNIS2要件に適合しているか](https://www.rapid7.com/blog/post/so-aligning-security-programmes-with-nis2-requirements) | 28.0 | 20.0 | 42.0 |
| [China-Nexus攻撃者が米国の研究者を1年間検知されずにスパイしていた](https://www.darkreading.com/threat-intelligence/china-nexus-actor-us-researchers-undetected) | 28.0 | 20.0 | 42.0 |
| [中国のハッカーがREDCapサーバーに侵入し、医療研究データを窃取](https://www.bleepingcomputer.com/news/security/chinese-hackers-breach-redcap-servers-steal-medical-research/) | 28.0 | 20.0 | 42.0 |
| [フランス政府のメッセージングプラットフォームが謎の「Misere」ハッカーに侵害される](https://www.securityweek.com/french-government-messaging-platform-breached-by-mysterious-misere-hacker/) | 28.0 | 20.0 | 42.0 |
| [PhishLumos：コンテンツを隠して検知を回避するフィッシングキャンペーンの実態解明](https://www.helpnetsecurity.com/2026/06/15/phishlumos-phishing-campaign-detection/) | 28.0 | 20.0 | 42.0 |
| [AIエージェントがネットワーク全体をスキャンしようとしてAWSから100万円以上の請求、運用していた人物が寄付を募る事態に](https://gigazine.net/news/20260615-dn42-ai-agent/) | 27.0 | 20.0 | 42.0 |
| [スコアを超えて：AIでCVEを実際のビジネスリスクに変換する方法](https://www.rapid7.com/blog/post/ai-beyond-the-score-translating-cves-into-real-business-risk) | 25.0 | 45.0 | 42.0 |
| [LiteLLMの脆弱性連鎖により低権限ユーザーがAIゲートウェイサーバーを乗っ取れる問題](https://thehackernews.com/2026/06/litellm-vulnerability-chain-lets-low.html) | 25.0 | 20.0 | 42.0 |
| [AnthropicのFable 5は特有の脅威ではないとサイバーセキュリティ専門家はみている](https://cyberscoop.com/cybersecurity-experts-anthropic-fable-5-not-unique-ai-threat/) | 25.0 | 20.0 | 42.0 |
| [ワンクリックでMicrosoft 365 Copilotの脆弱性によりメール、ファイル、MFAコードが盗まれる可能性](https://thehackernews.com/2026/06/one-click-microsoft-365-copilot-flaw.html) | 25.0 | 20.0 | 42.0 |
| [ソーシャルエンジニアリングの終焉の始まり](https://www.darkreading.com/cyberattacks-data-breaches/beginning-end-social-engineering) | 25.0 | 20.0 | 42.0 |
| [Cybersecurity専門家がAnthropicのAIモデル制限を行う米政府を批判](https://www.cybersecuritydive.com/news/anthropic-us-government-export-ban-mythos-fable/822909/) | 25.0 | 20.0 | 42.0 |
| [US政府の禁止措置後にClaude Fable 5とMythos 5が突然無効化](https://www.malwarebytes.com/blog/ai/2026/06/claude-fable-5-and-mythos-5-abruptly-disabled-after-us-gov-deems-them-too-clever) | 25.0 | 20.0 | 42.0 |
| [中国系ハッカーが北米の医療・軍事・AI研究を標的に攻撃](https://www.securityweek.com/chinese-hackers-target-medical-military-and-ai-research-in-north-america/) | 25.0 | 20.0 | 42.0 |
| [1Password Credential Brokerがアイデンティティベースの認証情報配信でシークレットの散在を削減](https://www.helpnetsecurity.com/2026/06/15/1password-credential-broker-reduces-secret-sprawl-through-identity-based-credential-delivery/) | 25.0 | 20.0 | 42.0 |
| [Trust3 AIのAgentDOSがAIエージェントの活動、データアクセス、トークン消費を監視](https://www.helpnetsecurity.com/2026/06/15/trust3-ais-agentdos-monitors-ai-agent-activity-data-access-and-token-consumption/) | 25.0 | 20.0 | 42.0 |
| [NewCoreがステルスモードを解除、6600万ドルの資金調達を発表](https://www.securityweek.com/newcore-emerges-from-stealth-mode-with-66-million-in-funding/) | 25.0 | 20.0 | 42.0 |
| [Microsoft 365 Copilotを1クリックでデータ窃取する攻撃手法に転用する新たな攻撃](https://www.bleepingcomputer.com/news/security/new-attack-turned-microsoft-365-copilot-into-1-click-data-theft-tool/) | 25.0 | 20.0 | 42.0 |
| [Omada Agent Governanceが組織のAIエージェントのアクセス、リスク、コンプライアンスを管理支援](https://www.helpnetsecurity.com/2026/06/15/omada-agent-governance/) | 25.0 | 20.0 | 42.0 |
| [Anthropic、米政府の要請でサイバーセキュリティ向けAIモデルを無効化と発表](https://therecord.media/anthropic-says-gov-forced-it-to-disable-cyber-ai-models) | 25.0 | 20.0 | 42.0 |
| [AnthropicのAIモデルに対する乱用懸念を受けた米国の取り締まり強化](https://www.darkreading.com/cyber-risk/us-cracks-down-anthropic-ai-models-abuse-concerns) | 25.0 | 20.0 | 42.0 |
| [AIによる脆弱性発見が2026年のCVEを66,000件へ押し上げる](https://www.helpnetsecurity.com/2026/06/15/first-2026-cve-forecast/) | 25.0 | 20.0 | 42.0 |
| [Cybersecurity専門家、USにAnthropicのFrontier AIモデル禁止解除を要請](https://www.infosecurity-magazine.com/news/cyber-experts-urge-us-lift-ban/) | 25.0 | 20.0 | 42.0 |
| [LTMのBlueVerse for iRunがマネージドIT運用にエージェンティックAIを適用](https://www.helpnetsecurity.com/2026/06/15/ltms-blueverse-for-irun-applies-agentic-ai-to-managed-it-operations/) | 25.0 | 20.0 | 42.0 |
| [英国政府、AIハッカソンで400件超の脆弱性を発見](https://www.infosecurity-magazine.com/news/uk-government-400-vulnerabilities/) | 25.0 | 20.0 | 42.0 |
| [Microsoft Defenderメールセキュリティのベンチマーク：1年間のデータから得られた主要な知見](https://www.microsoft.com/en-us/security/blog/2026/06/15/microsoft-defender-email-security-benchmarking-key-insights-from-one-year-of-data/) | 22.0 | 20.0 | 42.0 |
| [土木事務所で戸籍謄本などが所在不明 - 高知県](https://www.security-next.com/185691) | 22.0 | 20.0 | 42.0 |
| [「Node.<wbr>js」に重要度「高」の脆弱性 - 更新を予告](https://www.security-next.com/185893) | 22.0 | 20.0 | 42.0 |
| [イベント申込フォームで個人情報が閲覧可能に - 涌谷町](https://www.security-next.com/185462) | 22.0 | 20.0 | 42.0 |
| [市教委会議資料の個人情報にマスキング不備 - 川崎市](https://www.security-next.com/185746) | 22.0 | 20.0 | 42.0 |
| [海外グループ会社のメルアカに不正アクセス - 大気社](https://www.security-next.com/185811) | 22.0 | 20.0 | 42.0 |
| [「SimpleHelp」に認証回避の脆弱性 - 管理操作が可能に](https://www.security-next.com/185887) | 22.0 | 20.0 | 42.0 |
| [Maine、偽の報告を受けてデータ侵害ポータルを一般公開停止](https://therecord.media/maine-turns-off-breach-portal-fake-reports) | 20.0 | 20.0 | 42.0 |
| [ShinyHuntersによるPeopleSoft侵害で欧州評議会がハッキング被害](https://www.theregister.com/cyber-crime/2026/06/15/council-of-europe-hacked-in-shinyhunters-peoplesoft-heist/5255757) | 20.0 | 20.0 | 42.0 |
| [OptinMonster WordPressプラグインがCDNのサプライチェーン攻撃で改ざんされる](https://www.bleepingcomputer.com/news/security/optinmonster-wordpress-plugin-hacked-in-cdn-supply-chain-attack/) | 20.0 | 20.0 | 42.0 |
| [NIS2で高まる要求にどう備え、レジリエンスへつなげるか](https://www.rapid7.com/blog/post/so-nis2-compliance-turn-readiness-into-resilience) | 20.0 | 20.0 | 42.0 |
| [人気のWordPressプラグインを乗っ取ってバックドアを展開する攻撃者](https://www.infosecurity-magazine.com/news/wordpress-plugin-supply-chain/) | 20.0 | 20.0 | 42.0 |
| [米国データセンター法が失効へ、後継法案なく政府は対応遅れ](https://www.theregister.com/public-sector/2026/06/15/feds-snooze-as-us-datacenter-law-set-to-lapse-with-no-replacement-in-site/5255679) | 20.0 | 20.0 | 42.0 |
| [多くのCISOがセキュリティの悪いニュースを隠すよう圧力を受けている](https://www.darkreading.com/cyber-risk/most-cisos-report-pressure-to-bury-bad-security-news) | 20.0 | 20.0 | 42.0 |
| [欧州評議会、ShinyHuntersによるデータ侵害の主張を調査](https://www.bleepingcomputer.com/news/security/council-of-europe-investigates-shinyhunters-data-breach-claims/) | 20.0 | 20.0 | 42.0 |
| [Microsoftサイトで証明書の更新を忘れたため警告が表示される件](https://www.theregister.com/security/2026/06/15/microsoft-site-throwing-warnings-after-someone-forgot-to-renew-cert/5255597) | 20.0 | 20.0 | 42.0 |
| [FBI、仮想通貨詐欺で配達員を使って現金をだまし取る手口を警告](https://www.bleepingcomputer.com/news/security/fbi-fraudsters-use-couriers-to-steal-money-in-crypto-scams/) | 20.0 | 20.0 | 42.0 |
| [中国関連のスパイが認証スタックにバックドアを仕掛け、数年間潜伏していた件](https://www.helpnetsecurity.com/2026/06/15/velvet-ant-backdoored-authentication-persistence/) | 20.0 | 20.0 | 42.0 |
| [ロシアの技術企業Astralへのサイバー攻撃でビジネスと政府サービスが1週間停止](https://therecord.media/cyberattack-on-russian-tech-firm-astral-disrupts-business-government-services) | 20.0 | 20.0 | 42.0 |
| [DelineaとCyeraが連携し、データを意識したアイデンティティセキュリティを実現](https://www.helpnetsecurity.com/2026/06/15/delinea-cyera-product-integration/) | 20.0 | 20.0 | 42.0 |
| [ディープフェイクポルノサイトが相次いで閉鎖へ（再放送）](https://www.malwarebytes.com/blog/podcast/2026/06/deepfake-porn-sites-are-going-offline-re-air-lock-and-code-s07e12) | 20.0 | 20.0 | 42.0 |
| [Vibe codersが生み出すコードスパrawlへのCISOの対策](https://www.bleepingcomputer.com/news/security/vibe-coders-are-gonna-vibe-code-how-cisos-are-tackling-code-sprawl/) | 20.0 | 20.0 | 42.0 |
| [Arch Linux、悪意あるコミットの増加を受けAURの新規登録を制限](https://www.theregister.com/security/2026/06/15/arch-linux-locks-down-aur-signups-amid-wave-of-malicious-commits/5255511) | 20.0 | 20.0 | 42.0 |
| [Maine州、虚偽の通報提出を受けデータ侵害ポータルを停止](https://www.bitdefender.com/en-us/blog/hotforsecurity/maine-take-down-data-breach-portal) | 20.0 | 20.0 | 42.0 |
| [Infinite Campusのデータ侵害で13万7000件の学校職員アカウントに影響](https://www.bleepingcomputer.com/news/security/infinite-campus-data-breach-affects-137-000-school-staff-accounts/) | 20.0 | 20.0 | 42.0 |
| [Red SiftとGMO GlobalSignの提携でメール認証とBIMI導入を簡素化](https://www.helpnetsecurity.com/2026/06/15/globalsign-red-sift-partnership/) | 20.0 | 20.0 | 42.0 |
| [MS-ISAC、連邦資金と多数のメンバー失い不透明な新時代へ](https://www.cybersecuritydive.com/news/ms-isac-membership-loss-states-federal-funding-cut/821984/) | 20.0 | 20.0 | 42.0 |
| [オンボーディング時のパスワード設定ミスが生む不要なリスク](https://thehackernews.com/2026/06/the-onboarding-password-mistake-that.html) | 20.0 | 20.0 | 42.0 |
| [Ozempic製造元のNovo NordiskがITシステムへの不正侵入を公表](https://www.securityweek.com/ozempic-maker-novo-nordisk-says-hackers-breached-it-systems/) | 20.0 | 20.0 | 42.0 |
| [152件のChrome壁紙拡張機能、10万5000件のインストールがアドウェアと偽トラフィックに関連付けられる](https://thehackernews.com/2026/06/152-chrome-wallpaper-extensions-with.html) | 20.0 | 20.0 | 42.0 |
| [ShinyHuntersが欧州評議会への侵入を主張](https://www.securityweek.com/shinyhunters-claims-council-of-europe-hack/) | 20.0 | 20.0 | 42.0 |
| [Modat、MagnifyにPassive DNSを追加し脅威ハンティングとインフラ分析を高速化](https://www.helpnetsecurity.com/2026/06/15/modat-enhances-magnify-with-passive-dns-for-faster-threat-hunting-and-infrastructure-analysis/) | 20.0 | 20.0 | 42.0 |
| [MicrosoftのWi-Fiによる職場チェックインがオフィス在席者を追跡し、全員が歓迎しているわけではない](https://www.helpnetsecurity.com/2026/06/15/microsoft-teams-workplace-wi-fi-check-in/) | 20.0 | 20.0 | 42.0 |
| [人気のWordPressプラグインのスクリプトが改ざんされ、サイトに隠しバックドアを仕込む手口が確認される](https://thehackernews.com/2026/06/popular-wordpress-plugin-scripts.html) | 20.0 | 20.0 | 42.0 |
| [FBIとGoogleが「Outsider Enterprise」フィッシングサービスを解体](https://www.securityweek.com/fbi-google-dismantle-outsider-enterprise-phishing-service/) | 20.0 | 20.0 | 42.0 |
| [Maine州、偽の入力を受けて侵害報告ポータルを停止](https://www.infosecurity-magazine.com/news/maine-breach-reporting-portal/) | 20.0 | 20.0 | 42.0 |
| [Maine州、偽の申請によりデータ侵害ポータルを停止](https://www.securityweek.com/maine-disables-data-breach-portal-due-to-fake-submissions/) | 20.0 | 20.0 | 42.0 |

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
