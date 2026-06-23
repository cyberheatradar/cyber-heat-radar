# 📡 サイレーダー 2026-06-24 05:00 JST

このレポートは、2026-06-23 17:00 JST〜2026-06-24 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 100
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 74

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CISA Adds Four Known Exploited Vulnerabilities to Catalog](#topic-18888) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [F5 launches AI Security Platform to uncover and secure shadow AI](#topic-18930) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-18888"></a>

### 1. CISA Adds Four Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、実際の悪用が確認されたとして、KEV Catalogに4件の脆弱性を新たに追加しました。
対象はLantronix EDS5000のコードインジェクション脆弱性と、Ubiquiti UniFi OSのアクセス制御不備、パストラバーサル、入力検証不備に関する3件です。
KEV Catalogへの追加は、当該脆弱性が実運用環境で悪用されている可能性を示すため、対応の優先度を上げる目安になります。
特に公開資産を持つ組織では、放置すると侵害リスクが高まるため注意が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 該当製品の利用有無を確認し、ベンダーの修正情報とCISAのKEV掲載状況を突き合わせる。
- 外部公開されている機器や管理画面を優先して点検し、更新が可能なら速やかに適用する。
- 更新前後を含め、侵害の痕跡がないかログや設定変更履歴を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-67038 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-34908 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-34909 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-34910 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Four Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/06/23/cisa-adds-four-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補あり（URL 1件以上 / 該当CVE 1件）。

---

<a id="topic-18930"></a>

### 2. F5 launches AI Security Platform to uncover and secure shadow AI

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

F5は、企業内のAIアプリケーション、モデル、エージェント、関連APIを継続的に可視化・統制・保護するための「F5 AI Security Platform」を発表しました。
あわせてSurePath AIの買収も発表されており、影のAIを含む企業のAI利用を把握しやすくする狙いがあるとされています。
AIの利用が部門ごとに広がる中で、把握されていないAIサービスや接続点が新たなリスクになり得るためです。
セキュリティとガバナンスを一体で扱う製品動向として、企業のAI運用設計に影響する可能性があります。

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

- 社内で許可されたAIサービスと、把握できていないAI利用の棚卸しを進める。
- AIモデル本体だけでなく、接続するAPIやデータ連携の管理方針を確認する。
- AI導入時の可視化、検証、保護を継続運用に組み込めるかを評価する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [F5 launches AI Security Platform to uncover and secure shadow AI](https://www.helpnetsecurity.com/2026/06/23/f5-launches-ai-security-platform-to-uncover-and-secure-shadow-ai/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
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
| [ダークウェブの内側：95セントで売られる盗まれたID、マルウェア、そして詐欺代行サービス](https://www.malwarebytes.com/blog/threat-intel/2026/06/inside-the-dark-web-stolen-identities-for-95%c2%a2-malware-and-scams-for-hire) | 28.0 | 20.0 | 48.0 |
| [macOSの新たなClickFix攻撃、DMGを静かにマウントして情報窃取型マルウェアを配布](https://www.bleepingcomputer.com/news/security/new-macos-clickfix-attack-silently-mounts-dmgs-to-push-infostealer/) | 28.0 | 20.0 | 42.0 |
| [「有給休暇を提供するフィッシング訓練」で職員の反発を招いたカナダの医療委員会、サイバー啓発キャンペーンの注意点を専門家が指摘](https://www.itpro.com/security/they-risk-damaging-confidence-a-canadian-health-board-outraged-staff-with-phishing-tests-offering-paid-leave-experts-say-shows-why-you-need-to-be-careful-with-cyber-awareness-campaigns) | 28.0 | 20.0 | 42.0 |
| [FortiGateファイアウォールを運用する組織にとってのFortibleedキャンペーンの意味](https://www.helpnetsecurity.com/2026/06/23/fortibleed-investigation-remediation/) | 28.0 | 20.0 | 42.0 |
| [FortiBleed攻撃でファイアウォールが認証情報窃取に悪用される、被害が継続](https://www.darkreading.com/cyberattacks-data-breaches/fortibleed-attackers-firewalls-credentials-stealers) | 28.0 | 20.0 | 42.0 |
| [FortiBleedキャンペーンの背後にいるロシアの初期アクセスブローカー](https://www.securityweek.com/russian-initial-access-broker-behind-fortibleed-campaign/) | 28.0 | 20.0 | 42.0 |
| [日常的なMicrosoft 365のワークフローに潜むフィッシング](https://www.helpnetsecurity.com/2026/06/23/microsoft-365-collaboration-features-phishing/) | 28.0 | 20.0 | 42.0 |
| [不動産業者がAIで加工した物件画像が賃貸探しを混乱させている](https://gigazine.net/news/20260623-generative-ai-impossible-homes/) | 27.0 | 20.0 | 42.0 |
| [メルカリ、ChatGPT上で商品検索から出品準備まで可能に 「Apps in ChatGPT」に公式アプリ](https://www.itmedia.co.jp/news/articles/2606/23/news134.html) | 26.0 | 20.0 | 42.0 |
| [日本IBM、AIファーストBPO拠点を北九州に新設--間接業務の変革と共創を加速](https://japan.zdnet.com/article/35249292/) | 26.0 | 20.0 | 42.0 |
| [リコージャパン、画像・図表も活用し社内ナレッジのAI活用を高度化--「RICOH デジタルバディ」](https://japan.zdnet.com/article/35249290/) | 26.0 | 20.0 | 42.0 |
| [Five Eyes各機関が警鐘を鳴らす、AIによるサイバーセキュリティへの脅威](https://therecord.media/five-eyes-alert-artificial-intelligence) | 25.0 | 20.0 | 42.0 |
| [Dragos、OTセキュリティ向けAIを発表](https://www.securityweek.com/dragos-unveils-ai-for-ot-security/) | 25.0 | 20.0 | 42.0 |
| [SIEMが統合セキュリティ運用へ向かう理由：Rapid7がIDC MarketScapeで主要ベンダーに選出](https://www.rapid7.com/blog/post/dr-siem-moving-toward-unified-security-operations-rapid7-named-idc-marketscape-major-player) | 25.0 | 20.0 | 42.0 |
| [Dify AIプラットフォームでデータ漏えいの不備、100万アプリに影響の可能性](https://www.securityweek.com/data-exposure-flaws-threaten-dify-ai-platform-powering-over-1-million-apps/) | 25.0 | 20.0 | 42.0 |
| [偽のAIエージェントスキルがセキュリティスキャンを通過し、26,000人のエージェントに到達したと報告される](https://thehackernews.com/2026/06/fake-ai-agent-skill-passed-security.html) | 25.0 | 20.0 | 42.0 |
| [Chatbotセキュリティにおける欠けている層としてのAI偵察](https://www.akamai.com/blog/security/2026/jun/ai-reconnaissance-missing-layer-chatbot-security) | 25.0 | 20.0 | 42.0 |
| [AIによって加速する脅威への対応には緊急のサイバーセキュリティ改善が必要とFive Eyes加盟国が警告](https://www.cybersecuritydive.com/news/ai-cyberattacks-five-eyes-frontier-models-warning/823526/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、Daybreakを拡充し防御側の脆弱性修正を支援](https://www.infosecurity-magazine.com/news/openai-daybreak-gpt-5-5-cyber/) | 25.0 | 20.0 | 42.0 |
| [N-ableの新機能、エンドポイントとネットワーク全体でのAI利用状況を可視化](https://www.helpnetsecurity.com/2026/06/23/n-able-shadow-ai-visibility/) | 25.0 | 20.0 | 42.0 |
| [Dragos、重要インフラ向けのOTネイティブAIを発表し脅威の優先順位付けを迅速化](https://www.helpnetsecurity.com/2026/06/23/dragos-unveils-ot-native-ai-to-help-critical-infrastructure-teams-prioritize-threats-faster/) | 25.0 | 20.0 | 42.0 |
| [Redditを使ってAI検索結果を操作するのは驚くほど簡単](https://www.helpnetsecurity.com/2026/06/23/reddit-ai-search-poisoning-research/) | 25.0 | 20.0 | 42.0 |
| [AI脅威への備え 第4の柱：脅威をリアルタイムで検知・封じ込める](https://www.wiz.io/blog/ai-threat-readiness-pillar-4) | 25.0 | 20.0 | 42.0 |
| [Agentic AI：もはや戦士を必要としない武器](https://thehackernews.com/2026/06/agentic-ai-weapon-that-no-longer-needs.html) | 25.0 | 20.0 | 42.0 |
| [OpenAI、サイバーセキュリティ対策を新規発見よりパッチ適用へ重点移行](https://www.securityweek.com/openai-refocuses-cybersecurity-efforts-on-patching-over-discovery/) | 25.0 | 20.0 | 42.0 |
| [Hack The Box、危機シミュレーションとSOCトレーニングを追加しサイバー対応力を強化](https://www.helpnetsecurity.com/2026/06/23/hack-the-box-expands-cyber-readiness-platform/) | 25.0 | 20.0 | 42.0 |
| [MavenirがNOCの知見を自動化し、自律型ネットワークを実現](https://www.helpnetsecurity.com/2026/06/23/mavenir-turns-noc-knowledge-into-automation-for-autonomous-networks/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、AIに脆弱性の発見だけでなく修正も担わせたい](https://www.helpnetsecurity.com/2026/06/23/openai-expanded-daybreak-cybersecurity-initiative/) | 25.0 | 20.0 | 42.0 |
| [Five Eyes諸国がフロンティアAIの脅威への緊急対応を要請](https://www.infosecurity-magazine.com/news/five-eyes-issues-urgent-call/) | 25.0 | 20.0 | 42.0 |
| [Hubbell Aclara Metrum Cellular Web Interfaceの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-174-07) | 24.0 | 46.0 | 50.0 |
| [ABB Freelanceのセキュリティロック](https://www.cisa.gov/news-events/ics-advisories/icsa-26-174-05) | 24.0 | 46.0 | 50.0 |
| [FFmpegのPixelSmash脆弱性によりVideo Player、Media Server、NAS ApplianceでRCEが可能に](https://www.securityweek.com/ffmpeg-pixelsmash-flaw-allows-rce-on-video-players-media-servers-nas-appliances/) | 24.0 | 38.0 | 42.0 |
| [アルジェリア人男性、サイバー犯罪マーケットプレイス運営で米国へ送還](https://www.securityweek.com/algerian-man-extradited-to-us-for-running-cybercrime-marketplaces/) | 22.0 | 20.0 | 43.0 |
| [サイトで障害、受注などに影響なし - 大阪有機化学工業](https://www.security-next.com/186133) | 22.0 | 20.0 | 42.0 |
| [個人情報含む警察発表を記者が個人SNSに投稿 - 苫小牧民報](https://www.security-next.com/186005) | 22.0 | 20.0 | 42.0 |
| [KDDIのISP向けメールシステム侵害 - 提供先6社に影響](https://www.security-next.com/186287) | 22.0 | 20.0 | 42.0 |
| [KDDI提供のISP向けメールシステムに不正アクセス、最大1422万件が漏洩か](https://xtech.nikkei.com/atcl/nxt/news/24/03272/) | 21.0 | 20.0 | 42.0 |
| [悪意あるnpmパッケージがPostCSSツールを装いWindows向けRATを配信](https://thehackernews.com/2026/06/malicious-npm-packages-pose-as-postcss.html) | 20.0 | 30.0 | 42.0 |
| [Mythosが発見したClinton政権時代から未検出だったメモリリーク「Squidbleed」](https://www.theregister.com/security/2026/06/23/mythos-discovers-squidbleed-a-memory-leak-thats-gone-undetected-since-clinton-era/5260367) | 20.0 | 28.0 | 50.0 |
| [Siemens SIPROTEC 5のDIGSI5プロトコル利用に関する脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-174-02) | 20.0 | 28.0 | 50.0 |
| [ポスト量子暗号EOは重要な節目、今こそ実装に取り組む時](https://blog.cloudflare.com/post-quantum-eo-2026/) | 20.0 | 20.0 | 48.0 |
| [アルジェリア人男性が2つのサイバー犯罪市場運営で起訴される](https://cyberscoop.com/algerian-man-charged-cybercrime-marketplaces/) | 20.0 | 20.0 | 48.0 |
| [Cordyceps：悪意あるプルリクエストの増殖が開発者のワークフローを脅かす](https://www.darkreading.com/application-security/cordyceps-malicious-pull-requests-developer-workflows) | 20.0 | 20.0 | 42.0 |
| [司法省、サイバー詐欺と犯罪マーケットプレイスに利用されたインフラを押収](https://cyberscoop.com/doj-huione-group-cybercrime-seizure/) | 20.0 | 20.0 | 42.0 |
| [東南アジア企業に関連するとみられるサイバー詐欺インフラをFedsが差し押さえ](https://therecord.media/feds-seize-alleged-cyber-scam-infrastructure-southeast-asia) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderのハッカー、裁判初日に有罪を認める](https://krebsonsecurity.com/2026/06/scattered-spider-hackers-plead-guilty-on-day-1-of-trial/) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderのメンバー、Transport for Londonへの不正アクセスで有罪を認める](https://www.bleepingcomputer.com/news/security/scattered-spider-members-plead-guilty-to-hacking-transport-for-london/) | 20.0 | 20.0 | 42.0 |
| [米下院指導部が児童のオンライン安全法案を公表、重要な欠落もあり](https://therecord.media/compromise-kids-online-safety-bill-unveiled-omission) | 20.0 | 20.0 | 42.0 |
| [Trump大統領令、連邦政府の耐量子暗号移行期限を2030年に設定](https://thehackernews.com/2026/06/trump-order-sets-2030-deadline-for.html) | 20.0 | 20.0 | 42.0 |
| [政府機関と契約業者に対する耐量子暗号導入の新期限をトランプ氏が設定](https://www.cybersecuritydive.com/news/quantum-cryptography-white-house-executive-order/823530/) | 20.0 | 20.0 | 42.0 |
| [Lookalike npmパッケージに隠された多段階Windows RAT](https://www.infosecurity-magazine.com/news/lookalike-npm-package-postcss/) | 20.0 | 20.0 | 42.0 |
| [GitHub、actions/checkoutを更新し一般的なPwn Request攻撃パターンを防止](https://thehackernews.com/2026/06/github-updates-actionscheckout-to-block.html) | 20.0 | 20.0 | 42.0 |
| [脆弱性は存在しなくても攻撃成立を証明する方法](https://www.bleepingcomputer.com/news/security/the-exploit-doesnt-exist-you-can-still-prove-it-works-against-you/) | 20.0 | 20.0 | 42.0 |
| [Trump、大統領令でポスト量子移行を迅速化](https://www.infosecurity-magazine.com/news/trump-eo-post-quantum-migration/) | 20.0 | 20.0 | 42.0 |
| [LastPass、Klueのサプライチェーン攻撃でデータ侵害を確認](https://www.bleepingcomputer.com/news/security/lastpass-confirms-data-breach-in-klue-supply-chain-attack/) | 20.0 | 20.0 | 42.0 |
| [SocGholishのテイクダウンが示す悪意あるTDSの脅威](https://www.darkreading.com/cyber-risk/socgholish-takedown-malicious-tds-threats) | 20.0 | 20.0 | 42.0 |
| [Meta、セキュリティレビュー後に物議を醸した従業員追跡プログラムを停止](https://www.malwarebytes.com/blog/news/2026/06/meta-pauses-controversial-employee-tracking-program-after-security-review) | 20.0 | 20.0 | 42.0 |
| [GTA 6の予約開始に乗じた詐欺が出現](https://www.infosecurity-magazine.com/news/gta-6-scams-emerge-as-preorders/) | 20.0 | 20.0 | 42.0 |
| [8年前のSamsung KNOXの脆弱性で数百万台のGalaxy端末がカーネル攻撃にさらされていた](https://www.securityweek.com/eight-year-old-samsung-knox-flaw-exposed-millions-of-galaxy-devices-to-kernel-attacks/) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderのメンバー2人がロンドンの交通機関を麻痺させたサイバー攻撃で有罪を認める](https://therecord.media/guilty-plea-tfl-cyberattack-scattered-spider-members) | 20.0 | 20.0 | 42.0 |
| [CISO対談：Deep InstinctのCISO兼CIOを務めるCarl Froggettの取り組み](https://www.securityweek.com/ciso-conversations-carl-froggett-combining-ciso-and-cio-at-deep-instinct/) | 20.0 | 20.0 | 42.0 |
| [ブラジルの全国アラートシステムが乗っ取られ、数百万台の携帯電話に「misanthropy」が送信される](https://www.bitdefender.com/en-us/blog/hotforsecurity/hacker-hijacks-brazils-national-alert-system) | 20.0 | 20.0 | 42.0 |
| [EvilTokens：「Ghost」コードが米欧企業を脅かす仕組み](https://any.run/cybersecurity-blog/eviltokens-ghost-code-analysis/) | 20.0 | 20.0 | 42.0 |
| [GTA 6早期アクセスを装う詐欺でゲーマーの暗号資産が狙われる](https://www.helpnetsecurity.com/2026/06/23/gta-6-early-access-scam/) | 20.0 | 20.0 | 42.0 |
| [ハッカーが300万人のテキサス州民のパスポートと運転免許証情報を窃取](https://www.malwarebytes.com/blog/data-breaches/2026/06/hackers-steal-passport-and-drivers-license-data-of-3-million-texans) | 20.0 | 20.0 | 42.0 |
| [NTTPC、レンタルサーバーサービス「WebARENA」における不正アクセスについて調査結果を発表](https://internet.watch.impress.co.jp/docs/news/2119429.html) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderの2人のハッカー、Transport for Londonへのサイバー攻撃で有罪を認める](https://www.helpnetsecurity.com/2026/06/23/transport-london-cyberattack-scattered-spider-members-plead-guilty/) | 20.0 | 20.0 | 42.0 |
| [TfLへのサイバー攻撃に関与したとして起訴された2人が、長期にわたる複雑な捜査の末に有罪を認める](https://www.itpro.com/security/cyber-attacks/duo-accused-of-role-in-tfl-cyber-attack-plead-guilty-after-lengthy-highly-complex-and-painstaking-investigation) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderのティーンエイジャーら、TfLへのサイバー攻撃で有罪判決](https://www.infosecurity-magazine.com/news/scattered-spider-teens-convicted/) | 20.0 | 20.0 | 42.0 |
| [カナダの電力会社London Hydroがデータ侵害を公表](https://www.securityweek.com/canadian-electricity-provider-london-hydro-discloses-data-breach/) | 20.0 | 20.0 | 42.0 |
| [Omada Identity Sovereign、欧州の高まるデジタル主権需要を狙う](https://www.helpnetsecurity.com/2026/06/23/omada-identity-sovereign-targets-europes-growing-digital-sovereignty-demands/) | 20.0 | 20.0 | 42.0 |
| [GTA 6早期アクセスは詐欺にすぎない](https://www.malwarebytes.com/blog/threat-intel/2026/06/gta-6-early-access-is-nothing-but-a-scam) | 20.0 | 20.0 | 42.0 |
| [Trumpが量子耐性暗号への移行を加速する大統領令に署名](https://www.securityweek.com/trump-signs-executive-order-accelerating-post-quantum-cryptography-migration/) | 20.0 | 20.0 | 42.0 |
| [KDDI 最大1422万件情報漏えいか](https://news.yahoo.co.jp/pickup/6585365?source=rss) | 20.0 | 20.0 | 42.0 |

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
