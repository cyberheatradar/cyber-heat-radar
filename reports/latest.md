# 📡 サイレーダー 2026-05-27 05:00 JST

このレポートは、2026-05-26 17:00 JST〜2026-05-27 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 107
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [ABB AbilityTM Zenon Remote Transport Vulnerability](#topic-10344) | 41.0 | 64.0 | 51.0 | 音声 | 温度感上位枠 |
| 2 | [Hackers Exploited KnowledgeDeliver Zero-Day for Web Shell Deployment](#topic-10358) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [AI Threat Landscape Digest March-April 2026](#topic-10371) | 41.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Anthropic: Claude Mythos identified 10,000+ software flaws](#topic-10324) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [CERT-In Recommends 12-Hour Patching for Internet-Facing Flaws Amid AI-Assisted Attacks](#topic-10380) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [Iran-Linked Hackers Target US Aviation with Phishing and SEO Poisoning Campaign](#topic-10381) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-10344"></a>

### 1. ABB AbilityTM Zenon Remote Transport Vulnerability

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>防御・運用</nobr> / <nobr>政策・規制</nobr> / <nobr>KEV</nobr> / <nobr>認証バイパス</nobr> / <nobr>TTP</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 41.0 |
| <nobr>実務影響</nobr> | 64.0 |
| <nobr>確度</nobr> | 51.0 |

#### 概要

ABBの産業向けソフトウェア「ABB Ability™ zenon」のRemote Transport機能に、認証を回避してOS再起動を引き起こせる脆弱性（CVE-2025-8754）が公表されています。
影響範囲はzenon 7.50から14までとされ、悪用には対象ネットワーク内への到達が前提になるとされています。
産業制御系で認証不要の再起動は、可用性に直接影響しうるため注意が必要です。現時点で広範な野良悪用は確認されていないものの、ネットワーク内侵入後の影響を大きくしうる点が問題です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 対象システムをインターネットや不要なネットワークから分離し、アクセス制御を見直す。
- Remote Transport機能の利用要否を確認し、使わない場合は関連サービスの停止を検討する。
- zenon 7.50〜14を利用している環境では、再起動や不審な操作の監視を強化し、ベンダーの案内を確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-8754 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-8754](https://nvd.nist.gov/vuln/detail/CVE-2025-8754) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [ABB AbilityTM Zenon Remote Transport Vulnerability](https://www.cisa.gov/news-events/ics-advisories/icsa-26-146-03) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-10358"></a>

### 2. Hackers Exploited KnowledgeDeliver Zero-Day for Web Shell Deployment

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ゼロデイ</nobr> / <nobr>RCE</nobr> / <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 41.0 |
| <nobr>実務影響</nobr> | 56.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

KnowledgeDeliver に関するゼロデイ脆弱性が悪用され、Webシェルの設置につながったと報じられています。
公開情報では、設定ファイル内のハードコードされた machineKey が ViewState のデシリアライズ攻撃に利用され、結果としてリモートコード実行に至った可能性が示されています。
ゼロデイの悪用が観測されている点は、被害が拡大する前の早期対応が重要であることを示します。
設定不備や認証まわりの実装が遠隔コード実行につながるため、同種の構成を持つ環境では影響確認が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- KnowledgeDeliver を利用している環境があるかを確認し、関連する製品・設定の影響有無を点検する。
- 設定ファイルや ViewState 関連の保護設定、ハードコードされた機密値の有無を見直す。
- 不審な Web シェル配置や、想定外の管理者権限・プロセス起動など侵害痕跡を点検する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Hackers Exploited KnowledgeDeliver Zero-Day for Web Shell Deployment](https://www.securityweek.com/hackers-exploited-knowledgedeliver-zero-day-for-web-shell-deployment/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-10371"></a>

### 3. AI Threat Landscape Digest March-April 2026

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>AI</nobr> / <nobr>脆弱性</nobr> / <nobr>国家支援</nobr> / <nobr>脅威レポート</nobr> / <nobr>ランサムウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 41.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

2026年3〜4月の脅威動向として、攻撃側でのAI活用が計画支援の段階から、実際の運用に組み込まれる段階へ進んだとされています。
個人の攻撃者、ランサムウェア関連の活動、国家関与が疑われる諜報活動など、複数の文脈で商用AIモデルが長期の攻撃ワークフローに使われた可能性が示されています。
AIが調査や文章生成の補助にとどまらず、攻撃の実行補助や自動化に使われると、攻撃の量と速度が上がるおそれがあります。
防御側は、従来の手口だけでなく、AIを前提にした運用の変化も視野に入れる必要があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIを使った高度な自動化を前提に、検知・封じ込めの判断基準を見直す。
- ランサムウェアや諜報活動を含む複数の脅威文脈で、異常な作業連鎖や短時間の大量試行を監視する。
- Microsoft関連の脆弱性として挙がっている個別CVEは、別途自組織への影響有無を確認して優先度を判断する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-55182 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2025-59536 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-21852 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-34197 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-33626 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [AI Threat Landscape Digest March-April 2026](https://research.checkpoint.com/2026/ai-threat-landscape-digest-march-april-2026/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-10324"></a>

### 4. Anthropic: Claude Mythos identified 10,000+ software flaws

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>脆弱性</nobr> / <nobr>ゼロデイ</nobr> / <nobr>クラウド</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Anthropicは、Project Glasswingの進捗報告の中で、Claude Mythosとその協力先が重要ソフトウェアにおける1万件超の高危険度または重大な脆弱性を見つけたと発表しました。
材料によれば、Claude Mythosはゼロデイ脆弱性の発見やエクスプロイト生成を自律的に行うモデルとして紹介されていますが、個別の検証状況はこの材料だけでは断定できません。
脆弱性の発見をAIが大規模に支援する流れは、診断・検証の効率化につながる一方、悪用可能性のある情報が短時間で大量に把握されうる点で注目されます。
ベンダーや防御側にとっては、発見件数そのものよりも、どの脆弱性が実際に修正・緩和へ結びつくかが重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- AI支援の脆弱性発見結果は、件数だけでなく重複排除や再現性、修正優先度を確認して扱う。
- 重要ソフトウェアに関する報告は、関連ベンダーの修正情報や緩和策の公表を継続監視する。
- ゼロデイや高危険度の文脈では、資産の露出状況を点検し、該当製品の更新適用を急ぐ。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Cisco | 言及あり | 0.80 |
| ai_model_or_project | Anthropic | 主題 | 0.80 |
| ai_model_or_project | Claude Mythos | 主題 | 0.80 |
| ai_model_or_project | Claude | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Anthropic: Claude Mythos identified 10,000+ software flaws](https://www.helpnetsecurity.com/2026/05/26/anthropic-project-glasswing-update/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-10380"></a>

### 5. CERT-In Recommends 12-Hour Patching for Internet-Facing Flaws Amid AI-Assisted Attacks

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>脅威アクター</nobr> / <nobr>脆弱性</nobr> / <nobr>政策・規制</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

インドのCERT-Inが、インターネットに公開されたシステムで見つかった重要な脆弱性について、可能な場合は12時間以内に修正するよう求める方針を示しました。
背景には、攻撃者がAIツールやLLMを使って脆弱性の悪用や自動化を進める可能性への警戒があります。
公開システムの修正猶予を大幅に短縮する考え方は、パッチ運用や緊急対応の優先順位に直接影響します。
AIの活用が攻撃側の速度を押し上げるという前提が広がれば、脆弱性管理の体制見直しが必要になるためです。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 外部公開資産の棚卸しと、重要度の高い脆弱性に対する緊急パッチ手順を再確認する。
- 通常の定期更新とは別に、短時間で判断・適用できる例外対応の連絡経路を整えておく。
- 脆弱性情報の受領から検証、適用、再確認までの所要時間を測り、ボトルネックを把握する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [CERT-In Recommends 12-Hour Patching for Internet-Facing Flaws Amid AI-Assisted A](https://thehackernews.com/2026/05/cert-in-mandates-12-hour-patching-for.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-10381"></a>

### 6. Iran-Linked Hackers Target US Aviation with Phishing and SEO Poisoning Campaign

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>フィッシング</nobr> / <nobr>地政学・サイバー紛争</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>マルウェア</nobr> / <nobr>AI</nobr> / <nobr>国家支援</nobr> |
| <nobr>分類理由</nobr> | AI×Security枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

イランに関連するとされる攻撃者グループが、米国の航空業界を狙ったフィッシングとSEOポイズニングのキャンペーンを展開していると報じられています。
報道では、AIを用いて作成されたとされるバックドア「MiniFast」が利用されているとされていますが、公開情報ベースでは詳細は限定的です。
航空業界は社会インフラとして影響が広く、標的型の侵入が業務や情報資産に波及する可能性があります。
フィッシングと検索経由の誘導は一般ユーザーや担当者が遭遇しやすく、防御側の注意喚起が重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- メール経由の認証情報詐取を想定し、MFAや不審ログインの監視を強化する。
- 検索結果からの誘導先が正規サイトに見えても、外部リンクやダウンロードに注意し、アクセス元の検証を徹底する。
- 航空関連の重要部門では、端末・メール・Webアクセスの監視と、既知の侵害痕跡に対する点検を優先する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Iran-Linked Hackers Target US Aviation with Phishing and SEO Poisoning Campaign](https://www.infosecurity-magazine.com/news/iranian-hackers-us-aviation/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。

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
| [Microsoftが修正したSharePointの高深刻度RCE脆弱性（CVE-2026-45659）](https://thehackernews.com/2026/05/microsoft-patches-sharepoint-rce-flaw.html) | 30.0 | 46.0 | 54.0 |
| [MuddyWaterが9か国を標的とした諜報キャンペーンでDLLサイドローディングを使用](https://thehackernews.com/2026/05/muddywater-uses-dll-side-loading-in.html) | 28.0 | 20.0 | 42.0 |
| [中国の脅威アクターが静的なフィッシングページを捨て、ライブ認証情報窃取へ移行](https://www.infosecurity-magazine.com/news/chinese-phishing-live-credential/) | 28.0 | 20.0 | 42.0 |
| [Iranian APTが航空・ソフトウェア企業を新たなツールで標的にする](https://www.securityweek.com/iranian-apt-targets-aviation-software-companies-with-updated-tools/) | 28.0 | 20.0 | 42.0 |
| [2026年5月の主なサイバー攻撃：偽招待状、Agent Tesla、BlobPhishなど](https://any.run/cybersecurity-blog/major-cyber-attacks-may-2026/) | 28.0 | 20.0 | 42.0 |
| [700以上の教育・技術系サイトが乗っ取られた大規模なClickFixマルウェアキャンペーン](https://www.malwarebytes.com/blog/bugs/2026/05/700-education-and-tech-websites-hijacked-in-huge-clickfix-malware-campaign) | 28.0 | 20.0 | 42.0 |
| [ロシアのハッカーが利用する耐障害性ホスティングサービスの管理者、オランダで逮捕](https://www.securityweek.com/admins-of-bulletproof-hosting-service-used-by-russian-hackers-arrested-in-netherlands/) | 28.0 | 20.0 | 42.0 |
| [Varonis AtlasがClaude Compliance APIを統合してAIガバナンスを強化](https://www.bleepingcomputer.com/news/security/how-varonis-atlas-integrates-claude-compliance-api-for-ai-governance/) | 25.0 | 20.0 | 42.0 |
| [AppOmniのMarlin AI、SaaSセキュリティに自律的な調査機能を導入](https://www.securityweek.com/appomnis-marlin-ai-brings-autonomous-investigation-to-saas-security/) | 25.0 | 20.0 | 42.0 |
| [Detectify、MCP Serverと継続的テストでAIエージェント向けAppSec自動化を実現](https://www.helpnetsecurity.com/2026/05/26/detectify-mcp-server/) | 25.0 | 20.0 | 42.0 |
| [Conifers、AI搭載のSOCを展開し統合セキュリティ運用と自動対応を実現](https://www.helpnetsecurity.com/2026/05/26/conifers-ai-agentic-soc/) | 25.0 | 20.0 | 42.0 |
| [セキュリティリーダーが複雑さを乗り越えて成果を高める方法](https://www.rapid7.com/blog/post/it-security-leaders-cut-through-complexity-driving-stronger-outcomes-webinar) | 25.0 | 20.0 | 42.0 |
| [AIを悪用した新たなDDoS攻撃はより巧妙に、対抗策を学ぶウェビナー](https://thehackernews.com/2026/05/new-ai-ddos-attacks-are-smarter-learn.html) | 25.0 | 20.0 | 42.0 |
| [Anthropic、Claudeのエンタープライズ向けセキュリティガバナンスを28件の新規連携で拡張](https://www.securityweek.com/anthropic-expands-claudes-enterprise-security-reach-with-28-new-integrations/) | 25.0 | 20.0 | 42.0 |
| [Tamnoon、技能ベースのAIオーケストレーションによる自律型クラウド防御を発表](https://www.helpnetsecurity.com/2026/05/26/tamnoon-tami-ai-skills/) | 25.0 | 20.0 | 42.0 |
| [Open Source DockSecがAIでDockerイメージの脆弱性ノイズを削減](https://www.securityweek.com/open-source-docksec-uses-ai-to-cut-through-vulnerability-noise-in-docker-images/) | 25.0 | 20.0 | 42.0 |
| [英国とオーストラリア、AIセキュリティで連携強化へ](https://www.itpro.com/security/uk-and-australia-agree-to-work-more-closely-on-ai-security) | 25.0 | 20.0 | 42.0 |
| [ABB Terra ACにおける脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-146-01) | 24.0 | 46.0 | 50.0 |
| [ABB B&R Automation RuntimeのSystem Diagnostics Manager（SDM）におけるDoS脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-146-04) | 24.0 | 46.0 | 50.0 |
| [ABB Ability Camera Connectの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-146-05) | 24.0 | 46.0 | 50.0 |
| [システム障害が発生、サイバー攻撃の可能性 - 精電舎電子工業](https://www.security-next.com/184290) | 22.0 | 20.0 | 42.0 |
| [県内高校で生徒情報含む連携支援シートを紛失 - 新潟県](https://www.security-next.com/184953) | 22.0 | 20.0 | 42.0 |
| [レンズ交換式もある「GoPro MISSION 1」は映像表現の幅を広げる小さなシネマカメラだった](https://www.itmedia.co.jp/news/articles/2605/26/news118.html) | 21.0 | 20.0 | 42.0 |
| [スクエニ、27日午後10時から「ドラゴンクエストからのお知らせ」プレミア公開](https://www.itmedia.co.jp/news/articles/2605/26/news134.html) | 21.0 | 20.0 | 42.0 |

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
