# 📡 サイレーダー 2026-05-27 11:00 JST

このレポートは、2026-05-27 05:00 JST〜2026-05-27 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 83
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Weekly Report: Palo Alto Networks製PAN-OSにおける認証回避の脆弱性（CVE-2026-0265）に関する注意喚起](#topic-4257) | 47.0 | 74.0 | 60.0 | 音声 | 温度感上位枠 |
| 2 | [KnowledgeDeliver flaw exploited as a zero-day to install web shells](#topic-10418) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [From poisoned search results to GPU mining: A cryptojacking campaign abusing ScreenConnect and Microsoft .<wbr>NET utilities](#topic-10561) | 35.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-4257"></a>

### 1. Weekly Report: Palo Alto Networks製PAN-OSにおける認証回避の脆弱性（CVE-2026-0265）に関する注意喚起

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>認証バイパス</nobr> / <nobr>KEV</nobr> / <nobr>防御・運用</nobr> / <nobr>脅威アクター</nobr> / <nobr>政策・規制</nobr> / <nobr>PoC</nobr> / <nobr>クラウド</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 再燃 |
| <nobr>温度感</nobr> | 47.0 |
| <nobr>実務影響</nobr> | 74.0 |
| <nobr>確度</nobr> | 60.0 |

#### 概要

Palo Alto NetworksのPAN-OSに認証回避の脆弱性（CVE-2026-0265）が公表され、Cloud Authentication Service（CAS）を有効にしている構成で影響を受ける可能性が示されています。
対象はPA-Series、VM-Series、Panoramaの一部で、Cloud NGFWとPrisma Accessは影響なしとされています。
認証を迂回されると、管理系や公開ログイン面への不正アクセスにつながるおそれがあるためです。公開情報では実証やPoC言及もあり、該当構成の有無確認と修正適用が注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 公開PoC・検証コード言及あり。
- 公開PoC/Exploitコード: 確認あり。
- 直接PoCリンク: 掲載しません。
- 確認方針: NVD、ベンダー公式、公的機関、信頼できる技術分析を優先し、GitHub等のコードは防御・検証目的で別途確認します。

#### 担当者向け確認ポイント

- CASを使った認証プロファイルがログインインターフェースに付与されているか確認する。
- 影響対象バージョンの場合は、利用系統に応じた修正版への更新を優先する。
- 旧式やサポート外のPAN-OSを使っている場合は、サポート対象の固定版への移行計画を早めに立てる。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-0265 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-0300 | 主要CVE | 1.00 |
| ベンダー | Palo Alto | 言及あり | 0.80 |
| ベンダー | Cisco | 言及あり | 0.80 |
| ベンダー | Atlassian | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-0265](https://nvd.nist.gov/vuln/detail/CVE-2026-0265) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>公的・一次情報</nobr> | [Weekly Report: Palo Alto Networks製PAN-OSにおける認証回避の脆弱性（CVE-2026-0265）に関する注意喚起](https://www.jpcert.or.jp/wr/2026/wr260527.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>公的・一次情報</nobr> | [注意喚起: Palo Alto Networks製PAN-OSにおける認証回避の脆弱性（CVE-2026-0265）に関する注意喚起  (公開)](https://www.jpcert.or.jp/at/2026/at260015.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0265: Authentication Bypass in Palo Alto Networks PAN-OS](https://www.rapid7.com/blog/post/etr-cve-2026-0265-authentication-bypass-in-palo-alto-networks-pan-os) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0265 PAN-OS: Authentication Bypass with Cloud Authentication Service (C](https://security.paloaltonetworks.com/CVE-2026-0265) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: あり。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。

---

<a id="topic-10418"></a>

### 2. KnowledgeDeliver flaw exploited as a zero-day to install web shells

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ゼロデイ</nobr> / <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

KnowledgeDeliver の学習管理システム（LMS）を搭載したサーバーにおいて、重大なゼロデイ脆弱性が悪用され、Godzilla web shell の設置につながったと報じられています。
現時点の情報では、悪用が観測されている点が重要ですが、影響範囲や被害の詳細は限定的です。
ゼロデイとして実際に悪用されているため、該当製品を利用する組織では迅速な確認と対応が必要になる可能性があります。
web shell の設置は侵害後の継続的な不正操作につながりやすく、監視と封じ込めが重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- KnowledgeDeliver を利用しているサーバーがないか棚卸しし、対象があればベンダー情報と更新状況を確認する。
- 不審なファイル改変、未知の管理者権限、異常な外部通信など、侵害の兆候を重点的に点検する。
- Web サーバー配下の変更履歴やアクセスログを見直し、疑わしい端末・アカウントがあれば隔離と調査を進める。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [KnowledgeDeliver flaw exploited as a zero-day to install web shells](https://www.bleepingcomputer.com/news/security/knowledgedeliver-flaw-exploited-as-a-zero-day-to-install-web-shells/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-10561"></a>

### 3. From poisoned search results to GPU mining: A cryptojacking campaign abusing ScreenConnect and Microsoft .<wbr>NET utilities

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>攻撃キャンペーン</nobr> / <nobr>AI</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 35.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Microsoftは、SEO汚染された検索結果を起点に、ScreenConnectやMicrosoft .<wbr>NET系のユーティリティを悪用して高性能PCを暗号資産マイニングに使うクリプトジャッキングの手口を公表しました。
悪性サイトがAIチャットボット経由でも見つかっていたとされ、検索や生成AIを経由した誘導にも注意が必要です。
正規ツールや広く使われる仕組みを悪用するため、検知や切り分けが難しくなるおそれがあります。
利用者が検索結果やAIの回答を起点に不審サイトへ誘導される点も、従来の警戒ポイントを広げる必要があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ScreenConnectなどのリモート管理ツールや .<wbr>NET 実行の不審な利用、未知の外部接続、GPU負荷の異常上昇を確認する。
- 検索経由・AI経由の誘導を前提に、ダウンロード元や配布サイトの真偽確認を徹底し、ユーザー向け注意喚起を行う。
- エンドポイント保護とログ監視で、正規ツールを装った実行や永続化の兆候を早期に把握できる体制を整える。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| ベンダー | VMware | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [From poisoned search results to GPU mining: A cryptojacking campaign abusing Scr](https://www.microsoft.com/en-us/security/blog/2026/05/26/poisoned-search-results-gpu-mining-cryptojacking-campaign-abusing-screenconnect-microsoft-net-utilities/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり・低信頼。
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
| [松沢書店にランサムウェア攻撃、「楽譜ナビ」「注文くん」ほか各種サービスに影響](https://scan.netsecurity.ne.jp/article/2026/05/27/55359.html) | 29.0 | 30.0 | 42.0 |
| [東京鋪装工業にランサムウェア攻撃、顧客・取引先・従業員の情報が流出した可能性を完全に否定できず](https://scan.netsecurity.ne.jp/article/2026/05/27/55356.html) | 29.0 | 30.0 | 42.0 |
| [新日本検定協会へのランサムウェア攻撃、共栄火災海上保険の顧客等の個人情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/05/27/55355.html) | 29.0 | 30.0 | 42.0 |
| [ランサムウェア被害は前年比389％増 爆増・爆速化の背景とは？](https://atmarkit.itmedia.co.jp/ait/articles/2605/27/news050.html) | 29.0 | 30.0 | 42.0 |
| [穴吹ハウジングサービスがランサム被害](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/041800012/051800327/) | 29.0 | 30.0 | 42.0 |
| [Claude Mythosが1万件超の脆弱性を発見 その裏で開発者コミュニティーに走る緊張](https://atmarkit.itmedia.co.jp/ait/articles/2605/27/news055.html) | 27.0 | 20.0 | 42.0 |
| [AI駆動開発と仕様駆動開発 見えてきた課題と現時点での開発環境の実装](https://ascii.jp/elem/000/004/404/4404615/?rss=) | 26.0 | 20.0 | 42.0 |
| [Google がウェブを AI の餌食にする共食いの構図](https://scan.netsecurity.ne.jp/article/2026/05/27/55361.html) | 26.0 | 20.0 | 42.0 |
| [AIエージェント導入で満足度が73％向上--オンライン旅行会社が実践した5つのステップ](https://japan.zdnet.com/article/35247671/) | 26.0 | 20.0 | 42.0 |
| [後編：進むべき道--AI時代の勝機をつかむ「ガバナンスファースト」戦略](https://japan.zdnet.com/article/35247837/) | 26.0 | 20.0 | 42.0 |
| [経理業務における対話型AI活用 約60％が「使用せず」と回答](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020600010/052100225/) | 26.0 | 20.0 | 42.0 |
| [VPNクライアント「OpenVPN Connect」macOS版に脆弱性 - 修正版公開](https://www.security-next.com/185001) | 22.0 | 20.0 | 42.0 |
| [「WebSphere」のウェブサーバプラグインに深刻な脆弱性](https://www.security-next.com/184994) | 22.0 | 20.0 | 42.0 |
| [「LiteSpeed cPanel Plugin」に脆弱性 - すでに悪用も、侵害有無の確認を](https://www.security-next.com/184986) | 22.0 | 20.0 | 42.0 |
| [秘密を分散させて漏えいを防ぐ「シャミアの秘密共有」の仕組みとは？](https://gigazine.net/news/20260527-shamirs-secret-sharing/) | 22.0 | 20.0 | 42.0 |
| [イミュータブル「Linux」ディストロ「Aurora」--使いやすさと安全性を両立](https://japan.zdnet.com/article/35248043/) | 21.0 | 20.0 | 42.0 |
| [ロッキング・オン・ジャパン、元従業員が個人情報をUSBメモリで持ち出し 退職時に](https://www.itmedia.co.jp/news/articles/2605/27/news069.html) | 21.0 | 20.0 | 42.0 |
| [AD環境ではパスワード変更だけでは侵害が止まらない理由とは](https://news.mynavi.jp/techplus/article/20260527-4456274/) | 21.0 | 20.0 | 42.0 |
| [正社員の5人に1人が「六月病」経験 6月前後にモチベ低下や疲労感](https://www.itmedia.co.jp/news/articles/2605/27/news068.html) | 21.0 | 20.0 | 42.0 |
| [「世界一地味なデモ」が魅せた圧倒的な性能 超高速タイムスタンプエンジン開発の舞台裏](https://ascii.jp/elem/000/004/404/4404870/?rss=) | 21.0 | 20.0 | 42.0 |
| [「食品減税」と「所得連動給付」どっちがお得？ 年収などから分かるシミュレータ、チームみらいが公開](https://www.itmedia.co.jp/news/articles/2605/27/news066.html) | 21.0 | 20.0 | 42.0 |
| [Dropboxの共同創業者、ヒューストンCEOが退任して会長へ](https://www.itmedia.co.jp/news/articles/2605/27/news067.html) | 21.0 | 20.0 | 42.0 |
| [不審メール送信アカウント廃止 ～ リスク排除の観点](https://scan.netsecurity.ne.jp/article/2026/05/27/55360.html) | 21.0 | 20.0 | 42.0 |
| [三浦工業への不正アクセス、5,021 件の個人情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/05/27/55358.html) | 21.0 | 20.0 | 42.0 |

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
