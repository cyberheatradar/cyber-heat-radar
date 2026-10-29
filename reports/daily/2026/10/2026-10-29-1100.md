# 📡 サイレーダー 2026-10-29 11:00 JST

このレポートは、2026-10-29 05:00 JST〜2026-10-29 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 71
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 45

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Inside KeyDrift: Analyzing historical UAT-11473 activity on Cisco SD-WAN](#topic-17617) | 47.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 2 | [Vulnerabilities in Node.<wbr>js Affecting Cisco Products: October 2026](#topic-39379) | 39.0 | 64.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [Yet Another ClickFix Campaign, (Wed, Oct 28th)](#topic-40148) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-17617"></a>

### 1. Inside KeyDrift: Analyzing historical UAT-11473 activity on Cisco SD-WAN

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>国⁠家⁠支⁠援</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 47.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Cisco Talosは、Cisco SD-WAN環境を狙った脅威活動「UAT-11473」による歴史的な活動を分析し、CVE-2026-20127の悪用に関する文脈を示しました。
Ciscoの公表では、この脆弱性は認証をバイパスして高権限を取得できる可能性があり、影響を受ける製品には修正アップデートが提供されています。
SD-WANの管理基盤はネットワーク全体の制御に関わるため、認証バイパスが成立すると影響が広範囲に及ぶおそれがあります。
脅威アクターの活動文脈と結びついている点から、単なる脆弱性情報よりも優先度を上げて確認すべき事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Ciscoの該当製品が影響対象に含まれるかを確認し、提供済みの修正アップデートを適用する。
- 管理系インターフェースへの不審な認証試行や権限変更、設定変更の有無を点検する。
- 外部公開された管理面の露出を見直し、不要な到達経路を最小化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20127 | 関連CVE | 1.00 | 候補あり（URL 6件以上） |
| 脆弱性 | CVE-2026-20245 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Catalyst SD-WAN Manager | 言及あり | 0.80 | — |
| 脅威アクター | Volt Typhoon | 主題 | 0.80 | — |
| 製品 | OpenSSL | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20127](https://nvd.nist.gov/vuln/detail/CVE-2026-20127) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-rpa-EHchtZk) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Inside KeyDrift: Analyzing historical UAT-11473 activity on Cisco SD-WAN](https://blog.talosintelligence.com/uat-11473-keydrift/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Malicious hackers exploit Cisco zero-day for highest access level at communicati](https://cyberscoop.com/cisco-sd-wan-zero-day-exploit-communications-provider/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco adds another SD-WAN box to max-severity bug advisory](https://www.theregister.com/security/2026/06/17/cisco-adds-another-sd-wan-box-to-max-severity-bug-advisory/5257621) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-40148"></a>

### 2. Yet Another ClickFix Campaign, (Wed, Oct 28th)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

SANS Internet Storm Centerが、ClickFixに関連する新たな攻撃キャンペーンについて取り上げています。
提供された情報からは詳細な手口や影響範囲は読み取れませんが、継続的に観測されている脅威として注目されています。
ClickFix系のキャンペーンは、利用者の操作を誘導して被害につながる可能性があるため、実務上は注意が必要です。
新たな事例として共有されていることから、現場では関連するフィッシングや不審な誘導への警戒を再確認する意味があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 不審な操作誘導や認証・確認を装う画面遷移がないか、利用者向け注意喚起を見直す。
- メール、Web、チャット経由の誘導について、URLや文面の異常を検知・報告しやすい運用にする。
- 同種のキャンペーンに備え、端末保護・ブラウザ保護・ログ監視の基本設定を点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Yet Another ClickFix Campaign, (Wed, Oct 28th)](https://isc.sans.edu/diary/rss/33466) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-39379"></a>

### 1. Vulnerabilities in Node.<wbr>js Affecting Cisco Products: October 2026

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Node.<wbr>jsのBrotliデコーダに関する脆弱性「CVE-2026-111497」について、Ciscoなど複数ベンダーが関連製品への影響を案内しています。
公開情報では、特定のBrotliデータを処理するアプリケーションでリモートコード実行につながる可能性が示されており、Node.<wbr>jsの修正版提供も案内されています。
Node.<wbr>jsは多くの製品やサービスの基盤で使われているため、影響範囲が広がる可能性があります。
関連ベンダーが注意喚起を出していることから、依存している製品やサービスの更新優先度が高い話題です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 11 sources。
- 実悪用・ゼロデイ文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Node.<wbr>jsの該当リリース系統を使っているか、また組み込み利用している製品がないか確認する。
- ベンダーの修正版・緩和策の適用状況を点検し、更新計画を前倒しする。
- Brotliを扱う処理や外部入力を受ける機能について、例外や異常終了の監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-105482 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-105483 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-106069 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-111497 | 関連CVE | 1.00 | 候補あり（URL 29件以上） |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| ベンダー | Wiz | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-111497](https://nvd.nist.gov/vuln/detail/CVE-2026-111497) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in Node.<wbr>js Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-oct2026-node-js-Jj3SQ19u) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-111497 Portfolio Status: Impact of Brotli Vulnerability (CVE-2026-11149](https://security.paloaltonetworks.com/CVE-2026-111497) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Adobe Commerce PolyShell Attacks Breach Hundreds of Stores as Brotli Exploit Tra](https://thehackernews.com/2026/10/adobe-commerce-polyshell-attacks-breach.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Brotli bug reaches far beyond Node.<wbr>js (CVE-2026-111497)](https://www.helpnetsecurity.com/2026/10/27/node2shell-broccoli2shell-vulnerability-cve-2026-111497/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Experts temper emergency-level alarms over critical Brotli defect](https://cyberscoop.com/brotli-critical-vulnerability-decompression-library-node2shell-broccoli2shell/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [eMudhra, Brotli, and the Long Tail of a Security Fix](https://socket.dev/blog/emudhra-brotli-security-fix) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft releases emergency .<wbr>NET security fixes for Google Brotli bug](https://www.theregister.com/security/2026/10/26/microsoft-releases-emergency-net-security-fixes-for-google-brotli-bug/5305515) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（5件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [1回25ドルで始まる自動攻撃--プルーフポイントが警鐘を鳴らすAIハーネスの脅威](https://japan.zdnet.com/article/35254113/) | 29.0 | 30.0 | 42.0 |
| [クラウドの「中枢」を奪われたら何が起きる？ 495社の仮想サーバを止めたIDCFランサムウェア攻撃の全容](https://atmarkit.itmedia.co.jp/ait/articles/2610/29/news044.html) | 29.0 | 30.0 | 42.0 |
| [IDCFクラウド障害、侵入経路は特定 194組織のデータが取り出し可能に](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/102201517/) | 29.0 | 30.0 | 42.0 |
| [VPNがあるのは外から分かるので狙われる。パッチ当てはもう自動化するしかない――日本ハッカー協会・杉浦隆幸代表理事が語る、AI時代のランサムウェア対処策【Security Days Fall 2026】](https://internet.watch.impress.co.jp/docs/event/2151590.html) | 28.0 | 30.0 | 42.0 |
| [「IDCFクラウド」が不正アクセスの調査結果公開、データ流出は「ありませんでした」 原因はオープンソースソフトウェアの脆弱性、段階的に提供再開の見通し](https://internet.watch.impress.co.jp/docs/news/2151956.html) | 28.0 | 30.0 | 42.0 |
| [「Claude Enterprise」、AIの投資対効果を把握する3つの機能を一般提供](https://japan.zdnet.com/article/35254135/) | 28.0 | 20.0 | 42.0 |
| [Googleが世界一高性能なAI「Gemini 4 Carbon」を発表、ついにOpenAIやAnthropicの最先端モデルを超える](https://gigazine.net/news/20261029-gemini-4-carbon/) | 27.0 | 20.0 | 42.0 |
| [無料で災害や非常時にオフラインで動作できるサバイバル知識満載のAIアシスタント「Survival LLM」、停電時の食料の安全な保管方法・火傷の手当て方法・水の浄化方法などを信頼できる情報源から回答し出典も表示可能](https://gigazine.net/news/20261029-survival-llm/) | 27.0 | 20.0 | 42.0 |
| [OpenAIとAnthropicが2026年夏から秋にかけてLLM料金を相次いで値下げした理由とは？](https://gigazine.net/news/20261029-openai-anthropic-llm-price-cuts/) | 27.0 | 20.0 | 42.0 |
| [パナソニック、禁止された生成AIに約33万人分の個人情報をアップロード](https://news.mynavi.jp/techplus/article/20261029-5214710/) | 26.0 | 20.0 | 42.0 |
| [AI の「ハッカー」が広く使われる産業制御ソフトの深刻な脆弱性 4 件を 4 時間足らずで発見](https://scan.netsecurity.ne.jp/article/2026/10/29/56622.html) | 26.0 | 20.0 | 42.0 |
| [ルールに違反し外部生成AIサービスにパナソニックグループ従業員の個人情報をアップロード](https://scan.netsecurity.ne.jp/article/2026/10/29/56617.html) | 26.0 | 20.0 | 42.0 |
| [生成AIで精巧な偽ログイン画面を作成、企業アカウント乗っ取りの恐れ](https://news.mynavi.jp/techplus/article/20261029-5209700/) | 26.0 | 20.0 | 42.0 |
| [Google、「Gemini 4 Carbon」発表 「Argon」公開から2週間、サイバー防御能力などを強化](https://www.itmedia.co.jp/news/article/2610/29/2000002690/) | 26.0 | 20.0 | 42.0 |
| [みずほが3万人にAIエージェント 「Cowork」で非定型業務も自律化](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/102201515/) | 26.0 | 20.0 | 42.0 |
| [エアークローゼット、AIで自動開発 変更の95％超、人手を介さず本番へ](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/102201520/) | 26.0 | 20.0 | 42.0 |
| [京都銀行、粉飾見抜くAIを内製 10年分の決算書や行員の知見基に](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/102201518/) | 26.0 | 20.0 | 42.0 |
| [進化するAIが落とす影](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/101900258/101900001/) | 26.0 | 20.0 | 42.0 |
| [「Gemini Notebook」で名刺を文字起こしして管理！ PFUの小型スキャナー「ScanSnap iX110」活用（後編）【自宅Wi-Fiの“わからない”をスッキリ！】](https://internet.watch.impress.co.jp/docs/column/homewifi/2151171.html) | 25.0 | 20.0 | 42.0 |
| [LinuxカーネルやVMware ESXの脆弱性、悪用を確認 - 米当局](https://www.security-next.com/192136) | 24.0 | 20.0 | 43.0 |
| [Cloudbase、CNAPPに蓄積された情報を起点に重要資産への到達経路を検証する「コンテキスト・ドリブン・ペネトレーションテスト」提供](https://scan.netsecurity.ne.jp/article/2026/10/29/56613.html) | 23.0 | 20.0 | 42.0 |
| [「Sophos UTM」に深刻なRCE脆弱性 - EOLで手動パッチ必要](https://www.security-next.com/192142) | 22.0 | 20.0 | 42.0 |
| [Smashing Security podcast #490: Jared KushnerのiPhoneが2度ハッキングされたとされる件](https://grahamcluley.com/smashing-security-podcast-490/) | 22.0 | 20.0 | 42.0 |
| [Ciscoの「ASA」「FTD」にDoS脆弱性 - すでに悪用も](https://www.security-next.com/192131) | 22.0 | 20.0 | 42.0 |
| [渦中のGMO、熊谷代表の発信は“火に油”か？ 「経営トップが自ら広報」の功罪](https://www.itmedia.co.jp/news/article/2610/29/2000002674/) | 21.0 | 20.0 | 42.0 |
| [バンナム、メアド34万件漏えい ガンダムグッズ店のポイント会員が対象 ユミルリンクへの不正アクセスが原因](https://www.itmedia.co.jp/news/article/2610/29/2000002694/) | 21.0 | 20.0 | 42.0 |
| [「ツイキャス」不正アクセスで停止 復旧までに「相応の時間」](https://www.itmedia.co.jp/news/article/2610/29/2000002692/) | 21.0 | 20.0 | 42.0 |
| [「異常検知はもう通用しない」 フロンティアAIが覆すセキュリティの前提、ガートナーが警鐘](https://atmarkit.itmedia.co.jp/ait/articles/2610/29/news026.html) | 21.0 | 20.0 | 42.0 |
| [攻撃者に屈する前に“システムを自ら止める”――そのための「経営層の理解」をどう得る？ NRIが打ち出した支援策とは](https://atmarkit.itmedia.co.jp/ait/articles/2610/29/news040.html) | 21.0 | 20.0 | 42.0 |
| [三井住友DS投信直販ネットのマイページにログインできない状況に、取引委託業者のシステムで不正アクセスを検知](https://scan.netsecurity.ne.jp/article/2026/10/29/56621.html) | 21.0 | 20.0 | 42.0 |
| [「ショップサーブ」に不正アクセス、漏えい対象者数は約2,335万6,000人](https://scan.netsecurity.ne.jp/article/2026/10/29/56620.html) | 21.0 | 20.0 | 42.0 |
| [フジテレビの番組宣伝システムに不正アクセス、メディア関係者の個人情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/10/29/56619.html) | 21.0 | 20.0 | 42.0 |
| [医療機関業務支援システム「@link（アットリンク）」に不正アクセス、サービスの提供を一時停止](https://scan.netsecurity.ne.jp/article/2026/10/29/56618.html) | 21.0 | 20.0 | 42.0 |
| [BtoC通販向け決済「NP後払い」に不正アクセス](https://scan.netsecurity.ne.jp/article/2026/10/29/56616.html) | 21.0 | 20.0 | 42.0 |
| [石油資源開発が利用するラクスライトクラウドのASPサービス「blastmail」に不正アクセス](https://scan.netsecurity.ne.jp/article/2026/10/29/56615.html) | 21.0 | 20.0 | 42.0 |
| [丸木医科器械へのサイバー攻撃で基幹システムがダウン、FAX で注文受付](https://scan.netsecurity.ne.jp/article/2026/10/29/56614.html) | 21.0 | 20.0 | 42.0 |
| [電子納品物検査支援システムにインストール時の不適切なファイルアクセス権設定の脆弱性](https://scan.netsecurity.ne.jp/article/2026/10/29/56612.html) | 21.0 | 20.0 | 42.0 |
| [ローソン、個人情報215万件漏洩 自動検知すり抜け人手の調査で発覚](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/102201519/) | 21.0 | 20.0 | 42.0 |
| [件数の多い脆弱性から直すのは正解か ネットワーク診断の指摘、半数超は「パッチ管理」](https://www.itmedia.co.jp/enterprise/articles/2610/29/news013.html) | 21.0 | 20.0 | 42.0 |
| [主要なBulletproof Hosting提供事業者Virtualineのドメインを当局が差し押さえ](https://cyberscoop.com/virtualine-bulletproof-hosting-provider-seized/) | 20.0 | 20.0 | 42.0 |
| [三菱UFJ・静岡銀はなぜ「止める決断」？ PHP欠陥が突きつけた銀行の“思わぬ弱点”](https://www.sbbit.jp/article/fj/187855?ref=rss) | 20.0 | 20.0 | 42.0 |
| [Leak siteに、ハクティビストが入手した4万1000人超のDHS職員データが公開される](https://cyberscoop.com/dhs-employee-data-leak-ddosecrets/) | 20.0 | 20.0 | 42.0 |
| [ランサムウェアやサイバー犯罪に関連するVirtualineの耐弾性サービスを警察が摘発](https://www.bleepingcomputer.com/news/security/police-seize-virtualine-bulletproof-service-tied-to-ransowmare-cybercrime/) | 20.0 | 20.0 | 42.0 |
| [Japan Airlinesがデータ侵害を警告、相次ぐサイバーインシデントに日本が直面](https://therecord.media/japan-airlines-warns-of-breach-country-grapples-with-incidents) | 20.0 | 20.0 | 42.0 |
| [「楽天トラベル」に不正アクセス 顧客情報最大約260万件など流出か 予約者約3.6万件のクレカ情報も](https://www.itmedia.co.jp/news/article/2610/27/2000002606/) | 10.0 | 20.0 | 42.0 |

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
