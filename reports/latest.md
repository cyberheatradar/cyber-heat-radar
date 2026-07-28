# 📡 サイレーダー 2026-07-28 11:00 JST

このレポートは、2026-07-28 05:00 JST〜2026-07-28 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 62
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 35

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Hackers target US firms in FastJson RCE zero-day attacks](#topic-24560) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [Arista patches VeloCloud Orchestrator zero-day exploited in attacks](#topic-24585) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-24560"></a>

### 1. Hackers target US firms in FastJson RCE zero-day attacks

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

FastJson のオープンソース Java ライブラリに関する脆弱性が、実際に悪用されていると報じられています。
報道では、対象環境でリモートコード実行につながる可能性があり、ユーザー操作や昇格権限を必要としない点が懸念されています。
Java ライブラリは多くのシステムや製品に組み込まれているため、影響範囲が広がる可能性があります。
ゼロデイとして悪用が観測されている点から、公開情報ベースでも早めの確認と対応が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- FastJson を利用しているアプリケーションや依存関係を洗い出し、影響有無を確認する。
- ベンダーやコミュニティの修正版・回避策の案内が出ていないか継続的に確認する。
- 外部公開している Java アプリケーションのログや異常動作を点検し、侵害兆候がないか確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Hackers target US firms in FastJson RCE zero-day attacks](https://www.bleepingcomputer.com/news/security/hackers-target-us-firms-in-fastjson-rce-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-24585"></a>

### 2. Arista patches VeloCloud Orchestrator zero-day exploited in attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Aristaは、オンプレミス版VeloCloud Orchestratorに存在する深刻なコマンドインジェクション脆弱性への修正を公開しました。
公開情報では、この問題は攻撃に悪用されているとされており、ゼロデイとして扱われています。
管理系製品でのコマンド実行につながる脆弱性は、侵害時の影響が大きくなりやすい点が注目されています。特に悪用が確認されている場合、該当環境では早急な対応が必要になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- オンプレミス版VeloCloud Orchestratorの利用有無を確認し、ベンダーの修正内容を適用する。
- 管理画面や関連ログを点検し、不審な操作や想定外のコマンド実行の痕跡がないか確認する。
- 外部公開範囲やアクセス制御を見直し、当面は管理系インターフェースへの到達経路を最小化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-16812 | 主題CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Arista patches VeloCloud Orchestrator zero-day exploited in attacks](https://www.bleepingcomputer.com/news/security/arista-patches-velocloud-orchestrator-zero-day-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |

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
| [ネットワークジャパンにランサムウェア攻撃、復旧と引き換えに暗号資産を要求する文書を設置](https://scan.netsecurity.ne.jp/article/2026/07/28/55796.html) | 29.0 | 30.0 | 42.0 |
| [FBIによるLockBit摘発を加速させたアフィリエイトの信頼崩壊](https://www.darkreading.com/cybersecurity-operations/fbi-breaking-affiliate-trust-lockbit-takedown) | 28.0 | 30.0 | 42.0 |
| [Dysphoria DDoSボットネットが世界中の20万台のデバイスに拡散](https://www.bleepingcomputer.com/news/security/new-dysphoria-ddos-botnet-spreads-to-200k-devices-worldwide/) | 28.0 | 20.0 | 42.0 |
| [サイバー攻撃グループの名前から国家や動機を分かりやすく。Googleが新命名規則を展開 「APT44」は「SANDWORM RELIC」に](https://internet.watch.impress.co.jp/docs/news/2128210.html) | 28.0 | 20.0 | 42.0 |
| [Socket、Nuxtのセキュリティ脆弱性に対する無料の認証済みパッチを公開](https://socket.dev/blog/patches-for-nuxt-security-vulnerabilities) | 26.0 | 38.0 | 42.0 |
| [「Claude」の共有チャットがGoogle検索で一時丸見えに](https://japan.zdnet.com/article/35251007/) | 26.0 | 20.0 | 42.0 |
| [前例のないAIサイバー脅威への対抗手段が課題となっている欧州中央銀行（ECB）](https://ascii.jp/elem/000/004/422/4422283/?rss=) | 26.0 | 20.0 | 42.0 |
| [NVIDIA、「Open Secure AI Alliance」を設立--OSS脆弱性をAIで解決](https://japan.zdnet.com/article/35251002/) | 26.0 | 20.0 | 42.0 |
| [ガートナー、Tenable を AI を活用したエクスポージャー評価分野における「Company to Beat」に位置付け](https://scan.netsecurity.ne.jp/article/2026/07/28/55792.html) | 26.0 | 20.0 | 42.0 |
| [GitLab 19.2 リリース、AI エージェント活用や依存関係スキャンの自動修正に対応](https://scan.netsecurity.ne.jp/article/2026/07/28/55791.html) | 26.0 | 20.0 | 42.0 |
| [日本マイクロソフト、「Copilot」の進化でAI活用を次の段階へ](https://japan.zdnet.com/article/35250998/) | 26.0 | 20.0 | 42.0 |
| [NVIDIAやMicrosoftなど30社超、オープンAIの防御ツール共同開発の「Open Secure AI Alliance」設立](https://www.itmedia.co.jp/news/articles/2607/28/news059.html) | 26.0 | 20.0 | 42.0 |
| [AIエージェントがタイ財務省へのスパイ攻撃を主導](https://www.darkreading.com/cyberattacks-data-breaches/ai-agent-espionage-attack-thai-ministry-finance) | 25.0 | 20.0 | 42.0 |
| [Microsoft、AIを活用したサイバーセキュリティ製品群を発表、競争が激化](https://cyberscoop.com/microsoft-ai-cybersecurity-project-perception/) | 25.0 | 20.0 | 42.0 |
| [Microsoft、競合プラットフォームを上回るとするAIセキュリティツールを発表](https://arstechnica.com/security/2026/07/microsoft-unveils-ai-security-tools-it-says-outperform-competing-platforms/) | 25.0 | 20.0 | 42.0 |
| [「VeloCloud Orchestrator」に脆弱性、悪用を確認 - 侵害調査を](https://www.security-next.com/187930) | 24.0 | 20.0 | 43.0 |
| [米当局、「FortiOS」「VeloCloud Orchestrator」の脆弱性悪用を確認](https://www.security-next.com/187925) | 24.0 | 20.0 | 43.0 |
| [「TeamCity」に深刻な脆弱性 - アップデートで修正](https://www.security-next.com/187935) | 22.0 | 20.0 | 42.0 |
| [新たなCertighostのPoCエクスプロイトで攻撃者がWindowsドメインを乗っ取れるように](https://www.bleepingcomputer.com/news/security/new-certighost-poc-exploit-lets-attackers-hijack-windows-domains/) | 22.0 | 20.0 | 42.0 |
| [iOS 26.6公開、Spotlight最適化やセキュリティ修正 MacBook Neoの安定性向上も](https://news.mynavi.jp/techplus/article/20260728-4749072/) | 21.0 | 20.0 | 42.0 |
| [Google がサイバー犯罪集団の独自分類体系を導入 ～ Microsoft と CrowdStrike が推進した業界統一規則はいずこへ](https://scan.netsecurity.ne.jp/article/2026/07/28/55800.html) | 21.0 | 20.0 | 42.0 |
| [丸投げからの脱却・ノウハウゼロの挑戦 ～ なぜ脆弱性診断の内製化は「ツールを入れただけ」だと失敗するのか？](https://scan.netsecurity.ne.jp/article/2026/07/28/55799.html) | 21.0 | 20.0 | 42.0 |
| [メディア4uのSMS送信システムにサイバー攻撃、個人情報漏えいと不正なSMS送信を確認](https://scan.netsecurity.ne.jp/article/2026/07/28/55798.html) | 21.0 | 20.0 | 42.0 |
| [野々市市職員が戸籍謄本を閲覧・印刷、減給処分に](https://scan.netsecurity.ne.jp/article/2026/07/28/55797.html) | 21.0 | 20.0 | 42.0 |
| [アフラック生命保険に不正アクセス、保険料振替口座が漏えいしたことを踏まえ金融機関と連携](https://scan.netsecurity.ne.jp/article/2026/07/28/55795.html) | 21.0 | 20.0 | 42.0 |
| [はてな資金流出、捜査協力の一環と信じ込まされ会社資金の流出を招いたことを認定](https://scan.netsecurity.ne.jp/article/2026/07/28/55794.html) | 21.0 | 20.0 | 42.0 |
| [TwoFive、2026年上半期のフィッシングトレンドを公開 ～ Azure の悪用拡大](https://scan.netsecurity.ne.jp/article/2026/07/28/55793.html) | 21.0 | 20.0 | 42.0 |
| [ASMツール「GMOサイバー攻撃ネットde診断 ASM」が CVSS v4.0 に対応](https://scan.netsecurity.ne.jp/article/2026/07/28/55789.html) | 21.0 | 20.0 | 42.0 |
| [在大連領事事務所関係者を装ったなりすましメールに注意を呼びかけ](https://scan.netsecurity.ne.jp/article/2026/07/28/55788.html) | 21.0 | 20.0 | 42.0 |
| [WordPressの脆弱性「wp2shell」 古いバージョンでも自動更新していても安心できない理由](https://www.itmedia.co.jp/enterprise/articles/2607/28/news014.html) | 21.0 | 20.0 | 42.0 |
| [防犯カメラの録画が途切れる 初期設定ポートの変更で解決](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/041800004/071600103/) | 21.0 | 20.0 | 42.0 |
| [注目高まる「SCS評価制度」](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/041800012/071700334/) | 21.0 | 20.0 | 42.0 |
| [「Android 17」の侵入ログ機能を有効化する方法--今すぐ使うべきセキュリティ](https://japan.zdnet.com/article/35250854/) | 21.0 | 20.0 | 42.0 |
| [Trumpが中間選挙前に郵便投票の制限を認めるよう最高裁に求める](https://cyberscoop.com/trump-supreme-court-mail-in-voting/) | 20.0 | 20.0 | 42.0 |
| [Google CloudとMicrosoft Azureに残る「Confused Deputy」脆弱性](https://www.darkreading.com/cloud-security/confused-deputy-flaws-google-cloud-microsoft-azure) | 20.0 | 20.0 | 42.0 |

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
