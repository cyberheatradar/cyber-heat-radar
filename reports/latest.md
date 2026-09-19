# 📡 サイレーダー 2026-09-20 05:00 JST

このレポートは、2026-09-19 17:00 JST〜2026-09-20 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 39
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 13

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [米当局、「Linuxカーネル」の脆弱性3件を悪用リストに追加](#topic-33538) | 39.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [Critical Pre-Auth RCE in Orkes Conductor Workflow Platform Exploited in the Wild](#topic-33505) | 37.0 | 64.0 | 55.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-33538"></a>

### 1. 米当局、「Linuxカーネル」の脆弱性3件を悪用リストに追加

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

米当局が、Linuxカーネルに存在する3件の脆弱性について、実際に悪用されているとして注意喚起を行いました。
行政機関に対しては、対象システムの確認と早急な対応が求められています。基盤となるLinuxカーネルの脆弱性が悪用対象に含まれると、広範なシステムに影響が及ぶ可能性があります。
公的機関が注意喚起している点からも、優先度の高い対応が必要とみられます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 利用中のLinuxカーネル版と適用済み更新の有無を確認する。
- ベンダーや配布元の修正版・緩和策の案内を確認し、優先的に適用する。
- 対象サーバーや重要端末で不審な挙動がないか、監視とログ確認を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-39964 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 製品 | Linux kernel | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [米当局、「Linuxカーネル」の脆弱性3件を悪用リストに追加](https://www.security-next.com/190557) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33505"></a>

### 2. Critical Pre-Auth RCE in Orkes Conductor Workflow Platform Exploited in the Wild

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>R⁠C⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

Orkes Conductor に関する重大な脆弱性 CVE-2026-58138 について、公開情報では実際の攻撃で悪用されているとされています。
認証なしでリモートコード実行につながる可能性があると報告されており、影響範囲の大きい問題として扱われています。
認証前に任意コード実行へつながる類型は、侵害成立までの障壁が低く、公開済み製品の防御優先度が高いです。
すでに悪用観測があるとされるため、通常の脆弱性情報よりも早急な対応が求められます。

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

- Orkes Conductor の該当バージョン利用有無を確認し、ベンダー案内に沿って修正済み版への更新を優先する。
- 外部公開された管理・ワークフロー関連の入口を洗い出し、不要な露出を減らす。
- 関連ログを点検し、想定外のワークフロー定義や不審な実行痕跡がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-58138 | 関連CVE | 1.00 | 候補あり（URL 5件以上） |
| ベンダー | Fortinet | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-58138](https://nvd.nist.gov/vuln/detail/CVE-2026-58138) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Critical Pre-Auth RCE in Orkes Conductor Workflow Platform Exploited in the Wild](https://thehackernews.com/2026/09/critical-pre-auth-rce-in-orkes.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Orkes Conductor Vulnerability Exploited in Attacks](https://www.securityweek.com/critical-orkes-conductor-vulnerability-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |

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
| [無料でAIエージェントの追跡・評価・プロンプト管理・本番環境の監視ができる「Opik」、セルフホスト可能](https://gigazine.net/news/20260919-opik/) | 29.0 | 20.0 | 42.0 |
| [ShinyHuntersがClopのリークサイトを侵害し、ランサムウェアグループを脅迫](https://www.bleepingcomputer.com/news/security/shinyhunters-hacks-clop-leak-site-threatens-to-extort-ransomware-gang/) | 28.0 | 30.0 | 42.0 |
| [悪意ある拡張機能を通じてAIブラウザエージェントを乗っ取るBragJack攻撃](https://www.bleepingcomputer.com/news/security/bragjack-attacks-hijack-ai-browser-agents-through-malicious-extensions/) | 27.0 | 20.0 | 42.0 |
| [VRAM容量32GBで30万円未満なIntelグラボ「Intel Arc Pro B70 Creator 32GB」でローカルLLM「Qwen3.8 27B」や動画生成AI「MiniMax H3」を実行して生成速度を確かめてみた](https://gigazine.net/news/20260919-arc-pro-b70-llm-review/) | 27.0 | 20.0 | 42.0 |
| [Claude Opus 5が連鎖的な脆弱性を悪用してOpenAIスタッフのアカウントを乗っ取るのを研究者が確認](https://thehackernews.com/2026/09/claude-opus-5-helped-researchers-take.html) | 25.0 | 20.0 | 42.0 |
| [バイラルAI女優Tilly Norwoodを呼び出すには顔スキャンへの同意が必要](https://www.bleepingcomputer.com/news/security/calling-viral-ai-actress-tilly-norwood-agree-to-a-face-scan-first/) | 25.0 | 20.0 | 42.0 |
| [Viral AI女優のホットラインが全通話者の顔をスキャンし、感情を監視している](https://www.bleepingcomputer.com/news/security/viral-ai-actress-hotline-face-scans-every-caller-watches-their-mood/) | 25.0 | 20.0 | 42.0 |
| [SolarWindsのARMに存在するハードコードされた鍵の脆弱性を修正、認証不要のRCEが可能に](https://thehackernews.com/2026/09/solarwinds-patches-arm-hard-coded-key.html) | 24.0 | 46.0 | 50.0 |
| [TigerByte Cyberが300万ドルの資金調達を実施しステルスから登場](https://www.securityweek.com/tigerbyte-cyber-emerges-from-stealth-with-3-million-in-funding/) | 20.0 | 20.0 | 42.0 |
| [Agentic Securityは誰か賢いスタートアップが解決すべき10億ドル規模の課題](https://www.theregister.com/security/2026/09/19/agentic-security-is-the-billion-dollar-challenge-for-some-clever-startup-to-solve/5297546) | 20.0 | 20.0 | 42.0 |
| [北朝鮮系のWaterPlumハッカーが世界中で3万台の端末に感染させる](https://www.bleepingcomputer.com/news/security/north-korean-waterplum-hackers-infected-30-000-devices-worldwide/) | 20.0 | 20.0 | 42.0 |
| [2026年のID可視化：アイデンティティセキュリティの基盤](https://thehackernews.com/2026/09/identity-visibility-in-2026-foundation.html) | 20.0 | 20.0 | 42.0 |
| [新しいCVEが攻撃者より先に悪用可能だと証明できるか？このウェビナーで学ぶ方法](https://thehackernews.com/2026/09/can-you-prove-new-cve-is-exploitable.html) | 10.0 | 20.0 | 42.0 |

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
