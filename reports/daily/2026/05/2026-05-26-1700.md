# 📡 サイレーダー 2026-05-26 17:00 JST

このレポートは、2026-05-26 11:00 JST〜2026-05-26 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 59
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [KnowledgeDeliver LMS Flaw Exploited to Deploy Godzilla and Cobalt Strike](#topic-9892) | 50.0 | 64.0 | 55.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [ファイルサーバでランサム被害を確認 - ダイヤモンド関連企業](#topic-10210) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-10210"></a>

### 1. ファイルサーバでランサム被害を確認 - ダイヤモンド関連企業

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | - |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

オリエンタルダイヤモンドが、ファイルサーバでランサムウェア被害が確認されたと公表しました。
同社は宝飾用ダイヤモンドの輸入、製造、販売を手がける企業で、サイバー攻撃を受けた事実が明らかになっています。
ファイルサーバが被害を受けた場合、業務データや共有資料の停止・復旧に影響が及ぶ可能性があります。サプライチェーンや顧客対応への波及も含め、事業継続の観点で注目されます。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 共有ファイルサーバのバックアップ状況と復旧手順を再点検する。
- ランサムウェア検知後の初動対応と連絡体制を確認する。
- 外部公開前提の情報だけでなく、社内共有データの重要度分類を見直す。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [ファイルサーバでランサム被害を確認 - ダイヤモンド関連企業](https://www.security-next.com/184467) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-9892"></a>

### 1. KnowledgeDeliver LMS Flaw Exploited to Deploy Godzilla and Cobalt Strike

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>脅威アクター</nobr> / <nobr>Windows</nobr> / <nobr>ゼロデイ</nobr> / <nobr>IoC</nobr> / <nobr>iOS</nobr> / <nobr>RCE</nobr> / <nobr>CVE</nobr> / <nobr>防御・運用</nobr> / <nobr>政策・規制</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 50.0 |
| <nobr>実務影響</nobr> | 64.0 |
| <nobr>確度</nobr> | 55.0 |

#### 概要

KnowledgeDeliver LMS において、ASP.<wbr>NET の machineKey が複数環境で共通だったことに起因する脆弱性が悪用され、未認証のリモートコード実行につながったと報告されています。
攻撃後は、Godzilla としても知られる Web シェルの配置や、Cobalt Strike による感染へ発展した事例が確認されています。
日本で利用されることの多い LMS に関する事案であり、1つの秘密情報の漏えいが複数の導入先に波及し得る点が問題視されています。
認証前の侵入から Web シェル設置、端末感染までつながるため、サーバー防御だけでなく利用状況の監視も重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- KnowledgeDeliver の機器・サーバーでは、個別に強固な machineKey が設定されているか確認し、共有値が残っていれば速やかに更新する。
- Web ルート配下の .js / .aspx / .config の改ざん、IIS ワーカープロセスからの不審な子プロセス、ASP.<wbr>NET の ViewState 関連ログを確認する。
- LMS への到達範囲を必要最小限に絞り、異常なリクエストや不審なユーザーエージェントの痕跡がないか継続的に監視する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-5426 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-5426](https://nvd.nist.gov/vuln/detail/CVE-2026-5426) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [KnowledgeDeliver LMS Flaw Exploited to Deploy Godzilla and Cobalt Strike](https://thehackernews.com/2026/05/knowledgedeliver-lms-flaw-exploited-to.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Exploitation of KnowledgeDeliver via ViewState Deserialization Vulnerability](https://cloud.google.com/blog/topics/threat-intelligence/knowledgedeliver-viewstate-deserialization-vulnerability/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [F-Secure Internet Securityがフィッシングサイトや偽店舗、SMS詐欺をブロックする製品紹介](https://www.helpnetsecurity.com/2026/05/26/product-showcase-f-secure-internet-security-android/) | 36.0 | 30.0 | 42.0 |
| [ランサムウェア攻撃が「持続可能なビジネス」に 侵入コスト6万6000円、復旧に2億3000万円](https://www.itmedia.co.jp/news/articles/2605/26/news108.html) | 29.0 | 30.0 | 42.0 |
| [Microsoft 365 CopilotのAIエージェント機能「Cowork」が勝手にファイルを流出させる可能性があるとセキュリティ企業が指摘](https://gigazine.net/news/20260526-microsoft-copilot-cowork-exfiltrates-files/) | 27.0 | 20.0 | 42.0 |
| [AnthropicのAI「Claude Mythos」、1カ月で1万件超の脆弱性発見 修正作業追いつかず](https://news.mynavi.jp/techplus/article/20260526-4504331/) | 26.0 | 20.0 | 42.0 |
| [WordPressプラグイン・テーマの脆弱性最新情報 第29回 WordPress脆弱性13件、AI Engineの権限昇格や認証バイパスに注意【5月14日～5月20日】](https://news.mynavi.jp/techplus/article/wordpressvulnerability-29/) | 26.0 | 20.0 | 42.0 |
| [ソフトバンク、「AIデータセンター GPUクラウド」を10月に提供開始～運用負荷の軽減と柔軟性を実現するクラウドサービス](https://internet.watch.impress.co.jp/docs/news/2111560.html) | 25.0 | 20.0 | 42.0 |
| [NTTドコモが販売する「CM51FD」など、Atermの5Gモバイルルーター2製品に脆弱性。最新のファームウェアにアップデートを](https://internet.watch.impress.co.jp/docs/news/2111596.html) | 24.0 | 38.0 | 42.0 |
| [元従業員が取引先情報を持ち出し - ロッキング・オン・ジャパン](https://www.security-next.com/184948) | 22.0 | 20.0 | 42.0 |
| [iOS版「Firefox」にアップデート - 「なりすまし」脆弱性を解消](https://www.security-next.com/184942) | 22.0 | 20.0 | 42.0 |
| [ISC Stormcast 2026年5月26日（火）版](https://isc.sans.edu/diary/rss/33020) | 22.0 | 20.0 | 42.0 |
| [薬局で受け取った薬の情報、マイナポータルで当日中に確認可能に 「薬」画面をリニューアル](https://www.itmedia.co.jp/news/articles/2605/26/news106.html) | 21.0 | 20.0 | 42.0 |
| [フェラーリ、初のEV「Ferrari Luce」発表 元Appleデザイナー、ジョニー・アイブ氏のLoveFromがデザイン担当](https://www.itmedia.co.jp/news/articles/2605/26/news096.html) | 21.0 | 20.0 | 42.0 |
| [松下幸之助氏の「AI偽動画」に注意 PHP研究所が再告知 津田健次郎さんによるTikTok提訴受け](https://www.itmedia.co.jp/news/articles/2605/26/news080.html) | 21.0 | 20.0 | 42.0 |
| [被害長女がChatGPTに相談→児相に通報か 巨人・阿部前監督の暴行事件](https://www.itmedia.co.jp/news/articles/2605/26/news081.html) | 21.0 | 20.0 | 42.0 |
| [加齢に伴う血液の変化が大動脈瘤を悪化させる仕組みを解明](https://ascii.jp/elem/000/004/400/4400132/?rss=) | 21.0 | 20.0 | 42.0 |
| [dnsmasqにおける複数の脆弱性](https://jvn.jp/vu/JVNVU90845089/) | 20.0 | 20.0 | 42.0 |
| [7-Elevenのデータ侵害で18万5000人の個人情報が流出](https://www.bleepingcomputer.com/news/security/7-eleven-data-breach-exposes-personal-information-of-185-000-people/) | 20.0 | 20.0 | 42.0 |
| [機械IDを管理する：見落とされがちな特権アクセス層への対策](https://www.helpnetsecurity.com/2026/05/26/delinea-managing-managing-machine-identities-access/) | 20.0 | 20.0 | 42.0 |
| [今すぐ応募できるサイバーセキュリティ求人：2026年5月26日](https://www.helpnetsecurity.com/2026/05/26/cybersecurity-jobs-available-right-now-may-26-2026/) | 20.0 | 20.0 | 42.0 |
| [TCLのチューナー搭載大型テレビがAmazonで安い！4K対応75インチが9万4800円 98インチの「98Q6C」が31万8000円！](https://internet.watch.impress.co.jp/docs/shopping/2111627.html) | 20.0 | 20.0 | 42.0 |
| [ポータブル電源が安い！AmazonにてJackery製品がタイムセール 容量1070Whモデルの「ポータブル電源 1000 New」が6万9483円など](https://internet.watch.impress.co.jp/docs/shopping/2111616.html) | 20.0 | 20.0 | 42.0 |
| [ロボット農機の遠隔操作、山間部でも可能に～NTT・クボタ・NTTドコモが通信技術を実証 モバイル通信と衛星通信の連携と映像制御の組み合わせ](https://internet.watch.impress.co.jp/docs/news/2111563.html) | 20.0 | 20.0 | 42.0 |
| [「最新モデル以外のChromecastのサポートが終了」との海外報道、早とちりだったと判明【やじうまWatch】](https://internet.watch.impress.co.jp/docs/yajiuma/2111556.html) | 20.0 | 20.0 | 42.0 |
| [「忙しければ延期できます」Windows Updateに関するMicrosoftの異例のアピールが話題【やじうまWatch】](https://internet.watch.impress.co.jp/docs/yajiuma/2111557.html) | 20.0 | 20.0 | 42.0 |

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
