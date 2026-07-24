# 📡 サイレーダー 2026-07-25 05:00 JST

このレポートは、2026-07-24 17:00 JST〜2026-07-25 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 74
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 46

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [In Other News: Dolphin X AI-Powered Malware, Car Anti-Theft Device Hack, 400 Linux Kernel Flaws](#topic-24224) | 41.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 2 | [Zero-day flaw in Check Point SmartConsole is under exploitation](#topic-24214) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Hermes AI agent used to automate attack on Thai Finance Ministry](#topic-24204) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-24224"></a>

### 1. In Other News: Dolphin X AI-Powered Malware, Car Anti-Theft Device Hack, 400 Linux Kernel Flaws

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報では、AIを悪用したとみられるマルウェアや、Linux kernelに関する多数の脆弱性など、複数のセキュリティ話題がまとめて取り上げられています。
あわせて、産業機器の脆弱性やメール製品を狙った諜報活動、ランサムウェアによる恐喝の話題も含まれており、幅広い領域で注意が必要な状況が示されています。
AIを含む新しい攻撃手法と、既存の基盤ソフトウェアや業務システムの脆弱性が同時に注目されているため、守るべき範囲が広いことを示しています。
実務では、単一製品だけでなく、端末・サーバー・産業機器まで含めた横断的な確認が必要になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Linux kernelや関連コンポーネントの脆弱性情報を確認し、影響範囲に応じて更新計画を見直す。
- メールやコラボレーション基盤について、侵害の兆候や不審な認証・アクセスの監視を強化する。
- AIを使った新種の脅威は断定しすぎず、検知ルール・EDR・ログ分析の見直しを進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Zimbra | 言及あり | 0.80 | — |
| 製品 | Linux kernel | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [In Other News: Dolphin X AI-Powered Malware, Car Anti-Theft Device Hack, 400 Lin](https://www.securityweek.com/in-other-news-dolphin-x-ai-powered-malware-car-anti-theft-device-hack-400-linux-kernel-flaws/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-24214"></a>

### 2. Zero-day flaw in Check Point SmartConsole is under exploitation

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Check PointのSmartConsoleにゼロデイ脆弱性があり、悪用が観測されていると報じられています。
研究者は、この問題により攻撃者がセキュリティ設定に重要な変更を加えられる可能性があると警告しています。
セキュリティ管理系の製品に関わる脆弱性であり、悪用されると防御設定そのものが影響を受けるおそれがあります。ゼロデイとして扱われているため、未対応環境では優先的な確認が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Check Point SmartConsoleの利用有無と適用状況を確認し、ベンダー情報を継続監視する。
- 管理者向けのアクセス権限や到達経路を見直し、不要な公開・露出がないか点検する。
- 設定変更や管理操作のログを確認し、不審な変更がないか監査を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-16232 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Check Point | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Zero-day flaw in Check Point SmartConsole is under exploitation](https://www.cybersecuritydive.com/news/zero-day-flaw-check-point-smartconsole-exploitation/826149/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-24204"></a>

### 3. Hermes AI agent used to automate attack on Thai Finance Ministry

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、脅威者がオープンソースのAIエージェント「Hermes」を、監視を最小化した自動実行モードで用い、タイ財務省への侵害が疑われる事案の後続作業を自動化したとされています。
AIを攻撃の一部に組み込む動きとして、運用の省力化や継続性の観点から注目されています。
生成AIやAIエージェントは防御側だけでなく攻撃側にも利用されうるため、実際の侵害でどう悪用され得るかを示す事例として重要です。
今後は、AIツールの安全な利用管理や、侵害後の不審な自動化挙動の検知がより課題になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIエージェントや自動化ツールの利用状況を把握し、想定外の実行モードや権限付与がないか確認する。
- 侵害後の横展開や情報収集を示す不自然な自動化挙動を監視し、通常業務の自動処理と区別できるようにする。
- AI関連ツールの導入時は、ログ取得、権限最小化、実行制御を前提に運用ルールを整備する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Hermes AI agent used to automate attack on Thai Finance Ministry](https://www.bleepingcomputer.com/news/security/hermes-ai-agent-used-to-automate-attack-on-thai-finance-ministry/) | <nobr>内容確認・補足情報</nobr> |

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
| [大学を標的としたランサムウェア攻撃の増加](https://www.infosecurity-magazine.com/news/university-ransomware-attacks-rise/) | 28.0 | 30.0 | 42.0 |
| [未修正のZimbraサーバーを悪用してメールを窃取するロシアのハッカー](https://www.helpnetsecurity.com/2026/07/24/laundry-bear-zimbra-vulnerability-cve-2025-66376/) | 28.0 | 20.0 | 48.0 |
| [Play Storeの外で広がるAndroid脅威の実態](https://www.malwarebytes.com/blog/inside-malwarebytes/2026/07/beyond-the-play-store-how-android-threats-really-spread) | 28.0 | 20.0 | 48.0 |
| [HOLLOWGRAPH：クラウドベースのスパイ活動の新たな姿](https://blog.polyswarm.io/hollowgraph-the-new-face-of-cloud-based-espionage) | 28.0 | 20.0 | 42.0 |
| [BlueNoroffのZoomフィッシングキット、マルウェア配信前に暗号資産ウォレットをプロファイル化](https://thehackernews.com/2026/07/bluenoroff-zoom-phishing-kit-profiles.html) | 28.0 | 20.0 | 42.0 |
| [更新されたサイバー脅威アクター命名システム](https://cloud.google.com/blog/topics/threat-intelligence/updated-cyber-threat-actor-naming-system/) | 28.0 | 20.0 | 42.0 |
| [ホテルのWi-Fiルーターが侵害され、訪問者の企業ログイン情報を窃取](https://www.infosecurity-magazine.com/news/hotel-wifi-dns-poisoning/) | 28.0 | 20.0 | 42.0 |
| [Golden Chickensが4つの新たなマルウェアファミリーとモジュール型インプラントで再登場](https://thehackernews.com/2026/07/golden-chickens-resurfaces-with-four.html) | 28.0 | 20.0 | 42.0 |
| [NCSCが企業を狙う「ゼロクリック」フィッシング攻撃に警告](https://www.itpro.com/security/phishing/ncsc-issues-alert-over-zero-click-phishing-campaign-hitting-enterprises) | 28.0 | 20.0 | 42.0 |
| [Google、開発者向けにパッチも自動生成するAIバグハンターを提供](https://www.helpnetsecurity.com/2026/07/24/google-codemender-ai-agent-code-security/) | 27.0 | 20.0 | 43.0 |
| [スーパーに並んだ「ごちゃごちゃ生成AIポップ」が物議 “看板王”こと、きぬた歯科院長「これはアリ」](https://www.itmedia.co.jp/news/articles/2607/24/news094.html) | 26.0 | 20.0 | 42.0 |
| [Microsoftやテック企業、オープンソースAIの普及を後押し](https://cyberscoop.com/tech-leaders-open-source-ai-cybersecurity/) | 25.0 | 20.0 | 42.0 |
| [OpenAIのエージェントがセキュリティテスト中にサンドボックスを脱出](https://www.malwarebytes.com/blog/news/2026/07/openais-agent-escaped-its-sandbox-during-a-security-test) | 25.0 | 20.0 | 42.0 |
| [最も脆弱なAI製品は、オンライン上で最も広く露出している製品でもある](https://www.cybersecuritydive.com/news/industrial-control-systems-ai-internet-exposure-censys-report-preview/826133/) | 25.0 | 20.0 | 42.0 |
| [生成AI利用経験者 24年度から倍増](https://news.yahoo.co.jp/pickup/6589191?source=rss) | 25.0 | 20.0 | 42.0 |
| [Slopsquatting、Phantom Domains、HalluSquattingは同一のAI攻撃](https://www.bleepingcomputer.com/news/security/slopsquatting-phantom-domains-and-hallusquatting-are-the-same-ai-attack/) | 25.0 | 20.0 | 42.0 |
| [Meta、AI生成アカウント対策でFacebookの無料認証バッジを導入](https://www.helpnetsecurity.com/2026/07/24/meta-facebook-verified-badge-selfie-verification/) | 25.0 | 20.0 | 42.0 |
| [AegisAI、AI搭載のメールセキュリティで3600万ドルを調達](https://www.securityweek.com/aegisai-raises-36-million-for-ai-powered-email-security/) | 25.0 | 20.0 | 42.0 |
| [ChatGPT Agentの脆弱性により、フィッシングリンク経由で不正なWorkspaceエージェントが展開される可能性](https://thehackernews.com/2026/07/chatgpt-agentforger-flaw-could-deploy.html) | 25.0 | 20.0 | 42.0 |
| [AIエージェントを見守るだけでは不十分、セキュリティチームは実行可能な行動を制御すべき](https://thehackernews.com/2026/07/seeing-ai-agents-is-not-enough-security.html) | 25.0 | 20.0 | 42.0 |
| [OpenAIモデルによるHugging Faceハッキングへの業界の反応とフィードバックフライデー](https://www.securityweek.com/industry-reactions-to-openai-models-hacking-hugging-face-feedback-friday/) | 25.0 | 20.0 | 42.0 |
| [ChatGPTがフィッシング攻撃で最もなりすましされるブランド上位10位入り、Check Pointが報告](https://www.infosecurity-magazine.com/news/chatgpt-most-impersonated-brands/) | 25.0 | 20.0 | 42.0 |
| [HackerがThai Finance MinistryでHermes AI Agentを無人運用し、侵害後の活動を実施](https://thehackernews.com/2026/07/hacker-runs-hermes-ai-agent-unattended.html) | 25.0 | 20.0 | 42.0 |
| [ふるさと納税寄付者向けのメールに他寄付者の個人情報 - 太田市](https://www.security-next.com/187307) | 22.0 | 20.0 | 42.0 |
| [従業員リスト持出、再就職先の侵害調査から発覚 - あすか製薬](https://www.security-next.com/187604) | 22.0 | 20.0 | 42.0 |
| [アンケートフォームで不備、個人情報が閲覧可能に - 関市](https://www.security-next.com/187608) | 22.0 | 20.0 | 42.0 |
| [「ManageEngine ADAudit Plus」に脆弱性 - 4月に修正実施](https://www.security-next.com/187840) | 22.0 | 20.0 | 42.0 |
| [「BIND 9」にキャッシュ汚染など複数脆弱性 - 修正版を公開](https://www.security-next.com/187829) | 22.0 | 20.0 | 42.0 |
| [「LINE広告」の一部記録など約3年半分を誤って削除 LINEヤフー](https://www.itmedia.co.jp/news/articles/2607/24/news096.html) | 21.0 | 20.0 | 42.0 |
| [Bing Imagesの脆弱性により、細工されたSVGでMicrosoftサーバー上でSYSTEM権限のコマンド実行が可能に](https://thehackernews.com/2026/07/bing-images-flaws-let-crafted-svgs-run.html) | 20.0 | 28.0 | 50.0 |
| [ハッカーがホテルのWi-FiのDNSを乗っ取りMicrosoft 365アカウントを窃取](https://www.bleepingcomputer.com/news/security/hackers-hijack-hotel-wi-fi-dns-to-steal-microsoft-365-accounts/) | 20.0 | 20.0 | 42.0 |
| [Andy Burnham、英国のサイバー政策継続を示唆し、省廃止後も大臣を再任](https://therecord.media/andy-burnham-liz-lloyd-cyber-policy-uk) | 20.0 | 20.0 | 42.0 |
| [暗号資産保有者を狙った「Wrench」攻撃が増加か](https://therecord.media/wrench-attacks-against-cryptocurrency-holders) | 20.0 | 20.0 | 42.0 |
| [TikTokのレジンアート詐欺にだまされないで](https://www.malwarebytes.com/blog/scams/2026/07/dont-get-fooled-by-tiktok-resin-art-scams) | 20.0 | 20.0 | 42.0 |
| [Call of Duty Mobileで無料ポイントを装う詐欺、プレイヤーアカウントを窃取](https://www.malwarebytes.com/blog/threat-intel/2026/07/call-of-duty-mobile-scam-uses-fake-free-points-to-steal-player-accounts) | 20.0 | 20.0 | 42.0 |
| [Certighostの脆弱性により低権限のActive Directoryユーザーがドメインコントローラーを偽装可能に](https://thehackernews.com/2026/07/certighost-exploit-lets-low-privileged.html) | 20.0 | 20.0 | 42.0 |
| [Chick-fil-Aのデータ侵害で1万3000人超の顧客に影響](https://www.bleepingcomputer.com/news/security/chick-fil-a-data-breach-affects-more-than-13-000-customers/) | 20.0 | 20.0 | 42.0 |
| [Googleが顔の自撮り動画を保存したい理由](https://www.malwarebytes.com/blog/privacy/2026/07/google-wants-to-store-a-selfie-video-of-your-face) | 20.0 | 20.0 | 42.0 |
| [Vatican公式祈祷アプリで70万人超の個人情報が漏えい](https://www.darkreading.com/vulnerabilities-threats/vatican-official-prayer-app-leaks-700k-pii) | 20.0 | 20.0 | 42.0 |
| [Europolが「The Com」摘発で4,340件のURL削除を要請](https://www.bleepingcomputer.com/news/security/europol-flags-4-340-urls-for-removal-in-the-com-crackdown/) | 20.0 | 20.0 | 42.0 |
| [Azure Automationの既定設定によりクロステナントID乗っ取りが可能に](https://www.darkreading.com/cloud-security/default-azure-automation-setting-cross-tenant-identity-takeover) | 20.0 | 20.0 | 42.0 |
| [米国、海外のサイバー犯罪者にビザ取消を通告](https://www.theregister.com/security/2026/07/24/uncle-sam-tells-overseas-cybercrooks-their-visas-are-canceled/5278212) | 20.0 | 20.0 | 42.0 |
| [Snapchatの女性750人分のアカウントをハッキングした男に懲役6年](https://www.bleepingcomputer.com/news/security/man-gets-six-years-for-hacking-750-womens-snapchat-accounts/) | 20.0 | 20.0 | 42.0 |
| [Cyber Legends: The Connector](https://www.security.com/expert-perspectives/cyber-legends-connector) | 20.0 | 20.0 | 42.0 |
| [Microsoft、Windows Enterpriseのライセンス認証セキュリティを強化](https://www.helpnetsecurity.com/2026/07/24/microsoft-kms-tpm-security-update/) | 20.0 | 20.0 | 42.0 |
| [Googleの新しいサインイン方法はカメラを見つめるよう求める](https://www.helpnetsecurity.com/2026/07/24/google-selfie-video-sign-in-verification/) | 20.0 | 20.0 | 42.0 |

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
