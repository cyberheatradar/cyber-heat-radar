# 📡 サイレーダー 2026-09-27 05:00 JST

このレポートは、2026-09-26 17:00 JST〜2026-09-27 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 36
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 9

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Attackers Bypass WAFs to Exploit Oracle PeopleSoft Flaw and Deploy Web Shells](#topic-16788) | 48.0 | 67.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [New x47.c Windows Botnet Weaponizes xAI Grok, AI API Draining](#topic-34489) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-16788"></a>

### 1. Attackers Bypass WAFs to Exploit Oracle PeopleSoft Flaw and Deploy Web Shells

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 48.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 67.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Oracle PeopleSoftの脆弱性CVE-2026-35273について、実際の悪用が確認されていると複数の情報源が伝えています。
認証なしでリモートコード実行につながる可能性があるとされ、Webシェルの設置などにつながる事例が報告されています。
基幹業務で使われる製品の脆弱性が、公開後まもなく実悪用されている点が重要です。CISAの既知悪用脆弱性リストにも追加されており、早急な対応が求められます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 9 sources。
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

- Oracleの公式アドバイザリと修正状況を確認し、適用可能なパッチを優先的に適用する。
- PeopleSoft環境の外部公開状況、認証要件、アクセス制御を見直し、不要な露出を減らす。
- 関連ホストの不審なファイル配置、Webシェル痕跡、認証失敗や異常な管理操作のログを点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-35273 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-41091 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-45657 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-50507 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ランサムウェアグループ | Clop | 主題 | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Oracle | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-35273](https://nvd.nist.gov/vuln/detail/CVE-2026-35273) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Attackers Bypass WAFs to Exploit Oracle PeopleSoft Flaw and Deploy Web Shells](https://thehackernews.com/2026/09/attackers-bypass-wafs-to-exploit-oracle.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [15th June – Threat Intelligence Report](https://research.checkpoint.com/2026/15th-june-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShinyHunters is actively extorting universities after exploiting an unpatched Or](https://cyberscoop.com/oracle-peoplesoft-zero-day-vulnerability-shinyhunters-extortion/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Active Exploitation of Oracle PeopleSoft Zero-Day (CVE-2026-35273)](https://www.rapid7.com/blog/post/etr-active-exploitation-of-oracle-peoplesoft-zero-day-cve-2026-35273) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/06/12/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google Confirms Exploitation of Oracle PeopleSoft Zero-Day by ShinyHunters](https://www.securityweek.com/google-confirms-exploitation-of-oracle-peoplesoft-zero-day-by-shinyhunters/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShinyHunters Exploits Oracle PeopleSoft Zero-Day (CVE-2026-35273) to Breach Univ](https://thehackernews.com/2026/06/shinyhunters-exploits-oracle-peoplesoft.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-34489"></a>

### 2. New x47.c Windows Botnet Weaponizes xAI Grok, AI API Draining

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、Windows向けのボットネット「x47.c」がAIサービスのxAI Grokを利用して、あらかじめ用意された行動から選択しながら動作を継続しているとされています。
あわせて、AI APIの利用を大量に消費するような挙動も示唆されており、攻撃とサービス濫用の両面で注目されています。
AIサービスが攻撃の自動化や継続運用に組み込まれると、従来の不正通信監視だけでは把握しにくい形で悪用が進む可能性があります。
さらに、正規APIの利用が絡むため、検知や費用管理の観点でも影響が出やすい点が注目されます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI APIの利用状況を監視し、想定外の呼び出し増加や利用パターンの偏りを確認する。
- 端末側では、ボットネット由来の持続化や不審な自動実行の兆候を通常のマルウェア対策と合わせて点検する。
- AI機能を業務で使う環境では、APIキー管理、利用上限、監査ログの確認を徹底する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | xAI | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | xAI Grok | 主題 | 0.80 | — |
| AIモデル/プロジェクト | Grok | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New x47.c Windows Botnet Weaponizes xAI Grok, AI API Draining](https://www.securityweek.com/new-x47-c-windows-botnet-weaponizes-xai-grok-ai-api-draining/) | <nobr>内容確認・補足情報</nobr> |

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
| [ShinyHuntersがOracle PeopleSoft攻撃でWAF回避の手口を使用](https://www.bleepingcomputer.com/news/security/shinyhunters-uses-waf-bypass-trick-in-oracle-peoplesoft-attacks/) | 28.0 | 20.0 | 42.0 |
| [Lunex StealerがAMDドライバを悪用してセキュリティ監視を無効化し、ブラウザ認証情報を窃取](https://thehackernews.com/2026/09/lunex-stealer-abuses-amd-driver-to.html) | 28.0 | 20.0 | 42.0 |
| [GitHub Actionsが再有効化、Mini Shai-Huludペイロードはなおも活動中](https://www.bleepingcomputer.com/news/security/github-actions-re-enabled-with-mini-shai-hulud-payload-still-active/) | 28.0 | 20.0 | 42.0 |
| [中国と米国、AI安全対話の窓口設置と貿易・軍事協議の継続で合意](https://www.securityweek.com/china-and-us-agree-to-establish-ai-safety-channel-and-continue-trade-and-military-talks/) | 25.0 | 20.0 | 42.0 |
| [Claude Opus 5.5は長文回答になりつつも、ダッシュの使用を95％削減](https://www.bleepingcomputer.com/news/artificial-intelligence/claude-opus-55-uses-95-percent-fewer-em-dashes-but-its-answers-are-getting-longer/) | 25.0 | 20.0 | 42.0 |
| [OpenAIのAIエージェントがユーザー提供画像を第三者サイトに誤ってアップロード](https://www.bleepingcomputer.com/news/artificial-intelligence/openais-ai-agents-accidentally-uploaded-user-provided-images-to-third-party-sites/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントのゼロトラストはゼロ可視性の解消から始まる](https://thehackernews.com/2026/09/zero-trust-for-ai-agents-starts-with.html) | 25.0 | 20.0 | 42.0 |
| [OpenAIが新たなモデルの不適切動作開示で米政府サイトに関与したと発表](https://www.securityweek.com/openai-says-its-models-engaged-with-us-government-websites-in-new-model-misbehavior-disclosure/) | 25.0 | 20.0 | 42.0 |
| [ElementorのCSRF脆弱性により、管理者のクリック後にサイトを乗っ取られる可能性](https://thehackernews.com/2026/09/elementor-csrf-flaw-lets-attackers-take.html) | 24.0 | 38.0 | 42.0 |

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
