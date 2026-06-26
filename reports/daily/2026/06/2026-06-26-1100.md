# 📡 サイレーダー 2026-06-26 11:00 JST

このレポートは、2026-06-26 05:00 JST〜2026-06-26 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 57
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 30

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [「Cisco Unified CM」など脆弱性2件の悪用に注意喚起 - 米当局](#topic-19421) | 39.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [AIエージェント時代、CAPTCHAは消えるのか？ 次に来るWeb防御の正体](#topic-19464) | 34.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [Photo ZIP campaign targeting hospitality industry delivers Node.<wbr>js implant for persistent access](#topic-19448) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-19421"></a>

### 1. 「Cisco Unified CM」など脆弱性2件の悪用に注意喚起 - 米当局

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

米当局が、Ciscoのコミュニケーション基盤ソフトとPTCの業務ソフトで見つかった脆弱性について、悪用が確認されているとして注意喚起を行いました。
対象製品を利用している組織には、早急な対策が求められています。実際の悪用が示されているため、単なる未修正の脆弱性よりも優先度が高い事案です。
業務通信や基幹系に関わる製品が含まれる可能性があり、影響範囲の確認が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 対象製品の利用有無を確認し、ベンダーの修正情報と緩和策を速やかに確認する。
- 外部公開の管理画面や関連サービスの露出状況を点検し、不要な公開を見直す。
- 監視強化を行い、異常な認証・設定変更・通信の兆候がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-12569 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20230 | 関連CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [「Cisco Unified CM」など脆弱性2件の悪用に注意喚起 - 米当局](https://www.security-next.com/186433) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補あり（URL 3件以上 / 該当CVE 1件）。

---

<a id="topic-19464"></a>

### 2. AIエージェント時代、CAPTCHAは消えるのか？ 次に来るWeb防御の正体

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 34.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

CAPTCHAは長年、人間と機械を見分けるためのWeb防御として使われてきましたが、生成AIやブラウザエージェントの普及でその前提が揺らぎつつあります。
記事は、CAPTCHAをめぐる攻防の変化と、今後のWeb防御がどの方向へ進むのかを歴史的な流れも踏まえて整理しています。
AIが自動でWeb操作を行う場面が増えると、従来の「人間らしさ」を前提にした判定だけでは十分でない可能性があります。
認証やボット対策を運用する側にとって、今後の防御設計を見直すきっかけになる話題です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- CAPTCHA単独に依存せず、行動分析やレート制御など複数の対策を組み合わせているか確認する。
- 生成AIやブラウザ自動化を前提に、ログイン・登録・決済など重要導線の不正利用検知を点検する。
- ユーザー体験と防御強度の両立を意識し、誤検知や離脱の影響も含めて運用を見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [AIエージェント時代、CAPTCHAは消えるのか？　次に来るWeb防御の正体](https://atmarkit.itmedia.co.jp/ait/articles/2606/26/news043.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-19448"></a>

### 3. Photo ZIP campaign targeting hospitality industry delivers Node.<wbr>js implant for persistent access

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoft Threat Intelligenceは、欧州とアジアの宿泊業界の組織を狙った多段階の侵入キャンペーンを確認したとしています。
写真を装ったZIPアーカイブや画像に見せかけたショートカットファイルが使われ、Node.<wbr>jsのインプラントを通じて継続的なアクセスにつながる可能性が示されています。
宿泊業界は予約、顧客情報、社内運用など多様な情報を扱うため、侵入が起きると影響が広がりやすい点が注目されます。
正規ファイルに見せかけた誘導が使われているとされ、利用者側の警戒だけでなく端末防御と検知の見直しが重要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ZIPやショートカット形式の不審な添付ファイルを入口に、メール経由の受信・展開を再点検する。
- Node.<wbr>js関連の不審な常駐や、通常業務と合わないプロセス生成・外部通信を監視対象に含める。
- 宿泊業界の業務端末では、権限分離、マクロやスクリプト実行の制御、EDRのアラート確認を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Photo ZIP campaign targeting hospitality industry delivers Node.<wbr>js implant for p](https://www.microsoft.com/en-us/security/blog/2026/06/25/photo-zip-campaign-targeting-hospitality-industry-delivers-node-js-implant-persistent-access/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
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
| [山一電機 フィリピン子会社にランサムウェア攻撃、ログの暗号化と削除が行われ初期侵入経路の完全な特定に至らず](https://scan.netsecurity.ne.jp/article/2026/06/26/55583.html) | 29.0 | 30.0 | 42.0 |
| [身代金要求型攻撃グループに企業侵入口を販売するアクセスブローカーに関連した自己破壊型Misticバックドア](https://www.theregister.com/security/2026/06/25/self-destructing-mistic-backdoor-linked-to-access-broker-selling-corporate-footholds-to-ransomware-gangs/5262579) | 28.0 | 30.0 | 42.0 |
| [Ex-Huntressアナリストが、社内関係者がランサムウェア犯に情報を流していたと主張、SNSで騒動に発展](https://www.theregister.com/cyber-crime/2026/06/25/ex-huntress-analyst-claims-company-insider-fed-info-to-a-ransomware-crim-social-media-drama-ensues/5262538) | 28.0 | 30.0 | 42.0 |
| [Russian APT「Gamaredon」が攻撃手法を強化、新たな防御が必要に](https://www.darkreading.com/threat-intelligence/russia-apt-gamaredon-arsenal-defense) | 28.0 | 20.0 | 42.0 |
| [HENNGE、「東京大学 × ベンチャー企業産学連携 AI 研究フォーラム」に参画](https://scan.netsecurity.ne.jp/article/2026/06/26/55577.html) | 26.0 | 20.0 | 42.0 |
| [Notion、メールアプリ「Notion Mail」終了へ AIエージェントに全面移行](https://www.itmedia.co.jp/news/articles/2606/26/news060.html) | 26.0 | 20.0 | 42.0 |
| [AIチャットボットはPCの問題解決に使えるか--「Copilot」に効果的な方法を尋ねてみた](https://japan.zdnet.com/article/35249403/) | 26.0 | 20.0 | 42.0 |
| [Anthropicがモバイル向けにデスクトップ版のClaude Coworkをテスト中](https://www.bleepingcomputer.com/news/artificial-intelligence/anthropic-is-testing-desktop-like-claude-cowork-for-mobile/) | 25.0 | 20.0 | 42.0 |
| [「Chrome」が脆弱性を修正 - 前回アップデートから2日](https://www.security-next.com/186427) | 22.0 | 20.0 | 42.0 |
| [セールスフォースが説く「エージェンティックエンタープライズへの“4R”の取り組み」とは](https://japan.zdnet.com/article/35249452/) | 21.0 | 20.0 | 42.0 |
| [「Windows 10」の無料サポート延長プログラム、2027年10月12日まで1年間再延期](https://www.itmedia.co.jp/news/articles/2606/26/news061.html) | 21.0 | 20.0 | 42.0 |
| [狙われたのは忘れられたシステム ～ サイバー攻撃被害企業が語ったインシデント対応の現実](https://scan.netsecurity.ne.jp/article/2026/06/26/55585.html) | 21.0 | 20.0 | 42.0 |
| [苫小牧民報社記者が個人情報含む文書をSNS投稿、「報道機関としてはあってはならない」](https://scan.netsecurity.ne.jp/article/2026/06/26/55584.html) | 21.0 | 20.0 | 42.0 |
| [ファクトリージャパングループに不正アクセス](https://scan.netsecurity.ne.jp/article/2026/06/26/55582.html) | 21.0 | 20.0 | 42.0 |
| [「佐嘉平川屋オンラインショップ」に不正アクセス、5,783 名のカード情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/06/26/55581.html) | 21.0 | 20.0 | 42.0 |
| [セキュリティシステムの誤検知で「お問い合わせ内容の通知メール」が不通に](https://scan.netsecurity.ne.jp/article/2026/06/26/55580.html) | 21.0 | 20.0 | 42.0 |
| [個人情報部分を非表示処理にとどめた状態を削除済みと誤認 ～ 川越商工会議所で会員データを外部に送信](https://scan.netsecurity.ne.jp/article/2026/06/26/55579.html) | 21.0 | 20.0 | 42.0 |
| [5つのKubernetes認定を全制覇 ～ スリーシェイク川俣裕紀氏が「Kubestronaut」に認定](https://scan.netsecurity.ne.jp/article/2026/06/26/55578.html) | 21.0 | 20.0 | 42.0 |
| [HENNGE One、ノーコード業務アプリ作成ツール「サスケWorks」と SSO 連携](https://scan.netsecurity.ne.jp/article/2026/06/26/55576.html) | 21.0 | 20.0 | 42.0 |
| [7 / 30・31 開催「Google Cloud Next Tokyo」にHENNGEが出展、豊田龍彦氏 登壇](https://scan.netsecurity.ne.jp/article/2026/06/26/55575.html) | 21.0 | 20.0 | 42.0 |
| [「検知してから対応」はもう遅い――WithSecureが語る“AI時代の敗北条件”](https://atmarkit.itmedia.co.jp/ait/articles/2606/26/news040.html) | 21.0 | 20.0 | 42.0 |
| [「漏えい確認なし」でもサーバ廃止へ NTTPCが下した異例の判断、その背景は](https://atmarkit.itmedia.co.jp/ait/articles/2606/25/news134.html) | 21.0 | 20.0 | 42.0 |
| [誰かがアカウントを監視・不正アクセスしている10の兆候と対策](https://japan.zdnet.com/article/35249224/) | 21.0 | 20.0 | 42.0 |
| [終わらない「レガシー延命」が命取りに AI時代のサイバー危機にセキュリティ機関が声明](https://www.itmedia.co.jp/enterprise/articles/2606/25/news105.html) | 21.0 | 20.0 | 42.0 |
| [Yubicoに聞く、なぜ今物理的な「セキュリティキー」が必要なのか](https://japan.zdnet.com/article/35249377/) | 21.0 | 20.0 | 42.0 |
| [CISA ICS Advisory / ICS Medical Advisory（2026年06月25日）](https://jvn.jp/vu/JVNVU99109287/) | 20.0 | 20.0 | 42.0 |
| [PolandでSIMスワッピング犯グループを摘発、数百万ドル規模の暗号資産窃取に関与](https://www.bleepingcomputer.com/news/security/poland-busts-sim-swapping-gang-tied-to-millions-in-crypto-theft/) | 20.0 | 20.0 | 42.0 |
| [「フリマサイトの画像流用」「コード決済の『送る』機能を使わせる」など、悪質通販サイトの新手口を国民センターが説明](https://internet.watch.impress.co.jp/docs/news/2119769.html) | 20.0 | 20.0 | 42.0 |
| [24時間足らずで武器化されたCisco CUCMの脆弱性](https://www.darkreading.com/cyberattacks-data-breaches/less-than-24-hours-attackers-weaponize-cisco-cucm-flaw) | 20.0 | 20.0 | 42.0 |
| [EdTech攻撃者が学校からソフトウェア供給元へ標的を移す](https://www.darkreading.com/cyberattacks-data-breaches/edtech-attackers-shift-schools-software-suppliers) | 20.0 | 20.0 | 42.0 |

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
