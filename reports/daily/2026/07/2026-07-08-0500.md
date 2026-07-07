# 📡 サイレーダー 2026-07-08 05:00 JST

このレポートは、2026-07-07 17:00 JST〜2026-07-08 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 92
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 62

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Hitachi Energy e-mesh EMS](#topic-4593) | 50.0 | 67.0 | 63.0 | 音声 | 温度感上位枠 |
| 2 | [CISA Adds Three Known Exploited Vulnerabilities to Catalog](#topic-21269) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Suspected Chinese espionage group used a Roundcube exploit chain to burrow into universities](#topic-21304) | 34.0 | 28.0 | 54.0 | 音声 | 温度感上位枠 |
| 4 | [Adaptive AI for Detecting Modern DGA Attacks](#topic-21225) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [社内システムが侵害、マルウェア感染の可能性 - ハンズHD](#topic-21307) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-4593"></a>

### 1. Hitachi Energy e-mesh EMS

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 50.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 67.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

公開情報では、CVE-2026-42945に関連する脆弱性について、影響範囲や悪用可能性が報告されています。
CISAの勧告では、Hitachi Energy e-mesh EMSにバッファオーバーフローの問題があり、サービス停止や任意コード実行につながる可能性があるとされています。
制御・運用系製品に影響しうるため、脆弱性の有無や適用状況の確認が重要です。実際の悪用観測に関する報道もあり、対応の優先度を上げる材料になっています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 技術詳細・再現情報あり。
- 脅威・攻撃キャンペーン文脈。
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

- 対象製品・対象バージョンに該当するかを確認し、提供元の推奨する修正や回避策を確認する。
- 外部から到達可能な経路や関連サービスの露出状況を見直し、不要な公開を避ける。
- 異常な停止や不審なリクエスト増加など、サービス影響の兆候を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-42945 | 関連CVE | 1.00 | 未確認 |
| 製品 | Ivanti Connect Secure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-42945](https://nvd.nist.gov/vuln/detail/CVE-2026-42945) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Hitachi Energy e-mesh EMS](https://www.cisa.gov/news-events/ics-advisories/icsa-26-188-03) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers are exploiting critical NGINX vulnerability (CVE-2026-42945)](https://www.helpnetsecurity.com/2026/05/18/ngnix-vulnerability-exploited-cve-2026-42945/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [NGINX CVE-2026-42945 Exploited in the Wild, Causing Worker Crashes and Possible ](https://thehackernews.com/2026/05/nginx-cve-2026-42945-exploited-in-wild.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [NGINXでリモートコード実行の脆弱性が発見される、影響を受けるバージョンはこれ](https://gigazine.net/news/20260515-nginx-remote-code-execution/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [18-Year-Old NGINX Rewrite Module Flaw Enables Unauthenticated RCE](https://thehackernews.com/2026/05/18-year-old-nginx-rewrite-module-flaw.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（2件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-21269"></a>

### 2. CISA Adds Three Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、実際に悪用が確認されたとして3件の脆弱性をKnown Exploited Vulnerabilities（KEV）Catalogに追加しました。
対象はJoomShaper SP Page Builder、Langflow、Joomlack Page Builderに関する脆弱性です。
KEV Catalogへの追加は、当該脆弱性が現実の攻撃に使われていることを示す重要なシグナルです。
特に公開資産や該当製品を運用している組織では、通常の脆弱性より優先度を上げて対応する必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当製品の利用有無を確認し、影響範囲を洗い出す。
- 公開されている資産や外部到達可能なシステムを優先して更新・緩和策を適用する。
- 修正前後を含め、侵害の有無を点検し、必要に応じてログや設定変更の確認を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-48908 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-55255 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-56290 | 関連CVE | 1.00 | 未確認 |
| 製品 | Langflow | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Three Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/07/07/cisa-adds-three-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21304"></a>

### 3. Suspected Chinese espionage group used a Roundcube exploit chain to burrow into universities

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>国⁠家⁠支⁠援</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>Exploit Kit</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 34.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 28.0 |
| <nobr>確⁠度</nobr> | 54.0 |

#### 概要

米国とカナダの大学にあるRoundcubeのWebメール環境を狙った攻撃活動が報告されています。
公開済みで修正済みの脆弱性、特にCVE-2024-42009を含む脆弱性連鎖が悪用された可能性が示されており、大学の理工系部門が標的になったとされています。
大学のメール環境は認証情報や研究関連情報の起点になりやすく、侵害されると被害が広がるおそれがあります。
修正済み脆弱性でも、未適用環境が残っている場合は継続的に狙われる点が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Roundcubeの該当脆弱性対応状況を確認し、必要なパッチ適用とバージョン管理を急ぐ。
- 理工系部門など外部からのアクセスが想定されるメール環境について、認証情報の不審な利用やログイン異常を点検する。
- Webメール経由の侵入を前提に、アカウント保護の強化と侵害前提の監視・通知体制を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2024-42009 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2025-49113 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2024-42009](https://nvd.nist.gov/vuln/detail/CVE-2024-42009) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Suspected China-Aligned Hackers Exploit Roundcube Flaws Against Universities](https://thehackernews.com/2026/07/suspected-china-aligned-hackers-exploit.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Suspected Chinese espionage group used a Roundcube exploit chain to burrow into ](https://cyberscoop.com/china-espionage-attacks-us-canada-universities-proofpoint/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21225"></a>

### 4. Adaptive AI for Detecting Modern DGA Attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Akamai Security Intelligenceは、現代的なDGA（ドメイン生成アルゴリズム）攻撃の検知に向けた適応型AIの考え方を紹介しています。
DGAは不正通信やボットネット関連の活動で使われることがあり、検知精度の向上は防御側にとって重要な課題です。
従来のルールベース検知では追随しにくい変化の速い脅威に対して、AIをどう活用するかが注目されています。
DNS監視や脅威インテリジェンスの運用に関わる組織では、検知ロジックの見直しや補完策の検討材料になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- DNSログやドメイン解決の異常を継続的に観測し、既存の検知ルールとのギャップを確認する。
- AIベースの検知を導入する場合は、誤検知率と運用負荷を含めて評価する。
- DGA関連の検知結果を脅威インテリジェンスや他のテレメトリと突き合わせて、優先度判断に使う。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Adaptive AI for Detecting Modern DGA Attacks](https://www.akamai.com/blog/security/2026/jul/adaptive-ai-detecting-modern-dga-attacks) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21307"></a>

### 5. 社内システムが侵害、マルウェア感染の可能性 - ハンズHD

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

ハンズホールディングスは、社内システムが侵害され、マルウェアに感染した可能性があると公表しました。
現在は詳細を調査している段階で、影響範囲や侵入経路などはまだ明らかになっていません。
社内システムへの侵害の可能性は、業務停止や情報管理への影響につながるため、企業にとって重要な事案です。
公表時点で調査中であることから、続報によって対応状況や影響の見極めが必要になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 社内端末・サーバーの異常兆候や不審な通信の有無を確認する。
- 影響が疑われる範囲のアカウント、機器、ログを速やかに保全して調査に備える。
- 関連する認証情報の見直しと、必要に応じたパスワード・鍵の更新を検討する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [社内システムが侵害、マルウェア感染の可能性 - ハンズHD](https://www.security-next.com/186908) | <nobr>内容確認・補足情報</nobr> |

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
| [UAT-7810、新たなマルウェアでORBネットワークの構築を継続](https://blog.talosintelligence.com/uat-7810/) | 30.0 | 20.0 | 42.0 |
| [Giteaの重大な脆弱性が現在悪用中、研究者が警告](https://www.securityweek.com/critical-gitea-flaw-under-active-exploitation-researchers-warn/) | 28.0 | 46.0 | 54.0 |
| [CAI Cloudワーム、競合マルウェアを排除し秘密情報を窃取したうえで暗号資産をマイニング](https://www.theregister.com/cyber-crime/2026/07/07/cai-cloud-worm-gives-competitors-malware-the-boot-then-steals-secrets-and-mines-for-coin/5267856) | 28.0 | 45.0 | 42.0 |
| [サイバー専門家が初の「エージェント型ランサムウェア」を特定、ただし注意点あり](https://www.itpro.com/security/its-a-marker-of-where-extortion-tradecraft-is-heading-cyber-experts-say-theyve-identified-the-first-case-of-agentic-ransomware-but-theres-a-catch) | 28.0 | 30.0 | 42.0 |
| [中国系ハッカーがORBネットワーク拡大のためにLONGLEASHマルウェアを開発](https://www.bleepingcomputer.com/news/security/chinese-hackers-develop-longleash-malware-to-expand-orb-network/) | 28.0 | 20.0 | 42.0 |
| [RedWingのMaaSパッケージがTelegramレンタルサービスとしてAndroid銀行詐欺を提供](https://thehackernews.com/2026/07/redwing-maas-packages-android-bank.html) | 28.0 | 20.0 | 42.0 |
| [Predatorgate監視騒動の被害者ら、スパイウェアメーカーを8百万ユーロで提訴](https://www.theregister.com/security/2026/07/07/predatorgate-victims-launch-8m-sueball-at-spyware-maker/5267766) | 28.0 | 20.0 | 42.0 |
| [One Email Closer to the Edge: UNK_MassTractionとエクスプロイトの物理学](https://www.proofpoint.com/us/blog/threat-insight/one-email-closer-edge-unkmasstraction-physics-exploitation) | 28.0 | 20.0 | 42.0 |
| [DEBULLツールがMicrosoft Device Codeフローを悪用してM365アカウントを標的にする](https://thehackernews.com/2026/07/debull-tooling-abuses-microsoft-device.html) | 28.0 | 20.0 | 42.0 |
| [Banana RATの進化：ANY.RUNを通じて比較する2つの最新系統](https://any.run/cybersecurity-blog/banana-rat-evolution-analysis/) | 28.0 | 20.0 | 42.0 |
| [Database内の「Ghost」：Machine DPAPIで有効なADFS署名鍵を復元する方法](https://cloud.google.com/blog/topics/threat-intelligence/recovering-active-adfs-signing-keys-machine-dpapi/) | 28.0 | 20.0 | 42.0 |
| [Netflix、Coca-Cola、FIFAをかたる偽求人詐欺がマーケターを標的に](https://www.malwarebytes.com/blog/scams/2026/07/fake-netflix-coca-cola-and-fifa-job-scams-target-marketers) | 28.0 | 20.0 | 42.0 |
| [Iran関連のハッカーがサイバー攻撃でモジュール型C&Cフレームワークを使用](https://www.securityweek.com/iran-linked-hackers-using-modular-cc-framework-in-cyberattacks/) | 28.0 | 20.0 | 42.0 |
| [Microsoft Teamsで偽のIT担当者が従業員をだましてマルウェアをインストールさせる手口](https://www.theregister.com/cyber-crime/2026/07/07/fake-it-bods-on-microsoft-teams-coax-workers-into-installing-malware/5267610) | 28.0 | 20.0 | 42.0 |
| [ハッカーがAdobe ColdFusionの最高深刻度の脆弱性を悪用](https://www.infosecurity-magazine.com/news/exploit-maximum-severity-adobe/) | 28.0 | 20.0 | 42.0 |
| [FortiBleedキャンペーンの悪化で全組織のリスクが急増](https://www.itpro.com/security/cyber-attacks/the-risk-to-every-organization-has-increased-exponentially-the-fortibleed-campaign-just-took-a-turn-for-the-worse) | 28.0 | 20.0 | 42.0 |
| [英国、国家防衛のため自律型AI「Cyber Shield」構築を計画](https://therecord.media/britain-plans-autonomous-ai-cyber-shield) | 25.0 | 20.0 | 42.0 |
| [AI向けにネットワークを近代化する企業、攻撃対象領域の拡大と可視性不足を懸念](https://www.cybersecuritydive.com/news/ai-network-expansion-security-concerns-cisco/824581/) | 25.0 | 20.0 | 42.0 |
| [CyberProofのAgentic MXDRサービス、AIエージェントをMDRに導入](https://www.helpnetsecurity.com/2026/07/07/cyberproof-agentic-mxdr-service/) | 25.0 | 20.0 | 42.0 |
| [Writer AIの脆弱性により、エージェントのプレビューでテナント間のセッショントークンが漏えいする可能性](https://thehackernews.com/2026/07/writer-ai-flaw-could-let-agent-previews.html) | 25.0 | 20.0 | 42.0 |
| [CISAがAnthropicのMythosを使って政府ソフトウェアの脆弱性をスキャンしていると報道](https://www.securityweek.com/cisa-reportedly-using-anthropics-mythos-to-scan-government-software-for-flaws/) | 25.0 | 20.0 | 42.0 |
| [エンタープライズAI、十分な検討なしの導入でなお課題が残る](https://www.theregister.com/security/2026/07/07/enterprise-ai-still-smarting-from-leaping-before-looking/5267353) | 25.0 | 20.0 | 42.0 |
| [Commvault、AI攻撃シミュレーションでサイバー復旧体制を評価](https://www.helpnetsecurity.com/2026/07/07/commvault-measures-cyber-recovery-readiness-with-ai-attack-simulations/) | 25.0 | 20.0 | 42.0 |
| [Cyber Shield：サイバー防御におけるエージェント型AI時代への道](https://www.ncsc.gov.uk/blogs/cyber-shield-the-path-to-an-agentic-ai-future-for-cyber-defence) | 25.0 | 20.0 | 42.0 |
| [AIがコードを書くソフトウェア供給網で何が変わるのか](https://thehackernews.com/2026/07/what-changes-when-your-software-supply.html) | 25.0 | 20.0 | 42.0 |
| [Claude Codeに隠されたトラッカーは「実験」だったとAnthropicが説明](https://www.malwarebytes.com/blog/news/2026/07/claude-codes-hidden-tracker-was-an-experiment-says-anthropic) | 25.0 | 20.0 | 42.0 |
| [Radware、Agentic AI ProtectionをAIガバナンスとコンプライアンス機能で更新](https://www.helpnetsecurity.com/2026/07/07/radware-agentic-ai-protection-enhancements/) | 25.0 | 20.0 | 42.0 |
| [詐欺師がAIを悪用してあり得ない花を販売している](https://www.malwarebytes.com/blog/scams/2026/07/scammers-are-using-ai-to-sell-impossible-flowers) | 25.0 | 20.0 | 42.0 |
| [Keyfactor、AIと耐量子セキュリティに向けて10億ドル超の投資を獲得](https://www.securityweek.com/keyfactor-scores-1-billion-investment-for-ai-post-quantum-security/) | 25.0 | 20.0 | 42.0 |
| [Digi International PortServer TSおよびDigi One SP IAの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-188-07) | 24.0 | 46.0 | 50.0 |
| [GitHubのエージェント型ワークフローからプライベートデータが漏えいする「GitLost」脆弱性](https://www.darkreading.com/cyber-risk/gitlost-leaks-private-data-github-agentic-workflows) | 24.0 | 38.0 | 42.0 |
| [Hydro-Québec Le Circuit Electrique充電ステーションのバックエンド](https://www.cisa.gov/news-events/ics-advisories/icsa-26-188-01) | 22.0 | 40.0 | 50.0 |
| [持込用学習端末のECサイトにサイバー攻撃 - 個人情報流出の可能性](https://www.security-next.com/186704) | 22.0 | 20.0 | 42.0 |
| [農業従事者情報を含むデータを誤送信 - フィルタ解除で閲覧可能](https://www.security-next.com/186821) | 22.0 | 20.0 | 42.0 |
| [学生情報含む書類を宿泊施設に置き忘れて紛失 - 新潟県](https://www.security-next.com/186765) | 22.0 | 20.0 | 42.0 |
| [Microsoft Sentinelのコストを削減しつつ検知精度を損なわない方法 ― 第2回：ファイアウォール探索](https://blog.nviso.eu/2026/07/07/reducing-microsoft-sentinel-costs-without-compromising-detection-part-2-the-firewall-quest/) | 22.0 | 20.0 | 42.0 |
| [GitHub ActionsにおけるCIセキュリティスキャナーが見逃す攻撃パターン](https://www.bleepingcomputer.com/news/security/the-github-actions-attack-pattern-your-ci-security-scanners-miss/) | 20.0 | 45.0 | 42.0 |
| [Hitachi Energy PROMOD Vの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-188-02) | 20.0 | 28.0 | 50.0 |
| [Labcenter Proteus 9に関する脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-188-06) | 20.0 | 28.0 | 50.0 |
| [Cloudflareが英国政府のCyber Resilience Pledgeに参加](https://blog.cloudflare.com/cloudflare-joins-uk-cyber-resilience-pledge/) | 20.0 | 20.0 | 48.0 |
| [FBI情報提供を受け、スペインが親ロシア派ハクティビスト容疑者を拘束](https://www.theregister.com/security/2026/07/07/alleged-pro-russia-hacktivist-arrested-in-palencia/5267569) | 20.0 | 20.0 | 48.0 |
| [Air Gapped環境を強化するためのヒント](https://www.security.com/product-insights/tips-harden-your-air-gapped-environments) | 20.0 | 20.0 | 42.0 |
| [RedditとDiscordの偽通報詐欺によるアカウント窃取手口](https://www.malwarebytes.com/blog/threat-intel/2026/07/how-the-reddit-and-discord-false-report-scam-steals-accounts) | 20.0 | 20.0 | 42.0 |
| [郡政府がサイバー恐喝グループに100万ドルを支払ったと報じられる](https://www.securityweek.com/county-government-reportedly-paid-1-million-to-cyber-extortion-group/) | 20.0 | 20.0 | 42.0 |
| [Tendaルーターのファームウェアに隠されたバックドアが管理者アクセスを許可](https://www.bleepingcomputer.com/news/security/hidden-backdoor-in-tenda-router-firmware-grants-admin-access/) | 20.0 | 20.0 | 42.0 |
| [Rogue Agentの脆弱性によりGoogle Dialogflow CXチャットボットが乗っ取られる可能性](https://thehackernews.com/2026/07/rogue-agent-flaw-could-have-let.html) | 20.0 | 20.0 | 42.0 |
| [脆弱なRoundcubeサーバーを悪用して大学を狙う中国系脅威グループの疑い](https://www.infosecurity-magazine.com/news/china-aligned-cluster-roundcube/) | 20.0 | 20.0 | 42.0 |
| [スペインで親ロシア系ハクティビストグループのメンバーとみられる人物を逮捕](https://www.bleepingcomputer.com/news/security/spain-arrests-suspected-member-of-pro-russian-hacktivist-groups/) | 20.0 | 20.0 | 42.0 |
| [日本の大手通信事業者、サイバー攻撃で1200万件のメールアドレス流出](https://therecord.media/major-japanese-telco-cyberattack-12-million-emails) | 20.0 | 20.0 | 42.0 |
| [Public GitHub IssueでGitHubのAgentic Workflowが非公開リポジトリのデータを漏えいさせる可能性](https://thehackernews.com/2026/07/public-github-issue-could-trick-github.html) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderの組織構造は統一されたギャングというよりサイバー犯罪集団に近い](https://www.infosecurity-magazine.com/news/scattered-spider-as-cybercrime/) | 20.0 | 20.0 | 42.0 |
| [Barracuda、Evo Securityの買収でPAMとID保護を強化](https://www.helpnetsecurity.com/2026/07/07/barracuda-evo-security-acquisition/) | 20.0 | 20.0 | 42.0 |
| [Picus Autonomous Exposure Validation Platformが実環境でのCVE悪用可能性を検証](https://www.helpnetsecurity.com/2026/07/07/picus-autonomous-exposure-validation-platform-validates-real-world-cve-exploitability/) | 20.0 | 20.0 | 42.0 |
| [英政府のサイバー誓約、閣僚の呼びかけも大手企業の参加はわずか](https://therecord.media/uk-cyber-pledge-draws-limited-partners-despite-ministerial-appeal) | 20.0 | 20.0 | 42.0 |
| [クレジットカードフィッシングで2人を逮捕、オランダが欧州で最悪の決済詐欺国に認定](https://www.bitdefender.com/en-us/blog/hotforsecurity/two-arrested-credit-card-phishing-netherlands-europe-payment-fraud) | 20.0 | 20.0 | 42.0 |
| [JanuscapeのLinux脆弱性によりIntel・AMDデバイスでVMエスケープが可能に](https://www.bleepingcomputer.com/news/linux/new-januscape-linux-kernel-flaw-allows-vm-escape-on-intel-amd-devices/) | 20.0 | 20.0 | 42.0 |
| [CISO Conversations: Tarah Wheeler, サイバーセキュリティリーダー、思想的リーダー、独創的な発想者](https://www.securityweek.com/ciso-conversations-tarah-wheeler-cybersecurity-leader-thought-leader-and-original-thinker/) | 20.0 | 20.0 | 42.0 |
| [政府のサイバー誓約に60組織が署名、M&SやCapitaも参加](https://www.theregister.com/security/2026/07/07/governments-cyber-pledge-lands-60-signatories-including-ms-and-somehow-capita/5267554) | 20.0 | 20.0 | 42.0 |
| [Linux Kernelの脆弱性によりIntelおよびAMDシステムでVMエスケープが可能に](https://www.securityweek.com/linux-kernel-vulnerability-allows-vm-escape-on-intel-and-amd-systems/) | 20.0 | 20.0 | 42.0 |
| [英国政府、60以上の賛同者を得てサイバー・レジリエンス誓約を開始](https://www.infosecurity-magazine.com/news/uk-gov-launches-cyber-resilience/) | 20.0 | 20.0 | 42.0 |
| [英国のサイバー・レジリエンス誓約、60社の参加で強化策が加速](https://www.itpro.com/security/uks-cyber-resilience-pledge-gathers-momentum-as-60-firms-sign-up-to-bolster-capabilities) | 20.0 | 20.0 | 42.0 |
| [BeyondTrust、リモートアクセスソフトウェアの深刻な脆弱性を警告](https://www.bleepingcomputer.com/news/security/beyondtrust-warns-of-critical-flaws-in-remote-access-software/) | 20.0 | 20.0 | 42.0 |

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
