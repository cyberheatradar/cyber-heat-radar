# 📡 サイレーダー 2026-10-01 11:00 JST

このレポートは、2026-10-01 05:00 JST〜2026-10-01 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 73
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 45

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Threat Brief: NetScaler Zero Days CVE-2026-88771 and CVE-2026-88772 Exploited in the Wild (Updated September 30)](#topic-34525) | 52.0 | 74.0 | 67.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [Apple製品やCiscoのSD-WAN管理製品の脆弱性悪用に注意喚起 - 米当局](#topic-35273) | 39.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Microsoft Malware Protection Engine における任意の特権ファイルの書き込みが可能となるファイル操作での検証不備（Scan Tech Report）](#topic-35282) | 34.0 | 23.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Malicious Custom GPTs Turn ChatGPT Into RAT Delivery Lure](#topic-35332) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-35273"></a>

### 1. Apple製品やCiscoのSD-WAN管理製品の脆弱性悪用に注意喚起 - 米当局

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

米当局が、Apple製品およびCiscoのSD-WAN管理製品に関する脆弱性について、実際の悪用が確認されているとして注意喚起を行いました。
対象製品を利用している組織では、関連情報の確認と対応状況の点検が必要です。脆弱性の存在だけでなく悪用が観測されている点が重要で、被害拡大のリスクが高まります。
製品の性質上、管理系や広く使われる環境に影響しうるため、運用面での影響確認が求められます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Apple製品とCiscoの該当SD-WAN管理製品の利用有無を確認し、ベンダーの修正版や回避策の適用状況を点検する。
- 資産管理情報から、影響を受ける可能性のある端末・管理基盤・関連サービスを洗い出す。
- 異常な認証試行や管理画面への不審なアクセスなど、周辺の監視ログを確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Apple | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Apple製品やCiscoのSD-WAN管理製品の脆弱性悪用に注意喚起 - 米当局](https://www.security-next.com/190890) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35282"></a>

### 2. Microsoft Malware Protection Engine における任意の特権ファイルの書き込みが可能となるファイル操作での検証不備（Scan Tech Report）

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 34.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 23.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Microsoft Malware Protection Engine に、ファイル操作時の検証不備に起因して、任意の特権ファイルを書き込める可能性がある問題が報じられています。
現時点の材料では詳細な影響範囲や悪用の有無は断定できませんが、セキュリティ製品の中核機能に関わるため注目されています。
防御製品側の不備は、端末保護の前提に影響しうるため、通常の脆弱性よりも運用面の警戒が必要です。
特権ファイルへの書き込みが成立する場合、システムへの影響が大きくなる可能性があります。

#### 温度感の理由

##### 温度感
- 技術詳細・再現情報あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 技術詳細により影響確認が進みやすい。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Microsoftの修正情報や関連アドバイザリを確認し、適用対象製品と影響範囲を早めに把握する。
- 保護機能の更新状況を点検し、検知ログや異常なファイル操作の有無を確認する。
- 必要に応じて、影響を受けうる端末の優先度を上げてパッチ適用や再起動計画を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft Malware Protection Engine における任意の特権ファイルの書き込みが可能となるファイル操作での検証不備（Scan Te](https://scan.netsecurity.ne.jp/article/2026/10/01/56364.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-35332"></a>

### 3. Malicious Custom GPTs Turn ChatGPT Into RAT Delivery Lure

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報では、悪意あるカスタムGPTを悪用し、ChatGPT関連の画面や正規ドメインを装って利用者を誘導するキャンペーンが報告されています。
説明では、OpenAIやGoogleの正規サービスに見せかけることで、ユーザーをだまして不正なダウンロードや実行につなげる手口が示唆されています。
生成AIサービスの見た目や信頼性を悪用するため、利用者が警戒しにくい点が問題です。
企業内でAIツールの利用が広がる中、正規サービス名を装った誘導は誤操作やマルウェア感染の入口になり得ます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI関連の案内であっても、外部リンクやダウンロード先の正当性を必ず確認すること。
- ChatGPTやカスタムGPTを名乗る不審な導線について、社内で注意喚起と利用ルールを整備すること。
- WebフィルタやEDRで、正規サービスを装う不審なリダイレクトや実行ファイル取得の兆候を監視すること。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | ChatGPT | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Malicious Custom GPTs Turn ChatGPT Into RAT Delivery Lure](https://www.darkreading.com/cyberattacks-data-breaches/malicious-custom-gpts-chatgpt-rat-delivery-lure) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-34525"></a>

### 1. Threat Brief: NetScaler Zero Days CVE-2026-88771 and CVE-2026-88772 Exploited in the Wild (Updated September 30)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 52.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Citrix NetScaler ADCとGatewayに影響する2件の深刻な脆弱性、CVE-2026-88771とCVE-2026-88772が、実際の攻撃で悪用されていると報告されています。
Citrixは修正済みのセキュリティ更新を公開しており、複数の情報源でもゼロデイとしての悪用が確認されたとされています。
NetScalerは外部公開されやすい境界機器であるため、影響を受ける環境では侵入の足がかりになり得ます。
公開PoCや悪用報告が出ている点から、未修正環境のリスクが相対的に高いとみられます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Citrix NetScaler ADC / Gateway の該当バージョンを確認し、ベンダー提供の修正を適用する。
- インターネット公開中のNetScalerについて、異常な認証・管理操作・通信の痕跡を点検する。
- 周辺ログと監視ルールを見直し、侵害兆候がないか追加確認を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-88771 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-88772 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-88771](https://nvd.nist.gov/vuln/detail/CVE-2026-88771) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: NetScaler Zero Days CVE-2026-88771 and CVE-2026-88772 Exploited in](https://unit42.paloaltonetworks.com/netscaler-zero-days-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Government, Finance Orgs Targeted in Weeks-Long NetScaler Zero-Day Attacks](https://www.securityweek.com/government-finance-orgs-targeted-in-weeks-long-netscaler-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [NetScaler zero-day exploitation escalates into mass attacks (CVE-2026-88771)](https://www.helpnetsecurity.com/2026/09/29/netscaler-zero-day-exploitation-escalates-into-mass-attacks-cve-2026-88771/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix patches actively exploited NetScaler zero-days after a weekend of unoffic](https://cyberscoop.com/citrix-zero-days-delayed-disclosure/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-88771 and CVE-2026-88772: Two Critical Citrix NetScaler Flaws Under Act](https://www.bitsight.com/blog/critical-vulnerability-alert-cve-2026-88771-cve-2026-88772-citrix-netscaler-flaws-under-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zero-Day Exploitation of Citrix NetScaler ADC and Gateway: CVE-2026-88771 and CV](https://www.rapid7.com/blog/post/etr-zero-day-exploitation-of-citrix-netscaler-adc-and-gateway-cve-2026-88771-and-cve-2026-88772) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix NetScaler RCE zero-days exploited globally for weeks (CVE-2026-88771, CVE](https://www.helpnetsecurity.com/2026/09/28/citrix-netscaler-rce-zero-days-exploited-for-weeks-cve-2026-88771-cve-2026-88772/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（2件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [何者？ ランサムウェア集団を攻撃するサイバー犯罪集団「ShinyHunters」 FBI捜査官の個人情報窃取も主張](https://www.itmedia.co.jp/news/article/2610/01/2000001847/) | 29.0 | 30.0 | 42.0 |
| [急増する「DeadLock」による被害 感染後すぐに1対1のチャットに誘導](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/041600214/091400020/) | 29.0 | 30.0 | 42.0 |
| [ATMマルウェア計画に関与したTren de Aragua関連の10人に米国が制裁](https://therecord.media/us-sanctions-10-atm-jackpotting-tren-de-aragua) | 28.0 | 20.0 | 42.0 |
| [ロシアの国家支援ハッカーが新たなRedFlick手法でマルウェアを配布](https://www.bleepingcomputer.com/news/security/russian-state-hackers-use-new-redflick-technique-to-push-malware/) | 28.0 | 20.0 | 42.0 |
| [デルが強調する「OSより下のレイヤー保護」--生成AIで脅威増すエンドポイント防御](https://japan.zdnet.com/article/35253125/) | 26.0 | 20.0 | 42.0 |
| [Google、「Gemini 4 Pro」ではなく「Gemini 4 Agron」発表 まずはサイバー防御組織に限定提供、出力上限は100万トークンに](https://www.itmedia.co.jp/news/article/2610/01/2000001912/) | 26.0 | 20.0 | 42.0 |
| [シャープがAIサーバーの受注を開始 2030年度に売上高2500億円目指す](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/092401500/) | 26.0 | 20.0 | 42.0 |
| [Claude Codeの「ごまかし」に直面 マネージド版と併用で乗り切る](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/091300255/091300003/) | 26.0 | 20.0 | 42.0 |
| [生成AI＋「手足」＝AIエージェント 1年半前のClaude Code登場でブレーク](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/091300255/091300001/) | 26.0 | 20.0 | 42.0 |
| [AI出力文に「電子透かし」 EU規制受けアンソロピックが導入](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/092401505/) | 26.0 | 20.0 | 42.0 |
| [OpenAIが「ChatGPT Space」を発表--「Google Workspace」の代替ツールか](https://japan.zdnet.com/article/35253115/) | 26.0 | 20.0 | 42.0 |
| [SELECT権限からSYSADMIN権限へ昇格するSQL Copilotの脆弱性（CVE-2026-65669）](https://embracethered.com/blog/posts/2026/from-select-to-sysadmin-sql-copilot-bluehat-asia/) | 25.0 | 43.0 | 51.0 |
| [FTC、OpenAIとAnthropicに対する消費者への潜在的リスクを調査](https://www.securityweek.com/ftc-is-investigating-openai-and-anthropic-over-possible-risks-to-consumers/) | 25.0 | 20.0 | 42.0 |
| [OpenAIが明らかにした蒸留攻撃で使われた新たな暗号回避手法](https://cyberscoop.com/openai-moonshot-ai-model-distillation-attack/) | 25.0 | 20.0 | 42.0 |
| [OpenAIが他社から学習した技術を中国製モデルに盗用されたと主張し波紋](https://www.theregister.com/security/2026/09/30/irony-alert-openai-whines-that-chinese-model-stole-its-special-ip-that-it-stole-from-everybody-else/5300285) | 25.0 | 20.0 | 42.0 |
| [Trumpとテック大手、AI安全確保に向けた自主協定を締結](https://www.darkreading.com/cyber-risk/trump-tech-giants-strike-voluntary-ai-safety-accord) | 25.0 | 20.0 | 42.0 |
| [「Apache WSS4J」に認証回避など7件の脆弱性 - 修正版が公開](https://www.security-next.com/190893) | 22.0 | 20.0 | 42.0 |
| [「Catalyst SD-WAN Manager」にゼロデイ脆弱性 - 更新や侵害調査を](https://www.security-next.com/190883) | 22.0 | 20.0 | 42.0 |
| [ビル・ゲイツが「AI規制はサイバー攻撃やバイオテロを防ぐために必要」「AIは人間の仕事を奪う」とインタビューで語る](https://gigazine.net/news/20261001-bill-gates-warning-ai-ezra-klein/) | 22.0 | 20.0 | 42.0 |
| [AIと自動化がクラウド攻撃チェーンを加速（2026年クラウドネイティブ脅威動向レポートより）](https://ascii.jp/elem/000/004/437/4437872/?rss=) | 21.0 | 20.0 | 42.0 |
| [人材不足に打ち勝つセキュリティ運用とは ～ DNP との対談で明かされる効果、テクマトリックスが Palo Alto Networks の Cortex XSIAM で提案する次世代 SOC](https://scan.netsecurity.ne.jp/article/2026/10/01/56363.html) | 21.0 | 20.0 | 42.0 |
| [AWS WAF の保守運用にお悩みの方向け ～ 継続的ルール調整・誤検知対応を実現するオンラインセミナーを GMOイエラエが 10 / 7 開催](https://scan.netsecurity.ne.jp/article/2026/10/01/56362.html) | 21.0 | 20.0 | 42.0 |
| [「クロネコ代金後払いサービス」に不正アクセス](https://scan.netsecurity.ne.jp/article/2026/10/01/56361.html) | 21.0 | 20.0 | 42.0 |
| [「タイムズカー」に不正アクセス、運転免許証画像含む会員情報が第三者に取得されたことを確認](https://scan.netsecurity.ne.jp/article/2026/10/01/56360.html) | 21.0 | 20.0 | 42.0 |
| [スターツ出版「オズモール」に不正アクセス、会員のメールアドレス 最大447,610名分が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/10/01/56359.html) | 21.0 | 20.0 | 42.0 |
| [「ニッポンレンタカーアプリ」への不正アクセス、運転免許証情報が閲覧されたおそれも](https://scan.netsecurity.ne.jp/article/2026/10/01/56358.html) | 21.0 | 20.0 | 42.0 |
| [CMSプラグインの脆弱性公表を受け更新作業中に不正アクセスを発見](https://scan.netsecurity.ne.jp/article/2026/10/01/56357.html) | 21.0 | 20.0 | 42.0 |
| [当選が落選に「ULTRA MART」チケット抽選システムに不正アクセス](https://scan.netsecurity.ne.jp/article/2026/10/01/56356.html) | 21.0 | 20.0 | 42.0 |
| [「RESPECTion!シンポジウム」参加申込フォームに設定不備、他の申込者の回答内容が閲覧可能に](https://scan.netsecurity.ne.jp/article/2026/10/01/56355.html) | 21.0 | 20.0 | 42.0 |
| [NetScaler ADC および NetScaler Gateway に脆弱性、世界中で脅威アクターが積極的に悪用との情報](https://scan.netsecurity.ne.jp/article/2026/10/01/56354.html) | 21.0 | 20.0 | 42.0 |
| [Apache Tomcat に複数の脆弱性](https://scan.netsecurity.ne.jp/article/2026/10/01/56353.html) | 21.0 | 20.0 | 42.0 |
| [IPA、情報セキュリティ早期警戒パートナーシップガイドライン改訂案を公開](https://scan.netsecurity.ne.jp/article/2026/10/01/56352.html) | 21.0 | 20.0 | 42.0 |
| [C&Cサーバ検知共有スキームを実践フェーズへ、通信事業者らによる注意喚起・フィルタリング試行](https://scan.netsecurity.ne.jp/article/2026/10/01/56351.html) | 21.0 | 20.0 | 42.0 |
| [GMOサイバーセキュリティ byイエラエ、国際宇宙会議（IAC 2026）で衛星セキュリティ研究やデモを出展](https://scan.netsecurity.ne.jp/article/2026/10/01/56350.html) | 21.0 | 20.0 | 42.0 |
| [HENNGE がラグビーチーム「リコーブラックラムズ東京」とのオフィシャルパートナー契約を締結、公式戦ウェア背面にロゴ掲出](https://scan.netsecurity.ne.jp/article/2026/10/01/56349.html) | 21.0 | 20.0 | 42.0 |
| [「Gポイント」不正アクセスで一時停止 「会員識別子」約7万件漏えいか KDDI不正会計問題のジー・プランが運営](https://www.itmedia.co.jp/news/article/2610/01/2000001913/) | 21.0 | 20.0 | 42.0 |
| [すべての企業の“セキュリティ疲れ”解消を 「Symantec CBX」TD SYNNEXが提供開始](https://ascii.jp/elem/000/004/438/4438868/?rss=) | 21.0 | 20.0 | 42.0 |
| [日立、社会基盤事業「HMAX」拡充 DC運用やサイバー防御など](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/092401501/) | 21.0 | 20.0 | 42.0 |
| [オンプレミス回帰とディープテック人材の需要増がトレンドに--シスコ幹部が理由を解説](https://japan.zdnet.com/article/35253094/) | 21.0 | 20.0 | 42.0 |
| [インフォスティーラーの恐怖【前編】～認証を済ませた、その後が狙われるということの意味～](https://japan.zdnet.com/article/35252976/) | 21.0 | 20.0 | 42.0 |
| [佐川急便の荷物追跡サービスに不正アクセス 利用を一部制限](https://www.itmedia.co.jp/news/article/2610/01/2000001911/) | 21.0 | 20.0 | 42.0 |
| [機器破壊やデータ盗難など悪い事態を引き起こす恐れがあるUSB製品5選](https://japan.zdnet.com/article/35252909/) | 21.0 | 20.0 | 42.0 |
| [「能動的サイバー防御」のため、基幹インフラ事業者ら約100組織による協議会設置](https://internet.watch.impress.co.jp/docs/news/2144657.html) | 20.0 | 20.0 | 42.0 |
| [【注目記事】本日から関連法施行、「能動的サイバー防御」で何が変わる？](https://internet.watch.impress.co.jp/docs/readitnow/2144633.html) | 20.0 | 20.0 | 42.0 |
| [セイコーマート、会員のほぼ半数に当たる情報漏えい 約57万人分](https://www.itmedia.co.jp/news/article/2609/30/2000001906/) | 16.0 | 20.0 | 42.0 |

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
