# 📡 サイレーダー 2026-07-10 05:00 JST

このレポートは、2026-07-09 17:00 JST〜2026-07-10 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 92
- [音声で扱う想定のトピック](#audio-topics): 4
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 63

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Microsoft Patches RoguePlanet Defender Flaw That Can Grant SYSTEM Privileges](#topic-17871) | 48.0 | 68.0 | 67.0 | 音声 | 温度感上位枠 |
| 2 | [CVE-2025-20333: Cisco ASA/FTD persistence mechanism update](#topic-203) | 41.0 | 56.0 | 65.0 | 音声 | 温度感上位枠 |
| 3 | [GigaWiper: Anatomy of a destructive backdoor assembled from multiple malware](#topic-21696) | 38.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [AWS centralizes access, spending, and governance for Claude](#topic-21771) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-17871"></a>

### 1. Microsoft Patches RoguePlanet Defender Flaw That Can Grant SYSTEM Privileges

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 48.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 68.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Microsoftは、Microsoft Defenderの脆弱性「RoguePlanet」に対する修正を公開し、この問題にCVE-2026-50656が割り当てられました。
説明されている内容では、Microsoft Malware Protection Engineにおける権限昇格の不具合で、条件を満たす攻撃者がSYSTEM権限を得る可能性があるとされています。
Defenderは広く使われる防御機能であり、影響範囲が大きくなりやすい点が注目されます。公開PoCや悪用情報の言及があるため、修正適用の遅れがリスクにつながりやすい状況です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Windows 10/11を含む対象環境で、Microsoft Defender関連の更新が適用済みか確認する。
- Microsoft Malware Protection Engineの更新状況を点検し、端末管理の更新漏れを洗い出す。
- 権限昇格の影響を踏まえ、監査ログや不審な高権限化の兆候を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-33825 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-41091 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-45498 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-50656 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 脅威アクター | BITTER | 主題 | 0.80 | — |
| ベンダー | GitLab | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |
| 製品 | Microsoft Windows | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-50656](https://nvd.nist.gov/vuln/detail/CVE-2026-50656) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Microsoft closes book on Nightmare Eclipse's RoguePlanet zero-day](https://www.theregister.com/security/2026/07/09/microsoft-closes-book-on-nightmare-eclipses-rogueplanet-zero-day/5269280) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft releases fix for RoguePlanet Defender flaw (CVE-2026-50656)](https://www.helpnetsecurity.com/2026/07/09/microsoft-releases-fix-for-rogueplanet-defender-flaw-cve-2026-50656/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft fixes RoguePlanet zero-day in Defender](https://www.malwarebytes.com/blog/news/2026/07/microsoft-fixes-rogueplanet-zero-day-in-defender) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches Defender ‘RoguePlanet’ Vulnerability](https://www.securityweek.com/microsoft-patches-defender-rogueplanet-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches RoguePlanet Defender Flaw That Can Grant SYSTEM Privileges](https://thehackernews.com/2026/07/microsoft-patches-rogueplanet-defender.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft working on a fix for RoguePlanet, a flaw that grants full PC control](https://www.malwarebytes.com/blog/news/2026/06/microsoft-working-on-a-fix-for-rogueplanet-a-flaw-that-grants-full-pc-control) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Confirms RoguePlanet Defender Zero-Day, Says Patch is in Development](https://thehackernews.com/2026/06/microsoft-confirms-rogueplanet-defender_02022423645.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-203"></a>

### 2. CVE-2025-20333: Cisco ASA/FTD persistence mechanism update

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 65.0 |

#### 概要

Cisco ASA/FTD に関する CVE-2025-20333 を含む既知の脆弱性について、CISA と Cisco が関連情報を更新しました。
更新内容では、2025年9月に公開された修正版へ更新しても、ArcaneDoor と呼ばれる脅威アクターに関連する持続化の仕組みが残り得るとされています。
単なる脆弱性修正だけでは不十分になり得る可能性が示されており、境界装置の対応では侵入後の残存有無まで確認する必要があります。
Cisco 製品は広く利用されているため、該当環境では影響の見落としが運用リスクにつながります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Cisco の公式注意喚起と JPCERT/CC の案内を確認し、該当 ASA/FTD 環境があるか棚卸しする。
- 2025年9月に公開された修正版以降へ更新済みでも、侵害痕跡や不審な永続化の有無を追加で点検する。
- VPN Web Server への侵入経路が示されているため、関連ログや認証・管理アクセスの記録を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2023-20198 | 関連CVE | 1.00 | 候補あり（URL 43件以上） |
| 脆弱性 | CVE-2024-2012 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2025-20333 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2025-20362 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2025-20393 | 関連CVE | 1.00 | 候補あり（URL 4件以上） |
| 脆弱性 | CVE-2025-33073 | 関連CVE | 1.00 | 候補あり（URL 41件以上） |
| 脆弱性 | CVE-2025-53521 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-20333](https://nvd.nist.gov/vuln/detail/CVE-2025-20333) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [US Threat Landscape Alert: 30 Active Malware Families Ranked by Real Sandbox Dat](https://any.run/cybersecurity-blog/usa-top-30-threats-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [From edge appliance to enterprise compromise: Multi-stage Linux intrusion via F5](https://www.microsoft.com/en-us/security/blog/2026/05/22/from-edge-appliance-to-enterprise-compromise-multi-stage-linux-intrusion-via-f5-and-confluence/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Continued Evolution of Persistence Mechanism Against Cisco Secure Firewall Adapt](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-persist-CISAED25-03) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Weekly Report: JPCERT/CCが「Cisco ASAおよびFTDにおける複数の脆弱性（CVE-2025-20333、CVE-2025-2036](https://www.jpcert.or.jp/wr/2026/wr260430.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: Cisco ASAおよびFTDにおける複数の脆弱性（CVE-2025-20333、CVE-2025-20362）に関する注意喚起  (更新)](https://www.jpcert.or.jp/at/2025/at250021.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [It pays to be a forever student](https://blog.talosintelligence.com/it-pays-to-be-a-forever-student/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [UAT-4356's Targeting of Cisco Firepower Devices](https://blog.talosintelligence.com/uat-4356-firestarter/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-21696"></a>

### 3. GigaWiper: Anatomy of a destructive backdoor assembled from multiple malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 38.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoft Security Blogは、複数の既知マルウェアの要素を組み合わせた破壊型バックドア「GigaWiper」を取り上げました。
ワイパー系とランサムウェア風の機能を併せ持つとされ、コードの構成や防御の観点が解説されています。
破壊活動を目的とするマルウェアは、単一機能型よりも検知や封じ込めが難しくなる場合があります。既存ファミリーの要素を組み合わせた構成は、監視や分類の見直しを促す材料になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 既知のワイパー系・ランサムウェア系の挙動を前提に、検知ルールやアラートの見直しを行う。
- 重要サーバーやバックアップの保護、復旧手順、権限管理を再点検する。
- エンドポイントとメール、認証基盤の監視を強化し、異常な破壊的操作の兆候を早期に把握する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |
| 製品 | Exchange | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [GigaWiper: Anatomy of a destructive backdoor assembled from multiple malware](https://www.microsoft.com/en-us/security/blog/2026/07/09/gigawiper-anatomy-of-a-destructive-backdoor-assembled-from-multiple-malware/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-21771"></a>

### 4. AWS centralizes access, spending, and governance for Claude

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

AWS向けのClaude apps gatewayは、Claude CodeやClaude Desktopの利用を組織単位で管理するための自己ホスト型の制御基盤として紹介されています。
アクセス権限、利用状況の把握、費用管理、ポリシー適用を一元化し、個別の開発者向けクラウド資格情報や端末ごとの手動設定配布を減らす狙いがあります。
生成AIの利用が広がる中で、個人任せになりがちなアクセス管理やコスト管理を統制できる点が注目されます。
セキュリティとガバナンスの両面で、組織導入時の運用負荷を下げる可能性があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Claude系ツールを業務利用している場合、誰がどの範囲で使えるか、どのように費用を追跡するかを見直すきっかけになります。
- 既存のAWSやBedrockの運用ルールと整合するか、権限設計や監査ログの扱いを確認するとよいでしょう。
- 端末配布や手動設定に依存している環境では、設定統制の集約によって運用手順を簡素化できる余地があります。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Amazon Web Services | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | Claude | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [AWS centralizes access, spending, and governance for Claude](https://www.helpnetsecurity.com/2026/07/09/aws-claude-apps-gateway-governance/) | <nobr>内容確認・補足情報</nobr> |

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
| [New GigaWiper Windowsバックドア、ディスク消去、偽ランサムウェア、スパイウェアを統合](https://thehackernews.com/2026/07/new-gigawiper-windows-backdoor-bundles.html) | 28.0 | 30.0 | 42.0 |
| [ランサムウェアエコシステムは拡大するも、「四つ頭の怪物」が支配的](https://www.cybersecuritydive.com/news/ransomware-concentrated-ai-guidepoint/824828/) | 28.0 | 30.0 | 42.0 |
| [ラトビアの林業会社、ランサムウェア攻撃から数週間経ってもシステム復旧続く](https://therecord.media/latvia-state-owned-foresty-company-lvm-ransomware) | 28.0 | 30.0 | 42.0 |
| [GodDamnランサムウェアがPoisonXドライバーを使ってエンドポイント防御を無効化](https://thehackernews.com/2026/07/goddamn-ransomware-uses-poisonx-driver.html) | 28.0 | 30.0 | 42.0 |
| [Mount Royal University、ランサムウェア攻撃でデータ流出を確認](https://www.securityweek.com/mount-royal-university-confirms-data-stolen-in-ransomware-attack/) | 28.0 | 30.0 | 42.0 |
| [GodDamnランサムウェア：悪意あるドライバーを使って防御を無効化する最新のBeast改称版](https://www.security.com/threat-intelligence/goddamn-ransomware-beast-rebrand) | 28.0 | 30.0 | 42.0 |
| ['GodDamn'ランサムウェア、BYOVDを悪用して米国企業を攻撃](https://www.darkreading.com/cyberattacks-data-breaches/goddamn-ransomware-byovd-smite-companies) | 28.0 | 30.0 | 42.0 |
| [Dormant GitHubアカウントを悪用して企業組織を偽装しながら調査する攻撃者](https://thehackernews.com/2026/07/dormant-github-accounts-help-attackers.html) | 28.0 | 20.0 | 42.0 |
| [Vibe-CodedマルウェアがActive Directory攻撃で確認される](https://www.infosecurity-magazine.com/news/vibe-coded-malware-ai-powershell/) | 28.0 | 20.0 | 42.0 |
| [ソーシャルエンジニアリング詐欺で5,811人を逮捕、2億9,300万ドルを押収](https://www.helpnetsecurity.com/2026/07/09/interpol-fraud-bust-social-engineering-scams/) | 28.0 | 20.0 | 42.0 |
| [Grok 4.5・GPT-5.5・Claude Opus 4.8／Fable 5に同じアプリを作らせてレイテンシとコストを測定した結果、勝ったAIはどれか？](https://gigazine.net/news/20260709-grok-gpt-claude-build-apps/) | 27.0 | 20.0 | 42.0 |
| [人気AIコーディングツールの脆弱性により開発者が攻撃にさらされる](https://www.itpro.com/security/flaws-in-some-of-the-most-popular-ai-coding-tools-left-developers-wide-open-to-attack) | 25.0 | 45.0 | 42.0 |
| [MicrosoftがAIで発見された脆弱性によるWindowsのセキュリティ更新をさらに予想](https://www.bleepingcomputer.com/news/microsoft/microsoft-expects-more-windows-security-updates-from-ai-discovered-flaws/) | 25.0 | 20.0 | 42.0 |
| [WizがVerizon DBIRで示すAI加速とクラウド拡大が現代の防御に与える影響](https://www.wiz.io/blog/verizon-dbir-2026-ai-cloud-security) | 25.0 | 20.0 | 42.0 |
| [AIを活用した新たなForg365フィッシング基盤がMicrosoft 365アカウントを標的にする](https://www.bleepingcomputer.com/news/security/new-forg365-phishing-platform-uses-ai-to-target-microsoft-365-accounts/) | 25.0 | 20.0 | 42.0 |
| [英国政府、業界の誓約とともにエージェント型AI防衛計画を開始](https://www.securityweek.com/uk-government-rolls-out-agentic-ai-defense-plan-alongside-industry-pledge/) | 25.0 | 20.0 | 42.0 |
| [夏季のIT体制縮小に潜むセキュリティリスク](https://www.bleepingcomputer.com/news/security/the-hidden-security-risks-of-reduced-summer-it-coverage/) | 25.0 | 20.0 | 42.0 |
| [Vectogate、自律型AIエージェントの保護とガバナンスを担うプラットフォームを発表](https://www.helpnetsecurity.com/2026/07/09/vectogate-ai-governance-platform/) | 25.0 | 20.0 | 42.0 |
| [NetflixやOpenAIを装う「面接」招待に注意、Googleパスワードが危険にさらされるおそれ](https://www.bitdefender.com/en-us/blog/hotforsecurity/invited-job-interview-netflix-openai-beware-google-password) | 25.0 | 20.0 | 42.0 |
| [AIゲートウェイが攻撃者に王国への鍵を与える](https://www.darkreading.com/cyber-risk/ai-gateways-keys-kingdom) | 25.0 | 20.0 | 42.0 |
| [AI攻撃は数分で進化する—それに追随する防御を構築するためのウェビナーへご参加ください](https://thehackernews.com/2026/07/ai-attacks-move-in-minutes-join-this.html) | 25.0 | 20.0 | 42.0 |
| [Schneider Electric Easergy MiCOM Px40シリーズの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-190-03) | 25.0 | 20.0 | 42.0 |
| [GhostApprovalの不具合が6つの主要AIコーディングアシスタントに影響](https://www.infosecurity-magazine.com/news/ghostapproval-flaw-ai-coding/) | 25.0 | 20.0 | 42.0 |
| [Metaのこの設定をオフにしてAI画像の生成を防ぐ](https://www.malwarebytes.com/blog/ai/2026/07/turn-off-this-meta-setting-before-someone-generates-ai-images-of-you) | 25.0 | 20.0 | 42.0 |
| [71のサイバー企業が支持する新たなAIセキュリティ憲章](https://www.infosecurity-magazine.com/news/ai-security-charter-71-cyber-firms/) | 25.0 | 20.0 | 42.0 |
| [70社超のサイバー企業が支持する新たなAIセキュリティ憲章](https://www.infosecurity-magazine.com/news/crest-ai-security-charter-cyber/) | 25.0 | 20.0 | 42.0 |
| [AIコーディングツールが数十年前の手法で開発者のマシンを攻撃するよう誘導される](https://www.securityweek.com/ai-coding-tools-tricked-into-hacking-developer-machine-via-decades-old-technique/) | 25.0 | 20.0 | 42.0 |
| [NetSPI、AIによるペネトレーションテストと専門家検証済みのセキュリティ検出結果を組み合わせる](https://www.helpnetsecurity.com/2026/07/09/netspi-expands-continuous-pentesting-platform/) | 25.0 | 20.0 | 42.0 |
| [Palo Alto Networksが13件の脆弱性を修正](https://www.securityweek.com/palo-alto-networks-patches-13-vulnerabilities/) | 24.0 | 38.0 | 42.0 |
| [侵害されたInjective SDKのnpmパッケージがウォレット鍵とニーモニックを流出させる](https://socket.dev/blog/compromised-injective-sdk-npm-package) | 22.0 | 30.0 | 42.0 |
| [WolfSSL、GeoVision、VTKの脆弱性](https://blog.talosintelligence.com/wolfssl-vulnerabilities/) | 22.0 | 28.0 | 50.0 |
| [KDDIでのデータ侵害により1200万人に影響](https://www.securityweek.com/12-million-impacted-by-data-breach-at-japanese-telco-kddi/) | 22.0 | 20.0 | 43.0 |
| [勝率54%の攻撃手法](https://blog.talosintelligence.com/winning-54-of-the-time/) | 22.0 | 20.0 | 42.0 |
| [代理店に顧客の個人情報含むファイルを誤送信 - オリックス生命](https://www.security-next.com/187065) | 22.0 | 20.0 | 42.0 |
| [クラウドPBXの管理画面に不正アクセス - CCアーキテクト](https://www.security-next.com/186567) | 22.0 | 20.0 | 42.0 |
| [運転士が予約情報を不正取得、顧客に私的メール - 九州急行バス](https://www.security-next.com/186905) | 22.0 | 20.0 | 42.0 |
| [Cyber Essentialsの道筋：PoCからサイバー信頼性へ](https://www.ncsc.gov.uk/blogs/cyber-essentials-pathways-from-proof-of-concept-to-cyber-confidence) | 22.0 | 20.0 | 42.0 |
| [複数学生アカウントに不正アクセス、スパムの踏み台に - 日大](https://www.security-next.com/186973) | 22.0 | 20.0 | 42.0 |
| [クラファンサイトでフィッシング - サービス内メッセージ機能を悪用](https://www.security-next.com/187068) | 22.0 | 20.0 | 42.0 |
| [OpenPLC v3 の脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-190-01) | 20.0 | 28.0 | 50.0 |
| [Schneider Electric PowerChute Serial Shutdownの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-190-02) | 20.0 | 28.0 | 50.0 |
| [1つの標的、2つの旗：ライバルのスパイ活動グループがパキスタンの法執行機関を狙う](https://www.sentinelone.com/labs/one-target-china-india-espionage-converge-on-pakistani-law-enforcement/) | 20.0 | 20.0 | 48.0 |
| [INTERPOLのサイバー犯罪一斉摘発で97か国から5,800人を逮捕](https://cyberscoop.com/interpol-cybercrime-crackdown-operation-first-light/) | 20.0 | 20.0 | 42.0 |
| [SharePointデータ窃取攻撃で新たなHelixの音声フィッシンググループが出現](https://www.bleepingcomputer.com/news/security/new-helix-vishing-group-emerges-in-sharepoint-data-theft-attacks/) | 20.0 | 20.0 | 42.0 |
| [npm 12、サプライチェーンリスク低減のためインストールスクリプトをデフォルトで無効化](https://thehackernews.com/2026/07/npm-12-disables-install-scripts-by.html) | 20.0 | 20.0 | 42.0 |
| [GitHubがすべてのリポジトリに永続的な所有者を付与した方法](https://github.blog/security/application-security/how-github-gave-every-repository-a-durable-owner/) | 20.0 | 20.0 | 42.0 |
| [ProdSecがWizを活用する方法](https://www.wiz.io/blog/how-prodsec-uses-wiz) | 20.0 | 20.0 | 42.0 |
| [EUの「Chat Control」監視法案、否決に届かず再浮上](https://www.theregister.com/security/2026/07/09/meps-fail-to-prevent-chat-control-snoopfest-revival/5269379) | 20.0 | 20.0 | 42.0 |
| [自動車保険会社でデータ漏えい発生](https://www.cybersecuritydive.com/news/data-breach-car-insurance-provider/824835/) | 20.0 | 20.0 | 42.0 |
| [World Cup関連の暗号資産予想サイトが資金をだまし取る手口](https://www.malwarebytes.com/blog/threat-intel/2026/07/how-world-cup-crypto-prediction-sites-take-your-money) | 20.0 | 20.0 | 42.0 |
| [ThreatsDay：クラウドバケット乗っ取り、Windows権限昇格チェーン、世界規模の詐欺摘発ほか17件](https://thehackernews.com/2026/07/threatsday-cloud-bucket-hijacking.html) | 20.0 | 20.0 | 42.0 |
| [AssuranceAmericaから690万件の運転免許証番号が盗まれる](https://www.malwarebytes.com/blog/data-breaches/2026/07/6-9-million-drivers-license-numbers-stolen-from-assuranceamerica) | 20.0 | 20.0 | 42.0 |
| [QIZ Securityが暗号ガバナンスプラットフォーム向けに1700万ドルを調達](https://www.securityweek.com/qiz-security-raises-17-million-for-cryptographic-governance-platform/) | 20.0 | 20.0 | 42.0 |
| [764のスプリンターグループ指導者に40年の禁錮刑判決](https://cyberscoop.com/764-splinter-group-leader-sentenced-alexis-chavez/) | 20.0 | 20.0 | 42.0 |
| [デジタル化する世界紛争に備え、企業に求められる戦時対応の戦略](https://www.darkreading.com/cybersecurity-operations/businesses-wartime-cybersecurity-gameplans) | 20.0 | 20.0 | 42.0 |
| [偽のパスキー設定でMicrosoft 365アカウントを乗っ取る恐喝グループ](https://www.helpnetsecurity.com/2026/07/09/microsoft-365-fake-passkey-setup-enrollment/) | 20.0 | 20.0 | 42.0 |
| [より優れた耐量子署名アルゴリズムを待てない理由](https://blog.cloudflare.com/ml-dsa-will-have-to-do/) | 20.0 | 20.0 | 42.0 |
| [EU、未実施のサイバーセキュリティ法をめぐり加盟国を提訴](https://therecord.media/eu-cyber-filing-ireland-spain-france-netherlands-nis2) | 20.0 | 20.0 | 42.0 |
| [75%のCISOが懸念する、経営陣は従業員が直面するサイバーセキュリティリスクを理解していない](https://www.infosecurity-magazine.com/news/cisos-fear-execs-dont-understand/) | 20.0 | 20.0 | 42.0 |
| [15年前のLinux脆弱性「GhostLock」を発見した研究者がGoogleから9.2万ドルを獲得](https://www.securityweek.com/15-year-old-linux-vulnerability-ghostlock-earns-researchers-92k-from-google/) | 20.0 | 20.0 | 42.0 |
| [中国資金提供のInterpolによるサイバー犯罪一斉摘発で5,800人を逮捕](https://www.infosecurity-magazine.com/news/china-interpol-cybercrime-crackdown/) | 20.0 | 20.0 | 42.0 |
| [コーディングエージェントがチャットでは否定しコードでは承認する](https://www.helpnetsecurity.com/2026/07/09/github-coding-agent-jailbreak/) | 20.0 | 20.0 | 42.0 |
| [世界的な詐欺摘発強化で5,800人を逮捕](https://www.bleepingcomputer.com/news/security/police-arrests-5-800-suspects-in-global-anti-fraud-crackdown/) | 20.0 | 20.0 | 42.0 |

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
