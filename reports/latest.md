# 📡 サイレーダー 2026-05-14 17:00 JST 試作版

このレポートは、2026-05-14 11:00 JST〜2026-05-14 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 87
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 74.0 | 82.0 | 81.0 | GitHub | 直近掲載済み・再掲抑制 |
| 2 | [Researcher Drops YellowKey, GreenPlasma Windows Zero-Days](#topic-4582) | 42.0 | 50.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](#topic-31) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Threats Making WAVs - Incident Response to a Cryptomining Attack](#topic-29) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-4582"></a>

### 1. Researcher Drops YellowKey, GreenPlasma Windows Zero-Days

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>Windows</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 42.0 |
| <nobr>実務影響</nobr> | 50.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Windows向けの2件のゼロデイ脆弱性として、YellowKeyとGreenPlasmaが報告されています。
公開情報によれば、YellowKeyはBitLockerの回避に関わり物理アクセスが必要とされ、GreenPlasmaは権限昇格によりSYSTEM権限を得られるとされています。
BitLocker回避とSYSTEM権限への昇格は、端末の保護や管理権限に直接影響しうるため注目されています。
ゼロデイとして扱われている点から、影響範囲の確認と対応状況の把握が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Windows端末のBitLocker設定と物理アクセス管理を再点検する。
- 権限昇格につながる挙動がないか、端末監視やEDRの検知ルールを確認する。
- 該当情報のベンダー対応や修正状況を追跡し、優先度をつけて適用計画を立てる。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Researcher Drops YellowKey, GreenPlasma Windows Zero-Days](https://securityweek.com/researcher-drops-yellowkey-greenplasma-windows-zero-days) | <nobr>内容確認・補足情報</nobr> |

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

<a id="topic-31"></a>

### 2. PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>防御・運用</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Guardicore Labsの分析によると、MySQLサーバーを狙うランサムウェア関連の攻撃キャンペーンが確認されています。
攻撃者は二重の脅迫を用い、盗んだとされるデータを公開して被害組織に圧力をかける手口が示されています。
MySQLは多くのシステムで基盤となるため、影響を受けると業務やデータ保全への波及が大きくなり得ます。
公開情報として脅迫型のランサムウェア活動が示されているため、監視と防御の優先度を再確認する材料になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- MySQLのインターネット公開状況、認証設定、不要な外部接続の有無を見直す。
- バックアップの隔離、復旧手順の確認、重要データの暗号化・権限管理を点検する。
- 異常な接続、認証失敗の増加、データ転送の兆候など、侵入や持ち出しを示すログ監視を強化する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](https://akamai.com/blog/security/please-read-me-opportunistic-ransomware-devastating-mysql-servers) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-29"></a>

### 3. Threats Making WAVs - Incident Response to a Cryptomining Attack

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>防御・運用</nobr> / <nobr>マルウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Akamai Security Intelligence は、WAVファイルの中に暗号資産マイナーを隠したとされる攻撃について、検知から感染、横展開、解析までをまとめた事例を紹介しています。
公開された内容では、データセンター環境でのインシデント対応を改善する観点も示されています。
音声ファイルのような一見無害な形式が悪用される可能性があるため、受け取り側の警戒が必要です。
暗号資産マイニングは直接的な情報窃取でなくても、計算資源の消費や運用影響につながる点が注目されます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 不審なファイル形式や配布経路を前提にせず、受領ファイルの検査と隔離を徹底する。
- 端末やサーバーのCPU・GPU使用率、常駐プロセス、通信の異常を監視し、マイニング兆候を早期に把握する。
- インシデント対応手順を見直し、感染確認後の封じ込めと横展開防止の連絡・復旧フローを整理する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Threats Making WAVs - Incident Response to a Cryptomining Attack](https://akamai.com/blog/security/threats-making-wavs-incident-reponse-cryptomining-attack) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

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

CVE-2025-60710 は、Microsoft Windows の Taskhost 関連機能におけるローカル権限昇格の脆弱性として扱われています。
CISA の Known Exploited Vulnerabilities に含まれており、公開PoCや検証コードの言及もあるため、優先的な確認対象とみられます。
権限昇格系の脆弱性は、端末内での被害拡大や管理者権限の取得につながる可能性があるため、影響が大きくなりやすいです。
さらに、実際の悪用が確認されている扱いであることから、通常の脆弱性よりも早い対応が求められます。

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

- Windows 端末の適用状況を確認し、CVE-2025-60710 の修正有無を把握する。
- 特権アカウントの利用状況や、想定外の権限昇格の痕跡がないかを点検する。
- 公開PoCの存在を踏まえ、関連端末の監視を強め、優先度を上げて対応する。

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

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。
- 継続観測: 継続。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [Unifi Accessにおけるリモートコード実行（CVE-2025-52665）](https://catchify.sa/post/cve-2025-52665-rce-in-unifi-os-25-000) | 28.0 | 46.0 | 50.0 |
| [NGINX Rewrite Module の18年前からの脆弱性により認証不要のRCEが可能に](https://thehackernews.com/2026/05/18-year-old-nginx-rewrite-module-flaw.html) | 28.0 | 46.0 | 50.0 |
| [Netskopeのクロステナント認証バイパスに関するセキュリティ情報](https://blog.amberwolf.com/blog/2025/august/advisory---netskope-cross-tenant-authentication-bypass) | 28.0 | 38.0 | 42.0 |
| [Oracle of Delphiが認証情報を窃取する](https://akamai.com/blog/security/the-oracle-of-delphi-steal-your-credentials) | 28.0 | 20.0 | 42.0 |
| [Nansh0uキャンペーン―ハッカーの武器庫がさらに強化される](https://akamai.com/blog/security/the-nansh0u-campaign-hackers-arsenal-grows-stronger) | 28.0 | 20.0 | 42.0 |
| [Anthropicがビジネス分析・広告キャンペーン・簿記などの自動化ができる「Claude for Small Business」をリリース](https://gigazine.net/news/20260514-claude-for-small-business) | 27.0 | 20.0 | 42.0 |
| [AnthropicがClaude Agent SDKクレジットを発表、OpenClawなどのサードパーティー自律型AIエージェントハーネスを再び稼働させることができるように](https://gigazine.net/news/20260514-anthropic-claude-agent-sdk-credits) | 27.0 | 20.0 | 42.0 |
| [Meta AIとの「真のプライバシー保護」を実現した完全プライベートな会話を可能にする「Incognito Chat」が登場](https://gigazine.net/news/20260514-meta-ai-incognito-chat) | 27.0 | 20.0 | 42.0 |
| [EY、新サービス「AIレッドチーミング」提供開始、生成AIのセキュリティリスクを可視化](https://news.mynavi.jp/techplus/article/20260514-4458902) | 26.0 | 20.0 | 42.0 |
| [生成AI利用者の約3割がヒヤリハットを経験--サイバーセキュリティクラウド調査](https://japan.zdnet.com/article/35247508) | 26.0 | 20.0 | 42.0 |
| [FragnesiaのLinux脆弱性により攻撃者がroot権限を取得可能に](https://bleepingcomputer.com/news/security/new-fragnesia-linux-flaw-lets-attackers-gain-root-privileges) | 25.0 | 40.0 | 50.0 |
| [OpenAI Sora 2のセキュリティ：マルチモーダルLLMを駆動するシステムプロンプトの解析](https://mindgard.ai/resources/openai-sora-system-prompts) | 25.0 | 20.0 | 42.0 |
| [必見: Geminiをハッキングする多層的アプローチ](https://buganizer.cc/hacking-gemini-a-multi-layered-approach-md) | 25.0 | 20.0 | 42.0 |
| [ベクトル埋め込みのセキュリティギャップが企業AIパイプラインを露呈させる](https://helpnetsecurity.com/2026/05/14/vectorsmuggle-vector-embedding-security) | 25.0 | 20.0 | 42.0 |
| [企業におけるAIガバナンスのギャップを埋めるには](https://helpnetsecurity.com/2026/05/14/ai-governance-gap-video) | 25.0 | 20.0 | 42.0 |
| [くら寿司、万博店を再現した“メモリアル店“オープン 回転ベルトなど移設、世界70カ国の料理も](https://itmedia.co.jp/news/articles/2605/14/news084.html) | 24.0 | 20.0 | 43.0 |
| [Citrix NetScalerのメモリリークと反射型XSS（CVE-2025-12101）](https://bit.ly/48bPzCO) | 23.0 | 34.0 | 50.0 |
| [MixMaster MMORPGの逆アセンブルと解析](https://3r4y.github.io/posts/mixmasterreverseengineering) | 22.0 | 20.0 | 42.0 |
| [「あなたの忍者に関する知識はすべて間違っている」と題した動画を海外で人気の科学系YouTubeチャンネルKurzgesagtが公開](https://gigazine.net/news/20260514-ninja-image) | 22.0 | 20.0 | 42.0 |
| [ジャンボジェット機相当サイズのソーラードローンが自律型海上哨戒飛行の記録を更新して着水＆沈没](https://gigazine.net/news/20260514-solar-drone-jumbo-jet-wingspan-broke-record-crashed) | 22.0 | 20.0 | 42.0 |
| [ウェブサーバ「nginx」に複数脆弱性 - 「クリティカル」も](https://security-next.com/184434) | 22.0 | 20.0 | 42.0 |
| [Outlookの迷惑メールフォルダにおけるリンクプレビュー機能の簡単な回避方法](https://isc.sans.edu/diary/rss/32990) | 22.0 | 20.0 | 42.0 |
| [Gemini向けノートPC「Googlebook」の登場によってChromebookはどうなるのか？](https://gigazine.net/news/20260514-googlebooks-premium-focus) | 22.0 | 20.0 | 42.0 |
| [メモリの価格高騰がメモリの購入者であるAppleにとってむしろ有利に働く理由](https://gigazine.net/news/20260514-apple-memory-panic) | 22.0 | 20.0 | 42.0 |

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
