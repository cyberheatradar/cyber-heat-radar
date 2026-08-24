# 📡 サイレーダー 2026-08-25 05:00 JST

このレポートは、2026-08-24 17:00 JST〜2026-08-25 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 86
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 58

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CISA orders urgent patching of actively exploited Zimbra flaw](#topic-29080) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [Tricky 'SynkLoader' Multitool May Herald Ransomware](#topic-29034) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [WordlistLoader Delivers Amatera via ClickFix, SynkLoader Phishes Windows Passwords](#topic-29058) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-29080"></a>

### 1. CISA orders urgent patching of actively exploited Zimbra flaw

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

CISAは、Zimbra Collaboration Suite（ZCS）に存在する、実際に悪用が確認されている脆弱性について、米政府機関に対し短期間での対応を求めました。
現時点で公表情報からは詳細な脆弱性の内容までは断定できませんが、悪用観測があるため、優先度の高い対応案件として扱われています。
公的機関が緊急対応を指示していることから、影響範囲やリスクが無視できない可能性があります。Zimbraを運用している組織では、同種のリスクが自組織にも及ぶ前提で確認が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Zimbra Collaboration Suiteの利用有無と対象バージョンを確認し、ベンダー告知に沿って速やかに修正を適用する。
- 外部公開しているZimbra関連機能がないか見直し、必要最小限の公開に絞る。
- 適用前後で不審なログや認証失敗、予期しない変更がないか確認し、検知・監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-73570 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Zimbra | 言及あり | 0.80 | — |
| 製品 | Zimbra Collaboration | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA orders urgent patching of actively exploited Zimbra flaw](https://www.bleepingcomputer.com/news/security/cisa-orders-urgent-patching-of-actively-exploited-zimbra-flaw/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-29034"></a>

### 2. Tricky 'SynkLoader' Multitool May Herald Ransomware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Dark Readingによると、「SynkLoader」と呼ばれる多機能マルウェアが確認されており、画面ハイジャックを使った認証情報の窃取など、複数の機能を備えているとされています。
現時点では、この活動がランサムウェアにつながる可能性が示唆されている段階で、詳細な被害範囲は明らかではありません。
多機能型のマルウェアは、初期侵入から情報窃取、後続のランサムウェア展開まで複数段階で悪用されるおそれがあります。
古い手口と新しい機能を組み合わせている点から、従来の検知や防御だけでは見落としが出る可能性があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 認証情報の保護を強化し、画面共有やリモート操作時の不審挙動を監視する。
- EDRやメール/ダウンロード経路の検知ルールを見直し、初期侵入の兆候を広く拾えるようにする。
- 多機能マルウェアを前提に、侵入後の横展開・権限昇格・バックアップ保護の確認を行う。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Tricky 'SynkLoader' Multitool May Herald Ransomware](https://www.darkreading.com/threat-intelligence/tricky-synkloader-multitool-ransomware) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-29058"></a>

### 3. WordlistLoader Delivers Amatera via ClickFix, SynkLoader Phishes Windows Passwords

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

研究者は、WordlistLoaderとSynkLoaderという新たなマルウェア系統が確認されたと報告しています。
WordlistLoaderはClearFake系のキャンペーンを通じてAmatera Stealerの配布に使われているとされ、SynkLoaderはWindowsの認証情報を狙うフィッシングに関与している可能性が指摘されています。
いずれも次段階のマルウェア展開や侵害後のアクセス悪用につながるおそれがあり、ランサムウェア関連の脅威動向として注意が必要です。
新しい配布手口や認証情報窃取の手口が示唆されており、利用者・運用者双方の警戒が求められます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 偽のCAPTCHAやクリック誘導を伴う不審なWebページ、広告、リダイレクトの監視を強化する。
- Windows端末での認証情報保護を見直し、特にブラウザ保存情報や資格情報の取り扱いを最小化する。
- 不審な添付・ダウンロード・ログイン要求に対する教育を継続し、侵害後の横展開を想定した検知を確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [WordlistLoader Delivers Amatera via ClickFix, SynkLoader Phishes Windows Passwor](https://thehackernews.com/2026/08/wordlistloader-delivers-amatera-via.html) | <nobr>内容確認・補足情報</nobr> |

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
| [Gunraランサムウェア：知っておくべきこと](https://www.fortra.com/blog/gunra-ransomware-what-you-need-know) | 28.0 | 30.0 | 42.0 |
| [ClickFixや偽ダウンロード キャンペーンにおけるPavinLoaderの追跡](https://www.malwarebytes.com/blog/threat-intel/2026/08/tracking-pavinloader-across-clickfix-and-fake-download-campaigns) | 28.0 | 20.0 | 48.0 |
| [偽のGTA 6拡張映像とデモサイトがインフォスティーラーを配布](https://www.malwarebytes.com/blog/threat-intel/2026/08/fake-gta-6-extended-look-and-demo-sites-deliver-an-infostealer) | 28.0 | 20.0 | 42.0 |
| [Google Sitesを使ってmacOSマルウェアを配布する偽Codexダウンロード](https://www.infosecurity-magazine.com/news/fake-codex-download-google-sites/) | 28.0 | 20.0 | 42.0 |
| [Android車載システムを感染させてプロキシボットネットを構築するハッカーたち](https://therecord.media/android-botnet-china-hackers) | 28.0 | 20.0 | 42.0 |
| [Operation QUICSILVERがミャンマー政府とITを標的にQUICAgentバックドアを使用](https://thehackernews.com/2026/08/operation-quicsilver-targets-myanmar.html) | 28.0 | 20.0 | 42.0 |
| [Apollo Globalのデータ侵害で個人情報が流出](https://www.securityweek.com/personal-information-exposed-in-apollo-global-data-breach/) | 28.0 | 20.0 | 42.0 |
| [内蔵ソフトウェア更新機能を通じてプロキシボットネットマルウェアに感染したAndroid車載ヘッドユニット](https://www.helpnetsecurity.com/2026/08/24/android-malware-car-head-unit-badbox/) | 28.0 | 20.0 | 42.0 |
| [ソフトクリエイト、国内初「Secure AI Productivity」Specializationを取得 AI活用支援を強化](https://ascii.jp/elem/000/004/428/4428852/?rss=) | 26.0 | 20.0 | 42.0 |
| [謎のAI「Ox Alpha」が出現し無料テスト中、コンテキストウィンドウは100万トークンで1日数兆トークンを処理できる匿名ラボがAPIを提供](https://gigazine.net/news/20260824-ox-alpha/) | 25.0 | 20.0 | 43.0 |
| [⚡ 週間総括：AI搭載PLC攻撃、GitLabへの攻撃、Stripeキー漏えいなど](https://thehackernews.com/2026/08/weekly-recap-ai-powered-plc-attacks.html) | 25.0 | 20.0 | 42.0 |
| [発見が修復を上回る脆弱性ギャップ](https://www.darkreading.com/cybersecurity-operations/vulnerability-gap-why-discovery-is-outrunning-repair) | 25.0 | 20.0 | 42.0 |
| [AIコードの増加に対してセキュリティをどう管理するか、リメディエーション負債の抑え方](https://thehackernews.com/2026/08/shipping-more-ai-code-than-you-can.html) | 25.0 | 20.0 | 42.0 |
| [サイバーセキュリティ職の求人広告で求められるAIスキルが1年で倍増](https://www.helpnetsecurity.com/2026/08/24/cybersecurity-job-ads-ai-skills-research/) | 25.0 | 20.0 | 42.0 |
| [AI利用者の5％が最大のセキュリティリスクとなる理由](https://thehackernews.com/2026/08/the-outsized-shadow-why-5-of-ai-users.html) | 25.0 | 20.0 | 42.0 |
| [AI時代におけるアプリケーションセキュリティの再考](https://www.securityweek.com/rethinking-application-security-for-the-ai-era/) | 25.0 | 20.0 | 42.0 |
| [OpenAIのCEO Sam Altman、AIが起業ブームを促すと予測](https://www.itpro.com/security/we-are-about-to-see-the-greatest-boom-in-people-starting-smaller-businesses-that-weve-ever-seen-openai-ceo-sam-altman-thinks-ai-will-spark-a-new-wave-of-entrepreneurship) | 25.0 | 20.0 | 42.0 |
| [UAT-10147がAIを活用してサーバー攻撃を拡大し、EDRバイパスとLinuxルートキットを備えたSPECTREを展開](https://thehackernews.com/2026/08/uat-10147-uses-ai-to-scale-server.html) | 25.0 | 20.0 | 42.0 |
| [Rapid7による分析: Microsoft SharePointのリモートコード実行（CVE-2026-63520）](https://www.rapid7.com/blog/post/ra-microsoft-sharepoint-remote-code-execution-cve-2026-63520) | 24.0 | 46.0 | 50.0 |
| [Keycloakの重大なパスワードリセット脆弱性で未認証攻撃者が任意のアカウントを乗っ取れる可能性](https://thehackernews.com/2026/08/critical-keycloak-password-reset-flaw.html) | 24.0 | 46.0 | 50.0 |
| [HackersがWordPressサイトを狙うminiOrangeの認証バイパス攻撃](https://www.bleepingcomputer.com/news/security/hackers-target-wordpress-sites-in-miniorange-auth-bypass-attacks/) | 24.0 | 38.0 | 42.0 |
| [メール送信サービスのアクセスキーを第三者が不正利用 - 衣料品会社](https://www.security-next.com/188144) | 22.0 | 20.0 | 42.0 |
| [設定変更で他利用者情報が閲覧可能に - レジャー予約サイト](https://www.security-next.com/188709) | 22.0 | 20.0 | 42.0 |
| [医療機器会社が手術室でのX線画像を保有、経緯を調査 - 金沢大病院](https://www.security-next.com/189121) | 22.0 | 20.0 | 42.0 |
| [土木情報サイト、パスワード含む会員情報流出の可能性](https://www.security-next.com/188700) | 22.0 | 20.0 | 42.0 |
| [米財務省、イラン人ハッカー疑惑の人物に制裁　「経済版Dデイ」の一環として](https://cyberscoop.com/us-treasury-sanctions-iranian-hackers-economic-dday/) | 20.0 | 20.0 | 42.0 |
| [超量子時代を見据えたエネルギー分野の備えを目指す超党派上院法案](https://cyberscoop.com/quantum-guard-act-electric-grid-cybersecurity/) | 20.0 | 20.0 | 42.0 |
| [米国から逃亡したインド人男性、高齢者から750万ドルをだまし取った詐欺に関与した疑いで逮捕](https://therecord.media/cyber-scam-indian-arrested) | 20.0 | 20.0 | 42.0 |
| [ReliaQuest、ShinyHuntersによる侵害を確認するも影響は限定的と発表](https://www.securityweek.com/reliaquest-confirms-shinyhunters-hack-but-says-impact-was-limited/) | 20.0 | 20.0 | 42.0 |
| [イラン関連のサイバー攻撃で英国の発電所が停止](https://www.theregister.com/security/2026/08/24/iran-linked-cyberattack-shut-down-a-uk-power-plant/5291930) | 20.0 | 20.0 | 42.0 |
| [量子安全なハードウェアの主張を検証するための新ガイダンス](https://www.infosecurity-magazine.com/news/guidance-verify-quantum-safe/) | 20.0 | 20.0 | 42.0 |
| [NISTが警告するマルチクラウド環境における特有のセキュリティリスク](https://www.infosecurity-magazine.com/news/nist-risks-multi-cloud/) | 20.0 | 20.0 | 42.0 |
| [ReliaQuest、ShinyHuntersによる侵害後のデータ窃取攻撃未遂を確認](https://www.bleepingcomputer.com/news/security/reliaquest-confirms-failed-data-theft-attack-after-shinyhunters-breach/) | 20.0 | 20.0 | 42.0 |
| [英国の発電施設が国家関与の疑いがあるサイバー攻撃で数日間停止](https://www.cybersecuritydive.com/news/uk-power-facility-disabled-Iran-cyberattack/828599/) | 20.0 | 20.0 | 42.0 |
| [悪意あるFirefoxアドオンが暗号資産ウォレットのシードフレーズとブラウザ認証情報を窃取](https://www.bitdefender.com/en-us/blog/hotforsecurity/malicious-firefox-add-ons-stealing-cryptowallet-seed-phrases-browser-credentials) | 20.0 | 20.0 | 42.0 |
| [偽のMicrosoftセキュリティスキャンで被害者にアンチウイルスのアンインストールを促す手口](https://www.malwarebytes.com/blog/threat-intel/2026/08/fake-microsoft-security-scans-trick-victims-into-uninstalling-their-antivirus) | 20.0 | 20.0 | 42.0 |
| [MITRE ATT&CK T1003.001における検知ギャップ](https://www.security.com/expert-perspectives/detection-gap-mitre-attck-t1003001) | 20.0 | 20.0 | 42.0 |
| [下院民主党がCISAの人員削減をGAOに調査要請](https://www.cybersecuritydive.com/news/cisa-workforce-cuts-congress-letter-gao-study/828596/) | 20.0 | 20.0 | 42.0 |
| [あなたが亡くなったとき、データはどうなるのか？（Lock and Code S07E17）](https://www.malwarebytes.com/blog/podcast/2026/08/your-data-doesnt-die-when-you-do-lock-and-code-s07e17) | 20.0 | 20.0 | 42.0 |
| [AliExpressが無音音声を使って訪問者のブラウザを識別していた問題](https://www.malwarebytes.com/blog/privacy/2026/08/aliexpress-caught-using-silent-audio-to-fingerprint-visitors-browsers) | 20.0 | 20.0 | 42.0 |
| [Microsoft Teamsで管理者が会議への外部ボットをブロック可能に](https://www.bleepingcomputer.com/news/security/microsoft-teams-now-lets-admins-block-external-bots-from-meetings/) | 20.0 | 20.0 | 42.0 |
| [韓国のスタートアップ向けプラットフォーム侵害で明らかになった鍵管理の不備](https://www.bleepingcomputer.com/news/security/south-korean-startup-platform-breach-exposes-key-management-failures/) | 20.0 | 20.0 | 42.0 |
| [採用時と評価時のズレ：CISOの本当の課題](https://www.securityweek.com/hired-for-one-job-judged-on-another-the-cisos-real-problem/) | 20.0 | 20.0 | 42.0 |
| [イラン関連とみられる攻撃で英国の発電所が数日間停止](https://www.helpnetsecurity.com/2026/08/24/uk-power-plant-cyberattack/) | 20.0 | 20.0 | 42.0 |
| [Doubloon DredgerがNotionを悪用して認証トークンを収集](https://www.infosecurity-magazine.com/news/doubloon-dredger-notion/) | 20.0 | 20.0 | 42.0 |
| [Uber、運転手アカウントの自動停止を巡りオランダ当局から約10億ドルの罰金](https://www.securityweek.com/uber-fined-nearly-1-billion-by-dutch-regulators-over-automated-suspensions-of-driver-accounts/) | 20.0 | 20.0 | 42.0 |
| [AliExpressが無音音声トリックで購入者の指紋採取を行ったと非難される問題](https://www.theregister.com/security/2026/08/24/aliexpress-accused-of-fingerprinting-shoppers-with-silent-audio-trick-that-also-muted-a-devs-headphones/5291662) | 20.0 | 20.0 | 42.0 |
| [Spring Application Frameworkで91件の脆弱性を修正](https://www.securityweek.com/91-vulnerabilities-patched-in-spring-application-framework/) | 20.0 | 20.0 | 42.0 |
| [研究者が数千件の有効なAWSアクセスキーの公開漏えいを警告](https://www.itpro.com/security/researchers-warn-thousands-of-active-aws-access-keys-are-publicly-exposed) | 20.0 | 20.0 | 42.0 |
| [ATMジャックポッティングでベネズエラ人に連邦刑務所で記録的な実刑判決](https://www.securityweek.com/venezuelan-gets-record-federal-prison-term-for-atm-jackpotting/) | 20.0 | 20.0 | 42.0 |
| [CISAのログ記録ガイダンスは政府以外にも有効](https://www.helpnetsecurity.com/2026/08/24/cybersecurity-logging-guidelines-strategy/) | 20.0 | 20.0 | 42.0 |
| [オーストラリアで販売される4ドルの紙製パスワード帳にセキュリティ専門家が支持](https://www.theregister.com/security/2026/08/24/security-vets-rally-around-4-paper-password-books-for-sale-in-australia/5291234) | 20.0 | 20.0 | 42.0 |
| [イランによる英国の発電所へのサイバー攻撃は「この国を支えるあらゆる組織にとって懸念すべき」ものだった](https://www.itpro.com/security/cyber-attacks/iranian-cyber-attack-on-uk-power-plant-should-concern-every-organization-responsible-for-keeping-this-country-running) | 20.0 | 20.0 | 42.0 |
| [イラン関連のハッカーが英国の発電所を4日間停止させる](https://www.securityweek.com/iran-linked-hackers-shut-down-uk-power-plant-for-four-days/) | 20.0 | 20.0 | 42.0 |
| [TikTok、子どものプライバシーを巡り米司法省と4億ドルで和解](https://www.securityweek.com/tiktok-reaches-400-million-settlement-with-us-justice-department-over-childrens-privacy/) | 20.0 | 20.0 | 42.0 |
| [イランの攻撃で英国の発電所が停止、CNIに警鐘](https://www.infosecurity-magazine.com/news/cni-iranian-attack-shuts-uk-power/) | 20.0 | 20.0 | 42.0 |
| [Salesforceがすべての組織に無償スキャナーを提供も、攻撃者はその見落としを把握している](https://www.cybersecuritydive.com/spons/salesforce-gave-every-org-the-same-free-scanner-attackers-already-know-wha/828063/) | 20.0 | 20.0 | 42.0 |
| [研究者が数千件の漏えいしたAWSキーを発見](https://www.infosecurity-magazine.com/news/researchers-thousands-eaked-aws/) | 20.0 | 20.0 | 42.0 |

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
