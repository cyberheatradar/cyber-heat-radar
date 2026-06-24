# 📡 サイレーダー 2026-06-25 05:00 JST

このレポートは、2026-06-24 17:00 JST〜2026-06-25 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 93
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 62

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Zero-Day Exploitation of Vulnerability (CVE-2026-20245) in Cisco Catalyst SD-WAN Manager](#topic-15753) | 43.0 | 58.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [Cisco Unified CM flaw actively exploited to drop webshells (CVE-2026-20230)](#topic-14652) | 39.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 3 | [CISA Warns Critical Lantronix EDS5000 Flaw Is Being Actively Exploited](#topic-19075) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 4 | [StealC You Later: Proofpoint and IBM X-Force Support Operation Endgame Disruptions](#topic-19073) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Law enforcement hits StealC and Amadey malware networks](#topic-19083) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [Microsoft uses AI to link two malware operations in racketeering suit](#topic-19071) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [Malicious hackers exploit Cisco zero-day for highest access level at communications service provider](#topic-17617) | 32.0 | 64.0 | 59.0 | GitHub | 音声枠上限によりGitHubのみ |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-15753"></a>

### 1. Zero-Day Exploitation of Vulnerability (CVE-2026-20245) in Cisco Catalyst SD-WAN Manager

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Catalyst SD-WAN Managerに関するCVE-2026-20245は、認証済みの攻撃者が権限を昇格できる脆弱性として報告され、Ciscoは一部で悪用が観測されているとしています。
現時点では修正パッチが提供されていないとされ、関連製品の管理環境に注意が必要です。SD-WANはネットワーク運用の中核に近く、侵害されると広範な影響につながる可能性があります。
加えて、既存の認証情報や別脆弱性の悪用を足がかりに権限昇格へ進む可能性が示されているため、管理面の警戒が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Ciscoの最新アドバイザリと影響範囲を確認し、対象バージョンかどうかを早急に点検する。
- 管理者権限を持つアカウントの認証情報保護と、多要素認証の適用状況を見直す。
- 関連する脆弱性や不審な管理操作の有無を監視し、必要に応じてアクセス制御や一時的な運用制限を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20127 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20182 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20245 | 関連CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20245](https://nvd.nist.gov/vuln/detail/CVE-2026-20245) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Zero-Day Exploitation of Vulnerability (CVE-2026-20245) in Cisco Catalyst SD-WAN](https://cloud.google.com/blog/topics/threat-intelligence/zero-day-exploitation-cisco-catalyst-sd-wan-manager/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN V](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-privesc-4uxFrdzx) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco customers encounter another SD-WAN zero-day under attack](https://cyberscoop.com/cisco-sdwan-zero-day-vulnerability-exploited-cve202620245/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Manager CVE-2026-20245 Flaw Actively Exploited – No Patch ](https://thehackernews.com/2026/06/cisco-catalyst-sd-wan-manager-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco SD-WAN 0-day exploited, no patch available (CVE-2026-20245)](https://www.helpnetsecurity.com/2026/06/05/cisco-sd-wan-cve-2026-20245-0-day-exploited/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補あり（URL 6件以上 / 該当CVE 2件）。

---

<a id="topic-14652"></a>

### 2. Cisco Unified CM flaw actively exploited to drop webshells (CVE-2026-20230)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Cisco Unified CM / Unified CM SME に存在する CVE-2026-20230 について、実際の攻撃で webshell の設置につながる悪用が観測されていると報じられています。
Cisco の案内では、未認証のリモート攻撃者が特定の HTTP リクエストを通じて SSRF を引き起こし、条件次第で OS 上へのファイル書き込みにつながる可能性があるとされています。
音声・通話基盤として使われる製品の脆弱性が、すでに攻撃対象になっている点が重要です。
認証不要で外部から影響を受けうるため、公開面にある環境では優先的な確認と更新が必要になります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
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

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Cisco の修正済みソフトウェア適用状況を確認し、該当バージョンの有無を早急に棚卸しする。
- WebDialer の有効/無効を含め、該当機能の構成と露出範囲を点検する。
- 関連ログや不審なファイル生成、Web サービス周辺の異常を確認し、侵害の兆候がないか監視を強める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20230 | 関連CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20230](https://nvd.nist.gov/vuln/detail/CVE-2026-20230) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified CM flaw actively exploited to drop webshells (CVE-2026-20230)](https://www.helpnetsecurity.com/2026/06/24/cisco-unified-cm-flaw-exploited-to-drop-webshells-cve-2026-20230/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers Exploiting Cisco Unified CM Vulnerability](https://www.securityweek.com/hackers-exploiting-cisco-unified-cm-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified CM flaw CVE-2026-20230 now exploited in attacks](https://www.bleepingcomputer.com/news/security/cisco-unified-cm-sme-flaw-cve-2026-20230-now-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified Communications Manager Server-Side Request Forgery Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-cucm-ssrf-cXPnHcW) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補あり（URL 2件以上 / 該当CVE 1件）。

---

<a id="topic-19075"></a>

### 3. CISA Warns Critical Lantronix EDS5000 Flaw Is Being Actively Exploited

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

CISAは、Lantronix EDS5000 Series機器に影響するCVE-2025-67038について、実際の悪用が観測されているとして注意喚起しました。
この脆弱性はCVSS 9.8の重大な問題とされ、コードインジェクションにより任意のコード実行につながる可能性があるとされています。
産業用・ネットワーク機器の脆弱性は、対象機器が公開環境や重要インフラ周辺で使われている場合、影響が広がりやすい点が注目されます。
すでに悪用が観測されているため、未対策機器の早期確認と更新の優先度が高い事案です。

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

- Lantronix EDS5000 Seriesの利用有無を棚卸しし、該当モデルとファームウェア版を確認する。
- ベンダー提供の修正パッチや緩和策を適用し、更新可否が不明な機器は隔離やアクセス制限を検討する。
- 外部から到達可能な管理インターフェースや不審な設定変更・挙動がないかを点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-67038 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-67038](https://nvd.nist.gov/vuln/detail/CVE-2025-67038) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA Warns Critical Lantronix EDS5000 Flaw Is Being Actively Exploited](https://thehackernews.com/2026/06/cisa-warns-critical-lantronix-eds5000.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-19073"></a>

### 4. StealC You Later: Proofpoint and IBM X-Force Support Operation Endgame Disruptions

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

ProofpointとIBM X-Forceは、Europol主導の「Operation Endgame」の一環として、情報窃取マルウェア「StealC」のエコシステムに対する停止・無力化 நடவட作を支援したと公表しました。
今回の対応では、StealC関連のドメインやサーバーが対象となり、収集された認証情報や感染基盤に関する情報も示されています。
StealCは認証情報や各種機密データを狙うマルウェアとして広く使われており、その基盤への打撃は被害の拡大抑制につながります。
加えて、法執行機関と民間企業が連携してインフラや運用実態を把握し、継続的な対策に結びつけた点も重要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 認証情報の漏えい前提で、アカウント保護強化と多要素認証の徹底を再確認する。
- ブラウザ保存情報、メール/メッセージング、VPN、暗号資産ウォレット周辺の端末監視を見直す。
- StealCに限らず、情報窃取系マルウェアの検知・封じ込めを前提にEDRやログ監視の確認を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ransomware_group | LockBit | 主題 | 0.80 |
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [StealC You Later: Proofpoint and IBM X-Force Support Operation Endgame Disruptio](https://www.proofpoint.com/us/blog/threat-insight/stealc-you-later-proofpoint-and-ibm-x-force-support-operation-endgame) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-19083"></a>

### 5. Law enforcement hits StealC and Amadey malware networks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

国際的な法執行機関と民間企業の連携により、StealCとAmadeyに関係するマルウェア基盤への対処が行われたと報じられています。
両者は別系統の脅威グループに由来するとされますが、端末侵害や情報窃取に関連して連携して使われる文脈があるとされています。
攻撃インフラへの対処は、被害の拡大を抑えるうえで重要です。
特に情報窃取系マルウェアは、その後の不正アクセスやランサムウェア被害の起点になり得るため、影響範囲の把握が注目されます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- StealCやAmadeyに関連する検知・ブロック設定やEDRのアラート傾向を確認する。
- 侵害後の横展開や情報窃取につながる挙動がないか、認証情報・ブラウザデータ・不審な持続化を重点監視する。
- 関連するインフラ対処後も、既存感染端末や代替経路が残る可能性を前提に、端末の隔離・調査・資格情報の見直しを進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Law enforcement hits StealC and Amadey malware networks](https://www.helpnetsecurity.com/2026/06/24/operation-endgame-stealc-amadey-malware-disrupted/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-19071"></a>

### 6. Microsoft uses AI to link two malware operations in racketeering suit

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

MicrosoftがAIを用いて、StealCとAmadeyに関連するとみられる2つのマルウェア運用を結び付けたと報じられています。
あわせて、200台超のC2サーバーが停止したとされ、脅威インフラの把握と遮断にAIが活用された事例として注目されています。
攻撃インフラの関連付けや整理にAIを使う動きは、脅威インテリジェンスや対策の効率化に直結します。
個別のマルウェアだけでなく、背後の運用ネットワーク全体を見渡す重要性を示しています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIによる関連付け結果は、他の情報源や自組織の観測と突き合わせて確認する。
- C2や配布基盤の変化は、検知ルールやブロック対象の更新につなげる。
- 特定マルウェア名だけでなく、関連インフラや再利用パターンも監視対象に含める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft uses AI to link two malware operations in racketeering suit](https://www.theregister.com/security/2026/06/24/microsoft-uses-ai-to-link-two-malware-operations-in-racketeering-suit/5261656) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-17617"></a>

### 1. Malicious hackers exploit Cisco zero-day for highest access level at communications service provider

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 32.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

Cisco Catalyst SD-WAN Controllerなどに存在する認証回避の脆弱性（CVE-2026-20127）について、Ciscoは影響を受ける製品向けの修正版ソフトウェアを公開しています。
公開情報では、未認証のリモート攻撃者が管理者権限に近い高権限を取得しうるとされ、実際の悪用も観測されたと報じられています。
SD-WAN基盤は通信事業者や大規模ネットワークの中核になりやすく、影響が出ると設定変更や運用管理に直結するため注目されています。
既知の悪用が示されている点から、単なる理論上の脆弱性ではなく、優先度の高い対応対象とみられます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
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
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 影響を受けるCisco Catalyst SD-WAN製品のバージョンを確認し、提供済みの修正版への更新を優先する。
- 認証回避の兆候や不審な管理系アクセスがないか、関連ログを点検する。
- NETCONFなど設定変更に関わる経路の利用状況を見直し、不要な露出や権限の最小化を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2022-20775 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20127 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20182 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20245 | 関連CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20127](https://nvd.nist.gov/vuln/detail/CVE-2026-20127) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Malicious hackers exploit Cisco zero-day for highest access level at communicati](https://cyberscoop.com/cisco-sd-wan-zero-day-exploit-communications-provider/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco adds another SD-WAN box to max-severity bug advisory](https://www.theregister.com/security/2026/06/17/cisco-adds-another-sd-wan-box-to-max-severity-bug-advisory/5257621) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-rpa-EHchtZk) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補あり（URL 6件以上 / 該当CVE 2件）。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [AmadeyとStealCマルウェアのネットワークが破壊され、2700万件の窃取された認証情報を回収](https://thehackernews.com/2026/06/amadey-and-stealc-malware-network.html) | 36.0 | 30.0 | 42.0 |
| [MicrosoftとEuropolが主導したインフォスティーラー・マルウェアの国際摘発](https://www.cybersecuritydive.com/news/microsoft-europol-international-takedown-infostealer-malware/823655/) | 36.0 | 30.0 | 42.0 |
| [Operation EndgameでAmadeyとStealCのマルウェア活動を妨害](https://www.bleepingcomputer.com/news/security/amadey-stealc-malware-operations-disrupted-in-operation-endgame-action/) | 36.0 | 30.0 | 42.0 |
| [Iran関連のMuddyWaterがランサムウェア集団を装いサイバー諜報活動を隠蔽](https://www.infosecurity-magazine.com/news/iranlinked-muddywater-poses-as/) | 36.0 | 30.0 | 42.0 |
| [CAPTCHAだらけのウェブを変える人間証明システム「PACT」とは？](https://gigazine.net/news/20260624-mozilla-pact/) | 30.0 | 20.0 | 42.0 |
| [2025年にランサムウェア攻撃が増加し、従来型のデータ侵害は減少したとBitsightが報告](https://www.cybersecuritydive.com/news/ransomware-data-breaches-ai-bitsight/823649/) | 28.0 | 30.0 | 42.0 |
| [インドの自動車大手Bajaj Autoがランサムウェア被害](https://therecord.media/indian-auto-giant-bajaj-auto-hit-by-ransomware) | 28.0 | 30.0 | 42.0 |
| [新たな「Mistic」RATが複数のランサムウェアファミリーへの侵入口を開く](https://www.securityweek.com/new-mistic-rat-opens-door-to-several-ransomware-families/) | 28.0 | 30.0 | 42.0 |
| [ransomwareアクセスブローカーKongTukeに関連するステルス型Misticバックドア](https://www.bleepingcomputer.com/news/security/stealthy-mistic-backdoor-linked-to-ransomware-access-broker-kongtuke/) | 28.0 | 30.0 | 42.0 |
| [Backdoor.Mistic：ランサムウェアのアクセスブローカーに関連する可能性のある新たなバックドア](https://www.security.com/threat-intelligence/new-mistic-backdoor-modelorat) | 28.0 | 30.0 | 42.0 |
| [Microsoftと同盟各社がAmadeyとStealCマルウェアの共有インフラを摘発・遮断](https://www.securityweek.com/microsoft-and-allies-smash-shared-infrastructure-of-amadey-and-stealc-malware/) | 28.0 | 20.0 | 42.0 |
| [Malwarebytesを装った更新詐欺に注意](https://www.malwarebytes.com/blog/scams/2026/06/watch-out-for-renewal-scams-pretending-to-be-malwarebytes) | 28.0 | 20.0 | 42.0 |
| [「すべてのデバイスに完全アクセスできます」と脅すセクストーション詐欺が再び発生](https://www.malwarebytes.com/blog/scams/2026/06/total-access-to-all-your-devices-sextortion-scammers-strike-again) | 28.0 | 20.0 | 42.0 |
| [StrikeShark：SharkLoader経由でCobalt Strikeを配布する新たなキャンペーンの調査](https://securelist.com/strikeshark-campaign/120326/) | 28.0 | 20.0 | 42.0 |
| [情報が攻撃対象になるとき ― AIエージェントの罠を理解する](https://www.securityweek.com/when-information-becomes-the-attack-surface-understanding-ai-agent-traps/) | 25.0 | 20.0 | 42.0 |
| [More Malicious OpenClaw SkillsがAIサプライチェーンを脅かす](https://www.darkreading.com/cyber-risk/malicious-openclaw-skills-clawhub-threaten-ai-supply-chain) | 25.0 | 20.0 | 42.0 |
| [Researchers、AIブラウザをだまして認証情報を漏えいさせる](https://www.infosecurity-magazine.com/news/bioshocking-ai-browser-prompt/) | 25.0 | 20.0 | 42.0 |
| [Cisco、2026年7月1日公開予定のセキュリティアドバイザリ事前通知](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-notice-vwL7b0S7) | 25.0 | 20.0 | 42.0 |
| [エージェント型AIアーキテクチャが直面するレイテンシ危機](https://www.akamai.com/blog/ai/2026/jun/agentic-disconnect-latency-crisis-modern-ai-architecture) | 25.0 | 20.0 | 42.0 |
| [AIVEX：サプライチェーンの脅威とリスクを低減する新しいトリアージモデル](https://www.securityweek.com/exclusive-meet-aivex-a-new-triage-model-built-to-reduce-supply-chain-threat-and-risk/) | 25.0 | 20.0 | 42.0 |
| [macOSバックドアがAIトリアージ回避にプロンプトインジェクションを悪用](https://www.infosecurity-magazine.com/news/macos-gaslight-rust-backdoor/) | 25.0 | 20.0 | 42.0 |
| [AnthropicのClaude TagがAIエージェントに独立したアイデンティティを付与](https://www.helpnetsecurity.com/2026/06/24/anthropic-claude-tag-agent-identity-model/) | 25.0 | 20.0 | 42.0 |
| [AIがSecOpsの運用手順をどう書き換えているか](https://www.wiz.io/blog/ai-rewriting-secops-playbook) | 25.0 | 20.0 | 42.0 |
| [Agentic AIセキュリティ：誤った文脈が機械速度で誤判断を生む](https://www.securityweek.com/agentic-ai-security-wrong-context-wrong-decisions-at-machine-speed/) | 25.0 | 20.0 | 42.0 |
| [AIが攻撃をより低コスト・高速・秘匿化しているとReliaQuestが指摘](https://www.infosecurity-magazine.com/news/ai-attacks-cheaper-faster-covert/) | 25.0 | 20.0 | 42.0 |
| [攻撃者に狙われるUbiquitiの重大な脆弱性](https://www.securityweek.com/critical-ubiquiti-vulnerabilities-in-attackers-crosshairs/) | 24.0 | 38.0 | 42.0 |
| [CNAPPの進化：Microsoftが主要なクラウドリスク管理プラットフォームとどう連携するか](https://www.microsoft.com/en-us/security/blog/2026/06/24/cnapp-evolution-how-microsoft-aligns-with-leading-cloud-risk-management-platforms/) | 22.0 | 20.0 | 42.0 |
| [預かり証控が所在不明、文書整理で判明 - 旭川信金](https://www.security-next.com/186078) | 22.0 | 20.0 | 42.0 |
| [メルアカ侵害でスパムの踏み台に - 日本医業経営コンサルタント協会](https://www.security-next.com/186137) | 22.0 | 20.0 | 42.0 |
| [オンラインショップが侵害、影響など詳細を調査 - 村瀬鞄行](https://www.security-next.com/186131) | 22.0 | 20.0 | 42.0 |
| [StealCとAmadey：インフォスティーラーとそれを配布するサイバー犯罪サービスの分析](https://www.microsoft.com/en-us/security/blog/2026/06/24/stealc-and-amadey-breaking-down-infostealers-and-the-cybercrime-services-that-deliver-them/) | 22.0 | 20.0 | 42.0 |
| [府営住宅の募集案内書に個人情報混入、公共施設で配布 - 京都府](https://www.security-next.com/186070) | 22.0 | 20.0 | 42.0 |
| [非表示の個人情報を削除済みと誤認、外部に誤送信 - 川越商工会議所](https://www.security-next.com/186332) | 22.0 | 20.0 | 42.0 |
| [学校家庭調査で回答を誤公開 - 仕様確認を担当者に依存](https://www.security-next.com/186068) | 22.0 | 20.0 | 42.0 |
| [“PayPay送金詐欺”3カ月で22.4倍に急増 ゲーム・トレカサービスかたる新手口も](https://www.itmedia.co.jp/news/articles/2606/24/news135.html) | 21.0 | 20.0 | 42.0 |
| [「平文」は「へいぶん」「ひらぶん」どっち？](https://www.itmedia.co.jp/news/articles/2606/24/news132.html) | 21.0 | 20.0 | 42.0 |
| [「パスワードが変更できない」の声相次ぐ BIGLOBE、情報漏えいの可能性で変更呼びかけ マイページ高負荷が一因](https://www.itmedia.co.jp/news/articles/2606/24/news123.html) | 21.0 | 20.0 | 42.0 |
| [CordycepsのCI/CD脆弱性により300件超のGitHubリポジトリがサプライチェーン攻撃にさらされる](https://thehackernews.com/2026/06/cordyceps-cicd-flaws-expose-300-github.html) | 20.0 | 45.0 | 42.0 |
| [Klueのサプライチェーン攻撃によるLastPass顧客データ流出](https://www.helpnetsecurity.com/2026/06/24/lastpass-klue-data-breach-salesforce-environment/) | 20.0 | 45.0 | 42.0 |
| [PixelSmashの脆弱性で動画ファイルが攻撃ツールに変わる](https://www.malwarebytes.com/blog/news/2026/06/pixelsmash-flaw-turns-video-files-into-attack-tools) | 20.0 | 28.0 | 50.0 |
| [Europol主導のOperation Endgame、StealCとAmadeyの情報窃取マルウェアを摘発](https://www.infosecurity-magazine.com/news/operation-endgame-stealc-amadey/) | 20.0 | 20.0 | 42.0 |
| [CISAが警告するUbiquitiの重大脆弱性、攻撃で悪用確認](https://www.bleepingcomputer.com/news/security/cisa-warns-of-max-severity-ubiquiti-flaws-exploited-in-attacks/) | 20.0 | 20.0 | 42.0 |
| [アルジェリア国籍の男、サイバー犯罪マーケットプレイス運営の疑いで米国へ引き渡し](https://www.helpnetsecurity.com/2026/06/24/algerian-cybercrime-marketplace-operator-extradited-to-us/) | 20.0 | 20.0 | 42.0 |
| [サービスデスクを守る：ソーシャルエンジニアリング攻撃が成功し続ける理由](https://www.bleepingcomputer.com/news/security/securing-the-service-desk-why-social-engineering-attacks-keep-succeeding/) | 20.0 | 20.0 | 42.0 |
| [macOSの脆弱性を組み合わせてEndpoint Securityエージェントを静かに無効化する手口](https://www.securityweek.com/macos-weaknesses-chained-to-silently-disable-endpoint-security-agents/) | 20.0 | 20.0 | 42.0 |
| [ホワイトハウスの州インフラサイバーセキュリティ・イニシアチブが停滞](https://www.cybersecuritydive.com/news/white-house-states-cybersecurity-pilot-programs-oncd/823453/) | 20.0 | 20.0 | 42.0 |
| [DraftKingsへの不正アクセスを行った3人目のハッカーに18か月の禁錮刑](https://www.securityweek.com/third-draftkings-hacker-sentenced-to-18-months-in-prison/) | 20.0 | 20.0 | 42.0 |
| [KDDIの侵害で日本の6つのISPが影響を受け、14.2万件のメール認証情報が流出](https://www.infosecurity-magazine.com/news/kddi-breach-japanese-telcos/) | 20.0 | 20.0 | 42.0 |
| [初の事例、裁判所の差し止めで2つのサイバー犯罪ツールを同時に標的にする](https://cyberscoop.com/microsoft-amadey-stealc-takedown/) | 20.0 | 20.0 | 42.0 |
| [医療企業Xsolisへのフィッシング攻撃で140万人に影響](https://www.helpnetsecurity.com/2026/06/24/xsolis-data-breach-phishing-attack/) | 20.0 | 20.0 | 42.0 |
| [CISAの新ガイド、連邦機関の最新ゼロトラストアーキテクチャ移行を支援](https://www.cisa.gov/news-events/news/new-cisa-guide-assists-federal-agencies-transitioning-modernized-zero-trust-architectures) | 20.0 | 20.0 | 42.0 |
| [AppleのmacOSの不備によりユーザーがセキュリティツールを無効化可能に](https://www.darkreading.com/application-security/apple-macos-security-gap-users-disable-security-tools) | 20.0 | 20.0 | 42.0 |
| [最新のTIC 3.0ソリューションにおけるSASEの活用](https://www.cisa.gov/resources-tools/resources/using-sase-modern-tic-30-solution) | 20.0 | 20.0 | 42.0 |
| [ロンドン警察、ウェストエンドでライブ顔認証を導入](https://www.theregister.com/security/2026/06/24/london-cops-bring-live-facial-recognition-to-west-end/5261031) | 20.0 | 20.0 | 42.0 |
| [Apexエージェント型攻撃者の到来](https://thehackernews.com/2026/06/dawn-of-apex-agentic-adversary.html) | 20.0 | 20.0 | 42.0 |
| [悪用可能なCI/CDの脆弱性により数百万件のリポジトリが乗っ取りの危険にさらされる](https://www.securityweek.com/exploitable-ci-cd-vulnerabilities-expose-millions-of-repositories-to-hijacking/) | 20.0 | 20.0 | 42.0 |
| [雇用が懸かる中、CEOはサイバー攻撃からの復旧を数時間単位で求めるように](https://www.itpro.com/security/with-jobs-on-the-line-ceos-now-demand-cyber-attack-recovery-in-hours-not-days-or-weeks) | 20.0 | 20.0 | 42.0 |
| [BeyondTrustとLastPassが影響を受けたKlue-Salesforceインシデント](https://www.securityweek.com/beyondtrust-lastpass-impacted-by-klue-salesforce-incident/) | 20.0 | 20.0 | 42.0 |
| [Google Workspace、パスワードリセット通知を全管理者に拡大](https://www.helpnetsecurity.com/2026/06/24/google-workspace-admin-password-reset-alerts/) | 20.0 | 20.0 | 42.0 |
| [オープンソースセキュリティが政府にとって容易に解決できない課題を生んでいる](https://cyberscoop.com/open-source-software-security-crisis/) | 20.0 | 20.0 | 42.0 |
| [DoJ、サイバー詐欺の資金洗浄に関与したHuione Cloudアカウントを押収](https://thehackernews.com/2026/06/doj-seizes-huione-cloud-account-tied-to.html) | 20.0 | 20.0 | 42.0 |
| [英国の博物館が直面するサイバーセキュリティリスク、議員が警告](https://www.infosecurity-magazine.com/news/mps-criticize-government-museum/) | 20.0 | 20.0 | 42.0 |

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
