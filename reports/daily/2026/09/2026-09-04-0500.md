# 📡 サイレーダー 2026-09-04 05:00 JST

このレポートは、2026-09-03 17:00 JST〜2026-09-04 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 107
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 78

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Prolific Microsoft 0-day hunter drops CrowdStrike Falcon exploit PoC](#topic-30836) | 39.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [ランサム被害で店舗営業やサービスに影響 - REXT HD](#topic-30860) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-30836"></a>

### 1. Prolific Microsoft 0-day hunter drops CrowdStrike Falcon exploit PoC

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CrowdStrike Falconに関するエクスプロイトのPoCが共有されたとされ、Microsoft関連のゼロデイ研究者の動きとして注目されています。
材料上は「悪用観測あり」とされており、少なくとも概念実証の公開が話題の中心です。PoCの公開は、防御側にとって検知・緩和の見直しを急ぐサインになり得ます。
製品名が特定されているため、該当環境を使う組織は影響有無の確認が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- CrowdStrike Falconを利用している環境で、ベンダーの告知や更新情報を確認する。
- EDR/セキュリティ製品の検知・遮断設定や例外設定に不備がないか見直す。
- 関連する脆弱性情報が追加公開された場合に備え、資産棚卸しと適用優先度の確認を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | CrowdStrike | 言及あり | 0.80 | — |
| ベンダー | Kaspersky | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft Office | 言及あり | 0.80 | — |
| 製品 | Microsoft Windows | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Prolific Microsoft 0-day hunter drops CrowdStrike Falcon exploit PoC](https://www.theregister.com/security/2026/09/03/prolific-microsoft-0-day-hunter-drops-crowdstrike-falcon-exploit-poc/5294318) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-30860"></a>

### 2. ランサム被害で店舗営業やサービスに影響 - REXT HD

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | - |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

REXT Holdingsは、子会社REXTのシステムがサイバー攻撃を受けたと公表しました。
書籍やゲームの販売・買取を行う一部店舗では、臨時休業や営業時間の変更などの影響が出ています。店舗運営や対面サービスに直接影響が出ており、事業継続の観点で注目されます。
ランサムウェア被害として報じられており、復旧対応や顧客対応の進展が関心点です。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 店舗業務に直結するシステムの停止時に備え、代替運用や手作業手順を確認する。
- 営業時間変更や休業が発生した際の顧客案内を、迅速かつ一貫して出せる体制を整える。
- 感染拡大防止と復旧のため、関連システムの切り分け、バックアップ、外部連携先の確認を優先する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ランサム被害で店舗営業やサービスに影響 - REXT HD](https://www.security-next.com/188962) | <nobr>内容確認・補足情報</nobr> |

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
| [AI懐疑論者の予測はどれぐらい正確だったか？](https://gigazine.net/news/20260903-ai-skeptic-predictions/) | 29.0 | 20.0 | 42.0 |
| [SonicWall、連鎖する脆弱性への緊急パッチ適用を呼びかけ](https://www.cybersecuritydive.com/news/sonicwall-immediate-patching-chained-vulnerabilities/829567/) | 28.0 | 30.0 | 42.0 |
| [Node.<wbr>js: 古い手法が再び注目を集める](https://www.security.com/threat-intelligence/node-js-returns-ransomware) | 28.0 | 30.0 | 42.0 |
| [Pyramid Solutions NetStaX EtherNet/IP Stack の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-246-07) | 28.0 | 28.0 | 50.0 |
| [MetaとTikTokの広告経由で拡散するStreamRat Androidマルウェア](https://www.malwarebytes.com/blog/news/2026/09/streamrat-android-malware-spreads-through-meta-and-tiktok-ads) | 28.0 | 20.0 | 42.0 |
| [BraZetsuマルウェアが侵害したWindowsホストを犯罪マーケットの在庫に変える](https://thehackernews.com/2026/09/brazetsu-malware-turns-compromised.html) | 28.0 | 20.0 | 42.0 |
| [46か国に及ぶRMMフィッシングキャンペーンで米国が最大の標的に](https://thehackernews.com/2026/09/us-becomes-top-target-in-rmm-phishing.html) | 28.0 | 20.0 | 42.0 |
| [政府と業界が長期稼働していたSalityボットネットを停止](https://www.cybersecuritydive.com/news/doj-crowdstrike-botnet-sality-takedown/829512/) | 28.0 | 20.0 | 42.0 |
| [ロシア人男性、8万人のフリーランスにマルウェアを拡散したとして起訴](https://www.helpnetsecurity.com/2026/09/03/russian-national-indicted-freelance-platform-malware/) | 28.0 | 20.0 | 42.0 |
| [攻撃者が信頼されたNode.<wbr>jsランタイムをマルウェア配布ツールに転用、標的型攻撃で悪用](https://thehackernews.com/2026/09/attackers-turn-trusted-nodejs-runtime.html) | 28.0 | 20.0 | 42.0 |
| [国際合同作戦、Sality P2Pボットネットを壊滅](https://www.infosecurity-magazine.com/news/international-operation-disrupts/) | 28.0 | 20.0 | 42.0 |
| [Cisco IOS XR Software セキュリティ強化版リリース：2026年9月](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-hardening-iosxr-qg64NcM) | 27.0 | 46.0 | 51.0 |
| [AIプロンプトインジェクションからフィッシング回避へ広がるASCIIスミグリング](https://www.microsoft.com/en-us/security/blog/2026/09/03/ascii-smuggling-crosses-over-from-ai-prompt-injection-to-phishing-evasion/) | 27.0 | 20.0 | 42.0 |
| [Microsoft Officeの責任者が「AIが生成した質の低い文書」に対して苦言](https://gigazine.net/news/20260903-microsofts-office-ai/) | 27.0 | 20.0 | 42.0 |
| [日立、フィジカルAIの推進に向け「HMAX」ソリューションを拡充](https://japan.zdnet.com/article/35252261/) | 26.0 | 20.0 | 42.0 |
| [ニューヨーク市、公立校で生成AI利用を1年間禁止 8年生まで約60万人が対象](https://www.itmedia.co.jp/news/article/2609/03/2000001115/) | 26.0 | 20.0 | 42.0 |
| [オープンウェイトモデルがフロンティアモデルとの性能差を低コストで縮める：中国製の低価格AIモデルが米国ビッグテックに脅威となる可能性](https://www.itpro.com/security/open-weight-models-are-closing-the-capability-gap-with-frontier-models-at-a-fraction-of-the-cost-cheap-chinese-ai-models-could-spell-trouble-for-us-big-tech) | 25.0 | 20.0 | 42.0 |
| [OpenAIがChatGPTの障害を認め、Astraモデル発表を前に混乱](https://www.bleepingcomputer.com/news/artificial-intelligence/openai-confirms-chatgpt-is-down-ahead-of-astra-model-launch/) | 25.0 | 20.0 | 42.0 |
| [Anthropic、Claudeの障害を確認 複数モデルに影響](https://www.bleepingcomputer.com/news/artificial-intelligence/anthropic-confirms-claude-is-down-multiple-models-affected/) | 25.0 | 20.0 | 42.0 |
| [AI「機械速度」で2週間の攻撃が10時間に短縮](https://www.darkreading.com/cyberattacks-data-breaches/ai-machine-speed-2-week-attack-10-hours) | 25.0 | 20.0 | 42.0 |
| [GoogleのGemini 3.8 Flash、大型AIモデルに低コストで挑む](https://www.helpnetsecurity.com/2026/09/03/google-gemini-3-8-flash/) | 25.0 | 20.0 | 42.0 |
| [CREST、AI対応ペネトレーションテスト認定の第1期受講者を登録](https://www.infosecurity-magazine.com/news/crest-first-cohort-ai-pentesting/) | 25.0 | 20.0 | 42.0 |
| [HiddenLayerがAIランタイムセキュリティ向けに1億ドルを調達](https://www.securityweek.com/hiddenlayer-raises-100-million-for-ai-runtime-security/) | 25.0 | 20.0 | 42.0 |
| [AI Agent Firewallの新興企業AIR Securityがステルスを脱し5000万ドルを調達](https://www.securityweek.com/ai-agent-firewall-startup-air-security-emerges-from-stealth-with-50-million/) | 25.0 | 20.0 | 42.0 |
| [Shai-Huludの影響範囲が469件の認証情報保管先に拡大 それが意味するもの](https://thehackernews.com/2026/09/shai-huluds-reach-just-grew-to-469.html) | 25.0 | 20.0 | 42.0 |
| [「人気のある」AI活用事例は成果につながっていない、Gartnerは成功と手軽な成果のために基本に注力すべきと指摘](https://www.itpro.com/security/popular-ai-use-cases-arent-those-delivering-results-gartner-says-focus-on-the-basics-for-success-and-easy-wins) | 25.0 | 20.0 | 42.0 |
| [攻撃者がラテンアメリカの組織を標的にAIツールを継続使用していることが判明](https://unit42.paloaltonetworks.com/ai-tool-use-targeting-latam-orgs/) | 25.0 | 20.0 | 42.0 |
| [エンタープライズセキュリティ質問票におけるAgent Accessに関する質問への回答](https://securityboulevard.com/2026/09/agent-access-questions-on-the-enterprise-security-questionnaire-answered/) | 25.0 | 20.0 | 42.0 |
| [SCIM Agentプロビジョニング：主体が人間でない場合に起こる9つの失敗](https://securityboulevard.com/2026/09/scim-agent-provisioning-9-failures-when-the-principal-is-not-a-person/) | 25.0 | 20.0 | 42.0 |
| [Rockwell Automation ControlFLASH の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-246-03) | 24.0 | 46.0 | 50.0 |
| [IXON VPN Clientの脆弱性問題](https://www.cisa.gov/news-events/ics-advisories/icsa-26-246-02) | 24.0 | 46.0 | 50.0 |
| [300万件超のWordPressサイトに影響を与えるMigrationプラグインの脆弱性](https://www.securityweek.com/over-3-million-wordpress-sites-affected-by-migration-plugin-vulnerability/) | 24.0 | 46.0 | 50.0 |
| [HPEがArubaOS-CXのリモートコード実行の脆弱性を修正](https://www.bleepingcomputer.com/news/security/hpe-patches-critical-arubaos-cx-remote-code-execution-flaw/) | 24.0 | 38.0 | 42.0 |
| [Cisco、Secure Emailの未修正脆弱性と重大なSwitch脆弱性への対処を警告](https://www.securityweek.com/cisco-warns-of-unpatched-secure-email-flaws-patches-critical-switch-vulnerabilities/) | 24.0 | 38.0 | 42.0 |
| [インテリジェンスの裏にある物語](https://blog.talosintelligence.com/the-story-behind-the-intelligence/) | 22.0 | 20.0 | 42.0 |
| [BIツールから個人情報流出の可能性 - 2.5次元アイドル事務所](https://www.security-next.com/189031) | 22.0 | 20.0 | 42.0 |
| [レンタカーを借りた数時間後に自分の運転免許証がダークウェブで売りに出される](https://gigazine.net/news/20260903-rented-car-driver-license-sale/) | 22.0 | 20.0 | 42.0 |
| [大阪市の保育園サイトが改ざん - 個人情報流出は否定](https://www.security-next.com/189794) | 22.0 | 20.0 | 42.0 |
| [Rockwell Automation ArmorStart LTの脆弱性関連情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-246-04) | 21.0 | 34.0 | 50.0 |
| [“純金金貨”購入→中身は銅と鉄 田中貴金属やミキモトかたる偽サイトに注意 消費者庁](https://www.itmedia.co.jp/news/article/2609/03/2000001141/) | 21.0 | 20.0 | 42.0 |
| [トランプ政権「記事のAI学習は著作権侵害ではない」 OpenAIを支持する意見書、対New York Timesなどとの訴訟で](https://www.itmedia.co.jp/news/article/2609/03/2000001130/) | 21.0 | 20.0 | 42.0 |
| [Cisco Nexus 9000の重大な脆弱性により、認証不要のリモート攻撃者がroot権限でコード実行可能に](https://thehackernews.com/2026/09/critical-cisco-nexus-9000-flaw-lets.html) | 20.0 | 46.0 | 54.0 |
| [Inductive Automation Ignitionの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-246-06) | 20.0 | 28.0 | 50.0 |
| [OPCFoundation OPC UA LocalDiscoveryServer（LDS）の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-246-01) | 20.0 | 28.0 | 50.0 |
| [Tycon Systems TPDIN-Monitor-WEB3 の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-246-08) | 20.0 | 28.0 | 50.0 |
| [Rockwell Automation 1756-ENBTモジュール](https://www.cisa.gov/news-events/ics-advisories/icsa-26-246-05) | 20.0 | 28.0 | 50.0 |
| [CVEに追われる時代に答えを得るにはCTEMを試そう](https://www.theregister.com/security/2026/09/03/sponsored-drowning-in-cves-and-thirsty-for-answers-try-ctem/5293906) | 20.0 | 20.0 | 48.0 |
| [ThreatsDay: CEOフィッシングキット、5,000件のDropboxアカウント侵害、OAuthの罠とさらに17件の話題](https://thehackernews.com/2026/09/threatsday-ceo-phishing-kits-5k-dropbox.html) | 20.0 | 20.0 | 42.0 |
| [Manchester Airports Groupのデータ、身代金支払い拒否後に880万人分が流出](https://www.securityweek.com/manchester-airports-group-data-on-8-8-million-people-leaked-after-ransom-refusal/) | 20.0 | 20.0 | 42.0 |
| [PegasusのゼロクリックExploitがセルビアの学生活動家のiPhoneに感染](https://www.infosecurity-magazine.com/news/pegasus-zero-click-exploit/) | 20.0 | 20.0 | 42.0 |
| [Thomson ReutersのCourt Software侵害でSSNや封印データが流出した可能性](https://thehackernews.com/2026/09/thomson-reuters-court-software-breach.html) | 20.0 | 20.0 | 42.0 |
| [Outsider Phishing Kit、削除後も700件の新ページで存続](https://www.infosecurity-magazine.com/news/outsider-phishing-kit-survives/) | 20.0 | 20.0 | 42.0 |
| [従業員のパスワードがインフォスティーラーログに現れた場合の対応方法](https://www.bleepingcomputer.com/news/security/your-employees-password-appeared-in-an-infostealer-log-now-what/) | 20.0 | 20.0 | 42.0 |
| [Thomson Reutersが米国とカナダの裁判記録流出を公表](https://www.helpnetsecurity.com/2026/09/03/thomson-reuters-reveals-breach-that-exposed-u-s-and-canadian-court-records/) | 20.0 | 20.0 | 42.0 |
| [CybercrooksがFishbrainを狙ってパスワードハッシュを窃取](https://www.theregister.com/cyber-crime/2026/09/03/cybercrooks-trawl-fishbrain-to-net-password-hashes/5294158) | 20.0 | 20.0 | 42.0 |
| [ポスト量子時代に備えるための行動喚起](https://www.cisa.gov/resources-tools/resources/preparing-post-quantum-era-call-action) | 20.0 | 20.0 | 42.0 |
| [Cyber Brief 26-09 - 2026年8月版](https://cert.europa.eu/publications/threat-intelligence/cb26-09/) | 20.0 | 20.0 | 42.0 |
| [Thomson Reutersの侵害で米国とカナダの裁判所データが流出](https://therecord.media/thomson-reuters-cyberattack-data) | 20.0 | 20.0 | 42.0 |
| [米国とカナダの裁判記録がThomson Reutersのインシデント後に流出](https://www.infosecurity-magazine.com/news/us-canada-court-breach-thomson/) | 20.0 | 20.0 | 42.0 |
| [Plexがセキュリティ脆弱性の修正を直ちに適用するようユーザーに警告](https://www.bleepingcomputer.com/news/security/plex-warns-users-to-patch-security-vulnerabilities-immediately/) | 20.0 | 20.0 | 42.0 |
| [ダークウェブで1億5300万件の運転免許証画像が提供される](https://www.securityweek.com/153-million-driver-license-images-offered-on-dark-web/) | 20.0 | 20.0 | 42.0 |
| [サイバー保険を「無罪放免の切り札」と見なすべきではないと専門家が警告](https://www.itpro.com/security/security-experts-warn-cyber-insurance-should-not-be-treated-as-a-get-out-of-jail-free-card) | 20.0 | 20.0 | 42.0 |
| [Manchester Airports Groupへの攻撃：盗まれたデータが公開され、数百万人の旅行者に詐欺への警戒呼びかけ](https://www.itpro.com/security/data-breaches/manchester-airports-group-attack-millions-of-holidaymakers-urged-to-look-out-for-scams-as-hackers-publish-stolen-data-online) | 20.0 | 20.0 | 42.0 |
| [Dropbox侵害についてこれまでに判明していること](https://www.itpro.com/security/data-breaches/everything-we-know-about-the-dropbox-breach-so-far) | 20.0 | 20.0 | 42.0 |
| [FBI、1億5300万件の運転免許証情報流出の可能性を調査](https://www.infosecurity-magazine.com/news/fbi-probes-breach-153-million/) | 20.0 | 20.0 | 42.0 |
| [ホテル客室の隠しカメラ対策に使える7ドルのガジェットを研究者が開発](https://www.helpnetsecurity.com/2026/09/03/smartphone-hidden-camera-detector-sweepled/) | 20.0 | 20.0 | 42.0 |
| [UKのOnline Safety Actは「まったく効果がない」と子どもたちが語る](https://www.theregister.com/security/2026/09/03/uks-online-safety-act-has-made-absolutely-no-difference-kids-say/5293893) | 20.0 | 20.0 | 42.0 |
| [Release Notes: より迅速な脅威インテリジェンス調査、新たな脅威リサーチ、650件超の脅威カバレッジ更新](https://any.run/cybersecurity-blog/release-notes-august-2026/) | 20.0 | 20.0 | 42.0 |
| [SSOJet APIのエラーコード解説と再試行すべきでないケース](https://securityboulevard.com/2026/09/ssojet-api-error-codes-a-developer-reference-and-what-not-to-retry/) | 20.0 | 20.0 | 42.0 |
| [Java EEアプリにおけるエンタープライズSSO：ベンダーSDKなしでのOIDC実装](https://securityboulevard.com/2026/09/enterprise-sso-in-a-java-ee-app-oidc-without-a-vendor-sdk/) | 20.0 | 20.0 | 42.0 |
| [NGINX Plusを用いたエッジでのSSO：あらゆるバックエンド向けのOIDC](https://securityboulevard.com/2026/09/sso-at-the-edge-with-nginx-plus-oidc-for-any-backend/) | 20.0 | 20.0 | 42.0 |
| [Apacheのmod_auth_openidcを使ったSSO完全ガイド](https://securityboulevard.com/2026/09/sso-for-apache-with-mod_auth_openidc-a-complete-guide/) | 20.0 | 20.0 | 42.0 |
| [AndroidアプリにおけるEnterprise SSO：AppAuthとOIDCをステップごとに解説](https://securityboulevard.com/2026/09/enterprise-sso-in-an-android-app-appauth-and-oidc-step-by-step/) | 20.0 | 20.0 | 42.0 |
| [iOSアプリにおけるEnterprise SSO：AppAuthとOIDCのステップバイステップ解説](https://securityboulevard.com/2026/09/enterprise-sso-in-an-ios-app-appauth-and-oidc-step-by-step/) | 20.0 | 20.0 | 42.0 |
| [Angular アプリに Enterprise SSO を追加する方法（OIDC、ステップバイステップ）](https://securityboulevard.com/2026/09/how-to-add-enterprise-sso-to-an-angular-app-oidc-step-by-step/) | 20.0 | 20.0 | 42.0 |
| [VueアプリにエンタープライズSSOを追加する方法（OIDC、ステップバイステップ）](https://securityboulevard.com/2026/09/how-to-add-enterprise-sso-to-a-vue-app-oidc-step-by-step/) | 20.0 | 20.0 | 42.0 |
| [あなたのスマートフォンやパソコンが年齢確認を求めるようになるかもしれない](https://www.malwarebytes.com/blog/privacy/2026/09/your-phone-or-computer-may-soon-ask-how-old-you-are) | 20.0 | 20.0 | 42.0 |
| [Pegasusのゼロクリック型スパイウェア攻撃でセルビアの学生運動メンバーのiPhoneが感染](https://thehackernews.com/2026/09/pegasus-zero-click-spyware-exploit.html) | 20.0 | 20.0 | 42.0 |

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
