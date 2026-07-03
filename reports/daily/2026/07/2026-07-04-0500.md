# 📡 サイレーダー 2026-07-04 05:00 JST

このレポートは、2026-07-03 17:00 JST〜2026-07-04 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 51
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 21

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [In Other News: Canadian Hacker Jailed, Open Source Zero-Days, Two Sentenced for ATM Jackpotting](#topic-20789) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [New Avalon Malware Framework Packs CrownX Ransomware Capabilities](#topic-20786) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [Cyber experts issue alert after two ransomware groups team up on ‘unprecedented’ threat campaign](#topic-20813) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Agentic AI Used to Conduct Ransomware Attack via Langflow](#topic-20809) | 33.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Armored Likho digging a snake pit: inside the covert BusySnake Stealer campaign](#topic-20815) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-20789"></a>

### 1. In Other News: Canadian Hacker Jailed, Open Source Zero-Days, Two Sentenced for ATM Jackpotting

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | - |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

公開情報では、Canadian hacker の有罪・収監、オープンソース関連プロジェクトでのゼロデイ公開、ATM jackpotting での有罪判決といった複数の話題がまとめて扱われています。
個別事案の詳細は材料内では限定的ですが、いずれも攻撃・悪用・法執行の文脈に関わるニュースです。
ゼロデイやATM不正のような話題は、実際の被害や防御優先度に直結しやすいため注目されます。オープンソースの脆弱性情報は、利用している製品や依存関係の点検を促す材料にもなります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 利用中のオープンソース依存関係を棚卸しし、関連する脆弱性情報や更新の有無を確認する。
- ATMや金融端末を運用する場合は、認証・監視・物理防護を含めた不正取引対策の見直しを行う。
- 脆弱性公開や悪用報道が出た際は、影響範囲の確認とパッチ適用の優先順位付けを速やかに進める。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [In Other News: Canadian Hacker Jailed, Open Source Zero-Days, Two Sentenced for ](https://www.securityweek.com/in-other-news-canadian-hacker-jailed-open-source-zero-days-two-sentenced-for-atm-jackpotting/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-20786"></a>

### 2. New Avalon Malware Framework Packs CrownX Ransomware Capabilities

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

新たに確認されたモジュール型マルウェア基盤「Avalon」は、複数段階のフィッシング連鎖を通じて配布されるとされ、認証情報の取得、横展開、遠隔操作、復旧妨害、ランサムウェア実行といった機能を組み合わせていると報告されています。
関連情報では、この基盤がCrownXランサムウェアの機能を備えている点が注目されています。
単体のマルウェアではなく、侵入から暗号化、復旧妨害までをまとめて担える構成である可能性が示されており、被害の広がりや対応の難度が高まるおそれがあります。
初出の脅威として、メール経由の侵入対策や検知・封じ込めの見直しが意識されます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 多段階フィッシングを前提に、メール認証や不審な添付・リンクの監視を強化する。
- 認証情報の窃取や横展開を想定し、特権アカウントの保護と多要素認証、最小権限を再確認する。
- 復旧妨害の可能性を踏まえ、バックアップの隔離保管と復旧手順の定期検証を行う。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New Avalon Malware Framework Packs CrownX Ransomware Capabilities](https://thehackernews.com/2026/07/new-avalon-malware-framework-packs.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20813"></a>

### 3. Cyber experts issue alert after two ransomware groups team up on ‘unprecedented’ threat campaign

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

複数のサイバー専門家が、2つのランサムウェア グループの連携に関する新たな脅威キャンペーンについて注意を呼びかけています。
公開情報では、従来よりも攻撃の参入障壁を下げる形の「工業化された」展開モデルが示唆されていますが、詳細は限定的です。
ランサムウェア運用の分業・連携が進むと、攻撃の量産化や拡散が起こりやすくなり、組織側の防御負荷が高まります。
単発事案ではなく、脅威の運用モデルそのものの変化として注目されています。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ランサムウェアの初期侵入経路と権限昇格の監視を改めて点検する。
- バックアップの分離保管と復旧手順の実効性を確認し、定期的に復旧訓練を行う。
- 侵害兆候の早期検知に向けて、EDRやログ監視のアラート条件を見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Cyber experts issue alert after two ransomware groups team up on ‘unprecedented’](https://www.itpro.com/security/ransomware/cyber-experts-issue-alert-after-two-ransomware-groups-team-up-on-unprecedented-threat-campaign) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20809"></a>

### 4. Agentic AI Used to Conduct Ransomware Attack via Langflow

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

報道によると、Langflowに関連する事例で、エージェント型AIがランサムウェア攻撃の実行に使われたとされています。
LLMエージェントが既知の手口とリアルタイムの判断を組み合わせ、複数段階の侵入を自動化しうる点が示されたとされています。
AIが攻撃の一部を自律的に進める可能性が改めて示され、従来型の防御や監視だけでは見落としが増えるおそれがあります。
AI活用基盤や連携コンポーネントを含めたリスク評価が、運用面でも重要になっています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIエージェントに外部操作や高権限の処理を持たせる場合は、権限分離と監査ログの確認を徹底する。
- LangflowのようなAIワークフロー基盤は、公開設定・認証・入力制御・依存関係の更新状況を定期的に点検する。
- 不審な自動化挙動や短時間での多段階アクセスを検知できるよう、監視ルールとインシデント対応手順を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | Langflow | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Agentic AI Used to Conduct Ransomware Attack via Langflow](https://www.securityweek.com/agentic-ai-used-to-conduct-ransomware-attack-via-langflow/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20815"></a>

### 5. Armored Likho digging a snake pit: inside the covert BusySnake Stealer campaign

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>A⁠I</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Kasperskyは、Armored Likhoとされる活動が関与したとみられるBusySnake Stealerキャンペーンについて報告しました。
報告では、スピアフィッシングやAI生成のローダー、新たなPythonベースのツールが使われ、ロシア、カザフスタン、ブラジルの組織が標的になっているとされています。
攻撃手法としてAI生成要素が含まれている点が注目され、脅威側の運用がより効率化・巧妙化している可能性を示します。
対象地域に関係する組織では、標的型メールや不審な添付・実行ファイルへの警戒が改めて重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 標的型メール対策を見直し、送信元や添付ファイルの検証を強化する。
- エンドポイントで不審なPython実行や未知のローダー挙動を監視する。
- 関連地域や取引先を持つ組織では、認証情報の保護と侵害前提の検知体制を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脅威アクター | Turla | 主題 | 0.80 | — |
| ベンダー | Kaspersky | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Mozilla | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Meta | 言及あり | 0.80 | — |
| 製品 | Google Chrome | 言及あり | 0.80 | — |
| 製品 | Chromium | 言及あり | 0.80 | — |
| 製品 | Mozilla Firefox | 言及あり | 0.80 | — |
| 製品 | OpenSSH | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Armored Likho digging a snake pit: inside the covert BusySnake Stealer campaign](https://securelist.com/tr/armored-likho-apt-with-busysnake-stealer/120292/) | <nobr>内容確認・補足情報</nobr> |

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
| [Armored Likhoが政府機関と電力部門をBusySnake Stealerで標的にする](https://thehackernews.com/2026/07/armored-likho-targets-government.html) | 31.0 | 20.0 | 43.0 |
| [北朝鮮関連のnpmパッケージがRollup Polyfillsを装い開発者の秘密情報を窃取](https://thehackernews.com/2026/07/north-korea-linked-npm-packages-mimic.html) | 28.0 | 45.0 | 42.0 |
| [Qilinがランサムウェア市場を支配、サイバー犯罪の集約が進行中](https://www.infosecurity-magazine.com/news/qilin-dominates-ransomware-market/) | 28.0 | 30.0 | 42.0 |
| [Ransomware GangがTeamPCPと提携した後の“Industrialized”なサイバー攻撃への警告](https://www.infosecurity-magazine.com/news/industrialized-cyberattacks/) | 28.0 | 30.0 | 42.0 |
| [GoogleとFBIが200万台規模のボットネットを標的に、NetNutが侵害される](https://www.theregister.com/security/2026/07/03/netnut-cracked-as-google-and-fbi-target-2-million-device-botnet/5266414) | 28.0 | 20.0 | 48.0 |
| [AdaptHealth、攻撃者が巧みに侵入しクラウドシステムから患者データを窃取されたと発表](https://www.theregister.com/security/2026/07/03/adapthealth-crooks-stole-our-passwords-patient-health-data/5266512) | 28.0 | 20.0 | 42.0 |
| [Verified X広告がMacマルウェアを拡散、ConsentFixがMicrosoftアカウントを窃取](https://www.malwarebytes.com/blog/news/2026/07/verified-x-ad-spreads-mac-malware-while-consentfix-steals-microsoft-accounts) | 28.0 | 20.0 | 42.0 |
| [FBIとGoogle、サイバー脅威アクターに利用されたNetNutプロキシネットワークを摘発・遮断](https://www.infosecurity-magazine.com/news/fbi-google-take-down-netnut-proxy/) | 28.0 | 20.0 | 42.0 |
| [関係者リストを誤送信、入力用様式と同一ファイル名で取り違え - 堺市](https://www.security-next.com/186506) | 22.0 | 20.0 | 42.0 |
| [「国家安全保障にまつわる機密情報が悪用される懸念」からスペイン政府がデータ分析大手のPalantir Technologiesをブラックリストに登録](https://gigazine.net/news/20260703-spain-orders-blacklist-us-tech-giant-palantir/) | 22.0 | 20.0 | 42.0 |
| [Android開発者認証は「保護を装った脅威」だとF-Droidが主張](https://gigazine.net/news/20260703-android-developer-verification-malware-f-droid/) | 22.0 | 20.0 | 42.0 |
| [「WatchGuard Firebox」のVPN機能に深刻なRCE脆弱性](https://www.security-next.com/186797) | 22.0 | 20.0 | 42.0 |
| [防衛省のLUUP導入で小泉大臣がコメント 「情報保全上の問題ない」](https://www.itmedia.co.jp/news/articles/2607/03/news128.html) | 21.0 | 20.0 | 42.0 |
| [GoogleやFBI、悪質プロキシ「NetNut」をテイクダウン スマートTVなど200万台超をボット化](https://atmarkit.itmedia.co.jp/ait/articles/2607/03/news125.html) | 21.0 | 20.0 | 42.0 |
| [GoogleとFBI、数百万台のデバイスを悪用したNetNutの住宅用プロキシネットワークを妨害](https://www.securityweek.com/google-fbi-disrupt-netnut-residential-proxy-network-powered-by-millions-of-devices/) | 20.0 | 20.0 | 48.0 |
| [NetNutプロキシネットワークが妨害され、200万台の感染デバイスが遮断される](https://www.bleepingcomputer.com/news/security/netnut-proxy-network-disrupted-2-million-infected-devices-cut-off/) | 20.0 | 20.0 | 42.0 |
| [ARToken PhaaSがEvilTokensのMicrosoft 365フィッシングツールキットを公開](https://www.bleepingcomputer.com/news/security/artoken-phaas-exposes-eviltokens-microsoft-365-phishing-toolkit/) | 20.0 | 20.0 | 42.0 |
| [中国製LLMが攻撃者と防御者の格差をさらに広げる](https://www.darkreading.com/cyber-risk/chinese-llms-broaden-gap-between-attackers-and-defenders) | 20.0 | 20.0 | 42.0 |
| [Medtronicのデータ侵害で380万人に影響](https://www.securityweek.com/medtronic-data-breach-impacts-3-8-million-people/) | 20.0 | 20.0 | 42.0 |
| [Scattered Spider関与のハッカーが米国へ身柄引き渡し](https://www.securityweek.com/alleged-scattered-spider-hacker-extradited-to-us/) | 20.0 | 20.0 | 42.0 |
| [PamStealerが偽のMaccyサイトとPAMチェックを悪用してMacのログインパスワードを窃取](https://thehackernews.com/2026/07/pamstealer-uses-fake-maccy-sites-and.html) | 20.0 | 20.0 | 42.0 |

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
