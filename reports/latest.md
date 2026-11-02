# 📡 サイレーダー 2026-11-03 05:00 JST

このレポートは、2026-11-02 17:00 JST〜2026-11-03 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 103
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 73

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Over 1,000 GitLab servers vulnerable to ongoing RCE attacks](#topic-40935) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [CVE-2026-111357: CISA KEV catalog addition](#topic-40747) | 40.0 | 67.0 | 59.0 | 音声 | 温度感上位枠 |
| 3 | [Ivanti patches two more Connect Secure zero-days chained in attacks](#topic-40966) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Shutting the Door on the XCPE Botnet](#topic-40917) | 33.0 | 45.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [AI-powered infostealer picks out the most profitable parts of your stolen data](#topic-40903) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 6 | [Government Linux Servers Targeted With SysGoRAT and Suspected AI-Generated Scripts](#topic-40954) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-40935"></a>

### 1. Over 1,000 GitLab servers vulnerable to ongoing RCE attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>R⁠C⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

公開情報によると、インターネットに公開されたGitLabサーバーのうち1,000台超が、リモートコード実行につながる深刻な脆弱性に対して未適用の状態にあるとされています。
さらに、この問題は既に悪用が観測されている文脈で扱われており、対応の遅れが継続リスクにつながる状況です。
GitLabは開発・運用の中核に置かれることが多く、脆弱なままだと認証情報やソースコード、CI/CD環境への影響が広がる可能性があります。
悪用が観測されているため、単なる注意喚起ではなく早急な対処が求められます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当するGitLabインスタンスのバージョンと適用状況を至急確認し、ベンダー案内に沿って修正を適用する。
- インターネット公開されている管理画面や関連サービスの露出を見直し、不要な公開を一時的に制限する。
- 適用後も不審なログイン、ジョブ実行、設定変更の有無を確認し、侵害の兆候がないか点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-97229 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| ベンダー | GitLab | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Over 1,000 GitLab servers vulnerable to ongoing RCE attacks](https://www.bleepingcomputer.com/news/security/over-1-000-gitlab-servers-vulnerable-to-code-execution-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-40747"></a>

### 2. CVE-2026-111357: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 40.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 67.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

CISAは、Ivanti Connect Secureに影響するCVE-2026-111357をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
公開情報では、実際の悪用が観測されており、Ivantiは関連する修正を案内しています。
KEV入りは、当該脆弱性がすでに現実の攻撃対象になっていることを示すため、優先度の高い対応が求められます。
特にVPN/リモートアクセス機器は侵入の起点になりやすく、影響が広がりやすい点が注目されます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 技術詳細・再現情報あり。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 技術詳細により影響確認が進みやすい。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Ivanti Connect Secureの利用有無を確認し、該当バージョンかどうかを点検する。
- ベンダーの修正情報を確認し、可能なら早急に適用する。
- 外部公開している管理面の露出状況や不審な認証・昇格の痕跡を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-111357 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-118527 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Ivanti | 言及あり | 0.80 | — |
| 製品 | Ivanti Connect Secure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-111357](https://nvd.nist.gov/vuln/detail/CVE-2026-111357) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA to federal agencies: Remediate exploited Ivanti Connect Secure vulnerabilit](https://www.helpnetsecurity.com/2026/11/02/cisa-to-federal-agencies-remediate-exploited-ivanti-connect-secure-vulnerabilities-cve-2026-111357-cve-2026-118527/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Additional Ivanti Connect Secure zero-days exploited in the wild (CVE-2026-11135](https://www.rapid7.com/blog/post/etr-additional-ivanti-connect-secure-zero-days-exploited-in-the-wild-cve-2026-111357-cve-2026-118527) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Chain Three Ivanti Connect Secure Flaws to Gain Unauthenticated Root A](https://thehackernews.com/2026/10/attackers-chain-three-ivanti-connect.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-40966"></a>

### 3. Ivanti patches two more Connect Secure zero-days chained in attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Ivantiは、Connect Secureに存在する2件の追加脆弱性に対して修正を公開しました。
これらは少なくとも10月1日以降、ゼロデイ攻撃で連鎖的に悪用されていたとされています。
リモートアクセス基盤に関わる製品であり、侵害されると社内ネットワークへの入口になり得るため注目されます。実際の悪用が観測されている点から、早急な適用や影響確認が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象バージョンと公開された修正内容を確認し、速やかにアップデート計画を立てる。
- Connect Secureの認証ログや管理ログを点検し、不審なアクセスや設定変更の有無を確認する。
- 外部公開しているリモートアクセス機器として、暫定的な露出最小化やアクセス制御の見直しを行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Ivanti | 言及あり | 0.80 | — |
| 製品 | Ivanti Connect Secure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Ivanti patches two more Connect Secure zero-days chained in attacks](https://www.bleepingcomputer.com/news/security/ivanti-patches-two-more-connect-secure-zero-days-chained-in-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-40917"></a>

### 4. Shutting the Door on the XCPE Botnet

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>I⁠o⁠C</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>A⁠n⁠d⁠r⁠o⁠i⁠d</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>サ⁠プ⁠ラ⁠イ⁠チ⁠ェ⁠ー⁠ン</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 45.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Googleと業界パートナーは、1.3百万台超のセットトップボックスを巻き込んだXCPEバックドア／ボットネットの活動を妨害したと公表しました。
分析では、このバックドアは複数年にわたり機器へ組み込まれ、広告不正や住宅向けプロキシ化などの収益化に使われていた可能性が高いとされています。
端末メーカー側の供給網に悪性コードが入り込むと、購入後も長期にわたり利用者の端末が不正利用されるおそれがあります。
今回の件は、組み込み機器の検証、ファームウェア整合性確認、そして住宅向けプロキシ系の悪用対策の重要性を示しています。

#### 温度感の理由

##### 温度感
- 技術詳細・再現情報あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 技術詳細により影響確認が進みやすい。
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- セットトップボックスやAndroid TV機器で、未承諾の常駐アプリや不審なプロキシ系動作がないか確認する。
- Google Play Protectや端末側の保護機能が有効かを点検し、無効化されていないか監視する。
- OEM/ODM由来の機器を導入する際は、ファームウェアの信頼性、更新体制、ベンダーのセキュリティ実績を調達条件に含める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Exchange | 言及あり | 0.80 | — |
| 製品 | Ivanti Policy Secure | 言及あり | 0.80 | — |
| 製品 | Active Directory | 言及あり | 0.80 | — |
| 攻撃/検証ツール | FRP | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Shutting the Door on the XCPE Botnet](https://cloud.google.com/blog/topics/threat-intelligence/shutting-the-door-on-the-xcpe-botnet/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-40903"></a>

### 5. AI-powered infostealer picks out the most profitable parts of your stolen data

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Cisco Talosの調査で、Windows向けの情報窃取型マルウェアが、盗んだデータをAIモデルに渡して価値の高い情報を選別していると報告されました。
対象のマルウェアはVOLTA-AUTODOXERと名乗っており、広く情報を集めたうえで、利益につながりそうな項目を優先する動きが示唆されています。
単なる大量窃取ではなく、AIで被害情報の“選別”を行う発想が確認された点が注目されています。
攻撃者がより効率的に利益化を図る可能性があり、情報窃取後の二次被害リスクを見直す材料になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 情報窃取の検知だけでなく、外部送信や不審なAI/API利用の痕跡も含めて監視する。
- 端末保護では、認証情報・セッション情報・業務文書など高価値データの所在を把握し、最小権限と多要素認証を徹底する。
- 感染後の被害拡大を抑えるため、EDRの隔離運用、資格情報の失効・再発行手順、漏えい時の対応訓練を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [AI-powered infostealer picks out the most profitable parts of your stolen data](https://www.helpnetsecurity.com/2026/11/02/ai-powered-infostealer-volta-victim-profiling/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-40954"></a>

### 6. Government Linux Servers Targeted With SysGoRAT and Suspected AI-Generated Scripts

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

政府系および国家関連のLinuxインフラを狙ったサイバー諜報活動が報告されました。
調査では、SysGoRATと呼ばれるマルウェアや、AI生成の可能性があるスクリプトの利用が示唆されています。
政府機関や関連組織のLinux環境が標的になっている点から、重要インフラや機密情報を扱う組織にとって無視できない動きです。
攻撃でAI支援のコードが使われた可能性があるなら、検知や分析の難しさが増す懸念があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 政府・関連組織のLinuxサーバーで、不審な永続化や認証情報の流出兆候がないか確認する。
- 既知のマルウェア名だけでなく、異常なスクリプト実行や不自然な自動化の痕跡も含めて監視する。
- 侵害の有無にかかわらず、ログ保全、権限管理、リモートアクセス経路の見直しを進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Government Linux Servers Targeted With SysGoRAT and Suspected AI-Generated Scrip](https://thehackernews.com/2026/11/government-linux-servers-targeted-with.html) | <nobr>内容確認・補足情報</nobr> |

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
| [it-sa 2026振り返り：セキュリティ運用を形作る主要トレンド](https://any.run/cybersecurity-blog/it-sa-2026-recap/) | 30.0 | 20.0 | 42.0 |
| [SynologyがNAS機器を狙うC3RB3Rランサムウェア攻撃に警告](https://www.bleepingcomputer.com/news/security/synology-warns-customers-of-ongoing-c3rb3r-ransomware-attacks/) | 28.0 | 30.0 | 42.0 |
| [FBIがBinanceの不正流出を北朝鮮のTraderTraitorに帰属](https://www.infosecurity-magazine.com/news/fbi-attributes-binance-north/) | 28.0 | 20.0 | 48.0 |
| [感染した130万台のAndroid TVボックスを操るボットネットを摘発](https://www.theregister.com/cyber-crime/2026/11/02/cops-bust-botnet-of-13m-infected-android-tv-boxes/5307045) | 28.0 | 20.0 | 42.0 |
| [Google、100万台規模のXCPE Androidマルウェアボットネットを遮断しTVボックスメーカーを禁止](https://www.bleepingcomputer.com/news/security/google-disrupts-million-device-xcpe-android-malware-botnet-bans-tv-box-maker/) | 28.0 | 20.0 | 42.0 |
| [週次まとめ：重大なCVE、Linux DDoSボットネット、デバイスコード型フィッシング、Androidスパイウェアなど](https://thehackernews.com/2026/11/weekly-recap-critical-cves-linux-ddos.html) | 28.0 | 20.0 | 42.0 |
| [Google、XCPEボットネットを阻止　背後の企業を利用停止に](https://www.helpnetsecurity.com/2026/11/02/xcpe-botnet-android-backdoor/) | 28.0 | 20.0 | 42.0 |
| [Googleが130万台規模のAndroidボットネットを阻止、TVボックスメーカーが犯罪者へのアクセスを販売か](https://thehackernews.com/2026/11/google-disrupts-13-million-device.html) | 28.0 | 20.0 | 42.0 |
| [DarkBlinders、イスラエルの標的とイラク・クルド自治政府のクラウド環境を侵害](https://thehackernews.com/2026/11/darkblinders-compromises-israeli-target.html) | 28.0 | 20.0 | 42.0 |
| [世界各地の複数のスパイ活動キャンペーンで悪用されたAgenticペンテストツール](https://www.cybersecuritydive.com/news/agentic-pen-testing-tool-espionage-campaigns/873427/) | 28.0 | 20.0 | 42.0 |
| [PapRATによるサイバースパイ活動キャンペーンが南アジアに苦い後味を残す](https://www.darkreading.com/cyberattacks-data-breaches/paprat-cyberespionage-campaign-bitter-south-asia) | 28.0 | 20.0 | 42.0 |
| [Bitterがアジア向けサイバースパイ活動でPapRATを展開](https://www.infosecurity-magazine.com/news/paprat-bitter-cyberespionage/) | 28.0 | 20.0 | 42.0 |
| [Cursor公式マーケットプレイスの「Claude Code」にSSHバックドアが発見される](https://gigazine.net/news/20261102-official-claude-code-extension-compromise/) | 27.0 | 20.0 | 42.0 |
| [LLMJackingの台頭：脅威アクターはいかに侵害したクラウドとモデル資源を収益化するか](https://cloud.google.com/blog/topics/threat-intelligence/llmjacking-monetizing-compromised-cloud-models/) | 25.0 | 45.0 | 42.0 |
| [Trigger AIワークフローツールから環境変数が盗まれる](https://www.theregister.com/security/2026/11/02/thieves-pilfer-environment-variables-from-trigger-ai-workflow-tool/5306998) | 25.0 | 20.0 | 42.0 |
| [クラウドホスト型AIワークフローツールでセキュリティインシデントにより環境変数が窃取される](https://www.theregister.com/security/2026/11/02/cloud-hosted-ai-workflow-tool-has-environment-variables-snatched-in-security-incident/5306998) | 25.0 | 20.0 | 42.0 |
| [MicrosoftのAIリスクレポートが見落としている重要な点](https://www.darkreading.com/cyberattacks-data-breaches/microsoft-ai-cyber-risk-report-miss) | 25.0 | 20.0 | 42.0 |
| [ReactiveからProactiveへ：Wiz RedおよびBlueエージェントでSOCチームを強化する](https://www.wiz.io/blog/soc-alerts-red-and-blue-agents) | 25.0 | 20.0 | 42.0 |
| [ホワイトハウスがAIタスクフォースを打ち出す一方でCISAが不在な理由](https://www.cybersecuritydive.com/news/cisa-white-house-ai-task-force-missing-trump/873338/) | 25.0 | 20.0 | 42.0 |
| [Langflowの重大な脆弱性により未認証の攻撃者がサーバー上でコードを実行可能にする恐れ](https://thehackernews.com/2026/11/critical-langflow-flaws-could-let.html) | 25.0 | 20.0 | 42.0 |
| [あなたのSOCはAIエージェントに対応できるか：導入前の成熟度チェック](https://thehackernews.com/2026/11/is-your-soc-ready-for-ai-agents.html) | 25.0 | 20.0 | 42.0 |
| [Cursorのサプライチェーン攻撃で配布された悪意あるClaude Code拡張機能](https://www.securityweek.com/malicious-claude-code-extension-served-in-cursor-supply-chain-attack/) | 25.0 | 20.0 | 42.0 |
| [Chainalysis、AI駆動のサイバー攻撃によるデータ侵害を公表](https://www.securityweek.com/chainalysis-discloses-data-breach-following-ai-driven-cyberattack/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントを安全に運用するための3つの問い](https://www.cybersecuritydive.com/spons/3-questions-for-securing-ai-agents/873054/) | 25.0 | 20.0 | 42.0 |
| [Chainalysis、"Offensive Agentic"セキュリティインシデント後に顧客へ警告](https://www.infosecurity-magazine.com/news/chainalysis-customers-offensive/) | 25.0 | 20.0 | 42.0 |
| [CyberStrikeAIの実戦投入：組織を標的とした実際の攻撃におけるAIの利用](https://securelist.com/tr/cyberstrikeai-attacks/121715/) | 25.0 | 20.0 | 42.0 |
| [外務省のネットワークで侵害 - 個人情報流出の可能性](https://www.security-next.com/192256) | 22.0 | 20.0 | 42.0 |
| [アイリスオーヤマ通販サイトで侵害 - 詳細を調査](https://www.security-next.com/192208) | 22.0 | 20.0 | 42.0 |
| [個人情報漏洩の個人向け被害者相談窓口を強化 - IPA](https://www.security-next.com/192287) | 22.0 | 20.0 | 42.0 |
| [GMO、2年前の脆弱性指摘後も再診断せず 自社AI診断のグループ適用は事件後](https://xtech.nikkei.com/atcl/nxt/column/18/00001/12148/) | 21.0 | 20.0 | 42.0 |
| [GMO熊谷代表、涙の謝罪会見でも“熊谷節”さく裂──「31年間、もうけるという言葉は使ったことがない」](https://www.itmedia.co.jp/news/article/2611/02/2000002823/) | 21.0 | 20.0 | 42.0 |
| [GMO熊谷代表、会見で改めて謝罪 SNS投稿巡り「配慮が欠けていた」](https://www.itmedia.co.jp/news/article/2611/02/2000002806/) | 21.0 | 20.0 | 42.0 |
| [NTTデータの情報漏洩、委託先はSecuritizeと判明 楽天証券などに影響](https://xtech.nikkei.com/atcl/nxt/column/18/00001/12147/) | 21.0 | 20.0 | 42.0 |
| [AIで脆弱性発見が加速、すべてを修正する必要はあるのか？ レッドハットが解説](https://news.mynavi.jp/techplus/article/20261102-5242704/) | 21.0 | 20.0 | 42.0 |
| [不正アクセスでGMO熊谷会長が謝罪、SNS発信も「配慮欠いた」](https://xtech.nikkei.com/atcl/nxt/news/24/03453/) | 21.0 | 20.0 | 42.0 |
| [パスキー万能説破れる？ Google同期パスキー実装に見つかった“想定外の穴”](https://atmarkit.itmedia.co.jp/ait/articles/2611/02/news025.html) | 21.0 | 20.0 | 42.0 |
| [FBI、Binanceの63億ドル規模の暗号資産窃盗を北朝鮮ハッカーの犯行と断定](https://www.theregister.com/security/2026/11/02/fbi-pins-63b-binance-crypto-heist-on-north-korean-hackers/5306889) | 20.0 | 20.0 | 48.0 |
| [FBIがBinanceの63億ドル仮想通貨窃盗を北朝鮮の犯行と断定、焦る利用者を詐欺師が狙う](https://www.helpnetsecurity.com/2026/11/02/fbi-north-korea-binance-hack/) | 20.0 | 20.0 | 48.0 |
| [FBIがNorth KoreaのBinanceハッキングに関連する600超のアドレスを特定](https://www.securityweek.com/fbi-flags-over-600-addresses-tied-to-north-koreas-binance-heist/) | 20.0 | 20.0 | 48.0 |
| [サイバー攻撃の疑いでFintechプラットフォームSageworksが停止](https://www.bleepingcomputer.com/news/security/fintech-platform-sageworks-taken-offline-after-suspected-cyberattack/) | 20.0 | 20.0 | 42.0 |
| [Polymarket、サイト侵害後に被害者へ390万ドルを返還すると表明](https://therecord.media/polymarket-returning-funds-to-customers-after-site-compromise) | 20.0 | 20.0 | 42.0 |
| [ロシア統計局、ベラルーシとウクライナのハッカーによるサイバー攻撃を確認](https://therecord.media/hackers-ukraine-belarus-russia) | 20.0 | 20.0 | 42.0 |
| [トークン窃取で企業に1日10万ドル超の不正LLM課金被害](https://www.theregister.com/security/2026/11/02/token-thieves-costing-companies-100k-per-day-in-illicit-llm-charges/5306967) | 20.0 | 20.0 | 42.0 |
| [BTCPay Serverの旧バージョン環境でホットウォレットの暗号資産盗難に警告](https://www.bleepingcomputer.com/news/security/btcpay-server-warns-of-hot-wallet-thefts-targeting-outdated-instances/) | 20.0 | 20.0 | 42.0 |
| [携帯通信事業者は通話履歴を何年も保存している](https://www.bleepingcomputer.com/news/security/your-mobile-carrier-stores-your-call-logs-for-years/) | 20.0 | 20.0 | 42.0 |
| [2026年10月に発表された37件のサイバーセキュリティM&A動向まとめ](https://www.securityweek.com/cybersecurity-ma-roundup-37-deals-announced-in-october-2026/) | 20.0 | 20.0 | 42.0 |
| [Armadinのテストで重大な脆弱性の88%がベンダーのアドバイザリ外に判明](https://www.infosecurity-magazine.com/news/armadin-severe-exposures-missed/) | 20.0 | 20.0 | 42.0 |
| [ロシアとウクライナ、緊急警報アプリへの攻撃を報告](https://www.theregister.com/security/2026/11/02/nuclear-threats-and-street-brawls-russia-ukraine-report-attacks-on-their-emergency-alert-apps/5306901) | 20.0 | 20.0 | 42.0 |
| [Florida Student Aid Websiteのハッキングで490万人のデータが危険にさらされる](https://www.securityweek.com/florida-student-aid-website-hack-puts-data-of-4-9-million-people-at-risk/) | 20.0 | 20.0 | 42.0 |
| [Apple、99カ国のユーザーに傭兵型スパイウェアの警告](https://therecord.media/apple-warns-users-99-countries-mercenary-spyware) | 20.0 | 20.0 | 42.0 |
| [ロシアとウクライナのハッカーが緊急アプリを乗っ取り偽の核攻撃警報を拡散](https://therecord.media/ukraine-hackers-russia-alert-system) | 20.0 | 20.0 | 42.0 |
| [欧州のスーパーマーケットでハッカーが冷蔵システムを妨害](https://www.bleepingcomputer.com/news/security/hackers-disrupt-refrigeration-systems-at-european-supermarkets/) | 20.0 | 20.0 | 42.0 |
| [欧州のスーパーマーケットを襲う冷蔵設備への第二波サイバー攻撃](https://www.helpnetsecurity.com/2026/11/02/european-supermarkets-refrigeration-units-cyberattacks/) | 20.0 | 20.0 | 42.0 |
| [星5評価を売買する地下の偽レビュー取引の実態](https://www.malwarebytes.com/blog/threat-intel/2026/11/5-stars-for-sale-inside-the-underground-fake-review-trade) | 20.0 | 20.0 | 42.0 |
| [Applebee’sの顧客データ、アプリに残されたパスワードが原因で流出](https://www.malwarebytes.com/blog/news/2026/11/applebees-customer-data-exposed-by-password-left-in-app) | 20.0 | 20.0 | 42.0 |
| [Microsoft、10月のWindows更新で壊れたSmart App Controlを修正](https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-smart-app-control-broken-by-october-windows-update/) | 20.0 | 20.0 | 42.0 |
| [Revolveのデータ侵害、少なくとも18万人に影響](https://www.securityweek.com/revolve-data-breach-impacts-at-least-180000-people/) | 20.0 | 20.0 | 42.0 |
| [ノジマ 700万人分の個人情報流出](https://news.yahoo.co.jp/pickup/6601104?source=rss) | 20.0 | 20.0 | 42.0 |
| [Google、Root-in-Cloudのバグ報奨金を25万ドルに設定](https://www.securityweek.com/google-introduces-250000-root-in-cloud-bug-bounty-reward/) | 20.0 | 20.0 | 42.0 |
| [Frozen part II: ヨーロッパのスーパーマーケットでハッカーが再び青果を遠隔解凍](https://www.theregister.com/cyber-crime/2026/11/02/frozen-part-ii-hackers-remotely-defrost-produce-in-euro-supermarkets-again/5306924) | 20.0 | 20.0 | 42.0 |
| [InfostealerがLLMを使って被害者の詳細情報を収集・整理](https://www.itpro.com/security/malware/infostealer-uses-llms-to-compile-dossiers-on-victims) | 20.0 | 20.0 | 42.0 |
| [欧州各地のスーパーマーケット冷凍庫を狙った疑いのあるサイバー攻撃の第2波](https://therecord.media/cyberattack-grocery-freezers-europe) | 20.0 | 20.0 | 42.0 |
| [Trezorの一部ウォレットにシード窃取用インプラントが潜んでいる可能性を警告](https://www.helpnetsecurity.com/2026/11/02/trezor-hardware-wallet-implant-cryptobilis/) | 20.0 | 20.0 | 42.0 |
| [CISAが2026年の重要インフラセキュリティ・レジリエンス月間を開始](https://www.cisa.gov/news-events/news/cisa-kicks-critical-infrastructure-security-and-resilience-month-2026) | 20.0 | 20.0 | 42.0 |
| [Chainalysisが“offensive agentic techniques”で侵害される](https://www.helpnetsecurity.com/2026/11/02/chainalysis-breached-using-offensive-agentic-techniques/) | 20.0 | 20.0 | 42.0 |
| [Microsoft TeamsでITサポートを装い、AD CSを悪用して企業データを窃取する攻撃](https://thehackernews.com/2026/11/attackers-pose-as-it-support-on.html) | 20.0 | 20.0 | 42.0 |
| [「GMOトラスト・ログイン」で2492社・4万5030人の情報漏えい、設定不備でファイルが公開領域に](https://internet.watch.impress.co.jp/docs/news/2153245.html) | 20.0 | 20.0 | 42.0 |
| [中堅組織が高度な脅威に対抗するためにXDRを活用する方法](https://www.security.com/expert-perspectives/how-midsize-organizations-use-xdr-fight-sophisticated-threats) | 20.0 | 20.0 | 42.0 |
| [Nick Andersen氏の暫定職務は続くのか？](https://cyberscoop.com/nick-andersen-cisa-acting-director-nomination/) | 20.0 | 20.0 | 42.0 |
| [GMO攻撃 警視庁が捜査本部設置](https://news.yahoo.co.jp/pickup/6601090?source=rss) | 20.0 | 20.0 | 42.0 |
| [業務を止めずにOT・IoT・医療機器を保護する方法](https://www.cybersecuritydive.com/spons/protecting-ot-iot-and-medical-devices-without-disrupting-operations/833813/) | 20.0 | 20.0 | 42.0 |
| [PolymarketがDNSハイジャックを受けたとしてDebugBearが指摘、トレーダーに390万ドルを返金](https://www.securityweek.com/polymarket-returns-3-9-million-to-traders-as-debugbear-cites-dns-hijack/) | 20.0 | 20.0 | 42.0 |
| [セキュリティの1週間（10月26日～11月1日）](https://www.malwarebytes.com/blog/news/2026/11/a-week-in-security-october-26-november-1-2) | 20.0 | 20.0 | 42.0 |

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
