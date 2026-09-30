# 📡 サイレーダー 2026-10-01 05:00 JST

このレポートは、2026-09-30 17:00 JST〜2026-10-01 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 84
- [音声で扱う想定のトピック](#audio-topics): 8
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 51

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-76504: CISA KEV catalog addition](#topic-35199) | 65.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [Higher education is under siege, and fragmented security is making it harder to respond](#topic-35204) | 53.0 | 48.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Government, Finance Orgs Targeted in Weeks-Long NetScaler Zero-Day Attacks](#topic-34525) | 52.0 | 74.0 | 67.0 | 音声 | 温度感上位枠 |
| 4 | [Apple Patches CoreGraphics Zero Day Exploited in Attacks](#topic-34785) | 45.0 | 46.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 5 | [Bitget hacked via zero-day in third-party security products](#topic-35236) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [Vulnerability Discovery and Exploitation Trends in the AI Era](#topic-35209) | 37.0 | 20.0 | 43.0 | 音声 | AI×Security枠 |
| 7 | [Attackers Abuse ChatGPT Custom GPTs to Deliver RAT via ClickFix Lures](#topic-35202) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 8 | [Attackers Combine ChatGPT Feature Abuse With ClickFix to Deliver Trojan Malware](#topic-35230) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 9 | [Suspected state-sponsored hackers exploited NetScaler zero-day since early September (CVE-2026-88772)](#topic-35219) | 30.0 | 20.0 | 43.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-35199"></a>

### 1. CVE-2026-76504: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 65.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

CISAは、Cisco Catalyst SD-WAN Managerに関するCVE-2026-76504をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
公開情報では、この脆弱性は認証回避につながる可能性があり、実際の悪用が観測されているとされています。Ciscoは修正版を案内しており、現時点で回避策はないとされています。
KEVへの追加は、当該脆弱性がすでに攻撃者の標的になっていることを示すため、優先度の高い対応が必要になります。
SD-WAN管理基盤が影響を受けるため、ネットワーク運用全体への波及も懸念されます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Cisco Catalyst SD-WAN Managerの利用有無を確認し、該当する場合は修正版の適用状況を早急に点検する。
- 管理インターフェースやAPIへの到達経路、外部公開の有無を確認し、不要な露出を抑える。
- 関連ログを確認し、不審なAPIアクセスや認証を伴わない管理操作の兆候がないかを点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-76504 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Catalyst SD-WAN Manager | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-76504](https://nvd.nist.gov/vuln/detail/CVE-2026-76504) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Warns of Attackers Exploiting Critical Authentication Bypass in SD-WAN Man](https://thehackernews.com/2026/09/cisco-warns-of-attackers-exploiting.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Cisco Catalyst SD-WAN Manager API authentication bypass exploited in th](https://www.rapid7.com/blog/post/etr-critical-cisco-catalyst-sd-wan-manager-api-authentication-bypass-exploited-in-the-wild-cve-2026-76504) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of new SD-WAN zero-day exploited in attacks](https://www.bleepingcomputer.com/news/security/cisco-warns-of-new-sd-wan-authentication-bypass-zero-day-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Manager API Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-webauth-xr8beuuU) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/09/30/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-35204"></a>

### 2. Higher education is under siege, and fragmented security is making it harder to respond

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 53.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

高等教育機関は、学生情報や研究データなど機微な情報を大量に抱える一方で、開放的なネットワークや分散した利用者、レガシー環境を抱えており、サイバー攻撃の対象になりやすい状況にあります。
特にマルチキャンパスの大学では、セキュリティ運用が分断されていると、脅威情報やインシデント対応の連携が遅れ、被害の把握や封じ込めが難しくなると指摘されています。
教育分野では攻撃件数や被害額が大きく、ランサムウェアが授業や研究、事務運営に直接影響しうるためです。
組織内の可視性と連携の不足が、単独のインシデントを学内全体のリスクに広げる可能性があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- キャンパス単位で分かれた検知・対応手順を見直し、学内横断で脅威情報を共有できる体制を整える。
- 資産管理、脆弱性対応、パッチ適用の進捗を組織全体で把握し、対応の抜けを減らす。
- 重複しやすいツールや運用を棚卸しし、限られた人員で広い環境を監視できるよう優先順位を整理する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脅威アクター | Equation | 主題 | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Higher education is under siege, and fragmented security is making it harder to ](https://www.rapid7.com/blog/post/it-higher-education-under-siege-fragmented-security) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-34525"></a>

### 3. Government, Finance Orgs Targeted in Weeks-Long NetScaler Zero-Day Attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 52.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Citrix NetScaler ADCとNetScaler Gatewayに影響する深刻な脆弱性CVE-2026-88771について、実際の悪用が確認されていると複数の情報源が伝えています。
対象には政府機関や金融関連組織が含まれているとされ、Citrixは修正更新を公開しています。
ネットワーク境界で使われる製品が対象のため、侵害が起きると組織内への影響が広がりやすい点が注目されています。
公開PoCの言及もあり、未対策環境ではリスクが高まる可能性があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Citrix NetScaler ADC / Gateway の該当バージョンと適用状況を確認し、提供済みの修正更新を優先して適用する。
- インターネット公開されているNetScalerの管理・公開面を点検し、想定外の露出や不要な公開設定がないか確認する。
- 関連ログを遡って不審な認証・管理操作や設定変更の兆候がないか確認し、必要に応じて追加監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-88771 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-88772 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-88771](https://nvd.nist.gov/vuln/detail/CVE-2026-88771) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Government, Finance Orgs Targeted in Weeks-Long NetScaler Zero-Day Attacks](https://www.securityweek.com/government-finance-orgs-targeted-in-weeks-long-netscaler-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [NetScaler zero-day exploitation escalates into mass attacks (CVE-2026-88771)](https://www.helpnetsecurity.com/2026/09/29/netscaler-zero-day-exploitation-escalates-into-mass-attacks-cve-2026-88771/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix patches actively exploited NetScaler zero-days after a weekend of unoffic](https://cyberscoop.com/citrix-zero-days-delayed-disclosure/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: NetScaler Zero Days CVE-2026-88771 and CVE-2026-88772 Exploited in](https://unit42.paloaltonetworks.com/netscaler-zero-days-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-88771 and CVE-2026-88772: Two Critical Citrix NetScaler Flaws Under Act](https://www.bitsight.com/blog/critical-vulnerability-alert-cve-2026-88771-cve-2026-88772-citrix-netscaler-flaws-under-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zero-Day Exploitation of Citrix NetScaler ADC and Gateway: CVE-2026-88771 and CV](https://www.rapid7.com/blog/post/etr-zero-day-exploitation-of-citrix-netscaler-adc-and-gateway-cve-2026-88771-and-cve-2026-88772) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix NetScaler RCE zero-days exploited globally for weeks (CVE-2026-88771, CVE](https://www.helpnetsecurity.com/2026/09/28/citrix-netscaler-rce-zero-days-exploited-for-weeks-cve-2026-88771-cve-2026-88772/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（2件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-35236"></a>

### 4. Bitget hacked via zero-day in third-party security products

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

暗号資産取引所Bitgetは、先週発生した約3億8750万ドル相当の被害について、第三者のセキュリティ製品に存在したゼロデイ脆弱性が侵入に悪用されたと公表しました。
現時点では、影響を受けた製品名や侵入経路の詳細は限定的で、公開情報ベースでは事案の全容はまだ確定していません。
第三者製品のゼロデイが実際の大規模被害につながった点は、サプライチェーン経由のリスクを改めて示しています。
取引所や金融関連組織だけでなく、同種のセキュリティ製品を使う運用側にも点検の必要性を意識させる事案です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 利用中の第三者セキュリティ製品について、ベンダー通知と緊急パッチ情報を継続確認する。
- 重要システムでは、単一製品への依存を避け、異常検知や権限分離を含む多層防御を見直す。
- 被害が疑われる場合に備え、ログ保全、資産影響範囲の確認、インシデント対応手順の再点検を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | Exchange | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Bitget hacked via zero-day in third-party security products](https://www.bleepingcomputer.com/news/security/bitget-hacked-via-zero-day-in-third-party-security-products/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35209"></a>

### 5. Vulnerability Discovery and Exploitation Trends in the AI Era

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>M⁠C⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Google Threat Intelligence Groupは、AIの活用が脆弱性の発見と悪用の両方を加速させている可能性を示す分析を公表しました。
2026年は脆弱性公開数が増え、実際に悪用された脆弱性も増加している一方、AIで見つかる脆弱性は比較的高リスクで、特にRCEにつながるものの比率が高いとしています。
あわせて、AI/LLM基盤そのものを狙う脆弱性も増えており、オーケストレーションや推論基盤、AIゲートウェイ周辺が重点領域として挙げられています。
脆弱性の数が増えるだけでなく、優先して対処すべき高リスク案件が増えている点が重要です。
AIを使った開発・運用が広がるほど、従来の一律パッチ適用よりも、悪用可能性に基づく優先順位付けが必要になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- XSS系。
- 情報漏えい系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 公開件数の増加だけで判断せず、悪用観測や資産への到達性を含めてトリアージする。
- エッジ機器、認証前の管理系API、企業向けAIゲートウェイなど、初期侵入に使われやすい面を優先して点検する。
- AI/LLM基盤を使う環境では、オーケストレーション、推論サーバー、ファイルアップロードやワークフロー実行まわりの設定と更新を重点確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Mandiant | 言及あり | 0.80 | — |
| ベンダー | BeyondTrust | 言及あり | 0.80 | — |
| ベンダー | Anthropic | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| ベンダー | Oracle | 言及あり | 0.80 | — |
| 製品 | BeyondTrust Remote Support | 言及あり | 0.80 | — |
| 製品 | Linux kernel | 言及あり | 0.80 | — |
| 製品 | Langflow | 言及あり | 0.80 | — |
| 製品 | Oracle WebLogic Server | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Vulnerability Discovery and Exploitation Trends in the AI Era](https://cloud.google.com/blog/topics/threat-intelligence/vulnerability-discovery-and-exploitation-trends-in-the-ai-era/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-35202"></a>

### 6. Attackers Abuse ChatGPT Custom GPTs to Deliver RAT via ClickFix Lures

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

攻撃者がChatGPTのCustom GPT機能を悪用し、正規の製品やサービスに見せかけてユーザーを誘導している事例が報告されています。
誘導先ではClickFixと呼ばれる手口が使われ、結果としてRATの配布につながる可能性があるとされています。
信頼されやすいAIプラットフォーム上の機能が悪用されると、利用者が警戒しにくくなるため注意が必要です。
AIサービスを装った誘導は、従来のフィッシング対策だけでは見逃しやすい面があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ChatGPTや関連AI機能を名乗る案内でも、外部サイトへの誘導先を必ず確認する。
- ユーザー教育では、正規UIやチャット内メッセージでもファイル実行や設定変更を急がせる誘導に注意喚起する。
- メールやWebだけでなく、AIチャット経由の不審リンク・不審誘導も検知対象に含める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| AIモデル/プロジェクト | ChatGPT | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Attackers Abuse ChatGPT Custom GPTs to Deliver RAT via ClickFix Lures](https://thehackernews.com/2026/09/attackers-abuse-chatgpt-custom-gpts-to.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35230"></a>

### 7. Attackers Combine ChatGPT Feature Abuse With ClickFix to Deliver Trojan Malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、攻撃者がChatGPT関連の機能悪用とClickFixを組み合わせ、トロイの木馬型マルウェアを配布するキャンペーンが確認されています。
GoogleでChatGPTを検索する利用者を狙う形とされており、AIサービス周辺の検索行動が悪用される点が特徴です。
AIサービスの利用を装った誘導は、正規サービスを探す一般ユーザーに紛れ込みやすく、注意喚起が難しくなります。
業務端末へのマルウェア侵入につながる可能性があるため、検索経由の偽サイト対策や利用者教育の重要性が高まります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 検索結果や広告経由での誘導先を確認し、ChatGPT関連の正規導線を周知する。
- ブラウザ実行やダウンロードを伴う不審な案内に対するユーザー教育を強化する。
- 端末側でEDRやWebフィルタリングを活用し、未知の実行ファイルや不審なアクセスを監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Google | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | ChatGPT | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Attackers Combine ChatGPT Feature Abuse With ClickFix to Deliver Trojan Malware](https://www.infosecurity-magazine.com/news/chatgpt-feature-abuse-to-deliver/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35219"></a>

### 8. Suspected state-sponsored hackers exploited NetScaler zero-day since early September (CVE-2026-88772)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>通⁠信⁠基⁠盤</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

MandiantのCharles Carmakal氏によると、CVE-2026-88772を悪用したNetScalerへの侵入は、9月初旬から始まっていた可能性があるとされています。
関与したのは高度な脅威アクターで、国家支援型と疑われるグループの可能性があるものの、現時点では断定はされていません。
影響は北米と欧州の複数組織に及び、政府、金融、教育、通信、法律・専門サービスなどの分野が含まれるとされています。
NetScalerは広く使われる機器・製品群のため、ゼロデイ悪用の把握は被害拡大の抑止に直結します。
影響組織の範囲が複数地域・複数業種に広がっている点からも、継続的な確認と迅速な対応が重要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- NetScaler環境でCVE-2026-88772に関連するベンダー情報や更新情報を確認し、適用可能な対策を優先する。
- 外部からの不審な認証・アクセスや、通常と異なる管理系通信の有無を点検する。
- 政府・金融・教育・通信など、影響が報告された業種の組織は、自組織の該当性を前提にログ確認とインシデント調査を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-88772 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Mandiant | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Suspected state-sponsored hackers exploited NetScaler zero-day since early Septe](https://www.helpnetsecurity.com/2026/09/30/cve-2026-88772-netscaler-exploitation-zero-day/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-34785"></a>

### 1. Apple Patches CoreGraphics Zero Day Exploited in Attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>i⁠O⁠S</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Appleは、CoreGraphicsに関するゼロデイ脆弱性CVE-2026-86950を修正する更新を公開しました。
複数の報道によると、この問題は特定の標的に対する攻撃で悪用されていたとされ、iOSとmacOSの一部旧ブランチが影響を受けます。
ゼロデイかつ実際の悪用が報告されているため、放置すると被害につながる可能性があります。対象となる端末が多いApple製品の更新である点も、注目度が高い理由です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 7 sources。
- 実悪用・ゼロデイ文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象OSの更新適用状況を早急に確認し、未適用端末を優先してアップデートする。
- iOS/macOSの旧ブランチ利用端末がないか棚卸しし、サポート状況と更新経路を整理する。
- 不審なファイル受領や、標的型攻撃を想定した監視・注意喚起を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-86950 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Apple | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Apple iOS | 言及あり | 0.80 | — |
| ベンダー | Meta | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-86950](https://nvd.nist.gov/vuln/detail/CVE-2026-86950) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Apple Patches CoreGraphics Zero Day Exploited in Attacks](https://www.infosecurity-magazine.com/news/apple-patches-coregraphics-zero/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Zero-Day Vulnerability Weaponized in Targeted Attacks](https://www.darkreading.com/cyberattacks-data-breaches/apple-zero-day-vulnerability-weaponized-targeted-attacks) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple patches CoreGraphics zero-day already exploited in targeted attacks](https://www.theregister.com/security/2026/09/29/apple-patches-coregraphics-zero-day-already-exploited-in-targeted-attacks/5299721) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Update your iPhone, iPad, or Mac: Flaw could run attackers’ code](https://www.malwarebytes.com/blog/bugs/2026/09/update-your-iphone-ipad-or-mac-flaw-could-run-attackers-code) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple squashes zero-day bug exploited in “extremely sophisticated” attack (CVE-2](https://www.helpnetsecurity.com/2026/09/29/apple-core-graphics-zero-day-cve-2026-86950-fixed/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Patches Zero-Day Linked to ‘Extremely Sophisticated Attack’](https://www.securityweek.com/apple-patches-meta-reported-zero-day-linked-to-extremely-sophisticated-attack/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Emergency Patch for iOS 26, macOS26, macOS15 (CVE-2026-86950), (Mon, Sep 2](https://isc.sans.edu/diary/rss/33376) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [生産性向上拡張機能が攻撃プラットフォームに変わるとき](https://www.akamai.com/blog/security-research/2026/sep/when-productivity-extensions-become-attack-platforms) | 28.0 | 20.0 | 42.0 |
| [攻撃者がZimbraの脆弱性を悪用し、Webシェルを設置して認証情報を窃取](https://thehackernews.com/2026/09/attackers-exploit-zimbra-flaw-to-deploy.html) | 28.0 | 20.0 | 42.0 |
| [攻撃者がMSP360を悪用してデュアルRMMフィッシング攻撃でScreenConnectを展開](https://thehackernews.com/2026/09/attackers-abuse-msp360-to-deploy.html) | 28.0 | 20.0 | 42.0 |
| [Star BlizzardがClickFixをやめ、フィッシング網を拡大](https://www.darkreading.com/threat-intelligence/russia-star-blizzard-apt-ditches-clickfix-widen-phishing-net) | 28.0 | 20.0 | 42.0 |
| [ウクライナの研究者によるモバイルマルウェア警告、iPhone exploit kitも含む](https://therecord.media/ukraine-ssscip-mobile-malware-warning-ios-android) | 28.0 | 20.0 | 42.0 |
| [Russian FSB関連ハッカー、ウクライナ支援者へのフィッシング攻撃を拡大](https://therecord.media/russia-hackers-ukraine-blizzard) | 28.0 | 20.0 | 42.0 |
| [Russian APT Star Blizzard、最近の攻撃で「RedFlick」感染チェーンを使用](https://www.securityweek.com/russian-apt-star-blizzard-uses-redflick-infection-chain-in-recent-attacks/) | 28.0 | 20.0 | 42.0 |
| [米国を標的にした役員向けフィッシングでMicrosoft 365セッションを窃取し、RMMツールを配布して遠隔アクセスを確立](https://thehackernews.com/2026/09/us-focused-csuite-phishing-steals.html) | 28.0 | 20.0 | 42.0 |
| [英国企業の半数以上が基本的なサイバー技能に自信を持てず](https://www.theregister.com/security/2026/09/30/more-than-half-of-uk-businesses-lack-confidence-in-basic-cyber-skills/5299991) | 28.0 | 20.0 | 42.0 |
| [Attackers exploit NetScalerの脆弱性でroot権限を取得し、WHIPSHOTとSLAPSHOTを展開](https://thehackernews.com/2026/09/attackers-exploit-netscaler-flaw-for.html) | 28.0 | 20.0 | 42.0 |
| [AIの普及で悪用が加速、脆弱性開示は月1万件に倍増](https://therecord.media/google-vulnerabilities-cyberattacks-ai) | 25.0 | 20.0 | 42.0 |
| [AIで変わるSOCキャリアの階段、91%が満足する一方で約半数が入口の厳しさを実感](https://www.darkreading.com/cybersecurity-careers/ai-reshapes-soc-career-ladder) | 25.0 | 20.0 | 42.0 |
| [Cisco、2026年10月7日公開予定のセキュリティアドバイザリ事前通知](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-notice-fBn58ELx) | 25.0 | 20.0 | 42.0 |
| [Google、AIは脆弱性発見の速度と特徴を変えている](https://www.securityweek.com/google-ai-is-changing-the-pace-and-profile-of-vulnerability-discovery/) | 25.0 | 20.0 | 42.0 |
| [AIの第3波：コワーカーがエージェントで機能していたセキュリティモデルを崩す](https://www.bleepingcomputer.com/news/security/ais-third-wave-coworkers-break-the-security-model-that-worked-for-agents/) | 25.0 | 20.0 | 42.0 |
| [Trumpと6つのAI大手企業が「Super Intelligence」安全協定に署名](https://www.infosecurity-magazine.com/news/trump-ai-giants-super-intelligence/) | 25.0 | 20.0 | 42.0 |
| [AIがSOCアナリストの対応能力を高める一方でスキル向上を妨げる可能性](https://www.infosecurity-magazine.com/news/ai-boosts-soc-analyst-capacity/) | 25.0 | 20.0 | 42.0 |
| [AIコーディングエージェントが社内スクリーンショット13,000件を公開GitHubリポジトリに漏えい](https://www.helpnetsecurity.com/2026/09/30/ai-coding-agents-github-screenshot-leak/) | 25.0 | 20.0 | 42.0 |
| [AIコーディングエージェントが13,000件の内部画像をGitHub上で公開、請求記録も含む](https://thehackernews.com/2026/09/ai-coding-agents-exposed-13000-internal.html) | 25.0 | 20.0 | 42.0 |
| [Anthropic、AIエージェントの責任リスクを指摘　OpenAIはハッキング訴訟に直面](https://www.securityweek.com/anthropic-flags-ai-agent-liability-risks-as-openai-faces-hacking-lawsuit/) | 25.0 | 20.0 | 42.0 |
| [CISAが警告するMikroTik RouterOSの認証前RCE脆弱性](https://www.bleepingcomputer.com/news/security/cisa-warns-of-critical-pre-auth-rce-flaw-in-mikrotik-routeros/) | 24.0 | 38.0 | 42.0 |
| [中国関連のUAT-11587がAntinoバックドアでアジア各地の政府・政策機関を標的にする](https://blog.talosintelligence.com/china-nexus-uat-11587-targets-government-and-policy-organizations-across-asia-with-antino-backdoor/) | 22.0 | 20.0 | 48.0 |
| [インターネット公開メールサーバーにおける未認証のコマンドインジェクション：CVE-2026-73570の追跡](https://www.microsoft.com/en-us/security/blog/2026/09/30/unauthenticated-command-injection-on-internet-facing-mail-servers-tracking-cve-2026-73570/) | 22.0 | 20.0 | 42.0 |
| [2支店で顧客情報記載の書類が所在不明 - 青森みちのく銀](https://www.security-next.com/190648) | 22.0 | 20.0 | 42.0 |
| [「代金後払いサービス」で侵害、サービスを停止 - ヤマト運輸](https://www.security-next.com/190835) | 22.0 | 20.0 | 42.0 |
| [チケット販売「イープラス」、払戻し申請した顧客顧客の個人情報が流出](https://www.security-next.com/190837) | 22.0 | 20.0 | 42.0 |
| [セイコーマート、会員のほぼ半数に当たる情報漏えい 約57万人分](https://www.itmedia.co.jp/news/article/2609/30/2000001906/) | 21.0 | 20.0 | 42.0 |
| [「タイムズカー」不正アクセス、免許証画像など約160万件が漏洩](https://xtech.nikkei.com/atcl/nxt/news/24/03401/) | 21.0 | 20.0 | 42.0 |
| [集英社のブロガー管理システムに不正アクセス 2835人分の個人情報漏えい、結婚状況や子の有無も](https://www.itmedia.co.jp/news/article/2609/30/2000001898/) | 21.0 | 20.0 | 42.0 |
| [OpenInfra EuropeのJFrog Artifactoryインスタンスが侵害され、パッケージが改ざんされた可能性](https://www.helpnetsecurity.com/2026/09/30/openinfra-jfrog-artifactory-instance-compromised/) | 20.0 | 45.0 | 42.0 |
| [フィッシング対応プロトコル：ANY.RUNの最新アップデートで強化されたSOCの3つの重要ステップ](https://any.run/cybersecurity-blog/phishing-response-protocol/) | 20.0 | 20.0 | 48.0 |
| [16歳の研究者がMicrosoftのバグを発見し、17.3兆行のデータベースに管理者アクセスを取得](https://www.theregister.com/security/2026/09/30/16-year-old-researcher-found-a-microsoft-bug-got-admin-access-to-databases-with-173-trillion-rows/5300240) | 20.0 | 20.0 | 42.0 |
| [公開GitHubリポジトリで54万3,000件超の有効な認証情報が流出](https://www.bleepingcomputer.com/news/security/over-543-000-valid-credentials-exposed-in-public-github-repositories/) | 20.0 | 20.0 | 42.0 |
| [Kubernetesサプライチェーンの保護：WizOS Helm Chartの紹介](https://www.wiz.io/blog/wizos-helm-charts) | 20.0 | 20.0 | 42.0 |
| [Arizona州の裁判所から保護命令と里親保護記録が窃取される](https://www.malwarebytes.com/blog/data-breaches/2026/09/hackers-steal-protective-order-and-foster-care-records-from-arizona-courts) | 20.0 | 20.0 | 42.0 |
| [Citrix NetScalerの大規模な悪用：現時点でわかっていること](https://www.cybersecuritydive.com/news/exploitation-citrix-netscaler-what-we-know/831780/) | 20.0 | 20.0 | 42.0 |
| [National cyber directorが民間部門のハッキングプログラムを擁護、セキュリティの基本対策を重視するよう促す](https://www.cybersecuritydive.com/news/oncd-white-house-sean-cairncross-regulation-deterrence-ai/831768/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、10月からEntra IDのスクリプトインジェクション攻撃をブロックへ](https://www.bleepingcomputer.com/news/security/microsoft-to-block-entra-id-script-injection-attacks-starting-october/) | 20.0 | 20.0 | 42.0 |
| [WatchGuard Fireware OSの重大なコードインジェクション脆弱性を修正](https://www.securityweek.com/watchguard-patches-critical-fireware-os-code-injection-vulnerability/) | 20.0 | 20.0 | 42.0 |
| [TeamViewer、深刻な脆弱性をできるだけ早急に修正するようユーザーに呼びかけ](https://www.bleepingcomputer.com/news/security/teamviewer-urges-users-to-patch-severe-flaws-as-soon-as-possible/) | 20.0 | 20.0 | 42.0 |
| [Chrome、Firefoxのアップデートで100件超の脆弱性を修正](https://www.securityweek.com/chrome-firefox-updates-patch-over-100-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [2026年におけるブラウザベースの攻撃手法を知る](https://thehackernews.com/2026/09/know-your-enemy-browser-based-attack.html) | 20.0 | 20.0 | 42.0 |
| [セコマ個人情報漏えい 第三者閲覧](https://news.yahoo.co.jp/pickup/6597106?source=rss) | 20.0 | 20.0 | 42.0 |
| [あなたの車のアプリがBig Techにあなたの身元や行き先を知らせているかもしれない](https://www.malwarebytes.com/blog/news/2026/09/your-cars-app-could-be-telling-big-tech-who-you-are-and-where-you-go) | 20.0 | 20.0 | 42.0 |
| [米国国防総省人事データベース侵害で数百万人の個人情報が流出](https://www.bitdefender.com/en-us/blog/hotforsecurity/pentagon-personnel-database-breach-personal-data-millions) | 20.0 | 20.0 | 42.0 |
| [FBIがメンバーに出頭を呼びかけた後も強気の姿勢を崩さないShinyHunters](https://www.securityweek.com/shinyhunters-defiant-after-fbi-calls-on-members-to-come-forward/) | 20.0 | 20.0 | 42.0 |
| [年末に向けてテックチームの拡充を図る英国企業](https://www.itpro.com/business/careers-and-training/uk-employers-look-to-expand-tech-teams-before-year-end) | 20.0 | 20.0 | 42.0 |
| [WaterISAC、夏のサイバー攻撃ラッシュを受けて多様な脅威に対応](https://cyberscoop.com/water-utility-cyberattacks-waterisac-cyware-threat-intelligence/) | 20.0 | 20.0 | 42.0 |
| [Signal、iOSとデスクトップ向けに暗号化されたローカルバックアップとクロスプラットフォーム復元を追加](https://www.helpnetsecurity.com/2026/09/30/signal-encrypted-backups-ios-8-30/) | 20.0 | 20.0 | 42.0 |
| [英国鉄道警察の32万ポンド顔認証走査で一致ゼロ](https://www.theregister.com/security/2026/09/30/uk-rail-cops-320k-face-scanning-spree-nets-zero-matches/5299793) | 20.0 | 20.0 | 42.0 |
| [OpenSSLが高深刻度のDTLS脆弱性を修正、暗号化されないヒープメモリ漏えいの恐れ](https://thehackernews.com/2026/09/openssl-fixes-high-severity-dtls-flaw.html) | 20.0 | 20.0 | 42.0 |

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
