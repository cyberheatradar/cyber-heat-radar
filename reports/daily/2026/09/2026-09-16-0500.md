# 📡 サイレーダー 2026-09-16 05:00 JST

このレポートは、2026-09-15 17:00 JST〜2026-09-16 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 110
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 2
- [低温だが記録しておくトピック](#low-record-topics): 78

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cisco patches actively exploited email gateway zero-day (CVE-2026-76461)](#topic-32497) | 62.0 | 74.0 | 67.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [Microsoft 2026年9月 Patch Tuesday 関連まとめ](#topic-31499) | 57.0 | 60.0 | 57.0 | GitHub | audio_eligible_by_public_rules_false |
| 3 | [China spy chief points at US AI models in cyber threat warning](#topic-32726) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 4 | [Human Attacker Exploits Marimo RCE, Reaches SSH Bastion in Eight Seconds](#topic-32751) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 5 | [CISA: Critical VMware RCE flaw now exploited by ransomware gangs](#topic-32736) | 32.0 | 48.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [Multiple Vulnerabilities in Cisco Secure Email Products Could Allow for Remote Code Execution](#topic-32716) | 32.0 | 38.0 | 42.0 | 音声 | 温度感上位枠 |
| 7 | [Iranian cyber targeting of dissidents, activists and journalists](#topic-32739) | 31.0 | 20.0 | 43.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-32726"></a>

### 1. China spy chief points at US AI models in cyber threat warning

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

中国の情報機関トップが、米国のAIモデルをサイバー脅威の文脈で取り上げ、脆弱性探索やマルウェア関連の能力向上につながり得ると警告したと報じられています。
今回の件は、特定製品の実害を示すものではなく、AIが攻撃側・防御側の両面でサイバー能力を押し上げるという懸念を再確認させる話題です。
AIの進化が、脆弱性調査や悪用可能性の評価、攻撃の自動化をめぐるリスク認識に影響していることを示しています。
セキュリティ担当者にとっては、AI利用のガバナンスや検知・監視体制の見直しを考えるきっかけになります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI利用時の入力データ管理と権限分離を改めて確認する。
- 脆弱性調査や検知ルールの自動化にAIを使う場合は、誤判定や過信を前提に検証する。
- 攻撃の巧妙化を見据え、フィッシング対策やログ監視、異常挙動の検出を継続強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Anthropic | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [China spy chief points at US AI models in cyber threat warning](https://therecord.media/china-spy-chief-warns-of-us-ai-models) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32751"></a>

### 2. Human Attacker Exploits Marimo RCE, Reaches SSH Bastion in Eight Seconds

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>R⁠C⁠E</nobr> / <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Sysdigの報告として、脆弱なMarimoノートブックへの侵入後、攻撃者がごく短時間でSSHバスチョンへ到達した事例が紹介されています。
AIによって攻撃の速度が上がるという文脈の中で、人手による攻撃でも初期侵入後の展開が非常に速いことを示す内容です。
初期侵入後の横展開や重要経路への到達が短時間で起こりうるため、検知と封じ込めの遅れがそのまま被害拡大につながります。
AI関連の話題ですが、実際には人間の攻撃者の迅速な操作能力にも注意が必要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Marimoのような外部公開サービスやノートブック基盤の露出状況、認証設定、権限分離を確認する。
- SSHバスチョンなど重要な中継点への到達を前提に、監査ログ・アラート・多要素認証の有効性を点検する。
- 初期侵入後の短時間の横展開を想定し、封じ込め手順とインシデント対応の初動速度を見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Human Attacker Exploits Marimo RCE, Reaches SSH Bastion in Eight Seconds](https://thehackernews.com/2026/09/human-attacker-exploits-marimo-rce.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32736"></a>

### 3. CISA: Critical VMware RCE flaw now exploited by ransomware gangs

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 32.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

CISAは、7月に修正されたVMware vCenter Serverの重大な脆弱性を悪用する攻撃について注意喚起しました。
公開情報では、これまでの攻撃に加えてランサムウェア グループも関与しているとされています。仮想化基盤の管理製品が狙われると、広範な環境に影響が及ぶ可能性があります。
ランサムウェア文脈での悪用が示されているため、未対応環境の早期確認が重要です。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- VMware vCenter Serverの修正状況を確認し、該当パッチが適用済みか点検する。
- 外部公開されている管理面の露出やアクセス制御を見直し、不要な公開を避ける。
- 不審な管理操作や認証関連の異常がないか、監査ログとアラートを重点的に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-60710 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-59310 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Broadcom | 言及あり | 0.80 | — |
| 製品 | VMware vCenter Server | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA: Critical VMware RCE flaw now exploited by ransomware gangs](https://www.bleepingcomputer.com/news/security/cisa-critical-vmware-vcenter-rce-flaw-now-exploited-by-ransomware-gangs/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32716"></a>

### 4. Multiple Vulnerabilities in Cisco Secure Email Products Could Allow for Remote Code Execution

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>R⁠C⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 32.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Cisco Secure Email製品群に複数の脆弱性が見つかっており、最も深刻なものはリモートコード実行につながる可能性があるとされています。
対象には Cisco Secure Email Gateway と Cisco Secure Email and Web Manager が含まれ、影響が及ぶと機器の完全侵害につながるおそれがあります。
メールセキュリティ基盤は組織の受信防御や運用管理の要となるため、影響範囲が広くなりやすい点が注目されています。
特に管理系製品を含むため、侵害時の影響はメール経路だけでなく運用面にも及ぶ可能性があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Cisco の案内を確認し、該当製品とバージョンの影響有無を点検する。
- 公開情報に基づく対処状況を確認し、優先度を上げて更新計画を立てる。
- 管理画面や関連ログの不審な挙動を点検し、必要に応じて監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20353 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-76440 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-76441 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-76443 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-76461 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Multiple Vulnerabilities in Cisco Secure Email Products Could Allow for Remote C](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-cisco-secure-email-products-could-allow-for-remote-code-execution_2026-096) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32739"></a>

### 5. Iranian cyber targeting of dissidents, activists and journalists

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>国⁠家⁠支⁠援</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 31.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

英国NCSCは、CHOSEN BRICKマルウェアに関する注意喚起を公表し、イランによる反体制派、活動家、ジャーナリストを狙ったサイバー活動について説明しました。
技術的な分析に加え、個人や組織向けの防御上の助言も示されています。標的が特定の個人・団体に向いているため、一般的な大規模攻撃とは異なるリスク管理が必要です。
公的機関の注意喚起として、関連分野の組織は監視強化と利用者保護の見直しを検討する材料になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象者へのフィッシングや端末侵害を前提に、アカウント保護と多要素認証の徹底を確認する。
- 端末の更新状況、管理権限、監視ログを点検し、異常な挙動の早期検知に備える。
- 高リスクの利用者には、通信手段や端末利用ルールを含む安全対策の周知を行う。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Iranian cyber targeting of dissidents, activists and journalists](https://www.ncsc.gov.uk/news/iranian-cyber-targeting-of-dissidents-activists-and-journalists) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-32497"></a>

### 1. Cisco patches actively exploited email gateway zero-day (CVE-2026-76461)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 62.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Cisco Secure Email Gatewayに影響するCVE-2026-76461について、実際に悪用されているゼロデイ脆弱性として注意喚起が出ています。
影響を受ける環境では、細工されたメール処理を通じて深刻な権限でのコード実行につながるおそれがあり、Ciscoは修正アップデートを公開しています。
メールゲートウェイは社内外の通信の入口にあたるため、侵害されると広範囲の影響につながりやすい点が重要です。
加えて、公開情報では悪用やPoCの言及もあり、対応の遅れがリスクを高めます。

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

- 該当するCisco AsyncOS / Secure Email Gatewayの利用有無とバージョンを確認し、修正済み版へ速やかに更新する。
- Ciscoが示す侵害痕跡やアドバイザリの確認項目を点検し、不審な挙動がないかログを確認する。
- メールゲートウェイ周辺の監視を強化し、異常な送受信や管理操作の兆候を優先的に洗い出す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-76461 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-76461](https://nvd.nist.gov/vuln/detail/CVE-2026-76461) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco email security boxes can be rooted by... an email](https://www.theregister.com/security/2026/09/15/cisco-email-security-boxes-can-be-rooted-by-an-email/5296604) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns customers of actively exploited zero-day in email gateways](https://cyberscoop.com/cisco-secure-email-gateway-zero-day-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-76461: Critical Cisco Secure Email Gateway Vulnerability Exploited in t](https://www.rapid7.com/blog/post/etr-cve-2026-76461-critical-cisco-secure-email-gateway-vulnerability-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco patches actively exploited email gateway zero-day (CVE-2026-76461)](https://www.helpnetsecurity.com/2026/09/15/cve-2026-76461-cisco-email-gateway-zero-day-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: Cisco Secure Email GatewayにおけるSQLインジェクションの脆弱性（CVE-2026-76461）に関する注意喚起  (公開](https://www.jpcert.or.jp/at/2026/at260027.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Email Gateway Flaw Exploited in the Wild, Enables Root Command Exec](https://thehackernews.com/2026/09/cisco-secure-email-gateway-flaw.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Root RCE Zero-Day in Cisco Secure Email Gateway Under Active Exploitation](https://www.securityweek.com/root-rce-zero-day-in-cisco-secure-email-gateway-under-active-exploitation/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（1件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-31499"></a>

### 2. Microsoft 2026年9月 Patch Tuesday 関連まとめ

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>A⁠I</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 57.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 60.0 |
| <nobr>確⁠度</nobr> | 57.0 |

#### 概要

Microsoftの2026年9月のPatch Tuesdayでは、合計973件という過去最多規模の脆弱性修正が公開され、うち113件がCriticalに分類されました。
公開時点で公表済みのゼロデイはない一方、実際に悪用されたとされる脆弱性が2件含まれており、Windowsの権限昇格や一部製品の重大なRCE修正が注目されています。
件数が非常に多く、対象製品も広いため、単一の重大脆弱性だけでなく全体の適用計画が重要になります。特に実悪用が示されている修正は、優先度を上げて確認すべき対象です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 11 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 実悪用が示された修正を最優先で適用し、影響を受ける製品とバージョンを早急に洗い出す。
- Windowsの権限昇格系と、RCEが修正されたサーバー系製品を重点的に確認する。
- 件数が多いため、通常の月次運用ではなく資産棚卸しと段階的な適用計画を前提に進める。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft Patch Tuesday inadvertently takes down copy and paste in Excel – and t](https://www.itpro.com/security/microsoft-patch-tuesday-inadvertently-takes-down-copy-and-paste-in-excel-and-theres-no-way-to-fix-it-yet) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Shatters Patch Tuesday Record With 974 CVE Fixes in September 2026](https://www.infosecurity-magazine.com/news/microsoft-patch-tuesday-record/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft breaks Patch Tuesday record with 974-CVE deluge](https://www.theregister.com/security/2026/09/09/microsoft-breaks-patch-tuesday-record-with-974-cve-deluge/5295160) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft posts nearly 1,000 bugs for Patch Tuesday as CISA warns two being expl](https://therecord.media/microsoft-patch-tuesday-september-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patch Tuesday for September 2026 — Snort rules and prominent vulnerabi](https://blog.talosintelligence.com/microsoft-patch-tuesday-for-september-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Patch Tuesday - September 2026](https://www.rapid7.com/blog/post/em-patch-tuesday-september-2026) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [多くの企業はランサムウェアから迅速に復旧できない](https://www.infosecurity-magazine.com/news/four-of-800-clients-hit-ransomware/) | 28.0 | 30.0 | 42.0 |
| [スイスの裁判所、52歳のウクライナ人ランサムウェア開発者に約13年の禁錮刑を言い渡す](https://www.theregister.com/security/2026/09/15/swiss-court-sentences-52-year-old-ukrainian-ransomware-dev-to-nearly-13-years-in-the-cooler/5296482) | 28.0 | 30.0 | 42.0 |
| [HBO Maxの認証済みRedditアカウントが乗っ取られマルウェア拡散に悪用される](https://www.malwarebytes.com/blog/news/2026/09/hbo-maxs-verified-reddit-account-hijacked-to-spread-malware) | 28.0 | 20.0 | 48.0 |
| [低品質なカジノサイトが極めて危険な脅威アクターを隠蔽している](https://www.theregister.com/security/2026/09/15/low-quality-casino-sites-conceal-highly-dangerous-threat-actors/5296652) | 28.0 | 20.0 | 42.0 |
| [KREMLIN Banking MalwareがChromeとEdgeを乗っ取り、認証情報とセッショントークンを窃取](https://thehackernews.com/2026/09/kremlin-banking-malware-hijacks-chrome.html) | 28.0 | 20.0 | 42.0 |
| [イランのスパイがWindows端末をChosen Brickデータ窃取マルウェアで攻撃](https://www.theregister.com/security/2026/09/15/iranian-spies-hit-windows-machines-with-chosen-brick-data-stealing-malware/5296646) | 28.0 | 20.0 | 42.0 |
| [VectraRATでWindows企業を月額250ドルで攻撃可能](https://www.darkreading.com/endpoint-security/vectrarat-hack-windows-enterprises) | 28.0 | 20.0 | 42.0 |
| [イランのハッカー、Telegramで制御するマルウェアを使い反体制派とジャーナリストを監視](https://thehackernews.com/2026/09/iranian-hackers-use-telegram-controlled.html) | 28.0 | 20.0 | 42.0 |
| [BambooTokenマルウェアがMQTTを悪用してWindowsとLinuxシステムを制御](https://thehackernews.com/2026/09/bambootoken-malware-uses-mqtt-to.html) | 28.0 | 20.0 | 42.0 |
| [BambooTokenマルウェアがMQTTを介してWindowsとLinuxシステムを制御](https://www.bleepingcomputer.com/news/security/bambootoken-malware-controls-windows-and-linux-systems-via-mqtt/) | 28.0 | 20.0 | 42.0 |
| [ハッカーがサードパーティ製WooCommerceプラグイン経由でWordPressサイトを標的にする](https://www.bleepingcomputer.com/news/security/hackers-target-wordpress-sites-via-third-party-woocommerce-plugin/) | 28.0 | 20.0 | 42.0 |
| [eBook: Identity-First脅威インテリジェンス](https://www.helpnetsecurity.com/2026/09/15/enzoic-ebook-identity-first-threat-intelligence/) | 28.0 | 20.0 | 42.0 |
| [Google DocのサイドバーがMacとWindowsユーザーを異なるマルウェア経路へ誘導](https://www.huntress.com/blog/google-doc-sidebar-malware-mac-windows) | 28.0 | 20.0 | 42.0 |
| [英国と同盟国がイラン国家関係者による反体制派・活動家・ジャーナリスト標的のスパイウェアを暴露](https://www.ncsc.gov.uk/news/uk-allies-expose-spyware-iranian-state-actors-target-dissidents-activists-journalists) | 28.0 | 20.0 | 42.0 |
| [公開された開発サーバーからクラウド認証情報を抽出するためにViteの脆弱性を悪用する大規模スキャン活動](https://thehackernews.com/2026/09/mass-scanning-campaign-exploits-vite.html) | 28.0 | 20.0 | 42.0 |
| [攻撃者がHBO MaxのRedditアカウントを乗っ取り、48時間にわたりマルバタイジングを実施](https://www.helpnetsecurity.com/2026/09/15/hbo-max-reddit-account-clickfix-infostealer-malware/) | 28.0 | 20.0 | 42.0 |
| [HBO MaxのRedditアカウントが乗っ取られClickFix攻撃でマルウェア配布に悪用された件](https://www.securityweek.com/hacked-hbo-reddit-account-used-for-malware-delivery-via-clickfix-attack/) | 28.0 | 20.0 | 42.0 |
| [Black Hat USA 2026｜OpenAIとHugging Faceに関する「Breaking」ニュース](https://www.darkreading.com/vulnerabilities-threats/bhusa26huggingfacetalk) | 27.0 | 20.0 | 43.0 |
| [ポスト・ミトス時代におけるゼロデイ対応のあるべき姿](https://www.bleepingcomputer.com/news/security/what-zero-day-response-should-be-in-the-post-mythos-era/) | 27.0 | 20.0 | 43.0 |
| [会社を丸ごとAIに経営させるAIエージェント「Pion」が登場、メール・電話・銀行機能まで使って事業を自律運営](https://gigazine.net/news/20260915-pion/) | 27.0 | 20.0 | 42.0 |
| [シャープがAIサーバー受注開始、2030年度に2500億円目指す オンプレ用途で](https://xtech.nikkei.com/atcl/nxt/column/18/00001/12035/) | 26.0 | 20.0 | 42.0 |
| [Exein、Physical AIセキュリティで2億7000万ドルを調達し評価額17億ドルに到達](https://www.securityweek.com/exein-secures-270m-at-1-7b-valuation-for-physical-ai-security/) | 25.0 | 20.0 | 42.0 |
| [AIチャットボットの学習対象から除外する方法](https://www.malwarebytes.com/blog/how-to/2026/09/how-to-opt-out-of-ai-chatbot-training) | 25.0 | 20.0 | 42.0 |
| [AIが新たなサイバーセキュリティ投資を牽引する主要要因に](https://www.cybersecuritydive.com/news/ai-leading-driver-cybersecurity-spending/830418/) | 25.0 | 20.0 | 42.0 |
| [企業のAIは誰が管理するのか：エンタープライズ向けエージェントとモデルのための信頼フレームワーク](https://www.theregister.com/security/2026/09/15/sponsored-whos-governing-your-ai-a-trust-framework-for-enterprise-agents-and-models/5294237) | 25.0 | 20.0 | 42.0 |
| [企業のAI戦略はエージェント型ツールを考慮していない](https://www.cybersecuritydive.com/news/ai-governance-agents-ey/830282/) | 25.0 | 20.0 | 42.0 |
| [UltraViolet Cyber EquinoxによるMITREフレームワークに対する検知カバレッジの評価](https://www.helpnetsecurity.com/2026/09/15/ultraviolet-cyber-equinox/) | 25.0 | 20.0 | 42.0 |
| [Globalgigが企業向けAI保護のためマネージドセキュリティポートフォリオを拡充](https://www.helpnetsecurity.com/2026/09/15/globalgig-expands-managed-security-with-ai-protection/) | 25.0 | 20.0 | 42.0 |
| [サイバー予算が横ばいの中で新規支出の最優先となるAI](https://www.infosecurity-magazine.com/news/ai-top-priority-new-spend-cyber/) | 25.0 | 20.0 | 42.0 |
| [検索で見つけやすくしつつAI学習は許可しない方法](https://blog.cloudflare.com/accountable-mixed-use-ai-crawlers/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、AIエージェントがRubyGems攻撃に関与したとする報告を調査](https://www.securityweek.com/openai-investigates-report-linking-ai-agents-to-rubygems-attack/) | 25.0 | 20.0 | 42.0 |
| [Manhattan DA、12のAIディープフェイクポルノサイトを摘発](https://therecord.media/manhattan-da-takes-down-12-ai-deepfake-porn-sites) | 25.0 | 20.0 | 42.0 |
| [ハッキングフォーラムでChatGPTやClaudeの脱獄代替として販売される検閲なしAI](https://www.helpnetsecurity.com/2026/09/15/luciferus-uncensored-ai-service-hacking-forum/) | 25.0 | 20.0 | 42.0 |
| [Gartner：AIが今後3年間でビジネスをどう変革するか](https://www.itpro.com/technology/gartner-heres-how-ai-will-remake-business-in-the-next-three-years) | 25.0 | 20.0 | 42.0 |
| [Schneider Electric SCADAPack x70製品に関する脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-258-04) | 25.0 | 20.0 | 42.0 |
| [Microsoft、AIモデル向けにセキュリティと安全性のルールを設定](https://www.helpnetsecurity.com/2026/09/15/microsoft-ai-safety-rules-humanist-ai-code-of-conduct/) | 25.0 | 20.0 | 42.0 |
| [Meta AIが家族の投稿をもとに子どもの詳細なプロファイルを構築](https://www.malwarebytes.com/blog/family-and-parenting/2026/09/meta-ai-builds-detailed-profiles-of-children-from-years-of-family-posts) | 25.0 | 20.0 | 42.0 |
| [MicrosoftのAI行動規範が定めるサイバー攻撃の境界、指揮系統、安全制約](https://www.securityweek.com/microsoft-ai-code-of-conduct-sets-cyberattack-boundaries-chain-of-command-safety-constraints/) | 25.0 | 20.0 | 42.0 |
| [AkuityがAIエージェントに運用コンテキストを与え、安全にソフトウェアをリリース可能にする](https://www.helpnetsecurity.com/2026/09/15/akuity-agentic-control-plane/) | 25.0 | 20.0 | 42.0 |
| [Traefik Labs、AIエージェントのガバナンスに独立検証を導入](https://www.helpnetsecurity.com/2026/09/15/traefik-labs-sovereign-trust-plane/) | 25.0 | 20.0 | 42.0 |
| [Siemens MendixのSAMLに関する脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-258-06) | 24.0 | 46.0 | 50.0 |
| [Digital Watchdog VMAX DVRおよびNVR製品群](https://www.cisa.gov/news-events/ics-advisories/icsa-26-258-01) | 24.0 | 46.0 | 50.0 |
| [Siemens Teamcenterのセキュリティ情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-258-07) | 24.0 | 46.0 | 50.0 |
| [Siemens Reyrolle 7SR5の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-258-05) | 24.0 | 46.0 | 50.0 |
| [CareCam CM2507の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-258-08) | 24.0 | 46.0 | 50.0 |
| [mySCADA myPRO Managerの脆弱性問題](https://www.cisa.gov/news-events/ics-advisories/icsa-26-258-03) | 24.0 | 46.0 | 50.0 |
| [Fortinetの脆弱性を悪用したタイのブロードバンド事業者への侵害](https://www.securityweek.com/thai-broadband-provider-hacked-via-fortinet-vulnerability/) | 22.0 | 32.0 | 42.0 |
| [Apple、新しいiOS 27とmacOS Golden Gate 27で200件の脆弱性を修正](https://www.securityweek.com/apple-patches-200-vulnerabilities-with-new-ios-27-macos-golden-gate-27-releases/) | 22.0 | 32.0 | 42.0 |
| [研修会申込者の個人情報が閲覧可能に、フォーム設定ミス - 静岡県](https://www.security-next.com/190136) | 22.0 | 20.0 | 42.0 |
| [予約サイトなどで侵害、影響など調査中 - 審美歯科チェーン](https://www.security-next.com/189665) | 22.0 | 20.0 | 42.0 |
| [サイト公開した表計算ファイル、非公開シートに過去の名簿 - 大川市](https://www.security-next.com/190201) | 22.0 | 20.0 | 42.0 |
| [円谷プロの購入抽選に不正アクセス - 「当選」が「落選」に](https://www.security-next.com/190315) | 22.0 | 20.0 | 42.0 |
| [サイト改ざん被害、CMS脆弱性で - 東京都管工事工業協同組合](https://www.security-next.com/189799) | 22.0 | 20.0 | 42.0 |
| [Wärtsilä FOS-Onboardの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-258-02) | 20.0 | 28.0 | 50.0 |
| [CenterPoint Energyがサイバー攻撃で顧客データ流出を確認](https://www.bleepingcomputer.com/news/security/centerpoint-energy-confirms-customer-data-stolen-in-cyberattack/) | 20.0 | 20.0 | 42.0 |
| [イランのサイバー諜報員が偽のMRIスキャン結果を使って「体制の敵」をハッキング](https://therecord.media/iran-cyber-spies-use-fake-mri-scans-as-lure) | 20.0 | 20.0 | 42.0 |
| [100万ドルのサンドボックスチャレンジがLinux Kernelの脆弱性を発見](https://www.securityweek.com/1-million-sandbox-challenge-uncovers-linux-kernel-flaws/) | 20.0 | 20.0 | 42.0 |
| [CenterPoint Energy、情報漏えいを確認　ハッカーがデータを流出](https://www.securityweek.com/texas-utility-centerpoint-energy-confirms-breach-after-hacker-leaks-data/) | 20.0 | 20.0 | 42.0 |
| [不正採用の多くは発覚前に認証情報を受け取る](https://www.infosecurity-magazine.com/news/fraudulent-hires-credentials/) | 20.0 | 20.0 | 42.0 |
| [Zelensky大統領、元警察長官をウクライナのサイバー調整センター責任者に任命](https://therecord.media/ukraine-cyber-coordination-center-ihor-klymenko) | 20.0 | 20.0 | 42.0 |
| [CenterPoint Energy、ダークウェブ投稿後にデータ侵害を警告](https://therecord.media/centerpoint-energy-data-breach) | 20.0 | 20.0 | 42.0 |
| [人員削減時におけるITセキュリティリスクと運用レジリエンス](https://www.huntress.com/blog/operational-resilience-reduced-staffing-risks) | 20.0 | 20.0 | 42.0 |
| [Black Axeメンバー、インターネット詐欺容疑で米国に送致](https://www.infosecurity-magazine.com/news/black-axe-members-extradited-us/) | 20.0 | 20.0 | 42.0 |
| [Postman Passportで認証情報を公開せずにAPIアクセスを制御する方法](https://www.helpnetsecurity.com/2026/09/15/postman-passport/) | 20.0 | 20.0 | 42.0 |
| [チームメンバーとエージェントに適切な権限レベルでWorkersへのアクセスを付与する方法](https://blog.cloudflare.com/workers-granular-authorization/) | 20.0 | 20.0 | 42.0 |
| [Wiz DefendとGoogle Security Operationsによる共同投資と防御の取り組み](https://www.wiz.io/blog/wiz-defend-and-google-security-operations) | 20.0 | 20.0 | 42.0 |
| [サイバー脅威の3分の2は依然として手動対応が必要](https://www.itpro.com/security/two-thirds-of-cyber-threats-still-require-manual-resolution) | 20.0 | 20.0 | 42.0 |
| [CISAとNIST、連邦政府のクラウドIDシステムをトークン窃取・偽造・悪用から守るためのガイドラインを公開](https://www.cisa.gov/news-events/news/cisa-and-nist-release-guidelines-protect-federal-cloud-identity-systems-token-theft-forgery-and) | 20.0 | 20.0 | 42.0 |
| [Akamai、2026年Gartner Peer Insights™ Report for SEBでStrong Performerに選出](https://www.akamai.com/blog/security/2026/sep/akamai-strong-performer-gartner-peer-insights-report-seb) | 20.0 | 20.0 | 42.0 |
| [トークンとアサーションの偽造・窃取・悪用からの保護：政府機関とクラウドサービス提供者向け実装推奨事項](https://www.cisa.gov/resources-tools/resources/protecting-tokens-and-assertions-forgery-theft-and-misuse-implementation-recommendations-agencies) | 20.0 | 20.0 | 42.0 |
| [日本のデジタル庁で24万人が被害を受けたデータ漏えい](https://www.securityweek.com/240000-hit-by-data-breach-at-japans-digital-agency/) | 20.0 | 20.0 | 42.0 |
| [攻撃面だけでなく攻撃チェーンも考慮すべき理由――個別技術のテストでは本質を見落とす](https://thehackernews.com/2026/09/attack-chains-not-just-attack-surfaces.html) | 20.0 | 20.0 | 42.0 |
| [米国で疑われるBlack Axeギャングの首謀者ら、サイバー犯罪で起訴](https://www.bleepingcomputer.com/news/security/black-axe-gang-members-extradited-to-us-face-cybercrime-charges/) | 20.0 | 20.0 | 42.0 |
| [元AT&T店舗従業員、SIMスワップ詐欺集団の内通者として兼業し収監される](https://www.bitdefender.com/en-us/blog/hotforsecurity/former-at-t-worker-jailed-sim-swap) | 20.0 | 20.0 | 42.0 |
| [SOCとMSSPのための2026年上半期サイバーリスクレポート：6か月間の警戒状況](https://any.run/cybersecurity-blog/h1-2026-cyber-risk-report/) | 20.0 | 20.0 | 42.0 |
| [Search結果から偽のBitrefill決済ページへ誘導される問題](https://www.malwarebytes.com/blog/threat-intel/2026/09/search-results-are-sending-people-to-fake-bitrefill-checkouts) | 20.0 | 20.0 | 42.0 |
| [Microsoft、KB5002914のExcel更新でコピー＆ペースト不具合を確認](https://www.bleepingcomputer.com/news/microsoft/microsoft-september-kb5002914-security-update-breaks-excel-copy-and-paste/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、RDSの脆弱性を修正する緊急パッチを公開](https://www.infosecurity-magazine.com/news/microsoft-releases-emergency-patch/) | 20.0 | 20.0 | 42.0 |

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
