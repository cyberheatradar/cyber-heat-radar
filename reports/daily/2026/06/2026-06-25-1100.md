# 📡 サイレーダー 2026-06-25 11:00 JST

このレポートは、2026-06-25 05:00 JST〜2026-06-25 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 66
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 2
- [低温だが記録しておくトピック](#low-record-topics): 39

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Mandiant reveals how Cisco SD-WAN zero-day attacks gained root access](#topic-15753) | 43.0 | 58.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [The hits keep on coming for Cisco vulnerabilities](#topic-14652) | 39.0 | 64.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [Malicious Edge extension abuses Native Messaging as bridge to malware](#topic-19234) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-19234"></a>

### 1. Malicious Edge extension abuses Native Messaging as bridge to malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoft Edgeの悪性拡張機能「Edgecution」が、ブラウザの制限を回避するためにNative Messagingを悪用し、マルウェア展開につながったと報じられています。
報道では、この手口がランサムウェア攻撃の文脈で使われ、Pythonベースのバックドア配備に関係していたとされています。
ブラウザ拡張機能は利便性が高い一方、正規機能との組み合わせで端末側へ影響が及ぶ可能性があるため注意が必要です。
特に管理対象端末では、拡張機能の導入管理や権限の見直しが重要になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Edge拡張機能の導入状況を棚卸しし、不要な拡張機能は削除・無効化する。
- Native Messagingを利用する拡張機能について、許可対象と接続先の管理方針を確認する。
- EDRやログで、ブラウザ起点の不審なプロセス生成やバックドア挙動の兆候を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Malicious Edge extension abuses Native Messaging as bridge to malware](https://www.bleepingcomputer.com/news/security/malicious-edge-extension-abuses-native-messaging-as-bridge-to-malware/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-15753"></a>

### 1. Mandiant reveals how Cisco SD-WAN zero-day attacks gained root access

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 58.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Catalyst SD-WAN Managerにおける権限昇格の脆弱性「CVE-2026-20245」について、Mandiantがゼロデイ攻撃で悪用された状況を公表しました。
公開情報によると、攻撃者は初期アクセス後に権限を引き上げ、root権限に到達したとされています。
Ciscoは現時点で修正パッチを提供していないとされ、影響範囲の把握と暫定対策が重要です。
ネットワーク管理基盤が対象で、権限昇格により機器の制御や設定変更につながる可能性があるためです。
さらに、悪用観測が示されている一方で未修正の状況が続いており、運用現場での警戒度が高い案件です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

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

- Ciscoの告知と対象製品の影響有無を確認し、管理系アクセスの保護を強化する。
- 関連する初期侵入経路や不審な管理者権限の利用、root相当の変更履歴を点検する。
- 公式の修正情報が出るまで、公開範囲の最小化や監視強化などの暫定対策を継続する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20127 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20182 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20245 | 関連CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20245](https://nvd.nist.gov/vuln/detail/CVE-2026-20245) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Mandiant reveals how Cisco SD-WAN zero-day attacks gained root access](https://www.bleepingcomputer.com/news/security/mandiant-reveals-how-cisco-sd-wan-zero-day-attacks-gained-root-access/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zero-Day Exploitation of Vulnerability (CVE-2026-20245) in Cisco Catalyst SD-WAN](https://cloud.google.com/blog/topics/threat-intelligence/zero-day-exploitation-cisco-catalyst-sd-wan-manager/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller, Catalyst SD-WAN Manager, and Catalyst SD-WAN V](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-privesc-4uxFrdzx) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco customers encounter another SD-WAN zero-day under attack](https://cyberscoop.com/cisco-sdwan-zero-day-vulnerability-exploited-cve202620245/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Manager CVE-2026-20245 Flaw Actively Exploited – No Patch ](https://thehackernews.com/2026/06/cisco-catalyst-sd-wan-manager-cve-2026.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco SD-WAN 0-day exploited, no patch available (CVE-2026-20245)](https://www.helpnetsecurity.com/2026/06/05/cisco-sd-wan-cve-2026-20245-0-day-exploited/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補あり（URL 7件以上 / 該当CVE 3件）。

---

<a id="topic-14652"></a>

### 2. The hits keep on coming for Cisco vulnerabilities

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Unified Communications Manager（Unified CM）とUnified CM SMEに存在するCVE-2026-20230について、公開された情報では悪用が観測されているとされています。
Ciscoの説明によれば、この問題は特定のHTTPリクエスト処理における入力検証不備に起因し、認証なしのリモート攻撃者によるSSRFにつながる可能性があります。
影響対象が通信基盤として使われる製品で、成功するとシステム権限の奪取につながるおそれがあるため、優先度が高い脆弱性です。
加えて、修正パッチは提供済みで、実際の悪用観測も報じられているため、放置リスクが上がっています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
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

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Ciscoの修正済みソフトウェアを適用し、対象バージョンの有無を確認する。
- WebDialerサービスの有効化状況を確認し、不要なら無効化を検討する。
- Unified CM/SMEの外向き通信や不審なHTTPリクエスト、ファイル生成などの兆候を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20230 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20245 | 関連CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20230](https://nvd.nist.gov/vuln/detail/CVE-2026-20230) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [The hits keep on coming for Cisco vulnerabilities](https://www.theregister.com/security/2026/06/24/the-hits-keep-on-coming-for-cisco-vulnerabilities/5261797) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified CM flaw actively exploited to drop webshells (CVE-2026-20230)](https://www.helpnetsecurity.com/2026/06/24/cisco-unified-cm-flaw-exploited-to-drop-webshells-cve-2026-20230/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers Exploiting Cisco Unified CM Vulnerability](https://www.securityweek.com/hackers-exploiting-cisco-unified-cm-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified CM flaw CVE-2026-20230 now exploited in attacks](https://www.bleepingcomputer.com/news/security/cisco-unified-cm-sme-flaw-cve-2026-20230-now-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified Communications Manager Server-Side Request Forgery Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-cucm-ssrf-cXPnHcW) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補あり（URL 5件以上 / 該当CVE 2件）。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [D&Mにランサムウェア攻撃、過去約 2 年分の FAX 受注データが外部流出した可能性](https://scan.netsecurity.ne.jp/article/2026/06/25/55567.html) | 29.0 | 30.0 | 42.0 |
| [ランサムウェア犯も失敗したくない ホワイトハッカーが明かす“身代金ビジネス”の実態](https://atmarkit.itmedia.co.jp/ait/articles/2606/25/news054.html) | 29.0 | 30.0 | 42.0 |
| [EDR停止まで“サービスで提供” 攻撃者を支える闇のプラットフォームの実態](https://atmarkit.itmedia.co.jp/ait/articles/2606/25/news039.html) | 29.0 | 30.0 | 42.0 |
| [YCC情報システムが第5報 管理者アカウントを使われたか](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/031800050/061700088/) | 29.0 | 30.0 | 42.0 |
| [D-Linkルータなど4300台超が感染、古い機種狙う新マルウェア](https://news.mynavi.jp/techplus/article/20260625-4618569/) | 29.0 | 20.0 | 42.0 |
| [Smashing Security podcast #473: ハッカーがワールドカップ全体をRickrollできた可能性](https://grahamcluley.com/smashing-security-podcast-473/) | 28.0 | 30.0 | 42.0 |
| [ソフトバンクと OpenAI が協業、サイバーセキュリティ対策「Patching as a Service」提供](https://scan.netsecurity.ne.jp/article/2026/06/25/55564.html) | 26.0 | 20.0 | 42.0 |
| [7 / 22・23 開催「AI DevEx conference 2026」にエーアイセキュリティラボ 出展・登壇](https://scan.netsecurity.ne.jp/article/2026/06/25/55563.html) | 26.0 | 20.0 | 42.0 |
| [電子ペーパー採用のAIスマートノート「iFLYTEK AINOTE 2」、大型アプデで翻訳・文字起こしなどの機能を強化](https://internet.watch.impress.co.jp/docs/news/2119756.html) | 25.0 | 20.0 | 42.0 |
| [SearchLeak: M365 Copilotをワンクリックでデータ流出兵器に変えた手口](https://cloudsecurityalliance.org/articles/searchleak-how-we-turned-m365-copilot-into-a-one-click-data-exfiltration-weapon) | 25.0 | 20.0 | 42.0 |
| [誰も聞いていないとき、ポートは何を聞くのか：自動化サイバー犯罪の評価［ゲストダイアリー］](https://isc.sans.edu/diary/rss/33104) | 22.0 | 20.0 | 42.0 |
| [Cisco、7月1日の脆弱性修正を事前予告 - 「Catalyst Center」など対象](https://www.security-next.com/186380) | 22.0 | 20.0 | 42.0 |
| [「Chrome」に「クリティカル」4件を含む脆弱性修正アップデート](https://www.security-next.com/186374) | 22.0 | 20.0 | 42.0 |
| [ログ統合と高速分析で発見統制を強化、情報漏えいをリアルタイムでブロック―全体最適化を実現した CrowdStrike Falcon 統合基盤](https://news.mynavi.jp/techplus/kikaku/20260625-4558399/) | 21.0 | 20.0 | 42.0 |
| [守るべきはIT資産ではなく事業プロセス – IPA・青山氏が語る「事業を止めない」セキュリティ](https://news.mynavi.jp/techplus/article/20260625-4594108/) | 21.0 | 20.0 | 42.0 |
| [「マシンスピードの攻撃」にどう立ち向かうか AI時代に必要な先制的サイバーセキュリティ](https://ascii.jp/elem/000/004/413/4413235/?rss=) | 21.0 | 20.0 | 42.0 |
| [KDDIメール基盤から最大で1422万件漏えい ニフティやBIGLOBEなど6社に波及](https://www.itmedia.co.jp/enterprise/articles/2606/25/news043.html) | 21.0 | 20.0 | 42.0 |
| [CSIRT支援室 第36回 CVEを年間数十件取得している猛者たちにそのモチベーションを聞いてみた：後編](https://scan.netsecurity.ne.jp/article/2026/06/25/55574.html) | 21.0 | 20.0 | 42.0 |
| [KDDIのISP事業者向けメールシステムに不正アクセス、最大1,422万件のメールアドレス・パスワードが漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/06/25/55573.html) | 21.0 | 20.0 | 42.0 |
| [「WebARENA 大容量ファイル転送機能」への不正アクセス、提供再開は2026年12月頃を目途](https://scan.netsecurity.ne.jp/article/2026/06/25/55572.html) | 21.0 | 20.0 | 42.0 |
| [Fortinet製品に関連する認証情報の漏えいに注意を呼びかけ](https://scan.netsecurity.ne.jp/article/2026/06/25/55571.html) | 21.0 | 20.0 | 42.0 |
| [AeyeScan、SaaS型Webアプリケーション脆弱性診断・管理市場でシェア1位を獲得](https://scan.netsecurity.ne.jp/article/2026/06/25/55570.html) | 21.0 | 20.0 | 42.0 |
| [はてな資金流出、11 億 7,900 万円を特別損失として計上](https://scan.netsecurity.ne.jp/article/2026/06/25/55569.html) | 21.0 | 20.0 | 42.0 |
| [UPSIDERホールディングスへの不正アクセス、個人情報・法人情報の流出の可能性は極めて低いと判断](https://scan.netsecurity.ne.jp/article/2026/06/25/55568.html) | 21.0 | 20.0 | 42.0 |
| [VPN 脆弱性の放置や安易なパスワードで指導 ～ 個人情報保護委員会 令和 7 年度 4Q 監視レポート](https://scan.netsecurity.ne.jp/article/2026/06/25/55566.html) | 21.0 | 20.0 | 42.0 |
| [世界から選抜された捜査官160名が挑戦 ～ GMOサイバー犯罪対策センター局長 福森氏が実践演習を監修](https://scan.netsecurity.ne.jp/article/2026/06/25/55565.html) | 21.0 | 20.0 | 42.0 |
| [日立がMythosのアクセス権獲得 社会インフラの安全性向上に一手](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/061801453/) | 21.0 | 20.0 | 42.0 |
| [個人情報保護法改正案が衆院通過 統計特例に付帯決議、罰則には異論](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/061801455/) | 21.0 | 20.0 | 42.0 |
| [スマホを通じた「シャドープロファイル」--データ収集の手法とその対策を解説](https://japan.zdnet.com/article/35249230/) | 21.0 | 20.0 | 42.0 |
| [内閣官房のIPA指名停止は隠蔽誘発か 再委託先の違反報告でも処分対象](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/061801456/) | 21.0 | 20.0 | 42.0 |
| [KDDIのメールシステムに不正アクセス 最大1422万件情報漏えいの恐れ](https://atmarkit.itmedia.co.jp/ait/articles/2606/25/news036.html) | 21.0 | 20.0 | 42.0 |
| [AIのトークンが企業や経済を左右する--格差の到来とコスト高騰の未来](https://japan.zdnet.com/article/35249257/) | 21.0 | 20.0 | 42.0 |
| [AmazonのASUSストアでWindowsノートがセール中！ Windows 11搭載14インチノートは8万9800円から。GeForce RTX 5060搭載のゲーミングノートPCも安い](https://internet.watch.impress.co.jp/docs/shopping/2119855.html) | 20.0 | 20.0 | 42.0 |
| [初学者でも気軽に挑戦できる「セキュリティ・キャンプ2026ミニ」、全国9地域で参加受付開始 講義内容や講師情報も一斉公開](https://internet.watch.impress.co.jp/docs/news/2119751.html) | 20.0 | 20.0 | 42.0 |
| [AGA治療や痩身目的のオンライン診療、処方薬が意図せず定期購入契約にされるトラブルに、国民生活センターが注意喚起](https://internet.watch.impress.co.jp/docs/news/2119582.html) | 20.0 | 20.0 | 42.0 |
| [DraftKingsのハッカー「Snoopy」に18か月の禁錮刑](https://www.bleepingcomputer.com/news/security/draftkings-hacker-snoopy-sentenced-to-18-months-in-prison/) | 20.0 | 20.0 | 42.0 |
| [金融庁準拠だけでは「サイバー防衛」は大変？新評価基準「CRI Profile」が役立つワケ](https://www.sbbit.jp/article/fj/185757?ref=rss) | 20.0 | 20.0 | 42.0 |
| [攻撃者がCisco SD-WANの脆弱性を公開2か月前に悪用](https://www.darkreading.com/cyberattacks-data-breaches/attackers-hit-cisco-sd-wan-flaw-2-months-before-disclosure) | 20.0 | 20.0 | 42.0 |
| [2026 FIFA World Cupを狙うサイバー脅威の急増](https://www.darkreading.com/cybersecurity-operations/2026-fifa-world-cup-faces-surge-cyber-threats) | 20.0 | 20.0 | 42.0 |

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
