# 📡 サイレーダー 2026-05-20 05:00 JST

このレポートは、2026-05-19 17:00 JST〜2026-05-20 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 116
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [Exposing Fox Tempest: A malware-signing service operation](#topic-7178) | 38.0 | 30.0 | 48.0 | 音声 | 温度感上位枠 |
| 2 | [Huawei zero-day attack behind last year’s crash of Luxembourg's entire telecoms network](#topic-7164) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Microsoft disrupts Fox Tempest malware-signing-as-a-service platform tied to ransomware gangs](#topic-7169) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Microsoft Disrupts Malware-Signing Service Run by ‘Fox Tempest’](#topic-7173) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Microsoft disrupts cybercrime service that abused software verification systems en masse](#topic-7180) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-7178"></a>

### 1. Exposing Fox Tempest: A malware-signing service operation

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> / <nobr>マルウェア</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>脅威アクター</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 38.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 48.0 |

#### 概要

Microsoftの公開情報によると、Fox Tempestは金銭目的の脅威アクターで、他のサイバー犯罪者向けにマルウェアの署名を支援する「malware-signing-as-a-service（MSaaS）」を運用していたとされています。
これにより、Vanilla Tempestや一部のStorm系グループなどが、ランサムウェアを含む悪意あるコードをより通しやすく配布していた可能性が示されています。
署名付きの不正コードは、検知や信頼の見た目をすり抜けやすく、防御側の判断を難しくします。
ランサムウェアの流通を支える周辺サービスの実態が明らかになる点でも、実務上の関心が高い話題です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 署名の有無だけで信頼せず、配布元・挙動・証明書の不自然さも含めて確認する。
- ランサムウェア関連の封じ込めでは、侵入経路だけでなく、署名済み不正ファイルの流通も前提に監視する。
- Microsoftなどの脅威情報を参照し、関連するグループ名や活動パターンを検知ルールや調査観点に反映する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ransomware_group | Akira | 主題 | 0.80 |
| ransomware_group | Qilin | 主題 | 0.80 |
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Exposing Fox Tempest: A malware-signing service operation](https://www.microsoft.com/en-us/security/blog/2026/05/19/exposing-fox-tempest-a-malware-signing-service-operation/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-7164"></a>

### 2. Huawei zero-day attack behind last year’s crash of Luxembourg's entire telecoms network

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ゼロデイ</nobr> / <nobr>脆弱性</nobr> / <nobr>通信基盤</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

昨年ルクセンブルクの通信網全体に障害が発生した件について、Huawei製品に関するゼロデイ攻撃が背景にあった可能性が報じられています。
現時点では同様の事象の再発は確認されておらず、原因となった脆弱性の詳細も公には説明されていません。
通信インフラ全体に影響が及ぶと、広範なサービス停止につながるため、影響範囲の大きさが注目されています。
原因が未解明のままだと、同種環境を運用する組織では継続的な監視とリスク評価が必要になります。

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

- 該当ベンダー製機器を使う通信・ネットワーク環境では、障害時の切り分け手順とログ保全を改めて確認する。
- 重要インフラや基幹網では、単一機器・単一経路への依存を避け、冗長化とフェイルオーバーの動作確認を行う。
- ベンダーの通知、修正情報、回避策の有無を継続的に追い、未解明の障害として扱う間は監視を強める。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Huawei zero-day attack behind last year’s crash of Luxembourg's entire telecoms ](https://therecord.media/huawei-zero-day-behind-last-year-luxembourg-telecom-outage) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 初出。

---

<a id="topic-7169"></a>

### 3. Microsoft disrupts Fox Tempest malware-signing-as-a-service platform tied to ransomware gangs

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>マルウェア</nobr> / <nobr>ランサムウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Microsoftは、ランサムウェア集団につながるとされる「Fox Tempest」というマルウェア署名支援サービスの妨害に踏み切ったと明らかにしました。
公開された訴訟資料によると、このサービスは2025年5月から活動していたとされ、サイバー犯罪者向けにコード署名に関わる機能を提供していたようです。
コード署名の悪用は、悪性ファイルの信頼性を装う手口に結びつくため、検知や封じ込めを難しくする可能性があります。
ランサムウェア関連の支援基盤が断たれることで、関連攻撃の継続性に影響が出る点が注目されます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 正規のコード署名証明書や署名済みファイルを前提にした信頼判断を見直す。
- 署名済みでも不審な配布経路・実行挙動を検知できるよう、端末側の監視を強化する。
- ランサムウェア関連の初期侵入・横展開・実行兆候に対するログ確認とアラート設定を再点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft disrupts Fox Tempest malware-signing-as-a-service platform tied to ran](https://therecord.media/microsoft-disrupts-fox-tempest-malware-signing-service) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-7173"></a>

### 4. Microsoft Disrupts Malware-Signing Service Run by ‘Fox Tempest’

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>マルウェア</nobr> / <nobr>ランサムウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Microsoftが、Fox Tempestとされるグループに関連したマルウェア署名サービスを妨害したと報じられています。
このサービスは、正規ソフトを装ってランサムウェアや他のマルウェアを配布する用途で悪用されていたとされています。
正規ソフトに見せかけた配布は検知や利用者の見分けを難しくするため、ランサムウェア対策の観点で注目されます。
今回の件は、脅威アクターの流通基盤に対する対処が行われた事例として重要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 正規ソフトに見える実行ファイルや署名付きファイルでも、入手元と配布経路の確認を徹底する。
- 不審な配布物に対しては、署名の有無だけでなく、ハッシュ・配布元・更新経路を含めて検証する。
- ランサムウェア文脈のため、検知ルールや隔離手順、ユーザー通知フローを改めて確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft Disrupts Malware-Signing Service Run by ‘Fox Tempest’](https://www.securityweek.com/microsoft-disrupts-malware-signing-service-run-by-fox-tempest/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-7180"></a>

### 5. Microsoft disrupts cybercrime service that abused software verification systems en masse

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> / <nobr>マルウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Microsoft disrupts cybercrime service that abused software verification systems en masse に関する脅威・攻撃キャンペーン系の話題です。
攻撃者、標的、TTP、IoC、悪用技術、検知観点を中心に確認する価値があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 標的OS、仮想化基盤、暗号化対象、バックアップ影響を確認する。
- 初期侵入、横展開、認証情報窃取、永続化のTTPを確認する。
- EDR/SIEMで検知すべきIoCや振る舞いを確認する。
- ESXi、vCenter、バックアップ基盤、特権アカウントの保護状況を確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ransomware_group | Akira | 主題 | 0.80 |
| ransomware_group | Qilin | 主題 | 0.80 |
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft disrupts cybercrime service that abused software verification systems ](https://cyberscoop.com/microsoft-digital-crimes-unit-disrupts-fox-tempest/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

今回はGitHubのみ掲載の注目トピックはありません。

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [ZKTeco製CCTVカメラ](https://www.cisa.gov/news-events/ics-advisories/icsa-26-139-04) | 32.0 | 46.0 | 50.0 |
| [Linux KernelのCVE-2026-31635 LPE脆弱性に対するDirtyDecrypt PoC公開](https://thehackernews.com/2026/05/dirtydecrypt-poc-released-for-linux.html) | 31.0 | 50.0 | 52.0 |
| [PDB文字列からMaaSへ：中国語話者の脅威アクターが利用する一般的なBadIISエコシステムの追跡](https://blog.talosintelligence.com/from-pdb-strings-to-maas-tracking-a-commodity-badiis-ecosystem/) | 30.0 | 20.0 | 42.0 |
| [Mini Shai-Huludが再来、数百件のnpmパッケージが侵害される](https://cyberscoop.com/mini-shai-hulud-malware-npm-packages-compromised-again/) | 28.0 | 45.0 | 42.0 |
| [Shai-Huludマルウェアの新たな波が600件のnpmパッケージを侵害](https://www.bleepingcomputer.com/news/security/new-shai-hulud-malware-wave-compromises-600-npm-packages/) | 28.0 | 35.0 | 42.0 |
| [Microsoftがランサムウェア支援の署名ツールを提供していたFox Tempestを摘発](https://www.infosecurity-magazine.com/news/microsoft-takes-down-fox-tempest/) | 28.0 | 30.0 | 42.0 |
| [Microsoft Self-Service Password Resetを悪用したAzureデータ窃取攻撃](https://www.bleepingcomputer.com/news/security/microsoft-self-service-password-reset-abused-in-azure-data-theft-attacks/) | 28.0 | 20.0 | 42.0 |
| [Trapdoor Android広告詐欺スキームが455アプリを使って1日6億5900万件の入札リクエストを発生させた件](https://thehackernews.com/2026/05/trapdoor-android-ad-fraud-scheme-hit.html) | 28.0 | 20.0 | 42.0 |
| [PureLogs infostealerが世界中で認証情報を窃取](https://www.helpnetsecurity.com/2026/05/19/purelogs-infostealer-delivery-steganography/) | 28.0 | 20.0 | 42.0 |
| [レガシーなWindowsツールMSHTAがサイレントマルウェア攻撃の急増を助長](https://www.securityweek.com/legacy-windows-tool-mshta-fuels-surge-in-silent-malware-attacks/) | 28.0 | 20.0 | 42.0 |
| [Google、“動画版Nano Banana”こと「Gemini Omni」公開 会話で映像を生成・編集](https://www.itmedia.co.jp/news/articles/2605/20/news063.html) | 26.0 | 20.0 | 42.0 |
| [日立、Anthropicと提携 グループ29万人に「Claude」などAI導入 社会インフラ分野にも展開へ](https://www.itmedia.co.jp/news/articles/2605/19/news120.html) | 26.0 | 20.0 | 42.0 |
| [デル、「Dell Deskside Agentic AI」を発表--AIとデータの主導権は「企業が握れ！」](https://japan.zdnet.com/article/35247694/) | 26.0 | 20.0 | 42.0 |
| [Taskhost Windows タスクにおけるローカル権限昇格の脆弱性（CVE-2025-60710）](https://nvd.nist.gov/vuln/detail/CVE-2025-60710) | 25.0 | 82.0 | 81.0 |
| [Rapid7の2026年グローバルサイバーセキュリティサミット：セキュリティリーダー向けの重要ポイント](https://www.rapid7.com/blog/post/it-2026-global-cybersecurity-summit-key-takeaways-security-leaders) | 25.0 | 20.0 | 42.0 |
| [サイバー進化の動的なブイヤベースを振り返り、未来を見据える](https://www.darkreading.com/cybersecurity-operations/looking-back-looking-forward-bouillabaisse-cyber-evolution) | 25.0 | 20.0 | 42.0 |
| [Selector、AI駆動の可観測性をマルチクラウド環境へ拡張](https://www.helpnetsecurity.com/2026/05/19/selector-ai-driven-observability-capabilities/) | 25.0 | 20.0 | 42.0 |
| [LaunchDarkly、運用中のAIエージェントにリアルタイム制御機能を追加](https://www.helpnetsecurity.com/2026/05/19/launchdarkly-agentcontrol/) | 25.0 | 20.0 | 42.0 |
| [Canonical、Ubuntu Core 26を15年間のセキュリティ保守付きで提供](https://www.helpnetsecurity.com/2026/05/19/ubuntu-core-26-released/) | 25.0 | 20.0 | 42.0 |
| [AIが脆弱性認識とセキュア・バイ・デザインなソフトウェアの基準を引き上げる](https://www.infosecurity-magazine.com/news/ai-raises-vulnerability-awareness/) | 25.0 | 20.0 | 42.0 |
| [Agentic AIがソフトウェアビルドとモバイルアプリ攻撃を加速させる](https://www.infosecurity-magazine.com/news/agentic-ai-accelerates-software/) | 25.0 | 20.0 | 42.0 |
| [2026年に企業を狙うフィッシング主導のソーシャルエンジニアリング攻撃5選](https://any.run/cybersecurity-blog/social-engineering-attacks-2026/) | 25.0 | 20.0 | 42.0 |
| [YouTube、ディープフェイク対策に顔認証を導入へ](https://www.malwarebytes.com/blog/ai/2026/05/youtube-wants-your-face-to-fight-deepfakes) | 25.0 | 20.0 | 42.0 |
| [ABB CoreSense HMおよびCoreSense M10の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-139-01) | 24.0 | 46.0 | 50.0 |

---

## 📊 スコアの見方

| <nobr>指標</nobr> | 意味 |
|---|---|
| <nobr>温度状態</nobr> | 話題のライフサイクルを示す補助ラベルです。例: 低温、継続監視、温度上昇中、高温、冷却中。 |
| <nobr>温度感</nobr> | 話題として今どれだけ注目・拡散・更新されているかを示します。 |
| <nobr>実務影響</nobr> | 対象組織・担当者にとって、対応優先度や被害可能性がどれだけ大きいかを示します。 |
| <nobr>確度</nobr> | 公的機関、ベンダー公式、複数ソース、CVE/KEV、一次資料などにより、情報をどれだけ確認できているかを示します。事件報道系は、複数報道があっても司法文書・当局発表などの一次資料が弱い場合、脆弱性KEV系より低く出ることがあります。 |

スコアは、公開情報から抽出した特徴量と事前定義した重み付けに基づく参考指標です。詳しい算出方針は [スコアリング方針](../docs/scoring.md) を参照してください。

## 🔒 公開しない内部情報について

サイレーダーでは、温度感の補助シグナルとして、公的機関・ベンダー公式・信頼できる報道機関・技術者コミュニティ・国内外の公開反応などを利用します。

これらのシグナルは、一次情報、報道波及、技術者反応、開発者反応、PoC・悪用観測などに分けて評価します。

ただし、ランキング操作、スパム的誘導、監視回避を防ぐため、個別の監視対象、取得手段、検索条件、評価対象サービス名、内部的な重み付けやしきい値は公開しません。

また、公開反応の多さだけで掲載順位を決めることはありません。重要度の判定では、ベンダー公式情報、公的機関、一次資料、信頼できる技術分析、実務影響を優先します。

## ⚠️ 注意事項

このレポートは、収集・観測できた公開情報をもとにした参考情報です。完全性、正確性、即時性を保証するものではありません。

重要な判断を行う場合は、必ずベンダー公式情報、公的機関、一次情報を確認してください。

サイレーダーは、広告・スポンサー・企業関係に基づいて掲載順位や温度感スコアを変更しません。
