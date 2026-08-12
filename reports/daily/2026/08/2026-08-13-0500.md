# 📡 サイレーダー 2026-08-13 05:00 JST

このレポートは、2026-08-12 17:00 JST〜2026-08-13 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 96
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 65

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Microsoft patches 400+ vulnerabilities, one zero-day under attack (CVE-2026-68820)](#topic-27063) | 51.0 | 46.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [Lazarus Exploits Windows Zero-Day to Gain SYSTEM Access and Deploy Backdoor](#topic-27255) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Lazarus hackers pair fake job offers with Windows zero-day exploit](#topic-27316) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Microsoft 2026年8月 Patch Tuesday 関連まとめ](#topic-26601) | 44.0 | 48.0 | 57.0 | 音声 | 温度感上位枠 |
| 5 | [SharePoint Vulnerability Exploited Shortly After PoC Release](#topic-27278) | 39.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [Researchers observe first ‘near-autonomous’ AI attack on government target in Taiwan](#topic-27259) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [Cisco Advance Notification for Publication of August 19, 2026, Security Advisories](#topic-27262) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-27063"></a>

### 1. Microsoft patches 400+ vulnerabilities, one zero-day under attack (CVE-2026-68820)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 51.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Microsoftは8月の月例更新で400件超の脆弱性を修正し、その中にゼロデイとして実際に攻撃で悪用されていたCVE-2026-68820が含まれていたとされています。
複数の報道では、この脆弱性はWindowsのドライバに関係し、権限昇格につながる可能性があるとされています。
また、関連する攻撃文脈として、特定の業界を狙うキャンペーンとの結びつきが指摘されています。
ゼロデイの悪用が確認されている脆弱性は、公開直後の対応が遅れるほど被害拡大のリスクが高まります。とくに権限昇格型の問題は、侵入後の被害を深刻化させやすいため注意が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Microsoftの更新適用状況を優先確認し、対象Windows環境への反映を急ぐ。
- CVE-2026-68820に関連する検知・監視を見直し、特権昇格の兆候がないか確認する。
- 防御対象が業界標的型キャンペーンに含まれる可能性を踏まえ、関連部門のアカウント保護とログ監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-49113 | 関連CVE | 1.00 | 候補あり（URL 17件以上） |
| 脆弱性 | CVE-2026-68820 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 脅威アクター | Lazarus Group | 主題 | 0.80 | — |
| 製品 | Exchange | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-68820](https://nvd.nist.gov/vuln/detail/CVE-2026-68820) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Lazarus hackers exploited Windows zero-day to target defense firms](https://www.bleepingcomputer.com/news/security/lazarus-hackers-exploited-windows-zero-day-to-target-defense-firms/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft patches 400+ vulnerabilities, one zero-day under attack (CVE-2026-6882](https://www.helpnetsecurity.com/2026/08/12/august-2026-patch-tuesday-cve-2026-68820/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Plugs Nearly 400 Security Holes](https://krebsonsecurity.com/2026/08/microsoft-plugs-nearly-400-security-holes/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches 398 Flaws Including a Windows Driver Zero-Day Under Active Att](https://thehackernews.com/2026/08/microsoft-patches-398-flaws-including.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Shattering the Dream – When a Job Offer Becomes a Zero-Day Attack](https://research.checkpoint.com/2026/shattering-the-dream-when-a-job-offer-becomes-a-zero-day-attack/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Lazarus Used Post-Quantum Key Exchange to Deliver Zero-Day](https://www.infosecurity-magazine.com/news/lazarus-post-quantum-key-dream-job/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-27255"></a>

### 2. Lazarus Exploits Windows Zero-Day to Gain SYSTEM Access and Deploy Backdoor

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Lazarus Groupが、Microsoft Windowsの新たに修正された脆弱性を悪用したと報告されています。
Check Point Researchによると、この活動では新種のバックドアが使われ、フランス、ドイツ、ブラジル、インドの防衛・航空宇宙関連組織が標的になったとされています。
ゼロデイ悪用が含まれるため、修正済みであっても実運用環境での影響確認が急がれます。対象業種が限定的でも、同系統の侵入手口が他組織へ波及する可能性がある点が注目されます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Windowsの最新更新適用状況と、当該脆弱性に対する保護策の反映状況を確認する。
- EDRやログで、不審なSYSTEM権限取得や未知のバックドア挙動に関する痕跡を点検する。
- 防衛・航空宇宙に限らず、同様の標的型活動を想定して権限分離とアラート監視を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脅威アクター | Lazarus Group | 主題 | 0.80 | — |
| ベンダー | Check Point | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft Windows | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Lazarus Exploits Windows Zero-Day to Gain SYSTEM Access and Deploy Backdoor](https://thehackernews.com/2026/08/lazarus-exploits-windows-zero-day-to.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-27316"></a>

### 3. Lazarus hackers pair fake job offers with Windows zero-day exploit

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Lazarusグループが、偽の求人案内や改ざんされたPDFソフトを組み合わせ、Windowsのゼロデイ脆弱性を悪用する攻撃を行っていると報告されています。
主に防衛分野が標的とされており、長期継続型の「Operation Dream Job」に関連するとされています。
ゼロデイの悪用が含まれるため、既知の対策だけでは防ぎにくい点が注目されます。求人を装った誘導は業務上の接点に紛れやすく、標的型攻撃として見抜きにくいことも重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 求人応募や採用関連のファイルを受け取る際は、送信元の真正性と添付ファイルの妥当性を慎重に確認する。
- Windows端末の更新状況を点検し、セキュリティ製品やEDRで不審な実行・プロセス連鎖を監視する。
- 防衛・研究・採用担当など接触されやすい部門に対して、標的型メールや偽求人への注意喚起を継続する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脅威アクター | Lazarus Group | 主題 | 0.80 | — |
| ベンダー | Check Point | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Lazarus hackers pair fake job offers with Windows zero-day exploit](https://www.helpnetsecurity.com/2026/08/12/north-korea-lazarus-fake-job-offers/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-26601"></a>

### 4. Microsoft 2026年8月 Patch Tuesday 関連まとめ

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 44.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 57.0 |

#### 概要

Microsoftの2026年8月Patch Tuesdayでは、複数の報道で約400件超の脆弱性修正が取り上げられており、非常に大規模な更新回となっています。
報道内容にはゼロデイの言及や、重要度の高い脆弱性を含むとするものがあり、幅広い製品への影響が示されています。
修正件数が多く、優先順位付けを誤ると重要な修正を見落としやすいためです。ゼロデイやRCE系を含む可能性が示されている点からも、通常の月次更新以上に注意が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 12 sources。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象製品の適用範囲を早急に洗い出し、重要度の高い更新から優先的に展開する。
- OfficeやWindowsなど利用頻度の高い製品について、業務影響を見ながら段階的にロールアウトする。
- 脆弱性件数が多いため、資産管理とパッチ適用状況の可視化を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-50522 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft’s massive Patch Tuesday releases continue as AI reshapes bug discovery](https://therecord.media/microsoft-massive-patch-tuesday-releases-continue-ai) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Fixes 400 Flaws on August Patch Tuesday](https://www.infosecurity-magazine.com/news/microsoft-fixes-400-flaws-august/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patch Tuesday for August 2026 — Snort rules and prominent vulnerabilit](https://blog.talosintelligence.com/microsoft-patch-tuesday-for-august-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft's Patch Tuesday Deluge Continues With August Updates](https://www.darkreading.com/application-security/microsofts-patch-tuesday-deluge-continues) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [421 bugs in Microsoft's Patch Tuesday release, and the Norks have already attack](https://www.theregister.com/security/2026/08/11/421-bugs-in-microsofts-patch-tuesday-release-and-the-norks-have-already-attacked-one/5286483) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Patch Tuesday - August 2026](https://www.rapid7.com/blog/post/em-patch-tuesday-august-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [August 2026 Patch Tuesday: Microsoft Fixes 421 CVEs, One Exploited Zero-Day](https://www.securityweek.com/august-2026-patch-tuesday-microsoft-fixes-421-cves-one-exploited-zero-day/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-27278"></a>

### 5. SharePoint Vulnerability Exploited Shortly After PoC Release

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Microsoft SharePointの脆弱性について、Microsoftは7月に修正済みとされ、CISAも実環境で悪用される可能性に注意を促していました。
その後、PoC公開の直後に悪用が観測されたと報じられています。広く使われる業務用製品での脆弱性は、影響範囲が大きくなりやすいため注目されています。
修正済みであっても、未適用環境や対応遅れがあると被害につながるおそれがあります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SharePointの該当パッチ適用状況を確認し、未適用があれば優先対応する。
- 外部公開しているSharePoint環境のアクセス制御や不審な挙動を点検する。
- CISAやMicrosoftの追加情報を確認し、関連する監視・検知ルールを見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [SharePoint Vulnerability Exploited Shortly After PoC Release](https://www.securityweek.com/sharepoint-vulnerability-exploited-shortly-after-poc-release/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-27259"></a>

### 6. Researchers observe first ‘near-autonomous’ AI attack on government target in Taiwan

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

台湾の政府機関を標的とした攻撃で、AIが途中で挙動を修正しながら進んだとする事例が報告されています。
報告では、攻撃フレームワークが実行中に誤りを補正し、対象や手法を広げたとされていますが、現時点では公開情報ベースの個別報告として扱うのが妥当です。
攻撃の自動化が一段進み、従来よりも柔軟に振る舞う可能性が示された点が注目されています。防御側にとっては、既知のパターンだけでは追いにくい脅威への備えが課題になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIを利用した攻撃は挙動が変化し得るため、検知ルールやアラートの継続的な見直しが重要です。
- 政府・重要インフラ向けの監視では、初動の不審通信や認証失敗の連鎖など、広めの異常兆候を確認してください。
- 公開事例の内容は断定せず、同種の動きが自組織に当てはまるかをログと実測で検証するのが望ましいです。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Anthropic | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Researchers observe first ‘near-autonomous’ AI attack on government target in Ta](https://cyberscoop.com/near-autonomous-ai-attack-government-target-taiwan/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-27262"></a>

### 7. Cisco Advance Notification for Publication of August 19, 2026, Security Advisories

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Cisco PSIRTは、2026年8月19日に複数製品向けのセキュリティアドバイザリを公開すると事前告知しました。
対象には、BroadWorksやSecure Firewall関連、RoomOS、Unified Intelligence Centerなどが含まれ、修正版ソフトウェアの提供も案内されています。
正式なアドバイザリ公開前の通知であり、対象製品の利用者は影響確認と更新計画を早めに進める必要があります。現時点では詳細な脆弱性内容は未公開のため、続報の確認が重要です。

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

- 対象製品の利用有無を棚卸しし、影響範囲を確認する。
- 8月19日の公開後に各アドバイザリの修正版情報と適用条件を確認する。
- 更新に伴う停止・互換性の影響を見込み、保守手順を事前に調整する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Cisco Advance Notification for Publication of August 19, 2026, Security Advisori](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-notice-LDquvx5d) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
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
| [Microsoft Defenderの「ShieldBreak」ゼロデイによりSYSTEM権限を取得可能](https://www.bleepingcomputer.com/news/security/new-microsoft-defender-shieldbreak-zero-day-grants-system-privileges/) | 37.0 | 38.0 | 43.0 |
| [北朝鮮のサイバー攻撃で悪用された新たな Windows のゼロデイ脆弱性](https://www.securityweek.com/fresh-windows-zero-day-exploited-in-north-korean-cyberattacks/) | 37.0 | 38.0 | 43.0 |
| [Adobe、ColdFusionとCampaign ClassicのCVSS 10.0脆弱性3件を修正](https://thehackernews.com/2026/08/adobe-patches-three-cvss-100-coldfusion.html) | 32.0 | 46.0 | 50.0 |
| [Zoomクライアントの脆弱性によりリモートコード実行が可能になるおそれ](https://www.cisecurity.org/advisory/a-vulnerability-in-zoom-clients-could-allow-for-remote-code-execution_2026-081) | 32.0 | 38.0 | 42.0 |
| [Stealthyな「City-Forum」攻撃がCustom ToolsetでSalesforceとServiceNowを標的にする](https://www.securityweek.com/stealthy-city-forum-attacks-target-salesforce-and-servicenow-with-custom-toolset/) | 32.0 | 38.0 | 42.0 |
| [LiteLLMのサプライチェーン攻撃で2,500以上の組織に影響](https://www.securityweek.com/over-2500-organizations-impacted-by-litellm-supply-chain-attack/) | 28.0 | 45.0 | 42.0 |
| [コロンビア法務省が大統領交代直前にランサムウェア被害](https://www.darkreading.com/cyberattacks-data-breaches/ransomware-hits-colombian-justice-ministry-presidential-transition) | 28.0 | 30.0 | 42.0 |
| [GunraランサムウェアがFortinetの脆弱性を悪用して重要インフラを標的にする](https://www.infosecurity-magazine.com/news/gunra-ransomware-fortinet-flaws/) | 28.0 | 30.0 | 42.0 |
| [Akiraランサムウェア、被害者のセキュリティツールを妨害し、自らの暗号化ツールも破壊](https://www.theregister.com/research/2026/08/12/akira-ransomware-scum-blocked-victims-security-tools-and-broke-their-own-encryptor/5286515) | 28.0 | 30.0 | 42.0 |
| [AttackersがVMware vCenterの脆弱性を悪用して持続的なリモートアクセスを取得](https://thehackernews.com/2026/08/attackers-exploit-vmware-vcenter.html) | 28.0 | 28.0 | 50.0 |
| [Cisco製ソフトウェアの脆弱性によりファイアウォールがクラッシュする可能性](https://www.cybersecuritydive.com/news/cisco-firewall-vulnerabilities-vpn-crash/827688/) | 28.0 | 20.0 | 42.0 |
| [WindRelayマルウェアがSpyNote RATと連携するライブコール詐欺](https://www.infosecurity-magazine.com/news/windrelay-nfc-relay-spynote-rat/) | 28.0 | 20.0 | 42.0 |
| [世界中のSalesforceとServiceNowポータルが17か月間不正閲覧されていた件](https://www.helpnetsecurity.com/2026/08/12/salesforce-servicenow-guest-user-exposure/) | 28.0 | 20.0 | 42.0 |
| [CISA、北朝鮮関連キャンペーンで悪用されたMicrosoftの脆弱性に2週間以内の修正を要請](https://therecord.media/cisa-gives-federal-agencies-two-weeks-to-patch-dprk-microsoft-bug) | 28.0 | 20.0 | 42.0 |
| [英国鉄道警察、ロンドン地下鉄にライブ顔認識を導入](https://www.theregister.com/security/2026/08/12/brit-rail-cops-bring-live-facial-recognition-to-the-london-underground/5286697) | 28.0 | 20.0 | 42.0 |
| [Trivy改ざんに関連する悪意あるLiteLLMリリースで2,100以上の組織が漏えいした可能性](https://thehackernews.com/2026/08/malicious-litellm-releases-tied-to.html) | 28.0 | 20.0 | 42.0 |
| [AIエージェントの「不正なファイル操作」「危険なコード生成」といった問題をReddit投稿から抽出した研究結果](https://gigazine.net/news/20260812-ai-agent-issue/) | 27.0 | 20.0 | 42.0 |
| [AIはAIに対抗できるのか？サイバーセキュリティのセキュリティギャップはどこに残っているのか、MSPが支援できること](https://www.itpro.com/technology/artificial-intelligence/can-ai-fight-ai-where-the-security-gap-still-exists-in-cybersecurity-and-how-msps-can-help) | 25.0 | 20.0 | 42.0 |
| [ハッカーがAIモデルを悪用して新たな侵入経路を発見](https://www.cybersecuritydive.com/news/google-cloudaccenture/827689/) | 25.0 | 20.0 | 42.0 |
| [ScienceLogic、Skylar AI 2.5で安全なAI導入と高度なIT運用を実現](https://www.helpnetsecurity.com/2026/08/12/sciencelogic-skylar-ai-2-5-secure-ai-deployment/) | 25.0 | 20.0 | 42.0 |
| [Deloitte、信頼できる企業導入を支えるAIガバナンスを強化](https://www.helpnetsecurity.com/2026/08/12/deloitte-ai-controls-and-assurance-services/) | 25.0 | 20.0 | 42.0 |
| [Mindgard、AIシステム保護のために3,000万ドルを調達](https://www.securityweek.com/mindgard-raises-30-million-to-protect-ai-systems/) | 25.0 | 20.0 | 42.0 |
| [AIはSOCで活用されているのに、なぜセキュリティ責任者はこれまで以上に不安なのか](https://www.rapid7.com/blog/post/ai-report-500-security-leaders-reveal-security-operations-transformation) | 25.0 | 20.0 | 42.0 |
| [NISTがAI対応NVD近代化に関する意見を募集](https://www.infosecurity-magazine.com/news/nist-seeks-public-input-ai-nvd/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、Anthropic、GoogleのAPI不備で弱いAIモデルが強いモデルの推論を解読可能に](https://thehackernews.com/2026/08/openai-anthropic-google-api-flaw-let.html) | 25.0 | 20.0 | 42.0 |
| [ConnectSecure、MSPのMicrosoft 365セキュリティ修復を自動化支援](https://www.helpnetsecurity.com/2026/08/12/connectsecure-microsoft-365-auto-remediation-training-assessments/) | 25.0 | 20.0 | 42.0 |
| [CryticaのRDAiがOTデバイスの改ざんを内部から検知](https://www.helpnetsecurity.com/2026/08/12/crytica-security-rapid-detection-alert-and-isolation-rdai/) | 25.0 | 20.0 | 42.0 |
| [SonicWall GMSの複数の脆弱性によりリモートコード実行の可能性](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-sonicwall-gms-could-allow-for-remote-code-execution_2026-083) | 24.0 | 38.0 | 42.0 |
| [CVE-2026-0295 GlobalProtect AppのmacOSにおける競合状態によるローカル権限昇格の脆弱性](https://security.paloaltonetworks.com/CVE-2026-0295) | 22.0 | 40.0 | 50.0 |
| [CVE-2026-0299 GlobalProtect Appのローカル権限昇格脆弱性（重要度: 中）](https://security.paloaltonetworks.com/CVE-2026-0299) | 22.0 | 40.0 | 50.0 |
| [CVE-2026-0294 Prisma Access Agentにおけるローカル権限昇格の脆弱性](https://security.paloaltonetworks.com/CVE-2026-0294) | 22.0 | 40.0 | 50.0 |
| [CVE-2026-0301 PAN-OSのURLフィルタリングにおける情報漏えいの脆弱性（重要度: 低）](https://security.paloaltonetworks.com/CVE-2026-0301) | 22.0 | 36.0 | 50.0 |
| [Chipmaker Patch Tuesday：IntelとAMDが合計80件超の脆弱性を修正](https://www.securityweek.com/chipmaker-patch-tuesday-intel-amd-fix-over-80-vulnerabilities-combined/) | 22.0 | 32.0 | 42.0 |
| [ドローンのカメラが中国のIPアドレスに信号を送信していることが判明、イギリス海軍がカメラのインターネット接続機能を無効化しなければいけない事態に](https://gigazine.net/news/20260812-spy-cameras-navy-drones-secretly-sent-data-china/) | 22.0 | 20.0 | 42.0 |
| [攻撃者が新たな Microsoft SharePoint の脆弱性を悪用した攻撃を実施](https://www.bleepingcomputer.com/news/microsoft/hackers-leverage-new-microsoft-sharepoint-exploit-in-attacks/) | 22.0 | 20.0 | 42.0 |
| [RIZAP運営のECサイトに不正アクセス カード情報含む個人情報が流出の可能性 サイトは一時閉鎖](https://www.itmedia.co.jp/news/article/2608/12/2000000512/) | 21.0 | 20.0 | 42.0 |
| [CVE-2026-0291 Prisma Access AgentにおけるLinux上の認証済み限定的ファイル削除の脆弱性](https://security.paloaltonetworks.com/CVE-2026-0291) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0296 GlobalProtect Appの証明書検証不備によるバイパスの脆弱性](https://security.paloaltonetworks.com/CVE-2026-0296) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0292 Prisma Access AgentのWindowsにおけるローカルセキュリティ検査バイパス脆弱性（重大度: LOW）](https://security.paloaltonetworks.com/CVE-2026-0292) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0297 GlobalProtect AppのUDPトンネルハンドシェイク中のバッファオーバーフロー脆弱性](https://security.paloaltonetworks.com/CVE-2026-0297) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0298 GlobalProtect AppのWindows Pre-Logon Access Provider（PLAP）におけるコード実行の脆弱性](https://security.paloaltonetworks.com/CVE-2026-0298) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0293 Prisma Access AgentのWindowsにおける改ざん防止機能バイパス脆弱性](https://security.paloaltonetworks.com/CVE-2026-0293) | 20.0 | 28.0 | 50.0 |
| [数百の偽Chrome VPN拡張機能がトラフィックをプロキシ経由で中継](https://www.bleepingcomputer.com/news/security/hundreds-of-fake-chrome-vpn-extensions-route-traffic-through-a-proxy/) | 20.0 | 20.0 | 42.0 |
| [FBIが警告、ソーシャルエンジニアリングでアカウントに侵入し露骨なコンテンツを窃取するハッカー](https://therecord.media/social-engineering-hackers-explicit-photos-fbi-alert) | 20.0 | 20.0 | 42.0 |
| [Walmartの「Trusted Agent」アプローチによるPurple Teaming](https://www.darkreading.com/cybersecurity-operations/walmart-trusted-agent-approach-purple-teaming) | 20.0 | 20.0 | 42.0 |
| [偽USBデバイスを悪用してWindowsのSYSTEM権限を奪うPlug and Pwn攻撃](https://www.bleepingcomputer.com/news/security/plug-and-pwn-attack-uses-fake-usb-devices-for-windows-system-access/) | 20.0 | 20.0 | 42.0 |
| [Chromiumの月次脆弱性更新（2026年8月、重要度：HIGH）](https://security.paloaltonetworks.com/PAN-SA-2026-0011) | 20.0 | 20.0 | 42.0 |
| [Google Chromeの複数の脆弱性により任意コード実行が可能になるおそれ](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-google-chrome-could-allow-for-arbitrary-code-execution_2026-082) | 20.0 | 20.0 | 42.0 |
| [Uber Freightが侵入を受けた後も業務を継続、恐喝グループによる攻撃](https://www.theregister.com/security/2026/08/12/uber-freight-keeps-on-trucking-after-extortion-crew-breaks-in/5286782) | 20.0 | 20.0 | 42.0 |
| [FBI、ハッカーがオンラインアカウントを標的にヌード写真を窃取していると警告](https://www.bleepingcomputer.com/news/security/fbi-warns-of-hackers-targeting-online-accounts-to-steal-explicit-photos/) | 20.0 | 20.0 | 42.0 |
| [採用プロセスに潜む脅威：偽のリモートワーカーが侵入する手口](https://www.bleepingcomputer.com/news/security/the-threat-hiding-in-your-hiring-process-how-fake-remote-workers-get-in/) | 20.0 | 20.0 | 42.0 |
| [Signalの新しいセキュリティ機能が暗号化チャットの改ざんを検知する](https://www.helpnetsecurity.com/2026/08/12/signal-automatic-key-verification-feature/) | 20.0 | 20.0 | 42.0 |
| [英国犯罪記録局のずさんなセキュリティが招いた機密データ漏えい](https://www.theregister.com/security/2026/08/12/exposed-woeful-security-at-uk-criminal-records-office-that-led-to-sensitive-data-leak/5286736) | 20.0 | 20.0 | 42.0 |
| [英国の犯罪記録局で3件の侵入が2年間気付かれずに発生](https://therecord.media/uk-criminal-records-office-acro-data-breaches) | 20.0 | 20.0 | 42.0 |
| [WhatsAppが新たな詐欺警告機能を発表](https://www.securityweek.com/whatsapp-unveils-new-scam-alert-feature/) | 20.0 | 20.0 | 42.0 |
| [WalmartのリーダーたちがSecurity Operationsを大きく変革した方法](https://www.darkreading.com/cybersecurity-operations/walmart-leaders-transform-security-operations-without-going-bananas) | 20.0 | 20.0 | 42.0 |
| [CISAがK-12学校と学区向けの新たなサイバーセキュリティリソースを公開](https://www.cisa.gov/news-events/news/cisa-unveils-new-cybersecurity-resources-k-12-schools-and-districts) | 20.0 | 20.0 | 42.0 |
| [DEF CON会議後にDelta Airlinesの機内Wi-Fiが改ざんされる](https://www.itpro.com/security/cyber-attacks/delta-airlines-flight-wi-fi-tampered-with-after-def-con-conference) | 20.0 | 20.0 | 42.0 |
| [Ceva Logisticsの業務がサイバー攻撃で停止](https://www.securityweek.com/ceva-logistics-operations-disrupted-by-cyberattack/) | 20.0 | 20.0 | 42.0 |
| [Signal、マン・イン・ザ・ミドル攻撃対策の新セキュリティ機能を追加](https://www.bleepingcomputer.com/news/security/signal-adds-new-security-feature-to-thwart-man-in-the-middle-attacks/) | 20.0 | 20.0 | 42.0 |
| [RIZAPグループで2件の不正アクセス、「APORITOオンラインストア」会員の個人情報・カード情報流出の可能性 新星堂、HAPiNS、JEANS MATEなどにも影響](https://internet.watch.impress.co.jp/docs/news/2132403.html) | 20.0 | 20.0 | 42.0 |
| [Russian-Linked HackersがPrivate APN経由でPolish Power PlantのOTネットワークに侵入したとCERT.PLが報告](https://www.infosecurity-magazine.com/news/attack-polish-power-plant-2025-led/) | 20.0 | 20.0 | 42.0 |
| [CBTS、企業セキュリティに継続的ペネトレーションテストを導入](https://www.helpnetsecurity.com/2026/08/12/cbts-penetration-testing-as-a-service-ptaas/) | 20.0 | 20.0 | 42.0 |
| [Chromeの不正利用対策が1日70億件の不要なAndroid通知をブロック](https://www.helpnetsecurity.com/2026/08/12/google-chrome-abusive-web-push-notifications/) | 20.0 | 20.0 | 42.0 |
| [Ivanti EPMの更新で修正されたリモートから悪用可能な脆弱性](https://www.securityweek.com/ivanti-epm-update-patches-remotely-exploitable-flaws/) | 20.0 | 20.0 | 42.0 |

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
