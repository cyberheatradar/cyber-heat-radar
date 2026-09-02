# 📡 サイレーダー 2026-09-03 05:00 JST

このレポートは、2026-09-02 17:00 JST〜2026-09-03 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 97
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 66

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [SonicWall SMA 1000 appliances under attack via zero-day flaws](#topic-30622) | 59.0 | 74.0 | 60.0 | 音声 | 温度感上位枠 |
| 2 | [Hackers exploit critical JFrog Artifactory flaw to forge admin tokens](#topic-30390) | 55.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 3 | [CISA Adds Seven Known Exploited Vulnerabilities to Catalog](#topic-30663) | 49.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Cisco IOS XR Software Security Hardening Release: September 2026](#topic-30627) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 5 | [SonicWall's SMA1000 boxes under active attack again](#topic-30625) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [AI agents carried out every step of this ransomware attack – then left the victim an 80-page security audit](#topic-30617) | 33.0 | 30.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-30622"></a>

### 1. SonicWall SMA 1000 appliances under attack via zero-day flaws

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 59.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 60.0 |

#### 概要

SonicWallは、SMA1000アプライアンスに影響する2件の脆弱性について公表し、実際に悪用が確認されているとしています。
1件は認証前のSSRF、もう1件は管理機能に関するコマンドインジェクションで、組み合わせると未認証でのリモートコード実行につながる可能性があるとされています。
SMA1000はネットワーク境界に置かれることが多く、外部公開されやすい構成では影響が大きくなり得ます。公開後に悪用が広がる前提で、早急な更新と侵害有無の確認が求められます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象バージョンのSMA1000を使っている場合は、SonicWallが案内する修正版プラットフォームホットフィックスへの更新を優先する。
- 単純なパッチ適用だけでなく、すでに侵害されていないかをログやベンダー案内に沿って確認する。
- 侵害の兆候があれば、再イメージングや再展開、パスワード変更、TOTPトークンの再設定を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-83548 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-83549 | 関連CVE | 1.00 | 未確認 |
| ベンダー | SonicWall | 言及あり | 0.80 | — |
| 製品 | SonicWall SMA | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-83548](https://nvd.nist.gov/vuln/detail/CVE-2026-83548) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Critical SonicWall SMA1000 Vulnerabilities CVE-2026-83548, CVE-2026-83549 Exploi](https://www.rapid7.com/blog/post/etr-critical-sonicwall-sma1000-vulnerabilities-cve-2026-83548-cve-2026-83549-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit Two SonicWall SMA 1000 Zero-Days That May Form an Attack Chain](https://thehackernews.com/2026/09/attackers-exploit-two-sonicwall-sma.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [SonicWall SMA 1000 appliances under attack via zero-day flaws](https://www.helpnetsecurity.com/2026/09/02/sonicwall-sma-1000-cve-2026-83548-cve-2026-83549-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-30390"></a>

### 2. Hackers exploit critical JFrog Artifactory flaw to forge admin tokens

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 55.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

JFrog Artifactoryに存在する認証バイパスの脆弱性CVE-2026-82329について、公開後まもなく実際の悪用が観測されたと報じられています。
影響を受ける環境では、管理者権限につながるトークンが不正に作成される可能性があるとされています。
Artifact管理基盤が侵害されると、ソフトウェア供給網や内部リポジトリへの影響が広がり得るため、優先度の高い対応対象です。
既に悪用観測がある点から、修正適用の遅れがそのままリスクにつながります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
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

- JFrogの案内に従い、影響範囲のあるArtifactoryインスタンスを早急に確認し、修正版への更新を優先する。
- 管理者権限やトークン周りの不審な作成・利用、想定外の認証成功がないか監査ログを点検する。
- 外部公開されている管理系エンドポイントを見直し、必要最小限のアクセスに制限する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-82329 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | watchTowr | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-82329](https://nvd.nist.gov/vuln/detail/CVE-2026-82329) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Hackers exploit critical JFrog Artifactory flaw to forge admin tokens](https://www.bleepingcomputer.com/news/security/hackers-exploit-critical-jfrog-artifactory-flaw-to-forge-admin-tokens/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Pounce on Critical Artifactory Bug Following Disclosure](https://www.darkreading.com/application-security/attackers-pounce-critical-artifactory-flaw-disclosure) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit Critical JFrog Artifactory Flaw to Mint Admin Tokens Days Afte](https://thehackernews.com/2026/09/attackers-exploit-critical-jfrog.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical JFrog Artifactory Vulnerability Reportedly Exploited in the Wild](https://www.securityweek.com/critical-jfrog-artifactory-vulnerability-reportedly-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-30663"></a>

### 3. CISA Adds Seven Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 49.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、実際に悪用されている証拠があるとして、Known Exploited Vulnerabilities（KEV）カタログに7件の脆弱性を新たに追加しました。
対象には、Sangoma Switchvox、Starlette、Kestra OSS、BerriAI LiteLLM、JFrog Artifactory、SonicWall SMA1000に関する脆弱性が含まれています。
KEVへの追加は、これらの脆弱性が机上の懸念ではなく、優先的な対応が必要な状態にあることを示します。
公開系システムや認証周りに関わるものが含まれるため、影響範囲の確認と迅速な修正が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当製品の利用有無を確認し、インターネット公開資産を優先して影響調査を行う。
- ベンダーやCISAの修正情報を確認し、パッチ適用や緩和策を早急に進める。
- 適用前に侵害の兆候がないかログや設定変更履歴を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | SonicWall | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Seven Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/09/02/cisa-adds-seven-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-30627"></a>

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

Cisco IOS XR Software向けに、2026年9月のセキュリティ強化リリースが案内されています。
Ciscoによる内部テストで見つかった複数の脆弱性に対応する更新で、現時点では活発な悪用は確認されていないとされています。
対象がネットワーク機器向けOSのため、更新の遅れが運用機器の防御力低下につながる可能性があります。
なお、対処策としてはソフトウェア更新が示されており、代替の回避策は案内されていません。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Cisco IOS XRの影響有無を資産棚卸しで確認し、該当する場合は優先度を上げて更新計画に入れる。
- 複数の脆弱性がまとめて修正されているため、関連CVEを個別ではなく一括で管理・追跡する。
- 回避策がないため、適用前後のメンテナンス手順や障害時の切り戻し計画を事前に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco IOS XR | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20274](https://nvd.nist.gov/vuln/detail/CVE-2026-20274) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco IOS XR Software Security Hardening Release: September 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-hardening-iosxr-qg64NcM) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-30625"></a>

### 5. SonicWall's SMA1000 boxes under active attack again

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

SonicWallのSMA1000製品に対して、再び実際の攻撃が確認されているとされています。
材料では、複数のゼロデイ脆弱性が関与した可能性が示されており、今後も追加の攻撃が起きる可能性が高いとみられています。
SMA1000はリモートアクセス基盤として使われることがあり、侵害されると社内ネットワークへの影響が広がりやすい点が懸念されます。
ゼロデイを含む実悪用の文脈であるため、未対策の環境では早急な確認が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SonicWall SMA1000の利用有無を確認し、ベンダー告知や緊急パッチ情報を追う。
- 公開範囲の制限、不要な外部公開の停止、管理系アクセスの制御を見直す。
- 認証失敗や不審な管理操作、予期しない設定変更などの兆候を重点監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-15409 | 関連CVE | 1.00 | 候補あり（URL 5件以上） |
| 脆弱性 | CVE-2026-83548 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-83549 | 関連CVE | 1.00 | 未確認 |
| ベンダー | SonicWall | 言及あり | 0.80 | — |
| 製品 | SonicWall SMA | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [SonicWall's SMA1000 boxes under active attack again](https://www.theregister.com/security/2026/09/02/sonicwalls-sma1000-boxes-under-active-attack-again/5293969) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-30617"></a>

### 6. AI agents carried out every step of this ransomware attack – then left the victim an 80-page security audit

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、AIエージェントがランサムウェア攻撃の各段階に関与したとされ、攻撃後には被害者向けに80ページのセキュリティ監査レポートが残されたと伝えられています。
現時点の材料では、個別の技術的詳細や被害規模は限定的で、報道ベースの話題として扱うのが適切です。AIが攻撃の自動化にどう使われ得るかを示す事例として注目されます。
防御側にとっては、従来のマルウェア検知だけでなく、AIを使った多段階の不審挙動を想定した監視が重要になるためです。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIを利用した攻撃は、偵察・侵入・横展開・情報整理など複数工程が連動する前提でログを確認する。
- 被害後の分析や説明文書が精緻でも、正当な監査ではない可能性を踏まえ、内容の真偽を検証する。
- AI利用の有無にかかわらず、認証強化、権限の最小化、バックアップの隔離など基本対策の徹底が重要。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [AI agents carried out every step of this ransomware attack – then left the victi](https://www.theregister.com/security/2026/09/02/ai-agents-carried-out-every-step-of-this-ransomware-attack-then-left-the-victim-an-80-page-security-audit/5294009) | <nobr>内容確認・補足情報</nobr> |

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
| [ハッカーが2件の新たなSonicWallゼロデイ脆弱性を連鎖利用](https://www.infosecurity-magazine.com/news/hackers-chain-sonicwall-zeroday/) | 37.0 | 38.0 | 43.0 |
| [約2万2000台のMicrosoft Exchangeサーバーが重大な脆弱性（CVE-2026-62911）に引き続き露出](https://www.helpnetsecurity.com/2026/09/02/microsoft-exchange-cve-2026-62911-critical-authentication-bypass-flaw/) | 32.0 | 46.0 | 50.0 |
| [親ウクライナの新たなハッカー集団がロシア企業をカスタムランサムウェアで標的に](https://therecord.media/new-pro-ukraine-hacker-group-custom-ransomware-russia) | 28.0 | 30.0 | 42.0 |
| [MSP向けランサムウェア対策：迅速な復旧のための6項目チェックリスト](https://www.bleepingcomputer.com/news/security/ransomware-protection-for-msps-a-6-point-checklist-for-faster-recovery/) | 28.0 | 30.0 | 42.0 |
| [Sangoma Switchvoxの脆弱性（CVE-2026-9586）の悪用が進行中](https://www.helpnetsecurity.com/2026/09/02/exploitation-of-sangoma-switchvox-flaw-underway-cve-2026-9586/) | 28.0 | 28.0 | 50.0 |
| [80,000人のフリーランスを感染させたマルウェアキャンペーンでロシア人国籍の男に20年の刑の可能性](https://therecord.media/russian-national-facing-20-years-malware-campaign) | 28.0 | 20.0 | 42.0 |
| [23年にわたり稼働したロシア拠点のボットネットが解体](https://cyberscoop.com/sality-botnet-dismantled/) | 28.0 | 20.0 | 42.0 |
| [Threat Gang「Springs」によるMicrosoft Teamsユーザーへのボイスフィッシング攻撃](https://www.darkreading.com/cyberattacks-data-breaches/threat-gang-springs-vishing-attacks-microsoft-teams-users) | 28.0 | 20.0 | 42.0 |
| [偽のソフトウェアインストーラーがWindows Updateを無効化しMicrosoft Defenderを弱体化させる](https://thehackernews.com/2026/09/fake-software-installers-disable.html) | 28.0 | 20.0 | 42.0 |
| [フリーランスを狙ったマルウェア キャンペーンに関与したロシア人が引き渡しへ](https://www.infosecurity-magazine.com/news/russian-man-extradited-malware/) | 28.0 | 20.0 | 42.0 |
| [悪意あるApacheモジュールがブラジル政府サイトの通信を乗っ取り賭博ページへ誘導](https://thehackernews.com/2026/09/malicious-apache-modules-hijack.html) | 28.0 | 20.0 | 42.0 |
| [詐欺師はターゲットの選び方がより巧妙にしています](https://www.malwarebytes.com/blog/scams/2026/09/scammers-are-getting-smarter-about-where-they-target-you) | 28.0 | 20.0 | 42.0 |
| [Meta Adsを悪用してAndroidトロイの木馬「StreamRat」を配信、ほぼ完全な端末制御が可能に](https://thehackernews.com/2026/09/meta-ads-push-streamrat-android-trojan.html) | 28.0 | 20.0 | 42.0 |
| [長期間活動していたボットネットSalityがついに壊滅](https://therecord.media/sality-botnet-cyber-doj) | 28.0 | 20.0 | 42.0 |
| [プレッシャー下でのコミュニケーション：サービスプロバイダーのベストプラクティス](https://www.cisa.gov/resources-tools/resources/communicating-under-pressure-best-practices-service-providers) | 28.0 | 20.0 | 42.0 |
| [BGPハイジャック経由で配信された悪意のあるVirtualizorアップデート](https://www.securityweek.com/malicious-virtualizor-update-served-via-bgp-hijacking/) | 28.0 | 20.0 | 42.0 |
| [中国語話者の攻撃者がブラジル政府サイトをSEO兵器化した手口](https://research.checkpoint.com/2026/gaming-the-system-how-a-chinese-speaking-actor-turned-brazilian-government-sites-into-an-seo-weapon/) | 28.0 | 20.0 | 42.0 |
| [Excelマルウェアキャンペーンで数千台に感染させたロシア人ハッカー、引き渡し後に起訴される](https://thehackernews.com/2026/09/extradited-russian-hacker-faces-charges.html) | 28.0 | 20.0 | 42.0 |
| [米国、マルウェアで8万人のフリーランスを感染させたロシア人を起訴](https://www.bleepingcomputer.com/news/security/us-charges-russian-for-infecting-80-000-freelancers-with-malware/) | 28.0 | 20.0 | 42.0 |
| [Salityボットネットの23年にわたる活動がグローバルなシンクホール作戦で終了](https://www.helpnetsecurity.com/2026/09/02/sality-botnet-disruption-crowdstrike-law-enforcement/) | 28.0 | 20.0 | 42.0 |
| [23年続いたSality P2Pボットネットの摘発](https://www.securityweek.com/23-year-old-sality-p2p-botnet-disrupted/) | 28.0 | 20.0 | 42.0 |
| [Salityボットネットのインフラが国際共同摘発で解体](https://www.bleepingcomputer.com/news/security/sality-botnet-infrastructure-dismantled-in-joint-global-takedown/) | 28.0 | 20.0 | 42.0 |
| [OpenAIのAstra、ゼロデイ発見により「クリティカル」なサイバー閾値を突破](https://www.securityweek.com/openais-astra-becomes-first-model-to-cross-critical-cybersecurity-threshold/) | 27.0 | 20.0 | 43.0 |
| [委託業者が無断でAI利用か――ヨルシカ、ライブ映像上映会のチケットサンプル画像が文字化け デザインにも影響](https://www.itmedia.co.jp/news/article/2609/02/2000001082/) | 26.0 | 20.0 | 42.0 |
| [OpenLeash、危険なAIエージェント操作に人による確認を追加](https://www.securityweek.com/openleash-adds-a-human-check-to-risky-ai-agent-actions/) | 25.0 | 20.0 | 42.0 |
| [悪意ある.git設定によりClaude、Codex、CursorなどのAIエージェントが攻撃者コードを実行する可能性](https://thehackernews.com/2026/09/malicious-git-configs-can-make-claude.html) | 25.0 | 20.0 | 42.0 |
| [Anthropicがセキュリティインシデントへの対応とエンタープライズ向け保護策を公開](https://www.securityweek.com/anthropic-details-response-to-security-incidents-unveils-enterprise-safeguards/) | 25.0 | 20.0 | 42.0 |
| [企業AIを安全に守る方法：導入からインシデント対応準備まで](https://thehackernews.com/2026/09/how-to-secure-enterprise-ai-from.html) | 25.0 | 20.0 | 42.0 |
| [APIキー窃取によりハッカーが60万ドルのAI利用料金を発生させ、数週間誰も気づかずとMETRが発表](https://www.itpro.com/security/cyber-attacks/hackers-ran-up-a-usd600-000-ai-bill-after-swiping-api-keys-says-metr-and-nobody-realized-for-weeks) | 25.0 | 20.0 | 42.0 |
| [AI支援型サイバー攻撃の実態：Unit 42の調査内部記録](https://unit42.paloaltonetworks.com/ai-assisted-cyber-attack-inside-a-unit-42-investigation/) | 25.0 | 20.0 | 42.0 |
| [UKサイバー法案はAI開発事業者ではなく利用者を対象にする](https://www.theregister.com/security/2026/09/02/uk-cyber-bill-targets-ai-users-not-the-vendors-building-it/5293738) | 25.0 | 20.0 | 42.0 |
| [あなたのAIとのチャットが法廷で使われる可能性](https://www.malwarebytes.com/blog/ai/2026/09/your-ai-chats-could-be-used-in-court) | 25.0 | 20.0 | 42.0 |
| [Cisco Nexus 9000 Series Switches Silicon Oneのリモートコード実行の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-n9k-s1-rce-EH8dEtr) | 24.0 | 46.0 | 50.0 |
| [Cisco Desk Phone 9800シリーズ、IP Phone 7800/8800シリーズおよびVideo Phone 8875のSIPソフトウェアにおけるサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-phone-dos-txMYNRzv) | 24.0 | 46.0 | 50.0 |
| [Cisco Secure EmailのS/MIME暗号文復号の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-esa-smime-disc-dzw4rEdY) | 24.0 | 46.0 | 50.0 |
| [WordPressバックアッププラグインの欠陥により数百万サイトが乗っ取り攻撃の危険にさらされる](https://www.bleepingcomputer.com/news/security/wordpress-backup-plugin-flaw-exposes-millions-of-sites-to-takeover-attacks/) | 24.0 | 38.0 | 42.0 |
| [GeoNetworkの政府向けGeoportalバックエンドに影響する未認証RCEチェーンを修正](https://thehackernews.com/2026/09/geonetwork-fixes-unauthenticated-rce.html) | 24.0 | 38.0 | 42.0 |
| [ChromeとFirefoxのアップデートで多数の脆弱性を修正](https://www.securityweek.com/chrome-and-firefox-updates-patch-dozens-of-vulnerabilities/) | 22.0 | 32.0 | 42.0 |
| [システムに不正アクセス、顧客情報が流出 - 01銀行](https://www.security-next.com/189728) | 22.0 | 20.0 | 42.0 |
| [第三者がアプリDBデータを削除、サービスは復旧 - コープやまぐち](https://www.security-next.com/189731) | 22.0 | 20.0 | 42.0 |
| [サイトに脆弱性を突く不正アクセス - 日産財団](https://www.security-next.com/189669) | 22.0 | 20.0 | 42.0 |
| [三井不動産に不正アクセス 社員・社外関係者の情報最大5万5000件漏えいか](https://www.itmedia.co.jp/news/article/2609/02/2000001091/) | 21.0 | 20.0 | 42.0 |
| [NECがAnthropicの「Mythos」利用権、社内の脆弱性管理に活用](https://xtech.nikkei.com/atcl/nxt/news/24/03370/) | 21.0 | 20.0 | 42.0 |
| [ServiceNow、AI時代のセキュリティ「Autonomous Security」発表 - Shift Zeroで脅威ゼロを目指す](https://news.mynavi.jp/techplus/article/20260902-4906071/) | 21.0 | 20.0 | 42.0 |
| [悪意のあるWebサイトでユーザーを危険にさらすChromeの2件の重大な脆弱性](https://www.malwarebytes.com/blog/bugs/2026/09/two-critical-chrome-flaws-put-users-at-risk-on-malicious-websites) | 20.0 | 28.0 | 50.0 |
| [FCC、通信事業者のロボコール対策を消費者が評価できる仕組みを検討](https://cyberscoop.com/the-fcc-wants-consumers-to-rate-their-telecoms-anti-robocall-protections/) | 20.0 | 20.0 | 42.0 |
| [Aesto記録システムから950万人超の健康データが流出](https://therecord.media/health-data-aesto-cyberattack-leak) | 20.0 | 20.0 | 42.0 |
| [テクニカルサポート詐欺は今こう変わった、注意すべき点はこれです](https://www.malwarebytes.com/blog/scams/2026/09/tech-support-scams-look-different-now-heres-what-to-watch-for) | 20.0 | 20.0 | 42.0 |
| [英国、重要インフラから高リスクな技術供給業者を排除へ](https://www.securityweek.com/uk-moves-to-block-high-risk-tech-suppliers-from-critical-infrastructure/) | 20.0 | 20.0 | 42.0 |
| [Serbian activistsの端末で見つかったPegasusとNoviSpy亜種のスパイウェア](https://cyberscoop.com/pegasus-novispy-variant-spyware-found-on-devices-of-serbian-activists/) | 20.0 | 20.0 | 42.0 |
| [Wyden氏、商用VPN利用に関するNSAのセキュリティガイダンス強化を要求](https://cyberscoop.com/wyden-nsa-commercial-vpn-security-guidance/) | 20.0 | 20.0 | 42.0 |
| [Revolutを悪用した詐欺波でJersey住民から4週間で18万ポンドを窃取](https://www.bitdefender.com/en-us/blog/hotforsecurity/revolut-scam-jersey) | 20.0 | 20.0 | 42.0 |
| [旧Lenovoログインにより5,000件のDropboxアカウントが攻撃者に公開された](https://www.theregister.com/security/2026/09/02/legacy-lenovo-login-opens-5000-dropbox-accounts-to-attackers/5293924) | 20.0 | 20.0 | 42.0 |
| [Gambling Goblinがブラジル政府サイトをSEO兵器化](https://www.infosecurity-magazine.com/news/gambling-goblin-brazilian/) | 20.0 | 20.0 | 42.0 |
| [Google Chromeの複数の脆弱性により任意のコードが実行される可能性](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-google-chrome-could-allow-for-arbitrary-code-execution_2026-085) | 20.0 | 20.0 | 42.0 |
| [DNSはHTTPSの中に隠れている――その理由とは](https://www.akamai.com/blog/security/2026/sep/your-dns-hiding-https-why-it-matters) | 20.0 | 20.0 | 42.0 |
| [Rockwell Automation、複数製品にわたる十数件の脆弱性を修正](https://www.securityweek.com/rockwell-automation-patches-over-a-dozen-vulnerabilities-across-products/) | 20.0 | 20.0 | 42.0 |
| [Lenovoのメール認証の不備によりDropboxアカウントが侵害される](https://www.bleepingcomputer.com/news/security/dropbox-accounts-breached-through-lenovo-email-verification-flaw/) | 20.0 | 20.0 | 42.0 |
| [Fresh Cleo Harmonyの脆弱性に対するエクスプロイトが公開される](https://www.securityweek.com/exploit-published-for-fresh-cleo-harmony-vulnerability/) | 20.0 | 20.0 | 42.0 |
| [著名人を狙うOAuthフィッシング攻撃、FBIが警告](https://www.helpnetsecurity.com/2026/09/02/oauth-consent-phishing-fbi-warning/) | 20.0 | 20.0 | 42.0 |
| [Nutex Health、患者データ流出を公表し、ハッカーがリークを予告](https://www.infosecurity-magazine.com/news/nutex-patient-data-stolen/) | 20.0 | 20.0 | 42.0 |
| [Microsoft Defenderが正規のGoogle検索リンクを悪意あるものとして検出](https://www.bleepingcomputer.com/news/security/microsoft-defender-flags-legitimate-google-search-links-as-malicious/) | 20.0 | 20.0 | 42.0 |
| [1億5300万件超の運転免許証が新たなダークウェブプラットフォームで販売中](https://www.malwarebytes.com/blog/news/2026/09/dark-web-site-puts-153-million-drivers-licenses-and-millions-more-ids-up-for-sale) | 20.0 | 20.0 | 42.0 |
| [DLP Network Discover Clusterは常に監視しているので、チームが監視する必要はない](https://www.security.com/product-insights/dlp-network-discover-cluster-always-watching-so-your-team-doesnt-have) | 20.0 | 20.0 | 42.0 |
| [バッテリー蓄電システムへのサイバー攻撃は、調整不良の制御装置そのものに見える](https://www.helpnetsecurity.com/2026/09/02/grid-battery-storage-cyberattack/) | 20.0 | 20.0 | 42.0 |
| [FulcrumSecがManchester Airport Groupへの侵害の責任を主張](https://www.infosecurity-magazine.com/news/fulcrumsec-manchester-airport/) | 20.0 | 20.0 | 42.0 |

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
