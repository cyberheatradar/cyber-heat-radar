# 📡 サイレーダー 2026-05-10 14:11 JST 試作版

このレポートは、2026-05-09 14:10 JST〜2026-05-10 14:10 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 49
- [音声で扱う想定のトピック](#audio-topics): 0
- [GitHubのみ掲載想定のトピック](#github-only-topics): 4
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>音声掲載理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 74.0 | 82.0 | 81.0 | GitHub | - |
| 2 | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](#topic-31) | 36.0 | 30.0 | 42.0 | GitHub | - |
| 3 | [Fake OpenAI repository on Hugging Face pushes infostealer malware](#topic-2068) | 33.0 | 20.0 | 42.0 | GitHub | - |
| 4 | [Threats Making WAVs - Incident Response to a Cryptomining Attack](#topic-29) | 30.0 | 20.0 | 42.0 | GitHub | - |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

今回は音声で扱う想定のトピックはありません。

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-12"></a>

### 1. Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>Windows</nobr> / <nobr>権限昇格</nobr> / <nobr>TTP</nobr> / <nobr>脆弱性</nobr> / <nobr>KEV</nobr> |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 74.0 |
| <nobr>実務影響</nobr> | 82.0 |
| <nobr>確度</nobr> | 81.0 |

#### 概要

CVE-2025-60710は、Microsoft WindowsのTaskhost関連タスクに起因するローカル権限昇格の脆弱性として整理されています。
CISAのKnown Exploited Vulnerabilitiesに含まれており、公開PoCや検証コードの言及もあるため、優先度の高い確認対象と見られます。
権限昇格系の脆弱性は、端末内での被害拡大や管理者権限の取得につながる可能性があるため、影響が大きくなりやすいです。
さらに、実利用や再現可能性を示す情報がある場合は、運用環境での対応を急ぐ必要があります。

#### CISA KEV詳細

- **CVE**: CVE-2025-60710
- **Vendor / Project**: Microsoft
- **Product**: Windows
- **Vulnerability Name**: Microsoft Windows Link Following Vulnerability
- **Date Added**: 2026-04-13
- **Due Date**: 2026-04-27
- **Known Ransomware Use**: Unknown

**Required Action**

> Apply mitigations per vendor instructions, follow applicable BOD 22-01 guidance for cloud services, or discontinue use of the product if mitigations are unavailable.

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- CISA KEV関連。
- 公開PoC・検証コード言及あり。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 公開PoCにより再現・悪用可能性が上がる。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 公開PoC・検証コード言及あり。
- 公開PoC/Exploitコード: 確認あり。
- 直接PoCリンク: 掲載しません。
- 確認方針: NVD、ベンダー公式、公的機関、信頼できる技術分析を優先し、GitHub等のコードは防御・検証目的で別途確認します。

#### 担当者向け確認ポイント

- Windows端末で該当CVEの影響有無を確認し、ベンダーの修正情報や回避策を適用する。
- 特権アカウントの利用状況と、Taskhost関連の不審な挙動や異常な権限昇格の兆候を監視する。
- 優先度の高い脆弱性として、資産台帳に基づく対象範囲の洗い出しとパッチ適用計画を前倒しで進める。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-60710 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 影響ベンダー | 1.00 |
| 製品 | Windows | 影響製品 | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-60710](https://nvd.nist.gov/vuln/detail/CVE-2025-60710) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>公的機関</nobr> | [CISA KEV: CVE-2025-60710](https://www.cisa.gov/known-exploited-vulnerabilities-catalog?field_cve=CVE-2025-60710) | <nobr>KEV掲載内容、Date Added、Due Date、Required Action</nobr> |
| <nobr>公的機関データ</nobr> | [CISA KEV JSON](https://www.cisa.gov/sites/default/files/feeds/known_exploited_vulnerabilities.json) | <nobr>CISA公式の機械可読データ。CVE IDで検索して確認</nobr> |
| <nobr>出典</nobr> | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](https://github.com/Wh04m1001/CVE-2025-60710) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。
- 継続観測: 継続。

---

<a id="topic-31"></a>

### 2. PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>防御・運用</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Akamai Security Intelligence が、MySQL サーバーを狙うランサムウェアのキャンペーンを取り上げています。
公開情報では、攻撃者が二重恐喝の手口を用い、被害者への圧力としてデータ公開を行っているとされています。
MySQL は業務システムの基盤として使われることが多く、侵害されると広い範囲に影響が及ぶ可能性があります。
ランサムウェアは暗号化だけでなく情報流出を伴う場合があり、復旧と対外対応の負担が大きくなりやすい点が注目されます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- MySQL サーバーの公開範囲、認証設定、アクセス制御を点検し、不要な露出を減らす。
- バックアップの取得状況と復元手順を確認し、実際に戻せるか定期的に検証する。
- 監視ログやアラートで、不審な認証失敗や想定外の管理操作を早期に検知できるようにする。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](https://akamai.com/blog/security/please-read-me-opportunistic-ransomware-devastating-mysql-servers) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 未評価。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-2068"></a>

### 3. Fake OpenAI repository on Hugging Face pushes infostealer malware

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>マルウェア</nobr> / <nobr>Windows</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Hugging Face上で、OpenAIの「Privacy Filter」プロジェクトを装った不正なリポジトリが見つかり、Windows利用者向けに情報窃取型マルウェアを配布していたと報じられています。
公開情報では、この偽リポジトリはプラットフォーム上で注目される状態に達していたとされています。
AI関連の公開リポジトリやモデル配布基盤が、正規プロジェクトを装う供給網型の悪用に使われうることを示しています。
利用者や運用側にとっては、信頼できる発行元の確認と導入前の検証が重要になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI/ML関連リポジトリでも、発行元・説明・公開履歴の整合性を確認する。
- 社内端末では不審な実行ファイルやスクリプトの持ち込みを制限し、EDRで異常挙動を監視する。
- 従業員に対して、人気順や見た目の正しさだけで取得・実行しないよう注意喚起する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ai_model_or_project | OpenAI | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Fake OpenAI repository on Hugging Face pushes infostealer malware](https://bleepingcomputer.com/news/security/fake-openai-repository-on-hugging-face-pushes-infostealer-malware) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 弱。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-29"></a>

### 4. Threats Making WAVs - Incident Response to a Cryptomining Attack

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>防御・運用</nobr> / <nobr>マルウェア</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Akamai Security Intelligenceは、WAVファイルの中に暗号資産マイナーを隠したとされる攻撃について、検知から感染、ネットワーク内での拡散、マルウェア解析までを整理した分析を公開しました。
あわせて、データセンターでのインシデント対応を改善するための示唆もまとめられています。音声ファイルのように一見安全に見える形式が悪用される可能性を示す事例として注目されます。
実運用環境での検知・封じ込め・調査の体制が十分かを見直す材料になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- WAVなど一般的なファイル形式でも不審な挙動があれば、内容だけでなく実行・展開時の監視を強化する。
- 感染後の横展開を想定し、セグメンテーションや権限管理、異常通信の検知を確認する。
- インシデント対応では初動の検知から封じ込め、証跡保全、復旧までの手順を定期的に点検する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Threats Making WAVs - Incident Response to a Cryptomining Attack](https://akamai.com/blog/security/threats-making-wavs-incident-reponse-cryptomining-attack) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 未評価。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [Unifi Accessにおけるリモートコード実行の脆弱性（CVE-2025-52665）](https://catchify.sa/post/cve-2025-52665-rce-in-unifi-os-25-000) | 28.0 | 46.0 | 50.0 |
| [Netskopeのクロステナント認証バイパスに関するセキュリティ情報](https://blog.amberwolf.com/blog/2025/august/advisory---netskope-cross-tenant-authentication-bypass) | 28.0 | 38.0 | 42.0 |
| [Nansh0uキャンペーン - ハッカーの武器庫がさらに強化される](https://akamai.com/blog/security/the-nansh0u-campaign-hackers-arsenal-grows-stronger) | 28.0 | 20.0 | 42.0 |
| [Oracle of Delphiが認証情報を窃取する](https://akamai.com/blog/security/the-oracle-of-delphi-steal-your-credentials) | 28.0 | 20.0 | 42.0 |
| [JDownloaderサイトが改ざんされ、インストーラーがPython RATマルウェアに差し替えられる](https://bleepingcomputer.com/news/security/jdownloader-site-hacked-to-replace-installers-with-python-rat-malware) | 28.0 | 20.0 | 42.0 |
| [AI生成画像の背景を透明化するのに役立つ画像背景削除ツール「Rembg」](https://gigazine.net/news/20260510-rembg) | 27.0 | 20.0 | 42.0 |
| [「執筆に生成AIを使った疑い」で大手出版社がホラー小説の出版を中止、この騒動が意味するAI執筆と出版の問題とは？](https://gigazine.net/news/20260509-horror-novel-pulled-ai-concerns) | 27.0 | 20.0 | 42.0 |
| [cPanelとWHMの3件の新たな脆弱性修正パッチ公開、今すぐ適用を](https://thehackernews.com/2026/05/cpanel-whm-patch-3-new-vulnerabilities.html) | 25.0 | 40.0 | 50.0 |
| [カメラの出っ張りゼロで背面フラットな「Google Pixel 10a」の写真撮影性能を検証するべくいろいろ撮影してきました](https://gigazine.net/news/20260509-google-pixel-10a-photo-example) | 25.0 | 20.0 | 43.0 |
| [Security: OpenAI Sora 2の内部解析 - マルチモーダルLLMを動かすシステムプロンプトの解明](https://mindgard.ai/resources/openai-sora-system-prompts) | 25.0 | 20.0 | 42.0 |
| [Must see: Geminiのハッキング - 多層的アプローチ](https://buganizer.cc/hacking-gemini-a-multi-layered-approach-md) | 25.0 | 20.0 | 42.0 |
| [Security: Citrix NetScalerのメモリリークと反射型XSS（CVE-2025-12101）](https://bit.ly/48bPzCO) | 23.0 | 34.0 | 50.0 |
| [GitHubだけで配布されているAndroid用アプリをF-Droidのようにインストールして管理＆自動更新できる「Obtainium」レビュー](https://gigazine.net/news/20260509-obtainium) | 23.0 | 20.0 | 42.0 |
| [MixMaster MMORPGのリバースエンジニアリングとセキュリティ分析](https://3r4y.github.io/posts/mixmasterreverseengineering) | 22.0 | 20.0 | 42.0 |
| [手持ちの小型扇風機みたいな見た目の折り畳み小型ドローン「DJI Flip」を飛ばして撮影性能を確かめてみた](https://gigazine.net/news/20260510-dji-flip-gravitate-osaka) | 22.0 | 20.0 | 42.0 |
| [茨木市の日本最長の歩行者専用つり橋で3眼カメラドローン「DJI Mavic 4 Pro」空撮レビューしてみた](https://gigazine.net/news/20260510-dji-mavic-4-pro-gravitate-osaka) | 22.0 | 20.0 | 42.0 |
| [人は「怒り」を感じると信頼性の低い情報源からのニュースを拡散しやすくなる](https://gigazine.net/news/20260510-anger-accelerates-misinformation-sharing) | 22.0 | 20.0 | 42.0 |
| [テスラのCybertruckがまたもやリコール、2024～2026年に販売された18インチスチールホイール装着モデルでホイール故障のリスクあり](https://gigazine.net/news/20260510-cybertruck-recall-tesla-rotor-cracks) | 22.0 | 20.0 | 42.0 |
| [砂漠のド真ん中に1週間だけの街を作り上げる「バーニングマン」は終了後に数週間かけてゴミ掃除をしている](https://gigazine.net/news/20260510-burning-man-moop) | 22.0 | 20.0 | 42.0 |
| [Duolingoの採用試験では「会場に着くまでのタクシー運転手への態度」が選考基準になっていた](https://gigazine.net/news/20260510-duoling-interview-test) | 22.0 | 20.0 | 42.0 |
| [「働くネコ」たちを写真とエピソードで記録した「Bodega Cats of New York」プロジェクト](https://gigazine.net/news/20260509-bodega-cats-of-new-york) | 22.0 | 20.0 | 42.0 |
| [Chromeの「オンデバイスAI」がGoogleサーバーにデータを送信していないという主張を削除](https://gigazine.net/news/20260509-chrome-on-device-ai) | 22.0 | 20.0 | 42.0 |
| [IntelがApple端末向けのチップの一部を製造することで両社が予備合意](https://gigazine.net/news/20260509-apple-intel-preliminary-chip-making-agreement) | 22.0 | 20.0 | 42.0 |
| [中国産ソシャゲ「NTE」をプレイしたマンガ家が思う「アニメ調オープンワールド大作」を日本が作らなくてもいい理由](https://itmedia.co.jp/news/articles/2605/10/news014.html) | 21.0 | 20.0 | 42.0 |

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
