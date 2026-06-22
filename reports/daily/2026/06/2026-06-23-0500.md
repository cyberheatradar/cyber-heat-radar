# 📡 サイレーダー 2026-06-23 05:00 JST

このレポートは、2026-06-22 17:00 JST〜2026-06-23 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 80
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 51

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [One intrusion, two cyberattackers: Uncovering parallel threat activity](#topic-18615) | 38.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 2 | [Beyond the Pitch: Assessing Cyber Risks to the 2026 FIFA World Cup](#topic-18605) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [⚡ Weekly Recap: Browser Bugs, EDR Killers, TV Botnet, OpenBSD Flaw, Android Trojan, and More](#topic-18656) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Microsoft Attributes Mastra AI Supply Chain Attack to North Korea](#topic-18649) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [What the Latest ShinyHunters Breaches Reveal About Modern Cyberattacks](#topic-18659) | 30.0 | 20.0 | 43.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-18615"></a>

### 1. One intrusion, two cyberattackers: Uncovering parallel threat activity

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 38.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftのセキュリティブログは、1件の侵害に対して2つの攻撃者が並行して関与していたとみられる事例を取り上げています。
ランサムウェア事案の文脈で、手口や回避策が重なり合うと、単独の兆候だけでは全体像を見誤る可能性があることを示しています。
攻撃活動が一つのグループに限定されない場合、検知や調査で関連事象を切り分けにくくなります。こうした重層的な侵入は、初動対応や被害範囲の把握に影響するため注目されています。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 単発のアラートで判断せず、認証・横展開・永続化など周辺の痕跡を含めて相関確認する。
- 同時期に見つかる異なるTTPや不自然な重複痕跡があれば、別系統の活動として分けて評価する。
- ランサムウェア対応では、侵入経路の特定だけでなく、複数主体の関与可能性を前提に封じ込め範囲を広めに見積もる。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [One intrusion, two cyberattackers: Uncovering parallel threat activity](https://www.microsoft.com/en-us/security/blog/2026/06/22/one-intrusion-two-cyberattackers-uncovering-parallel-threat-activity/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-18605"></a>

### 2. Beyond the Pitch: Assessing Cyber Risks to the 2026 FIFA World Cup

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>通⁠信⁠基⁠盤</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

2026年のFIFAワールドカップを取り巻くサイバーリスクについて、スポーツ、交通、宿泊、通信、金融、政府など幅広い分野が標的になり得ると整理されています。
公開されている脅威インテリジェンスでは、破壊的マルウェア、情報窃取型、ランサムウェアなど複数の脅威が想定されているとされています。
大会は開催国3か国・複数都市にまたがるため、1つの組織だけでなく周辺の重要インフラやサービス提供者まで影響が及ぶ可能性があります。
大規模イベントは注目度が高く、妨害、金銭目的、情報収集など複数の動機が重なりやすい点が警戒されています。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 大会運営に関わる組織は、業務停止に直結するランサムウェア対策としてバックアップ、復旧手順、権限管理を再点検する。
- 交通・宿泊・通信などの委託先や関連事業者も含め、サプライチェーン全体の可視化とインシデント連絡経路を確認する。
- 大会期間中は監視体制を強化し、認証情報の流出、フィッシング、重要システムへの不審なアクセスを重点的に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ransomware_group | BlackCat | 主題 | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Beyond the Pitch: Assessing Cyber Risks to the 2026 FIFA World Cup](https://blog.polyswarm.io/beyond-the-pitch-assessing-cyber-risks-to-the-2026-fifa-world-cup) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-18656"></a>

### 3. ⚡ Weekly Recap: Browser Bugs, EDR Killers, TV Botnet, OpenBSD Flaw, Android Trojan, and More

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠n⁠d⁠r⁠o⁠i⁠d</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

今週の脅威動向として、ブラウザの不具合、EDRを無効化しようとする攻撃、TV機器を狙うボットネット、OpenBSDの脆弱性、Androidトロイの木馬などがまとめられています。
内容全体としては、偽ツールや不正な拡張機能、脆弱な認証情報、WordPressサイトの悪用といった、既知の手口が引き続き使われていることが示されています。
単発の出来事というより、複数の攻撃面にまたがって同種のリスクが継続している点が重要です。防御側はブラウザ、端末、モバイル、Web基盤を横断して点検する必要があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ブラウザ拡張機能や配布元不明のツールに広い権限を与えていないか確認する。
- EDRや管理ツールの停止・改変を狙う挙動を前提に、検知と復旧手順を見直す。
- WordPressやモバイル端末を含め、更新状況と認証情報の管理を再点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [⚡ Weekly Recap: Browser Bugs, EDR Killers, TV Botnet, OpenBSD Flaw, Android Troj](https://thehackernews.com/2026/06/weekly-recap-browser-bugs-edr-killers.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-18649"></a>

### 4. Microsoft Attributes Mastra AI Supply Chain Attack to North Korea

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>サ⁠プ⁠ラ⁠イ⁠チ⁠ェ⁠ー⁠ン</nobr> / <nobr>A⁠I</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftのセキュリティ研究者が、Mastraを狙ったサプライチェーン攻撃に北朝鮮系とされる脅威アクター「Sapphire Sleet」が関与したとしています。
現時点では公開情報ベースの報告であり、詳細な影響範囲や被害の全容は不明です。
AI関連の開発基盤や依存関係を狙うサプライチェーン攻撃は、下流の利用者にも影響が波及し得るため注目されています。
脅威アクターの帰属が示されている点からも、継続的な監視と検証が重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 利用しているAI/開発系パッケージや依存関係に不審な変更がないか確認する。
- ベンダーやコミュニティの注意喚起、更新情報を継続的に追う。
- 導入済みコンポーネントの整合性確認と、更新時のレビュー手順を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft Attributes Mastra AI Supply Chain Attack to North Korea](https://www.infosecurity-magazine.com/news/mastra-ai-supply-chain-attack/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-18659"></a>

### 5. What the Latest ShinyHunters Breaches Reveal About Modern Cyberattacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

SecurityWeekは、ShinyHuntersに関連する最新の侵害事例を通じて、攻撃者がマルウェアやゼロデイ脆弱性に依存しなくても大きな被害を与え得る点を指摘しています。
高度な技術攻撃だけでなく、より幅広い手口が企業被害につながる可能性を示す話題です。
防御側にとっては、脆弱性対策だけでは不十分で、認証情報の管理や権限、運用面の統制も含めた対策が重要であることを示します。
攻撃の入口が限定されないため、監視と検知の範囲を広く見直す必要があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 認証情報の漏えい・使い回し・多要素認証の有無を重点的に確認する。
- 不審なログインや権限昇格、設定変更などの運用イベントを監視対象に含める。
- 外部公開サービスや委託先経由のリスクも含め、アカウント管理とアクセス権限を定期点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [What the Latest ShinyHunters Breaches Reveal About Modern Cyberattacks](https://www.securityweek.com/what-the-latest-shinyhunters-breaches-reveal-about-modern-cyberattacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

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
| [ShapedPlugin WordPress Proプラグインがサプライチェーン攻撃でバックドア化](https://thehackernews.com/2026/06/shapedplugin-wordpress-pro-plugins.html) | 28.0 | 45.0 | 42.0 |
| [GentleKiller Frameworkが被害者のセキュリティソフトを無効化](https://www.infosecurity-magazine.com/news/gentlekiller-gentlemen-ransomware/) | 28.0 | 30.0 | 42.0 |
| [精巧な偽評価向上キャンペーンを悪用した暗号資産窃取事件](https://www.darkreading.com/cyberattacks-data-breaches/crypto-heist-fake-reputation-boosting-campaign) | 28.0 | 20.0 | 42.0 |
| [AryStingerボットネットに制御された数千台のD-Linkルーター](https://www.malwarebytes.com/blog/news/2026/06/thousands-of-d-link-routers-under-control-of-arystinger-botnet) | 28.0 | 20.0 | 42.0 |
| [CISAがFortinetの認証情報流出を受けてデバイスの強化を呼びかけ](https://www.cybersecuritydive.com/news/cisa-device-hardening-thousands-fortinet-credentials-compromised/823397/) | 28.0 | 20.0 | 42.0 |
| [新たなOXLOADERローダーが悪意あるGoogle広告を悪用してCastleStealerを配布](https://thehackernews.com/2026/06/new-oxloader-loader-uses-malicious.html) | 28.0 | 20.0 | 42.0 |
| [WhatsApp経由で拡散されるVBScriptキャンペーンによるRMMソフトウェアの展開](https://securelist.com/whatsapp-vbs-rmm-campaign/120290/) | 28.0 | 20.0 | 42.0 |
| [Gizmodoの読者がアカウント侵害後にClickFixマルウェアのプロンプト被害に遭遇](https://www.theregister.com/security/2026/06/22/gizmodo-readers-hit-with-clickfix-malware-prompts-after-account-compromise/5259226) | 28.0 | 20.0 | 42.0 |
| [Fortinet、FortiBleedキャンペーンに対応](https://www.securityweek.com/fortinet-responds-to-fortibleed-campaign/) | 28.0 | 20.0 | 42.0 |
| [カナダのスパイ機関、ボットネット感染端末の駆除に初の令状を使用](https://thehackernews.com/2026/06/canadas-spy-agency-used-first-of-its.html) | 28.0 | 20.0 | 42.0 |
| [NCSCがFortinet顧客にFortiBleedの影響への対処を促す](https://www.infosecurity-magazine.com/news/ncsc-fortinet-customers-tackle/) | 28.0 | 20.0 | 42.0 |
| [アメリカ政府がAnthropicの「Claude Mythos」の規制命令を下すもAnthropicが選定した「Project Glasswing」のメンバーにはプレビュー版が提供されたままであるという報道](https://gigazine.net/news/20260622-mythos-still-access/) | 27.0 | 20.0 | 42.0 |
| [AIを高速実行するためのx86拡張命令「ACE」の仕様が発表される](https://gigazine.net/news/20260622-ace-x86-ai-computation-extensions/) | 27.0 | 20.0 | 42.0 |
| [OpenAI Daybreak Cyber Partner Programで信頼できるパートナーに選定されたTrendAI™](https://newsroom.trendmicro.com/2026-06-22-TrendAI-TM-Named-Trusted-Partner-in-the-OpenAI-Daybreak-Cyber-Partner-Program) | 25.0 | 20.0 | 42.0 |
| [DifyのDifyTapの脆弱性によりテナント間でAIチャットが漏えいする可能性](https://thehackernews.com/2026/06/researchers-detail-difytap-flaws-in.html) | 25.0 | 20.0 | 42.0 |
| [Intel機関：Frontier AIモデルが予想以上の速さでサイバーセキュリティを変革する](https://cyberscoop.com/five-eyes-alliance-say-advanced-ai-hacking-models-months-away/) | 25.0 | 20.0 | 42.0 |
| [ITチームはAIツールに前向きだが、セキュリティ対策が追いつかないことを懸念している](https://www.itpro.com/security/it-teams-are-bullish-on-ai-tools-but-theyre-worried-security-practices-cant-keep-pace) | 25.0 | 20.0 | 42.0 |
| [AIシフトがもたらすサイバーリスクと、リーダーが今すぐ行動すべき理由](https://www.ncsc.gov.uk/news/the-ai-shift-in-cyber-risk-why-leaders-must-act-now) | 25.0 | 20.0 | 42.0 |
| [レガシーインフラがAIエージェントを乗っ取らないようにする方法](https://thehackernews.com/2026/06/stop-your-legacy-infrastructure-from.html) | 25.0 | 20.0 | 42.0 |
| [AIが企業のデータリスクを変革する中、セキュリティ責任者はどう対応しているか](https://www.cybersecuritydive.com/spons/ai-is-transforming-enterprise-data-risk-heres-how-security-leaders-are-re/823180/) | 25.0 | 20.0 | 42.0 |
| [AIがセキュリティ運用を変革する3つの方法と、実際に効果を発揮する領域](https://www.cybersecuritydive.com/spons/3-ways-ai-is-transforming-security-operations-and-where-it-delivers-real/822590/) | 25.0 | 20.0 | 42.0 |
| [23件のClawHubプラグインが公式スコープを横取りし、AIレジストリのセキュリティ上の欠陥を露呈](https://www.helpnetsecurity.com/2026/06/22/clawhub-code-executing-plugins-video/) | 25.0 | 20.0 | 42.0 |
| [PAN-OSの脆弱性により認証回避が可能になるおそれ](https://www.cisecurity.org/advisory/a-vulnerability-in-pan-os-could-allow-for-authentication-bypass_2026-062) | 24.0 | 38.0 | 42.0 |
| [「映像のまち・かわさき」関連サイトで障害 - 攻撃受けた可能性](https://www.security-next.com/186190) | 22.0 | 20.0 | 42.0 |
| [医療機関向けの補助金案内メールで誤送信 - 大阪市](https://www.security-next.com/186076) | 22.0 | 20.0 | 42.0 |
| [行政文書の個人情報、墨塗りせず交付 - 神奈川県](https://www.security-next.com/186135) | 22.0 | 20.0 | 42.0 |
| [Appleの起動防御を回避する新たな攻撃手法、数百万台のiPhoneに影響](https://www.securityweek.com/new-exploit-bypasses-apples-boot-defenses-affects-millions-of-iphones/) | 22.0 | 20.0 | 42.0 |
| [予約管理システムが侵害、個人情報が流出 - アソビュー](https://www.security-next.com/185170) | 22.0 | 20.0 | 42.0 |
| [患者情報含むUSBメモリを一時紛失 - 関西医科大病院](https://www.security-next.com/185803) | 22.0 | 20.0 | 42.0 |
| [GPS信号の妨害・改ざんを宇宙から可視化、ロシア西側国境付近で大規模な影響が判明](https://gigazine.net/news/20260622-satellite-reveal-gps-signal-tampering/) | 22.0 | 20.0 | 42.0 |
| [Cisco Packaged Contact Center EnterpriseおよびCisco Unified Contact Center Enterpriseのクロスサイトスクリプティング脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ucce-pcce-xss-2JVyg3uD) | 21.0 | 34.0 | 50.0 |
| [North Korean HackersによるMastraのNPMサプライチェーン攻撃](https://www.securityweek.com/north-korean-hackers-blamed-for-mastra-npm-supply-chain-attack/) | 20.0 | 45.0 | 42.0 |
| [6月22日 脅威インテリジェンスレポート](https://research.checkpoint.com/2026/22nd-june-threat-intelligence-report/) | 20.0 | 28.0 | 50.0 |
| [MicrosoftがAutoGen Studioのコード実行を可能にする脆弱性を修正](https://www.bleepingcomputer.com/news/security/microsoft-fixes-autogen-studio-flaw-that-enabled-code-execution/) | 20.0 | 20.0 | 42.0 |
| [INTERPOLとEuropol、ハッカーやその他の犯罪者対策で協力協定を更新](https://www.cybersecuritydive.com/news/interpol-europol-cybercrime-cooperation-renew/823398/) | 20.0 | 20.0 | 42.0 |
| [Symantec CBXがエンドポイントの可視性を全面的に提供する5つの理由](https://www.security.com/product-insights/5-reasons-symantec-cbx-endpoint-visibility) | 20.0 | 20.0 | 42.0 |
| [29年前のSquid Proxyの脆弱性「Squidbleed」で平文HTTPリクエストが漏えいする可能性](https://thehackernews.com/2026/06/29-year-old-squid-proxy-bug-squidbleed.html) | 20.0 | 20.0 | 42.0 |
| [カナダの公益事業会社がデータ侵害を公表、詳細は依然不明](https://www.theregister.com/security/2026/06/22/canadian-utility-fesses-up-to-data-breach-but-key-details-remain-off-grid/5259309) | 20.0 | 20.0 | 42.0 |
| [ブラジルの一部地域でサイバー攻撃の疑いにより誤った緊急警報が発報](https://therecord.media/suspected-cyberattack-triggers-false-emergency-alerts-brazil) | 20.0 | 20.0 | 42.0 |
| [盗まれた認証情報を扱う「Search Your Target」市場の実態](https://www.bleepingcomputer.com/news/security/a-glimpse-into-the-search-your-target-market-for-stolen-credentials/) | 20.0 | 20.0 | 42.0 |
| [Apple A12・A13チップに影響する修正不能なBootROM欠陥](https://www.infosecurity-magazine.com/news/apple-bootrom-exploit-a12-a13/) | 20.0 | 20.0 | 42.0 |
| [数十年前から存在するSquidプロキシの脆弱性「Squidbleed」でユーザーデータが漏えいする可能性](https://www.securityweek.com/decades-old-squid-proxy-flaw-squidbleed-can-expose-user-data/) | 20.0 | 20.0 | 42.0 |
| [Windows環境向けのクラウドネイティブセキュリティ：Wiz Runtime Sensor for Windowsの発表](https://www.wiz.io/blog/wiz-runtime-sensor-for-your-windows-environment) | 20.0 | 20.0 | 42.0 |
| [文書配達を装う詐欺とは何か、その目的は何か](https://www.malwarebytes.com/blog/scams/2026/06/document-delivery-scams-what-are-they-and-whats-their-goal) | 20.0 | 20.0 | 42.0 |
| [ブラジル、全国で発生した不正アラートを受け緊急警報システムを調査](https://www.theregister.com/security/2026/06/22/brazil-begins-investigating-emergency-alert-system-breach/5259421) | 20.0 | 20.0 | 42.0 |
| [AttackersがGravity SMTPプラグインの脆弱性を悪用してWordPressの重要データを収集](https://www.securityweek.com/attackers-exploit-gravity-smtp-plugin-flaw-to-harvest-valuable-wordpress-data/) | 20.0 | 20.0 | 42.0 |
| [保健委員会が偽の休暇通知で職員をフィッシングしたことを謝罪](https://www.theregister.com/security/2026/06/22/canadian-health-board-sorry-after-tasteless-phishing-test/5259320) | 20.0 | 20.0 | 42.0 |
| [Klueの侵害によりOAuthトークンを通じてサイバーセキュリティ企業が侵害される](https://www.infosecurity-magazine.com/news/klue-breach-compromise/) | 20.0 | 20.0 | 42.0 |
| [英情報コミッショナー、職場調査を受け辞任](https://www.infosecurity-magazine.com/news/information-commissioner-resigns/) | 20.0 | 20.0 | 42.0 |
| [Klueのハッキングによる影響をさらに多くのサイバーセキュリティ企業が開示](https://www.securityweek.com/more-cybersecurity-firms-disclose-impact-from-klue-hack/) | 20.0 | 20.0 | 42.0 |
| [インフラ停止の損失は1時間あたり5万ドル、対応時間を分単位に短縮せよ](https://www.cybersecuritydive.com/spons/infrastructure-downtime-has-a-50k-per-hour-price-tag-its-time-to-turn-ho/822869/) | 20.0 | 20.0 | 42.0 |

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
