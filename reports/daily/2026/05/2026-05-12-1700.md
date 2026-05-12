# 📡 サイレーダー 2026-05-12 17:01 JST 試作版

このレポートは、2026-05-12 11:00 JST〜2026-05-12 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 83
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 74.0 | 82.0 | 81.0 | 音声 | 温度感上位枠 |
| 2 | [PLEASE_READ_ME: The Opportunistic Ransomware Devastating MySQL Servers](#topic-31) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [大友克洋がアニメ制作スタジオ「OVAL GEAR animation studio」を設立して新作アニメ制作を開始](#topic-3374) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Threats Making WAVs - Incident Response to a Cryptomining Attack](#topic-29) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [毎週数百万回ダウンロードされる人気JavaScriptライブラリ群「TanStack」にサプライチェーン攻撃、問題のあるバージョンをインストールした開発環境では認証情報流出の恐れ](#topic-3344) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-12"></a>

### 1. Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>Windows</nobr> / <nobr>権限昇格</nobr> / <nobr>TTP</nobr> / <nobr>脆弱性</nobr> / <nobr>KEV</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 74.0 |
| <nobr>実務影響</nobr> | 82.0 |
| <nobr>確度</nobr> | 81.0 |

#### 概要

CVE-2025-60710は、Microsoft WindowsのTaskhost関連のタスク処理におけるローカル権限昇格の脆弱性として扱われています。
CISAのKnown Exploited Vulnerabilitiesに掲載されており、公開PoCや検証コードの言及もあるため、影響確認の優先度が高いとみられます。
権限昇格は、侵入後の被害拡大や管理者権限の取得につながるため、実運用への影響が大きい分野です。
さらに、KEV掲載と公開PoCの示唆があることで、放置するとリスクが高まりやすい点が注目されています。

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

- 影響を受けるWindows環境で、CVE-2025-60710の修正適用状況を確認する。
- Taskhostや関連タスクの異常な動作・権限変化がないか、監視とログ確認を強化する。
- 公開PoCの存在を踏まえ、優先度を上げて脆弱性管理と資産棚卸しを見直す。

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
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>防御・運用</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Akamai Security Intelligenceは、MySQLサーバーを狙うランサムウェア関連のキャンペーンを報告しています。
攻撃者は二重の脅迫手法を用い、窃取したとみられるデータを公開して被害組織に圧力をかけるとされています。
データベースサーバーは業務への影響が大きく、侵害されると情報漏えいと停止被害の両方につながり得ます。
ランサムウェアの典型的な脅し方に加え、公開を伴う圧力が示されている点が注目されます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- MySQLサーバーの露出状況、認証設定、不要な公開ポートを確認する。
- バックアップの隔離保管と復元手順を点検し、復旧可能性を定期的に検証する。
- 監査ログや不審な接続・権限変更の検知を強化し、データ流出の兆候も含めて監視する。

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

<a id="topic-3374"></a>

### 3. 大友克洋がアニメ制作スタジオ「OVAL GEAR animation studio」を設立して新作アニメ制作を開始

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

大友克洋氏がアニメ制作スタジオ「OVAL GEAR animation studio」を設立し、新作アニメの制作を開始したと伝えられています。
あわせて、同スタジオではアニメーターや制作スタッフの募集も行われているとのことです。著名クリエイターの新たな制作体制の発表であり、今後の作品展開に関心が集まりやすい話題です。
サイバーセキュリティ上の直接的な影響は示されていませんが、広く注目されるニュースとして把握しておく価値があります。

#### 温度感の理由

##### 温度感
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 現時点ではセキュリティ上の脅威情報ではないため、通常の監視対象と切り分けて扱う。
- 関連報道や公式発表が増える可能性があるため、誤情報やなりすまし投稿の有無は確認する。
- 採用募集を装った不審連絡が出る可能性があるため、問い合わせ先は公式情報で確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ransomware_group | Akira | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [大友克洋がアニメ制作スタジオ「OVAL GEAR animation studio」を設立して新作アニメ制作を開始](https://gigazine.net/news/20260512-katsuhiro-ohtomo-oval-gear-animation-studio) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 未評価。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-29"></a>

### 4. Threats Making WAVs - Incident Response to a Cryptomining Attack

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

Akamai Security Intelligenceが、WAVファイルの中に仮想通貨マイナーを隠したとされる攻撃事案の分析結果を公表しました。
報告では、検知、感染、ネットワーク内での拡散、マルウェア解析までの流れが整理され、インシデント対応の改善点も示されています。
音声ファイルのように一見無害に見える形式が悪用されると、従来の確認だけでは見落としにつながる可能性があります。
データセンター環境での侵害対応や、暗号資産マイニングを伴う不正利用への備えを見直す材料になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- WAVなどの一般的なファイル形式であっても、受信・配置・実行の各段階で想定外の挙動がないか確認する。
- 暗号資産マイニング由来のCPU/GPU負荷、未知のプロセス、横展開の兆候を監視対象に含める。
- インシデント対応では、初動の隔離、影響範囲の特定、再侵入防止までを手順化しておく。

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

<a id="topic-3344"></a>

### 5. 毎週数百万回ダウンロードされる人気JavaScriptライブラリ群「TanStack」にサプライチェーン攻撃、問題のあるバージョンをインストールした開発環境では認証情報流出の恐れ

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>マルウェア</nobr> / <nobr>サプライチェーン</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

人気JavaScriptライブラリ群「TanStack」のnpmパッケージに対し、マルウェアを含むバージョンが公開されるサプライチェーン攻撃があったと報じられています。
公式の事後報告によると、複数の関連パッケージに不正なコードが混入したとされ、問題のある版を導入した開発環境では認証情報流出の恐れがあります。
TanStackは多くの開発現場で使われているため、影響がライブラリ利用者全体に広がる可能性があります。
依存関係の汚染は、直接の脆弱性がなくても開発環境やビルド工程に被害が及ぶ点で注意が必要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 依存パッケージのバージョンを確認し、問題のある公開期間に入ったものを使っていないか点検する。
- 開発端末やCI/CDで使った認証情報、トークン、秘密情報の扱いを見直し、必要に応じてローテーションする。
- パッケージ管理の監査ログやビルド履歴を確認し、不審な更新や自動取得がないかを把握する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [毎週数百万回ダウンロードされる人気JavaScriptライブラリ群「TanStack」にサプライチェーン攻撃、問題のあるバージョンをインストールした開発環境では](https://gigazine.net/news/20260512-tanstack-supply-chain-attack) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 未評価。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 未評価。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 弱。
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
| [ランサム攻撃で個人情報3万件流出か 貿易貨物の検査機関・新日本検定協会](https://itmedia.co.jp/news/articles/2605/12/news104.html) | 29.0 | 30.0 | 42.0 |
| [UniFi Access のリモートコード実行（CVE-2025-52665）](https://catchify.sa/post/cve-2025-52665-rce-in-unifi-os-25-000) | 28.0 | 46.0 | 50.0 |
| [Netskopeにおけるクロステナント認証バイパスの脆弱性](https://blog.amberwolf.com/blog/2025/august/advisory---netskope-cross-tenant-authentication-bypass) | 28.0 | 38.0 | 42.0 |
| [2026年のランサムウェアの現状](https://securelist.com/state-of-ransomware-in-2026/119761) | 28.0 | 30.0 | 42.0 |
| [The Oracle of Delphiが認証情報を窃取する](https://akamai.com/blog/security/the-oracle-of-delphi-steal-your-credentials) | 28.0 | 20.0 | 42.0 |
| [Nansh0uキャンペーン―ハッカーの武器庫がさらに強化](https://akamai.com/blog/security/the-nansh0u-campaign-hackers-arsenal-grows-stronger) | 28.0 | 20.0 | 42.0 |
| [OCR・音声・構造化出力などの定型タスクに特化したAIモデル「Interfaze」登場](https://gigazine.net/news/20260512-interfaze-new-model-architecture) | 27.0 | 20.0 | 42.0 |
| [GitLabがAIエージェント時代へ向け大規模再編、人員削減や管理階層の削減を計画](https://gigazine.net/news/20260512-gitlab-act-2) | 27.0 | 20.0 | 42.0 |
| [OpenAIが企業のAI導入を助ける新会社「OpenAI Deployment Company」を設立](https://gigazine.net/news/20260512-openai-deployment-company) | 27.0 | 20.0 | 42.0 |
| [Z世代の新入社員、研修の切り札はAI パソコン相手に接客特訓、システム開発 リスクは](https://itmedia.co.jp/news/articles/2605/12/news111.html) | 26.0 | 20.0 | 42.0 |
| [OpenAI Sora 2のセキュリティ内部分析：マルチモーダルLLMを動かすシステムプロンプトの解明](https://mindgard.ai/resources/openai-sora-system-prompts) | 25.0 | 20.0 | 42.0 |
| [Must see: Geminiをハックする - 多層的アプローチ](https://buganizer.cc/hacking-gemini-a-multi-layered-approach-md) | 25.0 | 20.0 | 42.0 |
| [OpenAI、AIを活用した脆弱性検出とパッチ検証のDaybreakを発表](https://thehackernews.com/2026/05/openai-launches-daybreak-for-ai-powered.html) | 25.0 | 20.0 | 42.0 |
| [Security: Citrix NetScalerのメモリリークと反射型XSS（CVE-2025-12101）](https://bit.ly/48bPzCO) | 23.0 | 34.0 | 50.0 |
| [MixMaster MMORPGのリバースエンジニアリングにおけるセキュリティ分析](https://3r4y.github.io/posts/mixmasterreverseengineering) | 22.0 | 20.0 | 42.0 |
| [90日間の脆弱性開示ポリシーはもはや意味をなさないという指摘、AIがバグ発見とエクスプロイト開発を爆速に](https://gigazine.net/news/20260512-disclosure-policy-dead) | 22.0 | 20.0 | 42.0 |
| [Google検索が落ちて検索不能になる事態が発生](https://gigazine.net/news/20260512-google-search) | 22.0 | 20.0 | 42.0 |
| [「SandboxJS」にサンドボックス回避のRCE脆弱性](https://security-next.com/184296) | 22.0 | 20.0 | 42.0 |
| [「Exim」に複数脆弱性 - 「クリティカル」との評価も](https://security-next.com/184302) | 22.0 | 20.0 | 42.0 |
| [あらゆるトレカの中で最も偽造された数が多かったのは「リザードン」、TCG鑑定会社のPSAが2025年のレポートを公開](https://gigazine.net/news/20260512-tcg-fake) | 22.0 | 20.0 | 42.0 |
| [複数のClaude Codeを1画面で管理できる公式機能「agent view」が登場＆Claudeの全機能がAWS経由で使用可能に](https://gigazine.net/news/20260512-claude-code-agent-view-aws) | 22.0 | 20.0 | 42.0 |
| [AIの入出力を既存のターン制からリアルタイムに変えるAI「Interaction Models」をOpenAIの元CTOが新設したThinking Machines Labが研究プレビューを発表](https://gigazine.net/news/20260512-thinking-machines-lab-interaction-models) | 22.0 | 20.0 | 42.0 |
| [サイバー犯罪グループがAIを使って2要素認証を回避できるゼロデイ脆弱性を発見していたとGoogleが報告](https://gigazine.net/news/20260512-hacker-use-ai-mass-exploitation-google) | 22.0 | 20.0 | 42.0 |
| [「Netflixがユーザーの同意なく情報を収集するスパイ行為をした」とテキサス州が提訴](https://gigazine.net/news/20260512-texas-sues-netflix-for-spying) | 22.0 | 20.0 | 42.0 |

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
