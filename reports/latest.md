# 📡 サイレーダー 2026-05-26 05:00 JST

このレポートは、2026-05-25 17:00 JST〜2026-05-26 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 74
- [音声で扱う想定のトピック](#audio-topics): 4
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [⚡ Weekly Recap: Linux Flaws, Defender 0-Days, Router Botnets, and Supply Chain Chaos](#topic-9976) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [25th May – Threat Intelligence Report](#topic-8637) | 36.0 | 46.0 | 59.0 | 音声 | 温度感上位枠 |
| 3 | [一部サーバでランサムウェア被害 - キャンディルグループ会社](#topic-9987) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [TeamPCP Supply Chain Campaign: Activity Through 2026-05-24, (Mon, May 25th)](#topic-9980) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-9976"></a>

### 1. ⚡ Weekly Recap: Linux Flaws, Defender 0-Days, Router Botnets, and Supply Chain Chaos

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>サプライチェーン</nobr> / <nobr>Linux</nobr> / <nobr>フィッシング</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 45.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Linuxの脆弱性、Microsoft Defenderのゼロデイ、ルータのボットネット化、サプライチェーン混乱など、複数の脅威が並行して話題になった週次まとめです。
既知の古い脆弱性の再浮上や、セキュリティ製品自体への対策が必要になる状況も示されており、攻撃対象が広がっていることがうかがえます。
単発の個別事案というより、企業のLinuxサーバー、端末防御、ネットワーク機器、開発・供給網まで広く影響しうるテーマが同時進行している点が重要です。
複数の層で更新遅れや見落としがあると、侵入や横展開の足がかりになりやすいため、優先順位付けが求められます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Linuxや周辺製品の脆弱性情報を継続監視し、影響資産の棚卸しと更新状況の確認を行う。
- 端末防御製品や管理系ツールについても、例外設定や保護状態を見直し、検知ログを重点確認する。
- ルータや境界機器、古いサーバーなどの放置資産を洗い出し、不要公開の停止と更新適用を進める。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [⚡ Weekly Recap: Linux Flaws, Defender 0-Days, Router Botnets, and Supply Chain C](https://thehackernews.com/2026/05/weekly-recap-linux-flaws-defender-0.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-8637"></a>

### 2. 25th May – Threat Intelligence Report

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>KEV</nobr> / <nobr>ランサムウェア</nobr> / <nobr>権限昇格</nobr> / <nobr>DDoS</nobr> / <nobr>マルウェア</nobr> / <nobr>TTP</nobr> / <nobr>脅威レポート</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 再燃 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 46.0 |
| <nobr>確度</nobr> | 59.0 |

#### 概要

Microsoft Defenderに関する2件の脆弱性、CVE-2026-41091とCVE-2026-45498について、実際の悪用が観測されていると報じられています。
CVE-2026-41091は権限昇格につながる可能性があり、CISAのKnown Exploited Vulnerabilitiesカタログにも追加されています。
防御製品そのものが狙われるため、影響は個別端末にとどまらず、組織全体の検知・防御体制に波及し得ます。
既知の悪用事例として扱われているため、優先度を上げて対応状況を確認する必要があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Microsoftの修正情報と適用状況を確認し、対象環境で更新が未適用の端末を洗い出す。
- Defender関連の異常動作や権限昇格の兆候、サービス停止などの挙動を監視する。
- CISAの既知悪用リストに載っている脆弱性として、資産管理とパッチ優先順位付けに反映する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-41091 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-34926 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-45498 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-9082 | 主要CVE | 1.00 |
| ransomware_group | Qilin | 主題 | 0.80 |
| ベンダー | Microsoft | 言及あり | 0.80 |
| ransomware_group | Akira | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-41091](https://nvd.nist.gov/vuln/detail/CVE-2026-41091) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [25th May – Threat Intelligence Report](https://research.checkpoint.com/2026/25th-may-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Defender vulnerabilities exploited in the wild (CVE-2026-41091, CVE-20](https://www.helpnetsecurity.com/2026/05/21/microsoft-defender-vulnerabilities-cve-2026-41091-cve-2026-45498/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Warns of Two Actively Exploited Defender Vulnerabilities](https://thehackernews.com/2026/05/microsoft-warns-of-two-actively.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-9987"></a>

### 3. 一部サーバでランサムウェア被害 - キャンディルグループ会社

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

キャンディルのグループ会社で、住宅メンテナンスサービスなどを手がけるキャンディルパートナーズが、一部サーバに対するランサムウェア被害を公表しました。
現時点では、被害の範囲や業務への影響の詳細は材料からは確認できません。
ランサムウェア被害は、情報漏えいや業務停止につながるおそれがあるため、企業の事業継続と顧客対応の両面で注目されます。
国内企業グループでの公表事案として、同種の被害への備えや初動対応の重要性を示しています。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象サーバの隔離、侵入経路の確認、影響範囲の切り分けを優先する。
- バックアップの健全性と復旧手順を確認し、復旧優先度を整理する。
- 関連する認証情報や外部公開設定を点検し、再侵入防止の対策を進める。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [一部サーバでランサムウェア被害 - キャンディルグループ会社](https://www.security-next.com/184740) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-9980"></a>

### 4. TeamPCP Supply Chain Campaign: Activity Through 2026-05-24, (Mon, May 25th)

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>サプライチェーン</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>政策・規制</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

TeamPCPに関連するサプライチェーン型の動きが継続しており、複数のパッケージエコシステムにまたがって活動していると報告されています。
公開情報では、GitHubの内部コードベースやMicrosoftが公開したPython SDKに関する言及があり、供給網を狙うリスクが示唆されています。
ソフトウェア供給網に関わるため、単一の利用者や組織にとどまらず、依存関係を通じて影響が広がる可能性があります。
開発・運用の現場では、パッケージやSDKの信頼性確認が改めて重要になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 利用しているパッケージやSDKの出所、保守状況、更新履歴を点検する。
- 依存関係の変更時に、署名・整合性・配布元の確認を徹底する。
- CI/CDや開発端末で、想定外の更新や不審な依存追加がないか監視を強化する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [TeamPCP Supply Chain Campaign: Activity Through 2026-05-24, (Mon, May 25th)](https://isc.sans.edu/diary/rss/33016) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [TeamPCP Supply Chain Campaign: Activity Through 2026-05-24, (Mon, May 25th)](https://isc.sans.edu/diary/rss/33014) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

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
| [Ghost CMSのCVE-2026-26980を悪用した700以上のサイト乗っ取りによるClickFix攻撃](https://thehackernews.com/2026/05/ghost-cms-cve-2026-26980-exploited-to.html) | 28.0 | 46.0 | 54.0 |
| [オランダ、サイバー攻撃支援で800台のサーバーを押収し2人を逮捕](https://krebsonsecurity.com/2026/05/netherlands-seizes-800-servers-arrests-2-for-aiding-cyberattacks/) | 28.0 | 20.0 | 42.0 |
| [Radiology Associates of Richmondでのデータ侵害、26万6000人に影響](https://www.securityweek.com/266000-affected-by-data-breach-at-radiology-associates-of-richmond/) | 28.0 | 20.0 | 42.0 |
| [Laravel-Langパッケージがマルウェア配布のために改ざんされる](https://www.securityweek.com/laravel-lang-packages-poisoned-for-malware-delivery/) | 28.0 | 20.0 | 42.0 |
| [Lazarus、金融・暗号資産企業を狙ってRemotePEメモリ常駐型RATを展開](https://thehackernews.com/2026/05/lazarus-deploys-remotepe-memory-only.html) | 28.0 | 20.0 | 42.0 |
| [富士通、学び続けるマルチAIエージェント技術を開発--業務経験を自ら検証、学習](https://japan.zdnet.com/article/35247971/) | 28.0 | 20.0 | 42.0 |
| [「Claude Mythos」が1万件以上の脆弱性を発見 しかし修正追い付かず Anthropicが報告書](https://www.itmedia.co.jp/news/articles/2605/25/news130.html) | 26.0 | 20.0 | 42.0 |
| [日大、教職員1万人が「Google AI Pro」活用へ](https://www.itmedia.co.jp/news/articles/2605/25/news129.html) | 26.0 | 20.0 | 42.0 |
| [Anthropicの制限付きClaude MythosモデルがClaude Codeに登場する可能性](https://www.bleepingcomputer.com/news/artificial-intelligence/anthropics-restricted-claude-mythos-model-may-be-coming-to-claude-code/) | 25.0 | 20.0 | 42.0 |
| [Anthropic、Claude向けに28件のセキュリティおよびコンプライアンス統合を追加](https://www.helpnetsecurity.com/2026/05/25/anthropic-security-compliance-integrations-claude/) | 25.0 | 20.0 | 42.0 |
| [Cisco、AI時代に向けたリスクベース脆弱性開示を改訂](https://www.helpnetsecurity.com/2026/05/25/cisco-risk-based-vulnerability-disclosure-ai/) | 25.0 | 20.0 | 42.0 |
| [アラートの洪水にようやく対抗策が現れる](https://thehackernews.com/2026/05/the-alert-firehose-finally-meets-its.html) | 25.0 | 20.0 | 42.0 |
| [Anthropic、1,000のOSSプロジェクトで23,000件の潜在的脆弱性を検出](https://www.securityweek.com/anthropic-mythos-detected-23000-potential-vulnerabilities-across-1000-oss-projects/) | 25.0 | 20.0 | 42.0 |
| [Microsoft Access VBAに関する脆弱性情報](https://isc.sans.edu/diary/rss/33012) | 22.0 | 20.0 | 42.0 |
| [交通指導員が小学校児童の登下校用名簿を紛失 - 名古屋市](https://www.security-next.com/184673) | 22.0 | 20.0 | 42.0 |
| [メール誤送信、ポイント事業参加店舗のメアドが流出 - 宮城県](https://www.security-next.com/184887) | 22.0 | 20.0 | 42.0 |
| [人間には普通の契約書に見えるのに「嘘のフォント」でAIだけ別の文章を読まされる「Noroboto」攻撃とは？](https://gigazine.net/news/20260525-noroboto/) | 22.0 | 20.0 | 42.0 |
| [マクドナルド店頭の注文端末が使いにくいと物議に 広報「アップデートを行っているところ」](https://www.itmedia.co.jp/news/articles/2605/25/news137.html) | 21.0 | 20.0 | 42.0 |
| [U-NEXT、アニメ制作会社GoHandsを買収 過去作に「生徒会役員共」「デキる猫は今日も憂鬱」など](https://www.itmedia.co.jp/news/articles/2605/25/news128.html) | 21.0 | 20.0 | 42.0 |
| [基地局が"クマ見張り役"に ドコモ、AIカメラで出没検知の実証実験 北海道で](https://www.itmedia.co.jp/news/articles/2605/25/news127.html) | 21.0 | 20.0 | 42.0 |
| [NTT、クボタ、NTTドコモが山間部におけるロボット農機の遠隔操作実験--モバイル通信と衛星通信の連携](https://japan.zdnet.com/article/35247975/) | 21.0 | 20.0 | 42.0 |
| [PayPay誘導型が急増、4月下旬にはフィッシング報告の半数に 中国発攻撃も復活](https://news.mynavi.jp/techplus/article/20260525-4485997/) | 21.0 | 20.0 | 42.0 |
| [近鉄とシャープ、画像処理技術を活用した車両床下検査システム--異常の有無を自動で検査](https://japan.zdnet.com/article/35247969/) | 21.0 | 20.0 | 42.0 |
| [AIデータセンター、電力と冷却が限界に--シュナイダーが示す次世代インフラ](https://japan.zdnet.com/article/35247967/) | 21.0 | 20.0 | 42.0 |

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
