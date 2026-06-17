# 📡 サイレーダー 2026-06-18 05:00 JST

このレポートは、2026-06-17 17:00 JST〜2026-06-18 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 104
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 72

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Microsoft working on patch for RoguePlanet Defender zero-day (CVE-2026-50656)](#topic-17871) | 53.0 | 58.0 | 55.0 | 音声 | 温度感上位枠 |
| 2 | [FreeBSoD: Leveraging Language Models to Find and Exploit Kernel Bugs (Part 1 of 2)](#topic-17867) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 3 | [The Top 10 Attack Surface Exposures in 2026](#topic-17948) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [CISA orders feds to patch max severity Joomla plugin flaw by Friday](#topic-17950) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [Microsoft working on Defender patch for RoguePlanet zero-day](#topic-17968) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [Crypto Clipper Campaign Abuses Fake Reviews, AI Narrators, and VirusTotal Comments](#topic-17869) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [North Korean Hiring Fraud Runs on AI and US Laptop Farms](#topic-17889) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-17871"></a>

### 1. Microsoft working on patch for RoguePlanet Defender zero-day (CVE-2026-50656)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 53.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

Microsoftは、Microsoft Defenderの脆弱性「RoguePlanet」に関連して、CVE-2026-50656として識別されたゼロデイ問題の修正パッチを準備していると公表しました。
報告では、これは権限昇格につながる脆弱性とされ、CVSS 7.8と評価されています。Defenderは広く利用されているため、修正前後の影響範囲が大きくなる可能性があります。
権限昇格に関わるため、侵害後の被害拡大や防御回避の足がかりになり得る点が注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Microsoftの修正提供状況と関連アドバイザリを継続確認し、適用可能になり次第速やかに展開する。
- Microsoft Defenderの保護機能が対象環境で最新状態かを確認し、更新遅延がないか点検する。
- 認証済みユーザー起点の不審な挙動や、Defender周辺の権限変化・異常なプロセス動作を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-50656 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-50656](https://nvd.nist.gov/vuln/detail/CVE-2026-50656) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Confirms RoguePlanet Defender Zero-Day, Says Patch is in Development](https://thehackernews.com/2026/06/microsoft-confirms-rogueplanet-defender_02022423645.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft working on patch for RoguePlanet Defender zero-day (CVE-2026-50656)](https://www.helpnetsecurity.com/2026/06/17/rogueplanet-zero-day-cve-2026-50656/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17867"></a>

### 2. FreeBSoD: Leveraging Language Models to Find and Exploit Kernel Bugs (Part 1 of 2)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

Praetorianの公開記事では、FreeBSDカーネルの脆弱性研究について、AIモデルを用いてバグの発見や検証を進めた取り組みが紹介されています。
関連するCVEとしてCVE-2026-3038が挙げられていますが、公開情報だけでは詳細な影響範囲や実際の被害状況は断定できません。
カーネル脆弱性は影響が大きく、権限昇格やシステム侵害につながる可能性があるため注目されます。加えて、AI支援の脆弱性研究が実運用レベルで進んでいる点も関心を集めます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- FreeBSDを利用する環境では、該当CVEの公表情報やベンダー案内を継続確認する。
- カーネル更新の適用状況を点検し、保守対象外の旧版が残っていないか確認する。
- AI支援の研究動向により新しい検出・検証手法が増える可能性があるため、脆弱性管理の優先度付けを見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-3038 | 主要CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-3038](https://nvd.nist.gov/vuln/detail/CVE-2026-3038) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [FreeBSoD: Leveraging Language Models to Find and Exploit Kernel Bugs (Part 1 of ](https://www.praetorian.com/blog/ai-vulnerability-research-freebsd-kernel/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17948"></a>

### 3. The Top 10 Attack Surface Exposures in 2026

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

公開情報では、侵害は必ずしもゼロデイから始まるわけではなく、公開された管理画面や再利用された認証情報のような露出した攻撃対象領域が起点になりうるとされています。
記事は、インターネット公開資産が脆弱性の発見後すぐに狙われやすい状況を背景に、2026年に注意すべき攻撃対象の露出を整理しています。
攻撃対象領域の見落としや認証情報の使い回しは、既知の脆弱性がなくても侵害につながるため、運用上の基本対策が改めて重要になります。
脆弱性の悪用までの時間が短くなる傾向が示唆されており、公開資産の把握と初動対応の速さが問われます。

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

- インターネット公開中の管理画面、API、リモート管理機能を棚卸しし、不要な公開を減らす。
- 認証情報の再利用を避け、多要素認証と権限最小化を徹底する。
- 外部公開資産の異常な認証失敗や不審なアクセスを継続監視し、脆弱性公開時の緊急点検手順を用意する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [The Top 10 Attack Surface Exposures in 2026](https://thehackernews.com/2026/06/the-top-10-attack-surface-exposures-in.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17950"></a>

### 4. CISA orders feds to patch max severity Joomla plugin flaw by Friday

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAが、Joomla向けのWidget Factory Joomla Content Editor（JCE）プラグインにある重大な脆弱性について、連邦機関に迅速な対応を求めました。
公開情報では、この問題は実際に悪用されているとされており、影響範囲のある環境では優先的な確認が必要です。
政府機関向けに期限付きで対応が求められていることから、緊急性の高い脆弱性として扱われています。公開情報で悪用が観測されている点も、放置時のリスクを高めます。

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

- Joomla環境でJCEプラグインを利用しているかを確認し、該当バージョンの有無を点検する。
- ベンダーや公的機関の案内に沿って、修正済みバージョンへの更新や暫定対策の適用を優先する。
- 外部公開された管理画面や不審な変更、ログ上の異常なアクセスがないかを確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA orders feds to patch max severity Joomla plugin flaw by Friday](https://www.bleepingcomputer.com/news/security/cisa-orders-feds-to-patch-max-severity-joomla-plugin-flaw-by-friday/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17968"></a>

### 5. Microsoft working on Defender patch for RoguePlanet zero-day

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Microsoft Defenderに関連するゼロデイ脆弱性「RoguePlanet」について、Microsoftが修正パッチの準備を進めていると報じられています。
公開情報では、すでに悪用に関する情報がある文脈で扱われており、早期の対応状況が注目されています。
セキュリティ製品そのものに関わる脆弱性は、端末防御の前提に影響するため注目度が高いです。ゼロデイかつ悪用情報があるとされる点から、組織の検知・緩和対応の優先度が上がります。

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

- Microsoftからの修正公開や追加の注意喚起が出ていないか継続確認する。
- Defender関連の保護状態、適用状況、例外設定を点検する。
- 関連アラートや不審な端末挙動がないか、監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft working on Defender patch for RoguePlanet zero-day](https://www.bleepingcomputer.com/news/microsoft/microsoft-working-on-defender-patch-for-rogueplanet-zero-day/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17869"></a>

### 6. Crypto Clipper Campaign Abuses Fake Reviews, AI Narrators, and VirusTotal Comments

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Check Point Researchの分析として、暗号資産を狙うクリッパー系のキャンペーンが、偽レビューやAIナレーター、VirusTotalのコメント欄など複数の公開プラットフォームを使って信頼性を装っていたとされています。
あわせて、WordPressのフィッシングページを中心に、GitHubやSourceForgeのプロジェクト、YouTubeなどを組み合わせて誘導していたと見られます。
正規サービスや公開サイトを悪用して見た目の信頼性を高めるため、利用者が不審さを見抜きにくい点が注意されます。
暗号資産関連の詐取は被害が直接的になりやすく、周辺の情報発信やレビューも含めた監視が重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 公開サイト上のレビュー、コメント、動画説明欄などを単独では信頼せず、相互に整合性を確認する。
- 暗号資産関連の配布物や案内ページは、提供元の実在性と関連ドメインの一貫性を確認する。
- GitHub、SourceForge、YouTubeなど複数面で誘導される場合は、リンク先と配布物の正当性を慎重に検証する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Crypto Clipper Campaign Abuses Fake Reviews, AI Narrators, and VirusTotal Commen](https://thehackernews.com/2026/06/crypto-clipper-campaign-abuses-fake.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-17889"></a>

### 7. North Korean Hiring Fraud Runs on AI and US Laptop Farms

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>国⁠家⁠支⁠援</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

北朝鮮に関係するとみられるIT人材のなりすまし・不正採用スキームについて、AIを使った面接対応と米国内のノートPC群が運用に使われていたと報じられています。
調査会社Nisosがこの活動グループに入り込み、実態の一端を確認したとされていますが、材料からは個別の被害規模までは断定できません。
採用プロセスを悪用した侵入は、通常のセキュリティ対策だけでは見落とされやすく、企業の委託・雇用管理にも影響します。
AIの利用で偽装の精度が上がると、本人確認や面接審査の見直しが必要になるため注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 採用時の本人確認を強化し、面接・契約・端末受領までの各段階で整合性を確認する。
- 遠隔就業者や委託先に対して、端末の所在・初期設定・アクセス元の不自然な偏りを監視する。
- 人事、法務、情シス、SOCで不正採用を含むインサイダー/第三者リスクの連携フローを確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [North Korean Hiring Fraud Runs on AI and US Laptop Farms](https://www.infosecurity-magazine.com/news/north-korea-it-worker-fraud-ai/) | <nobr>内容確認・補足情報</nobr> |

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
| [Microsoftが「RoguePlanet」ゼロデイの修正に対応中](https://www.securityweek.com/microsoft-working-on-patch-for-rogueplanet-zero-day/) | 37.0 | 38.0 | 42.0 |
| [Chinaを装ったローダーチェーンを通じてDropping Elephantの手口を追跡する](https://www.rapid7.com/blog/post/tr-malware-tracking-dropping-elephant-tradecraft-china-themed-loader-chain) | 35.0 | 20.0 | 42.0 |
| [悪意あるJetBrainsプラグインがAI APIキーを窃取し、Chrome拡張機能がチャットボットの会話を取得](https://thehackernews.com/2026/06/malicious-jetbrains-plugins-steal-ai.html) | 33.0 | 20.0 | 42.0 |
| [Microsoft Teams Relay Serversを悪用したDragonForceランサムウェア攻撃](https://www.securityweek.com/microsoft-teams-relay-servers-abused-in-dragonforce-ransomware-attack/) | 28.0 | 30.0 | 42.0 |
| [攻撃者がFortinetの4月公開の2件の重大な脆弱性を悪用](https://cyberscoop.com/fortinet-fortisandbox-vulnerabilities-exploits/) | 28.0 | 28.0 | 50.0 |
| [Rokarolla Androidマルウェアがスマートフォンを乗っ取り、銀行口座のログイン情報を窃取できる問題](https://www.malwarebytes.com/blog/mobile/2026/06/rokarolla-android-malware-can-take-over-your-phone-and-steal-banking-logins) | 28.0 | 20.0 | 42.0 |
| [Novo Nordisk侵害の数日後に別の医療企業が攻撃される](https://www.helpnetsecurity.com/2026/06/17/irhythm-data-breach-patient-health-information-stolen/) | 28.0 | 20.0 | 42.0 |
| [星評価からUpvoteへ：偽の評判が暗号資産クリップボードハイジャッカーを助長する](https://research.checkpoint.com/2026/from-stars-to-upvotes-fake-reputation-fueling-a-crypto-clipboard-hijacker/) | 28.0 | 20.0 | 42.0 |
| [Rokarolla Androidトロイの木馬、銀行および暗号資産ユーザーを標的に端末を乗っ取り可能に](https://www.helpnetsecurity.com/2026/06/17/rokarolla-android-banking-trojan-device-takeover/) | 28.0 | 20.0 | 42.0 |
| [MalwarebytesがAV-TESTのTop Product賞を獲得、その他の第三者テストでも高評価](https://www.malwarebytes.com/blog/product/2026/06/malwarebytes-earns-av-test-top-product-award-aces-other-third-party-tests) | 28.0 | 20.0 | 42.0 |
| [AIがサイバー攻撃を加速させる―その先を行くための対策](https://techcommunity.microsoft.com/blog/microsoft-entra-blog/ai-is-accelerating-cyberattacks%E2%80%94here%E2%80%99s-how-to-stay-ahead/4528592) | 27.0 | 20.0 | 42.0 |
| [低スキル攻撃者がClaudeとCodexを使って14社に侵入](https://www.helpnetsecurity.com/2026/06/17/ai-agents-offensive-cyber-operations-claude-codex/) | 25.0 | 20.0 | 42.0 |
| [LLM脅威に対するデジタル初動対応としてのマイクロセグメンテーション](https://www.akamai.com/blog/security/2026/jun/microsegmentation-digital-first-responder-llm-threats) | 25.0 | 20.0 | 42.0 |
| [AIではサイバーセキュリティ人材不足は解決できない](https://www.cybersecuritydive.com/news/cybersecurity-workforce-ai-skills-shortage/823143/) | 25.0 | 20.0 | 42.0 |
| [Tigera、KubernetesベースのAIエージェント向け統合制御プレーンを発表](https://www.helpnetsecurity.com/2026/06/17/tigera-lynx/) | 25.0 | 20.0 | 42.0 |
| [AIモデルへの機密エンタープライズデータアップロードが1年で倍増](https://www.infosecurity-magazine.com/news/sensitive-ai-data-upload-doubles/) | 25.0 | 20.0 | 42.0 |
| [FlipがデジタルID、ノーコードアプリ、AI自動化でプラットフォームを拡張](https://www.helpnetsecurity.com/2026/06/17/flip-frontline-identity-and-flip-fusion/) | 25.0 | 20.0 | 42.0 |
| [Corelight、Open NDRを強化してAI駆動の脅威と未知の資産を検出可能に](https://www.helpnetsecurity.com/2026/06/17/corelight-open-ndr-platform-expansion/) | 25.0 | 20.0 | 42.0 |
| [AI脅威とアラート疲労がサイバーセキュリティチームに与える課題](https://www.infosecurity-magazine.com/news/ai-threats-alert-fatigue-challenge/) | 25.0 | 20.0 | 42.0 |
| [ArmorCodeが製品メーカーのEUサイバーレジリエンス法要件対応を支援](https://www.helpnetsecurity.com/2026/06/17/armorcode-agentic-ai-platform-cra-capabilities/) | 25.0 | 20.0 | 42.0 |
| [Legit Security、AppSecの修復とリスク低減にagentic AIを導入](https://www.helpnetsecurity.com/2026/06/17/legit-security-remediation-agents/) | 25.0 | 20.0 | 42.0 |
| [Tenet Security、600万ドルのシード資金調達を発表](https://www.securityweek.com/tenet-security-emerges-from-stealth-with-6-million-seed-funding/) | 25.0 | 20.0 | 42.0 |
| [AIが普及してもSOCの最大課題は人員不足とSANSが指摘](https://www.infosecurity-magazine.com/news/staffing-top-soc-challenge-ai/) | 25.0 | 20.0 | 42.0 |
| [Cisco Webex Appのオープンリダイレクト脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-webex-app-redirect-KOyxhffH) | 24.0 | 46.0 | 50.0 |
| [Cisco Identity Services Engineのリモートコード実行および情報漏えいの脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-multi-G5WP8vv) | 24.0 | 46.0 | 50.0 |
| [ChromeとFirefoxがCriticalおよびHigh Severityの脆弱性を修正するために更新](https://www.securityweek.com/chrome-and-firefox-updated-to-patch-critical-high-severity-vulnerabilities/) | 24.0 | 38.0 | 42.0 |
| [Cisco Umbrella Virtual Applianceの権限昇格脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-umbrella-priv-esc-F4wJB7AU) | 22.0 | 40.0 | 50.0 |
| [ブラウザの見落とし: セキュリティツールが想定どおりにブロックできていない理由 [Guest Diary] (Wed, Jun 17th)](https://isc.sans.edu/diary/rss/33084) | 22.0 | 20.0 | 42.0 |
| [台車においた患者情報含む書類が所在不明に - 埼玉病院](https://www.security-next.com/185815) | 22.0 | 20.0 | 42.0 |
| [「Cortex XSOAR」「XSIAM」向け「CommvaultSecurityIQ」連携に脆弱性](https://www.security-next.com/186036) | 22.0 | 20.0 | 42.0 |
| [「ドットマネー」などにサイバー攻撃 - サービスが一時停止](https://www.security-next.com/185799) | 22.0 | 20.0 | 42.0 |
| [スポーツ教室当選者宛てメールで誤送信 - 取消機能で再発](https://www.security-next.com/186010) | 22.0 | 20.0 | 42.0 |
| [ホンダ・シビックに任意のコードを実行可能な脆弱性「EvilValet」が見つかる](https://gigazine.net/news/20260617-honda-civic-evil-valet/) | 22.0 | 20.0 | 42.0 |
| [バス会社サイトにDDoS攻撃 - 閲覧障害が発生](https://www.security-next.com/186008) | 22.0 | 20.0 | 42.0 |
| [サイバーエージェントのポイント交換サービス、不正アクセスで停止中 復旧に1カ月かかる見込み](https://www.itmedia.co.jp/news/articles/2606/17/news123.html) | 21.0 | 20.0 | 42.0 |
| [〇〇ペイの「送る」機能で支払わせる「偽通販サイト」にご用心 国民生活センターが注意喚起](https://www.itmedia.co.jp/news/articles/2606/17/news116.html) | 21.0 | 20.0 | 42.0 |
| [Cisco、最大深刻度の脆弱性告知にSD-WAN製品を追加](https://www.theregister.com/security/2026/06/17/cisco-adds-another-sd-wan-box-to-max-severity-bug-advisory/5257621) | 20.0 | 46.0 | 54.0 |
| [Cisco Crosswork Network Controllerのサーバーサイドテンプレートインジェクション脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-cnc-inj-QNMeEmxk) | 20.0 | 28.0 | 50.0 |
| [英国の重要インフラへの攻撃の4分の3は敵対国によるものとサイバー責任者が警告](https://therecord.media/britain-nation-state-cyberattacks-richard-horne-rusi) | 20.0 | 20.0 | 42.0 |
| [Fortinetファイアウォールを狙った大規模なパスワード窃取攻撃、7.5万台に被害](https://www.theregister.com/cyber-crime/2026/06/17/massive-password-stealing-attack-hits-75k-fortinet-firewalls/5257877) | 20.0 | 20.0 | 42.0 |
| [CISA暫定長官「重大な重要インフラ障害は避けられない」](https://www.cybersecuritydive.com/news/cybersecurity-resilience-critical-infrastructure-cisa-nick-andersen/823166/) | 20.0 | 20.0 | 42.0 |
| [EU、ウクライナに大規模攻撃対応のサイバーセキュリティ予備リソース利用を認可](https://therecord.media/ukraine-access-eu-cybersecurity-reserve) | 20.0 | 20.0 | 42.0 |
| [リモートアクセスツール悪用に対する検知の再考](https://redcanary.com/blog/security-operations/rmm-detection/) | 20.0 | 20.0 | 42.0 |
| [C2停止後もTailscaleとOpenSSHでアクセスを維持した若年ハッカー](https://thehackernews.com/2026/06/junior-hacker-used-tailscale-and.html) | 20.0 | 20.0 | 42.0 |
| [FortiBleed漏えいでFortinet VPN認証情報7万3000件が流出](https://www.bleepingcomputer.com/news/security/fortibleed-leak-exposes-fortinet-vpn-credentials-for-73-000-devices/) | 20.0 | 20.0 | 42.0 |
| [Iranと関連する攻撃者による侵害主張を受け、Californiaの水道事業者が調査を開始](https://www.cybersecuritydive.com/news/california-water-utility-breach-iran-hacker/823148/) | 20.0 | 20.0 | 42.0 |
| [デジタル主権には運用モデルが必要です](https://www.theregister.com/security/2026/06/17/digital-sovereignty-needs-an-operating-model/5254631) | 20.0 | 20.0 | 42.0 |
| [Adversarial Exposure Validationでセキュリティの可視性を確実な優先順位付けへ変える](https://thehackernews.com/2026/06/adversarial-exposure-validation-turns.html) | 20.0 | 20.0 | 42.0 |
| [Red Agent POVシリーズの紹介](https://www.wiz.io/blog/red-agent-pov-series) | 20.0 | 20.0 | 42.0 |
| [30,000台超のFortinetデバイスが侵害された大規模な認証情報収集攻撃](https://www.darkreading.com/cyberattacks-data-breaches/sweeping-credential-harvesting-heist-compromises-30k-fortinet-devices) | 20.0 | 20.0 | 42.0 |
| [アカウント乗っ取りが増加している理由とその防止策](https://www.bleepingcomputer.com/news/security/why-account-takeovers-are-rising-and-how-to-stop-them/) | 20.0 | 20.0 | 42.0 |
| [Keep Your Tech FLAME Alive: Trailblazer Katrina Cole](https://www.akamai.com/blog/culture/2026/jun/keep-your-tech-flame-alive-trailblazer-katrina-cole) | 20.0 | 20.0 | 42.0 |
| [SE LabsがSymantec Endpoint Securityを高評価、今年も受賞](https://www.security.com/feature-stories/se-labs-awards-2026) | 20.0 | 20.0 | 42.0 |
| [GitHub上のサーバーレス型フィッシングキットがメキシコの銀行を標的にする](https://www.infosecurity-magazine.com/news/gitbait-github-pages-sheetbest/) | 20.0 | 20.0 | 42.0 |
| [Homebrew 6.0リリース、新たなセキュリティ機構とLinuxサンドボックスを搭載](https://www.theregister.com/devops/2026/06/17/homebrew-60-released-with-new-security-mechanism-linux-sandbox-and-more/5257570) | 20.0 | 20.0 | 42.0 |
| [インドのTelegram禁止がUAEにも影響、回避方法は？](https://www.bleepingcomputer.com/news/security/indias-telegram-ban-hit-the-uae-too-heres-how-to-get-around-it/) | 20.0 | 20.0 | 42.0 |
| [1PasswordがAponoを買収、報道では2億5000万～3億ドル規模とされる取引](https://www.securityweek.com/1password-acquires-apono-in-reported-250m-300m-deal/) | 20.0 | 20.0 | 42.0 |
| [Tenable Oneが継続的なセキュリティ管理策の検証を追加し、リスク優先順位付けを改善](https://www.helpnetsecurity.com/2026/06/17/tenable-one-validation-capabilities/) | 20.0 | 20.0 | 42.0 |
| [NCSC CEO、英国の重要システムに影響するサイバー攻撃の4分の3が敵対国に関連と発表](https://www.ncsc.gov.uk/news/ncsc-ceo-hostile-states-linked-to-three-quarters-of-cyber-attacks) | 20.0 | 20.0 | 42.0 |
| [VelocityEHSがQRコードを活用してインシデント報告とリスク対応を迅速化](https://www.helpnetsecurity.com/2026/06/17/velocityehs-qr-codes-for-incident-management/) | 20.0 | 20.0 | 42.0 |
| [Rockwell Automation、ICSコントローラーおよびソフトウェアの脆弱性を修正](https://www.securityweek.com/rockwell-automation-patches-vulnerabilities-in-ics-controllers-and-software/) | 20.0 | 20.0 | 42.0 |
| [より迅速なトリアージ、明確な証拠、低リスク：SOCのためのより良いアラート対応ガイド](https://any.run/cybersecurity-blog/triage-analyst-guide/) | 20.0 | 20.0 | 42.0 |
| [240億件の盗難データが公開、今すぐすべきこと](https://www.malwarebytes.com/blog/news/2026/06/24-billion-stolen-records-found-in-giant-data-dump-check-if-youre-affected) | 20.0 | 20.0 | 42.0 |
| [Android 17の新機能：盗難対策、詐欺検知、ペアレンタルコントロール](https://www.helpnetsecurity.com/2026/06/17/android-17-security-and-privacy-features/) | 20.0 | 20.0 | 42.0 |
| [Helpdesk詐欺師が訪問してうそをより現実的に見せる手口](https://www.theregister.com/cyber-crime/2026/06/17/helpdesk-scammers-are-making-house-calls-to-make-their-lies-feel-more-real/5257454) | 20.0 | 20.0 | 42.0 |
| [Warner氏、CISAの人員削減と人員不足を警告する書簡を暫定長官に送付](https://therecord.media/warner-warns-of-cisa-cuts-staffing-shortages) | 20.0 | 20.0 | 42.0 |
| [EUのセキュリティ専門家、サイバー攻撃時にウクライナの組織を支援へ](https://www.infosecurity-magazine.com/news/ukraine-included-eu-cyber-reserve/) | 20.0 | 20.0 | 42.0 |
| [Chainguard Athena連合が500のオープンソースプロジェクトに2,000件のパッチを適用](https://www.helpnetsecurity.com/2026/06/17/chainguard-athena-coalition-fix-open-source-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [JetBrains Marketplaceの15件のプラグインでAPIキーを窃取する事例が発覚](https://www.infosecurity-magazine.com/news/fifteen-jetbrains-marketplace/) | 20.0 | 20.0 | 42.0 |
| [Oracleの2回目の月次セキュリティ更新で245件のパッチを提供](https://www.securityweek.com/oracles-second-monthly-security-updates-deliver-245-patches/) | 20.0 | 20.0 | 42.0 |
| [ウクライナは大規模攻撃時にEUのサイバー支援を受けられるように](https://www.helpnetsecurity.com/2026/06/17/ukraine-eu-cybersecurity-reserve-support/) | 20.0 | 20.0 | 42.0 |
| [Apple、Hide My EmailとSign in with Appleを1つのドメインに統合へ](https://www.helpnetsecurity.com/2026/06/17/apple-hide-my-email-domain-change/) | 20.0 | 20.0 | 42.0 |

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
