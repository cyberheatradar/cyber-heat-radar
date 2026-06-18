# 📡 サイレーダー 2026-06-18 11:00 JST

このレポートは、2026-06-18 05:00 JST〜2026-06-18 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 55
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 28

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Crypto Clipper uses Tor and worm-like propagation for persistence and control](#topic-17991) | 30.0 | 20.0 | 48.0 | 音声 | 温度感上位枠 |
| 2 | [Smashing Security podcast #472: AI gets hacked, and BitLocker gets bypassed](#topic-17992) | 30.0 | 20.0 | 43.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-17991"></a>

### 1. Crypto Clipper uses Tor and worm-like propagation for persistence and control

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 48.0 |

#### 概要

Microsoft Threat Intelligenceが、暗号資産の送金先を書き換えるクリッパー型マルウェアのキャンペーンを分析しました。
クリップボード上の情報を狙う機能に加え、Torを使った通信や自己拡散に近い挙動、持続性や追加活動につながる軽量バックドア機能が確認されています。
単なる資産窃取にとどまらず、感染後も残り続けて横展開や追加侵害につながる可能性があるためです。暗号資産を扱う環境だけでなく、一般的な端末管理や通信監視の観点でも注意が必要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- クリップボード改変やウォレットアドレス置換を疑う端末挙動を監視する。
- Tor関連通信や不審な外向き通信がないか、端末・ネットワークの両面で確認する。
- 端末の永続化設定や不要な自動起動項目を点検し、感染端末の隔離と再調査を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Crypto Clipper uses Tor and worm-like propagation for persistence and control](https://www.microsoft.com/en-us/security/blog/2026/06/17/crypto-clipper-uses-tor-worm-like-propagation-for-persistence-control/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17992"></a>

### 2. Smashing Security podcast #472: AI gets hacked, and BitLocker gets bypassed

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

公開情報では、AIコーディング支援やAIエージェントの扱い方をめぐるリスクと、Microsoft製品に関する複数のゼロデイ脆弱性が話題になっています。
特に、BitLockerの保護を回避し得る事例が取り上げられており、物理アクセスを伴う端末防御の見直しが意識されています。
AIを業務システムに接続する際の権限管理や入力検証が不十分だと、意図しない情報流出につながる可能性があります。
また、端末の暗号化機能があっても、周辺の実装や設定に弱点があると防御が崩れるため、注目されています。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- AIアシスタントやAIエージェントに与える権限を最小限にし、メールやカレンダーなど機微情報への接続は慎重に管理する。
- Microsoft関連の脆弱性情報を確認し、該当製品の更新適用状況と端末の保護設定を点検する。
- 物理アクセス前提のリスクも想定し、BitLockerなどの暗号化だけに依存しない多層防御を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Smashing Security podcast #472: AI gets hacked, and BitLocker gets bypassed](https://grahamcluley.com/smashing-security-podcast-472/) | <nobr>内容確認・補足情報</nobr> |

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
| [「AIを使う学生」vs.「使わない学生」、エッセイが創造的なのはどっち？ 米大学が2025年に実証実験](https://www.itmedia.co.jp/news/articles/2606/18/news043.html) | 28.0 | 20.0 | 42.0 |
| [Roblox開発者がマルウェア攻撃でゲーム全体を失う被害](https://www.malwarebytes.com/blog/scams/2026/06/roblox-developers-are-losing-entire-games-to-malware-attacks) | 28.0 | 20.0 | 42.0 |
| [「Splunk」向けのAI拡張ツールに複数の脆弱性](https://www.security-next.com/186052) | 27.0 | 20.0 | 42.0 |
| [「徹底的にやらないとサイバー被害を防げない」時代 OPSWATがさらに2つの新技術を追加](https://ascii.jp/elem/000/004/411/4411460/?rss=) | 26.0 | 20.0 | 42.0 |
| [1年経っても生成AIの“成果創出”で足踏みする日本企業 PwCの6カ国比較にみる“分岐点”](https://ascii.jp/elem/000/004/411/4411364/?rss=) | 26.0 | 20.0 | 42.0 |
| [「AIコーディング」がたった5年で急進化したワケ NTT「tsuzumi 2」開発者が分析](https://www.itmedia.co.jp/news/articles/2606/18/news038.html) | 26.0 | 20.0 | 42.0 |
| [OpenAI×ソフトバンクの新サービスは脆弱性管理の常識を変える？ それとも期待先行？](https://atmarkit.itmedia.co.jp/ait/articles/2606/18/news041.html) | 26.0 | 20.0 | 42.0 |
| [ローカルで動くAIエージェント「Hermes」を使う](https://japan.zdnet.com/article/35248761/) | 26.0 | 20.0 | 42.0 |
| [漏えい情報でOpenAIがChatGPT for Scienceのサブスクリプションをテスト中と確認](https://www.bleepingcomputer.com/news/artificial-intelligence/leak-confirms-openai-is-testing-a-chatgpt-for-science-subscription/) | 25.0 | 20.0 | 42.0 |
| [豆腐通販サイトで決済アプリ改ざん - 個人情報流出の可能性](https://www.security-next.com/185929) | 22.0 | 20.0 | 42.0 |
| [「Cisco ISE」にRCE脆弱性 - 端末の接続に影響するおそれも](https://www.security-next.com/186046) | 22.0 | 20.0 | 42.0 |
| [「Chrome」が脆弱性33件を修正 - 「クリティカル」7件](https://www.security-next.com/186042) | 22.0 | 20.0 | 42.0 |
| [今日もどこかで情報漏えい 第49回「2026年5月の情報漏えい」その地方ならではのケジメのつけ方](https://scan.netsecurity.ne.jp/article/2026/06/18/55524.html) | 21.0 | 20.0 | 42.0 |
| [SCSK 公式ホームページで不審な認証表示](https://scan.netsecurity.ne.jp/article/2026/06/18/55523.html) | 21.0 | 20.0 | 42.0 |
| [日中経済協会のメールアカウントに不正アクセス、不審メール 565 件送信](https://scan.netsecurity.ne.jp/article/2026/06/18/55522.html) | 21.0 | 20.0 | 42.0 |
| [神姫バスのウェブサイトに DDoS 攻撃](https://scan.netsecurity.ne.jp/article/2026/06/18/55521.html) | 21.0 | 20.0 | 42.0 |
| [「情報セキュリティサービス基準審査登録制度」2026年度 第2回 登録申請募集開始](https://scan.netsecurity.ne.jp/article/2026/06/18/55520.html) | 21.0 | 20.0 | 42.0 |
| [SCS 評価制度対応支援でリコージャパンと SecureNavi が協業](https://scan.netsecurity.ne.jp/article/2026/06/18/55519.html) | 21.0 | 20.0 | 42.0 |
| [「ブラウザの偽警告」から「給与改定の社内通知」まで ～ 4 つの手口から読み解くサポート詐欺最新傾向](https://scan.netsecurity.ne.jp/article/2026/06/18/55518.html) | 21.0 | 20.0 | 42.0 |
| [東京都、都内中小企業向けに「CSIRT構築・IT-BCP策定」を無償支援 限定 60 社](https://scan.netsecurity.ne.jp/article/2026/06/18/55517.html) | 21.0 | 20.0 | 42.0 |
| [医療機関のセキュリティの現状を簡単に「見える化」～ HAIP、Webアセスメントサービス開始](https://scan.netsecurity.ne.jp/article/2026/06/18/55516.html) | 21.0 | 20.0 | 42.0 |
| [「パッチ適用実施していない」建設・不動産 29.5 ％、流通 17.0 ％、旅行・レジャー・飲食 10.0 ％、金融 0.0 ％](https://scan.netsecurity.ne.jp/article/2026/06/18/55515.html) | 21.0 | 20.0 | 42.0 |
| [点ではなく「振る舞い」を日常学習--ダークトレースのCISOが説く「ビヘイビアAI」](https://japan.zdnet.com/article/35249055/) | 21.0 | 20.0 | 42.0 |
| [AIが脆弱性を掘り起こし過ぎる時代へ FIRSTがCVE予測を6万6000件に上方修正](https://atmarkit.itmedia.co.jp/ait/articles/2606/18/news047.html) | 21.0 | 20.0 | 42.0 |
| [「Microsoft 365」の運用におけるリスク](https://japan.zdnet.com/article/35248532/) | 21.0 | 20.0 | 42.0 |
| [AIでオープンソースの脆弱性に対処--Chainguardが立ち上げた「Athena」連合とは](https://japan.zdnet.com/article/35249018/) | 21.0 | 20.0 | 42.0 |
| [SignalRGBカーネルドライバにおける不適切なアクセス制御およびIOCTLの脆弱性](https://jvn.jp/vu/JVNVU95564871/) | 20.0 | 20.0 | 42.0 |
| [Google、UKとEUのユーザーIPアドレスを広告パーソナライズに利用へ](https://www.bleepingcomputer.com/news/security/google-to-use-uk-and-eu-user-ip-addresses-for-ad-personalization/) | 20.0 | 20.0 | 42.0 |

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
