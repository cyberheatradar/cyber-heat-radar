# 📡 サイレーダー 2026-09-30 11:00 JST

このレポートは、2026-09-30 05:00 JST〜2026-09-30 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 64
- [音声で扱う想定のトピック](#audio-topics): 4
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 35

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks](#topic-216) | 72.0 | 99.0 | 92.0 | 音声 | AI×Security枠 |
| 2 | [Apple Zero-Day Vulnerability Weaponized in Targeted Attacks](#topic-34785) | 45.0 | 46.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [Custom ChatGPTs push ClickFix attacks to deploy RAT malware](#topic-35111) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 4 | [Phishing Abuses RMM Tools for Persistent Access](#topic-35101) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-216"></a>

### 1. CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 72.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 99.0 |
| <nobr>確⁠度</nobr> | 92.0 |

#### 概要

cPanel & WHMに関する認証回避の脆弱性「CVE-2026-41940」について、実際の悪用事例やランサムウェア攻撃との関連が報告されています。
公開PoCや検証コードへの言及もあり、サーバー管理基盤を狙う攻撃として注目されています。
cPanel & WHMはホスティング環境で広く使われるため、影響を受けると複数のサイトや顧客環境に波及するおそれがあります。
認証を回避される性質上、放置すると侵害の初動を許しやすく、優先的な確認が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 12 sources。
- CISA KEV関連。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- cPanel & WHMの利用有無と対象バージョンを確認し、ベンダーの修正情報を適用する。
- 管理画面や関連アカウントの不審なログイン履歴、設定変更、追加されたユーザーやキーの有無を点検する。
- ホスティング基盤や関連サーバーで、認証周辺の異常・不審な通信・侵入後の持続化の兆候を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-40473 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-41940 | 関連CVE | 1.00 | 候補あり（URL 40件以上） |
| 脆弱性 | CVE-2026-42208 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-76460 | 関連CVE | 1.00 | 未確認 |
| ベンダー | cPanel | 言及あり | 0.80 | — |
| 製品 | WHM | 言及あり | 0.80 | — |
| 製品 | cPanel | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-41940](https://nvd.nist.gov/vuln/detail/CVE-2026-41940) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Weekly Report: Acronis Backup plugin for cPanel & WHMに権限昇格の脆弱性](https://www.jpcert.or.jp/wr/2026/wr260930.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Ransomware incidents in Japan in the first half of 2026: Investigation of The Ge](https://blog.talosintelligence.com/ransomware-incidents-in-japan-in-the-first-half-of-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Large-Scale GitHub Actions Abuse Powers a Distributed cPanel and WHM Exploitatio](https://socket.dev/blog/github-actions-abuse-powers-cpanel-and-whm-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [What’s New in Rapid7 Products and Services: Q2 2026 in Review](https://www.rapid7.com/blog/post/pt-new-products-services-q2-2026-mdr) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Weekly Report: Apache Camelに複数の脆弱性](https://www.jpcert.or.jp/wr/2026/wr260513.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Stealthy hackers exploit cPanel flaw in active backdoor campaign (CVE-2026-41940](https://www.helpnetsecurity.com/2026/05/12/cpanel-vulnerability-exploited-backdoor-cve-2026-41940/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [cPanel CVE-2026-41940 Under Active Exploitation to Deploy Filemanager Backdoor](https://thehackernews.com/2026/05/cpanel-cve-2026-41940-under-active.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 採用あり（1件）。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-34785"></a>

### 2. Apple Zero-Day Vulnerability Weaponized in Targeted Attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>i⁠O⁠S</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Appleは、iOSやmacOSの複数の旧バージョン向けにセキュリティ修正を含む更新を公開し、CVE-2026-86950を修正しました。
報道によると、この脆弱性は標的型攻撃で悪用されていたとされ、Appleも特定の個人を狙った非常に高度な攻撃に使われた可能性を認めています。
ゼロデイとして悪用が確認・示唆される脆弱性は、一般ユーザーよりも特定組織や高リスク端末への影響が先に広がるおそれがあります。
対象バージョンが限られていても、更新の優先度は高い事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
- 実悪用・ゼロデイ文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- iOS/macOSの該当する旧バージョンを使っている端末は、優先して最新の修正版へ更新する。
- Appleが言及している通り、標的型攻撃の文脈があるため、端末の不審なファイル受信や外部共有を含む周辺の監視を強める。
- 資産棚卸しでApple端末のOSバージョンを確認し、更新漏れ端末が残っていないかを点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-86950 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Apple | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Apple iOS | 言及あり | 0.80 | — |
| ベンダー | Meta | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-86950](https://nvd.nist.gov/vuln/detail/CVE-2026-86950) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Apple Zero-Day Vulnerability Weaponized in Targeted Attacks](https://www.darkreading.com/cyberattacks-data-breaches/apple-zero-day-vulnerability-weaponized-targeted-attacks) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple patches CoreGraphics zero-day already exploited in targeted attacks](https://www.theregister.com/security/2026/09/29/apple-patches-coregraphics-zero-day-already-exploited-in-targeted-attacks/5299721) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Update your iPhone, iPad, or Mac: Flaw could run attackers’ code](https://www.malwarebytes.com/blog/bugs/2026/09/update-your-iphone-ipad-or-mac-flaw-could-run-attackers-code) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple squashes zero-day bug exploited in “extremely sophisticated” attack (CVE-2](https://www.helpnetsecurity.com/2026/09/29/apple-core-graphics-zero-day-cve-2026-86950-fixed/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Patches Zero-Day Linked to ‘Extremely Sophisticated Attack’](https://www.securityweek.com/apple-patches-meta-reported-zero-day-linked-to-extremely-sophisticated-attack/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Emergency Patch for iOS 26, macOS26, macOS15 (CVE-2026-86950), (Mon, Sep 2](https://isc.sans.edu/diary/rss/33376) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-35111"></a>

### 3. Custom ChatGPTs push ClickFix attacks to deploy RAT malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、OpenAIのChatGPTを装ったカスタム版がスポンサー広告経由で案内され、利用者を不審なサイトへ誘導する事例が報告されています。
誘導先ではClickFix型の手口が使われ、最終的にRATマルウェアの配布につながるとされています。
生成AI関連の見た目や名称を悪用して、正規サービスに見せかけた誘導が行われる点が注意材料です。検索広告やAIサービス利用時の信頼性確認が、従来以上に重要になっています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- スポンサー広告経由の遷移先を含め、AI関連サービス名をうたうページの正当性を確認する。
- 利用者向けに、Web上での不自然な操作要求や手動入力を促す画面への警戒を周知する。
- エンドポイントやメール、Webプロキシで不審なダウンロードや不審サイトへのアクセスを監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | ChatGPT | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Custom ChatGPTs push ClickFix attacks to deploy RAT malware](https://www.bleepingcomputer.com/news/security/custom-chatgpts-push-clickfix-attacks-to-deploy-rat-malware/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35101"></a>

### 4. Phishing Abuses RMM Tools for Persistent Access

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftは、フィッシング攻撃でRMM（リモート監視・管理）ツールが悪用され、MSP360経由でScreenConnectが展開される事例を観測したとしています。
これにより、攻撃者が後続活動のための遠隔操作手段を複数確保していた可能性が示されています。
正規の管理ツールが悪用されると、検知や遮断が難しくなり、侵害後の滞在期間が長引くおそれがあります。
遠隔管理系ツールの利用実態と、想定外の導入・接続を継続監視する重要性を示す事例です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- RMMツールや遠隔操作ツールの導入・更新・接続先を棚卸しし、未承認の利用がないか確認する。
- フィッシング起点の侵入を想定し、メール経由の初期侵入対策と多要素認証、権限管理を強化する。
- 正規ツールに見える通信でも、異常な認証失敗・新規端末・不審な永続化の兆候を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | ConnectWise | 言及あり | 0.80 | — |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Amazon Web Services | 言及あり | 0.80 | — |
| ベンダー | GitLab | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Adobe | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |
| 製品 | ConnectWise ScreenConnect | 言及あり | 0.80 | — |
| 製品 | Adobe Acrobat | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Phishing Abuses RMM Tools for Persistent Access](https://www.microsoft.com/en-us/security/blog/2026/09/29/phishing-abuses-rmm-tools-persistent-access/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

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
| [佐賀大学のNASにランサムウェア攻撃、ファイルが暗号化される被害](https://scan.netsecurity.ne.jp/article/2026/09/30/56346.html) | 29.0 | 30.0 | 42.0 |
| [京王電鉄にランサムウェア攻撃](https://scan.netsecurity.ne.jp/article/2026/09/30/56345.html) | 29.0 | 30.0 | 42.0 |
| [ランサムウェア被害件数が過去最多の123件に、警察庁が対策情報を紹介](https://scan.netsecurity.ne.jp/article/2026/09/30/56339.html) | 29.0 | 30.0 | 42.0 |
| [ランサム攻撃者の侵入経路に異変](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/041800012/091400342/) | 29.0 | 30.0 | 42.0 |
| [OpenAI、豪政府サイトへの不正アクセスで謝罪 最先端AI学習の安全指針も公開](https://www.itmedia.co.jp/news/article/2609/30/2000001869/) | 28.0 | 20.0 | 42.0 |
| [「AIによる人間支配」の危機を検証](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/040900481/092400038/) | 28.0 | 20.0 | 42.0 |
| [Russian hackers Star Blizzardがウクライナとその先を狙い、標的拡大と戦術変更](https://cyberscoop.com/microsoft-star-blizzard-redflick-phishing-campaigns/) | 28.0 | 20.0 | 42.0 |
| [OpenAI、常時稼働型エージェント「Dots」を発表--慎重にすべき理由](https://japan.zdnet.com/article/35253086/) | 26.0 | 20.0 | 42.0 |
| [AI企業トップらと昼食会のトランプ米大統領、政府内で「AI」を「SI」と呼び替える大統領令に署名](https://www.itmedia.co.jp/news/article/2609/30/2000001871/) | 26.0 | 20.0 | 42.0 |
| [AI コーディングやローコード開発の落とし穴を解説 ～ GMOイエラエ、10 / 6 に Web アプリ脆弱性診断のオンラインセミナー開催](https://scan.netsecurity.ne.jp/article/2026/09/30/56347.html) | 26.0 | 20.0 | 42.0 |
| [GMOイエラエ、AI 活用で最短 3 営業日納品の「クイック診断」など Webアプリ脆弱性診断 3 プランを提供開始](https://scan.netsecurity.ne.jp/article/2026/09/30/56336.html) | 26.0 | 20.0 | 42.0 |
| [AIで購入商品を提案 成約率を1.5倍に](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/092400572/092400002/) | 26.0 | 20.0 | 42.0 |
| [シャドーAIへの機密流出をブロック Microsoftがセキュリティ製品群をアップデート](https://www.itmedia.co.jp/enterprise/articles/2609/29/news035.html) | 26.0 | 20.0 | 42.0 |
| [Google、日本オフィスの設立25周年を記念し、特設サイトとブランドムービーを公開 AI活用のアイデアを表彰する「Google AI Challenge」も開催](https://internet.watch.impress.co.jp/docs/news/2144208.html) | 25.0 | 20.0 | 42.0 |
| [AIの悪夢に新たな懸念：自己複製するプロンプトインジェクション](https://www.theregister.com/security/2026/09/29/add-one-more-ai-worry-to-the-nightmare-scenario-self-replicating-prompt-injections/5299922) | 25.0 | 20.0 | 42.0 |
| [OpenAI CEOが開発者会議で新しいAIエージェントを発表し、セキュリティ懸念には言及せず](https://www.securityweek.com/openai-ceo-announces-new-ai-agent-and-avoids-mention-of-security-concerns-at-developer-conference/) | 25.0 | 20.0 | 42.0 |
| [ブラウザ「Chrome」にセキュリティ更新 - 脆弱性32件を修正](https://www.security-next.com/190829) | 22.0 | 20.0 | 42.0 |
| [AI利用料金の急増を招く「LLMジャッキング」をセキュリティ専門家が警告](https://japan.zdnet.com/article/35253085/) | 21.0 | 20.0 | 42.0 |
| [恐喝集団 ShinyHunters かく語りき「我々の収益は合法的な企業をも大きく上回る」](https://scan.netsecurity.ne.jp/article/2026/09/30/56348.html) | 21.0 | 20.0 | 42.0 |
| [日本郵便 調査請求 Web受付サービスに不正アクセス、一時的に受付を停止](https://scan.netsecurity.ne.jp/article/2026/09/30/56344.html) | 21.0 | 20.0 | 42.0 |
| [ID・パスワードが窃取が原因 ～「HALMEK up」に不正アクセス](https://scan.netsecurity.ne.jp/article/2026/09/30/56343.html) | 21.0 | 20.0 | 42.0 |
| [長野県大町市デジタルアーカイブサイトに不正アクセス、オンラインカジノサイト誘導ページに改ざん](https://scan.netsecurity.ne.jp/article/2026/09/30/56342.html) | 21.0 | 20.0 | 42.0 |
| [保育上の不適切な対応も確認 ～ 鎌倉市児童発達支援センターあおぞら園で個人情報を誤送付](https://scan.netsecurity.ne.jp/article/2026/09/30/56341.html) | 21.0 | 20.0 | 42.0 |
| [山口東京理科大チームが優勝 ～ 県警ら主催「サイバー攻撃共同対処訓練」で約 90 名が Micro Hardening 演習](https://scan.netsecurity.ne.jp/article/2026/09/30/56340.html) | 21.0 | 20.0 | 42.0 |
| [11 / 2 までエントリー受付「セキュリティ・キャンプ2026オンライン」初級・中級コースをオンライン開催](https://scan.netsecurity.ne.jp/article/2026/09/30/56338.html) | 21.0 | 20.0 | 42.0 |
| [HENNGE One、コンテンツプラットフォーム「riclink」と SSO 連携](https://scan.netsecurity.ne.jp/article/2026/09/30/56337.html) | 21.0 | 20.0 | 42.0 |
| [タイムズカーで不正アクセス 「退会済み」含む約660万件の情報が流出](https://atmarkit.itmedia.co.jp/ait/articles/2609/30/news038.html) | 21.0 | 20.0 | 42.0 |
| [1万件超のドメインを保有する攻撃者--悪用される「中古」ドメインの実態](https://japan.zdnet.com/article/35252932/) | 21.0 | 20.0 | 42.0 |
| [国産セキュリティー製品の勝ち筋](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/091400256/091400001/) | 21.0 | 20.0 | 42.0 |
| [企業のセキュリティー対策動向 外部委託と内製で方針二分](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020600010/092400234/) | 21.0 | 20.0 | 42.0 |
| [CISA ICS Advisory / ICS Medical Advisory（2026年09月29日）](https://jvn.jp/vu/JVNVU93754811/) | 20.0 | 20.0 | 42.0 |
| [Signal、iOSとデスクトップアプリに暗号化されたローカルバックアップ機能を追加](https://www.bleepingcomputer.com/news/security/signal-adds-encypted-local-backup-support-to-ios-desktop-apps/) | 20.0 | 20.0 | 42.0 |
| [Unsloth Studioの欠陥により、通常のモデル検査がコード実行に変わる](https://www.darkreading.com/application-security/unsloth-studio-flaw-model-inspection-code-execution) | 20.0 | 20.0 | 42.0 |
| [米空軍関係者、200万ドル超のサイバー窃盗で6年以上の実刑判決](https://therecord.media/us-air-force-members-given-6-year-sentence-cyber) | 20.0 | 20.0 | 42.0 |
| [FBIがShinyHuntersメンバーに最近の逮捕を受け出頭を呼びかけ](https://www.bleepingcomputer.com/news/security/fbi-tells-shinyhunters-members-to-turn-themselves-in-after-recent-arrest/) | 20.0 | 20.0 | 42.0 |

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
