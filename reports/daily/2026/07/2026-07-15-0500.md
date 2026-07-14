# 📡 サイレーダー 2026-07-15 05:00 JST

このレポートは、2026-07-14 17:00 JST〜2026-07-15 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 94
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 64

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Microsoft 2026年7月 Patch Tuesday 関連まとめ](#topic-22358) | 66.0 | 69.0 | 51.0 | 音声 | 温度感上位枠 |
| 2 | [Baddies caught exploiting extensions bugs with perfect 10 scores on vulnerable Joomla websites](#topic-22409) | 55.0 | 56.0 | 47.0 | 音声 | 温度感上位枠 |
| 3 | [SonicWall SMA appliances targeted in zero-day attacks (CVE-2026-15409, CVE-2026-15410)](#topic-22364) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 4 | [Microsoft Patches Record 622 Vulnerabilities, Including Two Exploited Zero-Days](#topic-22359) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [Progress confirms ShareFile zero-day flaw behind Storage Zone shutdown](#topic-22369) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-22358"></a>

### 1. Microsoft 2026年7月 Patch Tuesday 関連まとめ

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>A⁠I</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>A⁠n⁠d⁠r⁠o⁠i⁠d</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 66.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 69.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

Microsoftの2026年7月のPatch Tuesdayでは、非常に多数の脆弱性修正が含まれ、重大度の高いものも複数あるとされています。
公開前に把握されていた脆弱性や、すでに悪用が確認されているものも含まれるため、通常月以上に対応優先度が高い状況です。
既に悪用済みとされる脆弱性が含まれている点は、放置時の被害拡大につながるおそれがあるため注目されています。
影響範囲が広く、Edge関連のChromium修正も別途存在するため、更新漏れが起きやすい点にも注意が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 技術詳細・再現情報あり。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。
- 技術詳細により影響確認が進みやすい。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- まずは既知の悪用済み・公開済みとされる脆弱性の修正状況を優先確認する。
- Windows本体だけでなく、Edgeを含む関連製品の更新適用状況もまとめて点検する。
- 広範な修正が含まれるため、資産台帳に基づいて対象環境を洗い出し、段階的に展開と検証を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-26145 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-33842 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34328 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34346 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34348 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34349 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-40378 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-40400 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-40422 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-41087 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft Patch Tuesday July 2026 - The AI Acopolypse is Here , (Tue, Jul 14th)](https://isc.sans.edu/diary/rss/33154) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft July 2026 Patch Tuesday fixes massive 570 flaws, 3 zero-days](https://www.bleepingcomputer.com/news/microsoft/microsoft-july-2026-patch-tuesday-fixes-massive-570-flaws-3-zero-days/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [The July 2026 Security Update Review](https://www.thezdi.com/blog/2026/7/14/the-july-2026-security-update-review) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-22409"></a>

### 2. Baddies caught exploiting extensions bugs with perfect 10 scores on vulnerable Joomla websites

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 55.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 47.0 |

#### 概要

公開情報では、Joomla向け拡張機能の脆弱性が悪用されているとみられ、影響を受けるサイトでは不正アクセスや改ざんのリスクが懸念されています。
関連する脆弱性は高い深刻度で扱われており、パッチ未適用環境では注意が必要です。
CMSや拡張機能の脆弱性は、サイト本体ではなく周辺コンポーネント経由で広く影響が及ぶことがあります。実際の悪用が示唆されている場合、迅速な更新と監視の優先度が高まります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Joomla本体だけでなく、iCagendaやBalbooa Formsなど導入済み拡張機能の更新状況を確認する。
- 公開中の管理画面や不要な機能を見直し、外部から到達できる範囲を最小限にする。
- 不審な管理者操作、改ざん、見覚えのないファイル追加など、サイト改変の兆候を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-32201 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-45659 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-48939 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-55040 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-56164 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-56291 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-58644 | 関連CVE | 1.00 | 未確認 |
| 製品 | Joomla | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Urges SharePoint Hardening After New Exploitations](https://www.cisa.gov/news-events/alerts/2026/07/14/cisa-urges-sharepoint-hardening-after-new-exploitations) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Baddies caught exploiting extensions bugs with perfect 10 scores on vulnerable J](https://www.theregister.com/security/2026/07/14/baddies-caught-exploiting-extensions-bugs-with-perfect-10-scores-on-vulnerable-joomla-websites/5271001) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-22364"></a>

### 3. SonicWall SMA appliances targeted in zero-day attacks (CVE-2026-15409, CVE-2026-15410)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

SonicWallのSecure Mobile Access（SMA）1000シリーズ機器を狙うゼロデイ攻撃が報告され、同社はCVE-2026-15409とCVE-2026-15410を修正したとしています。
影響を受ける可能性がある組織には、修正版への更新と、侵害の痕跡がないかの確認が求められています。
VPN/リモートアクセス系の機器は社内外の接点になりやすく、侵害時の影響が広がりやすい点が注目されます。
悪用が観測されているとされるため、該当製品を使う組織では早急な対応判断が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SMA 1000シリーズの利用有無と対象バージョンを確認し、修正版への更新可否を評価する。
- ベンダーが示す侵害痕跡を点検し、ログや設定の異常がないかを確認する。
- もし侵害の疑いがある場合は、利用停止や再展開、パスワード変更、TOTPトークンの再設定を含む復旧手順を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-15409 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-15410 | 関連CVE | 1.00 | 未確認 |
| ベンダー | SonicWall | 言及あり | 0.80 | — |
| 製品 | SonicWall SMA | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-15409](https://nvd.nist.gov/vuln/detail/CVE-2026-15409) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [SonicWall SMA appliances targeted in zero-day attacks (CVE-2026-15409, CVE-2026-](https://www.helpnetsecurity.com/2026/07/14/sonicwall-sma-attacks-via-cve-2026-15409-cve-2026-15410/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22359"></a>

### 4. Microsoft Patches Record 622 Vulnerabilities, Including Two Exploited Zero-Days

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Microsoftは、記録的な件数となる622件の脆弱性に対する修正を公開しました。
提供された材料では、Active DirectoryとSharePoint Serverに関する2件の問題がゼロデイとして悪用されていたとされ、BitLockerの脆弱性も公表されています。
広く使われるMicrosoft製品に関わるため、組織への影響範囲が大きくなりやすい点が注目されています。特に悪用が確認された脆弱性は、優先度を上げて対応する必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 影響を受ける可能性があるMicrosoft製品の更新状況を確認し、適用優先度を見直す。
- Active DirectoryとSharePoint Serverを利用している環境では、関連する修正内容と自組織の構成を照合する。
- 公開情報ベースで悪用が示されているため、通常より早い監視強化と資産棚卸しを行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-50518 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-50522 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-50661 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-55008 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-55010 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-56155 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-56164 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-56188 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-56190 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-57092 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft Patches Record 622 Vulnerabilities, Including Two Exploited Zero-Days](https://www.securityweek.com/microsoft-patches-record-622-vulnerabilities-including-two-exploited-zero-days/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22369"></a>

### 5. Progress confirms ShareFile zero-day flaw behind Storage Zone shutdown

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

Progress Softwareは、ShareFileのStorage Zone Controllers停止の背景に高深刻度のゼロデイ脆弱性があったことを確認し、修正アップデートを公開しました。
現時点では詳細な技術情報は限られますが、影響製品を利用している組織は更新状況の確認が必要です。
ゼロデイ脆弱性は、対策前に悪用される可能性があるため影響が大きくなりやすい点が注目されています。ファイル共有系の基盤機能に関わるため、業務への波及も懸念されます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ShareFileおよびStorage Zone Controllersの利用有無を確認し、提供済みの修正更新を優先適用する。
- ベンダーの案内に沿って、停止や切り戻しを含む運用影響を確認し、必要な監視を強化する。
- 不審なアクセスや設定変更の有無を点検し、関連するログを保全しておく。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Progress Software | 言及あり | 0.80 | — |
| 製品 | Citrix ShareFile | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Progress confirms ShareFile zero-day flaw behind Storage Zone shutdown](https://www.bleepingcomputer.com/news/security/progress-confirms-sharefile-zero-day-flaw-behind-storage-zone-shutdown/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
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
| [米財務省、ランサムウェア集団を支援したFirst VPN Serviceなどに制裁を科す](https://cyberscoop.com/us-sanctions-first-vpn-ransomware/) | 36.0 | 30.0 | 42.0 |
| [米国、ランサムウェア攻撃を助長したVPNおよびマルウェア提供者に制裁](https://www.bleepingcomputer.com/news/security/us-sanctions-vpn-malware-providers-linked-to-ransomware-gangs/) | 36.0 | 30.0 | 42.0 |
| [米国、ランサムウェア支援で初のVPNサービスとマルウェア暗号化ツール販売者を制裁](https://thehackernews.com/2026/07/us-sanctions-first-vpn-service-and.html) | 36.0 | 30.0 | 42.0 |
| [Rockwell Automation 1715-AENTR EtherNet/IPアダプタの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-195-04) | 32.0 | 46.0 | 50.0 |
| [AsyncAPI名前空間の侵害されたnpmパッケージがMiasmaボットネットローダーを配布](https://socket.dev/blog/asyncapi-supply-chain-attack) | 30.0 | 30.0 | 42.0 |
| [MacOSマルウェアが正規のDeveloper IDを悪用しAppleのクラッシュレポーターを装う](https://www.infosecurity-magazine.com/news/macos-malware-apple-crash-reporter/) | 28.0 | 45.0 | 42.0 |
| [複数のJscramblerパッケージがサプライチェーン攻撃の影響を受ける](https://www.securityweek.com/multiple-jscrambler-packages-impacted-by-supply-chain-attack/) | 28.0 | 45.0 | 42.0 |
| [ランサムウェア被害者に数百万ドルの損失をもたらした内部犯行](https://www.malwarebytes.com/blog/news/2026/07/the-inside-job-that-cost-ransomware-victims-millions) | 28.0 | 30.0 | 42.0 |
| [正規ソフトウェアを装ってマルウェアを拡散する約300件のGitHubリポジトリ](https://www.bleepingcomputer.com/news/security/nearly-300-github-repos-pose-as-legit-software-to-push-malware/) | 28.0 | 20.0 | 42.0 |
| [Langflowが悪用されカスタムDDoS用Gafgytボットネットが構築される](https://www.akamai.com/blog/security-research/2026/jul/langflow-exploited-build-custom-ddos-gafgyt-botnets) | 28.0 | 20.0 | 42.0 |
| [LastPassとBitwardenのユーザーを狙う偽のセキュリティ警告](https://www.bleepingcomputer.com/news/security/lastpass-bitwarden-users-targeted-with-fake-security-alerts/) | 28.0 | 20.0 | 42.0 |
| [Appleのクラッシュ報告ツールを装う新たなmacOSマルウェア、パスワードを窃取](https://www.helpnetsecurity.com/2026/07/14/crashstealer-macos-infostealer-password-theft/) | 28.0 | 20.0 | 42.0 |
| [Microsoft署名の古いLinux向けUEFI Shim 11件がSecure Bootを回避される恐れ](https://thehackernews.com/2026/07/11-old-microsoft-signed-linux-uefi.html) | 28.0 | 20.0 | 42.0 |
| [OAuthクライアントIDのなりすましにより盗難されたMicrosoft Entra資格情報を検証可能にする脆弱性](https://thehackernews.com/2026/07/oauth-client-id-spoofing-lets-attackers.html) | 28.0 | 20.0 | 42.0 |
| [米国と同盟国、重要インフラのルーターを狙うロシアのサイバー攻撃に警告](https://www.securityweek.com/us-allies-warn-of-russian-cyberattacks-targeting-critical-infrastructure-routers/) | 28.0 | 20.0 | 42.0 |
| [CVE-2026-55040: Microsoft SharePointのJWTトークン認証バイパス（修正済み）](https://www.rapid7.com/blog/post/ve-cve-2026-55040-microsoft-sharepoint-jwt-token-authentication-bypass-fixed) | 27.0 | 20.0 | 42.0 |
| [AIで「人間が頂点の時代終わる」――孫正義氏が考える2040年 人類が生きる道は“スーパーヒューマン化”](https://www.itmedia.co.jp/news/articles/2607/14/news115.html) | 26.0 | 20.0 | 42.0 |
| [上半期「情報サービス業」倒産、過去10年で最多 生成AIやノーコード普及が零細に逆風](https://www.itmedia.co.jp/news/articles/2607/14/news104.html) | 26.0 | 20.0 | 42.0 |
| [Frontier AI：ジーニーは瓶から出たが、ルールブックはどこにあるのか？](https://www.darkreading.com/cybersecurity-operations/frontier-ai-genie-out-of-bottle-where-rulebook) | 25.0 | 20.0 | 42.0 |
| [サイバー防御におけるAI導入の急増で露呈した大きなガバナンスの空白](https://www.cybersecuritydive.com/news/ai-adoption-cyber-defense-governance-gap/825179/) | 25.0 | 20.0 | 42.0 |
| [未修正のClaude for Chromeの脆弱性により拡張機能がGmailとカレンダーを読み取れる問題](https://www.securityweek.com/unpatched-claude-for-chrome-flaw-lets-extensions-read-gmail-calendar/) | 25.0 | 20.0 | 42.0 |
| [AI主導の攻撃を妨害する「コンテキスト爆弾」、研究者が発見](https://www.helpnetsecurity.com/2026/07/14/context-bombs-for-defensive-prompt-injection/) | 25.0 | 20.0 | 42.0 |
| [「The bots are alive!」Jailbroken Geminiがわずか6分でロシアの詐欺師向け新C2サーバーを立ち上げた](https://www.theregister.com/research/2026/07/14/the-bots-are-alive-jailbroken-gemini-spun-up-new-c2-server-for-russian-fraudster-in-just-6-minutes/5270131) | 25.0 | 20.0 | 42.0 |
| [PenteraがAIセキュリティワークフローを検証エンジンへ変える方法](https://thehackernews.com/2026/07/how-pentera-turns-ai-security-workflows.html) | 25.0 | 20.0 | 42.0 |
| [ABB T-MAC Plusの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-195-03) | 24.0 | 46.0 | 50.0 |
| [VMware Avi Load Balancerで修正された7件の重大な脆弱性](https://www.securityweek.com/7-severe-vulnerabilities-patched-in-vmware-avi-load-balancer/) | 24.0 | 38.0 | 42.0 |
| [ClickFixの急拡大するエコシステムに対する新たな防御戦術](https://www.darkreading.com/cyberattacks-data-breaches/clickfixs-ecosystem-demands-new-defense) | 22.0 | 20.0 | 42.0 |
| [サイバー攻撃により6週間にわたり生産停止の影響を受けた繊維企業ZEGOが破産申請](https://gigazine.net/news/20260714-zego-insolvency/) | 22.0 | 20.0 | 42.0 |
| [サイバー攻撃でシステム障害、冷凍食品の出荷に影響 - ニチレイ](https://www.security-next.com/187300) | 22.0 | 20.0 | 42.0 |
| [個人情報含むファイルを誤送信、別ファイルと勘違い - 大阪市](https://www.security-next.com/186709) | 22.0 | 20.0 | 42.0 |
| [[動画] 保護の出発点：Cisco Talos Intelligence Integrations](https://blog.talosintelligence.com/video-where-protection-starts-cisco-talos-intelligence-integrations/) | 22.0 | 20.0 | 42.0 |
| [蛇の舌：Pythonを巣穴からおびき出す](https://blog.talosintelligence.com/the-serpents-tongue-luring-the-python-out-of-its-den/) | 22.0 | 20.0 | 42.0 |
| [「GCP」に他テナントのリポジトリを乗っ取れる脆弱性 - 5月に修正](https://www.security-next.com/187328) | 22.0 | 20.0 | 42.0 |
| [iOS 27やmacOS 27のパブリックベータ版が公開される、iPhoneのアップデート手順はこんな感じ](https://gigazine.net/news/20260714-apple-ios-macos-public-beta/) | 22.0 | 20.0 | 42.0 |
| [KFC、全店舗で品切れや臨時休業のおそれ ネット注文も停止 原因はニチレイへの不正アクセス](https://www.itmedia.co.jp/news/articles/2607/14/news113.html) | 21.0 | 20.0 | 42.0 |
| [M-Red-Team: GitHub Actionsを介したAsyncAPIのサプライチェーン侵害](https://www.wiz.io/blog/m-red-team-asyncapi-supply-chain-compromise-via-github-actions) | 20.0 | 45.0 | 42.0 |
| [ABB Advant Master Online Builderの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-195-01) | 20.0 | 28.0 | 50.0 |
| [米国、ロシアの防弾ホスティングサービス運営者とされる人物らに対する起訴を公開](https://therecord.media/us-unseals-indictment-russians-bulletproof-hosting) | 20.0 | 20.0 | 42.0 |
| [Microsoft、Windows 10向けKB5099539延長セキュリティ更新を公開](https://www.bleepingcomputer.com/news/microsoft/microsoft-releases-windows-10-kb5099539-extended-security-update/) | 20.0 | 20.0 | 42.0 |
| [Synopsys、Boschハック報道の中でデータ侵害の証拠なしと発表](https://www.securityweek.com/synopsys-finds-no-evidence-of-data-breach-following-bosch-hack-claims/) | 20.0 | 20.0 | 42.0 |
| [実践的な手順でベンダーリスクを管理する](https://www.darkreading.com/cyber-risk/manage-vendor-risk-in-a-few-practical-steps) | 20.0 | 20.0 | 42.0 |
| [フィンランド、巨大な心理療法データ漏えいの背後にいるハッカーに指名手配通知を発行](https://therecord.media/finland-issues-wanted-notice-for-hacker-vastaamo-breach) | 20.0 | 20.0 | 42.0 |
| [Adobe、ColdFusionの重大な脆弱性を修正](https://www.securityweek.com/adobe-patches-critical-coldfusion-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [LabubaRATがNVIDIAソフトウェアを装ってWindowsホストを制御](https://thehackernews.com/2026/07/labubarat-masquerades-as-nvidia.html) | 20.0 | 20.0 | 42.0 |
| [画面越しにSWATを煽ったWelsh Doxbin管理者に実刑判決](https://www.theregister.com/security/2026/07/14/welsh-doxbin-admin-jailed-for-egging-on-swatters-from-behind-a-screen/5271281) | 20.0 | 20.0 | 42.0 |
| [米国、国防請負業者向けCMMC第2段階要件を一時停止](https://www.infosecurity-magazine.com/news/us-pentagon-suspends-cmmc-2/) | 20.0 | 20.0 | 42.0 |
| [医療分野はサプライチェーンセキュリティとID管理で継続的な課題に直面している](https://www.cybersecuritydive.com/news/healthcare-cybersecurity-risk-management-identity-fortified/825175/) | 20.0 | 20.0 | 42.0 |
| [エクスプロイトを実行しなくても脆弱性の有無は分かる](https://www.bleepingcomputer.com/news/security/you-dont-have-to-run-an-exploit-to-know-if-youre-vulnerable/) | 20.0 | 20.0 | 42.0 |
| [RabbitMQの脆弱性によりOAuthシークレットが漏えいし、テナント間のキューメタデータが露出する可能性](https://thehackernews.com/2026/07/rabbitmq-flaws-could-leak-oauth-secrets.html) | 20.0 | 20.0 | 42.0 |
| [取締役会の議論は侵害後の生き残りへと移る](https://www.akamai.com/blog/security/2026/jul/podcast-boardroom-conversations-shift-surviving-breach) | 20.0 | 20.0 | 42.0 |
| [Cursor IDE、汚染されたリポジトリ内の悪意あるコードを自動実行してしまう問題](https://www.darkreading.com/application-security/cursor-ide-malicious-code-poisoned-repos) | 20.0 | 20.0 | 42.0 |
| [Microsoft 365アカウントを狙う新たなフィッシングキット、MFAを回避](https://www.bleepingcomputer.com/news/security/new-phishing-kits-target-microsoft-365-accounts-evade-mfa/) | 20.0 | 20.0 | 42.0 |
| [CISA、NSA、FBI、DC3および国際パートナーが警告する、通信・エネルギー・政府など重要インフラを狙うロシアのサイバー脅威活動](https://www.cisa.gov/news-events/news/cisa-joins-nsa-fbi-dc3-and-international-partners-warning-russian-cyber-threat-activity-targeting) | 20.0 | 20.0 | 42.0 |
| [SAPのNetWeaverとCommerce Cloudにおける重大な脆弱性を警告](https://www.bleepingcomputer.com/news/security/sap-warns-of-critical-flaws-in-netweaver-and-commerce-cloud/) | 20.0 | 20.0 | 42.0 |
| [SAP NetWeaver、Approuter、Commerce Cloudの深刻な脆弱性を修正するパッチを公開](https://www.securityweek.com/sap-patches-critical-vulnerabilities-in-netweaver-approuter-commerce-cloud/) | 20.0 | 20.0 | 42.0 |
| [FaceTimeを悪用して銀行口座を空にする詐欺に警告](https://www.malwarebytes.com/blog/news/2026/07/warning-scammers-are-using-facetime-to-empty-bank-accounts) | 20.0 | 20.0 | 42.0 |
| [古いshimがUEFI Secure Bootをどれだけ回避できるかは誰にもわからない](https://www.helpnetsecurity.com/2026/07/14/eset-uefi-secure-boot-bypass/) | 20.0 | 20.0 | 42.0 |
| [Kratos PhaaSが米国とEUを標的に：Microsoft 365アカウント乗っ取りリスクを低減する方法](https://any.run/cybersecurity-blog/kratos-phaas-account-takeover/) | 20.0 | 20.0 | 42.0 |
| [Lidl、第三者のITインシデントで顧客情報漏えいを警告](https://www.itpro.com/security/data-breaches/lidl-data-breach-supermarket-chain-warns-customers-after-third-party-it-incident-exposes-customer-information-heres-what-we-know-so-far) | 20.0 | 20.0 | 42.0 |
| [Lidl、第三者によるデータ侵害を顧客に通知](https://www.infosecurity-magazine.com/news/lidl-notifies-customers-of/) | 20.0 | 20.0 | 42.0 |
| [Valarianが主権インフラ制御レイヤー向けに5000万ドルを調達](https://www.securityweek.com/valarian-raises-50-million-for-sovereign-infrastructure-control-layer/) | 20.0 | 20.0 | 42.0 |
| [100万件超の詐欺電話に関与した詐欺プラットフォーム関連で英5人を起訴](https://www.helpnetsecurity.com/2026/07/14/russian-coms-nca-charges-scam-calls/) | 20.0 | 20.0 | 42.0 |
| [Microsoft Entra IDの認証刷新、2026年9月開始へ](https://www.helpnetsecurity.com/2026/07/14/microsoft-entra-passkey-authentication/) | 20.0 | 20.0 | 42.0 |
| [「Russian Coms」詐欺プラットフォーム事件で5人を起訴](https://www.infosecurity-magazine.com/news/five-charged-in-russian-coms-fraud/) | 20.0 | 20.0 | 42.0 |

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
