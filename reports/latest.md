# 📡 サイレーダー 2026-07-03 05:00 JST

このレポートは、2026-07-02 17:00 JST〜2026-07-03 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 90
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 57

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [FortiBleed campaign traced to INC and Lynx ransomware operations](#topic-20603) | 53.0 | 48.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [Oracle E-Business Suite was under attack via critical flaw before the public exploit code was even released](#topic-20074) | 45.0 | 56.0 | 64.0 | 音声 | 温度感上位枠 |
| 3 | [FortiBleed Actors Collaborating With Inc, Lynx Ransomware Gangs](#topic-20586) | 45.0 | 48.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [CISA: Microsoft SharePoint RCE flaw now actively exploited](#topic-20642) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [CISA Warns of Actively Exploited Microsoft SharePoint Vulnerability](#topic-10354) | 40.0 | 64.0 | 59.0 | 音声 | 温度感上位枠 |
| 6 | [Smooth AI criminal drives 'first' end-to-end agentic ransomware attack](#topic-20590) | 33.0 | 30.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [ThreatsDay: AI Compute Hijacking, Apple Email Flaw, BlueHammer Ransomware + 14 Stories](#topic-20601) | 33.0 | 30.0 | 42.0 | 音声 | AI×Security枠 |
| 8 | [Catan and Mouse](#topic-17641) | 30.0 | 46.0 | 62.0 | GitHub | 音声枠上限によりGitHubのみ |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-20603"></a>

### 1. FortiBleed campaign traced to INC and Lynx ransomware operations

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 53.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

FortiBleedと呼ばれる攻撃活動が、INCおよびLynxのランサムウェア運用と関連づけられていると報じられています。
研究者は、関与が疑われるゼロデイ脆弱性の可能性についても調査を続けているとされています。
ランサムウェア攻撃の背後関係や利用された脆弱性の特定は、封じ込めや再発防止の優先度を判断するうえで重要です。
ゼロデイが関与している可能性があるなら、既知の対策だけでは防ぎにくい点にも注意が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 関連製品・公開情報の更新を確認し、影響有無を早急に点検する。
- 異常な認証・管理操作・暗号化の兆候がないか、ログとアラートを横断的に確認する。
- バックアップの復元性とインシデント対応手順を再点検し、隔離・報告の連絡経路を明確にする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ランサムウェアグループ | Lynx | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [FortiBleed campaign traced to INC and Lynx ransomware operations](https://www.cybersecuritydive.com/news/fortibleed-campaign-traced-to-inc-and-lynx-ransomware-operations/824348/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20074"></a>

### 2. Oracle E-Business Suite was under attack via critical flaw before the public exploit code was even released

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 64.0 |

#### 概要

Oracle E-Business SuiteのOracle Paymentsに関する重大な脆弱性CVE-2026-46817について、公開PoCが出る前から実際の攻撃が観測されたと報じられています。
対象は認証や権限管理の不備に関連するとされ、影響を受ける環境では悪用されるおそれがあります。
業務基盤として使われるOracle E-Business Suiteが対象のため、侵害されると広範な業務影響につながる可能性があります。
公開PoC以前からの悪用報告は、パッチ未適用環境にとって特に注意が必要なサインです。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
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

- Oracle E-Business Suiteの該当バージョンとパッチ適用状況を早急に確認する。
- 外部公開された関連機能へのアクセス制御と、認証・権限設定に不備がないか点検する。
- 侵害兆候の有無を確認するため、関連ログと不審な操作履歴を優先的に監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-46817 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ランサムウェアグループ | Clop | 主題 | 0.80 | — |
| ベンダー | Oracle | 言及あり | 0.80 | — |
| 製品 | Oracle E-Business Suite | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-46817](https://nvd.nist.gov/vuln/detail/CVE-2026-46817) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Oracle E-Business Suite was under attack via critical flaw before the public exp](https://www.theregister.com/cyber-crime/2026/07/02/oracle-e-business-suite-was-under-attack-via-critical-flaw-before-the-public-exploit-code-was-even-released/5265710) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Researchers spot exploitation of another critical Oracle defect](https://cyberscoop.com/oracle-ebs-critical-vulnerability-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Oracle E-Business Suite Payments flaw under attack (CVE-2026-46817)](https://www.helpnetsecurity.com/2026/06/30/oracle-payments-cve-2026-46817-exploitation/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Oracle E-Business Suite Flaw CVE-2026-46817 Actively Exploited in the Wild](https://thehackernews.com/2026/06/oracle-e-business-suite-flaw-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-20586"></a>

### 3. FortiBleed Actors Collaborating With Inc, Lynx Ransomware Gangs

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Fortinet製ファイアウォールを狙った侵害活動に関連して、Lynxランサムウェア・グループとの関与が取り上げられています。
公開材料では、攻撃者が取得したアクセスを収益化しようとしている可能性や、Nextcloudのゼロデイ脆弱性が重ねて悪用されている文脈が示されています。
境界機器への侵害は、組織内ネットワークへの足がかりになりやすく、被害が広がると復旧や封じ込めが難しくなります。
ランサムウェア関連の動きと結びつくことで、単なる侵入ではなく実害につながるリスクとして注視が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Fortinet製品の設定・ログ・管理面を点検し、不審なアクセスや予期しない変更の有無を確認する。
- Nextcloudを含む外部公開サービスについて、最新の修正適用状況と露出範囲を見直す。
- 侵害の可能性を前提に、権限の見直し、侵入検知、バックアップの復旧性確認を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ランサムウェアグループ | Lynx | 主題 | 0.80 | — |
| ベンダー | Fortinet | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [FortiBleed Actors Collaborating With Inc, Lynx Ransomware Gangs](https://www.darkreading.com/threat-intelligence/fortibleed-actors-inc-lynx-ransomware-gangs) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20642"></a>

### 4. CISA: Microsoft SharePoint RCE flaw now actively exploited

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>R⁠C⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、Microsoft SharePointのリモートコード実行（RCE）脆弱性が現在悪用されていると注意喚起しました。
Microsoftはこの問題を5月に修正済みとされており、少なくとも公開情報上はその後に攻撃者による悪用が観測された形です。
SharePointは組織内で広く使われるため、RCE脆弱性の悪用はサーバー侵害や情報漏えいにつながるおそれがあります。
公的機関が実際の悪用を示している点から、単なる注意喚起ではなく早急な対応が求められます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SharePointの該当パッチ適用状況を確認し、未適用なら優先対応する。
- インターネット公開されているSharePoint環境は、アクセス制御や監視を強める。
- 不審な管理操作、Webシェル類似の痕跡、異常なプロセス起動などの兆候を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-45659 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA: Microsoft SharePoint RCE flaw now actively exploited](https://www.bleepingcomputer.com/news/security/cisa-microsoft-sharepoint-rce-flaw-now-actively-exploited/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-10354"></a>

### 5. CISA Warns of Actively Exploited Microsoft SharePoint Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 40.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

CISAが、Microsoft SharePointに関するリモートコード実行の脆弱性CVE-2026-45659について、実際の悪用が確認されているとして注意を促しています。
Microsoftはすでに修正更新を提供しており、影響を受けるSharePoint Server系製品では早急な適用が重要です。
SharePointは企業内で広く使われるため、重大度の高いRCE脆弱性が実際に悪用されているとなると、情報漏えいや横展開の起点になり得ます。
CISAのKEV対象入りは、優先度の高い対応が求められるサインです。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
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

- 対象のSharePoint Server製品に最新の修正プログラムが適用済みか確認する。
- CISAの既知悪用脆弱性として優先度を上げ、未対応インスタンスを洗い出す。
- SharePoint周辺の監査ログや不審な管理操作、異常なプロセス起動の有無を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-45659 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-45659](https://nvd.nist.gov/vuln/detail/CVE-2026-45659) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA Warns of Actively Exploited Microsoft SharePoint Vulnerability](https://www.securityweek.com/cisa-warns-of-actively-exploited-microsoft-sharepoint-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SharePoint RCE CVE-2026-45659 Added to CISA KEV After Active Exploitation](https://thehackernews.com/2026/07/sharepoint-rce-cve-2026-45659-added-to.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches SharePoint RCE Flaw CVE-2026-45659 Across Server Versions](https://thehackernews.com/2026/05/microsoft-patches-sharepoint-rce-flaw.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [High-severity SharePoint RCE bug patched by Microsoft (CVE-2026-45659)](https://www.helpnetsecurity.com/2026/05/26/sharepoint-vulnerability-cve-2026-45659/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-20590"></a>

### 6. Smooth AI criminal drives 'first' end-to-end agentic ransomware attack

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報では、AIを悪用したとされるエンドツーエンド型のランサムウェア事案が話題になっています。
記事では、LLMや関連製品名に触れつつ、身代金を支払ってもデータが必ず戻るとは限らない点が示唆されています。
AIを組み込んだ攻撃は、従来型のランサムウェアよりも自動化・高度化の可能性があり、被害対応や交渉の前提を揺さぶります。
生成AIの業務利用が広がる中で、攻撃側のAI活用が現実の脅威としてどう現れるかを確認する材料になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIを使う業務システムでも、暗号化・バックアップ・復旧手順など基本対策の有効性を再点検する。
- 身代金支払いが復旧保証にならない前提で、復旧優先のインシデント対応計画を準備する。
- AI連携基盤や自動化フローに対し、権限分離、監査ログ、異常検知の確認を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2021-29441 | 関連CVE | 1.00 | 候補あり（URL 11件以上） |
| 脆弱性 | CVE-2025-3248 | 関連CVE | 1.00 | 候補あり（URL 30件以上） |
| ベンダー | Qwen | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Langflow | 言及あり | 0.80 | — |
| 製品 | Microsoft Azure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Smooth AI criminal drives 'first' end-to-end agentic ransomware attack](https://www.theregister.com/security/2026/07/02/smooth-ai-criminal-drives-first-end-to-end-agentic-ransomware-attack/5266073) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20601"></a>

### 7. ThreatsDay: AI Compute Hijacking, Apple Email Flaw, BlueHammer Ransomware + 14 Stories

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

今週のセキュリティ関連ニュースは、AIシステム、メールの取り扱い、ランサムウェアなど、複数の領域で「小さな隙」が問題になる傾向が目立つ内容です。
公開情報では、AI計算資源の不正利用、Apple関連のメール不備、BlueHammerランサムウェアなどが話題として挙がっています。
AIやメールのように日常業務で広く使われる仕組みが対象のため、影響範囲が特定の製品や組織に限られない可能性があります。
実務では、個別の脆弱性だけでなく、権限設定や検証不足といった運用面の弱点も見直す必要があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI関連基盤では、計算資源やアクセス権限の使われ方を定期的に確認する。
- メール連携や自動処理は、例外処理や認可の抜けがないか点検する。
- ランサムウェア文脈では、バックアップ、復旧手順、権限分離の実効性を再確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Apple | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ThreatsDay: AI Compute Hijacking, Apple Email Flaw, BlueHammer Ransomware + 14 S](https://thehackernews.com/2026/07/threatsday-ai-compute-hijacking-apple.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-17641"></a>

### 1. Catan and Mouse

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 62.0 |

#### 概要

SimpleHelpのRMM製品に関するCVE-2026-48558は、OpenID Connect（OIDC）認証の構成で認証回避につながる可能性がある脆弱性として報告されています。
報道によれば、未認証の攻撃者がTechnicianアカウントを作成し、管理対象端末へのリモート操作やスクリプト実行などに悪用された事例が観測されています。
RMM製品は管理端末に広くアクセスできるため、侵害時の影響が大きくなりやすい点が注目されています。
すでに実運用環境での悪用が報じられており、認証設定の見直しと影響確認が急がれます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SimpleHelpをOIDC認証で運用している場合は、ベンダーの修正情報と回避策を確認し、適用状況を点検する。
- Technicianアカウントの新規作成や不審な認証・管理操作のログを確認し、異常がないか点検する。
- 管理対象端末側でも、想定外のスクリプト実行やリモート接続の痕跡がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-48558 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Sekoia.io | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| 製品 | Microsoft Azure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-48558](https://nvd.nist.gov/vuln/detail/CVE-2026-48558) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Catan and Mouse](https://blog.talosintelligence.com/catan-and-mouse/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit SimpleHelp CVE-2026-48558 to Deploy TaskWeaver and Djinn Steal](https://thehackernews.com/2026/06/attackers-exploit-simplehelp-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical SimpleHelp flaw exploited to deploy new stealer malware](https://www.bleepingcomputer.com/news/security/hackers-exploit-critical-simplehelp-flaw-deploy-new-djinn-infostealer-taskweaver-malware/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SimpleHelp RMM flaw could give attackers full access to managed endpoints (CVE-2](https://www.helpnetsecurity.com/2026/06/16/simplehelp-rmm-cve-2026-48558/) | <nobr>内容確認・補足情報</nobr> |

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
| [「Exploitarium」の研究者、未公開のゼロデイ脆弱性公開の経緯を説明](https://www.infosecurity-magazine.com/news/researcher-exploitarium-exploits/) | 39.0 | 38.0 | 43.0 |
| [ランサムウェアグループがCitrix Bleed 2、BYOVD、サプライチェーンの認証情報を悪用](https://thehackernews.com/2026/07/ransomware-groups-turn-to-citrix-bleed.html) | 36.0 | 30.0 | 42.0 |
| [Ransomware集団がInterpolを装って中小企業を誘引](https://www.darkreading.com/cyberattacks-data-breaches/attackers-use-interpol-lure-target-small-businesses) | 36.0 | 30.0 | 42.0 |
| [FortiBleedキャンペーンとINC、Lynxランサムウェア攻撃の関連性](https://www.securityweek.com/fortibleed-campaign-linked-to-inc-lynx-ransomware-attacks/) | 36.0 | 30.0 | 42.0 |
| [サイバー犯罪者がInterpolを装い、フィッシングメールで被害者をランサムウェアに感染させる](https://www.infosecurity-magazine.com/news/cybercriminals-pose-interpol/) | 36.0 | 30.0 | 42.0 |
| [FortiBleedによる認証情報窃取とINCおよびLynxランサムウェア運用との関連](https://thehackernews.com/2026/07/fortibleed-credential-theft-linked-to.html) | 36.0 | 30.0 | 42.0 |
| [AI AgentがLangflowのRCEを悪用しデータベースへのランサムウェア攻撃を自動化](https://thehackernews.com/2026/07/ai-agent-exploits-langflow-rce-to.html) | 33.0 | 30.0 | 42.0 |
| [マルチエージェントAIアーキテクチャとしてのレッドチーム攻撃手法の形式化](https://www.rapid7.com/blog/post/so-red-teaming-offensive-methodology-multi-agent-ai-architecture) | 33.0 | 20.0 | 42.0 |
| [コンテキストエンジニアリング：自動マルウェア解析のための圧縮とエージェントメモリ](https://www.sentinelone.com/labs/context-engineering-compaction-agent-memory-for-automated-malware-analysis/) | 30.0 | 20.0 | 42.0 |
| [マルウェア対策ソフト「ClamAV」に複数脆弱性 - Cisco製品にも影響](https://www.security-next.com/186715) | 30.0 | 20.0 | 42.0 |
| [Gentlemenランサムウェア：知っておくべきこと](https://www.fortra.com/blog/gentlemen-ransomware-what-you-need-know) | 28.0 | 30.0 | 42.0 |
| [Googleによる悪意あるResidential Proxyネットワークへの継続的な妨害](https://cloud.google.com/blog/topics/threat-intelligence/google-continued-disruption-residential-proxy-networks/) | 28.0 | 20.0 | 48.0 |
| [FBIがNetNutプロキシプラットフォームとPopaボットネットを押収](https://krebsonsecurity.com/2026/07/fbi-seizes-netnut-proxy-platform-popa-botnet/) | 28.0 | 20.0 | 42.0 |
| [想定外の可視化課題](https://www.security.com/product-insights/visibility-challenge-nobody-asked) | 28.0 | 20.0 | 42.0 |
| [偽のGoogleおよびCloudflare認証ページが複数のマルウェアを拡散](https://www.malwarebytes.com/blog/threat-intel/2026/07/fake-google-and-cloudflare-verification-pages-spread-multiple-malware-families) | 28.0 | 20.0 | 42.0 |
| [OperaブラウザーがClickFixマルウェア攻撃の対策を提示](https://www.itpro.com/security/malware/opera-browser-thinks-it-has-the-solution-to-stopping-clickfix-malware-attacks) | 28.0 | 20.0 | 42.0 |
| [SharkLoaderがステルス性の高いCobalt Strike配信フレームワークとして台頭](https://blog.polyswarm.io/sharkloader-emerges-as-stealthy-cobalt-strike-delivery-framework) | 28.0 | 20.0 | 42.0 |
| [ToddyCat関連マルウェア「Umbrij」がOAuthを悪用してGoogle API経由でGmailにアクセス](https://thehackernews.com/2026/07/toddycat-linked-umbrij-malware-abuses.html) | 28.0 | 20.0 | 42.0 |
| [GLM-5.2の開発元による中国製AIエージェントアプリ「ZCode」、AnthropicやOpenAIのAIモデルも活用可能](https://gigazine.net/news/20260702-zcode-ai-agent/) | 27.0 | 20.0 | 42.0 |
| [オープンソースのゲームエンジン「Godot」がAI製コードを今後受け付けないことを決定、AIを多用するユーザーが自分のコードを十分に理解して修正できるとは限らないため](https://gigazine.net/news/20260702-godot-ban-ai/) | 27.0 | 20.0 | 42.0 |
| [AI駆動ソフトウェア開発の監査を成功させる方法](https://www.securityweek.com/how-to-conduct-a-successful-audit-of-ai-driven-software-development/) | 25.0 | 20.0 | 42.0 |
| [ibossの新プラットフォーム、組織のAIツールと利用状況を即時可視化](https://www.helpnetsecurity.com/2026/07/02/iboss-ai-security-platform/) | 25.0 | 20.0 | 42.0 |
| [AnthropicのAIがバグを発見、IBMは50億ドルを投じて修正に期待](https://www.darkreading.com/vulnerabilities-threats/anthropic-s-ai-finds-bugs-ibm-bets-5b-it-can-fix-them-) | 25.0 | 20.0 | 42.0 |
| [CloudflareがAIクローラのアクセスルールを変更](https://www.helpnetsecurity.com/2026/07/02/cloudflare-ai-crawler-controls/) | 25.0 | 20.0 | 42.0 |
| [MicrosoftがOutlookでCopilotボタンを消していた不具合を修正](https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-bug-that-removed-copilot-button-in-outlook/) | 25.0 | 20.0 | 42.0 |
| [AIエージェント向けに設計されていないIDライフサイクル管理](https://thehackernews.com/2026/07/identity-lifecycle-management.html) | 25.0 | 20.0 | 42.0 |
| [Trump政権、サイバーセキュリティ警戒を受けAnthropicのClaudeモデルへの制限を解除](https://www.securityweek.com/trump-administration-lifts-restrictions-on-anthropics-claude-models-after-cybersecurity-alarm/) | 25.0 | 20.0 | 42.0 |
| [Wiz MCPを使ったAIセキュリティエージェントの構築](https://www.wiz.io/blog/introducing-wiz-mcp) | 25.0 | 20.0 | 42.0 |
| [AIブラウザをだまして認証情報を盗ませる「BioShocking」攻撃](https://www.securityweek.com/bioshocking-attack-tricks-ai-browsers-into-stealing-credentials/) | 25.0 | 20.0 | 42.0 |
| [ST Engineering iDirect iQシリーズ端末](https://www.cisa.gov/news-events/ics-advisories/icsa-26-183-01) | 24.0 | 46.0 | 50.0 |
| [Gardyn IoT Hubの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-183-03) | 24.0 | 46.0 | 50.0 |
| [Microsoftは悪用の可能性は「低い」としたが、CISAがSharePointのRCEをKEVリストに追加](https://www.theregister.com/security/2026/07/02/microsoft-said-exploitation-was-less-likely-but-cisa-just-added-sharepoint-rce-to-kev-list/5265886) | 24.0 | 38.0 | 42.0 |
| [Microsoftパートナーエコシステム全体のセキュリティ体制強化](https://www.microsoft.com/en-us/security/blog/2026/07/02/improving-security-posture-across-the-microsoft-partner-ecosystem/) | 22.0 | 20.0 | 42.0 |
| [CitrixBleedの新たな脆弱性が公表直後に悪用される](https://www.securityweek.com/new-citrixbleed-vulnerability-exploited-immediately-after-public-disclosure/) | 22.0 | 20.0 | 42.0 |
| [介護サービスの評価システムにサイバー攻撃 - システムを一時停止](https://www.security-next.com/186451) | 22.0 | 20.0 | 42.0 |
| [売店保有の個人情報、商品取扱業者がカタログ送付に利用 - 山口県](https://www.security-next.com/186574) | 22.0 | 20.0 | 42.0 |
| [個人情報をメールに誤添付、容量から気づく - 阪教大](https://www.security-next.com/186643) | 22.0 | 20.0 | 42.0 |
| [Cisco、Unified CMの脆弱性が実際に悪用されていることを確認](https://www.securityweek.com/cisco-confirms-in-the-wild-exploitation-of-unified-cm-vulnerability/) | 22.0 | 20.0 | 42.0 |
| [WinRARの脆弱性により攻撃者がコンピュータを制御できる可能性](https://www.malwarebytes.com/blog/news/2026/07/winrar-flaw-could-allow-attackers-to-take-control-of-your-computer) | 20.0 | 28.0 | 50.0 |
| [CubeSpace CW0057 Reaction Wheelの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-183-02) | 20.0 | 28.0 | 50.0 |
| [Scattered Spiderの長年のメンバーとされる人物が米国へ身柄送致される](https://cyberscoop.com/scattered-spider-peter-stokes-cybercrime-extradition/) | 20.0 | 20.0 | 48.0 |
| [見逃されたインシデント、持続的な脅威、対応のギャップ：侵害アセスメントプロジェクトから得られた知見](https://securelist.com/compromise-assessment-findings-2025/120542/) | 20.0 | 20.0 | 48.0 |
| [Knossos：手続き的に生成されるデコイ環境](https://www.praetorian.com/blog/knossos-decoy-environments/) | 20.0 | 20.0 | 42.0 |
| [AppleのHide My Emailはあまりうまく隠せない](https://www.malwarebytes.com/blog/news/2026/07/apples-hide-my-email-doesnt-hide-it-very-well) | 20.0 | 20.0 | 42.0 |
| [GitHubがシークレットスキャンでインボックスゼロを実現した方法](https://github.blog/security/application-security/how-github-used-secret-scanning-to-reach-inbox-zero/) | 20.0 | 20.0 | 42.0 |
| [Ctrl+Alt+Oops: FortiBleedの犯人のログイン情報が2つのギャングを結びつける](https://www.theregister.com/security/2026/07/02/ctrlaltoops-fortibleed-criminals-logins-stitch-two-gangs-together/5265912) | 20.0 | 20.0 | 42.0 |
| [サイバーセキュリティ担当者の多くが侵害の隠蔽を指示されたとの調査結果](https://www.cybersecuritydive.com/news/data-breach-coverups-ai-bitdefender/824331/) | 20.0 | 20.0 | 42.0 |
| [ConsentFixとClickFix：Microsoft 365アカウントが3秒で乗っ取られる仕組み](https://www.bleepingcomputer.com/news/security/consentfix-and-clickfix-how-microsoft-365-accounts-are-hijacked-in-3-seconds/) | 20.0 | 20.0 | 42.0 |
| [Scattered Spider関係者、800万ドルの身代金要求事件で身柄引き渡し](https://www.helpnetsecurity.com/2026/07/02/scattered-spider-criminal-group-suspect-extradited/) | 20.0 | 20.0 | 42.0 |
| [PacemakerメーカーMedtronic、患者の健康データがサイバー犯罪者に窃取された可能性を警告](https://www.theregister.com/security/2026/07/02/pacemaker-manufacturer-medtronic-warns-patients-cybercrooks-may-have-swiped-health-data/5265768) | 20.0 | 20.0 | 42.0 |
| [WhatsAppのユーザー名導入を巡り、インドがセキュリティ懸念の中で3日以内の説明を要求](https://www.theregister.com/security/2026/07/02/india-writes-to-whatsapp-over-usernames-security-concerns/5265744) | 20.0 | 20.0 | 42.0 |
| [Cisco、Unified CMの脆弱性を悪用する攻撃者の存在を確認](https://www.bleepingcomputer.com/news/security/cisco-finally-confirms-attackers-exploiting-unified-cm-flaw/) | 20.0 | 20.0 | 42.0 |
| [Opera、ClickFix攻撃対策のPaste Protect機能を導入](https://www.bleepingcomputer.com/news/security/opera-rolls-out-paste-protect-feature-to-fight-clickfix-attacks/) | 20.0 | 20.0 | 42.0 |
| [NCSCがペンテスターの作業を難しくするためのヒントを共有](https://www.infosecurity-magazine.com/news/ncsc-tips-make-pen-testers-job/) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderのハッカーとされる人物がフィンランドで拘束され米国へ送還](https://www.itpro.com/security/cyber-crime/alleged-scattered-spider-hacker-snared-in-finland-extradited-to-us) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderのハッカーが米国へ身柄引き渡し](https://www.bleepingcomputer.com/news/security/alleged-scattered-spider-hacker-extradited-to-the-united-states/) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderのメンバーとされる人物が米国に送還される](https://www.infosecurity-magazine.com/news/scattered-spider-member-extradited/) | 20.0 | 20.0 | 42.0 |

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
