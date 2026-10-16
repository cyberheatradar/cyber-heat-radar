# 📡 サイレーダー 2026-10-17 05:00 JST

このレポートは、2026-10-16 17:00 JST〜2026-10-17 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 89
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 62

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Chinese APT Exploited BeyondTrust Vulnerability as Zero-Day](#topic-37930) | 51.0 | 46.0 | 59.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [Rapid7 Intelligence Wins the 2026 Péter Szőr Award for Outstanding Research](#topic-38026) | 35.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-38026"></a>

### 1. Rapid7 Intelligence Wins the 2026 Péter Szőr Award for Outstanding Research

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>通⁠信⁠基⁠盤</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Rapid7 Intelligenceの研究「BPFdoor in Telecom Networks: Sleeper Cells in the Backbone」が、2026年のPéter Szőr Awardを受賞しました。
対象となったのは、通信事業者の環境で長期にわたり潜伏する不正アクセスやLinux系のバックドアに関する技術研究です。
通信ネットワークは個人・企業・政府の通信基盤に直結するため、こうした潜伏型の脅威は影響が広がりやすいとみられます。
あわせて、研究成果が検知や防御の実務に活かされる点でも注目されています。

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

- 通信事業者やネットワーク境界のLinux環境で、長期潜伏や不審な永続化の兆候がないか点検する。
- BPFDoor関連を含むLinuxインプラントの検知ルールや監視ロジックを、既知の手口に固定せず更新する。
- CERTや脅威インテリジェンスの共有情報を継続的に確認し、関連する新しい亜種や運用手口の変化を追う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| マルウェア | BPFdoor | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Rapid7 Intelligence Wins the 2026 Péter Szőr Award for Outstanding Research](https://www.rapid7.com/blog/post/tr-rapid7-intelligence-wins-2026-peter-szor-award-outstanding-research) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-37930"></a>

### 1. Chinese APT Exploited BeyondTrust Vulnerability as Zero-Day

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>国⁠家⁠支⁠援</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 51.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

BeyondTrust Remote Supportに存在するCVE-2026-102764が、ゼロデイとして悪用されたと複数の報道で伝えられています。
関連する脅威グループは中国系のスパイ活動グループとされ、初期侵入やログ削除に使われた可能性が示されています。
リモートサポート製品は社内外の保守・運用に使われるため、侵害されると広い範囲に影響が及ぶおそれがあります。
ゼロデイでの悪用が確認されている点から、パッチ適用前のリスク評価と監視強化が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
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

- BeyondTrust Remote Supportの利用有無を確認し、該当バージョンや修正状況を直ちに点検する。
- 侵入痕跡だけでなく、認証・操作・ログ削除の不自然な兆候がないかを確認する。
- 関連する公開情報やベンダー通知を継続監視し、必要に応じてアクセス制御や監査設定を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-102764 | 関連CVE | 1.00 | 未確認 |
| ベンダー | BeyondTrust | 言及あり | 0.80 | — |
| 製品 | BeyondTrust Remote Support | 言及あり | 0.80 | — |
| ベンダー | Mandiant | 言及あり | 0.80 | — |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Ivanti | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-102764](https://nvd.nist.gov/vuln/detail/CVE-2026-102764) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Prolific Chinese espionage group exploits BeyondTrust zero-day](https://cyberscoop.com/china-espionage-attacks-beyondtrust-zero-day-armory-castle/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Chinese APT Exploited BeyondTrust Vulnerability as Zero-Day](https://www.securityweek.com/chinese-apt-exploited-beyondtrust-vulnerability-as-zero-day/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [China-Linked Hackers Exploited BeyondTrust Zero-Day to Take Over Remote Support ](https://thehackernews.com/2026/10/china-linked-hackers-exploited.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [China-nexus espionage actor targets BeyondTrust support tool in zero-day campaig](https://www.cybersecuritydive.com/news/china-espionage-beyondtrust-zero-day-hacker/833240/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Suspected Chinese espionage attackers abusing BeyondTrust IT support zero-day](https://therecord.media/beyond-trust-cyberattack-china) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [China Espionage Actor Actively Targeting Critical BeyondTrust Flaw, Google Warns](https://www.infosecurity-magazine.com/news/china-actor-beyondtrust-flaw-google/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [CISA、既知の悪用済み脆弱性2件をカタログに追加](https://www.cisa.gov/news-events/alerts/2026/10/16/cisa-adds-two-known-exploited-vulnerabilities-catalog) | 49.0 | 56.0 | 43.0 |
| [IDCFクラウド障害、194組織のデータが取り出し可能に 侵入経路は特定](https://xtech.nikkei.com/atcl/nxt/column/18/03790/101600006/) | 29.0 | 30.0 | 42.0 |
| [身代金要求の交渉人が敵側に通じていた場合](https://www.darkreading.com/cyber-risk/when-your-ransomware-negotiator-works-other-side) | 28.0 | 30.0 | 42.0 |
| [ボルチモア郊外自治体がランサムウェア被害主張後に8月のデータ侵害を確認](https://therecord.media/anne-arundel-county-maryland-confirms-data-breach) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア集団、支払い強要に物理的暴力の脅しを強める](https://www.infosecurity-magazine.com/news/ransomware-threats-physical/) | 28.0 | 30.0 | 42.0 |
| [中国系国家関連ハッカーが自動スキャンとサイバー諜報ツールで米国の重要インフラを標的にする](https://blog.polyswarm.io/chinese-state-linked-hackers-target-us-critical-infrastructure-with-automated-scanning-and-cyber-espionage-tools) | 28.0 | 20.0 | 42.0 |
| [UAT-11985が偽のイベント招待を使い台湾の研究関係者をGoogleのAitMフィッシングで標的にする](https://thehackernews.com/2026/10/uat-11985-uses-fake-event-invites-to.html) | 28.0 | 20.0 | 42.0 |
| [ICS-Sniper攻撃、XWormマルウェア運用者のハッキング、25万ドルのChromeエクスプロイト](https://www.securityweek.com/in-other-news-ics-sniper-attack-hacking-xworm-malware-operators-250k-chrome-exploit/) | 28.0 | 20.0 | 42.0 |
| [サイバー脅威アクターが選挙・選挙運動関係者を標的に多様な手法を使用](https://www.cisa.gov/resources-tools/resources/cyber-threat-actors-use-variety-techniques-target-election-and-campaign-officials) | 28.0 | 20.0 | 42.0 |
| [DORAにおけるTLPT要件の解説：脅威インテリジェンスの位置づけ](https://any.run/cybersecurity-blog/dora-tlpt-requirements-explained/) | 28.0 | 20.0 | 42.0 |
| [偽のArch Linux AURパッケージが টাইポを悪用してroot権限でマルウェアを実行](https://www.helpnetsecurity.com/2026/10/16/arch-linux-aur-malware-yay-paru/) | 28.0 | 20.0 | 42.0 |
| [Perplexityが安全な自律型AIエージェント構築支援のためサンドボックスプラットフォーム「SPACE」をオープンソース化](https://gigazine.net/news/20261016-perplexity-space/) | 27.0 | 20.0 | 42.0 |
| [Security Concerns Rise as Enterprise AI Enters Risk Management Phase](https://www.darkreading.com/cyber-risk/enterprise-ai-risk-management-phase-security-concerns-rise) | 25.0 | 20.0 | 42.0 |
| [AIが16分でロボットアームの制御を掌握](https://www.darkreading.com/ics-ot-security/ai-takes-control-robotic-arm-16-minutes) | 25.0 | 20.0 | 42.0 |
| [OpenAIの研究用モデルが許可なく第三者のテスト用ETHを使ってスマートコントラクトをデプロイした件](https://thehackernews.com/2026/10/openai-research-model-spent-3rd-party.html) | 25.0 | 20.0 | 42.0 |
| [職場で従業員が個人のChatGPTを使用している場合にIT管理者が取るべき対応](https://www.bleepingcomputer.com/news/security/employees-using-personal-chatgpt-at-work-heres-what-it-admins-need-to-do/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントが侵害を起こした場合、人間は責任を問われない可能性がある](https://www.darkreading.com/insider-threats/ai-agents-breaches-humans-liable) | 25.0 | 20.0 | 42.0 |
| [OpenAIが子どもの安全とデータ利用を巡って提訴される](https://www.malwarebytes.com/blog/ai/2026/10/openai-sued-over-children-safety-and-data-use) | 25.0 | 20.0 | 42.0 |
| [OpenAIモデルがデータポータルを攻撃し、暗号資産ウォレットを奪取してタスクを完了](https://www.securityweek.com/openai-models-hacked-data-portals-raided-a-crypto-wallet-to-finish-tasks/) | 25.0 | 20.0 | 42.0 |
| [AndroidにAI搭載の詐欺警告機能を追加、銀行になりすます相手との通話を自動終了](https://www.helpnetsecurity.com/2026/10/16/android-enhanced-built-in-scam-protection/) | 25.0 | 20.0 | 42.0 |
| [F5とJuniper Networksが深刻な脆弱性を修正](https://www.securityweek.com/f5-juniper-networks-patch-critical-vulnerabilities/) | 24.0 | 38.0 | 42.0 |
| [Researchers、OpenBSDのルート権限取得エクスプロイトを37年前の共有メモリの脆弱性連鎖で実証](https://thehackernews.com/2026/10/researchers-demonstrate-openbsd-root.html) | 22.0 | 20.0 | 42.0 |
| [エンタープライズ展開におけるオープンウェイトモデルのリスク管理](https://www.microsoft.com/en-us/security/blog/2026/10/16/managing-open-weight-model-risk-in-enterprise-deployments/) | 22.0 | 20.0 | 42.0 |
| [アプリ会員の個人情報が流出、詳細を調査 - バーガーキング](https://www.security-next.com/191546) | 22.0 | 20.0 | 42.0 |
| [個人情報が流出、顧客宛のなりすましメールに過去の注文情報 - ムーンスター](https://www.security-next.com/190996) | 22.0 | 20.0 | 42.0 |
| [ECアプリに不正アクセス、会員情報流出の可能性 - アエナ](https://www.security-next.com/191554) | 22.0 | 20.0 | 42.0 |
| [「XenServer」「Citrix UniconOS」など3製品に脆弱性 - 修正版を公開](https://www.security-next.com/191442) | 22.0 | 20.0 | 42.0 |
| [組織で相次ぐ情報流出、IPAが特別相談窓口 - 被害疑わしき段階でも相談可](https://www.security-next.com/191572) | 22.0 | 20.0 | 42.0 |
| [タイムズカー、退会後も7年間保管していた免許証画像を全削除へ 約660万アカウント分の漏えい受け](https://www.itmedia.co.jp/news/article/2610/16/2000002346/) | 21.0 | 20.0 | 42.0 |
| [コミックシーモア、会員のメールアドレスや生年月日など流出 件数は精査中](https://www.itmedia.co.jp/news/article/2610/16/2000002345/) | 21.0 | 20.0 | 42.0 |
| [タイムズカー、本人確認書類画像を10月末までに全削除 確認後に即時消去](https://xtech.nikkei.com/atcl/nxt/news/24/03428/) | 21.0 | 20.0 | 42.0 |
| [相次ぐ不正アクセス「実態解明進めなければならない」 警察庁長官、担当幹部会議で指示](https://www.itmedia.co.jp/news/article/2610/16/2000002341/) | 21.0 | 20.0 | 42.0 |
| [ファンケルとアテニア、計約83万件の会員情報漏えい ECサイトに不正アクセス](https://www.itmedia.co.jp/news/article/2610/16/2000002340/) | 21.0 | 20.0 | 42.0 |
| [ヤマト運輸、氏名や住所など計530万件超が漏えい 「クロネコ代金後払い」不正アクセスで](https://www.itmedia.co.jp/news/article/2610/16/2000002339/) | 21.0 | 20.0 | 42.0 |
| [キヤノンITS、SCS評価制度対応をワンストップ支援 診断から実装まで提供](https://news.mynavi.jp/techplus/article/20261016-5138987/) | 21.0 | 20.0 | 42.0 |
| [Unit 42が2026年9月に観測した初期侵入の脅威ベクトル上位5件](https://unit42.paloaltonetworks.com/top-5-initial-access-vectors-september-2026/) | 20.0 | 20.0 | 42.0 |
| [Targeted adsを悪用してCandiruのスパイウェアをゼロクリック攻撃で感染させる手口](https://www.bleepingcomputer.com/news/security/zero-click-attacks-used-targeted-ads-to-deliver-candiru-spyware/) | 20.0 | 20.0 | 42.0 |
| [AOMEI Backupperの更新サーバーが数分間改ざんされバックドアが配布された件](https://thehackernews.com/2026/10/attackers-tampered-with-aomei.html) | 20.0 | 20.0 | 42.0 |
| [2026年10月のWindows更新後のネットワーク障害、原因はNTLMかもしれない](https://www.theregister.com/security/2026/10/16/networking-problems-after-the-october-2026-windows-update-ntlm-might-be-to-blame/5303503) | 20.0 | 20.0 | 42.0 |
| [BAE Systemsのサイバーセキュリティインシデントで米国破産裁判所システムに障害](https://cyberscoop.com/bae-systems-cybersecurity-incident-us-bankruptcy-courts/) | 20.0 | 20.0 | 42.0 |
| [Proofpoint、Varonisのデータセキュリティ事業を63億ドルで買収へ](https://therecord.media/proofpoint-varonis-cybersecurity-acquisition) | 20.0 | 20.0 | 42.0 |
| [オープンソースセキュリティはリスクの把握と修正の拡大にかかっている](https://www.cybersecuritydive.com/news/open-source-software-vulnerabilities-analysis-scaling-ibm/833230/) | 20.0 | 20.0 | 42.0 |
| [Eilikoロボットコンパニオンでプライベートチャットが漏えいし乗っ取り可能に](https://www.malwarebytes.com/blog/ai/2026/10/eiliko-robot-companion-exposes-private-chats-and-can-be-hijacked) | 20.0 | 20.0 | 42.0 |
| [Ukraineとロシアの侵害に関与したとされるDataSuckersハッカーをモスクワ警察が拘束](https://therecord.media/russia-datasuckers-hackers-arrested) | 20.0 | 20.0 | 42.0 |
| [BAE管理システムへの攻撃で米国破産裁判所に障害発生](https://www.theregister.com/security/2026/10/16/attack-on-bae-managed-system-disrupts-us-bankruptcy-courts/5303487) | 20.0 | 20.0 | 42.0 |
| [Verified botsの継続的なアカウンタビリティ](https://blog.cloudflare.com/verified-bots-accountability/) | 20.0 | 20.0 | 42.0 |
| [流出個人情報を売買 闇サイト実態](https://news.yahoo.co.jp/pickup/6599033?source=rss) | 20.0 | 20.0 | 42.0 |
| [ハッカーが有望なビジネス機会を装うフィッシング攻撃](https://www.helpnetsecurity.com/2026/10/16/rfq-phishing-emails-sales-procurement-staff/) | 20.0 | 20.0 | 42.0 |
| [Burger King Japanのデータ侵害で1100万件の顧客情報が流出](https://www.bleepingcomputer.com/news/security/burger-king-japan-data-breach-exposes-11-million-customer-records/) | 20.0 | 20.0 | 42.0 |
| [Super Intelligenceの訓練・評価におけるインシデント対応準備と対応の主要実践方法](https://www.cisa.gov/resources-tools/resources/key-practices-incident-readiness-and-response-super-intelligence-training-and-evaluation) | 20.0 | 20.0 | 42.0 |
| [「スプレー・アンド・プレイ」式の求人応募で詐欺を見抜きにくくなる可能性](https://www.malwarebytes.com/blog/news/2026/10/spray-and-pray-job-applications-could-make-it-harder-for-you-to-spot-a-scam) | 20.0 | 20.0 | 42.0 |
| [BAE Systemsのセキュリティインシデントが米国破産裁判所の通知を遅延](https://www.securityweek.com/bae-systems-security-incident-stalls-notices-from-us-bankruptcy-courts/) | 20.0 | 20.0 | 42.0 |
| [2026年中間選挙を前に、詐欺師が候補者の声を複製して金銭や有権者情報を盗むとFBIが警告](https://www.helpnetsecurity.com/2026/10/16/usa-2026-midterm-election-scams/) | 20.0 | 20.0 | 42.0 |
| [Israeliデジタル広告代理店が野外で初確認されたゼロクリック型スパイウェアを配信していたことが判明](https://www.itpro.com/security/malware/israeli-digital-ad-agency-caught-serving-first-in-the-wild-zero-click-spyware) | 20.0 | 20.0 | 42.0 |
| [Metropolitan PoliceのShadow IT利用に対するICOの戒告](https://www.itpro.com/security/data-breaches/ico-reprimands-metropolitan-police-over-use-of-shadow-it) | 20.0 | 20.0 | 42.0 |
| [学校撮影者のSDカードを強奪するひったくり事件](https://www.theregister.com/security/2026/10/16/thief-snatches-school-snappers-sd-cards-in-smash-grab/5303379) | 20.0 | 20.0 | 42.0 |
| [BAE Systemsでのサイバーインシデントが米連邦破産通知業務を妨害](https://www.infosecurity-magazine.com/news/cyber-incident-bae-us-bankruptcy/) | 20.0 | 20.0 | 42.0 |
| [Microsoft: 10月のWindows更新でSmart App Controlが動作しなくなる可能性](https://www.bleepingcomputer.com/news/microsoft/kb5127648-windows-security-update-may-break-smart-app-control/) | 20.0 | 20.0 | 42.0 |
| [攻撃受け 県メアドから迷惑メール](https://news.yahoo.co.jp/pickup/6599003?source=rss) | 20.0 | 20.0 | 42.0 |
| [日経新聞 個人情報が183万件流出](https://news.yahoo.co.jp/pickup/6599004?source=rss) | 20.0 | 20.0 | 42.0 |
| [日経新聞社、クラウドサービスへの不正アクセスで約183万件の個人情報漏えい](https://internet.watch.impress.co.jp/docs/news/2148878.html) | 20.0 | 20.0 | 42.0 |
| [ヤマト運輸、「クロネコ代金後払いサービス」不正アクセスで約530万件の個人情報漏えい](https://internet.watch.impress.co.jp/docs/news/2148860.html) | 20.0 | 20.0 | 42.0 |

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
