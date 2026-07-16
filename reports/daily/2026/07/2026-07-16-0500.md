# 📡 サイレーダー 2026-07-16 10:32 JST

このレポートは、2026-07-15 22:32 JST〜2026-07-16 10:32 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 93
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 2
- [低温だが記録しておくトピック](#low-record-topics): 55

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-15409: CISA KEV catalog addition](#topic-22364) | 62.0 | 74.0 | 67.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [Microsoft 2026年7月 Patch Tuesday 関連まとめ](#topic-22358) | 46.0 | 48.0 | 57.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN Validator Authenticated Privilege Escalation Vulnerability](#topic-15753) | 43.0 | 58.0 | 66.0 | 音声 | 温度感上位枠 |
| 4 | [「Oracle EBS」やビル設備向けプロトコルの脆弱性を悪用する攻撃](#topic-22685) | 39.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [CISA Urges Immediate Patching of Exploited SharePoint Vulnerabilities](#topic-22603) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [TuxBot v3 Evolution Shows Signs of LLM-Assisted IoT Botnet Development](#topic-22577) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 7 | [Google Gemini CLI abused as a hacking agent, malware botnet operator](#topic-22578) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-15753"></a>

### 1. Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN Validator Authenticated Privilege Escalation Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Catalyst SD-WAN Controller／Manager／Validator に、認証済みのローカル攻撃者が root 権限で任意コマンドを実行できる可能性のある脆弱性（CVE-2026-20245）が報告されています。
Cisco は、この問題が悪用された事例を確認しているとしており、現時点では対象製品の一部に対して未修正の状態が続いています。
SD-WAN の管理基盤はネットワーク運用の中枢にあたるため、権限昇格が成立すると影響範囲が大きくなりやすいです。
さらに、悪用観測があるとされる点から、単なる理論上の脆弱性ではなく、優先度を上げて確認すべき事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
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

#### 担当者向け確認ポイント

- 対象製品の利用有無とバージョンを確認し、Cisco の案内に沿って更新状況や回避策を点検する。
- 管理者権限や netadmin 権限のアカウントを見直し、不要なアカウントや不審な変更がないか監査する。
- SD-WAN 管理系システムのログを確認し、想定外のファイル操作や権限変更、root 相当のアクティビティを重点的に追跡する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20127 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-20182 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-20245 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-33017 | 関連CVE | 1.00 | 候補あり（URL 4件以上） |
| 脆弱性 | CVE-2026-34908 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-34909 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34910 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-41947 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-41948 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-55255 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20245](https://nvd.nist.gov/vuln/detail/CVE-2026-20245) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN V](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-privesc-4uxFrdzx) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [22nd June – Threat Intelligence Report](https://research.checkpoint.com/2026/22nd-june-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [29th June – Threat Intelligence Report](https://research.checkpoint.com/2026/29th-june-threat-intelligence-report-2/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco SD-WAN Zero-Day Exploited Months Before Patching](https://www.securityweek.com/cisco-sd-wan-zero-day-exploited-months-before-patching/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Zero-Day CVE-2026-20245 Exploited to Gain Root Access](https://thehackernews.com/2026/06/cisco-catalyst-sd-wan-zero-day-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Mandiant reveals how Cisco SD-WAN zero-day attacks gained root access](https://www.bleepingcomputer.com/news/security/mandiant-reveals-how-cisco-sd-wan-zero-day-attacks-gained-root-access/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zero-Day Exploitation of Vulnerability (CVE-2026-20245) in Cisco Catalyst SD-WAN](https://cloud.google.com/blog/topics/threat-intelligence/zero-day-exploitation-cisco-catalyst-sd-wan-manager/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-22685"></a>

### 2. 「Oracle EBS」やビル設備向けプロトコルの脆弱性を悪用する攻撃

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

米当局が、Oracle E-Business Suiteやビル設備などで利用されるKNXプロトコルの脆弱性がサイバー攻撃に悪用されているとして注意喚起しました。
現時点で、公開材料からは個別のCVEや詳細な攻撃手法までは確認できません。
業務基盤のERPと、建物制御などのOT/IoT寄りの領域が同時に話題になっており、影響範囲が広がる可能性があります。
実際の悪用が示唆されているため、一般的な脆弱性情報よりも優先度を上げて確認すべき案件です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Oracle E-Business Suiteの利用有無と、関連する公開面・接続経路を確認する。
- KNXを含むビル設備系機器や連携システムの資産把握、更新状況、外部公開状態を点検する。
- ベンダーや公的機関の注意喚起を継続監視し、該当環境では監視強化と緊急パッチ適用可否を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2023-4346 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-46817 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Oracle | 言及あり | 0.80 | — |
| 製品 | Oracle E-Business Suite | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [「Oracle EBS」やビル設備向けプロトコルの脆弱性を悪用する攻撃](https://www.security-next.com/187455) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22603"></a>

### 3. CISA Urges Immediate Patching of Exploited SharePoint Vulnerabilities

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、Microsoft SharePointに関連する脆弱性について、直ちに修正を適用するよう呼びかけています。
公開情報によれば、3件の脆弱性が実際の攻撃で悪用されており、そのうち2件はゼロデイとして狙われたとされています。
業務でSharePointを利用している組織では、対応の遅れが侵害リスクにつながるため注意が必要です。
公的機関が悪用確認を踏まえて対処を促している点から、優先度の高い警戒対象といえます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SharePointの利用有無を確認し、該当環境の更新状況を早急に点検する。
- ベンダーと公的機関の通知を継続的に確認し、該当パッチや緩和策を優先適用する。
- 外部公開されたSharePoint環境については、異常なアクセスや不審な挙動がないか監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-32201 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-45659 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-55040 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-56164 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-58644 | 関連CVE | 1.00 | 未確認 |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Urges Immediate Patching of Exploited SharePoint Vulnerabilities](https://www.securityweek.com/cisa-urges-immediate-patching-of-exploited-sharepoint-vulnerabilities/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22577"></a>

### 4. TuxBot v3 Evolution Shows Signs of LLM-Assisted IoT Botnet Development

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>A⁠I</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者は、未報告のIoTボットネット基盤「TuxBot v3 Evolution」について、LLMの支援を受けて開発された可能性があると指摘しました。
ただし、公開された内容ではAIの出力に安全上の注記が残るなど、開発の完成度には課題があったとみられます。
AIを悪用した脅威開発の兆候として注目されており、攻撃者側の開発効率化やコード生成の実態を考える材料になります。
IoT機器を狙うボットネットは依然としてリスクが高く、防御側は手口の変化を継続的に追う必要があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- IoT機器の不要な公開サービスや古い認証設定を見直し、露出を最小化する。
- ボットネット由来の不審な通信や、短時間に繰り返される接続試行を監視する。
- AI支援の有無にかかわらず、既存のIoT脅威対策と脆弱性管理を継続する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [TuxBot v3 Evolution Shows Signs of LLM-Assisted IoT Botnet Development](https://thehackernews.com/2026/07/tuxbot-v3-evolution-shows-signs-of-llm.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（1件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22578"></a>

### 5. Google Gemini CLI abused as a hacking agent, malware botnet operator

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、GoogleのオープンソースAIツール「Gemini CLI」が、脅威アクターにより不正に利用されたとされています。
報道では、ハッキング支援や小規模なボットネット運用に使われた可能性が示されていますが、詳細は限定的です。
生成AIやCLI型ツールが、正規の用途だけでなく攻撃支援に転用されうることを示す事例として注目されています。AIツールの利用状況や権限設定、監査の重要性を改めて意識させます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIツールの実行権限や接続先を最小化し、不要な機能は無効化する。
- ログ監査と異常検知を強化し、想定外の自動化・連続実行を早期に把握する。
- 社内でのAI利用ポリシーを明確にし、開発・運用環境での持ち込み利用を管理する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Google | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | Google Gemini | 主題 | 0.80 | — |
| AIモデル/プロジェクト | Gemini | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Google Gemini CLI abused as a hacking agent, malware botnet operator](https://www.bleepingcomputer.com/news/security/google-gemini-cli-abused-as-a-hacking-agent-malware-botnet-operator/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-22364"></a>

### 1. CVE-2026-15409: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 62.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

CVE-2026-15409は、SonicWall SMA 1000シリーズ機器に影響する脆弱性としてCISAのKEVカタログに追加された話題です。
複数の報道では、同時に公表された別の脆弱性とともに実際の悪用が確認されているとされ、SonicWallは修正版への更新を案内しています。
KEVへの追加は、少なくとも一部環境で優先対応が必要と見なされる指標になります。対象機器が外部公開されている場合、影響評価と更新、侵害痕跡の確認を急ぐ必要があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
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

- SMA 1000シリーズの導入有無を確認し、該当する場合は修正版への更新を優先する。
- 公開情報で示されている侵害痕跡の有無を点検し、異常があれば追加調査を行う。
- 管理者・利用者の認証情報や多要素認証トークンの見直しを含め、関連アカウントの安全性を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-15409 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-15410 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | SonicWall | 言及あり | 0.80 | — |
| 製品 | SonicWall SMA | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-15409](https://nvd.nist.gov/vuln/detail/CVE-2026-15409) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Rapid7 MDR Team Discovers New SonicWall SMA1000 Zero Days being Actively Exploit](https://www.rapid7.com/blog/post/etr-rapid7-mdr-team-discovers-new-sonicwall-sma1000-zero-days-being-actively-exploited-cve-2026-15409-cve-2026-15410) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Two SonicWall SMA 1000 Zero-Days Exploited, One Could Enable Admin Commands](https://thehackernews.com/2026/07/two-sonicwall-sma-1000-zero-days.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall Issues Urgent SMA Patch Warning for Two Zero-Day Exploits](https://www.securityweek.com/sonicwall-issues-urgent-sma-patch-warning-for-two-zero-day-exploits/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall warns of SMA1000 flaws exploited in zero-day attacks, patch now](https://www.bleepingcomputer.com/news/security/sonicwall-warns-of-sma1000-flaws-exploited-in-zero-day-attacks-patch-now/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall SMA appliances targeted in zero-day attacks (CVE-2026-15409, CVE-2026-](https://www.helpnetsecurity.com/2026/07/14/sonicwall-sma-attacks-via-cve-2026-15409-cve-2026-15410/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-22358"></a>

### 2. Microsoft 2026年7月 Patch Tuesday 関連まとめ

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>A⁠I</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 冷却中 |
| <nobr>温⁠度⁠感</nobr> | 46.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 57.0 |

#### 概要

Microsoftの2026年7月のPatch Tuesdayでは、622件の脆弱性が修正され、別途Chromium由来の脆弱性もEdgeに影響するとされています。
62件が重要度Criticalで、少なくとも2件は既に悪用が確認され、1件は事前公表済みとされています。
件数が非常に多く、ゼロデイや既に悪用されている脆弱性が含まれるため、優先度を付けた迅速な対応が必要です。
Windowsや関連製品の更新適用遅れは、侵害リスクの上昇につながります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 12 sources。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 悪用済みとされる脆弱性を優先して、対象システムへの更新適用状況を確認する。
- Windows本体だけでなく、Edgeなど関連コンポーネントの更新も漏れなく反映する。
- 資産範囲を洗い出し、業務影響の大きい端末・サーバーから段階的に適用計画を立てる。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-26145 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-27690 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-33842 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34328 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34346 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34348 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34349 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-40378 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-40400 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-40422 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft cancels Patch Tuesday for some Dell users over surprise shutdowns, ove](https://www.theregister.com/os-platforms/2026/07/15/microsoft-cancels-patch-tuesday-for-some-dell-users-over-surprise-shutdowns-overheating-devices/5271691) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [July 2026 Patch Tuesday fixes 622 Microsoft CVEs, including three zero-days](https://www.malwarebytes.com/blog/bugs/2026/07/july-2026-patch-tuesday-fixes-622-microsoft-cves-including-three-zero-days) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft smashes Patch Tuesday record for second successive month](https://therecord.media/microsoft-vulnerabilities-patch-tuesday-release) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Researcher Drops New Windows Zero-Day PoC Hours After Microsoft Patch Tuesday](https://thehackernews.com/2026/07/researcher-drops-new-windows-zero-day.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [AI-driven bug hunting fuels record Microsoft Patch Tuesday](https://www.helpnetsecurity.com/2026/07/15/microsoft-patch-tuesday-sharepoint-cve-2026-56164/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches 570 CVEs in Record Patch Tuesday](https://www.infosecurity-magazine.com/news/microsoft-570-cves-patch-tuesday/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Patch Tuesday - July 2026](https://www.rapid7.com/blog/post/em-patch-tuesday-july-2026) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: あり（1件）。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Identity攻撃がExploitを上回り、Ransomwareの主因に](https://www.darkreading.com/identity-access-management-security/identity-attacks-overtake-exploits-top-ransomware-cause) | 31.0 | 33.0 | 43.0 |
| [「Mac」狙いの新型マルウェア出現、クラッシュレポートツールを装う](https://japan.zdnet.com/article/35250633/) | 29.0 | 20.0 | 42.0 |
| [npmサプライチェーン攻撃は新段階に ClaudeやCursorを狙う自己増殖マルウェアの正体](https://atmarkit.itmedia.co.jp/ait/articles/2607/16/news039.html) | 29.0 | 20.0 | 42.0 |
| [AsyncAPIのnpmパッケージが認証情報窃取マルウェアに感染](https://www.bleepingcomputer.com/news/security/-asyncapi-npm-packages-infected-with-credential-stealing-malware/) | 28.0 | 45.0 | 42.0 |
| [TELEPUZ：CLICKFIX-VIDAR連鎖を通じて拡散するモジュラー型MaaSマルウェア](https://www.elastic.co/security-labs/telepuz-maas-malware-clickfix) | 28.0 | 20.0 | 42.0 |
| [OkoBotマルウェアフレームワークがLedgerとTrezorアプリにシードフレーズ詐取を注入](https://thehackernews.com/2026/07/okobot-malware-framework-injects-seed.html) | 28.0 | 20.0 | 42.0 |
| [eCardsを悪用してRMMツールを配布するフィッシングキャンペーン](https://www.infosecurity-magazine.com/news/seasonalinvite-phishing-ecards-rmm/) | 28.0 | 20.0 | 42.0 |
| [LabubaRATマルウェアがNVIDIAソフトウェアを装ってWindowsシステムに侵入](https://www.helpnetsecurity.com/2026/07/15/labubarat-rust-malware-nvidia-disguise/) | 28.0 | 20.0 | 42.0 |
| [Threat actorがGitHubで数百のブランドをなりすまし、情報窃取マルウェアを拡散](https://www.helpnetsecurity.com/2026/07/15/impersonated-brands-github-infostealer-download/) | 28.0 | 20.0 | 42.0 |
| [私たちは脆弱性自動生成機を作った：AIトークンを投入するとゼロデイが出てくる](https://www.bleepingcomputer.com/news/security/we-built-a-vulnerability-vending-machine-ai-tokens-in-zero-days-out/) | 27.0 | 20.0 | 43.0 |
| [日本IBM、AI駆動開発ソリューション「ALSEA」を発表--みずほFGの導入成果](https://japan.zdnet.com/article/35250623/) | 26.0 | 20.0 | 42.0 |
| [Excel資産を真のレガシーに 維持する手間は生成AIで省く](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020900021/070700221/) | 26.0 | 20.0 | 42.0 |
| [AIエージェントのID管理に4つの課題、過剰な権限を持たせず「小さく」設計](https://xtech.nikkei.com/atcl/nxt/column/18/03687/071000002/) | 26.0 | 20.0 | 42.0 |
| [富士通は「FDE＋C」、デロイトは「MDM」 AI時代に多様化するコンサル像](https://xtech.nikkei.com/atcl/nxt/column/18/03648/070800003/) | 26.0 | 20.0 | 42.0 |
| [Trump政権、サイバー脆弱性向けAI支援クリアリングハウスを発表](https://therecord.media/gold-eagle-cybersecurity-vulnerabilities-clearinghouse) | 25.0 | 20.0 | 42.0 |
| [「Tech-xit」は間近か？ AIを巡る対立の中で英国が主権確保を加速](https://www.darkreading.com/cybersecurity-operations/tech-xit-uk-sovereignty-push-amid-ai-strife) | 25.0 | 20.0 | 42.0 |
| [サイバーセキュリティ専門家がAIツールを導入する一方で、誤りの修正や出力確認に疲弊している件](https://www.itpro.com/security/cyber-professionals-are-flocking-to-ai-tools-but-theyre-getting-tired-of-fixing-mistakes-and-reviewing-outputs) | 25.0 | 20.0 | 42.0 |
| [Claudeの脆弱性でAIエージェントに悪意あるプロンプトが自動送信される](https://www.darkreading.com/vulnerabilities-threats/claude-flaw-malicious-prompts-ai-agents) | 25.0 | 20.0 | 42.0 |
| [AIの急増する脆弱性に対応するため米国が脆弱性情報集約拠点を設置](https://www.cybersecuritydive.com/news/vulnerability-clearinghouse-ai-white-house-launch-gold-eagle/825298/) | 25.0 | 20.0 | 42.0 |
| [Claude for Chromeの不具合により不正な拡張機能がGmailにアクセス可能に](https://www.malwarebytes.com/blog/news/2026/07/claude-for-chrome-flaw-could-let-rogue-extensions-access-your-gmail) | 25.0 | 20.0 | 42.0 |
| [F5 Insight for ADSPがガイド付きアップデートとAI監査証跡でBIG-IP運用を強化](https://www.helpnetsecurity.com/2026/07/15/f5-insight-for-adsp/) | 25.0 | 20.0 | 42.0 |
| [Zoomが警告する重大なアカウント乗っ取り脆弱性](https://www.bleepingcomputer.com/news/security/zoom-warns-of-critical-account-takeover-vulnerability/) | 24.0 | 38.0 | 42.0 |
| [「Veeam Updater」に権限昇格の脆弱性 - root権限取得のおそれ](https://www.security-next.com/187449) | 22.0 | 20.0 | 42.0 |
| [Windows版「Zoom」に深刻な脆弱性 - 最新版で修正済み](https://www.security-next.com/187443) | 22.0 | 20.0 | 42.0 |
| [Defender Expertsで脅威インテリジェンスを迅速な対処につなげる方法](https://www.microsoft.com/en-us/security/blog/2026/07/15/turning-threat-intelligence-into-decisive-action-with-defender-experts/) | 22.0 | 20.0 | 42.0 |
| [AI時代に従来型SASEは通用する？ フォーティネットが示す次世代アーキテクチャ](https://ascii.jp/elem/000/004/419/4419558/?rss=) | 21.0 | 20.0 | 42.0 |
| [Nginx UI における認証されていない利用者がバックアップファイルのダウンロードが可能となる脆弱性（Scan Tech Report）](https://scan.netsecurity.ne.jp/article/2026/07/16/55719.html) | 21.0 | 20.0 | 42.0 |
| [取引先に送付した「注文書フォーム」エクセルファイル内に顧客リストが残存](https://scan.netsecurity.ne.jp/article/2026/07/16/55718.html) | 21.0 | 20.0 | 42.0 |
| [停職 30 日の処分 ～ 医療従事者が患者の入院の事実と病状を示唆する内容を発言](https://scan.netsecurity.ne.jp/article/2026/07/16/55717.html) | 21.0 | 20.0 | 42.0 |
| [フィルタを解除すると全員のデータが閲覧可能なファイルを誤送信](https://scan.netsecurity.ne.jp/article/2026/07/16/55716.html) | 21.0 | 20.0 | 42.0 |
| [近畿大学薬学部の教員が個人情報が記載されたファイルをGoogleドライブ上で誤って学生に共有](https://scan.netsecurity.ne.jp/article/2026/07/16/55715.html) | 21.0 | 20.0 | 42.0 |
| [ニチレイへの不正アクセスによるシステム障害、冷蔵倉庫の入出庫業務や冷凍食品出荷業務に影響](https://scan.netsecurity.ne.jp/article/2026/07/16/55714.html) | 21.0 | 20.0 | 42.0 |
| [定番コマンド「GNU Wget」に脆弱性、意図しないリクエストを強制されるサーバサイドリクエストフォージェリに注意](https://scan.netsecurity.ne.jp/article/2026/07/16/55713.html) | 21.0 | 20.0 | 42.0 |
| [2026年度「ICT-ISAC表彰」発表、NEC川上氏・オプテージ清水氏・IIJ桃井氏が受賞](https://scan.netsecurity.ne.jp/article/2026/07/16/55712.html) | 21.0 | 20.0 | 42.0 |
| [注目の「SCS評価制度」最新動向をキャッチ、IPA がメルマガ登録受付中](https://scan.netsecurity.ne.jp/article/2026/07/16/55711.html) | 21.0 | 20.0 | 42.0 |
| [PHP向けパッケージ管理ツール「Composer」に脆弱性 更新前に確認したい3つのリスク](https://atmarkit.itmedia.co.jp/ait/articles/2607/16/news040.html) | 21.0 | 20.0 | 42.0 |
| [「国産だから安心」はもう通用しない？ セキュリティ新基準「日本度」の詳細を深掘り](https://atmarkit.itmedia.co.jp/ait/articles/2607/16/news019.html) | 21.0 | 20.0 | 42.0 |
| [AI導入を急ぐ企業に迫る「静かな崩壊」 被害を最小化するレジリエンスの鉄則とは？](https://techtarget.itmedia.co.jp/tt/news/2607/16/news05.html) | 21.0 | 20.0 | 42.0 |
| [脆弱性放置が平均345日 検知はできても直せない「死角」の正体](https://techtarget.itmedia.co.jp/tt/news/2607/16/news09.html) | 21.0 | 20.0 | 42.0 |
| [Apache Tomcatにおける複数の脆弱性(2026年7月14日)](https://jvn.jp/vu/JVNVU95286373/) | 20.0 | 28.0 | 50.0 |
| [Cisco Identity Services Engineのパストラバーサル脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-traversal-xNt7wb2Y) | 20.0 | 28.0 | 50.0 |
| [オランダ警察、1億ユーロ超をだまし取った投資詐欺グループを摘発](https://www.bleepingcomputer.com/news/security/dutch-police-bust-investment-fraud-ring-stealing-over-100-million/) | 20.0 | 20.0 | 42.0 |
| [Secure Bootの盲点を露呈する忘れられたブートローダー](https://www.darkreading.com/cyber-risk/forgotten-bootloaders-expose-secure-boot-blind-spot) | 20.0 | 20.0 | 42.0 |
| [Security researchers、Chromeの同期機能を悪用するストーカー行為を発見](https://cyberscoop.com/google-chrome-sync-cyberstalking-exploit/) | 20.0 | 20.0 | 42.0 |
| [Google Chromeの複数の脆弱性により任意のコードが実行される可能性](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-google-chrome-could-allow-for-arbitrary-code-execution_2026-069) | 20.0 | 20.0 | 42.0 |
| [DNI指名のJay Clayton氏、選挙セキュリティの質問で民主党議員から追及されるも失望広がる](https://cyberscoop.com/jay-clayton-dni-confirmation-hearing-election-security/) | 20.0 | 20.0 | 42.0 |
| [ヨーロッパのサイバー防御者の皆さまへ、Guten Tag、Bonjour、Hola！](https://www.darkreading.com/threat-intelligence/guten-tag-bonjour-hola-european-cyber-defenders) | 20.0 | 20.0 | 42.0 |
| [Operation Fake KickOff：攻撃者が採用担当者とSaaSを悪用して勤務用認証情報を窃取](https://www.intel471.com/blog/operation-fake-kickoff-attackers-abuse-recruiters-and-saas-to-harvest-work-credentials) | 20.0 | 20.0 | 42.0 |
| [Trump氏のDNI指名候補、選挙セキュリティと有権者不正を巡り追及される](https://therecord.media/jay-clayton-odni-nominee-senate-confirmation-hearing) | 20.0 | 20.0 | 42.0 |
| [23andMe、大規模漏えいで各州と1800万ドルの和解へ](https://therecord.media/genetic-testing-settlement-data-breach) | 20.0 | 20.0 | 42.0 |
| [モデルは忘れよう。サイバーセキュリティで重要なのはハーネスです](https://cyberscoop.com/ai-cybersecurity-harness-autonomous-hacking/) | 20.0 | 20.0 | 42.0 |
| [CISAがSharePointの複数の脆弱性が悪用されていると警告](https://www.cybersecuritydive.com/news/cisa-multiple-vulnerabilities-sharepoint-exploitation/825306/) | 20.0 | 20.0 | 42.0 |
| [未修正のCursor脆弱性によりユーザーがコード実行の危険にさらされる](https://www.securityweek.com/unpatched-cursor-vulnerability-exposes-users-to-code-execution/) | 20.0 | 20.0 | 42.0 |
| [脆弱なUEFI Shim 11件がSecure Bootのバイパスを可能にする](https://www.infosecurity-magazine.com/news/uefi-shims-secure-boot-bypass/) | 20.0 | 20.0 | 42.0 |
| [Xint PulseがWebアプリケーション向けオンデマンドのブラックボックス侵入テストを提供](https://www.helpnetsecurity.com/2026/07/15/xint-pulse/) | 20.0 | 20.0 | 42.0 |

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
