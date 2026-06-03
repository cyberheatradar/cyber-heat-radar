# 📡 サイレーダー 2026-06-04 05:00 JST

このレポートは、2026-06-03 17:00 JST〜2026-06-04 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 106
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 78

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-45247: CISA KEV catalog addition](#topic-14681) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 2 | [Acer working to patch max severity zero-days in Wave 7 routers](#topic-14687) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [TA4922: The Suspected Chinese Crime Group is Going Global](#topic-14647) | 35.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-14681"></a>

### 1. CVE-2026-45247: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

CISAは、CVE-2026-45247をKnown Exploited Vulnerabilities（KEV） Catalogに追加しました。
公開情報では、Mirasvit Full Page Cache Warmerにおける「信頼できないデータのデシリアライズ」に関する脆弱性で、実際の悪用が確認されたことを理由にしています。
KEV Catalogへの追加は、単なる未修正の脆弱性ではなく、実際の攻撃に使われている可能性が高いことを示します。
特に資産管理や脆弱性管理では、優先順位を上げて対応すべき対象になります。

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

- Mirasvit Full Page Cache Warmerを利用している環境がないか確認し、対象の有無を棚卸しする。
- 該当製品や関連コンポーネントの更新情報・ベンダー案内を確認し、速やかに適用可否を判断する。
- KEV掲載項目として、通常の脆弱性より高い優先度で検知・対応・監視の対象にする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-45247 | 主要CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-45247](https://nvd.nist.gov/vuln/detail/CVE-2026-45247) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/06/03/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・低信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-14687"></a>

### 2. Acer working to patch max severity zero-days in Wave 7 routers

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

AcerのWave 7メッシュルーターで、最大深刻度とされる2件のゼロデイ脆弱性への対応が進められているとされています。
現時点では詳細な技術情報は限られていますが、対象機器を利用している環境では、修正提供の有無や案内の確認が必要です。
ルーターはネットワーク境界に位置するため、脆弱性が放置されると家庭や拠点全体の通信に影響し得ます。ゼロデイかつ高深刻度とされる点から、パッチ公開前後の対応速度が重要になります。

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

- 対象モデルの利用有無を確認し、ベンダー告知と修正提供状況を継続監視する。
- 管理画面の露出範囲や外部公開設定を点検し、不要な公開を避ける。
- 修正が出た場合は、業務影響を見積もったうえで速やかに適用できる手順を準備する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Acer working to patch max severity zero-days in Wave 7 routers](https://www.bleepingcomputer.com/news/security/acer-warns-of-max-severity-zero-days-affecting-wave-7-routers/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 未確認。
- 開発者コミュニティ反応: 未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-14647"></a>

### 3. TA4922: The Suspected Chinese Crime Group is Going Global

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

TA4922と呼ばれる中国語圏の脅威グループが、主に日本を含むアジア圏から欧州・アフリカの一部へと対象地域を広げていると報告されています。
HR、給与、税務、請求書などのローカルな話題を装い、複数のマルウェアや正規ツールを組み合わせて配布している点が特徴です。
メールだけでなく、メッセージアプリやクラウド上のファイル共有、正規のリモート管理ツールまで悪用しており、従来の対策だけでは見落としが起きやすくなります。
対象地域や誘導文面が細かく作り分けられているため、組織ごとの注意喚起と検知強化が重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 人事・経理・税務を装うメールについて、添付ファイルや外部リンクの扱いを厳格化する。
- 正規ツールの悪用や不審なプロセス生成、テンポラリ領域からの実行を監視する。
- メール外の連絡手段へ誘導する不自然な指示（LINE、WhatsApp、Teams等）を警戒し、社内周知する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [TA4922: The Suspected Chinese Crime Group is Going Global](https://www.proofpoint.com/us/blog/threat-insight/ta4922-suspected-chinese-crime-group-going-global) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 反応あり・高信頼。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 未確認。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

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
| [ゼロデイの先へ：攻撃者の視点でネットワークを可視化するHD Mooreによるウェビナー](https://thehackernews.com/2026/06/beyond-zero-day-see-your-network-like.html) | 39.0 | 38.0 | 43.0 |
| [16人の数学者がAIの精度や信頼性など数学分野への潜在的な脅威について警告する「ライデン宣言」を発表](https://gigazine.net/news/20260603-leiden-declaration-on-ai-and-math/) | 29.0 | 20.0 | 42.0 |
| [なりすまし、クリックジャッキング、TDS：マルウェア配布エコシステムの内側](https://research.checkpoint.com/2026/impersonation-click-hijacking-and-tds-inside-a-malware-distribution-ecosystem/) | 28.0 | 20.0 | 48.0 |
| [詐欺師が構築中だった偽請求書キャンペーンを発見しました](https://www.malwarebytes.com/blog/threat-intel/2026/06/we-found-this-fake-invoice-campaign-while-scammers-were-still-building-it) | 28.0 | 20.0 | 42.0 |
| [KirkiとBurst StatisticsのWordPressプラグイン脆弱性が攻撃者の標的に](https://www.securityweek.com/kirki-burst-statistics-wordpress-plugin-flaws-in-attackers-crosshairs/) | 28.0 | 20.0 | 42.0 |
| [CIS SecureSuite Platformによるセキュリティ管理の簡素化](https://www.helpnetsecurity.com/2026/06/03/simplify-security-management-with-cis-securesuite-platform/) | 28.0 | 20.0 | 42.0 |
| [Minecraftユーザーを標的としたマルウェアキャンペーン、11万6000台超のシステムに感染](https://www.helpnetsecurity.com/2026/06/03/weedhack-minecraft-malware-campaign/) | 28.0 | 20.0 | 42.0 |
| [世界の証券取引所を狙った数か月にわたるメール攻撃キャンペーン](https://www.darkreading.com/cyberattacks-data-breaches/global-stock-exchange-hit-monthslong-email-campaign) | 28.0 | 20.0 | 42.0 |
| [5か月にわたり証券取引所幹部を標的にしたスパイ活動キャンペーン](https://www.security.com/threat-intelligence/stock-exchange-espionage) | 28.0 | 20.0 | 42.0 |
| [hentaiゲームに潜むArgamalマルウェア](https://securelist.com/argamal-rat-distributed-with-hentai-games/119999/) | 28.0 | 20.0 | 42.0 |
| [自律型AI駆動ワームが企業ネットワークを推論しながら侵入する](https://www.helpnetsecurity.com/2026/06/03/autonomous-ai-worm-prototype/) | 27.0 | 20.0 | 42.0 |
| [「使い物にならなくなった」──6月1日からの「GitHub Copilot」新料金、SNSで不満続出　他ツールへの移行表明も](https://www.itmedia.co.jp/news/articles/2606/03/news124.html) | 26.0 | 20.0 | 42.0 |
| [Coralogix、AIオブザーバビリティプラットフォーム拡大に向け2億ドルを調達、評価額は16億ドルに到達](https://www.securityweek.com/coralogix-raises-200m-at-1-6b-valuation-to-scale-ai-observability-platform/) | 25.0 | 20.0 | 42.0 |
| [WasmForgeへの入口：SliverをWebAssemblyにコンパイルする](https://www.praetorian.com/blog/wasmforge-sliver-webassembly/) | 25.0 | 20.0 | 42.0 |
| [「慌てるな」AIの現実を見極める動きが主要サイバーセキュリティ会議を席巻](https://www.cybersecuritydive.com/news/ai-cybersecurity-hype-reality-check-gartner/821867/) | 25.0 | 20.0 | 42.0 |
| [Microsoft、コード・AIエージェント・モデルが直面するセキュリティ課題に対応](https://www.helpnetsecurity.com/2026/06/03/microsoft-ai-agent-security-capabilities/) | 25.0 | 20.0 | 42.0 |
| [Infosecurity Europeで脆弱性管理イノベーターKonvuがCyber Startup Awardを受賞](https://www.infosecurity-magazine.com/news/konvu-wins-cyber-startup-award/) | 25.0 | 20.0 | 42.0 |
| [100のAIエージェントのセキュリティ評価と順位付け――知っておくべきこと](https://www.securityweek.com/security-of-100-ai-agents-tested-and-ranked-what-you-need-to-know/) | 25.0 | 20.0 | 42.0 |
| [悪意ある通知でGoogle Geminiユーザーをだます手口](https://www.darkreading.com/application-security/malicious-notifications-could-trick-google-gemini-users) | 25.0 | 20.0 | 42.0 |
| [AIワークロード向けのリアルタイムNodeBalancersメトリクス最適化](https://www.akamai.com/blog/cloud/2026/jun/optimize-ai-inference-nodebalancers-metrics-ai-workloads) | 25.0 | 20.0 | 42.0 |
| [本番環境のAIエージェントのうちセキュリティ基準を満たすのは11％のみ](https://www.helpnetsecurity.com/2026/06/03/research-ai-agent-security-capability/) | 25.0 | 20.0 | 42.0 |
| [Trump大統領、フロンティアAIモデルの自主的な審査を促す大統領令に署名](https://www.infosecurity-magazine.com/news/trump-eo-voluntary-frontier-ai/) | 25.0 | 20.0 | 42.0 |
| [Anthropic、Mythosの利用対象をさらに150組織に拡大](https://www.infosecurity-magazine.com/news/anthropic-glasswing-expansion/) | 25.0 | 20.0 | 42.0 |
| [Google、AIによるディープフェイク詐欺通話へのAndroid保護を追加](https://www.bleepingcomputer.com/news/security/google-adds-android-protection-against-ai-deepfake-scam-calls/) | 25.0 | 20.0 | 42.0 |
| [Infosecurity Europe: AIが数十年分の脆弱性を発見する中、パッチ対応の責任は依然として不明確なまま](https://www.infosecurity-magazine.com/news/patch-responsibility-ai-infosec/) | 25.0 | 20.0 | 42.0 |
| [Anthropic、Project Glasswingを15カ国以上の150組織に拡大](https://www.helpnetsecurity.com/2026/06/03/anthropic-project-glasswing-expansion/) | 25.0 | 20.0 | 42.0 |
| [Cisco Webex Meetingsのクロスサイトスクリプティング脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-webex-xss-jw3NeQzS) | 24.0 | 46.0 | 50.0 |
| [Cisco Unified Communications Managerのサーバーサイドリクエストフォージェリの脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-cucm-ssrf-cXPnHcW) | 24.0 | 46.0 | 50.0 |
| [Cisco Finesseのリモートファイルインクルージョン脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-finesse-rfi-gwpkdc89) | 24.0 | 46.0 | 50.0 |
| [CVE-2024-58266: Rust用shlexクレートにおけるコマンドインジェクションの脆弱性](https://nvd.nist.gov/vuln/detail/CVE-2024-58266) | 24.0 | 46.0 | 38.0 |
| [ロシアのハッカーがCRMを武器化しているとウクライナの元外相が警告](https://www.itpro.com/security/russian-hackers-are-weaponizing-crms-ukraines-former-foreign-minister-warns) | 22.0 | 20.0 | 43.0 |
| [ハッカーが世界の証券取引所を標的にしたスパイ活動](https://www.securityweek.com/hackers-target-global-stock-exchange-in-espionage-operation/) | 22.0 | 20.0 | 43.0 |
| [Microsoft、ゼロデイ公表への批判を受け法的懸念を沈静化へ](https://www.securityweek.com/microsoft-tries-to-calm-legal-threat-fears-after-zero-day-disclosure-backlash/) | 22.0 | 20.0 | 43.0 |
| [郵便物が所在わからず、原因は不明 - 日本郵便](https://www.security-next.com/185184) | 22.0 | 20.0 | 42.0 |
| [学校説明会の案内メールで誤送信 - サッカー総合専門学校](https://www.security-next.com/185276) | 22.0 | 20.0 | 42.0 |
| [宿泊予約サービスの口座情報が改ざん、不正送金被害 - ポラリスHD](https://www.security-next.com/185176) | 22.0 | 20.0 | 42.0 |
| [企業向け一斉送信メールに名簿ファイルを誤添付 - 沖縄県](https://www.security-next.com/184950) | 22.0 | 20.0 | 42.0 |
| [阿波銀行の情報漏えい、被害のテスト環境は「本来廃止すべきだった」 システム高度化作業でも利用](https://www.itmedia.co.jp/news/articles/2606/03/news138.html) | 21.0 | 20.0 | 42.0 |
| [Androidに122件の脆弱性、1件は標的型攻撃に悪用の可能性](https://news.mynavi.jp/techplus/article/20260603-4537001/) | 21.0 | 20.0 | 42.0 |
| [未修正のWindows Search URI脆弱性により攻撃者がNTLMv2ハッシュを窃取可能に](https://thehackernews.com/2026/06/unpatched-windows-search-uri.html) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-44777 jqの相互includeによるモジュール読み込み時のスタックオーバーフロー](https://nvd.nist.gov/vuln/detail/CVE-2026-44777) | 20.0 | 28.0 | 38.0 |
| [CVE-2026-33846 GnuTLS: DTLSハンドシェイク断片再構成におけるヒープバッファオーバーフローによるサービス拒否](https://nvd.nist.gov/vuln/detail/CVE-2026-33846) | 20.0 | 28.0 | 38.0 |
| [CVE-2025-55554: pytorch v2.8.0 の torch.nan_to_num-.long() に整数オーバーフローの脆弱性](https://nvd.nist.gov/vuln/detail/CVE-2025-55554) | 20.0 | 28.0 | 38.0 |
| [PyTorch v2.8.0のtorch.linalg.luにおけるスライス操作でDoSを引き起こされる脆弱性 (CVE-2025-55551)](https://nvd.nist.gov/vuln/detail/CVE-2025-55551) | 20.0 | 28.0 | 38.0 |
| [CVE-2025-5791 Usersでrootがグループ一覧に追加される問題](https://nvd.nist.gov/vuln/detail/CVE-2025-5791) | 20.0 | 28.0 | 38.0 |
| [CVE-2025-4574 Crossbeam-channelのdrop時におけるダブルフリー脆弱性](https://nvd.nist.gov/vuln/detail/CVE-2025-4574) | 20.0 | 28.0 | 38.0 |
| [CVE-2025-46327 Go Snowflake DriverのEasy Logging設定ファイルアクセス確認における競合状態問題](https://nvd.nist.gov/vuln/detail/CVE-2025-46327) | 20.0 | 28.0 | 38.0 |
| [BusyBox の tar における端末エスケープシーケンスを悪用したファイル名表示回避の脆弱性（CVE-2025-46394）](https://nvd.nist.gov/vuln/detail/CVE-2025-46394) | 20.0 | 28.0 | 38.0 |
| [BusyBoxのnetstatにおけるANSI端末エスケープシーケンスを含むargv[0]悪用によるサービス拒否の脆弱性（CVE-2024-58251）](https://nvd.nist.gov/vuln/detail/CVE-2024-58251) | 20.0 | 28.0 | 38.0 |
| [CVE-2025-1180 GNU Binutils ld elf-eh-frame.c の _bfd_elf_write_section_eh_frame におけるメモリ破損](https://nvd.nist.gov/vuln/detail/CVE-2025-1180) | 20.0 | 28.0 | 38.0 |
| [CVE-2025-1150 GNU Binutils ld libbfd.c の bfd_malloc におけるメモリリーク](https://nvd.nist.gov/vuln/detail/CVE-2025-1150) | 20.0 | 28.0 | 38.0 |
| [CVE-2025-1151: GNU Binutils ldのxmemdup.cにおけるメモリリーク](https://nvd.nist.gov/vuln/detail/CVE-2025-1151) | 20.0 | 28.0 | 38.0 |
| [CVE-2025-1152 GNU Binutils ldのxstrdup.cにおけるメモリリーク](https://nvd.nist.gov/vuln/detail/CVE-2025-1152) | 20.0 | 28.0 | 38.0 |
| [CVE-2024-30896: InfluxDB OSS 2.xにおいて管理者用オペレータートークンが既定組織に保存され、認可情報を閲覧できるユーザーにより取得可能になる脆弱性](https://nvd.nist.gov/vuln/detail/CVE-2024-30896) | 20.0 | 28.0 | 38.0 |
| [CVE-2019-11254 Kubernetes API Serverにおける悪意あるYAMLペイロードによるサービス拒否の脆弱性](https://nvd.nist.gov/vuln/detail/CVE-2019-11254) | 20.0 | 28.0 | 38.0 |
| [setuptools 0.7以前のeasy_installにおけるPyPI取得時のHTTP使用と整合性チェック不備によるMITM経由の任意コード実行脆弱性](https://nvd.nist.gov/vuln/detail/CVE-2013-1633) | 20.0 | 28.0 | 38.0 |
| [CVE-2023-1386 Qemu: 9pfsでファイル書き込み時にsuid/sgidビットが削除されない問題](https://nvd.nist.gov/vuln/detail/CVE-2023-1386) | 20.0 | 28.0 | 38.0 |
| [サイバー保険料は下がる一方で免責範囲が拡大している](https://www.darkreading.com/cyber-risk/cyber-insurance-rates-drop-exclusions-widen) | 20.0 | 20.0 | 42.0 |
| [新たな「HTTP/2 Bomb」DoS攻撃でWebサーバーが1分以内に停止](https://www.bleepingcomputer.com/news/security/new-http-2-bomb-dos-attack-crashes-web-servers-in-under-a-minute/) | 20.0 | 20.0 | 42.0 |
| [MDRアナリストの一日：現代のSOCの内部](https://www.rapid7.com/blog/post/it-day-in-the-life-mdr-analyst-inside-the-modern-soc) | 20.0 | 20.0 | 42.0 |
| [CISA、AndroidとLinuxの脆弱性を悪用する攻撃の活発化を警告](https://www.bleepingcomputer.com/news/security/cisa-warns-of-active-attacks-exploiting-android-linux-bugs/) | 20.0 | 20.0 | 42.0 |
| [CISAとFBI、産業用流体監視システムを標的とするハッカー集団に警告](https://www.cybersecuritydive.com/news/cisa-fbi-hackers-targeting-systems-monitor-industrial-fluits/821873/) | 20.0 | 20.0 | 42.0 |
| [銀行における345日間未検証の露出状態とは](https://www.bleepingcomputer.com/news/security/what-345-days-of-untested-exposure-looks-like-at-a-bank/) | 20.0 | 20.0 | 42.0 |
| [ワンクリックのGitHub Dev攻撃で攻撃者が完全なGitHub OAuthトークンを窃取可能に](https://thehackernews.com/2026/06/one-click-github-dev-attack-lets.html) | 20.0 | 20.0 | 42.0 |
| [怪しい番号から何度も着信？Scam Number Checkの紹介](https://www.malwarebytes.com/blog/product/2026/06/keep-getting-calls-from-questionable-numbers-meet-scam-number-check) | 20.0 | 20.0 | 42.0 |
| [IMA Diligence Servicesのデータ侵害で52万5000人に影響](https://www.securityweek.com/ima-diligence-services-data-breach-impacts-525000-people/) | 20.0 | 20.0 | 42.0 |
| [IVIPによるアイデンティティ可視化とインテリジェンスでIAMの攻撃対象領域を縮小する方法](https://thehackernews.com/2026/06/shrinking-iam-attack-surface-through.html) | 20.0 | 20.0 | 42.0 |
| [悪用が確認されたLinuxカーネルの脆弱性に関する組織への警告](https://www.securityweek.com/organizations-warned-of-exploited-linux-kernel-vulnerability/) | 20.0 | 20.0 | 42.0 |
| [HTTP/2 Bomb悪用でWebサーバーが数秒で停止](https://www.securityweek.com/http-2-bomb-exploit-knocks-web-servers-offline-in-seconds/) | 20.0 | 20.0 | 42.0 |
| [違法配信取り締まりで警察が9つの犯罪グループを摘発](https://www.bleepingcomputer.com/news/security/police-dismantles-9-crime-groups-in-illegal-streaming-crackdown/) | 20.0 | 20.0 | 42.0 |
| [Infosecurity Europe：取締役会にサイバーリスク定量化を優先させる方法](https://www.infosecurity-magazine.com/news/infosecurity-europe-board-cyber/) | 20.0 | 20.0 | 42.0 |
| [新たなサイバー軍創設には最大110億ドルの初期費用が必要と委員会が報告](https://therecord.media/new-cyber-force-would-cost-11-billion-commission) | 20.0 | 20.0 | 42.0 |
| [藤田医科大病院 患者情報漏えいか](https://news.yahoo.co.jp/pickup/6582816?source=rss) | 20.0 | 20.0 | 42.0 |
| [インフォスティーラーがフィッシングの主要なペイロードに台頭](https://www.malwarebytes.com/blog/threat-intel/2026/06/infostealers-are-becoming-the-go-to-phishing-payload) | 20.0 | 20.0 | 42.0 |
| [Google、連絡先を装う詐欺師を検知する静かなチェックを追加](https://www.helpnetsecurity.com/2026/06/03/android-fake-call-detection-feature/) | 20.0 | 20.0 | 42.0 |
| [HTTP/2の新たなBomb脆弱性によりNGINX、Apache、IIS、Envoy、CloudflareでリモートDoSが可能に](https://thehackernews.com/2026/06/new-http2-bomb-vulnerability-allows.html) | 20.0 | 20.0 | 42.0 |
| [Microsoft Scout agentが切り開く常時稼働型Autopilotの新たなカテゴリ](https://www.helpnetsecurity.com/2026/06/03/microsoft-scout-personal-agent/) | 20.0 | 20.0 | 42.0 |
| [Infosecurity EuropeでISACA専門家が警告、経営層はサイバー脅威を国家戦略と捉えるべき](https://www.infosecurity-magazine.com/news/execs-cisos-must-treat-cyber/) | 20.0 | 20.0 | 42.0 |

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
