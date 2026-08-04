# 📡 サイレーダー 2026-08-05 05:00 JST

このレポートは、2026-08-04 17:00 JST〜2026-08-05 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 124
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 94

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Prolific ransomware group behind SonicWall zero-day attacks](#topic-22364) | 60.0 | 84.0 | 67.0 | 音声 | 温度感上位枠 |
| 2 | [CVE-2026-18577: CISA KEV catalog addition](#topic-25667) | 55.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [CISA Adds Three Known Exploited Vulnerabilities to Catalog](#topic-25954) | 49.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [“Keep going, bro. You’ve got this!” A data-driven look at how adversaries are weaponizing AI](#topic-25980) | 35.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [AI developers targeted via trojanized GitHub repositories](#topic-25914) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [AI makes costly spearphishing attacks easier, cyber insurer says](#topic-25953) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-22364"></a>

### 1. Prolific ransomware group behind SonicWall zero-day attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 60.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 84.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

SonicWallのSecure Mobile Access（SMA）1000シリーズで、CVE-2026-15409を含む2件の脆弱性が実際の攻撃に悪用されていたとされています。
報道では、脅威アクターがこれらを組み合わせてカスタムマルウェアの展開や長期的な侵入に利用した可能性が示されています。
リモートアクセス機器は社内ネットワークへの入口になりやすく、侵害されると認証情報の窃取や横展開につながるおそれがあります。
さらに、公開PoCや悪用情報がある場合は、未修正環境のリスクが高まります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
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

#### 担当者向け確認ポイント

- SMA 1000シリーズの適用状況を確認し、SonicWallの修正版への更新可否を早急に点検する。
- ベンダーが示す侵害痕跡の有無を確認し、該当する場合は認証情報の変更やTOTPトークンの再設定を含めて対応する。
- 外部公開されるVPN/リモートアクセス機器は、ログ監視と資産棚卸しを強化し、想定外の管理操作や不審な挙動を継続監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-15409 | 関連CVE | 1.00 | 候補あり（URL 5件以上） |
| 脆弱性 | CVE-2026-15410 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | SonicWall | 言及あり | 0.80 | — |
| 製品 | SonicWall SMA | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-15409](https://nvd.nist.gov/vuln/detail/CVE-2026-15409) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Prolific ransomware group behind SonicWall zero-day attacks](https://cyberscoop.com/inc-ransomware-sonicwall-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall SMA zero-days were exploited weeks before disclosure](https://www.helpnetsecurity.com/2026/07/21/sonicwall-sma-zero-days-exploited-cve-2026-15409-cve-2026-15410/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall Zero-Days Exploited to Deliver Custom Malware for Weeks Before Patch](https://www.securityweek.com/sonicwall-zero-days-exploited-to-deliver-custom-malware-for-weeks-before-patch/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Rapid7 MDR Team Discovers New SonicWall SMA1000 Zero Days being Actively Exploit](https://www.rapid7.com/blog/post/etr-rapid7-mdr-team-discovers-new-sonicwall-sma1000-zero-days-being-actively-exploited-cve-2026-15409-cve-2026-15410) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Two SonicWall SMA 1000 Zero-Days Exploited, One Could Enable Admin Commands](https://thehackernews.com/2026/07/two-sonicwall-sma-1000-zero-days.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall Issues Urgent SMA Patch Warning for Two Zero-Day Exploits](https://www.securityweek.com/sonicwall-issues-urgent-sma-patch-warning-for-two-zero-day-exploits/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall warns of SMA1000 flaws exploited in zero-day attacks, patch now](https://www.bleepingcomputer.com/news/security/sonicwall-warns-of-sma1000-flaws-exploited-in-zero-day-attacks-patch-now/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-25667"></a>

### 2. CVE-2026-18577: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 55.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

CVE-2026-18577は、N-able N-centralに影響する認証回避の脆弱性で、公開情報では実環境で悪用が観測されているとされています。
対象はホスト型とオンプレミス型の両方のN-centralサーバーとされ、CISAのKEVカタログにも追加されています。
RMM製品は管理対象の端末や運用権限に直結するため、侵害されると影響範囲が広がりやすい点が注目されています。
認証回避が悪用可能とみられることで、通常の公開脆弱性よりも優先度を高く見て対応する必要があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
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

- N-ableの案内に従い、N-centralの該当バージョンと適用済み修正状況を確認する。
- 外部公開している管理画面や関連サービスのアクセス制御、認証ログ、異常な管理者操作の有無を点検する。
- 運用中のRMM基盤として、同種の管理製品も含めて脆弱性管理と監視優先度を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-18577 | 主題CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-18577](https://nvd.nist.gov/vuln/detail/CVE-2026-18577) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-18577: N-able N-central Authentication Bypass Exploited in the Wild](https://www.rapid7.com/blog/post/etr-cve-2026-18577-n-able-n-central-authentication-bypass-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit N-able Patch Bypass Flaw on RMM Servers](https://www.darkreading.com/vulnerabilities-threats/attackers-exploit-n-able-patch-bypass-flaw) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [N-able warns of N-central auth bypass flaw exploited in attacks](https://www.bleepingcomputer.com/news/security/n-able-warns-of-n-central-auth-bypass-flaw-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers exploit N-able N-central flaw to reach managed endpoints (CVE-2026-185](https://www.helpnetsecurity.com/2026/08/03/cve-2026-18577-n-able-n-central-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [N‑able Patches Vulnerability Exploited to Hack N-central Servers](https://www.securityweek.com/n-able-patches-vulnerability-exploited-to-hack-n-central-servers/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Feds get 3 days to patch N-able God mode flaw under active exploit](https://www.theregister.com/security/2026/08/04/feds-get-3-days-to-patch-n-able-god-mode-flaw-under-active-exploit/5282894) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-25954"></a>

### 3. CISA Adds Three Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 49.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、実際の悪用が確認されたとして、Known Exploited Vulnerabilities（KEV）カタログに3件の脆弱性を追加しました。
対象は IBM Langflow、N-able N-central、Apache Tomcat に関連するもので、いずれも優先的な対応が必要とされています。
KEVカタログ入りは、当該脆弱性が現実の攻撃で使われていることを示すため、対応の優先順位を上げる判断材料になります。
公開資産や広く使われる製品に影響する場合、被害の波及が大きくなりやすい点も重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 自組織で該当製品の利用有無を確認し、影響範囲をすぐに洗い出す。
- KEV対象として、通常の定期対応よりも前倒しで修正・緩和策を適用する。
- 公開状態の資産や認証まわりを点検し、未対応のまま露出していないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | Apache Tomcat | 言及あり | 0.80 | — |
| 製品 | Langflow | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Three Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/08/04/cisa-adds-three-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-25980"></a>

### 4. “Keep going, bro. You’ve got this!” A data-driven look at how adversaries are weaponizing AI

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Cisco Talosは、脅威アクターの端末から取得したプロンプトログをもとに、ClaudeやGeminiなどのクラウド型AIが攻撃者にどう利用されているかを分析したとしています。
公開情報上では、特定の脆弱性や単一製品の問題というより、AIが攻撃活動の中で使われる実態を整理した内容です。
生成AIやクラウドAIが、正規の業務支援だけでなく攻撃者側の作業にも使われ得ることを示す事例として注目されます。
防御側は、AI利用そのものではなく、周辺の不審な操作やアカウント悪用の兆候も含めて見る必要があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI支援ツールの利用ログやアクセス元の異常、短時間の大量問い合わせなど、通常と異なる挙動を確認する。
- 端末・アカウントの侵害前提で、権限の過不足や多要素認証、セッション管理を見直す。
- AI利用を含む業務フローで、機密情報の投入や外部連携の制御、監査ログの保全を徹底する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Qwen | 言及あり | 0.80 | — |
| ベンダー | GitLab | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| 製品 | WordPress | 言及あり | 0.80 | — |
| 製品 | Exchange | 言及あり | 0.80 | — |
| 製品 | Cursor | 言及あり | 0.80 | — |
| 製品 | Microsoft Azure | 言及あり | 0.80 | — |
| 製品 | Gitea | 言及あり | 0.80 | — |
| 攻撃/検証ツール | Ngrok | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [“Keep going, bro. You’ve got this!” A data-driven look at how adversaries are we](https://blog.talosintelligence.com/keep-going-bro-youve-got-this-a-data-driven-look-at-how-adversaries-are-weaponizing-ai/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-25914"></a>

### 5. AI developers targeted via trojanized GitHub repositories

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Netskope Threat Labsによると、攻撃者が人気のAIツールや開発者向けリソースのGitHubリポジトリを模倣し、情報窃取型マルウェアの配布に悪用しているとみられます。
対象はAI開発者やその周辺の利用者で、正規のリポジトリに見せかけた誘導が使われている点が特徴です。
開発者は信頼しやすい公開リポジトリ経由で感染や情報流出に巻き込まれるおそれがあり、サプライチェーン的なリスクとして注意が必要です。
AI関連ツールの利用が広がるほど、こうした模倣・改ざんの影響範囲も大きくなり得ます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- GitHub上のリポジトリは、名称や説明だけでなく所有者情報、更新履歴、配布ファイルの整合性も確認する。
- AI開発環境では、外部リポジトリ由来のスクリプトや実行ファイルを安易に信頼しない運用を徹底する。
- 利用者向けに、正規配布元の確認と不審な認証画面・ダウンロード誘導への注意喚起を行う。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [AI developers targeted via trojanized GitHub repositories](https://www.helpnetsecurity.com/2026/08/04/developers-github-fake-ai-tools-infostealer/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-25953"></a>

### 6. AI makes costly spearphishing attacks easier, cyber insurer says

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

サイバー保険会社Resilienceによると、同社が上半期に扱った損失の85％超は、なりすましを含むインパーソネーション型のキャンペーンに起因していたとされています。
記事は、AIの活用で標的型フィッシングの作成や実行が容易になり、こうした攻撃の被害が増えうる点を示しています。
標的型フィッシングは、技術的な防御だけでなく人的な判断も突くため、被害が高額化しやすいのが特徴です。
AIにより攻撃の質や量が上がると、なりすまし対策や本人確認の重要性がさらに増します。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 送信元確認や送金・依頼承認の手続きを再点検し、重要操作には追加確認を必須化する。
- なりすましを前提に、メール・チャット・音声をまたぐ本人確認手順を整備する。
- フィッシング訓練や不審連絡の通報フローを見直し、初動対応を早める。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [AI makes costly spearphishing attacks easier, cyber insurer says](https://www.cybersecuritydive.com/news/ai-spearphishing-cyber-insurance-claims/826732/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

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
| [N-ableがN-centralの「god mode」脆弱性に対する修正パッチを公開、MSPに即時適用を要請](https://www.itpro.com/security/cyber-attacks/msps-urged-to-patch-immediately-after-n-able-issues-hotfix-for-n-central-god-mode-flaw) | 32.0 | 38.0 | 42.0 |
| [診断ツールの脆弱性を狙うボットネットの探索活動](https://isc.sans.edu/diary/rss/33214) | 30.0 | 20.0 | 42.0 |
| [npmのサプライチェーン攻撃「ChainDrop」が数百のパッケージに感染](https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/) | 28.0 | 40.0 | 42.0 |
| [改変されたXcodeプロジェクトを通じてmacOS開発者を標的にする新たなXCSSET亜種](https://www.bleepingcomputer.com/news/security/new-xcsset-variant-targets-macos-devs-via-compromised-xcode-projects/) | 28.0 | 20.0 | 42.0 |
| [Smoke#Screen RMM乗っ取りの試みが脅威アクターの手口を暴露](https://www.darkreading.com/cyberattacks-data-breaches/latest-rmm-fueled-phishing-attack-exposes-threat-actor-playbook) | 28.0 | 20.0 | 42.0 |
| [偽のAdobeおよびZoom更新でScreenConnectをインストールし、永続的なリモートアクセスを確立](https://thehackernews.com/2026/08/fake-adobe-and-zoom-updates-install.html) | 28.0 | 20.0 | 42.0 |
| [RapidFort Runtimeが継続的なCVE監視と改ざん検知を提供](https://www.helpnetsecurity.com/2026/08/04/rapidfort-runtime/) | 28.0 | 20.0 | 42.0 |
| [マルウェアサンプルのほぼ半数がIPに直接通信](https://unit42.paloaltonetworks.com/malware-bypass-dns-direct-to-ip/) | 28.0 | 20.0 | 42.0 |
| [ホテルのWi-Fiネットワークにログインする旅行者を標的とした攻撃](https://www.malwarebytes.com/blog/news/2026/08/travelers-targeted-when-logging-into-hotel-wi-fi-networks) | 28.0 | 20.0 | 42.0 |
| [OMB M-26-14準拠：連邦CISO向け適応型エッジログ管理](https://www.akamai.com/blog/security/2026/aug/omb-m-26-14-compliance-adaptive-edge-logging-federal-cisos) | 28.0 | 20.0 | 42.0 |
| [CloudとSaaS環境が攻撃者の主要標的に、今やトップに](https://www.infosecurity-magazine.com/news/cloud-saas-targets-attackers/) | 28.0 | 20.0 | 42.0 |
| [ロシアのハッカーがホテルのWi-Fiネットワークを悪用し、Microsoft 365の認証情報を窃取してマルウェアを展開](https://www.helpnetsecurity.com/2026/08/04/midnight-blizzard-hotel-wi-fi-networks-hacking/) | 28.0 | 20.0 | 42.0 |
| [DOUBLECUPがClickFixとキャッシュされたPNGを用いてCountLoaderとDeviceManager RATを配信](https://thehackernews.com/2026/08/doublecup-uses-clickfix-and-cached-pngs.html) | 28.0 | 20.0 | 42.0 |
| [Frontier AI脆弱性バースト：オープンソースソフトウェアにおける自律的ゼロデイ発見の工業化](https://unit42.paloaltonetworks.com/frontier-ai-vulnerability-burst/) | 27.0 | 20.0 | 43.0 |
| [「中国軍がDeepSeek製AIを無人航空機に活用」「時速50kmの軍用車両にも搭載」 きょう公開の防衛白書](https://www.itmedia.co.jp/news/article/2608/04/2000000382/) | 26.0 | 20.0 | 42.0 |
| [AI普及でデザイン業の倒産が前年比2.7倍に 「独自性なき企業は淘汰」 東京商工リサーチ](https://www.itmedia.co.jp/news/article/2608/04/2000000377/) | 26.0 | 20.0 | 42.0 |
| [Keyv関連のnpmワームが数百件のパッケージを汚染し、Claude CodeとVS Codeのフックを設置](https://thehackernews.com/2026/08/keyv-linked-npm-worm-poisons-hundreds.html) | 25.0 | 45.0 | 42.0 |
| [民主党上院議員ら、AIセキュリティリスクに関するTrump政権の意思決定を批判](https://cyberscoop.com/trump-ai-policy-chinese-models-risk/) | 25.0 | 20.0 | 42.0 |
| [AIガードレールの回避はスクリプトキディでも容易である](https://www.theregister.com/security/2026/08/04/bypassing-ai-guardrails-is-so-easy-a-script-kiddie-can-do-it/5282973) | 25.0 | 20.0 | 42.0 |
| [Rethinking AI Security: CASBとDLPに必要な相互作用を考慮したレイヤー](https://www.securityweek.com/rethinking-ai-security-why-casb-and-dlp-need-an-interaction-aware-layer/) | 25.0 | 20.0 | 42.0 |
| [Salt、AIエージェントとAPI保護向けのAWS WAFマネージドルールセットを初公開](https://securityboulevard.com/2026/08/salt-debuts-first-aws-waf-managed-ruleset-for-ai-agent-and-api-protection/) | 25.0 | 20.0 | 42.0 |
| [AIがMicrosoftのバグハンターたちの過去最高2000万ドル報奨金獲得を後押し](https://www.theregister.com/security/2026/08/04/ai-helps-microsoft-bug-hunters-chase-a-record-20m-payday/5282821) | 25.0 | 20.0 | 42.0 |
| [Tech業界連合がAIエージェントの安全性報告プログラムを提案](https://www.cybersecuritydive.com/news/ai-agent-security-exchange-linux-foundation/826940/) | 25.0 | 20.0 | 42.0 |
| [n8nにおけるAgentic AIワークフローの保護：漏えいしたAPIキーから暗号鍵の侵害まで](https://securityboulevard.com/2026/08/securing-agentic-ai-workflows-in-n8n-from-leaked-api-keys-to-encryption-key-compromise/) | 25.0 | 20.0 | 42.0 |
| [Varonis Agent IBACでAIエージェントを意図した境界内に維持する](https://www.bleepingcomputer.com/news/security/varonis-agent-ibac-keeps-ai-agents-within-their-intended-boundaries/) | 25.0 | 20.0 | 42.0 |
| [武器化されたメールAIアシスタントが攻撃者によるアカウント乗っ取りを助ける可能性](https://www.securityweek.com/weaponized-email-ai-assistants-could-help-attackers-hijack-accounts/) | 25.0 | 20.0 | 42.0 |
| [Sevii APS Moduleが自律的なサイバー防御で攻撃を阻止](https://www.helpnetsecurity.com/2026/08/04/sevii-autonomous-preemptive-security-aps-module/) | 25.0 | 20.0 | 42.0 |
| [Zenity、シリーズCで1億2500万ドルを調達](https://www.securityweek.com/zenity-raises-125-million-in-series-c-funding/) | 25.0 | 20.0 | 42.0 |
| [ServiceNowが6つのソリューション領域で自律型セキュリティを体系化](https://www.helpnetsecurity.com/2026/08/04/servicenow-ai-specialists/) | 25.0 | 20.0 | 42.0 |
| [サイバー犯罪者が複数セッションにまたがって悪意あるタスクを分割しAI安全制御を回避](https://www.infosecurity-magazine.com/news/talos-attackers-split-tasks-evade/) | 25.0 | 20.0 | 42.0 |
| [プライバシー、AI、子どもの安全に関する法案パッケージを上院が審議へ](https://cyberscoop.com/senate-kids-online-safety-act-ai-bills-markup/) | 25.0 | 20.0 | 42.0 |
| [Snyk、継続的なAIペネトレーションテストとエージェントのレッドチーミングを発表](https://www.helpnetsecurity.com/2026/08/04/snyk-evo-continuous-offensive-security-cos/) | 25.0 | 20.0 | 42.0 |
| [Black Hat 2026でのWiz：AI脅威への備えを推進](https://www.wiz.io/blog/wiz-at-black-hat-2026) | 25.0 | 20.0 | 42.0 |
| [AIガバナンス：OpenAIのAIインシデント解説](https://securityboulevard.com/2026/08/ai-governance-the-openai-ai-incident-explained/) | 25.0 | 20.0 | 42.0 |
| [AIノートテイカーを悪用し、政府・企業のビデオ通話を盗聴する攻撃者](https://www.darkreading.com/application-security/ai-notetaker-spy-government-corporate-video-calls) | 25.0 | 20.0 | 42.0 |
| [AIが重要な脆弱性の悪用やサプライチェーンの混乱に広く利用される](https://www.cybersecuritydive.com/news/ai-exploit-critical-flaws-disrupt-supply-chains/826915/) | 25.0 | 20.0 | 42.0 |
| [Obsidian Securityが1億1,000万ドル評価で8,500万ドルを調達](https://www.securityweek.com/obsidian-security-raises-85-million-at-1-1-billion-valuation/) | 25.0 | 20.0 | 42.0 |
| [Google EarthのAIツール、公開1日で撤回へ](https://www.malwarebytes.com/blog/news/2026/08/online-backlash-ends-in-google-rolling-back-google-earth-ai-tool-after-a-day) | 25.0 | 20.0 | 42.0 |
| [Vibe HackingがAIを「理想の新人ハッカー」に変えるとき](https://thehackernews.com/2026/08/when-vibe-hacking-turns-ai-into-junior.html) | 25.0 | 20.0 | 42.0 |
| [Google、悪意あるGitHub Issueで特権エージェントを引き起こす恐れを受けて3つのADK AIワークフローを削除](https://thehackernews.com/2026/08/google-deletes-3-adk-ai-workflows-after.html) | 25.0 | 20.0 | 42.0 |
| [「作業時間短縮のためにツールを買ったのに、以前より手作業が増えた」──ペンテスターがAIで修正しきれないほど多くの脆弱性を発見](https://www.itpro.com/security/i-bought-the-tool-to-save-time-but-i-did-more-manual-work-than-before-pentesters-are-finding-more-bugs-with-ai-than-they-can-fix-theyre-even-battling-fake-hallucinated-cves) | 25.0 | 20.0 | 42.0 |
| [Indusface SwyftComply AIがAI発見の脆弱性に対する自律的な仮想パッチ適用を実現](https://www.helpnetsecurity.com/2026/08/04/indusface-swyftcomply-ai/) | 25.0 | 20.0 | 42.0 |
| [ESETが自律エージェントのセキュリティ向け新たなAI機能を発表](https://www.helpnetsecurity.com/2026/08/04/eset-introduces-new-ai-capabilities-for-autonomous-agent-security/) | 25.0 | 20.0 | 42.0 |
| [アフリカのサイバー犯罪の半数以上をAIが占めるとInterpolが指摘](https://www.infosecurity-magazine.com/news/ai-accounts-over-half-cybercrime/) | 25.0 | 20.0 | 42.0 |
| [Joinable Labs、脅威インテリジェンスとAI駆動型対応のためのJoinable Securityを発表](https://www.helpnetsecurity.com/2026/08/04/joinable-labs-threat-map/) | 25.0 | 20.0 | 42.0 |
| [Securonix、Unified Defense SIEMを強化しAIエージェント検知とデータコスト削減を実現](https://www.helpnetsecurity.com/2026/08/04/securonix-governed-ai-agent-detection/) | 25.0 | 20.0 | 42.0 |
| [Legit Security VibeGuard 2.0、AIコーディングエージェントにエンドポイントセキュリティとリアルタイムガードレールを提供](https://www.helpnetsecurity.com/2026/08/04/legit-security-vibeguard-2-0/) | 25.0 | 20.0 | 42.0 |
| [Tanium、自律型セキュリティをAI、露出管理、SecOpsへ拡大](https://www.helpnetsecurity.com/2026/08/04/tanium-expands-autonomous-security-across-ai-exposure-management-and-secops/) | 25.0 | 20.0 | 42.0 |
| [keyvおよびCacheable名前空間の人気npmパッケージがサプライチェーン攻撃で侵害される](https://socket.dev/blog/popular-npm-packages-in-the-keyv-and-cacheable-namespaces-compromised-in-active-supply-chain) | 22.0 | 30.0 | 42.0 |
| [Microsoft、供給網セキュリティ強化のためNuGet APIキーの有効期間を短縮](https://www.helpnetsecurity.com/2026/08/04/microsoft-reducing-nuget-api-keys-lifetime/) | 22.0 | 20.0 | 43.0 |
| [「権限の低いエージェントをハックして上位権限でコードを実行する」というGoogle ADKのハッキング手法が発見される](https://gigazine.net/news/20260804-agent-development-kit-attack/) | 22.0 | 20.0 | 42.0 |
| [システム障害で原因調査、産廃回収は継続 - 環境開発工業](https://www.security-next.com/187809) | 22.0 | 20.0 | 42.0 |
| [委託先で水道検針データ消失、誤操作で - 宜野湾市](https://www.security-next.com/188198) | 22.0 | 20.0 | 42.0 |
| [Synology製NAS検出ツールのWindows版に脆弱性 - 修正版が公開](https://www.security-next.com/188315) | 22.0 | 20.0 | 42.0 |
| [中部電力に不正アクセス 連絡先情報7万1700件が漏えいか 取引先や自治体の連絡先も漏えいの恐れ](https://www.itmedia.co.jp/news/article/2608/04/2000000380/) | 21.0 | 20.0 | 42.0 |
| [EPARKリラク＆エステに不正アクセス、顧客情報3300万レコードが漏洩の恐れ](https://xtech.nikkei.com/atcl/nxt/news/24/03330/) | 21.0 | 20.0 | 42.0 |
| [福岡大学が実践するDNS多層防御--プロテクティブDNSで先制的サイバー対策](https://japan.zdnet.com/article/35251264/) | 21.0 | 20.0 | 42.0 |
| [開発者端末から秘密情報を収集するクレデンシャル収集の手口](https://securityboulevard.com/2026/08/credential-harvesting-explained-how-attackers-collect-secrets-from-developer-machines/) | 20.0 | 45.0 | 42.0 |
| [keyvとcacheableのnpmパッケージがサプライチェーン攻撃で乗っ取り被害に遭う](https://www.wiz.io/blog/keyv-and-cacheable-npm-supply-chain-attack) | 20.0 | 30.0 | 42.0 |
| [Thermo Fisher Applied Biosystems Genetic Analyzersの脆弱性](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-216-01) | 20.0 | 28.0 | 54.0 |
| [Acrisure KARR BTおよびDR-100の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-216-01) | 20.0 | 28.0 | 50.0 |
| [cPanelの重大な脆弱性によりホスティング顧客がデータベースroot権限でSQLを実行できる可能性](https://thehackernews.com/2026/08/new-cpanel-critical-flaw-could-let.html) | 20.0 | 28.0 | 50.0 |
| [2026年7月の主要サイバー攻撃：米国とEUの組織がフィッシング、RAT、Stealerの被害に遭う](https://any.run/cybersecurity-blog/major-cyber-attacks-july-2026/) | 20.0 | 20.0 | 48.0 |
| [77件のOpen VSX拡張機能で開発者情報の収集が確認される](https://www.bleepingcomputer.com/news/security/77-open-vsx-extensions-found-harvesting-developer-info/) | 20.0 | 20.0 | 42.0 |
| [Greatness PhaaS、デバイスコードフィッシングを追加してMFAを回避しトークンを窃取](https://thehackernews.com/2026/08/greatness-phaas-adds-device-code.html) | 20.0 | 20.0 | 42.0 |
| [Black Hat USA 2026 ベンダー発表の概要（第2部）](https://www.securityweek.com/black-hat-usa-2026-summary-of-vendor-announcements-part-2/) | 20.0 | 20.0 | 42.0 |
| [Hacker Summer Campで起きたある一件](https://www.theregister.com/security/2026/08/04/this-one-time-at-hacker-summer-camp/5282999) | 20.0 | 20.0 | 42.0 |
| [開発者が今も悪意あるパッケージをダウンロードしてしまう5つの理由](https://securityboulevard.com/2026/08/5-reasons-developers-still-download-malicious-packages/) | 20.0 | 20.0 | 42.0 |
| [Żabka、第三者アカウント経由で侵害される](https://therecord.media/poland-convenience-store-chain-zabka-cyberattack) | 20.0 | 20.0 | 42.0 |
| [Mini Shai-Huludがkeyvを標的に、改ざん版リリースでCIシークレットをGitHub経由で流出](https://securityboulevard.com/2026/08/mini-shai-hulud-hits-keyv-trojanized-release-exfiltrates-ci-secrets-via-github/) | 20.0 | 20.0 | 42.0 |
| [Black Hat USA 2026で見逃せない注目ポイント](https://www.security.com/expert-perspectives/things-you-wont-want-miss-black-hat-usa-2026) | 20.0 | 20.0 | 42.0 |
| [Mallory、脅威インテリジェンス・露出コンテキスト・対応を統合するセキュリティチーム向けアーキテクチャを発表](https://securityboulevard.com/2026/08/mallory-unifies-threat-intelligence-exposure-context-and-response-into-one-architecture-for-security-teams/) | 20.0 | 20.0 | 42.0 |
| [BSidesSF 2026: CloudShellのかくれんぼ――静寂の中で楽しむ甘美な永続性](https://securityboulevard.com/2026/08/bsidessf-2026-cloudshell-hide-n-seek-enjoying-the-sweet-persistent-sounds-of-silence/) | 20.0 | 20.0 | 42.0 |
| [Oligoがランタイムセキュリティ向けに6000万ドルを調達](https://www.securityweek.com/oligo-raises-60-million-for-runtime-security/) | 20.0 | 20.0 | 42.0 |
| [OPM侵害被害者向けID盗難対策サービス、失効迫る中で議員が延長を模索](https://cyberscoop.com/opm-breach-lifetime-identity-protection-bill/) | 20.0 | 20.0 | 42.0 |
| [CISO対談: Russ Kirby - 情熱は燃え尽き症候群への特効薬](https://www.securityweek.com/ciso-conversation-russ-kirby-passion-is-the-antidote-to-burnout/) | 20.0 | 20.0 | 42.0 |
| [WhatsAppのLinked Devices機能を悪用したアカウント乗っ取り詐欺](https://www.infosecurity-magazine.com/news/whatsapp-voting-scam-linked/) | 20.0 | 20.0 | 42.0 |
| [Durov関連製品を「テロリスト」指定後にロシア企業が削除](https://therecord.media/russian-businesses-erase-durov-linked-products-terrorist-designation) | 20.0 | 20.0 | 42.0 |
| [サイバーセキュリティデータをリスク指標に変換する方法](https://securityboulevard.com/2026/08/how-to-change-cybersecurity-data-into-risk-metrics-kovrr/) | 20.0 | 20.0 | 42.0 |
| [Swiss IT agencyへの侵害で200アカウントが漏えい、SharePointの脆弱性が疑われる](https://therecord.media/swiss-bit-foitt-hacked-possibly-sharepoint-vulnerabilities) | 20.0 | 20.0 | 42.0 |
| [Tennessee州の下院候補者、ナンバープレートカメラへの発砲容疑で告発される](https://www.theregister.com/security/2026/08/04/us-house-candidate-allegedly-shoots-down-four-flock-cameras/5282696) | 20.0 | 20.0 | 42.0 |
| [正規のクラウドプラットフォームを悪用してフィッシング攻撃者がMFAを回避する手口](https://securelist.com/cloud-platforms-in-phishing/120832/) | 20.0 | 20.0 | 42.0 |
| [TP-Link Omada ZTPの脆弱性連鎖によるネットワーク完全乗っ取り](https://www.securityweek.com/tp-link-omada-ztp-vulnerabilities-chain-into-full-network-takeover/) | 20.0 | 20.0 | 42.0 |
| [CAF Bank、オンラインサービスを再開もさらなる障害に警告](https://www.theregister.com/security/2026/08/04/caf-bank-reopens-online-service-but-warns-of-further-outages/5282668) | 20.0 | 20.0 | 42.0 |
| [Geminiのエージェント間攻撃手法により機密情報が漏えいし、プルリクエスト改ざんが可能に](https://www.securityweek.com/gemini-agent-to-agent-attack-exposed-secrets-enabled-pull-request-tampering/) | 20.0 | 20.0 | 42.0 |
| [企業が秘密を明かさずにサイバーリスクを共有する方法](https://cyberscoop.com/zero-knowledge-proofs-cyber-risk-sharing-op-ed/) | 20.0 | 20.0 | 42.0 |
| [数十年前から存在するBMCの脆弱性により、数千のデータセンターが攻撃にさらされる](https://www.securityweek.com/decades-old-bmc-vulnerability-exposes-thousands-of-data-centers-to-attacks/) | 20.0 | 20.0 | 42.0 |
| [Uptime Kuma 2.5.0、新しい npm パッケージを信頼するまで2週間待機するように変更](https://www.helpnetsecurity.com/2026/08/04/uptime-kuma-2-5-0-cooldown-npm-updates/) | 20.0 | 20.0 | 42.0 |
| [中部電力、社内システムへの不正アクセスでメールおよび連絡先情報が漏えいの可能性](https://internet.watch.impress.co.jp/docs/news/2130524.html) | 20.0 | 20.0 | 42.0 |
| [偽のIRS通知で仮想通貨保有者を狙う](https://www.bitdefender.com/en-us/blog/hotforsecurity/fake-irs-letters-cryptocurrency) | 20.0 | 20.0 | 42.0 |
| [Police National Legal Databaseのデータがダークウェブに流出したことを確認](https://www.itpro.com/security/data-breaches/police-national-legal-database-confirms-data-leaked-on-the-dark-web) | 20.0 | 20.0 | 42.0 |
| [UKの警察法律データベースでデータ漏えいが発生](https://www.infosecurity-magazine.com/news/uks-police-national-legal-database/) | 20.0 | 20.0 | 42.0 |
| [Madera Community Hospitalのデータ侵害で15万人に影響](https://www.securityweek.com/150000-impacted-by-madera-community-hospital-data-breach/) | 20.0 | 20.0 | 42.0 |
| [中部電 7万人超の情報漏えい恐れ](https://news.yahoo.co.jp/pickup/6590517?source=rss) | 20.0 | 20.0 | 42.0 |

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
