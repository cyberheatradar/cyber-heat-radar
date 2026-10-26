# 📡 サイレーダー 2026-10-27 05:00 JST

このレポートは、2026-10-26 17:00 JST〜2026-10-27 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 96
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 68

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [PHP2Shell security flaws now sucessfully exploited in the wild](#topic-38753) | 56.0 | 74.0 | 67.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [Inside Node2Shell: A Closer Look at CVE-2026-111497](#topic-39379) | 37.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [Attackers Use Microsoft Teams IT Support Scams to Deploy Malware and Ransomware](#topic-39609) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-39379"></a>

### 1. Inside Node2Shell: A Closer Look at CVE-2026-111497

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

CVE-2026-111497は、Node.<wbr>jsに同梱されるBrotliデコーダーに関する脆弱性として報告されており、条件次第でメモリ破損やコード実行につながる可能性があるとされています。
関連する研究では、公式ビルド環境でも影響を受けうることが示され、複数のベンダーやプロジェクトが修正対応を進めています。
圧縮データの処理という広く使われる経路に関わるため、Node.<wbr>jsや関連製品を利用するサービスへの影響範囲が広がりやすい点が注目されています。
既に複数の製品・ベンダーが対策を取っていることから、依存関係を含めた確認が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 7 sources。
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

- Node.<wbr>jsやBrotliを利用するアプリケーションで、影響を受けるバージョンや同梱ライブラリの有無を確認する。
- HTTPレスポンスの自動展開など、外部入力をそのまま圧縮解除する経路がないか棚卸しする。
- ベンダーや配布元の修正版・緩和策を確認し、優先度を付けて更新を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-111497 | 関連CVE | 1.00 | 候補あり（URL 23件以上） |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| ベンダー | Wiz | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| マルウェア | ZLib | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-111497](https://nvd.nist.gov/vuln/detail/CVE-2026-111497) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-111497 Portfolio Status: Impact of Brotli Vulnerability (CVE-2026-11149](https://security.paloaltonetworks.com/CVE-2026-111497) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft releases emergency .<wbr>NET security fixes for Google Brotli bug](https://www.theregister.com/security/2026/10/26/microsoft-releases-emergency-net-security-fixes-for-google-brotli-bug/5305515) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP Issues Second Windows Security Update in Five Days to Fix Brotli Code Execut](https://thehackernews.com/2026/10/php-issues-second-windows-security.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-111497: Critical out-of-bounds write in the Node.<wbr>js Brotli decoder](https://www.rapid7.com/blog/post/etr-cve-2026-111497-critical-out-of-bounds-write-in-the-node-js-brotli-decoder) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Inside Node2Shell: A Closer Look at CVE-2026-111497](https://www.akamai.com/blog/security-research/2026/oct/inside-node2shell-closer-look-cve-2026-111497) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [BrotliのC言語実装における境界外書き込みの脆弱性（CVE-2026-111497）](https://jvn.jp/vu/JVNVU97400824/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Broccoli2shell: Everything You Need To Know About The Critical Brotli Decoder Vu](https://www.wiz.io/blog/cve-2026-111497-brotli-rce-node-js) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（2件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-39609"></a>

### 2. Attackers Use Microsoft Teams IT Support Scams to Deploy Malware and Ransomware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoft Teamsの外部チャット作成機能を悪用し、ITサポートを装うなりすましやマルウェア配布を行う攻撃手口が、複数の事例で繰り返し観測されていると報告されています。
こうした手口は、ランサムウェアにつながるケースも含まれており、単なる迷惑メッセージではなく侵害の入口として注目されています。
正規の業務ツールを起点にした社内外の信頼を悪用するため、ユーザーが警戒しにくく、初動対応の遅れにつながりやすい点が問題です。
組織内のコラボレーション基盤に対する運用・教育・監視の見直しが必要になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Teams上での外部ユーザーからの連絡やITサポート名乗りのメッセージに対する確認手順を明確にする。
- 不審な添付ファイル、リンク、認証要求があった場合の報告・遮断フローを整備する。
- 外部チャット機能の利用状況や不審なアカウント作成の兆候を監視対象に含める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft Teams | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Attackers Use Microsoft Teams IT Support Scams to Deploy Malware and Ransomware](https://thehackernews.com/2026/10/attackers-use-microsoft-teams-it.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-38753"></a>

### 1. PHP2Shell security flaws now sucessfully exploited in the wild

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 56.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

PHPの実行環境に存在する2件の脆弱性（CVE-2026-109618、CVE-2026-109619）が、実際に悪用されていると複数の情報源で報告されています。
いずれも認証なしのリモートコード実行につながる可能性があるとされ、WordPress、Drupal、Joomla などPHP上で動くWebアプリにも影響が及ぶおそれがあります。
公開PoCや悪用報告が出ているため、脆弱な環境では短期間で被害に結びつく可能性があります。PHPを利用する広範なシステムに関係しうるため、影響範囲が大きい点が注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 26 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- PHPの利用有無とバージョンを確認し、JPCERT/CCやベンダー案内に従って修正を適用する。
- 外部公開されたPHP実行環境や管理画面の監視を強化し、不審な要求や挙動を点検する。
- WordPress等のPHP आधारितアプリも含め、関連コンポーネント全体で影響確認を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-109618 | 関連CVE | 1.00 | 候補あり（URL 101件以上） |
| 脆弱性 | CVE-2026-109619 | 関連CVE | 1.00 | 候補あり（URL 14件以上） |
| 脆弱性 | CVE-2026-110264 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-114625 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-115560 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-109618](https://nvd.nist.gov/vuln/detail/CVE-2026-109618) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Millions of PHP Servers Face RCE Risk as PHP2Shell Exploitation Attempts Emerge](https://blog.polyswarm.io/millions-of-php-servers-face-rce-risk-as-php2shell-exploitation-attempts-emerge) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [26th October – Threat Intelligence Report](https://research.checkpoint.com/2026/26th-october-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP2Shell security flaws now sucessfully exploited in the wild](https://www.bleepingcomputer.com/news/security/php2shell-security-flaws-now-sucessfully-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: PHPにおける複数の脆弱性（CVE-2026-109618、CVE-2026-109619）に関する注意喚起  (更新)](https://www.jpcert.or.jp/at/2026/at260033.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-](https://security.paloaltonetworks.com/CVE-2026-109618) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [トレンドマイクロ、PHPの重大な脆弱性（PHP2Shell）への対応・支援策を発表](https://internet.watch.impress.co.jp/docs/news/2151086.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in PHP Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-php-october26-Jj384Daq) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（33件）。
- 国内開発者記事: 採用あり（1件）。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [953件のオンラインストアがJavaScriptを埋め込まれる被害、ほとんどがMagentoサイト](https://thehackernews.com/2026/10/hackers-infect-953-online-stores-with.html) | 28.0 | 20.0 | 42.0 |
| [UKのペンテスター「killa」がPHP2ShellのCapture the Flagコンテストで2000ドル相当のBitcoin賞金を獲得](https://www.theregister.com/security/2026/10/26/uk-pentester-killa-claims-2k-bitcoin-prize-in-php2shell-capture-the-flag-contest/5305429) | 28.0 | 20.0 | 42.0 |
| [Gheist攻撃者によるGitHubトークン悪用の試みが失敗](https://www.infosecurity-magazine.com/news/gheist-attackers-abuse-stolen/) | 28.0 | 20.0 | 42.0 |
| [953のオンラインストアが長期継続型マルウェア攻撃に感染](https://www.securityweek.com/953-online-stores-infected-in-long-lasting-malware-campaign/) | 28.0 | 20.0 | 42.0 |
| [Microsoft 365のトークンリプレイ攻撃で79組織の97アカウントが侵害された件](https://thehackernews.com/2026/10/microsoft-365-token-replay-attacks.html) | 28.0 | 20.0 | 42.0 |
| [AI熱狂の中でAnthropicがIPO申請へ、Trumpets blare and skies part](https://www.theregister.com/ai-and-ml/2026/10/26/trumpets-blare-and-skies-part-as-ai-hypefest-culminates-in-anthropic-ipo-filing/5305456) | 25.0 | 20.0 | 42.0 |
| [盗まれたAI推論が中国の安価な競合モデル構築を後押しする可能性](https://www.securityweek.com/stolen-ai-reasoning-could-help-china-build-cheaper-rivals/) | 25.0 | 20.0 | 42.0 |
| [Weekly Recap: This2Shell、That2Shell、あらゆるものがRCE？ Rogue AI、サプライチェーンの混乱など](https://thehackernews.com/2026/10/weekly-recap-this2shell-that2shell.html) | 25.0 | 20.0 | 42.0 |
| [AIエージェントがインシデントとなるとき、証拠はIDレコードにある](https://www.bleepingcomputer.com/news/security/when-an-ai-agent-is-the-incident-the-identity-record-is-the-evidence/) | 25.0 | 20.0 | 42.0 |
| [社員証を持つ従業員によるAIリスクが最大とみられる理由](https://www.helpnetsecurity.com/2026/10/26/ai-tools-security-worry-survey/) | 25.0 | 20.0 | 42.0 |
| [AI生成ハロウィーン動画であなたの写真は誰に渡るのか](https://www.malwarebytes.com/blog/ai/2026/10/ai-halloween-videos-whos-getting-your-photos) | 25.0 | 20.0 | 42.0 |
| [LiteLLMで失効していない鍵により攻撃者がユーザーを標的に可能になった問題](https://therecord.media/litellm-hackers-ai-malware) | 25.0 | 20.0 | 42.0 |
| [Downloadsフォルダに仕込まれた悪意ある指示に従ってしまうAIコーディングエージェント](https://www.helpnetsecurity.com/2026/10/26/ai-coding-agents-malware-openai-codex/) | 25.0 | 20.0 | 42.0 |
| [AIの助けで見つかったFortiOSの重大な脆弱性をFortinetが修正](https://www.helpnetsecurity.com/2026/10/26/fortinet-patches-critical-fortios-flaws-found-with-ai-help/) | 25.0 | 20.0 | 42.0 |
| [AIが生み出す脅威に対抗するため英国がAIへの大規模投資を表明](https://www.theregister.com/security/2026/10/26/britain-bets-big-on-ai-to-defend-against-the-threats-ai-is-helping-create/5305319) | 25.0 | 20.0 | 42.0 |
| [AnthropicがClaude Duetの暴走を防ぐ仕組みを詳述](https://www.helpnetsecurity.com/2026/10/26/anthropic-claude-duet-security-safeguards/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントを安全に導入する方法：Kaspersky製品がAI脅威をどう軽減するか](https://securelist.com/tr/how-to-secure-ai-agents/121444/) | 25.0 | 20.0 | 42.0 |
| [セキュリティを基盤とする現代のハイブリッド・ソブリン・アーキテクチャ](https://www.cybersecuritydive.com/spons/security-anchors-a-modern-hybrid-sovereign-architecture/833427/) | 25.0 | 20.0 | 42.0 |
| [メール配信システムで契約者情報が流出 - ラクスグループ会社](https://www.security-next.com/191846) | 22.0 | 20.0 | 42.0 |
| [荷物問合サービスの侵害、流出対象件数を取りまとめ - 佐川急便](https://www.security-next.com/191906) | 22.0 | 20.0 | 42.0 |
| [インターネットが脆弱な土台の上に成り立っていることとPHPocalypseへの備え不足](https://www.theregister.com/security/2026/10/26/we-shouldnt-be-surprised-about-the-phpocalypse-as-the-internet-is-built-on-sticks-and-glue/5305186) | 22.0 | 20.0 | 42.0 |
| [小中学校がPTAに生徒の個人情報を同意なしに提供 - 厚木市](https://www.security-next.com/191495) | 22.0 | 20.0 | 42.0 |
| [PHPの更新を適用していないサイトからビットコインを盗む賞金付きハッキングチャレンジが開催され19時間で突破される](https://gigazine.net/news/20261026-steal-my-bitcoin/) | 22.0 | 20.0 | 42.0 |
| [「PHP」にあらたな脆弱性、対象環境は限定的 - 次回更新時に修正](https://www.security-next.com/191902) | 22.0 | 20.0 | 42.0 |
| [口座解約に関する顧客情報が記録された記録媒体を紛失 - りそな銀](https://www.security-next.com/191783) | 22.0 | 20.0 | 42.0 |
| [NBA優勝記念リングを「無料プレゼント」と社員にメールするも実はフィッシング訓練で運営会社が謝罪](https://gigazine.net/news/20261026-nba-knicks-fake-offer/) | 22.0 | 20.0 | 42.0 |
| [ジョーシンへの不正アクセス、最大623万件漏えいか 運転免許証2件・マイナカード1件なども](https://www.itmedia.co.jp/news/article/2610/26/2000002601/) | 21.0 | 20.0 | 42.0 |
| [GMOが要請した「能動的サイバー防御」の論点、官房長官は対応明かさず](https://xtech.nikkei.com/atcl/nxt/column/18/00001/12127/) | 21.0 | 20.0 | 42.0 |
| [タイムズカー流出で顧客らが損害賠償求め運営会社提訴へ サイト開設の弁護士が記者会見](https://www.itmedia.co.jp/news/article/2610/26/2000002598/) | 21.0 | 20.0 | 42.0 |
| [野村総研、サイバー攻撃時の「能動的なシステム停止」を支援する新サービス](https://www.itmedia.co.jp/news/article/2610/26/2000002591/) | 21.0 | 20.0 | 42.0 |
| [普通のAIでも脆弱性を見つけられる今、企業にできる対策は？ Googleが15のポイントを解説](https://atmarkit.itmedia.co.jp/ait/articles/2610/26/news039.html) | 21.0 | 20.0 | 42.0 |
| [GheistがGitHubトークンを悪用してクラウドシークレットを窃取](https://www.darkreading.com/cyberattacks-data-breaches/gheist-stolen-github-tokens-cloud-secrets) | 20.0 | 45.0 | 42.0 |
| [Popcorn Timeの放置されたアップデーターにより数百万台のデバイスが乗っ取りの危険にさらされた](https://www.malwarebytes.com/blog/news/2026/10/popcorn-times-forgotten-updater-left-millions-of-devices-exposed-to-hijacking) | 20.0 | 28.0 | 50.0 |
| [CISAが今後4年間を見据えた戦略を公表](https://cyberscoop.com/cisa-2030-cybersecurity-strategy/) | 20.0 | 20.0 | 48.0 |
| [DreamHostが進行中の「incident」でパスワードリセットを強制](https://www.bleepingcomputer.com/news/security/dreamhost-forces-email-ftp-sftp-password-resets-in-ongoing-incident/) | 20.0 | 20.0 | 42.0 |
| [議員と人権団体、監視裁判所の意見書非公開は違法とトランプ政権を批判](https://cyberscoop.com/wyden-schiff-fisa-section-702-declassification/) | 20.0 | 20.0 | 42.0 |
| [当局、中国人被告を3,700万ドル投資詐欺容疑で送還](https://cyberscoop.com/chinese-national-extradited-investment-scam/) | 20.0 | 20.0 | 42.0 |
| [ISACAが会員を最新動向に追いつかせるために急ぐ取り組み](https://www.itpro.com/security/inside-isacas-race-to-help-its-members-stay-current) | 20.0 | 20.0 | 42.0 |
| [CISA 2030が重要インフラ向けに掲げる「積極的・先手を打つ」サイバー防衛戦略](https://www.infosecurity-magazine.com/news/cisa-aggressive-strategy-critical/) | 20.0 | 20.0 | 42.0 |
| [SECURITY.comポッドキャストで今も語り継がれる衝撃の瞬間](https://www.security.com/expert-perspectives/7-security-dot-com-podcast-moments-still-haunt-us) | 20.0 | 20.0 | 42.0 |
| [産業向けベンダーがPHP2Shell脆弱性を製品で確認](https://www.securityweek.com/industrial-vendors-check-products-for-php2shell-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [Genesysの侵害で内部システムから顧客データが流出](https://www.securityweek.com/genesys-hack-exposes-customer-data-from-internal-systems/) | 20.0 | 20.0 | 42.0 |
| [CISA、新戦略計画で先制的防御を約束](https://www.cybersecuritydive.com/news/cisa-strategic-plan-2030-infrastructure-partnerships/872750/) | 20.0 | 20.0 | 42.0 |
| [ウクライナ、Chinese製Dahua監視カメラの脆弱性を悪用するハッカーに警告](https://therecord.media/ukraine-cert-ua-warning-chinese-dahua-cameras-hacked) | 20.0 | 20.0 | 42.0 |
| [新幹線予約の個人情報17万件流出](https://news.yahoo.co.jp/pickup/6600235?source=rss) | 20.0 | 20.0 | 42.0 |
| [Linuxの脆弱性が修正前に露呈、root権限のエクスプロイトが公開される](https://www.infosecurity-magazine.com/news/linux-flaws-exposed-before-fixes/) | 20.0 | 20.0 | 42.0 |
| [未来250年に向けて構築された10のソフトウェアセキュリティ実践](https://www.darkreading.com/cyberattacks-data-breaches/10-software-security-practices-built-250-years) | 20.0 | 20.0 | 42.0 |
| [中国人男性、3600万ドルの仮想通貨詐欺への関与で身柄引き渡しへ](https://www.bleepingcomputer.com/news/security/chinese-man-extradited-for-role-in-36-million-cryptocurrency-scam/) | 20.0 | 20.0 | 42.0 |
| [PHP2Shellの悪用がプローブから実用的なシェルへ拡大](https://www.securityweek.com/php2shell-exploitation-moves-from-probes-to-working-shells/) | 20.0 | 20.0 | 42.0 |
| [Kali Linux 2026.3がkernel 7.1.5を搭載し、TicWatch Pro 3でwardrivingに対応](https://www.helpnetsecurity.com/2026/10/26/kali-linux-2026-3-released/) | 20.0 | 20.0 | 42.0 |
| [GitHub Actionsに対して今なお有効な攻撃手法とは](https://www.wiz.io/blog/github-actions-security-pwn-request-reckoning) | 20.0 | 20.0 | 42.0 |
| [Microsoft、重大な .<wbr>NET バッファオーバーフロー脆弱性に緊急パッチ更新を公開](https://www.infosecurity-magazine.com/news/microsoft-patch-update-net-flaw/) | 20.0 | 20.0 | 42.0 |
| [UK Biobank、Alibabaで50万人分のデータ販売未遂後にまもなくサービス再開へ](https://www.theregister.com/security/2026/10/26/uk-biobank-back-online-soon-months-after-someone-tried-to-sell-500k-peoples-data-on-alibaba/5305363) | 20.0 | 20.0 | 42.0 |
| [ユミルリンク、不正アクセスで情報漏えい件数を最大約5163万件と発表。対象が50システムに拡大 同社のドメインを悪用した迷惑メールにも注意喚起](https://internet.watch.impress.co.jp/docs/news/2151309.html) | 20.0 | 20.0 | 42.0 |
| [CISAが国家サイバー防衛と重要インフラ防御を強化する新戦略を発表](https://www.cisa.gov/news-events/news/cisa-unveils-new-strategy-strengthen-national-cyber-defense-and-critical-infrastructure-security) | 20.0 | 20.0 | 42.0 |
| [Wasmtimeの2件の重大な欠陥により悪意あるWebAssemblyモジュールがサンドボックスを突破する可能性](https://thehackernews.com/2026/10/two-critical-wasmtime-flaws-could-let.html) | 20.0 | 20.0 | 42.0 |
| [NFCリレー攻撃で銀行口座から40万ドル超を不正送金した容疑で2人をオランダ警察が逮捕](https://www.securityweek.com/dutch-police-arrest-two-over-nfc-relay-attacks-that-drained-400000/) | 20.0 | 20.0 | 42.0 |
| [楽天トラベルで2件の不正アクセス、海外ホテル予約サイト・多言語予約サイトで合計最大約350万件の個人情報が対象に](https://internet.watch.impress.co.jp/docs/news/2151305.html) | 20.0 | 20.0 | 42.0 |
| [Questの侵害で患者記録が流出：知っておくべきこと](https://www.malwarebytes.com/blog/data-breaches/2026/10/patient-records-exposed-in-quest-breach-what-you-need-to-know) | 20.0 | 20.0 | 42.0 |
| [アラートの間で攻撃者が通常の検知が見逃す隙間で行うこと](https://thehackernews.com/2026/10/between-alerts-what-attackers-do-in.html) | 20.0 | 20.0 | 42.0 |
| [GMOに攻撃 当初は約80億円要求](https://news.yahoo.co.jp/pickup/6600222?source=rss) | 20.0 | 20.0 | 42.0 |
| [Node2Shell: Brotliの脆弱性がMicrosoft、Node.<wbr>js、Pythonパッケージ全体で修正対応を促す](https://www.securityweek.com/node2shell-brotli-flaw-triggers-patching-across-microsoft-node-js-python-packages/) | 20.0 | 20.0 | 42.0 |
| [Blue Initiativeによる海事分野向け専用脆弱性データベースの提供](https://www.infosecurity-magazine.com/news/blue-initiative-maritime/) | 20.0 | 20.0 | 42.0 |
| [サイバー攻撃に緊急対策 首相方針](https://news.yahoo.co.jp/pickup/6600219?source=rss) | 20.0 | 20.0 | 42.0 |
| [Thales Imperva Cloud WAFの脆弱性情報](https://www.itpro.com/security/unified-threat-management/thales-imperva-cloud-waf-review-keeping-the-bad-actors-out-of-your-corporate-websites) | 20.0 | 20.0 | 42.0 |
| [Joshin 600万件超の情報漏えいか](https://news.yahoo.co.jp/pickup/6600214?source=rss) | 20.0 | 20.0 | 42.0 |
| [Ｊｏｓｈｉｎ、不正アクセスで最大約600万件の会員情報などが漏えいの可能性](https://internet.watch.impress.co.jp/docs/news/2151273.html) | 20.0 | 20.0 | 42.0 |
| [Mythos 5、7月の攻撃で実害を見逃す](https://www.securityweek.com/mythos-5-ignored-real-world-harm-in-july-attack/) | 20.0 | 20.0 | 42.0 |

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
