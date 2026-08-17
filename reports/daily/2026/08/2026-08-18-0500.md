# 📡 サイレーダー 2026-08-18 05:00 JST

このレポートは、2026-08-17 17:00 JST〜2026-08-18 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 79
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 46

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [17th August – Threat Intelligence Report](#topic-27063) | 49.0 | 56.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [CVE-2025-62593: CISA KEV catalog addition](#topic-27918) | 45.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 3 | [Microsoft working on Defender patch for ShieldBreak zero-day](#topic-27906) | 43.0 | 46.0 | 55.0 | 音声 | 温度感上位枠 |
| 4 | [Update your Mac: Screen Sharing vulnerability exploited in the wild](#topic-27912) | 43.0 | 46.0 | 55.0 | 音声 | 温度感上位枠 |
| 5 | [⚡ Weekly Recap: VMware Exploits, Windows 0-Day, MCP Attacks, Browser Hijacks and More](#topic-27909) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [Operation ASTERIX: Anatomy of a Crypto Fraud Pipeline](#topic-27922) | 35.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [When the Playbook Breaks: AI Incident Response for Systems That Don't Behave Like Anything Else](#topic-27886) | 33.0 | 30.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-27063"></a>

### 1. 17th August – Threat Intelligence Report

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 49.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

CVE-2026-68820は、Windows関連の脆弱性として、すでに悪用が確認されている文脈で報告されています。
関連情報では、Lazarus GroupによるとされるOperation Dream Jobキャンペーンの一部として、防衛分野、とくに航空宇宙・航空関連の組織が標的になっていたとされています。
ゼロデイとして悪用されていた可能性がある点に加え、対象が防衛・航空宇宙分野に及ぶため、影響範囲の見極めが重要です。
Microsoftの修正対象にも含まれており、優先度の高い更新確認が求められます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当するWindows環境で、Microsoftの修正適用状況を確認する。
- 防衛・航空宇宙関連の組織では、関連キャンペーンを前提にログや端末の異常挙動を点検する。
- 特に特権昇格につながる可能性があるため、最小権限や端末保護、EDRの検知状況を再確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-49113 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-53413 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-65400 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-68820 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-71362 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 脅威アクター | Lazarus Group | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-68820](https://nvd.nist.gov/vuln/detail/CVE-2026-68820) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [17th August – Threat Intelligence Report](https://research.checkpoint.com/2026/17th-august-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Lazarus hackers exploited Windows zero-day to target defense firms](https://www.bleepingcomputer.com/news/security/lazarus-hackers-exploited-windows-zero-day-to-target-defense-firms/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft patches 400+ vulnerabilities, one zero-day under attack (CVE-2026-6882](https://www.helpnetsecurity.com/2026/08/12/august-2026-patch-tuesday-cve-2026-68820/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Plugs Nearly 400 Security Holes](https://krebsonsecurity.com/2026/08/microsoft-plugs-nearly-400-security-holes/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches 398 Flaws Including a Windows Driver Zero-Day Under Active Att](https://thehackernews.com/2026/08/microsoft-patches-398-flaws-including.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Shattering the Dream – When a Job Offer Becomes a Zero-Day Attack](https://research.checkpoint.com/2026/shattering-the-dream-when-a-job-offer-becomes-a-zero-day-attack/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-27918"></a>

### 2. CVE-2025-62593: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

CISAは、実際の悪用が確認されたとして、CVE-2025-62593をKnown Exploited Vulnerabilities（KEV）Catalogに追加しました。
対象はRay Project Rayに関するコードインジェクションの脆弱性とされています。
KEV追加は、単なる未修正の脆弱性ではなく、攻撃者による悪用が疑われる優先対応対象であることを示します。
公開資産を含め、影響を受ける環境では迅速な確認と修正の優先度を上げる必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当製品の利用有無を確認し、ベンダー情報に基づいて修正対応を優先する。
- 公開されている資産や外部接続面で該当機能・コンポーネントがないか点検する。
- 侵害の兆候がないか、ログや認証・実行履歴を含めて確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-62593 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-62593](https://nvd.nist.gov/vuln/detail/CVE-2025-62593) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/08/17/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-27906"></a>

### 3. Microsoft working on Defender patch for ShieldBreak zero-day

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

Microsoft Defenderに関連するゼロデイ脆弱性「ShieldBreak」が報じられており、Microsoftは修正パッチの対応を進めているとされています。
材料ではCVE-2026-69414として追跡され、既存の修正を回避してSYSTEM権限の取得につながる可能性が示されています。
Defenderは広く利用される防御機能のため、回避可能な欠陥は端末保護の前提を揺るがすおそれがあります。
ゼロデイとして扱われている点から、公開後の修正までの間に悪用リスクが高まりやすい点が注目されます。

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

#### 担当者向け確認ポイント

- Microsoftからの修正情報と適用対象の更新有無を継続確認する。
- Defender関連の異常な権限昇格や保護機能の無効化兆候を監視する。
- OSとセキュリティ製品の更新適用状況を点検し、未適用端末を優先対応する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-69414 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-69414](https://nvd.nist.gov/vuln/detail/CVE-2026-69414) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [ShieldBreak bypasses Microsoft’s patch for earlier Defender flaw](https://www.malwarebytes.com/blog/bugs/2026/08/shieldbreak-bypasses-microsofts-patch-for-earlier-defender-flaw) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft working on Defender patch for ShieldBreak zero-day](https://www.bleepingcomputer.com/news/security/microsoft-working-on-defender-patch-for-shieldbreak-zero-day/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-27912"></a>

### 4. Update your Mac: Screen Sharing vulnerability exploited in the wild

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

AppleのmacOSにあるScreen Sharing関連の脆弱性（CVE-2026-65400）が、実際に悪用されていると報じられています。
報道によれば、認証を回避してroot権限を得たり、暗号資産のマイニング用ソフトを導入されたりする可能性があるため、Appleは修正版を含むアップデートを案内しています。
認証回避につながる脆弱性が実環境で悪用されている点が重要です。対象端末では権限昇格や不正なソフト導入につながるおそれがあるため、早急な更新確認が求められます。

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

#### 担当者向け確認ポイント

- macOS Sequoia 15.7.9、Sonoma 14.8.9、Tahoe 26.6.1 への更新状況を確認する。
- Screen Sharingの利用可否や外部からの到達性を見直し、不要なら無効化を検討する。
- 不審な高負荷、未知の常駐プロセス、暗号資産マイニングの兆候がないか端末を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-65400 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Apple | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-65400](https://nvd.nist.gov/vuln/detail/CVE-2026-65400) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Attackers exploit patched macOS Screen Sharing flaw to deploy cryptominer](https://www.helpnetsecurity.com/2026/08/17/apple-macos-screen-sharing-flaw/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Update your Mac: Screen Sharing vulnerability exploited in the wild](https://www.malwarebytes.com/blog/bugs/2026/08/update-your-mac-screen-sharing-vulnerability-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Recent macOS Screen Sharing Vulnerability Exploited in Attacks](https://www.securityweek.com/recent-macos-screen-sharing-vulnerability-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-27909"></a>

### 5. ⚡ Weekly Recap: VMware Exploits, Windows 0-Day, MCP Attacks, Browser Hijacks and More

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>サ⁠プ⁠ラ⁠イ⁠チ⁠ェ⁠ー⁠ン</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>M⁠C⁠P</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

今週の公開情報をまとめた記事では、VMware関連の悪用、Windowsのゼロデイ、MCPを狙う攻撃、ブラウザの乗っ取りなど、複数の話題が取り上げられています。
新しい手口というより、既存の脆弱性や露出したサービス、セッション管理の弱点が再び悪用される傾向が示されています。
個別の製品や単発の脆弱性に限らず、初期侵入後の横展開や既存アクセスの悪用が被害拡大につながる点が注目されます。
防御側は「未使用のはずの露出」「古い脆弱性の再利用」「ブラウザセッションの保護」を改めて見直す必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- VMwareやWindowsなど、対象製品の修正状況と自組織の適用状況を確認する。
- 外部公開サービスや不要な露出を棚卸しし、侵入経路になり得る面を減らす。
- ブラウザセッションや認証情報の保護を強化し、異常なアクセスや横展開の兆候を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Broadcom | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [⚡ Weekly Recap: VMware Exploits, Windows 0-Day, MCP Attacks, Browser Hijacks and](https://thehackernews.com/2026/08/weekly-recap-vmware-exploits-windows-0.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-27922"></a>

### 6. Operation ASTERIX: Anatomy of a Crypto Fraud Pipeline

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Rapid7は、暗号資産関連の詐欺キャンペーンを支える公開状態のサーバーを発見し、電話番号の選別、フィッシング、ボイスフィッシング、偽ウォレットアプリ、Telegram経由の情報送信などが連携した多段階の手口を確認したと報告しました。
あわせて、この運用の開発や調整にAIコーディング支援ツールが使われていた痕跡も見つかり、モデルを切り替えながら作業を進めようとした形跡も示されています。
暗号資産ユーザーを狙う詐欺が、メール・電話・偽アプリを組み合わせてより説得力を増している実態を示しています。
さらに、攻撃側がAIを開発補助や運用効率化に組み込んでいる点は、今後の対策や検知の考え方にも影響します。

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

- 本人確認やサポート連絡を装うメールと電話の組み合わせを前提に、問い合わせ経路や認証手順を再点検する。
- 偽ウォレットや不審なインストーラの配布経路を想定し、アプリ配布・署名・更新手順の案内を厳格化する。
- AI支援コードの悪用を前提に、フィッシング文面、反復的な自動化、外部送信先への異常通信をまとめて監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Anthropic | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Mozilla | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| ベンダー | Apple | 言及あり | 0.80 | — |
| 製品 | Exchange | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Operation ASTERIX: Anatomy of a Crypto Fraud Pipeline](https://www.rapid7.com/blog/post/tr-operation-asterix-crypto-fraud-vishing-phishing) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-27886"></a>

### 7. When the Playbook Breaks: AI Incident Response for Systems That Don't Behave Like Anything Else

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

生成AIの導入が進む一方で、AIシステムが侵害された際に「何を初動とするか」を明確にしたインシデント対応手順が整っていない組織が多い、という課題が示されています。
従来のランサムウェアやアカウント乗っ取り向けのプレイブックだけでは、AI特有の挙動や影響範囲に十分対応しにくい点が論点です。
AIが業務に組み込まれるほど、障害や不正利用が発生した際の影響は情報漏えいだけでなく、出力品質や業務判断にも及び得ます。
実務では、AI専用の封じ込め・停止・復旧の考え方をあらかじめ用意しておく必要があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIシステムを対象にしたインシデント分類と初動判断基準を、既存のIR手順に追加する。
- モデル、プロンプト、接続先、権限、ログなど、AI特有の確認対象を棚卸ししておく。
- 停止・切り戻し・代替手段の手順を、通常の障害対応と分けて事前に検証する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [When the Playbook Breaks: AI Incident Response for Systems That Don't Behave Lik](https://cloudsecurityalliance.org/articles/when-the-playbook-breaks-ai-incident-response-for-systems-that-don-t-behave-like-anything-else) | <nobr>内容確認・補足情報</nobr> |

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
| [Kimsuky、Operation GitPowerでローカルAI開発環境を通じてAI能力を拡張](https://blog.polyswarm.io/kimsuky-expands-ai-capabilities-through-a-local-ai-development-environment-in-operation-gitpower) | 33.0 | 20.0 | 42.0 |
| [Claude Agentsが自己複製型マルウェアを展開するよう促された対立するテスト目標](https://www.securityweek.com/conflicting-test-goals-pushed-claude-agents-to-deploy-self-replicating-malware/) | 33.0 | 20.0 | 42.0 |
| [Apple Screen Sharingのセキュリティ問題](https://isc.sans.edu/diary/rss/33252) | 30.0 | 20.0 | 42.0 |
| [PhilipsとGE、Clopランサムウェアによるデータ窃取の主張を調査](https://www.bleepingcomputer.com/news/security/philips-and-ge-investigating-clop-ransomware-data-theft-claims/) | 28.0 | 30.0 | 42.0 |
| [LinuxボットネットEvooo1BotがMiraiの機能をDDoSを大きく超えて拡張](https://www.darkreading.com/cyber-risk/linux-botnet-evooo1bot-mirai-capabilities-beyond-ddos) | 28.0 | 20.0 | 42.0 |
| [Evooo1Bot Linuxボットネット、既知の脆弱性を悪用してエッジデバイスをSOCKS5プロキシ化](https://thehackernews.com/2026/08/evooo1bot-linux-botnet-exploits-known.html) | 28.0 | 20.0 | 42.0 |
| [実はAnthropicには最上位のMythosよりも強力な「Model 2」というAIモデルがあるがリリース予定はない](https://gigazine.net/news/20260817-anthropic-model-2/) | 27.0 | 20.0 | 42.0 |
| [NTTドコモビジネスとエクサウィザーズ、「クローズドAIエージェント」を提供開始](https://japan.zdnet.com/article/35251625/) | 26.0 | 20.0 | 42.0 |
| [AIがSnowflakeのコードを解読し、別のAIエージェントがそれを悪用した話](https://www.theregister.com/security/2026/08/17/an-ai-broke-snowflakes-code-then-another-ai-agent-exploited-it/5288666) | 25.0 | 20.0 | 42.0 |
| [Irregular、AIハッキング事後報告の「誇張」表現に批判](https://therecord.media/irregular-ai-hacking-model-blog) | 25.0 | 20.0 | 42.0 |
| [機械学習を使ってFlockカメラから車両を隠す「見えない」車の研究](https://www.bitdefender.com/en-us/blog/hotforsecurity/invisible-car-machine-learning-hide-vehicle-flock-cameras) | 25.0 | 20.0 | 42.0 |
| [Wiz Red AgentがAI生成のGitHub Copilot「Autofix」によりSnowflakeの内部Jiraに侵入した件](https://www.wiz.io/blog/red-agent-snowflake-copilot-cicd-bug) | 25.0 | 20.0 | 42.0 |
| [FortinetがVirtue AIを買収しAIセキュリティ製品群を拡充](https://www.helpnetsecurity.com/2026/08/17/fortinet-virtue-ai-acquisition/) | 25.0 | 20.0 | 42.0 |
| [命名ミスがAIモデルによる実在企業への攻撃を可能にした経緯を不規則な詳細が明らかにする](https://www.securityweek.com/irregular-details-how-a-naming-error-let-ai-models-attack-a-real-company/) | 25.0 | 20.0 | 42.0 |
| [生成AIで標章偽造の疑い 書類送検](https://news.yahoo.co.jp/pickup/6592107?source=rss) | 25.0 | 20.0 | 42.0 |
| [あなたのWebサイトには今や2つのオーディエンスがいる：人間とAI](https://www.akamai.com/blog/trends/2026/aug/website-two-audiences-humans-ai) | 25.0 | 20.0 | 42.0 |
| [MCPサーバーが企業の機密情報を露呈させる仕組み](https://thehackernews.com/2026/08/how-mcp-servers-can-expose-enterprise.html) | 25.0 | 20.0 | 42.0 |
| [2026年版 主要AIガバナンスプラットフォーム比較ガイド](https://securityboulevard.com/2026/08/top-ai-governance-platforms-2026-comparison-guide-kovrr/) | 25.0 | 20.0 | 42.0 |
| [Code FixersがAIワープドライブを始動、新たな未知の世界へ](https://www.theregister.com/columnists/2026/08/17/code-fixers-have-fired-up-the-ai-warp-drive-strange-new-worlds-await/5287681) | 25.0 | 20.0 | 42.0 |
| [UNISOCモデムの脆弱性でビデオ通話経由のリモートコード実行が可能に](https://www.infosecurity-magazine.com/news/unisoc-modem-flaw-rce-calls/) | 24.0 | 38.0 | 42.0 |
| [WordPressプラグインの脆弱性により4万サイトが管理者乗っ取りの危険にさらされる](https://www.infosecurity-magazine.com/news/wordpress-plugin-flaw-40000-sites/) | 24.0 | 38.0 | 42.0 |
| [UnisocのVoLTEビデオ通話脆弱性連鎖により攻撃者がAndroidカーネルへ完全アクセス可能に](https://thehackernews.com/2026/08/unisoc-volte-video-call-exploit-chain.html) | 24.0 | 38.0 | 42.0 |
| [「PoE」好きが1人で作った自由すぎるビルド構築が魅力のローグライトARPG「響き、夢境に(Dream Echo)」をプレイしてみた](https://gigazine.net/news/20260817-dream-echo/) | 22.0 | 20.0 | 42.0 |
| [医師が病室に個人情報含む書類を置き忘れ、患者宅から回収 - 川崎市](https://www.security-next.com/188882) | 22.0 | 20.0 | 42.0 |
| [「うんこミュージアム」でサイト改ざん - 個人情報流出の可能性](https://www.security-next.com/188876) | 22.0 | 20.0 | 42.0 |
| [15歳未満のSNS利用禁止法案を表現の自由を侵害するとして最高裁が差し止め](https://gigazine.net/news/20260817-france-top-court-blocks-sns-ban-under-15s/) | 22.0 | 20.0 | 42.0 |
| [SAP Commerce Cloudの重大な脆弱性、公開3日後に悪用開始](https://www.securityweek.com/critical-sap-commerce-cloud-vulnerability-exploited-3-days-after-disclosure/) | 20.0 | 28.0 | 50.0 |
| [Pokémon Centerのデータ侵害で顧客情報が流出、一部注文をキャンセル](https://www.bleepingcomputer.com/news/security/pokemon-center-data-breach-exposes-customer-info-cancels-some-orders/) | 20.0 | 20.0 | 42.0 |
| [チャネルの次なる信頼試験は主権問題](https://www.itpro.com/security/data-protection/sovereignty-is-the-channels-next-trust-test) | 20.0 | 20.0 | 42.0 |
| [SafePal、最新の侵害で約4万人に影響する暗号資産ハードウェアウォレットメーカー被害](https://therecord.media/safepal-crypto-hardware-breach) | 20.0 | 20.0 | 42.0 |
| [Poland、MyDrヘルスケアソフトウェア侵害を調査、最大1900万人に影響の可能性](https://therecord.media/poland-probes-mydr-healthcare-software-breach) | 20.0 | 20.0 | 42.0 |
| [大手遺伝子検査企業、ハッキングで患者の機微情報が流出](https://www.cybersecuritydive.com/news/baylor-genetics-cyberattack-compromise-patient-data-genetic-testing/828019/) | 20.0 | 20.0 | 42.0 |
| [フランス税務当局、ハッカーによる侵害で67万8000人分のデータ流出を認める](https://www.helpnetsecurity.com/2026/08/17/france-tax-authority-data-breach/) | 20.0 | 20.0 | 42.0 |
| [フランス税務当局のデータ侵害で68万人に影響](https://www.securityweek.com/680000-impacted-by-french-tax-authority-data-breach/) | 20.0 | 20.0 | 42.0 |
| [ドローン攻撃の中、ロシアのEC大手Wildberriesがサイバー攻撃を受けたとウクライナが発表](https://therecord.media/russia-wildberries-cyberattack-ukraine) | 20.0 | 20.0 | 42.0 |
| [企業のAzureテナントから不正に窃取されたとされる数百万件のレコードを狙う攻撃者](https://www.theregister.com/security/2026/08/17/crook-hawks-millions-of-records-allegedly-plundered-from-corporate-azure-tenants/5288305) | 20.0 | 20.0 | 42.0 |
| [TikTokの偽リワードで現金を餌にする詐欺](https://www.malwarebytes.com/blog/scams/2026/08/fake-tiktok-rewards-promise-cash-youll-never-get) | 20.0 | 20.0 | 42.0 |
| [ETSI、サイバーレジリエンス法を支援する17のサイバーセキュリティ標準を提案](https://www.infosecurity-magazine.com/news/etsi-proposes-17-cybersecurity/) | 20.0 | 20.0 | 42.0 |
| [SafePalの侵害で39,798人の顧客に影響、データが販売されている可能性](https://www.helpnetsecurity.com/2026/08/17/safepal-data-breach-customer-order-information/) | 20.0 | 20.0 | 42.0 |
| [French tax authorityのデータ侵害、67万8000人に影響](https://www.bleepingcomputer.com/news/security/french-tax-authority-data-breach-affects-678-000-individuals/) | 20.0 | 20.0 | 42.0 |
| [Symantec CBXに関する謝罪なし](https://www.security.com/expert-perspectives/no-apologies-symantec-cbx) | 20.0 | 20.0 | 42.0 |
| [SafePalのデータ侵害で4万人に影響](https://www.securityweek.com/40000-impacted-by-safepal-data-breach/) | 20.0 | 20.0 | 42.0 |
| [SafePalのデータ侵害で数万人の顧客に影響](https://www.infosecurity-magazine.com/news/safepal-data-breach-tens-thousands/) | 20.0 | 20.0 | 42.0 |
| [セキュリティデータの増加が企業のリスク把握を曇らせる理由](https://www.cybersecuritydive.com/spons/why-more-security-data-has-blurred-companies-view-of-risk/827640/) | 20.0 | 20.0 | 42.0 |
| [Facebookの広告ブロッカー対策が詐欺師を利する理由](https://www.malwarebytes.com/blog/news/2026/08/why-facebooks-war-on-ad-blockers-could-help-scammers) | 20.0 | 20.0 | 42.0 |
| [警察が4日間で3000万ユーロを盗んだとされるサイバー犯罪組織を摘発](https://www.helpnetsecurity.com/2026/08/17/germany-brazil-bank-fraud-ring-dismantled/) | 20.0 | 20.0 | 42.0 |

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
