# 📡 サイレーダー 2026-09-25 17:00 JST

このレポートは、2026-09-25 11:00 JST〜2026-09-25 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 50
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 23

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [WSO2 and Adobe Commerce Flaws Exploited in Attacks, Added to CISA KEV](#topic-34326) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [A Closer Look at Malware From the Macfinger ClickFix Campaign, (Fri, Sep 25th)](#topic-34304) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [ChatGPTなどのAIに企業の偽の連絡先を出力させユーザーを詐欺へと導くサイバー攻撃「Dark Sourcery」](#topic-34310) | 30.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-34326"></a>

### 1. WSO2 and Adobe Commerce Flaws Exploited in Attacks, Added to CISA KEV

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>K⁠E⁠V</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAが、WSO2とAdobe Commerce/Magentoに影響する2件の脆弱性をKnown Exploited Vulnerabilities（KEV）に追加しました。
公的な情報として実際の悪用が確認されていることが背景にあり、少なくとも1件はWSO2 API Control Planeのパストラバーサル脆弱性とされています。
KEVへの追加は、単なる脆弱性情報ではなく「実際に攻撃で使われている」ことを示すため、優先度が上がります。該当製品を運用している組織では、影響範囲の確認と早期対応が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- WSO2 API Control PlaneおよびAdobe Commerce/Magentoの利用有無を確認し、対象資産を洗い出す。
- ベンダーやCISAの修正情報・緩和策を確認し、優先度を上げて適用計画を立てる。
- 外部公開面や管理系機能の露出を点検し、監視強化と不審な挙動の確認を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Adobe | 言及あり | 0.80 | — |
| 製品 | Adobe Commerce | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [WSO2 and Adobe Commerce Flaws Exploited in Attacks, Added to CISA KEV](https://thehackernews.com/2026/09/wso2-and-adobe-commerce-flaws-exploited.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34304"></a>

### 2. A Closer Look at Malware From the Macfinger ClickFix Campaign, (Fri, Sep 25th)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Macfinger ClickFixキャンペーンに関連するマルウェアについて、技術系ソースでの分析記事が公開されています。
現時点の材料からは、具体的な被害規模や影響範囲は確認できず、脅威動向の把握が主な論点です。
攻撃キャンペーンに関連するマルウェアの特徴が整理されることで、防御側は検知や監視の観点を見直しやすくなります。初期段階の情報でも、類似手口への注意喚起として価値があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 関連する不審な挙動や通信の検知ルールを見直す。
- 利用者向けに、誘導先の真偽確認や不審な操作要求への注意を再周知する。
- 同種キャンペーンに結びつく可能性のある端末ログやアラートを継続監視する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [A Closer Look at Malware From the Macfinger ClickFix Campaign, (Fri, Sep 25th)](https://isc.sans.edu/diary/rss/33368) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-34310"></a>

### 3. ChatGPTなどのAIに企業の偽の連絡先を出力させユーザーを詐欺へと導くサイバー攻撃「Dark Sourcery」

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

「Dark Sourcery」と呼ばれる攻撃キャンペーンについて、AIチャットボットの出力を汚染し、企業の連絡先などを誤って表示させて利用者を詐欺へ誘導する可能性が指摘されています。
対象としてChatGPTやGeminiが挙げられていますが、ここで示されているのは研究者の報告ベースの内容です。
生成AIの回答が外部情報に影響されやすい場合、利用者は見た目上もっともらしい誤情報を信じてしまうおそれがあります。
企業の問い合わせ先やサポート窓口の確認など、業務上の基本手順に影響し得る点が注目されています。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIが生成した連絡先や案内は、そのまま信用せず一次情報で照合する運用を徹底する。
- 社内向けに、AI経由で得たURLや連絡先を使う前の確認手順を明文化する。
- 外部公開情報や検索結果が業務判断に与える影響を見直し、誤情報前提の教育を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| AIモデル/プロジェクト | ChatGPT | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ChatGPTなどのAIに企業の偽の連絡先を出力させユーザーを詐欺へと導くサイバー攻撃「Dark Sourcery」](https://gigazine.net/news/20260925-dark-sourcery-hackers-manipulate-ai-scam/) | <nobr>内容確認・補足情報</nobr> |

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
| [窓口での待ち時間のイライラ、AI作成のBGMで軽減なるか 東京・港区が実証実験](https://www.itmedia.co.jp/news/article/2609/25/2000001741/) | 28.0 | 20.0 | 42.0 |
| [OpenAIのAIエージェントがオーストラリア政府機関のシステムをハッキングしたことが判明、OpenAIは3カ月間報告せず](https://gigazine.net/news/20260925-openai-hacked-australian-system/) | 27.0 | 20.0 | 42.0 |
| [Tencentが画像生成AI「Hy Image3.5」のプレビュー版をリリース](https://gigazine.net/news/20260925-tencent-hy-image-3-5/) | 27.0 | 20.0 | 42.0 |
| [【マネしないで】AIが暴走してやらかす“3つの主要パターン”を解説](https://atmarkit.itmedia.co.jp/ait/articles/2609/25/news059.html) | 26.0 | 20.0 | 42.0 |
| [目的達成のためハッキングを選択、AIエージェントの危険な挙動が判明](https://news.mynavi.jp/techplus/article/20260925-5025115/) | 26.0 | 20.0 | 42.0 |
| [AIエージェントのセキュリティ事案354件、実被害は127件 - オープンDB公開](https://news.mynavi.jp/techplus/article/20260925-5024486/) | 26.0 | 20.0 | 42.0 |
| [AIエージェントの発言ではなく行動に注目すること](https://www.helpnetsecurity.com/2026/09/25/ariel-assaraf-coralogix-ai-agent-guardrails/) | 25.0 | 20.0 | 42.0 |
| [ChatGPTを開いた後に別サイトで見たページの情報がOpenAIへ送られる仕組みが指摘される](https://gigazine.net/news/20260925-chatgpt-other-website/) | 22.0 | 20.0 | 42.0 |
| [「PHP」に複数の脆弱性 - セキュリティアップデートが公開](https://www.security-next.com/190695) | 22.0 | 20.0 | 42.0 |
| [RSAを素因数分解せずに破る攻撃を大規模実証、1024ビットRSAの署名偽造に成功](https://gigazine.net/news/20260925-rsa-nsnfsssfsfn/) | 22.0 | 20.0 | 42.0 |
| [Claudeで「セーフガードにブロックされたAI処理」に対する課金が開始される](https://gigazine.net/news/20260925-claude-safeguard-block-request/) | 22.0 | 20.0 | 42.0 |
| [国内企業の75％が「セキュリティ疲れ」 4つの構造的な要因とは](https://www.itmedia.co.jp/enterprise/articles/2609/26/news009.html) | 21.0 | 20.0 | 42.0 |
| [パルグループ、狙われたのは「老朽化システム」だった サーバ約100台停止から50日で復旧の軌跡](https://www.itmedia.co.jp/enterprise/articles/2609/25/news022.html) | 21.0 | 20.0 | 42.0 |
| [新入社員が知るべき情報漏えいの脅威【エスカとレンのセキュリティ通信】](https://ascii.jp/elem/000/004/430/4430234/?rss=) | 21.0 | 20.0 | 42.0 |
| [「LLMの出力コードを理解できない初心者ばかり」 PS5非公式ハックの主導者が離脱、AI時代のOSS開発に苦言](https://atmarkit.itmedia.co.jp/ait/articles/2609/25/news048.html) | 21.0 | 20.0 | 42.0 |
| [富士通とKELA、能動的サイバー防御支援サービスを開始](https://japan.zdnet.com/article/35252964/) | 21.0 | 20.0 | 42.0 |
| [Roundcube Webmailの脆弱性が攻撃者の標的に](https://www.securityweek.com/roundcube-webmail-vulnerability-in-attackers-crosshairs/) | 20.0 | 28.0 | 50.0 |
| [欧州で激化するロシアのハイブリッド・サイバー物理戦争](https://www.darkreading.com/physical-security/russia-hybrid-cyber-physical-war-europe) | 20.0 | 20.0 | 42.0 |
| [脅威ハンターの半数が不正確なデータを最大の課題と回答](https://www.helpnetsecurity.com/2026/09/25/sans-threat-hunting-data-quality/) | 20.0 | 20.0 | 42.0 |
| [Cloudflareの修正対応、あるコンテナが別顧客の残存ディスクデータを読み取れる不具合](https://thehackernews.com/2026/09/cloudflare-fixes-flaw-that-let-one.html) | 20.0 | 20.0 | 42.0 |
| [インシデント件数にいくつかの漏れがあります](https://www.helpnetsecurity.com/2026/09/25/eu-usa-retail-chain-cyberattacks/) | 20.0 | 20.0 | 42.0 |
| [baserCMS用プラグイン「アドオンマイグレーター」 における信頼できない制御領域からの機能の組み込みに関する脆弱性](https://jvn.jp/jp/JVN21754394/) | 20.0 | 20.0 | 42.0 |
| [baserCMSにおける複数の脆弱性](https://jvn.jp/jp/JVN14353754/) | 20.0 | 20.0 | 42.0 |

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
