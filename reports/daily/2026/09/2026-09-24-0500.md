# 📡 サイレーダー 2026-09-24 05:00 JST

このレポートは、2026-09-23 17:00 JST〜2026-09-24 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 97
- [音声で扱う想定のトピック](#audio-topics): 10
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 61

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [F5 Patches Critical BIG-IP APM Zero-Day Exploited for Unauthenticated RCE on OAuth Servers](#topic-33905) | 52.0 | 64.0 | 59.0 | 音声 | 温度感上位枠 |
| 2 | [Chinese Hackers Exploit Chrome-Windows Zero-Day Chain to Deploy CLEANGULP Malware](#topic-31075) | 41.0 | 46.0 | 63.0 | 音声 | 温度感上位枠 |
| 3 | [米当局、複数ネットワーク関連製品の脆弱性悪用に注意喚起](#topic-33985) | 39.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [WordPress 7.1.2 fixes critical unauthenticated path traversal vulnerability (CVE-2026-87902)](#topic-33901) | 38.0 | 46.0 | 54.0 | 音声 | 温度感上位枠 |
| 5 | [InfraTrust report warns network management systems under attack](#topic-33925) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [DarkMe RAT trades zero-days for plain phishing emails](#topic-33940) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 7 | [Arista patches actively exploited VeloCloud Orchestrator zero-day](#topic-33950) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 8 | [Considerations for Critical Infrastructure Operators Working With Third-Party ICS Integrators](#topic-33959) | 35.0 | 45.0 | 42.0 | 音声 | AI×Security枠 |
| 9 | [Malicious AI agents steal 600K credit cards, infect 100+ sites with skimmers](#topic-33909) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 10 | [Attackers Manipulate AI Chatbots in Mass Disinformation, Phishing Campaign](#topic-33924) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-33905"></a>

### 1. F5 Patches Critical BIG-IP APM Zero-Day Exploited for Unauthenticated RCE on OAuth Servers

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>R⁠C⁠E</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 52.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

F5は、BIG-IP Access Policy Manager（APM）に存在するCVE-2026-94127への対策を公表し、修正を提供しています。
公開情報では、この問題は認証なしでリモートコード実行につながる可能性があり、さらに悪用が観測されているとされています。
認証不要のRCEにつながり得る脆弱性は、影響範囲が限定的でも優先度が高い対応対象です。特に公開情報で悪用観測が示されているため、該当環境では早急な確認と更新が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- F5 BIG-IP APMを利用している場合は、対象バージョンと公開済み修正の適用状況を確認する。
- APMがOAuth認可サーバーとして動作している構成かどうかを把握し、該当有無を切り分ける。
- 監視ログや管理イベントを点検し、不審なアクセスや想定外の挙動がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-94127 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | F5 | 言及あり | 0.80 | — |
| 製品 | F5 BIG-IP | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-94127](https://nvd.nist.gov/vuln/detail/CVE-2026-94127) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Someone's attacking a critical 0-day RCE in F5 BIG-IP APM](https://www.theregister.com/security/2026/09/23/someones-attacking-a-critical-0-day-rce-in-f5-big-ip-apm/5298659) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-94127: Critical Unauthenticated RCE in F5 BIG-IP APM](https://www.rapid7.com/blog/post/etr-cve-2026-94127-critical-unauthenticated-rce-in-f5-big-ip-apm) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [F5 Patches Critical BIG-IP APM Zero-Day Exploited for Unauthenticated RCE on OAu](https://thehackernews.com/2026/09/f5-patches-critical-big-ip-apm-zero-day.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-31075"></a>

### 2. Chinese Hackers Exploit Chrome-Windows Zero-Day Chain to Deploy CLEANGULP Malware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>Exploit Kit</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Google Chromeの脆弱性CVE-2026-85046について、実際に悪用されていることが確認され、Googleは修正版を配信しています。
複数の報道では、ChromeとWindowsの欠陥を組み合わせた攻撃により、特定のマルウェア配布につながった可能性が示されていますが、詳細な攻撃の全体像は各報道の範囲にとどまります。
ブラウザのゼロデイが実環境で悪用されているため、更新の遅れがそのまま侵害リスクにつながります。CISAの既知悪用脆弱性リストにも載っており、優先度の高い対応対象とみなせます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Chromeを修正版へ速やかに更新し、配布完了までの端末を把握する。
- CISAのKEV掲載状況や社内の脆弱性管理基準に照らして優先対応する。
- 不審なWebアクセスやブラウザ経由の異常動作を監視し、関連端末の調査を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-85046 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-85880 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-87491 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Google | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Chromium | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-85046](https://nvd.nist.gov/vuln/detail/CVE-2026-85046) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Chinese Hackers Exploit Chrome-Windows Zero-Day Chain to Deploy CLEANGULP Malwar](https://thehackernews.com/2026/09/chinese-hackers-exploit-chrome-windows.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Volexity spots another China-aligned threat group exploiting Chrome and Microsof](https://cyberscoop.com/volexity-uta0565-china-exploit-chain-chrome-microsoft/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Chinese espionage groups swarm to exploit triple-link chain of zero-days](https://cyberscoop.com/china-espionage-groups-exploit-chain-zero-days/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Google patches actively exploited Chrome zero-day (CVE-2026-85046)](https://www.helpnetsecurity.com/2026/09/04/google-chrome-zero-day-cve-2026-85046/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/09/04/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33985"></a>

### 3. 米当局、複数ネットワーク関連製品の脆弱性悪用に注意喚起

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

米当局が、複数のネットワーク関連製品に存在する脆弱性について、実際にサイバー攻撃へ悪用されているとして注意喚起を行いました。
対象製品や個別の脆弱性はこの材料だけでは特定できませんが、既に悪用観測がある点が重要です。
ネットワーク機器や関連製品の脆弱性は、外部からの侵入や横展開の起点になりやすく、影響範囲が広がりやすい分野です。
悪用が確認されている場合は、公開情報だけでも早急な確認と優先度の見直しが必要になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象製品の資産棚卸しを行い、該当製品・該当バージョンの有無を確認する。
- ベンダーおよび公的機関の追加情報を確認し、修正パッチや回避策の適用可否を判断する。
- 管理画面や外部公開面のアクセス制限、監視強化、侵入の痕跡確認を優先する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [米当局、複数ネットワーク関連製品の脆弱性悪用に注意喚起](https://www.security-next.com/190591) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33901"></a>

### 4. WordPress 7.1.2 fixes critical unauthenticated path traversal vulnerability (CVE-2026-87902)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 38.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 54.0 |

#### 概要

WordPress 7.1.2では、認証不要で悪用される可能性がある重大なパストラバーサル脆弱性（CVE-2026-87902）が修正されています。
公開情報では、影響範囲は4.7.0から7.1.1までの各リリースとされており、条件がそろう環境ではサーバー上でコード実行につながる可能性があるとされています。
認証なしで影響しうるため、公開中のWordPressサイトでは優先度の高い対応対象になります。すでに悪用が始まっている可能性が示されており、放置すると侵害リスクが高まります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- WordPressを7.1.2へ早急に更新し、対象バージョンの利用有無を確認する。
- 公開WordPressサイトで不審なファイル追加や改変の有無を点検する。
- WAFや監視でWordPress周辺の異常なアクセス・ファイル操作を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-87902 | 関連CVE | 1.00 | 候補あり（URL 7件以上） |
| 製品 | WordPress | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-87902](https://nvd.nist.gov/vuln/detail/CVE-2026-87902) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Hackers start exploiting critical WordPress flaw for code execution](https://www.bleepingcomputer.com/news/security/hackers-start-exploiting-critical-wordpress-flaw-for-code-execution/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [WordPress 7.1.2 fixes critical unauthenticated path traversal vulnerability (CVE](https://www.helpnetsecurity.com/2026/09/23/cve-2026-87902-wordpress-7-1-2-security-release/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33925"></a>

### 5. InfraTrust report warns network management systems under attack

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

InfraTrustの報告として、企業インフラを制御するネットワーク管理システムが攻撃対象になっていると伝えられています。
複数の重要な脆弱性が、ベンダー公開の前後を問わず実際に悪用されたとされ、管理系システムの防御が改めて注目されています。
ネットワーク管理システムは、侵害されると広範囲の運用や監視に影響しうるため、被害の波及が大きくなりやすい領域です。
公開直後の脆弱性が素早く悪用される傾向が示されており、パッチ適用や露出確認の重要性が高まっています。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 管理系システムの公開範囲を見直し、不要なインターネット露出を減らす。
- ベンダーの修正情報を継続監視し、優先度を付けて迅速に適用する。
- 認証情報の保護と監査ログの確認を強化し、異常な管理操作を早期に検知する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [InfraTrust report warns network management systems under attack](https://www.bleepingcomputer.com/news/security/infratrust-report-warns-network-management-systems-under-attack/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33940"></a>

### 6. DarkMe RAT trades zero-days for plain phishing emails

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

DarkMe RATが再び確認され、従来のようなゼロデイ悪用ではなく、シンプルなフィッシングメールで端末上で実行させる手口が使われているとされています。
対象は情報窃取や遠隔操作に悪用されうるマルウェアであり、配布経路がメール主体に変わった点が注目されています。
高度な脆弱性悪用に依存しないため、より広い組織で一般的なメール防御が重要になります。既知の攻撃手法に近い形でも、実際の侵害につながる可能性がある点が警戒されています。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 不審なメールの添付ファイルやリンクを開かせないための注意喚起を徹底する。
- メール経由の初期侵入を想定し、Web/メールゲートウェイやEDRの検知・隔離設定を見直す。
- 未知の実行ファイルやダウンローダーの起動を抑える運用と、端末側の監視強化を確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [DarkMe RAT trades zero-days for plain phishing emails](https://www.helpnetsecurity.com/2026/09/23/darkme-rat-phishing-email-hits-corporate-targets/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33950"></a>

### 7. Arista patches actively exploited VeloCloud Orchestrator zero-day

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

Arista Networksは、VeloCloud Orchestrator（VCO）のオンプレミス環境に影響するゼロデイ脆弱性への修正を公開しました。
この問題はすでに悪用が確認されているとされ、対象環境では早急な対応が求められます。
ゼロデイかつ実際の悪用が報告されているため、公開された修正の適用が後手に回ると被害につながるおそれがあります。
特にオンプレミス運用の管理基盤は影響範囲が広くなりやすく、優先度の高い確認事項です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- VeloCloud Orchestrator のオンプレミス導入有無を確認し、該当する場合は提供された修正を優先適用する。
- 管理系システムへの不審なアクセスや設定変更、認証関連の異常を点検する。
- 修正適用までの間は、外部公開範囲や到達経路を最小化し、監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-93952 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Arista patches actively exploited VeloCloud Orchestrator zero-day](https://www.bleepingcomputer.com/news/security/arista-patches-actively-exploited-velocloud-orchestrator-zero-day/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Arista Urges Immediate Patching of Exploited VCO Zero-Day](https://www.securityweek.com/arista-urges-immediate-patching-of-exploited-vco-zero-day/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33959"></a>

### 8. Considerations for Critical Infrastructure Operators Working With Third-Party ICS Integrators

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>サ⁠プ⁠ラ⁠イ⁠チ⁠ェ⁠ー⁠ン</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 45.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

FBIとCISAは、重要インフラ事業者が第三者のICSインテグレーターと連携する際の注意点をまとめた文書を公表しました。
内容は、最小権限の徹底、リモートアクセスの管理、契約や運用手順におけるサイバーセキュリティ要件の明確化など、OT環境における第三者リスクの低減に焦点を当てています。
ICSやSCADAの運用では、委託先が広いアクセス権を持つほど、侵害時の影響が重要インフラ全体に及ぶおそれがあります。
第三者経由の侵害や設定不備は、設備や運用継続に直接関わるため、実務上の管理強化が注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 契約書やサービス合意に、データ保管場所、遠隔操作、パッチ管理、アクセス権限、変更管理の要件を明記する。
- インテグレーターのリモートアクセス経路は監視・記録し、可能であればオンデマンド型にして不要な常時接続を避ける。
- 万一に備え、手動運転やオフラインのバックアップ、インテグレーター不在時でも回復できる手順を確認しておく。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | Ivanti Connect Secure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Considerations for Critical Infrastructure Operators Working With Third-Party IC](https://www.cisa.gov/resources-tools/resources/considerations-critical-infrastructure-operators-working-third-party-ics-integrators) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-33909"></a>

### 9. Malicious AI agents steal 600K credit cards, infect 100+ sites with skimmers

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、金銭目的の脅威アクターがオープンソースのAIエージェントフレームワークを悪用し、複数のオンライン小売事業者を狙った攻撃を行ったとされています。
結果として、60万件超のクレジットカード情報が盗まれ、100以上のサイトにスキマーが仕込まれた可能性が示されています。
AIを使った攻撃の自動化や大規模化が、EC事業者や決済周辺の被害拡大につながり得る点が注目されています。
従来型の不正スクリプト被害に加えて、運用の速さや広がりに備える必要があるためです。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- オンラインストアや決済ページで、改ざん検知や不審な外部スクリプトの監視を強化する。
- カード情報を扱うシステムでは、ログ監査、権限管理、サードパーティ依存の棚卸しを定期的に行う。
- AI系ツールや自動化基盤の利用状況を把握し、想定外の連携や外部通信がないか確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Malicious AI agents steal 600K credit cards, infect 100+ sites with skimmers](https://www.bleepingcomputer.com/news/security/malicious-ai-agents-steal-600k-credit-cards-infect-100-plus-sites-with-skimmers/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-33924"></a>

### 10. Attackers Manipulate AI Chatbots in Mass Disinformation, Phishing Campaign

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

攻撃者がWeb上に不正なリンクやデータをばらまき、検索やAIチャットボットの回答に悪影響を与えようとしていると報じられています。
対象としてはChatGPTやGemini、GoogleのAI Overviewが挙げられていますが、現時点では公開情報ベースの報道内容として扱うのが適切です。
AIが生成・要約する回答が業務判断やユーザー誘導に使われる場面では、誤情報やフィッシングへの導線が拡大するおそれがあります。
検索結果や生成AIの回答品質が、従来のWeb対策だけでは十分に守れない可能性がある点が注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 社内でAI検索・要約機能を使う際は、回答をそのまま信頼せず一次情報で確認する運用を徹底する。
- 自社ブランド名や製品名を含む検索結果・AI要約に不自然な外部リンクや誘導文がないか定期的に確認する。
- フィッシング対策として、生成AI経由の問い合わせやリンク誘導も通常のメール・Web対策の対象に含める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Google | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Attackers Manipulate AI Chatbots in Mass Disinformation, Phishing Campaign](https://www.darkreading.com/threat-intelligence/attackers-manipulate-ai-chatbots-mass-disinformation-phishing-campaign) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

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
| [このWindowsマルウェアは最大4つのAIモデルに次の行動を投票させるよう設計されている](https://thehackernews.com/2026/09/windows-malware-is-built-to-let-up-to.html) | 33.0 | 20.0 | 42.0 |
| [Windows Botnet x47.c、AI APIの不正消費と18種類の攻撃手法を提供](https://www.infosecurity-magazine.com/news/x47c-botnet-ai-api-draining-18/) | 33.0 | 20.0 | 42.0 |
| [Fake Claude Maxプレゼント企画でユーザーのGoogleアカウント認証情報をだまし取る手口](https://www.helpnetsecurity.com/2026/09/23/fake-claude-max-giveaway-phishing/) | 33.0 | 20.0 | 42.0 |
| [Compromised MemTensorパッケージがnpmとPyPI経由でsckit認証情報窃取ツールを配布](https://thehackernews.com/2026/09/compromised-memtensor-packages-deliver.html) | 28.0 | 45.0 | 42.0 |
| [Ryukランサムウェア運用者に懲役2年の判決](https://cyberscoop.com/ryuk-ransomware-operator-karen-vardanyan-sentenced/) | 28.0 | 30.0 | 42.0 |
| [Ryukランサムウェア運営者、被害者から120万ドルを恐喝し2年の実刑判決](https://therecord.media/ransomware-ryuk-sentenced-doj) | 28.0 | 30.0 | 42.0 |
| [2026年、ランサムウェア攻撃が過去最多に到達](https://www.infosecurity-magazine.com/news/ransomware-attacks-reach-record/) | 28.0 | 30.0 | 42.0 |
| [Ryukランサムウェア関与者に24か月の禁錮刑](https://www.bleepingcomputer.com/news/security/ryuk-ransomware-member-sentenced-to-24-months-in-prison/) | 28.0 | 30.0 | 42.0 |
| [米国の主要5業界におけるフィッシングリスク：ANY.RUNのデータと対策](https://any.run/cybersecurity-blog/phishing-risk-industries/) | 28.0 | 20.0 | 42.0 |
| [未修正のUbuntu Linux脆弱性を悪用し、コンテナからホストroot権限へ脱出するエクスプロイト公開](https://thehackernews.com/2026/09/exploit-released-for-unpatched-ubuntu.html) | 27.0 | 38.0 | 52.0 |
| [AI従業員を雇って定型作業をお任せできる「Geta.Team」、各AI従業員に個別にメールアドレス・電話番号を割り当てできてセルフホスト可能、機能限定の無料版もあり](https://gigazine.net/news/20260923-geta-team/) | 27.0 | 20.0 | 42.0 |
| [Check Point Management ServerとSpark Firewall、F5 BIG-IP APMインスタンスへの攻撃](https://www.helpnetsecurity.com/2026/09/23/check-point-f5-big-ip-apm-zero-days-targeted/) | 26.0 | 38.0 | 43.0 |
| [AIによるインターネット掌握への懸念、終末シナリオの中で新たな切迫感を増す](https://www.securityweek.com/worries-about-an-ai-internet-takeover-gain-new-urgency-among-doomsday-scenarios/) | 25.0 | 20.0 | 42.0 |
| [OpenAIとウクライナ、電力網と水道システムを保護する「Daybreak」プログラムで提携](https://cyberscoop.com/openai-ukraine-cybersecurity-critical-infrastructure/) | 25.0 | 20.0 | 42.0 |
| [企業が最も懸念するのはサイバー攻撃、AIとサプライチェーンへの不安が背景に](https://www.cybersecuritydive.com/news/cybersecurity-risks-business-worries-travelers-report/831142/) | 25.0 | 20.0 | 42.0 |
| [AI対応企業のための可観測性ギャップの解消](https://www.theregister.com/security/2026/09/23/sponsored-closing-the-observability-gap-for-the-ai-ready-enterprise/5298070) | 25.0 | 20.0 | 42.0 |
| [Cofenseが実際のフィッシング脅威に対する従業員の対応力を測定](https://www.helpnetsecurity.com/2026/09/23/cofense-command-center/) | 25.0 | 20.0 | 42.0 |
| [中国のユーザーが米国のAI地域制限を回避する80,000台のリレーサーバー](https://www.helpnetsecurity.com/2026/09/23/china-ai-relay-frontier-model-abuse/) | 25.0 | 20.0 | 42.0 |
| [Portnoxが管理対象デバイスから未承認のAIアプリケーションを検出・削除](https://www.helpnetsecurity.com/2026/09/23/portnox-shadow-ai-control-and-visibility/) | 25.0 | 20.0 | 42.0 |
| [Barracudaが小規模組織向けにAIセキュリティとガバナンスを提供](https://www.helpnetsecurity.com/2026/09/23/barracuda-ai-data-security/) | 25.0 | 20.0 | 42.0 |
| [Lookout、スマホ向けリアルタイム保護でスミッシング、音声クローン、ビッシングに対抗](https://www.helpnetsecurity.com/2026/09/23/lookout-unveils-social-engineering-protection/) | 25.0 | 20.0 | 42.0 |
| [偽のClaude Max配布を装ったGoogleアカウントのフィッシング詐欺](https://www.malwarebytes.com/blog/threat-intel/2026/09/fake-claude-max-giveaway-hides-a-google-account-phishing-trap) | 25.0 | 20.0 | 42.0 |
| [Honeywell: OTセキュリティチームはAIを受け入れるも、自律運用は依然として稀少](https://www.securityweek.com/honeywell-ot-security-teams-embrace-ai-but-autonomy-still-rare/) | 25.0 | 20.0 | 42.0 |
| [AI主導権確立に向けた大統領の使命](https://cyberscoop.com/president-ai-leadership-mission-critical-infrastructure-op-ed/) | 25.0 | 20.0 | 42.0 |
| [545人のハッカーが先に試した、今度はAI向けXRangesがセキュリティエージェントの安全性を評価する](https://thehackernews.com/2026/09/545-hackers-tested-it-first-now-xranges.html) | 25.0 | 20.0 | 42.0 |
| [AnthropicとOpenAIのモデルは安全性テストでなお制限された操作を試みる](https://thehackernews.com/2026/09/anthropic-and-openai-models-still.html) | 25.0 | 20.0 | 42.0 |
| [MicrosoftがEvilTokensのAI搭載フィッシングプラットフォームを阻止](https://www.securityweek.com/ai-powered-phishing-platform-eviltokens-disrupted-by-microsoft/) | 25.0 | 20.0 | 42.0 |
| [研究者が警鐘を鳴らすAI終末シナリオの考察](https://www.securityweek.com/a-look-at-ai-doomsday-scenarios-that-researchers-say-could-put-humanity-at-risk/) | 25.0 | 20.0 | 42.0 |
| [OuterlimitがAIエージェントの暴走による被害防止で1600万ドルを調達](https://www.securityweek.com/outerlimit-raises-16-million-to-stop-rogue-ai-agents-from-causing-harm/) | 25.0 | 20.0 | 42.0 |
| [Claude Opus 5.5、自律型AIのコスト削減と安全対策を強化](https://www.helpnetsecurity.com/2026/09/23/anthropic-claude-opus-5-5/) | 25.0 | 20.0 | 42.0 |
| [MemTensorのnpmおよびPyPIパッケージが認証情報窃取のサプライチェーン攻撃で侵害される](https://socket.dev/blog/memtensor-compromise) | 22.0 | 45.0 | 42.0 |
| [Adobe ConnectとAEM Formsの重大な脆弱性を修正](https://www.securityweek.com/adobe-patches-critical-flaws-in-connect-aem-forms/) | 22.0 | 32.0 | 42.0 |
| [Microsoft Defenderにおけるエージェント時代のSOC再構築](https://www.microsoft.com/en-us/security/blog/2026/09/23/reimagining-the-soc-for-the-agentic-era-in-microsoft-defender/) | 22.0 | 20.0 | 48.0 |
| [ShinyHuntersがPeopleSoftのゼロデイを悪用してFBIをハッキングしたと主張](https://www.infosecurity-magazine.com/news/shinyhunters-fbi-hack-peoplesoft/) | 22.0 | 20.0 | 43.0 |
| [「VeloCloud Orchestrator」に深刻な脆弱性 - すでに悪用も](https://www.security-next.com/190602) | 22.0 | 20.0 | 42.0 |
| [ShinyHuntersがFBI侵害は「虚偽」報告への報復と主張](https://www.malwarebytes.com/blog/news/2026/09/shinyhunters-claims-fbi-breach-was-revenge-for-false-report) | 20.0 | 20.0 | 48.0 |
| [FBI、サードパーティの求人ポータルに関連するサイバー攻撃を調査](https://www.cybersecuritydive.com/news/fbi-hack-shinyhunters-jobs-portal/831175/) | 20.0 | 20.0 | 42.0 |
| [Pentagonのサイバー責任者「需要が供給を大きく上回っている」](https://cyberscoop.com/pentagon-cyber-operations-demand-exceeds-supply-defensetalks-2026/) | 20.0 | 20.0 | 42.0 |
| [流出したGitLabのIssueメールアドレスにより、誰でもあなたとしてコードのプッシュやCIジョブの実行が可能に](https://thehackernews.com/2026/09/a-leaked-gitlab-issue-email-address.html) | 20.0 | 20.0 | 42.0 |
| [MikroTrickチェーンにより攻撃者がMikroTikルーターをパスワードやSSHキーなしで乗っ取れる脆弱性](https://thehackernews.com/2026/09/mikrotrick-chain-let-attackers-take.html) | 20.0 | 20.0 | 42.0 |
| [Hannibalが自律的な侵入テストを制御可能にする](https://www.praetorian.com/blog/autonomous-penetration-testing-hannibal/) | 20.0 | 20.0 | 42.0 |
| [UAEとサウジアラビア、複雑化するサイバー攻撃の猛攻に直面](https://www.darkreading.com/threat-intelligence/uae-saudi-arabia-face-onslaught-of-increasingly-sophisticated-automated-cyberattacks) | 20.0 | 20.0 | 42.0 |
| [Adobe製品の複数の脆弱性により任意のコードが実行される可能性](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-adobe-products-could-allow-for-arbitrary-code-execution_2026-099) | 20.0 | 20.0 | 42.0 |
| [Academic publisher ElsevierがLAPSUS$のリダイレクト攻撃を受ける](https://www.theregister.com/security/2026/09/23/academic-publisher-elsevier-hit-by-lapsus-redirect-attack/5298592) | 20.0 | 20.0 | 42.0 |
| [漏えいした多数のGitHub Appキーが現在も認証に利用可能な状態にある](https://www.infosecurity-magazine.com/news/hundreds-leaked-github-app-keys/) | 20.0 | 20.0 | 42.0 |
| [FBI、求人サイトへのShinyHuntersによる侵害疑惑を調査](https://therecord.media/fbi-investigating-alleged-shinyhunters-job-site-breach) | 20.0 | 20.0 | 42.0 |
| [産業界のリーダー、攻撃頻発で高まるサイバーレジリエンスの課題](https://www.cybersecuritydive.com/news/industrial-cyber-resilience-gap/831131/) | 20.0 | 20.0 | 42.0 |
| [1つのKubernetes YAMLでGCP組織が乗っ取られる可能性](https://www.bleepingcomputer.com/news/security/how-one-kubernetes-yaml-can-hand-over-a-gcp-organization/) | 20.0 | 20.0 | 42.0 |
| [動的アプリケーションセキュリティテストが実行時のリスクを検証する方法](https://www.rapid7.com/blog/post/em-dynamic-application-security-testing-dast-validates-risk-at-runtime-idc-marketscape) | 20.0 | 20.0 | 42.0 |
| [Network Solutionsのダークウェブ監視、ドメイン関連のデータ流出を中小企業に警告](https://www.helpnetsecurity.com/2026/09/23/network-solutions-dark-web-monitoring/) | 20.0 | 20.0 | 42.0 |
| [MicrosoftのFront Doorを悪用したOAuthトークン窃取](https://www.huntress.com/blog/stealing-oauth-tokens-through-microsofts-front-door) | 20.0 | 20.0 | 42.0 |
| [Microsoftが「EvilTokens」サイバー犯罪サービスを停止](https://www.itpro.com/security/cyber-crime/microsoft-takes-down-eviltokens-hacker-service-that-used-ai-to-decide-who-to-target-who-to-impersonate-and-how-to-most-effectively-exploit-victims) | 20.0 | 20.0 | 42.0 |
| [ラトビア当局、電子機器修理会社への侵害でハッカー容疑者を逮捕](https://therecord.media/latvia-hacker-arrest-cyberattack) | 20.0 | 20.0 | 42.0 |
| [cPanelの新たな脆弱性によりホスティングアカウントがroot権限でコードを実行し、サーバーを完全に制御可能に](https://thehackernews.com/2026/09/new-cpanel-flaw-lets-hosting-account_0272795595.html) | 20.0 | 20.0 | 42.0 |
| [OfcomがPornhubのAppleを活用した年齢確認を厳しく調査](https://www.theregister.com/security/2026/09/23/ofcom-takes-a-hard-look-at-pornhubs-apple-powered-age-checks/5298558) | 20.0 | 20.0 | 42.0 |
| [英国規制当局、PornhubのApple利用年齢確認を厳しく精査](https://www.theregister.com/security/2026/09/23/british-regulator-takes-a-hard-look-at-pornhubs-apple-powered-age-checks/5298558) | 20.0 | 20.0 | 42.0 |
| [Microsoft、9月のWindows更新でAlways On VPN接続に不具合](https://www.bleepingcomputer.com/news/microsoft/microsoft-september-2026-windows-updates-break-always-on-vpn-connections/) | 20.0 | 20.0 | 42.0 |
| [Chrome 154で108件の脆弱性を修正](https://www.securityweek.com/chrome-154-patches-108-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [GPT-6 SolとLunaの提供開始、API価格が50%低下](https://www.helpnetsecurity.com/2026/09/23/gpt-6-sol-luna-lower-api-prices/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、12,000件の受信トレイへのアクセスを犯罪者に提供していたEvilTokensのフィッシングサービスを停止](https://www.helpnetsecurity.com/2026/09/23/microsoft-eviltokens-phishing-service-disrupted/) | 20.0 | 20.0 | 42.0 |
| [EU監査人、情報共有の不足がサイバーインシデント対応を妨げていると警告](https://www.infosecurity-magazine.com/news/eu-auditors-slam-blocs-cyberinfo/) | 20.0 | 20.0 | 42.0 |

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
