# 📡 サイレーダー 2026-09-29 05:00 JST

このレポートは、2026-09-28 17:00 JST〜2026-09-29 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 86
- [音声で扱う想定のトピック](#audio-topics): 10
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 51

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Dutch Police Arrest ‘Reformed’ Hacker in Shiny Hunters Investigation](#topic-16788) | 56.0 | 77.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [注意喚起: NetScaler ADCおよびNetScaler Gatewayにおける複数の脆弱性（CVE-2026-88771、CVE-2026-88772等）に関する注意喚起 (公開)](#topic-34525) | 47.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [Citrix Patches Critical Zero Days Under Active Exploitation](#topic-34744) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [US, UK warn of exploited Citrix NetScaler zero-day bugs](#topic-34675) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [Citrix urges immediate upgrades of NetScaler amid widespread exploitation attempts](#topic-34679) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [FBI job portals remain offline after ShinyHunters claims breach via PeopleSoft zero-day](#topic-34688) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 7 | [Exploitation of vulnerabilities affecting Citrix NetScaler ADC and Citrix NetScaler Gateway](#topic-34707) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 8 | [JadePuffer agentic AI attacks target Azure, destroy cloud resources](#topic-34676) | 33.0 | 30.0 | 42.0 | 音声 | AI×Security枠 |
| 9 | [RatHat Android Malware Console Uses Gemini to Identify Higher-Value Victims](#topic-34670) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 10 | [CLOSEDQUORUM: Malware Puts AI in the C2 Loop](#topic-34672) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-16788"></a>

### 1. Dutch Police Arrest ‘Reformed’ Hacker in Shiny Hunters Investigation

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 56.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 77.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

オランダ警察が、ShinyHuntersに関する捜査の一環として、データ窃取や恐喝への関与が疑われる人物を逮捕したと報じられています。
関連する動きとして、Oracle PeopleSoftの深刻な脆弱性CVE-2026-35273が悪用されているとされ、複数の組織が影響を受ける可能性が示されています。
この件は、脅威アクターの摘発と並行して実際の攻撃活動が続いていることを示しており、被害の拡大や手口の変化に注意が必要です。
CVE-2026-35273は既知の悪用対象として扱われているため、対象製品を使う組織にとって優先度の高い対応事項です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 10 sources。
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

- Oracle PeopleSoft環境でCVE-2026-35273への対処状況を確認し、ベンダーの修正情報や推奨対策を適用する。
- 外部公開されている管理系・業務系システムについて、認証不要で到達可能な経路がないか棚卸しする。
- 侵害の兆候として、異常なアクセス、設定変更、Webシェルの存在など基本的な監視項目を再点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-35273 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-41091 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-45657 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-50507 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ランサムウェアグループ | Clop | 主題 | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Oracle | 言及あり | 0.80 | — |
| 脅威アクター | Scattered Spider | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-35273](https://nvd.nist.gov/vuln/detail/CVE-2026-35273) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Dutch Police Arrest ‘Reformed’ Hacker in Shiny Hunters Investigation](https://krebsonsecurity.com/2026/09/dutch-police-arrest-reformed-hacker-in-shiny-hunters-investigation/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Bypass WAFs to Exploit Oracle PeopleSoft Flaw and Deploy Web Shells](https://thehackernews.com/2026/09/attackers-bypass-wafs-to-exploit-oracle.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [15th June – Threat Intelligence Report](https://research.checkpoint.com/2026/15th-june-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShinyHunters is actively extorting universities after exploiting an unpatched Or](https://cyberscoop.com/oracle-peoplesoft-zero-day-vulnerability-shinyhunters-extortion/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Active Exploitation of Oracle PeopleSoft Zero-Day (CVE-2026-35273)](https://www.rapid7.com/blog/post/etr-active-exploitation-of-oracle-peoplesoft-zero-day-cve-2026-35273) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/06/12/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google Confirms Exploitation of Oracle PeopleSoft Zero-Day by ShinyHunters](https://www.securityweek.com/google-confirms-exploitation-of-oracle-peoplesoft-zero-day-by-shinyhunters/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-34525"></a>

### 2. 注意喚起: NetScaler ADCおよびNetScaler Gatewayにおける複数の脆弱性（CVE-2026-88771、CVE-2026-88772等）に関する注意喚起 (公開)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 47.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Citrix NetScaler ADCおよびNetScaler Gatewayに関する複数の脆弱性について、少なくともCVE-2026-88771とCVE-2026-88772は実際に悪用されていると複数の公開情報で伝えられています。
JPCERT/CCも注意喚起を出しており、該当製品を利用する組織では更新状況の確認と影響有無の点検が重要です。
境界系製品に対するRCE脆弱性の悪用は、認証情報や社内ネットワークへの侵入につながるおそれがあるためです。
公開情報上、ゼロデイとしての悪用観測が示されており、優先度の高い対応対象と見られます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 7 sources。
- 実悪用・ゼロデイ文脈。
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

- Citrixの案内に沿って、該当バージョンの影響有無と修正パッチ適用状況を確認する。
- NetScaler ADC/Gatewayの管理画面や設定、ログに不審なアクセスや改ざんの痕跡がないか点検する。
- 外部公開しているNetScaler環境がある場合は、暫定的な露出範囲の見直しと監視強化を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-88771 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-88772 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-88771](https://nvd.nist.gov/vuln/detail/CVE-2026-88771) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: NetScaler Zero Days CVE-2026-88771 and CVE-2026-88772 Exploited in](https://unit42.paloaltonetworks.com/netscaler-zero-days-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-88771 and CVE-2026-88772: Two Critical Citrix NetScaler Flaws Under Act](https://www.bitsight.com/blog/critical-vulnerability-alert-cve-2026-88771-cve-2026-88772-citrix-netscaler-flaws-under-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zero-Day Exploitation of Citrix NetScaler ADC and Gateway: CVE-2026-88771 and CV](https://www.rapid7.com/blog/post/etr-zero-day-exploitation-of-citrix-netscaler-adc-and-gateway-cve-2026-88771-and-cve-2026-88772) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix NetScaler RCE zero-days exploited globally for weeks (CVE-2026-88771, CVE](https://www.helpnetsecurity.com/2026/09/28/citrix-netscaler-rce-zero-days-exploited-for-weeks-cve-2026-88771-cve-2026-88772/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: NetScaler ADCおよびNetScaler Gatewayにおける複数の脆弱性（CVE-2026-88771、CVE-2026-88772等](https://www.jpcert.or.jp/at/2026/at260029.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix Confirms 2 NetScaler Zero-Days After Admins Pulled the Plug](https://www.securityweek.com/citrix-confirms-2-netscaler-zero-days-after-admins-pulled-the-plug/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix confirms two NetScaler RCE zero-days exploited in attacks](https://www.bleepingcomputer.com/news/security/citrix-admins-warned-to-shut-down-netscalers-over-2-exploited-zero-days/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（1件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-34744"></a>

### 3. Citrix Patches Critical Zero Days Under Active Exploitation

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Citrixが、実際に悪用されている2件の重大なゼロデイ脆弱性に対する修正を公表しました。
公開情報では、いずれもRCEに関わる問題とされていますが、影響範囲や詳細な悪用状況は確認できる範囲に限られています。
ゼロデイかつ実悪用が確認されているため、放置すると侵入や侵害につながる可能性があります。Citrix製品を利用する組織では、緊急度の高い対応対象として扱う必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象となるCitrix製品とバージョンを確認し、修正パッチの適用状況を点検する。
- 公開情報に基づき、関連ログや不審な認証・接続・管理操作の有無を確認する。
- 外部公開しているCitrix関連サービスがあれば、暫定的な保護策やアクセス制御の見直しを優先する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Citrix | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Citrix Patches Critical Zero Days Under Active Exploitation](https://www.infosecurity-magazine.com/news/citrix-patches-critical-zero-days/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34675"></a>

### 4. US, UK warn of exploited Citrix NetScaler zero-day bugs

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Citrix NetScaler Gatewayに関する新たな脆弱性について、各国のサイバー当局が注意喚起を出し、Citrixも複数の脆弱性を確認したとされています。
報告内容では、ゼロデイとして悪用された可能性がある文脈で扱われており、運用中の製品利用者は影響確認が必要です。
認証やリモート接続の入口に使われやすい製品での脆弱性は、侵入の足がかりになりやすいため注目されています。公的機関が注意喚起している点からも、対応の優先度が高い話題です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当するCitrix NetScaler Gatewayの利用有無と、バージョン・構成を早急に確認する。
- Citrixおよび各国当局の修正・緩和策の案内を確認し、適用可否を判断する。
- 認証ログや管理系アクセスの異常、想定外の設定変更など、周辺の不審兆候を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [US, UK warn of exploited Citrix NetScaler zero-day bugs](https://therecord.media/us-uk-warn-of-citrix-netscaler-zero-day-bug) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34679"></a>

### 5. Citrix urges immediate upgrades of NetScaler amid widespread exploitation attempts

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CitrixがNetScalerの更新を急ぐよう呼びかけており、関連製品に対する広範な悪用試行が観測されているとされています。
公的な確認が進む前から、セキュリティチームに対して迅速な対応が求められる状況です。NetScalerは組織の外部公開面に置かれることが多く、侵害されると影響が大きくなり得ます。
悪用観測がある段階では、未修正環境のリスク評価と優先対応が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象のNetScaler環境を棚卸しし、ベンダー案内に沿って優先度高く更新状況を確認する。
- 外部公開している装置について、異常な認証失敗や不審なアクセス傾向を監視し、必要に応じて一時的な保護策を検討する。
- 公式の修正情報や注意喚起を継続監視し、影響範囲がある場合は関連サービスへの波及を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Citrix | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Citrix urges immediate upgrades of NetScaler amid widespread exploitation attemp](https://www.cybersecuritydive.com/news/citrix-upgrades-netscaler-exploitation/831502/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34688"></a>

### 6. FBI job portals remain offline after ShinyHunters claims breach via PeopleSoft zero-day

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

FBIの採用関連ポータルが、ShinyHuntersによる侵害主張の後も停止したままであると報じられています。
ShinyHuntersは、Oracle PeopleSoftの未確認のゼロデイ脆弱性を使ったと主張していますが、現時点ではその詳細は確認されていません。
米国の捜査機関に関連する公開向けサービスが影響を受けている可能性があり、信頼性や可用性の観点で注目されています。
ゼロデイを伴うとされる主張は、関連製品を利用する組織にとっても警戒材料になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- PeopleSoftなど外部公開システムの停止・異常を監視し、業務継続手順を確認する。
- ベンダーの更新情報や公的機関の続報を追い、未確認情報を前提にした判断を避ける。
- 採用・申請ポータルのような公開系システムでは、認証、ログ監視、権限管理の点検を改めて行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-35273 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| ベンダー | Oracle | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [FBI job portals remain offline after ShinyHunters claims breach via PeopleSoft z](https://www.helpnetsecurity.com/2026/09/28/fbi-job-portals-offline-shinyhunters-breach/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34707"></a>

### 7. Exploitation of vulnerabilities affecting Citrix NetScaler ADC and Citrix NetScaler Gateway

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

英国NCSCは、Citrix NetScaler ADCおよびCitrix NetScaler Gatewayに影響する脆弱性について、組織に速やかな対処を呼びかけています。
公表内容では、少なくとも2件の脆弱性が実際に悪用されているとされています。境界機器にあたる製品での脆弱性は、影響範囲が広くなりやすく、対応の遅れがそのままリスクにつながります。
悪用観測があるため、通常の定期対応ではなく優先度を上げて確認する必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当するCitrix NetScaler ADC / Gatewayの導入有無を確認し、ベンダーの修正情報と影響範囲を至急照合する。
- 公開情報で悪用観測があるため、パッチ適用や緩和策の適用を前倒しで進める。
- 外部公開面の監視、認証・管理系ログの確認、異常なアクセスの有無を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Exploitation of vulnerabilities affecting Citrix NetScaler ADC and Citrix NetSca](https://www.ncsc.gov.uk/news/exploitation-of-vulnerabilities-affecting-citrix-netscaler-adc-and-citrix-netscaler-gateway) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34676"></a>

### 8. JadePuffer agentic AI attacks target Azure, destroy cloud resources

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>A⁠I</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

JadePufferと呼ばれる脅威アクターが、Azure環境を狙ったAIエージェント型の攻撃を行っているとされています。
公開情報では、偵察、認証情報の窃取、クラウドの中核コンポーネント破壊につながる活動が示唆されています。
クラウド環境に対する攻撃が、従来の侵入やランサムウェアに加えてAIの自動化で加速する可能性があるためです。
Azure利用組織にとっては、アカウント保護とリソース保全の重要性を改めて示す事例です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Azureの特権アカウントと認証情報の保護を優先し、多要素認証や権限最小化を確認する。
- クラウド管理操作や重要リソースの変更を監視し、異常な偵察・削除・権限変更の兆候を検知できるようにする。
- ランサムウェアを含む破壊的事象を想定し、バックアップと復旧手順が実際に機能するか定期的に検証する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脅威アクター | JadePuffer | 主題 | 0.80 | — |
| 製品 | Microsoft Azure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [JadePuffer agentic AI attacks target Azure, destroy cloud resources](https://www.bleepingcomputer.com/news/security/jadepuffer-agentic-ai-attacks-target-azure-destroy-cloud-resources/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34670"></a>

### 9. RatHat Android Malware Console Uses Gemini to Identify Higher-Value Victims

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠n⁠d⁠r⁠o⁠i⁠d</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Android向け銀行系トロイの木馬とされるRatHatの運用で、攻撃者側のWebコンソールにGeminiが使われ、収集情報からより価値の高い被害者を見分ける用途が示されたと報じられています。
Security企業Cleafyは、このコンソールの展開が複数確認されており、MaaS型の運用形態に近いとしています。
AIが脅威運用の効率化に使われる例として、検知や被害評価の難しさが増す可能性があります。
モバイル端末や銀行系認証情報を狙うマルウェアの運用が、より組織的・継続的になっている点も注目されます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- モバイル端末向けの不審な権限要求や配布経路を点検し、導入アプリの監視を強化する。
- 端末上の情報収集や外部送信の兆候を前提に、EDR/MDMや通信監視のルールを見直す。
- 銀行系・認証系の利用者に対して、多要素認証や取引確認の手順を再周知する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| AIモデル/プロジェクト | Gemini | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [RatHat Android Malware Console Uses Gemini to Identify Higher-Value Victims](https://thehackernews.com/2026/09/rathat-android-malware-console-uses.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34672"></a>

### 10. CLOSEDQUORUM: Malware Puts AI in the C2 Loop

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Cisco Talosの分析によると、CLOSEDQUORUMはWindows向けのマルウェアで、攻撃の一部に商用LLMを組み込み、C2の判断を外部AIに委ねる設計が確認されています。
報告では、複数のLLM提供元を参照してあらかじめ用意された悪性動作を選択し、結果や取得情報をDiscordに送る構成が示されています。
従来型の攻撃者管理サーバーに依存しない形で、AIサービスを攻撃チェーンの一部に使う例として注目されます。
実運用の有無は未確認でも、脅威の自動化と運用負荷の低減という観点で示唆があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIサービスを悪用した通信や不審な連携先がないか、エンドポイントとプロキシの監視観点を見直す。
- LLM利用を前提にした新しい手口として、既存のC2検知だけでなく挙動ベースの検知を強化する。
- 外部サービスとのやり取りが増えた際に備え、アプリケーション制御と権限管理を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | DeepSeek | 言及あり | 0.80 | — |
| ベンダー | Mistral AI | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Qwen | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CLOSEDQUORUM: Malware Puts AI in the C2 Loop](https://blog.polyswarm.io/closedquorum-malware-puts-ai-in-the-c2-loop) | <nobr>内容確認・補足情報</nobr> |

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
| [JadePufferによるAzureテナント侵害と破壊的クラウド攻撃](https://www.darkreading.com/cloud-security/jadepuffer-ai-actor-azure-tenant-destructive-cloud-attack) | 33.0 | 20.0 | 42.0 |
| [CarbonatoボットネットがDockerホストを侵害しTelegram制御のHermes AIエージェントを展開](https://thehackernews.com/2026/09/carbonato-botnet-compromises-docker.html) | 33.0 | 20.0 | 42.0 |
| [NeedyMantis：標的型攻撃で使用された侵害後マルウェアファミリーの解明](https://www.microsoft.com/en-us/security/blog/2026/09/28/needymantis-unpacking-a-post-compromise-malware-family-used-in-targeted-operations/) | 30.0 | 20.0 | 42.0 |
| [元兵士の通信会社ハッキング連発で70か月の実刑](https://www.theregister.com/cyber-crime/2026/09/28/ex-soldiers-telecom-hacking-spree-earns-him-70-months/5299440) | 28.0 | 20.0 | 42.0 |
| [Googleが警告したShinyHuntersによるOracle PeopleSoftへの新たな攻撃キャンペーン](https://www.securityweek.com/google-warns-of-shinyhunters-fresh-oracle-peoplesoft-campaign/) | 28.0 | 20.0 | 42.0 |
| [JADEPUFFER関連の攻撃者が侵害されたサービス プリンシパルを使ってAzureリソースを削除した件](https://thehackernews.com/2026/09/jadepuffer-linked-attackers-used.html) | 28.0 | 20.0 | 42.0 |
| [OpenAIはAIトレーニングに違法な海賊版書籍を使うことが危険であり作家の生活を脅かすと認識していたと裁判文書で明らかに](https://gigazine.net/news/20260928-openai-microsoft-know-book-piracy-illegal/) | 27.0 | 20.0 | 42.0 |
| [次期指導要領の全体像固まる 情報学習強化、英語でAI導入が柱](https://www.itmedia.co.jp/news/article/2609/28/2000001818/) | 26.0 | 20.0 | 42.0 |
| [OpenAI、研究用AIエージェントがDNSの抜け穴を利用して外部チャットボットに接続](https://news.mynavi.jp/techplus/article/20260928-5041662/) | 26.0 | 20.0 | 42.0 |
| [NTTドコモビジネス、「AI-Centric ICTプラットフォーム」による実装力を訴求](https://japan.zdnet.com/article/35253043/) | 26.0 | 20.0 | 42.0 |
| [オープンソースのAIセキュリティエージェントで24件のAndroid脆弱性を発見した方法](https://github.blog/security/how-we-found-24-android-vulnerabilities-using-our-open-source-ai-security-agent/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントは特権ユーザー：そのアクセスは誰が監査しているのか](https://www.darkreading.com/vulnerabilities-threats/ai-agents-are-privileged-users-who-is-auditing-their-access) | 25.0 | 20.0 | 42.0 |
| [AIの安全性が議論される中、NVIDIAがエージェント向けのオープンソースツールを公開](https://cyberscoop.com/nvidia-open-agent-safety-platform/) | 25.0 | 20.0 | 42.0 |
| [AIエージェント向けIAMの実践的なエンタープライズフレームワーク](https://thehackernews.com/2026/09/iam-for-ai-agent.html) | 25.0 | 20.0 | 42.0 |
| [ModulateがDeepfake検出の高度化に向けて2500万ドルを調達](https://www.securityweek.com/modulate-raises-25-million-to-advance-deepfake-detection/) | 25.0 | 20.0 | 42.0 |
| [ニッチなAIツールがインフラ運用者にもたらす重大なサイバーセキュリティリスク](https://www.cybersecuritydive.com/news/ai-apps-niche-cybersecurity-risk-trendai/831486/) | 25.0 | 20.0 | 42.0 |
| [Weekly Recap: 3億8700万ドル規模の暗号資産ハック、Citrixの脆弱性悪用、AIエージェントの逸脱行動などの脅威まとめ](https://thehackernews.com/2026/09/weekly-recap-387m-crypto-hack-citrix.html) | 25.0 | 20.0 | 42.0 |
| [80,000以上の組織でAIログイン情報が窃取される：Shadow AIからLLMjackingへ](https://www.bleepingcomputer.com/news/security/80-000-plus-organizations-had-ai-logins-stolen-from-shadow-ai-to-llmjacking/) | 25.0 | 20.0 | 42.0 |
| [OpenAIがインターネット制御をすり抜けたagentを受け、最上位AIモデルの開発を一時停止](https://www.malwarebytes.com/blog/ai/2026/09/openai-pauses-work-on-top-ai-models-after-agent-slips-past-internet-controls) | 25.0 | 20.0 | 42.0 |
| [NVIDIAがAIエージェントの安全性をソフトウェア任せにせずシリコンで強制することを提唱](https://www.helpnetsecurity.com/2026/09/28/nvidia-open-agent-safety-platform/) | 25.0 | 20.0 | 42.0 |
| [酔っぱらい”AIは秘密保持が苦手である](https://www.helpnetsecurity.com/2026/09/28/drunk-ai-models-jailbreak-research/) | 25.0 | 20.0 | 42.0 |
| [Nvidia、ハードウェアベースの監視機能を備えたAIエージェント安全性プラットフォームを発表](https://www.securityweek.com/nvidia-unveils-ai-agent-safety-platform-with-hardware-based-watchdog/) | 25.0 | 20.0 | 42.0 |
| [MCPが重大なガバナンス上の空白を生んでいると研究者が警告](https://www.infosecurity-magazine.com/news/mcp-creating-major-governance-gaps/) | 25.0 | 20.0 | 42.0 |
| [サイバーセキュリティにおけるエージェント型運用モデルは文脈が重要](https://www.cybersecuritydive.com/spons/context-matters-when-it-comes-to-cybersecuritys-agentic-operating-model/830973/) | 25.0 | 20.0 | 42.0 |
| [AI主導の攻撃者に追いつくためのセキュリティテストの進化](https://www.cybersecuritydive.com/spons/security-testing-has-to-keep-pace-with-ai-driven-attackers/830603/) | 25.0 | 20.0 | 42.0 |
| [Kiteworksが顧客にシステム停止を促した予防的警告を解除](https://www.cybersecuritydive.com/news/kiteworks-lifts-advisory-warning-shut-zero-day/831508/) | 22.0 | 20.0 | 43.0 |
| [教員5人のアカウントに不正アクセス、スパムの踏み台に - 日大](https://www.security-next.com/190319) | 22.0 | 20.0 | 42.0 |
| [最先端AIモデルの「思考しすぎてコスト増加」を解決するべくKimi K3ベースで開発されたAIモデル「Ember-1」が登場](https://gigazine.net/news/20260928-ember-1-fireworks/) | 22.0 | 20.0 | 42.0 |
| [事業所担当者向けの説明会連絡メールで誤送信 - 愛媛労働基準協会](https://www.security-next.com/190739) | 22.0 | 20.0 | 42.0 |
| [FBI職員の血液検査結果と診断メモが漏えい後に流出](https://www.malwarebytes.com/blog/data-breaches/2026/09/fbi-agents-blood-tests-and-doctors-notes-surface-after-breach) | 20.0 | 20.0 | 48.0 |
| [設定不備のSupabaseアプリで1万6000件超のデータベースがデータ公開状態に](https://www.bleepingcomputer.com/news/security/misconfigured-supabase-apps-expose-data-in-over-16-000-databases/) | 20.0 | 20.0 | 42.0 |
| [Bitget、第三者セキュリティ製品の欠陥を悪用され3億8800万ドルを盗まれる](https://thehackernews.com/2026/09/bitget-says-attacker-exploited-third.html) | 20.0 | 20.0 | 42.0 |
| [Chrome Storeで「Poper Blocker」を装うスパイウェアが数百万回ダウンロードされる](https://www.darkreading.com/application-security/chrome-store-poper-blocker-spyware-downloaded-millions) | 20.0 | 20.0 | 42.0 |
| [2026 CISO Forum Virtual Summitの講演募集開始](https://www.securityweek.com/call-for-presentations-open-for-2026-ciso-forum-virtual-summit/) | 20.0 | 20.0 | 42.0 |
| [Bitget、3億8750万ドルのウォレット侵害後にBitcoin出金を再開](https://www.infosecurity-magazine.com/news/bitget-restarts-withdrawals-387-5m/) | 20.0 | 20.0 | 42.0 |
| [ShinyHunters、FBIとの無謀な意地の張り合いへと方針転換し金銭恐喝から離脱](https://cyberscoop.com/fbi-data-breach-shinyhunters-agent-safety-risk/) | 20.0 | 20.0 | 42.0 |
| [NetScaler ADCおよびNetScaler Gatewayの複数の脆弱性によりリモートコード実行が可能になるおそれ](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-netscaler-adc-and-netscaler-gateway-could-allow-for-remote-code-execution_2026-103) | 20.0 | 20.0 | 42.0 |
| [16歳の研究者がMicrosoftの分析サービスに侵入し、17兆行のデータにアクセス](https://www.helpnetsecurity.com/2026/09/28/microsoft-titan-jwt-signature-flaw/) | 20.0 | 20.0 | 42.0 |
| [ポーランドの医療ソフトウェア提供企業へのサイバー攻撃で患者データが流出](https://therecord.media/poland-cyberattack-medical-medyc) | 20.0 | 20.0 | 42.0 |
| [Deepfakeが企業にもたらす高額な現実、報告書が警告](https://www.infosecurity-magazine.com/news/deepfakes-costly-reality-for/) | 20.0 | 20.0 | 42.0 |
| [Akamai、Athena Coalitionに参加し新たな脆弱性から利用者を保護](https://www.akamai.com/blog/security-research/2026/sep/akamai-joins-athena-coalition-shield-users-vulnerabilities) | 20.0 | 20.0 | 42.0 |
| [元米軍兵士がAT&TとVerizonをハッキングし懲役刑に処される](https://www.securityweek.com/prison-sentence-for-former-us-soldier-who-hacked-att-and-verizon/) | 20.0 | 20.0 | 42.0 |
| [OSのファイル通知を通じて他のユーザーが閲覧内容を監視し、キー入力のタイミングを推測できる問題](https://www.helpnetsecurity.com/2026/09/28/cve-2025-68788-file-notification-attacks/) | 20.0 | 20.0 | 42.0 |
| [DC Health Agency、40万件の受給者記録を公開状態にしていた](https://www.securityweek.com/dc-health-agency-exposes-400000-beneficiary-records/) | 20.0 | 20.0 | 42.0 |
| [New Mexico陪審、Facebookのプライバシー保護に関する欺瞞を認定](https://www.securityweek.com/new-mexico-jury-finds-facebook-liable-for-deceiving-users-about-privacy-protections/) | 20.0 | 20.0 | 42.0 |
| [画像ではない画像—SVGを悪用した攻撃を防ぐ](https://www.security.com/expert-perspectives/image-isnt-stopping-svg-borne-attacks) | 20.0 | 20.0 | 42.0 |
| [Kiteworksがサーバー停止を要請、Advanced Formsの脆弱性を確認](https://www.securityweek.com/kiteworks-urges-server-shutdown-finds-advanced-forms-vulnerability/) | 20.0 | 20.0 | 42.0 |
| [Bitget、3億8750万ドル規模の暗号資産流出後にBitcoin出金を再開](https://www.bleepingcomputer.com/news/security/bitget-resumes-bitcoin-withdrawals-after-3875-million-crypto-heist/) | 20.0 | 20.0 | 42.0 |
| [攻撃対象領域は思っているより広く、ハッカーはそれを知っている](https://www.cybersecuritydive.com/spons/your-attack-surface-is-bigger-than-you-think-and-hackers-know-that/830809/) | 20.0 | 20.0 | 42.0 |
| [元米兵、AT&TとSnowflakeのデータ窃取への関与で70か月の刑に](https://www.helpnetsecurity.com/2026/09/28/us-army-soldier-snowflake-breaches-extortion/) | 20.0 | 20.0 | 42.0 |
| [LinkedInがつながりによる職歴確認機能をテスト](https://www.helpnetsecurity.com/2026/09/28/linkedin-profile-verification-features/) | 20.0 | 20.0 | 42.0 |

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
