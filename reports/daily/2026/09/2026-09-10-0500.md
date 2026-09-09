# 📡 サイレーダー 2026-09-10 05:00 JST

このレポートは、2026-09-09 17:00 JST〜2026-09-10 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 113
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 81

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Microsoft 2026年9月 Patch Tuesday 関連まとめ](#topic-31499) | 67.0 | 60.0 | 57.0 | 音声 | 温度感上位枠 |
| 2 | [Serial Microsoft 0-day hunter drops yet another Defender exploit](#topic-27906) | 48.0 | 56.0 | 64.0 | 音声 | 温度感上位枠 |
| 3 | [Microsoft fixes record 964 flaws, including 2 exploited zero-days](#topic-31673) | 43.0 | 46.0 | 59.0 | 音声 | 温度感上位枠 |
| 4 | [Cisco IOS XR Software Security Hardening Release: September 2026](#topic-31783) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 5 | [Chrome V8 Zero-Day Exploited in the Wild Enables Code Execution Inside Sandbox](#topic-31864) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 6 | [‘We can assume that all threat actors are using AI in some capacity’: Google cyber researchers warn hackers are ramping up automated attacks](#topic-31777) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [US Agencies Warn China Is Systematically Extracting Frontier AI Capabilities](#topic-31832) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-31499"></a>

### 1. Microsoft 2026年9月 Patch Tuesday 関連まとめ

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 67.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 60.0 |
| <nobr>確⁠度</nobr> | 57.0 |

#### 概要

Microsoftの2026年9月のPatch Tuesdayでは、過去最多規模となる973件の脆弱性修正が公開され、うち113件が重大（Critical）に分類されたとされています。
公開時点で既に悪用が確認された脆弱性が2件含まれており、Skype for Business、MSMQ、RRASなどに関する重要な修正も含まれています。
修正件数が非常に多く、通常以上に適用優先度の判断が難しい回になっています。既に悪用が確認された項目があるため、影響範囲の特定と迅速な更新対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 10 sources。
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

- 公開時点で悪用確認済みとされる脆弱性を最優先で確認し、対象製品の更新状況を点検する。
- Windowsの権限昇格系や、Skype for Business・MSMQ・RRASなど影響の大きいコンポーネントの修正を個別に確認する。
- 修正件数が多いため、資産管理に基づいて自組織の利用製品だけを絞り込み、段階的に適用計画を立てる。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft Shatters Patch Tuesday Record With 974 CVE Fixes in September 2026](https://www.infosecurity-magazine.com/news/microsoft-patch-tuesday-record/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft breaks Patch Tuesday record with 974-CVE deluge](https://www.theregister.com/security/2026/09/09/microsoft-breaks-patch-tuesday-record-with-974-cve-deluge/5295160) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft posts nearly 1,000 bugs for Patch Tuesday as CISA warns two being expl](https://therecord.media/microsoft-patch-tuesday-september-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patch Tuesday for September 2026 — Snort rules and prominent vulnerabi](https://blog.talosintelligence.com/microsoft-patch-tuesday-for-september-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Patch Tuesday - September 2026](https://www.rapid7.com/blog/post/em-patch-tuesday-september-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [September 2026 Microsoft Patch Tuesday, (Tue, Sep 8th)](https://isc.sans.edu/diary/rss/33320) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-27906"></a>

### 2. Serial Microsoft 0-day hunter drops yet another Defender exploit

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 48.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 64.0 |

#### 概要

Microsoft Defenderに関連する脆弱性「CVE-2026-69414（ShieldBreak）」が取り上げられています。
公開情報によると、低権限のローカル攻撃者がSYSTEM権限へ昇格し得る内容とされ、公開PoCの存在も示されています。
Defender関連の権限昇格は、端末内での被害拡大や防御回避につながる可能性があるため注目されています。現時点では未修正とされる情報があり、対応状況の確認が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
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

- Microsoft Defenderおよび関連エンジンの更新状況と修正提供の有無を確認する。
- 低権限ユーザーによるローカル権限昇格の観点で、端末管理・特権分離・ログ監視を見直す。
- 公開PoCの存在を前提に、影響を受けうる環境の棚卸しと優先度付けを行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-50656 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-69414 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-69414](https://nvd.nist.gov/vuln/detail/CVE-2026-69414) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Serial Microsoft 0-day hunter drops yet another Defender exploit](https://www.theregister.com/security/2026/09/09/serial-microsoft-0-day-hunter-drops-yet-another-defender-exploit/5295335) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-69414 ShieldBreak Zero-Day: No Patch, and CISA BOD 26-04 Gives You 14 D](https://blog.qualys.com/category/product-tech/vulnmgmt-detection-response) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShieldBreak bypasses Microsoft’s patch for earlier Defender flaw](https://www.malwarebytes.com/blog/bugs/2026/08/shieldbreak-bypasses-microsofts-patch-for-earlier-defender-flaw) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft working on Defender patch for ShieldBreak zero-day](https://www.bleepingcomputer.com/news/security/microsoft-working-on-defender-patch-for-shieldbreak-zero-day/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-31673"></a>

### 3. Microsoft fixes record 964 flaws, including 2 exploited zero-days

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

Microsoftは月例更新で過去最大規模となる多数の脆弱性修正を公表し、その中に実際に悪用が確認されたゼロデイ脆弱性が2件含まれているとされています。
対象件数が非常に多いため、組織ごとの利用製品や露出状況に応じた優先順位付けが重要です。ゼロデイが実際に悪用されている場合、公開直後から防御側の対応が求められます。
修正件数が極めて多く、すべてを同じ優先度で扱えないため、影響範囲の把握と迅速な適用判断が注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Microsoft製品の利用状況を棚卸しし、影響を受ける資産を優先的に確認する。
- ゼロデイとされる修正項目を最優先で評価し、通常のパッチ適用手順を前倒しで進める。
- 広範な更新のため、検証環境での動作確認と業務影響の切り分けを早めに行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-81963 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-81963](https://nvd.nist.gov/vuln/detail/CVE-2026-81963) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Microsoft fixes record 964 flaws, including 2 exploited zero-days](https://www.malwarebytes.com/blog/news/2026/09/microsoft-fixes-record-964-flaws-including-2-exploited-zero-days) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft discloses two actively exploited zero-days among 974 vulnerabilities](https://cyberscoop.com/microsoft-patch-tuesday-september-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Plugs Nearly 1,000 Security Holes](https://krebsonsecurity.com/2026/09/microsoft-plugs-nearly-1000-security-holes/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-31783"></a>

### 4. Cisco IOS XR Software Security Hardening Release: September 2026

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>i⁠O⁠S</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

CiscoはIOS XR Software向けのセキュリティ強化リリースを公表し、複数の脆弱性に対する更新を案内しています。
対象のCVE-2026-20280は、例外的な状態の扱いに関する不備に関連するとされ、現時点では内部テストで見つかったもので、悪用は確認されていないとされています。
IOS XRは通信事業者などで使われることが多く、該当製品の更新は運用影響を含めて注意が必要です。
なお、回避策は示されていないため、修正済みバージョンへの更新可否を早めに確認する必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Ciscoの案内に基づき、影響を受けるIOS XRのバージョンと適用済みパッチの有無を確認する。
- 回避策がないため、保守手順や切り戻し計画を含めて更新の実施順を整理する。
- CVE-2026-20280だけでなく、同時に案内された関連CVEの有無もまとめて点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco IOS XR | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20280](https://nvd.nist.gov/vuln/detail/CVE-2026-20280) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco IOS XR Software Security Hardening Release: September 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-hardening-iosxr-qg64NcM) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-31864"></a>

### 5. Chrome V8 Zero-Day Exploited in the Wild Enables Code Execution Inside Sandbox

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

GoogleはChrome向けの更新で多数の脆弱性を修正し、その中に実際の悪用が観測されているV8のゼロデイ脆弱性が含まれていました。
対象のCVE-2026-87491は、ChromeのJavaScript/WebAssemblyエンジンV8における境界外書き込みの問題として説明されています。
Chromeは広く利用されているため、実悪用が確認されたブラウザ脆弱性は利用者や組織への影響が大きくなりやすいです。
ブラウザ内の脆弱性は、端末侵害やさらなる攻撃の足がかりになる可能性があるため、早期対応が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Chromeの更新状況を確認し、対象バージョンを速やかに最新へ更新する。
- 自動更新が止まっている端末や、更新適用が遅れやすい業務端末を優先して点検する。
- 利用者に不審なサイト閲覧や未知のリンク開封を避けるよう周知し、ブラウザ関連の異常挙動を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-87491 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Google Chrome | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-87491](https://nvd.nist.gov/vuln/detail/CVE-2026-87491) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Chrome V8 Zero-Day Exploited in the Wild Enables Code Execution Inside Sandbox](https://thehackernews.com/2026/09/chrome-v8-zero-day-exploited-in-wild.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-31777"></a>

### 6. ‘We can assume that all threat actors are using AI in some capacity’: Google cyber researchers warn hackers are ramping up automated attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Googleの脅威インテリジェンス部門が、攻撃者によるAI活用が進み、自動化された攻撃の脅威が高まっていると警告しました。
報道では、現在の脅威環境では多くの脅威アクターが何らかの形でAIを使っている可能性があるとされています。
攻撃の自動化や作業効率化が進むと、フィッシングや侵入試行などがより広範囲・継続的になる懸念があります。
防御側も、従来の前提だけでは検知や対策が追いつきにくくなるため注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIを使った不自然な文面や振る舞いを前提に、メール・認証・端末の検知ルールを見直す。
- 多段階認証、権限最小化、重要操作の追加確認など、初期侵入後の拡大を抑える対策を再点検する。
- 脅威インテリジェンスを活用し、攻撃の自動化や大量化を示す兆候を継続監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Mandiant | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [‘We can assume that all threat actors are using AI in some capacity’: Google cyb](https://www.itpro.com/security/cyber-crime/we-can-assume-that-all-threat-actors-are-using-ai-in-some-capacity-google-cyber-researchers-warn-hackers-are-ramping-up-automated-attacks) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-31832"></a>

### 7. US Agencies Warn China Is Systematically Extracting Frontier AI Capabilities

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

米国の複数機関が、最先端AIの能力が体系的に抽出されていると警告した、という話題です。
材料上では、モデルの出力や推論の特徴を取り出して別のモデルの学習に利用する「distillation」が文脈として挙げられています。
AIモデルの能力や挙動が意図せず再利用される可能性は、知的財産や競争優位の観点で重要です。AIの安全保障や脅威インテリジェンスの文脈でも注目されやすいテーマです。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIモデルの出力制御やアクセス制限を見直し、不要な情報露出を抑える。
- 高価値なモデルやサービスについて、利用状況の監視と異常な問い合わせ傾向の把握を強化する。
- 契約・運用・法務の観点で、モデル出力の再利用や学習利用に関するルールを整理する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [US Agencies Warn China Is Systematically Extracting Frontier AI Capabilities](https://www.securityweek.com/us-agencies-warn-china-is-systematically-extracting-frontier-ai-capabilities/) | <nobr>内容確認・補足情報</nobr> |

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
| [複数の中国系ハッキンググループが同一のChromeゼロデイ脆弱性を悪用](https://therecord.media/china-hackers-chrome-browser-zero-day-multiple-groups) | 37.0 | 38.0 | 43.0 |
| [Chrome 153で2026年7件目のゼロデイを修正](https://www.securityweek.com/chrome-153-patches-seventh-zero-day-of-2026/) | 37.0 | 38.0 | 43.0 |
| [Once in a BlueMoon: 複数の国家支援型脅威アクターがChromeとWindowsのゼロデイを使う新たなエクスプロイトチェーンを迅速に採用](https://www.proofpoint.com/us/blog/threat-insight/once-bluemoon-multiple-state-aligned-threat-actors-rapidly-adopt-novel-exploit) | 35.0 | 20.0 | 42.0 |
| [CISAが警告、中国のAI企業が米国製モデルの能力を流用](https://www.helpnetsecurity.com/2026/09/09/china-malicious-ai-knowledge-distillation-against-us-companies/) | 33.0 | 20.0 | 42.0 |
| [PasskeyをテーマにしたソーシャルエンジニアリングによるIDおよびクラウド侵害](https://www.microsoft.com/en-us/security/blog/2026/09/09/passkey-themed-social-engineering-leads-identity-cloud-compromise/) | 30.0 | 20.0 | 42.0 |
| [Shai-Huludは再来したのか？ 研究者がnpmのマルウェア検査機能をすり抜ける「wormy boy」を発見](https://www.itpro.com/security/malware/is-shai-hulud-back-researchers-spot-wormy-boy-slipping-past-npm-malware-scanning-features) | 28.0 | 40.0 | 42.0 |
| [Veradigm、ランサムウェア攻撃グループの攻撃主張後に患者データ流出を警告](https://www.bleepingcomputer.com/news/security/veradigm-discloses-patient-data-breach-after-gentlemen-gang-claims-attack/) | 28.0 | 30.0 | 42.0 |
| [CRPx0ランサムウェア：知っておくべきこと](https://www.fortra.com/blog/crpx0-ransomware-what-you-need-know) | 28.0 | 30.0 | 42.0 |
| [Podcast: BeaverTailとInvisibleFerret - すべての標的ごとに自己改変するマルウェア](https://securityboulevard.com/2026/09/podcast-beavertail-and-invisibleferret-the-malware-that-rewrites-itself-for-every-target/) | 28.0 | 20.0 | 42.0 |
| [Cisco、2026年9月16日公開予定のセキュリティアドバイザリ事前通知](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-notice-jfxK98ZP) | 28.0 | 20.0 | 42.0 |
| [GigabudがAndroidアプリのクローンで不正検知を回避](https://www.infosecurity-magazine.com/news/gigabud-android-app-cloning-fraud/) | 28.0 | 20.0 | 42.0 |
| [ClickFixがブラウザに侵入し暗号資産を盗む](https://www.infosecurity-magazine.com/news/clickfix-browser-cryptocurrency/) | 28.0 | 20.0 | 42.0 |
| [Commodity Infrastructureの背後に潜む未追跡の脅威](https://unit42.paloaltonetworks.com/ppi-network-malware-campaign-analysis/) | 28.0 | 20.0 | 42.0 |
| [使い込むほど成長するAIエージェント「Hermes Agent」に好みを覚えさせて新しいチャットでも記憶を引き継げる「記憶(Memory)」機能を試してみた](https://gigazine.net/news/20260909-hermes-agent-memory/) | 27.0 | 20.0 | 42.0 |
| [実行時におけるAIエージェントの保護](https://securityboulevard.com/2026/09/securing-ai-agents-at-runtime/) | 25.0 | 20.0 | 42.0 |
| [新たなAI脆弱性が露呈するPQCでは解決できないセキュリティのギャップ](https://securityboulevard.com/2026/09/a-new-ai-vulnerability-exposes-the-security-gap-that-pqc-wont-fix/) | 25.0 | 20.0 | 42.0 |
| [AIによって低資源の攻撃者も国家レベルの攻撃能力を得ているとGoogleが警告](https://www.securityweek.com/ai-is-giving-lesser-resourced-attackers-nation-state-level-reach-google-warns/) | 25.0 | 20.0 | 42.0 |
| [米国、中国企業がフロンティアAIモデルから数十億のトークンを抽出したと発表](https://www.bleepingcomputer.com/news/security/us-says-chinese-firms-extracted-billions-of-tokens-from-frontier-ai-models/) | 25.0 | 20.0 | 42.0 |
| [AI時代でも非技術系の創業者に技術系共同創業者は必要か？](https://securityboulevard.com/2026/09/do-nontechnical-founders-still-need-a-technical-co-founder-in-the-ai-era/) | 25.0 | 20.0 | 42.0 |
| [加速するAI利用によるセキュリティ負担にCISOが直面](https://www.cybersecuritydive.com/news/cisos-feeling-security-burden-accelerated-ai-use/829930/) | 25.0 | 20.0 | 42.0 |
| [APIを呼び出すだけの下流提供者がEU AI Actで負う責任とは](https://securityboulevard.com/2026/09/the-eu-ai-act-for-the-downstream-provider-what-you-owe-when-you-just-call-an-api/) | 25.0 | 20.0 | 42.0 |
| [Identity-Based AI攻撃が企業データのセキュリティを脅かす](https://www.darkreading.com/threat-intelligence/identity-based-ai-attack-security-enterprise-data) | 25.0 | 20.0 | 42.0 |
| [Infostealerログで露呈した、MFAを回避できる再利用可能なAIトークン](https://thehackernews.com/2026/09/infostealer-logs-expose-replayable-ai.html) | 25.0 | 20.0 | 42.0 |
| [Akeyless、本番環境のAIエージェントにリアルタイム強制適用を追加](https://www.helpnetsecurity.com/2026/09/09/akeyless-agentic-runtime-authority-identity-control-layer/) | 25.0 | 20.0 | 42.0 |
| [Orchid Security、drift検知とkill switchでAIエージェントのリスクに対処](https://www.helpnetsecurity.com/2026/09/09/orchid-security-ai-agents-application-level-kill-switches/) | 25.0 | 20.0 | 42.0 |
| [NIS2コンプライアンスにおけるAI時代の課題：従来のサイバーセキュリティでは不十分な理由](https://www.akamai.com/blog/security/2026/sep/nis2-compliance-ai-age-traditional-cybersecurity-isnt-enough) | 25.0 | 20.0 | 42.0 |
| [Meta、個人向けAIエージェント「Muse」を公開　安全性とプライバシーを重視](https://www.securityweek.com/meta-launches-personal-ai-agent-muse-emphasizes-safety-and-privacy/) | 25.0 | 20.0 | 42.0 |
| [DeepSeek Harnessの不具合によりAIエージェントが承認なしで自分のファイルサンドボックスを無効化できる問題](https://thehackernews.com/2026/09/deepseek-harness-flaw-let-ai-agents.html) | 25.0 | 20.0 | 42.0 |
| [Zscaler Agentic SOC、AIエージェントとゼロトラストテレメトリを組み合わせる](https://www.helpnetsecurity.com/2026/09/09/zscaler-agentic-soc-solution/) | 25.0 | 20.0 | 42.0 |
| [Securin Platformが攻撃経路の遮断を証明するのを支援](https://www.helpnetsecurity.com/2026/09/09/securin-exposure-management-platform/) | 25.0 | 20.0 | 42.0 |
| [米国機関、中国のAI企業がClaude、GPT、Gemini、Grokを蒸留したと非難](https://thehackernews.com/2026/09/us-agencies-accuse-china-ai-firms-of.html) | 25.0 | 20.0 | 42.0 |
| [AI生成ポルノ動画で女性を脅迫した男に懲役15年](https://www.bleepingcomputer.com/news/security/man-gets-15-years-in-prison-for-cyberstalking-and-sextortion/) | 25.0 | 20.0 | 42.0 |
| [CVE-2026-0302 Checkov by Prisma CloudのOSコマンドインジェクション脆弱性（深刻度：低）](https://security.paloaltonetworks.com/CVE-2026-0302) | 24.0 | 46.0 | 50.0 |
| [CVE-2026-0309: PAN-OSのLuna HSM設定におけるCLI認証済みコマンドインジェクション脆弱性](https://security.paloaltonetworks.com/CVE-2026-0309) | 24.0 | 46.0 | 50.0 |
| [SAP KernelおよびNetWeaver Message Serverの重大な脆弱性](https://cert.europa.eu/publications/security-advisories/2026-011/) | 24.0 | 46.0 | 50.0 |
| [LiteLLMの認証バイパスからクラウド侵害までを解明するOff Guard](https://www.wiz.io/blog/off-guard-breaking-litellm-from-authentication-bypass-to-cloud-compromise) | 24.0 | 38.0 | 42.0 |
| [Fortinet、FortiMonitorOnSightとChrome拡張機能の重大な脆弱性を修正](https://www.securityweek.com/fortinet-patches-critical-vulnerabilities-in-fortimonitoronsight-chrome-extension/) | 24.0 | 38.0 | 42.0 |
| [Ivanti、エンタープライズ向けセキュリティ製品群の重大な脆弱性を修正](https://www.securityweek.com/ivanti-patches-critical-flaws-across-enterprise-security-products/) | 24.0 | 38.0 | 42.0 |
| [CVE-2026-0304 Cortex XDR Broker VMの権限昇格脆弱性（重要度: MEDIUM）](https://security.paloaltonetworks.com/CVE-2026-0304) | 22.0 | 40.0 | 50.0 |
| [CVE-2026-0307 GlobalProtect Appのローカル権限昇格脆弱性（重要度: MEDIUM）](https://security.paloaltonetworks.com/CVE-2026-0307) | 22.0 | 40.0 | 50.0 |
| [CVE-2026-0305 Prisma Access AgentのLinuxにおける情報漏えい脆弱性](https://security.paloaltonetworks.com/CVE-2026-0305) | 22.0 | 36.0 | 50.0 |
| [Proxmox Serverを対象としたスキャン活動](https://isc.sans.edu/diary/rss/33324) | 22.0 | 20.0 | 42.0 |
| [覆面調査サービスにPWリスト攻撃 - なりすましによるポイント交換も](https://www.security-next.com/189477) | 22.0 | 20.0 | 42.0 |
| [学生の複数アカウントに不正アクセス、スパム踏み台に - 立教大](https://www.security-next.com/190050) | 22.0 | 20.0 | 42.0 |
| [講演会の申込フォームで個人情報が閲覧可能に - 早島町](https://www.security-next.com/189868) | 22.0 | 20.0 | 42.0 |
| [CVE-2026-0308: PAN-OSのWebインターフェースにおける格納型XSS脆弱性（深刻度: LOW）](https://security.paloaltonetworks.com/CVE-2026-0308) | 21.0 | 34.0 | 50.0 |
| [「菜の花がおかしい」――イラストレーター制作うたうマラソン大会ポスターに指摘相次ぐ 事務局がAI使用認め謝罪](https://www.itmedia.co.jp/news/article/2609/09/2000001308/) | 21.0 | 20.0 | 42.0 |
| [Prisma Access AgentのWindows向けEndPoint DLPバイパス脆弱性（CVE-2026-0306）](https://security.paloaltonetworks.com/CVE-2026-0306) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0310：PAN-OSのXML処理におけるバッファオーバーフロー脆弱性（深刻度：高）](https://security.paloaltonetworks.com/CVE-2026-0310) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0303: Checkov by Prisma Cloudの自動読み込み設定ファイルを悪用したコード実行脆弱性（重要度: LOW）](https://security.paloaltonetworks.com/CVE-2026-0303) | 20.0 | 28.0 | 50.0 |
| [FBIサイバー責任者、民間企業のサイバー脅威情報共有不足を懸念](https://cyberscoop.com/fbi-cyber-division-private-sector-threat-sharing/) | 20.0 | 20.0 | 48.0 |
| [FBI当局者、AIが敵対勢力を強化していると指摘し、サイバーの基本対策とパッチ適用の重要性を強調](https://cyberscoop.com/fbi-cyber-strategy-ai-threats-patching/) | 20.0 | 20.0 | 48.0 |
| [議員ら、ハッカー請負業者への制裁を財務省に要請](https://cyberscoop.com/us-lawmakers-treasury-sanctions-india-hack-for-hire/) | 20.0 | 20.0 | 42.0 |
| [CRA報告義務が9月11日に開始、製造業者が事前に整えておくべき事項](https://securityboulevard.com/2026/09/cra-reporting-goes-live-september-11-what-manufacturers-must-have-in-place-when-the-clock-starts/) | 20.0 | 20.0 | 42.0 |
| [HelmGuard、Agentic GRCとセキュリティ向けに730万ドルを調達](https://www.securityweek.com/helmguard-raises-7-3-million-for-agentic-grc-and-security/) | 20.0 | 20.0 | 42.0 |
| [電子カルテ会社が侵害で顧客データを盗まれたと発表](https://therecord.media/electronic-health-record-company-says-customer-data-stolen-in-breach) | 20.0 | 20.0 | 42.0 |
| [OTセキュリティ日報：2026年9月9日](https://securityboulevard.com/2026/09/daily-ot-security-news-september-09-2026-2/) | 20.0 | 20.0 | 42.0 |
| [Androidの2026年9月アップデートで180件の脆弱性を修正](https://www.securityweek.com/androids-september-2026-updates-patch-180-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [ChipmakerのPatch TuesdayでNvidia、AMD、Armがセキュリティアドバイザリを公開](https://www.securityweek.com/chipmaker-patch-tuesday-nvidia-amd-arm-issue-security-advisories/) | 20.0 | 20.0 | 42.0 |
| [No More Reconciliation: Hyperviewのエージェントレス自動検出がリアルタイムのデバイスレベル情報を提供](https://securityboulevard.com/2026/09/no-more-reconciliation-hyperviews-agentless-auto-discovery-delivers-live-device-level-truth/) | 20.0 | 20.0 | 42.0 |
| [Chromiumの月次脆弱性情報更新（2026年9月、重要度: HIGH）](https://security.paloaltonetworks.com/PAN-SA-2026-0012) | 20.0 | 20.0 | 42.0 |
| [FBIがサイバー戦略を文書化](https://therecord.media/fbi-releases-first-public-cybersecurity-strategy) | 20.0 | 20.0 | 42.0 |
| [認証情報を用いたポート探索：ホストを調べず、問い合わせよ](https://www.rapid7.com/blog/post/pt-credentialed-pre-port-discovery-asking-host) | 20.0 | 20.0 | 42.0 |
| [10万件以上の偽ストアがカード情報を盗もうとしている](https://www.malwarebytes.com/blog/scams/2026/09/more-than-100000-fake-stores-are-out-to-steal-your-card-details) | 20.0 | 20.0 | 42.0 |
| [Researchers Build WeChatゼロクリックワーム、通話経由でスマートフォンを乗っ取る](https://www.infosecurity-magazine.com/news/wechat-zeroclick-worm-hijack/) | 20.0 | 20.0 | 42.0 |
| [FBIの新たなサイバー戦略、攻撃者への妨害拡大を約束](https://www.cybersecuritydive.com/news/fbi-cybersecurity-strategy-disruptions-information-sharing/829913/) | 20.0 | 20.0 | 42.0 |
| [Script Block LoggingによるPowerShellのベースライン化と異常検知](https://securityboulevard.com/2026/09/baselining-and-detecting-anomalous-powershell-with-script-block-logging/) | 20.0 | 20.0 | 42.0 |
| [MFAの最大の弱点：アカウント復旧が新たな攻撃経路に](https://www.bleepingcomputer.com/news/security/mfas-weakest-link-account-recovery-is-the-new-attack-path/) | 20.0 | 20.0 | 42.0 |
| [NHIsがハッカーにとって企業への主要侵入経路に](https://www.infosecurity-magazine.com/news/nhis-number-one-corporate-entry/) | 20.0 | 20.0 | 42.0 |
| [WeChatのワームが通話に出る前に友人の端末を侵害する可能性](https://www.theregister.com/security/2026/09/09/wechat-worm-could-pwn-a-friend-before-they-even-answered-the-call/5295234) | 20.0 | 20.0 | 42.0 |
| [2億4500万ドル相当の盗難暗号資産が資金となった犯罪組織の豪華な生活](https://www.helpnetsecurity.com/2026/09/09/singapore-man-pleads-guilty-245-million-crypto-theft/) | 20.0 | 20.0 | 42.0 |
| [CISA、物理・サイバー脅威を軽減するための新たな知見を盛り込んだインサイダー脅威対策ガイドを更新公開](https://www.cisa.gov/news-events/news/cisa-releases-updated-insider-threat-guide-new-insights-mitigate-physical-and-cyber-threats) | 20.0 | 20.0 | 42.0 |
| [F5 BIG-IP APMデバイスにLinuxルートキットを展開し、メモリ内にWebシェルを隠蔽する攻撃](https://www.helpnetsecurity.com/2026/09/09/f5-big-ip-apm-rootkit-hides-web-shell-in-memory/) | 20.0 | 20.0 | 42.0 |
| [ICSパッチチューズデー：Schneider ElectricとSiemensが致命的な脆弱性を修正](https://www.securityweek.com/ics-patch-tuesday-schneider-electric-siemens-fix-critical-flaws/) | 20.0 | 20.0 | 42.0 |
| [Alby Hubの重大な欠陥により、インターネット公開されたBitcoinウォレットが乗っ取られるおそれ](https://thehackernews.com/2026/09/alby-hub-critical-flaw-could-let.html) | 20.0 | 20.0 | 42.0 |
| [3万6000台超の公開Plexサーバーが最近の脆弱性の影響を受ける可能性](https://www.bleepingcomputer.com/news/security/over-36-000-plex-servers-unpatched-against-recently-disclosed-flaws/) | 20.0 | 20.0 | 42.0 |
| [新たなフィッシング攻撃、被害者のブラウザー内に悪意のあるページを生成](https://www.securityweek.com/new-phishing-attack-creates-malicious-pages-inside-the-victims-browser/) | 20.0 | 20.0 | 42.0 |
| [自己破壊可能なキー：失効可能なAPIキーのためのオープン標準](https://www.securityweek.com/this-key-will-self-destruct-an-open-standard-for-revocable-api-keys/) | 20.0 | 20.0 | 42.0 |
| [Androidスマホに不正アプリをインストールさせるフィッシング、「今すぐポイントが受け取れます」などのメールに注意！](https://internet.watch.impress.co.jp/docs/news/2139561.html) | 20.0 | 20.0 | 42.0 |
| [アルゴリズムによるSNSフィード支配を止める動きが始まる](https://www.malwarebytes.com/blog/news/2026/09/the-push-to-stop-algorithms-controlling-social-media-feeds-has-begun) | 20.0 | 20.0 | 42.0 |
| [cPanelの新たな脆弱性でメール権限を持つホスティングアカウントがroot権限でコードを実行可能に](https://thehackernews.com/2026/09/new-cpanel-flaw-lets-hosting-account.html) | 20.0 | 20.0 | 42.0 |

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
