# 📡 サイレーダー 2026-07-07 05:00 JST

このレポートは、2026-07-06 17:00 JST〜2026-07-07 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 83
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 52

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [⚡ Weekly Recap: Proxy Botnets, Browser Ransomware, AI Agent Tricks, Fake PoC Malware and More](#topic-21051) | 43.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 2 | [Sysdig clocks first documented case of agentic ransomware](#topic-21032) | 41.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [Researchers Claim First Fully Agentic Ransomware: JadePuffer](#topic-21097) | 41.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [JadePuffer: The First Complete LLM-Driven Ransomware Attack](#topic-21026) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Prompt Injection Attacks Trick AI Agents Into Making Crypto Payments](#topic-21071) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-21051"></a>

### 1. ⚡ Weekly Recap: Proxy Botnets, Browser Ransomware, AI Agent Tricks, Fake PoC Malware and More

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

今週のセキュリティ動向をまとめた記事で、家庭用機器の悪用、ブラウザを介したランサムウェア、AIエージェントへの不適切な指示注入、偽のPoCマルウェアなど、複数の話題が取り上げられています。
共通しているのは、目立たない日常的な仕組みや信頼の前提が攻撃面になり得る、という点です。
AIと従来型の脅威が同時に扱われており、実務では端末・ブラウザ・AI利用の各層で見直しが必要になるためです。
特定の新手法だけでなく、既存の運用や権限設計の弱点が再確認される内容です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIエージェントや自動化機能に与える指示・権限の境界を再点検する。
- ブラウザの権限要求やリセット・認証フローなど、日常的なUIの信頼前提を見直す。
- 家庭用/IoT機器や社外依存コンポーネントを含む経路で不審な挙動がないか確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [⚡ Weekly Recap: Proxy Botnets, Browser Ransomware, AI Agent Tricks, Fake PoC Mal](https://thehackernews.com/2026/07/monday-recap-proxy-botnets-browser.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-21032"></a>

### 2. Sysdig clocks first documented case of agentic ransomware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Sysdigは、AIエージェントが関与した「agentic ransomware」の初の確認事例を報告しました。
公開情報によると、AIは攻撃の全工程を担ったわけではないものの、攻撃者の作業を簡素化し、進行を速める役割を果たしたとされています。
ランサムウェア攻撃にAIエージェントが組み込まれると、攻撃の効率化や実行速度の向上につながる可能性があります。
従来の自動化とは異なる形で脅威の運用負荷が下がるため、検知や対応の前提見直しが注目点です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIを悪用した攻撃は、単独で高度な自律性を持たなくても脅威の実効性を高めうるため、検知ルールや監視観点を更新する。
- ランサムウェア対策として、特権管理、バックアップの分離、復旧手順の定期確認を継続する。
- 生成AIやエージェント系ツールの社内利用状況を把握し、想定外の外部連携や権限付与がないか点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-3248 | 関連CVE | 1.00 | 候補あり（URL 30件以上） |
| ベンダー | Anthropic | 言及あり | 0.80 | — |
| ベンダー | DeepSeek | 言及あり | 0.80 | — |
| ベンダー | Qwen | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| 製品 | Langflow | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Sysdig clocks first documented case of agentic ransomware](https://cyberscoop.com/sysdig-judepuffer-ai-agentic-ransomware-attack/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21097"></a>

### 3. Researchers Claim First Fully Agentic Ransomware: JadePuffer

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者は、AIエージェントが自律的に関与するランサムウェアの事例として「JadePuffer」を報告しました。
現時点では公開情報ベースの主張であり、実際の攻撃規模や影響範囲は今後の追加確認が必要です。
ランサムウェアとAIエージェントの組み合わせは、攻撃の自動化や運用の効率化につながる可能性があるため注目されています。
AIを悪用した脅威の具体像を把握するうえで、検知・防御側の関心が高い話題です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIを使った攻撃は手口の変化が速いため、ランサムウェア検知ルールやアラート運用の見直しが重要です。
- 自律的な挙動を含む可能性を踏まえ、異常な実行連鎖や不自然な自動化の兆候を監視対象に含めるとよいでしょう。
- 今回の情報は初出のため、追加の技術情報や他ソースでの裏付けが出るまで断定を避けて評価するのが無難です。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Researchers Claim First Fully Agentic Ransomware: JadePuffer](https://www.infosecurity-magazine.com/news/researchers-first-agentic/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21026"></a>

### 4. JadePuffer: The First Complete LLM-Driven Ransomware Attack

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

JadePufferと呼ばれる脅威事例について、LLMを活用したとされるランサムウェア攻撃の一連の流れが報じられています。
公開情報では、Langflowの不具合を悪用して本番データベースサーバーからデータを取得し、他のシステムを暗号化したとされています。
LLMを使った攻撃が、単なる試行段階ではなく実際の侵害と結びついた事例として注目されています。
生成AIや自動化基盤を利用するサービスを運用する組織にとって、設定不備や脆弱性管理の重要性を改めて示す材料です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- LangflowのようなAI/自動化基盤は、最新版適用と公開設定の見直しを優先する。
- 本番データベースや周辺システムの権限分離、ネットワーク分離、バックアップの復元確認を再点検する。
- 異常なデータ取得や暗号化の兆候を想定し、ログ監視とインシデント対応手順を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | Langflow | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [JadePuffer: The First Complete LLM-Driven Ransomware Attack](https://www.darkreading.com/cyberattacks-data-breaches/jadepuffer-first-complete-llm-driven-ransomware-attack) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-21071"></a>

### 5. Prompt Injection Attacks Trick AI Agents Into Making Crypto Payments

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者は、悪意あるWebサイトに埋め込まれた間接的なプロンプトインジェクションが、Web閲覧型の自律AIエージェントに影響を与える可能性があると報告しました。
報告では、こうした手口によりAIエージェントが暗号資産の支払いに関わる動作を行わされる事例が指摘されています。
AIエージェントが外部コンテンツを参照しながら自動実行する用途では、通常のWeb攻撃とは異なるリスク管理が必要になります。
特に、指示の乗っ取りが金銭的な操作や意思決定に影響しうる点が注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIエージェントに外部Webを読ませる設計では、信頼できない入力を前提に権限分離や承認フローを入れること。
- 金銭移転や外部送信を伴う操作は、AIの自動実行に任せず人手確認を必須にすること。
- エージェントが参照するコンテンツの出所や挙動を監視し、想定外の指示混入を検知できる運用を整えること。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Prompt Injection Attacks Trick AI Agents Into Making Crypto Payments](https://www.securityweek.com/prompt-injection-attacks-trick-ai-agents-into-making-crypto-payments/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
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
| [Threat ActorsがGiteaのDocker脆弱性CVE-2026-20896を公開13日後に探索](https://thehackernews.com/2026/07/threat-actors-probe-gitea-docker-flaw.html) | 32.0 | 46.0 | 50.0 |
| [RCSとDNS: NAPTRレコードについて](https://isc.sans.edu/diary/rss/33124) | 30.0 | 20.0 | 42.0 |
| [16年前から存在するLinux KVMの脆弱性、IntelおよびAMDのx86システムでゲストVMがホストへ脱出可能に](https://thehackernews.com/2026/07/16-year-old-linux-kvm-flaw-lets-guest.html) | 29.0 | 38.0 | 52.0 |
| [北朝鮮系ハッカーがサプライチェーン攻撃でオープンソース開発者を標的にする](https://www.securityweek.com/north-korean-hackers-target-open-source-developers-in-supply-chain-attacks/) | 28.0 | 45.0 | 42.0 |
| [7月6日 脅威インテリジェンスレポート](https://research.checkpoint.com/2026/6th-july-threat-intelligence-report-2/) | 28.0 | 30.0 | 42.0 |
| [災害発生時に便乗するサイバー犯罪者：災害をテーマにした詐欺キャンペーンの持続的な脅威](https://blog.polyswarm.io/when-disaster-strikes-cybercriminals-follow-the-persistent-threat-of-disaster-themed-fraud-campaigns) | 28.0 | 20.0 | 42.0 |
| [Pegasus感染を受け、EUにスパイウェア調査担当MEPの対応を促す](https://www.theregister.com/security/2026/07/06/eus-latest-spyware-scandal-prompts-calls-for-urgent-action/5267054) | 28.0 | 20.0 | 42.0 |
| [Armored Likho APTによる政府・電力事業体を標的とした攻撃](https://www.securityweek.com/armored-likho-apt-targeting-government-electric-power-entities/) | 28.0 | 20.0 | 42.0 |
| [Vector Command Red Team Podと過ごす一日](https://www.rapid7.com/blog/post/so-ditl-day-with-your-vector-command-red-team-pod) | 28.0 | 20.0 | 42.0 |
| [Cavern Manticore：イラン関連のモジュラーC2フレームワークを暴露](https://research.checkpoint.com/2026/cavern-manticore-exposing-iran-linked-modular-c2-framework/) | 28.0 | 20.0 | 42.0 |
| [NetNutボットネットが打撃を受ける 次の被害者にならないために](https://www.malwarebytes.com/blog/news/2026/07/netnut-botnet-takes-a-hit-dont-be-part-of-the-next-one) | 28.0 | 20.0 | 42.0 |
| [中国系とみられるハッカーが偽のインド税申告ユーティリティを使ってDcRATを展開](https://thehackernews.com/2026/07/suspected-china-nexus-hackers-use-fake.html) | 28.0 | 20.0 | 42.0 |
| [URLの確認だけでは不十分：Microsoftサイトを悪用したデバイスコードフィッシング攻撃](https://securelist.com/microsoft-device-code-phishing-attack/120350/) | 28.0 | 20.0 | 42.0 |
| [Air-Gappedシステムからビデオケーブル放射を通じてデータを漏えいさせる新たなTrojPix攻撃](https://thehackernews.com/2026/07/new-trojpix-attack-leaks-data-from-air.html) | 28.0 | 20.0 | 42.0 |
| [Javaベースの新しいQuimaRAT MaaS、Windows・Linux・macOSで動作可能に](https://thehackernews.com/2026/07/new-java-based-quimarat-maas-built-to.html) | 28.0 | 20.0 | 42.0 |
| [AIエージェントは通常の生成AIよりも最大136倍エネルギーを消費する](https://gigazine.net/news/20260706-ai-agents-consume/) | 27.0 | 20.0 | 42.0 |
| [画像がAI生成かどうかを見分ける方法](https://www.malwarebytes.com/blog/ai/2026/07/how-to-tell-if-an-image-is-ai-generated) | 25.0 | 20.0 | 42.0 |
| [Webコンテンツを標的とするAIエージェントへの間接的なプロンプトインジェクション](https://www.infosecurity-magazine.com/news/indirect-prompt-injection-web/) | 25.0 | 20.0 | 42.0 |
| [LTMのBlueVerse RightLogic、AIリスク評価とサイバー修復計画を統合](https://www.helpnetsecurity.com/2026/07/06/ltm-blueverse-rightlogic/) | 25.0 | 20.0 | 42.0 |
| [2026年にAI SOCプラットフォームを評価する方法：リーダーをボルトオン型AIソリューションと分ける6つの能力](https://thehackernews.com/2026/07/how-to-evaluate-ai-soc-platform-in-2026.html) | 25.0 | 20.0 | 42.0 |
| [NCA、共有された子どもの写真がAIツールに悪用されるとして保護者に警告](https://www.infosecurity-magazine.com/news/nca-warn-parents-volume/) | 25.0 | 20.0 | 42.0 |
| [Frost & Sullivanの2025年Frost Radar™によるCloud Security Posture Managementに関する5つの洞察](https://www.microsoft.com/en-us/security/blog/2026/07/06/5-insights-from-frost-sullivans-2025-frost-radar-for-cloud-security-posture-management/) | 22.0 | 20.0 | 42.0 |
| [侵害受けたKDDIのISP向けメールシステム、ゼロデイ脆弱性が標的に](https://www.security-next.com/186871) | 22.0 | 20.0 | 42.0 |
| [YouTube StudioのAI機能で非公開動画の情報が漏れる可能性が指摘される](https://gigazine.net/news/20260706-youtube-ask-studio-leak/) | 22.0 | 20.0 | 42.0 |
| [Linuxの「Bad Epoll」Root権限取得脆弱性の概念実証エクスプロイト公開](https://www.securityweek.com/proof-of-concept-exploit-released-for-linux-bad-epoll-root-access-vulnerability/) | 22.0 | 20.0 | 42.0 |
| [講演会参加希望者向けのメールで誤送信 - 妙高市](https://www.security-next.com/186763) | 22.0 | 20.0 | 42.0 |
| [ピックルボール情報サイトに不正アクセス - プラグイン脆弱性を突かれる](https://www.security-next.com/186650) | 22.0 | 20.0 | 42.0 |
| [私的にシステム閲覧、身内に個人情報を漏洩した職員を処分 - 各務原市](https://www.security-next.com/186746) | 22.0 | 20.0 | 42.0 |
| [BIGLOBE、メルアド漏えいは約502万人分と判明 ニフティも約225万人分 KDDI基盤への不正アクセス続報](https://www.itmedia.co.jp/news/articles/2607/06/news121.html) | 21.0 | 20.0 | 42.0 |
| [Adobe ColdFusionの重大な脆弱性が攻撃で悪用されていることが判明](https://www.bleepingcomputer.com/news/security/max-severity-adobe-coldfusion-flaw-now-exploited-in-attacks/) | 20.0 | 28.0 | 50.0 |
| [Blogspotで配布される「Veil#Drop」攻撃のペイロード](https://www.securityweek.com/blogspot-hosted-payloads-delivered-in-veildrop-attacks/) | 20.0 | 20.0 | 42.0 |
| [イラン関連のハッカーが新しいCavern C2フレームワークを用いてイスラエルの組織を標的にする](https://thehackernews.com/2026/07/iran-linked-hackers-use-new-cavern-c2.html) | 20.0 | 20.0 | 42.0 |
| [HiAnimeアニメ海賊版サービスに関与した容疑者をベトナムで逮捕](https://www.bleepingcomputer.com/news/security/vietnam-arrests-suspects-behind-hianime-anime-piracy-service/) | 20.0 | 20.0 | 42.0 |
| [大手医療機器メーカーが約400万人への情報漏えいを通知](https://therecord.media/medical-device-maker-notifies-nearly-4-million-of-breach) | 20.0 | 20.0 | 42.0 |
| [US Armyのウェブサイトが改ざんされ、親クルド的なメッセージとトランプ氏への侮辱が表示される](https://cyberscoop.com/us-army-websites-defaced-404-hijacking-kurdistan/) | 20.0 | 20.0 | 42.0 |
| [アニメ配信サービスを妨害するサイバー攻撃で日本人少年を逮捕](https://therecord.media/japanese-teen-arrested-over-attack-disrupted-streaming-service) | 20.0 | 20.0 | 42.0 |
| [イラン関連の新たなハッキンググループがイスラエル政府とIT分野を標的にする](https://www.infosecurity-magazine.com/news/new-iran-hacking-group-targets/) | 20.0 | 20.0 | 42.0 |
| [ビジネスに沿ったリスク管理への移行](https://www.securityweek.com/the-shift-toward-business-aligned-risk-management/) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderの関係者とされる人物が米国へ送還される](https://www.cybersecuritydive.com/news/member-scattered-spider-extradited-us-retailer/824476/) | 20.0 | 20.0 | 42.0 |
| [Opera GXの脆弱性によりサイトからモッドを自動インストールしてデータ窃取が可能に](https://www.infosecurity-magazine.com/news/opera-gx-flaw-gx-mods-css/) | 20.0 | 20.0 | 42.0 |
| [ソフトウェアは思考速度で書かれるようになったが、セキュリティは追いついていない](https://www.bleepingcomputer.com/news/security/software-is-now-written-at-the-speed-of-thought-security-isnt/) | 20.0 | 20.0 | 42.0 |
| [Criminal IPがOpenCTIと連携し、脅威インテリジェンスを自動で強化する機能を提供](https://www.helpnetsecurity.com/2026/07/06/criminal-ip-integrates-threat-intelligence-with-opencti-for-automated-indicator-enrichment/) | 20.0 | 20.0 | 42.0 |
| [ウクライナのメディアがロシアのハッカーの「優先標的」に追加](https://therecord.media/ukraine-media-organizations-priority-hacking-targets-russia) | 20.0 | 20.0 | 42.0 |
| [WhatsAppのユーザー名は慎重に選ぼう](https://www.malwarebytes.com/blog/news/2026/07/choose-your-whatsapp-username-carefully) | 20.0 | 20.0 | 42.0 |
| [英スーパー大手、万引き犯検挙に顔認証をさらに強化](https://www.theregister.com/security/2026/07/06/brit-supermarket-giant-triples-down-on-facial-recog-to-nab-shoplifters/5266935) | 20.0 | 20.0 | 42.0 |
| [なぜ学校はハッカーの格好の標的となり、対抗に苦戦するのか](https://www.cybersecuritydive.com/news/schools-cybersecurity-threats-education-sector-reporters-notebook/824123/) | 20.0 | 20.0 | 42.0 |
| [KDDI情報流出 未知の脆弱性が原因](https://news.yahoo.co.jp/pickup/6586971?source=rss) | 20.0 | 20.0 | 42.0 |
| [ハッカーがInterpolを装って中小企業を標的に、知っておくべきこと](https://www.itpro.com/security/cyber-attacks/hackers-are-posing-as-interpol-to-target-small-business-heres-what-you-need-to-know) | 20.0 | 20.0 | 42.0 |
| [Moody Bible Instituteの侵害で230万件のアカウントが影響、cyber expertが指摘](https://www.theregister.com/security/2026/07/06/moody-bible-institute-breach-leaves-23m-accounts-needing-salvation-says-cyber-expert/5266827) | 20.0 | 20.0 | 42.0 |
| [次の10年を形づくるセキュリティリーダーたちは、まだCISOの座にはいない](https://www.cybersecuritydive.com/spons/the-security-leaders-defining-the-next-decade-arent-in-ciso-seats-yet/824263/) | 20.0 | 20.0 | 42.0 |
| [脆弱性を見つけることは、そもそも難しいことではなかった](https://cyberscoop.com/ai-cybersecurity-vulnerability-prioritization-op-ed/) | 20.0 | 20.0 | 42.0 |
| [KDDI パスワード760万人分漏えい](https://news.yahoo.co.jp/pickup/6586944?source=rss) | 20.0 | 20.0 | 42.0 |

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
