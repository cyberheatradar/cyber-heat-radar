# 📡 サイレーダー 2026-10-10 05:00 JST

このレポートは、2026-10-09 17:00 JST〜2026-10-10 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 88
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 58

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Unpatched AhsayCBS Vulnerabilities Exploited in the Wild](#topic-36850) | 51.0 | 46.0 | 55.0 | 音声 | 温度感上位枠 |
| 2 | [CVE-2015-3306: CISA KEV catalog addition](#topic-36852) | 45.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 3 | [China Linked Warlock Ransomware Campaign Targets Critical Infrastructure](#topic-36827) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [In Other News: AI Used in Korean Bank Breaches, Poem-Guided Botnet, Empire Admin Gets 40 Years](#topic-36857) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 5 | [Max severity SonicWall SMA1000 flaw now exploited in attacks](#topic-36416) | 32.0 | 64.0 | 55.0 | 音声 | 温度感上位枠 |
| 6 | [Citrix Patches Critical NetScaler Flaw That Could Enable RCE in SAML Deployments](#topic-36752) | 30.0 | 46.0 | 58.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-36850"></a>

### 1. Unpatched AhsayCBS Vulnerabilities Exploited in the Wild

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 51.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

AhsayCBSの未修正脆弱性が、実際の攻撃で悪用されていると報じられています。
少なくとも認証回避につながる不備が含まれており、影響を受けた環境ではWebシェルの設置や仮想通貨マイナーの配置につながった可能性が示されています。
バックアップ製品は重要データや管理権限に近いため、侵害されると横展開や復旧妨害につながりやすい点が懸念されます。
公開済みの欠陥がすでに悪用されているため、単なる脆弱性情報ではなく、優先度の高い対応対象として見られています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AhsayCBSを利用している場合は、該当バージョンの影響有無を確認し、ベンダーの修正情報を早急に適用する。
- バックアップサーバーの管理画面や関連ログを確認し、不審な認証失敗・成功、予期しないファイル配置、コマンド実行の痕跡がないか点検する。
- バックアップ製品をインターネットから直接公開している構成を見直し、アクセス制御と監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-105133 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-105133](https://nvd.nist.gov/vuln/detail/CVE-2026-105133) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit AhsayCBS Flaws to Deploy XMRig Miners Disguised as Microsoft E](https://thehackernews.com/2026/10/attackers-exploit-ahsaycbs-flaws-to.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Unpatched AhsayCBS Vulnerabilities Exploited in the Wild](https://www.securityweek.com/unpatched-ahsaycbs-vulnerabilities-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-36852"></a>

### 2. CVE-2015-3306: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>K⁠E⁠V</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

CISAはCVE-2015-3306をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
公開情報では、この脆弱性はProFTPDの不適切なアクセス制御に関係し、実際の悪用が観測された文脈で扱われています。
KEV入りは、単なる理論上の脆弱性ではなく、実際に攻撃で使われた可能性があることを示す重要なシグナルです。
対象製品を運用している組織では、優先度を上げて対応計画を見直す必要があります。

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

- ProFTPDの導入有無と影響範囲を確認し、該当バージョンの棚卸しを急ぐ。
- KEV掲載を踏まえ、通常の脆弱性優先度より高く扱って修正・緩和策を検討する。
- 関連ログや外向き通信の異常がないかを確認し、侵害兆候の有無を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2015-3306 | 関連CVE | 1.00 | 候補あり（URL 15件以上） |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2015-3306](https://nvd.nist.gov/vuln/detail/CVE-2015-3306) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Flax Typhoon Exploits Five Flaws as CISA Sets October 11 Deadline for Federal Ag](https://thehackernews.com/2026/10/flax-typhoon-exploits-five-flaws-as.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-36827"></a>

### 3. China Linked Warlock Ransomware Campaign Targets Critical Infrastructure

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>通⁠信⁠基⁠盤</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報では、Warlockランサムウェアに関連するキャンペーンが、重要インフラ分野を含む複数の組織を対象にしていたとされています。
対象分野としては水道、通信、政府、教育が挙げられ、地域は欧州、アフリカ、ラテンアメリカに及ぶとされています。
重要インフラや公共性の高い組織が含まれているため、業務停止や広範な影響につながる可能性がある点が注目されます。
攻撃主体や関連グループの分析は、同種の脅威に対する監視や防御の優先度付けに役立ちます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 重要インフラや公共機関を含む組織では、バックアップ、復旧手順、権限管理の見直しを優先する。
- ランサムウェアの侵入経路になりやすい認証情報の保護、MFAの徹底、外部公開資産の棚卸しを進める。
- 地域や業種をまたぐ類似事案として捉え、検知ルールやインシデント対応手順を継続的に点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [China Linked Warlock Ransomware Campaign Targets Critical Infrastructure](https://blog.polyswarm.io/china-linked-warlock-ransomware-campaign-targets-critical-infrastructure) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-36857"></a>

### 4. In Other News: AI Used in Korean Bank Breaches, Poem-Guided Botnet, Empire Admin Gets 40 Years

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報のまとめでは、韓国の銀行向け侵害にAIが使われた可能性や、詩を使って制御するボットネットに関する話題など、複数のサイバー関連ニュースが取り上げられています。
同時に、npm SDKの侵害やEmpire Market関係者の長期刑、NVIDIA GPU監視情報の露出といった別件も含まれており、広く脅威動向を把握する材料になっています。
AIの悪用や自動化された攻撃手法は、攻撃の効率化や検知の難しさにつながるため注視が必要です。
あわせて、サプライチェーンや周辺システムの情報露出も、実務上のリスク評価に影響します。

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

- AIを使った攻撃の話題は、手口の新規性よりも「自動化・適応化」の傾向として整理して共有する。
- npmなどの開発基盤に関する侵害情報は、依存関係の更新や配布物の検証を改めて確認するきっかけにする。
- GPU監視や運用系の可視化データの露出は、機密性の高いテレメトリや管理画面の公開範囲を点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [In Other News: AI Used in Korean Bank Breaches, Poem-Guided Botnet, Empire Admin](https://www.securityweek.com/in-other-news-ai-used-in-korean-bank-breaches-poem-guided-botnet-empire-admin-gets-40-years/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-36416"></a>

### 5. Max severity SonicWall SMA1000 flaw now exploited in attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 32.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

SonicWallのSMA1000シリーズに見つかったCVE-2026-102255を含む複数の脆弱性について、パッチ適用後に攻撃で悪用されているとの報道があります。
対象の脆弱性は、未認証の攻撃者が機器に内部向けの要求を送らせ、内部機能に पहुंचく可能性があるとされています。
境界機器の脆弱性は、組織内部への足がかりになりやすいため注目されます。今回は高深刻度とされ、悪用観測の文脈があることから、早期の対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SonicWallの公開情報を確認し、SMA1000シリーズの該当パッチ適用状況を点検する。
- インターネット公開されている管理・リモートアクセス系機器について、不要な露出がないか確認する。
- 侵害の兆候がないか、認証ログや通信ログなど関連ログを重点的に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-102255 | 関連CVE | 1.00 | 未確認 |
| ベンダー | SonicWall | 言及あり | 0.80 | — |
| 製品 | SonicWall SMA | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-102255](https://nvd.nist.gov/vuln/detail/CVE-2026-102255) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Max severity SonicWall SMA1000 flaw now exploited in attacks](https://www.bleepingcomputer.com/news/security/max-severity-sonicwall-sma1000-flaw-now-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall fixes pre-auth SSRF flaw in SMA 1000 appliances (CVE-2026-102255)](https://www.helpnetsecurity.com/2026/10/07/sonicwall-fixes-pre-auth-ssrf-flaw-in-sma-1000-appliances-cve-2026-102255/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-36752"></a>

### 6. Citrix Patches Critical NetScaler Flaw That Could Enable RCE in SAML Deployments

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>R⁠C⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>D⁠D⁠o⁠S</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 58.0 |

#### 概要

Citrixは、NetScaler ADCおよびNetScaler Gatewayに影響する重大な脆弱性CVE-2026-107406について修正を公開しました。
公開情報によると、この問題は特定の構成条件下でリモートコード実行やサービス停止につながる可能性があります。
認証やSAML関連の利用環境を含むネットワーク機器で影響しうるため、境界防御やリモートアクセス基盤に直結する点が注目されています。
CVE付きで複数ソースが報じており、早期対応が求められる種類の脆弱性です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- NetScaler ADC / Gateway の該当バージョンと構成を確認し、Citrixの修正版適用可否を早急に判断する。
- SAML利用など影響条件に該当する環境を優先して棚卸しし、外部公開面のリスク評価を行う。
- 修正までの間はアクセス制御、監視強化、ベンダー案内の暫定対策の有無を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-107406 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-107406](https://nvd.nist.gov/vuln/detail/CVE-2026-107406) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Citrix gives NetScaler admins another critical reason to patch](https://www.theregister.com/security/2026/10/09/citrix-gives-netscaler-admins-another-critical-reason-to-patch/5302212) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix Patches Critical NetScaler Flaw That Could Enable RCE in SAML Deployments](https://thehackernews.com/2026/10/citrix-patches-critical-netscaler-flaw.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix Urges Immediate Patching of Critical NetScaler Vulnerability](https://www.securityweek.com/citrix-urges-immediate-patching-of-critical-netscaler-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix warns admins to patch new NetScaler RCE flaw immediately](https://www.bleepingcomputer.com/news/security/citrix-warns-admins-to-patch-new-netscaler-rce-flaw-immediately/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [「NetScaler ADC/Gateway」に深刻なRCE脆弱性 - SAML構成に影響](https://www.security-next.com/191276) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [A Vulnerability in Citrix NetScaler ADC and Citrix NetScaler Gateway Could Allow](https://www.cisecurity.org/advisory/a-vulnerability-in-citrix-netscaler-adc-and-citrix-netscaler-gateway-could-allow-for-remote-code-execution_2026-110) | <nobr>内容確認・補足情報</nobr> |

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
| [「お前たちのクラウドはわれわれのもの」 IDCFクラウドの管理画面に出た攻撃者のメッセージ 内容に運営元は](https://www.itmedia.co.jp/news/article/2610/09/2000002184/) | 29.0 | 30.0 | 42.0 |
| [日本、Qilin関係者のロシア人逮捕を確認しドイツへ引き渡しへ](https://therecord.media/japan-germany-ransomware-arrest) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア関連の法執行・司法措置](https://www.bleepingcomputer.com/news/security/germany-arrests-alleged-core-qilin-ransomware-member-after-extradition/) | 28.0 | 30.0 | 42.0 |
| [2026年第3四半期、ランサムウェア攻撃が過去最多を記録](https://www.infosecurity-magazine.com/news/q3-new-record-ransomware/) | 28.0 | 30.0 | 42.0 |
| [FBI、中国関連のボットネットに関連するドメインを押収](https://www.cybersecuritydive.com/news/fbi-seizes-domains-china-botnet-flax-typhoon/832611/) | 28.0 | 20.0 | 48.0 |
| [未修正のAhsayCBS脆弱性が悪用され、webshell設置と暗号資産マイニングに利用される](https://www.bleepingcomputer.com/news/security/unpatched-ahsaycbs-flaws-exploited-to-deploy-webshells-mine-crypto/) | 28.0 | 20.0 | 42.0 |
| [150カ国以上の低価格Android端末を狙うプリインストール型ファームウェアマルウェア](https://www.securityweek.com/pre-baked-firmware-malware-hits-budget-android-devices-in-150-countries/) | 28.0 | 20.0 | 42.0 |
| [米国、中国政府支援のハッキングツールを妨害](https://www.securityweek.com/us-disrupts-chinese-state-sponsored-hacking-tools/) | 28.0 | 20.0 | 42.0 |
| [arXivがAI生成の大量低品質投稿を受けて著者へのレート制限を導入](https://socket.dev/blog/arxiv-rate-limiting-slop) | 27.0 | 20.0 | 42.0 |
| [山中で遭難の16歳少年、登山計画に生成AI「Claude」利用 救助隊は「ルートの妄信」警鐘](https://www.itmedia.co.jp/news/article/2610/09/2000002179/) | 26.0 | 20.0 | 42.0 |
| [Wikimediaが不正なAIエージェントによるプラットフォーム悪用を報告](https://www.infosecurity-magazine.com/news/wikimedia-confirms-platforms-rogue/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントの権限を適切に維持する方法](https://www.bleepingcomputer.com/news/security/how-to-keep-ai-agents-within-their-permissions/) | 25.0 | 20.0 | 42.0 |
| [OpenAIがChatGPTを悪用したロシアとイランの影響工作を阻止したと発表](https://therecord.media/openai-disrupts-russian-iranian-operations-chatgpt) | 25.0 | 20.0 | 42.0 |
| [Social Engineering AI Agents：2026年の新たなBEC脅威](https://www.darkreading.com/cybersecurity-operations/social-engineering-ai-agents-bec-2026) | 25.0 | 20.0 | 42.0 |
| [Anthropic、オープンソース向け無料AI脆弱性スキャナーを提供開始](https://thehackernews.com/2026/10/anthropic-launches-free-ai.html) | 25.0 | 20.0 | 42.0 |
| [フロンティアモデルの暴走を受け、大学がAIサイバーセキュリティ教育を強化](https://www.cybersecuritydive.com/news/ai-cybersecurity-education-university/832132/) | 25.0 | 20.0 | 42.0 |
| [AIの速度の逆説：セキュリティはなぜAIの野心に何十年も遅れているのか](https://thehackernews.com/2026/10/the-ai-velocity-paradox-why-security-is.html) | 25.0 | 20.0 | 42.0 |
| [Anthropic、オープンソース保守者向けに無料のAIセキュリティスキャンを提供](https://www.helpnetsecurity.com/2026/10/09/anthropic-oss-scanner-ai-security-scans/) | 25.0 | 20.0 | 42.0 |
| [AIトレーニングの重要性が高まるガバナンス上の課題](https://www.infosecurity-magazine.com/news/ai-training-critical-as-governance/) | 25.0 | 20.0 | 42.0 |
| [AI「Claude」への虐待行為 禁止](https://news.yahoo.co.jp/pickup/6598146?source=rss) | 25.0 | 20.0 | 42.0 |
| [Anthropic、AIによるバグ報告をOSSメンテナーへ迅速送付　OTセキュリティで11社と連携](https://www.securityweek.com/anthropic-fast-tracks-ai-bug-reports-to-oss-maintainers-taps-11-firms-for-ot-security/) | 25.0 | 20.0 | 42.0 |
| [Researchersが公開したAnyDesk Linuxの未認証脆弱性の実用的な攻撃コード、root権限取得が可能](https://thehackernews.com/2026/10/researchers-publish-working-exploit-for.html) | 24.0 | 38.0 | 42.0 |
| [会員管理システムに不正アクセス、個人情報が流出 - ブックオフ](https://www.security-next.com/191255) | 22.0 | 20.0 | 42.0 |
| [委託業務で個人情報を誤送付、操作ミスで - TOPPAN](https://www.security-next.com/190839) | 22.0 | 20.0 | 42.0 |
| [納税プレゼントキャンペーンのアンケートで不備、個人情報閲覧可能に - 鴨川市](https://www.security-next.com/190959) | 22.0 | 20.0 | 42.0 |
| [Hundreds of Reposを狙う新たなGhostAction攻撃、CI/CDシークレットからクラウド認証情報へ拡大](https://socket.dev/blog/ghostaction-cloud-credentials) | 22.0 | 20.0 | 42.0 |
| [ローソンIDと予約サービスに不正アクセス- 個人情報が流出](https://www.security-next.com/191245) | 22.0 | 20.0 | 42.0 |
| [システムに不正アクセス、顧客への不審メールで判明 - アバハウス](https://www.security-next.com/190998) | 22.0 | 20.0 | 42.0 |
| [APIゲートウェイ製品「IBM DataPower Gateway」に複数脆弱性](https://www.security-next.com/191271) | 22.0 | 20.0 | 42.0 |
| [ヤマハ・スズキも漏えいか 交流サイト基盤「コミューン」不正アクセス、計30万会員に影響の恐れ](https://www.itmedia.co.jp/news/article/2610/09/2000002178/) | 21.0 | 20.0 | 42.0 |
| [NewsPicks、メアド32.3万件やクレカ情報の一部36.2万件漏えいか【訂正あり】](https://www.itmedia.co.jp/news/article/2610/09/2000002175/) | 21.0 | 20.0 | 42.0 |
| [韓国の銀行狙ったサイバー攻撃、犯人は「中国在住の26歳」か Claudeで作られた“履歴書”から浮上](https://www.itmedia.co.jp/news/article/2610/09/2000002176/) | 21.0 | 20.0 | 42.0 |
| [政府が相次ぐ情報漏洩に注意喚起、委託先の管理も要請](https://xtech.nikkei.com/atcl/nxt/news/24/03421/) | 21.0 | 20.0 | 42.0 |
| [NVIDIAの高深刻度脆弱性、認証不要の攻撃者によるGPU監視機能のクラッシュを許す](https://www.helpnetsecurity.com/2026/10/09/nvidia-dcgm-exporter-vulnerability-cve-2026-47483/) | 20.0 | 46.0 | 54.0 |
| [FBIが世界規模のサイバー攻撃で使用されたFlax Typhoonのハッキングツールを破壊](https://www.helpnetsecurity.com/2026/10/09/fbi-flax-typhoon-microscan-fishhub-domains/) | 20.0 | 20.0 | 48.0 |
| [FBI、ShinyHuntersの別の容疑者を逮捕――Jobs Portal侵害への関与が報じられる](https://thehackernews.com/2026/10/fbi-arrests-another-shinyhunters.html) | 20.0 | 20.0 | 42.0 |
| [FBIがShinyHuntersに反撃した見逃しポイント](https://www.darkreading.com/identity-access-management-security/fbi-shinyhunters-claims-hack) | 20.0 | 20.0 | 42.0 |
| [FBI、ShinyHuntersによる機関侵害後に別の容疑者を逮捕](https://www.bleepingcomputer.com/news/security/fbi-arrests-another-suspected-shinyhunters-hacker-after-agency-breach/) | 20.0 | 20.0 | 42.0 |
| [P7 DarkSword iOS Exploit Kitに暗号資産ウォレットデータ窃取とリモートコマンド機能を追加](https://thehackernews.com/2026/10/p7-darksword-ios-exploit-kit-adds.html) | 20.0 | 20.0 | 42.0 |
| [役員本人だけでなく家族にも必要なセキュリティ教育](https://www.darkreading.com/cyber-risk/security-threats-don-t-stop-at-the-office-why-executives-families-need-training-too) | 20.0 | 20.0 | 42.0 |
| [バイオセンサー企業iRhythmのデータ侵害で数十万人に影響](https://therecord.media/irhythm-data-breach-reports) | 20.0 | 20.0 | 42.0 |
| [広範なマネーミュール組織の首謀者がサイバー犯罪収益のマネーロンダリングで有罪を認める](https://therecord.media/leader-of-money-mule-operation-for-cybercriminals-pleads-guilty) | 20.0 | 20.0 | 42.0 |
| [データ侵害に対応してFBIがShinyHuntersの別件逮捕を発表](https://therecord.media/shinyhunters-arrest-fbi-data-breach-investigation) | 20.0 | 20.0 | 42.0 |
| [中国のHafniumハッカー、Microsoft Exchange Server大規模攻撃で10万ドルの懸賞金対象に](https://www.bitdefender.com/en-us/blog/hotforsecurity/10-million-bounty-chinese-hafnium-hacker-microsoft-exchange-server-mega-attack) | 20.0 | 20.0 | 42.0 |
| [TP-Link、ルーターのセキュリティと中国との関係をめぐり米4州から追加提訴される](https://thehackernews.com/2026/10/tp-link-sued-by-four-more-us-states.html) | 20.0 | 20.0 | 42.0 |
| [個人情報巡る対策 政府が緊急要請](https://news.yahoo.co.jp/pickup/6598186?source=rss) | 20.0 | 20.0 | 42.0 |
| [コミュニティサービス「Commune」「Commune for Work」に不正アクセス、推計約30万人の個人情報が漏えい ヤマハ、スズキ、湖池屋、青森県など、多くのコミュニティサイトに影響](https://internet.watch.impress.co.jp/docs/news/2147291.html) | 20.0 | 20.0 | 42.0 |
| [Google Domainsに影響した最近のccTLDハイジャック](https://www.securityweek.com/google-domains-impacted-by-recent-cctld-domain-hijacks/) | 20.0 | 20.0 | 42.0 |
| [サイバー犯罪者向けに1万5000人のマネー・ミュール網を運営した男が認める](https://www.bleepingcomputer.com/news/security/ukrainian-russian-dual-citizen-admits-to-laundering-millions-for-cybercriminals/) | 20.0 | 20.0 | 42.0 |
| [ASOSの侵害に関する最新情報：ハッカーが顧客情報と検索履歴を窃取](https://www.malwarebytes.com/blog/data-breaches/2026/10/asos-breach-update-hackers-stole-customer-details-and-shopping-searches) | 20.0 | 20.0 | 42.0 |
| [Microsoft: 古いWindowsデバイスはセキュリティ更新プログラムの配信を停止へ](https://www.bleepingcomputer.com/news/microsoft/microsoft-outdated-windows-devices-will-lose-security-protection-next-year/) | 20.0 | 20.0 | 42.0 |
| [UKおよび同盟国がChinaのIntegrity Technology Groupによるサイバー脅威に警告](https://www.infosecurity-magazine.com/news/uk-allies-threat-china-integrity/) | 20.0 | 20.0 | 42.0 |
| [中国政府支援のハッカーが使用していた脆弱性スキャンおよびスピアフィッシングツールを米国が押収](https://www.itpro.com/security/cyber-crime/us-seizes-vulnerability-scanning-and-spear-phishing-tools-used-by-china-sponsored-hackers) | 20.0 | 20.0 | 42.0 |
| [GoBalanceの脆弱性によりTor形式の鍵を復元して.onionアドレスを乗っ取れる問題](https://thehackernews.com/2026/10/gobalance-flaw-lets-attackers-hijack.html) | 20.0 | 20.0 | 42.0 |
| [SimpleLoginでメールアドレスをエイリアスで非公開にする方法](https://www.helpnetsecurity.com/2026/10/09/product-showcase-simplelogin/) | 20.0 | 20.0 | 42.0 |
| [国家サイバー統括室、「もはや情報システム部門だけの問題ではありません」と不正アクセス事案を踏まえ注意喚起 IPA、総務省、経産省、金融庁も注意喚起を実施](https://internet.watch.impress.co.jp/docs/news/2147162.html) | 20.0 | 20.0 | 42.0 |
| [Pwn2Ownで3チームがGoogle Pixel 10を完全修正済みの状態から遠隔ハックを実演](https://thehackernews.com/2026/10/three-teams-demonstrate-remote-hacks-of.html) | 20.0 | 20.0 | 42.0 |
| [JR東、「えきねっと」などで漏えいか メルアドなど最大206万件 IDCFクラウドへの不正アクセスで](https://www.itmedia.co.jp/news/article/2610/09/2000002171/) | 16.0 | 20.0 | 42.0 |

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
