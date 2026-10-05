# 📡 サイレーダー 2026-10-06 05:00 JST

このレポートは、2026-10-05 17:00 JST〜2026-10-06 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 97
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 71

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [5th October – Threat Intelligence Report](#topic-34525) | 52.0 | 74.0 | 67.0 | GitHub | audio_eligible_by_public_rules_false |
| 2 | [CVE-2026-88779: CISA KEV catalog addition](#topic-35828) | 47.0 | 64.0 | 59.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-35828"></a>

### 1. CVE-2026-88779: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 47.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

CISA は、Citrix NetScaler に関する脆弱性 CVE-2026-88779 を Known Exploited Vulnerabilities（KEV）カタログに追加しました。
公開情報では、影響を受ける NetScaler ADC / Gateway に対するゼロデイ悪用が確認されており、主な影響はサービス停止につながる DoS とされています。
KEV への追加は、実際の悪用が確認された脆弱性として優先的な対応対象になることを意味します。
NetScaler は境界機器として使われることが多く、停止時の業務影響が大きくなりやすい点にも注意が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Citrix の緊急更新の適用状況を確認し、未適用の機器を優先的に更新する。
- NetScaler ADC / Gateway の稼働監視を強化し、再発するサービス停止や異常な負荷の兆候を確認する。
- 外部公開している管理・認証関連の経路を点検し、不要な露出を抑える。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-88779 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-88779](https://nvd.nist.gov/vuln/detail/CVE-2026-88779) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA flags new exploited NetScaler flaw as attackers crash appliances (CVE-2026-](https://www.helpnetsecurity.com/2026/10/05/cisa-flags-new-exploited-netscaler-flaw-as-attackers-crash-appliances-cve-2026-88779/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Exploitation of Citrix NetScaler Zero-Day Hits Appliances Patched Days Earlier](https://www.securityweek.com/exploitation-of-citrix-netscaler-zero-day-hits-appliances-patched-days-earlier/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix patches NetScaler SAML zero-day exploited in attacks](https://www.bleepingcomputer.com/news/security/citrix-patches-netscaler-saml-zero-day-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [「NetScaler」のSAML構成にDoS脆弱性 - すでに悪用も](https://www.security-next.com/191050) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [US, Australia warn of latest Citrix vulnerability after NetScaler advisory](https://therecord.media/us-australia-warn-of-latest-citrix-vulnerability) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix issues patch for third exploited flaw in NetScaler](https://www.cybersecuritydive.com/news/citrix-patch-third-exploited-flaw-netscaler/832128/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-34525"></a>

### 1. 5th October – Threat Intelligence Report

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 52.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Citrix NetScaler ADCおよびNetScaler Gatewayに関するCVE-2026-88771は、複数の公開情報で実際の悪用が報告されている脆弱性として扱われています。
Citrixは関連する修正更新を公開しており、周辺情報では公開PoCや検証コードの言及も見られます。
リモートコード実行に関わる脆弱性で、実際の悪用が確認されているとされるため、公開環境の影響が大きい点が注目されています。
公開PoCの存在が示唆されていることから、未対応の機器は優先的な確認対象になります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 9 sources。
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

- Citrix NetScaler ADC / Gatewayの該当バージョンを確認し、提供済みの修正更新の適用状況を点検する。
- インターネット公開の機器を優先して棚卸しし、不要な露出や運用設定の見直しを行う。
- 関連する認証・アクセスログを確認し、不審な管理者操作や想定外の通信がないかを監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-76504 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-86950 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-88771 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-88772 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-90970 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-88771](https://nvd.nist.gov/vuln/detail/CVE-2026-88771) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [5th October – Threat Intelligence Report](https://research.checkpoint.com/2026/5th-october-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Week in review: Researcher breaks into Microsoft analytics service, NetScaler RC](https://www.helpnetsecurity.com/2026/10/04/week-in-review-researcher-breaks-into-microsoft-analytics-service-netscaler-rce-0-day-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: NetScaler ADCおよびNetScaler Gatewayにおける複数の脆弱性（CVE-2026-88771、CVE-2026-88772等](https://www.jpcert.or.jp/at/2026/at260029.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: NetScaler Zero Days CVE-2026-88771 and CVE-2026-88772 Exploited in](https://unit42.paloaltonetworks.com/netscaler-zero-days-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Government, Finance Orgs Targeted in Weeks-Long NetScaler Zero-Day Attacks](https://www.securityweek.com/government-finance-orgs-targeted-in-weeks-long-netscaler-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [NetScaler zero-day exploitation escalates into mass attacks (CVE-2026-88771)](https://www.helpnetsecurity.com/2026/09/29/netscaler-zero-day-exploitation-escalates-into-mass-attacks-cve-2026-88771/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix patches actively exploited NetScaler zero-days after a weekend of unoffic](https://cyberscoop.com/citrix-zero-days-delayed-disclosure/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（2件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Weekly Recap：NetScalerとFortiMailのゼロデイ、AIコーディングの漏えい、Spectre v2とランサムウェア関連の逮捕事件](https://thehackernews.com/2026/10/weekly-recap-netscaler-and-fortimail-0.html) | 35.0 | 30.0 | 43.0 |
| [大阪公立大の大規模システム障害、サイバー攻撃が原因か 13万人超の個人情報流出恐れ](https://www.itmedia.co.jp/news/article/2610/05/2000002018/) | 29.0 | 30.0 | 42.0 |
| [University of Illinois Chicagoの医学部がランサムウェア攻撃の被害に遭う](https://therecord.media/ransomware-university-illinois-chicago) | 28.0 | 30.0 | 42.0 |
| [ミッションを支えるシステムを狙うOT脅威：米国の重要インフラと軍事作戦への影響](https://blog.polyswarm.io/targeting-the-systems-behind-the-mission-ot-threats-to-us-critical-infrastructure-and-military-operations) | 28.0 | 20.0 | 42.0 |
| [ClingSTUNマルウェアが未修正のIoTデバイスをプロキシノード化](https://www.infosecurity-magazine.com/news/clingstun-backdoor-unpatched-iot/) | 28.0 | 20.0 | 42.0 |
| [メールトラフィックを装う新たなステルス型Linuxバックドア、通信事業者を標的に](https://www.infosecurity-magazine.com/news/smtp-linux-backdoors-network-edge/) | 28.0 | 20.0 | 42.0 |
| [ベラルーシ系ハクティビストがロシアの医療ネットワークに2年間潜伏、研究者が報告](https://therecord.media/belarusian-hacktivists-two-years-Russian-healthcare-network) | 28.0 | 20.0 | 42.0 |
| [Malwarebytes Scam Link CheckがURLを解析し潜在的なリスクを解説](https://www.helpnetsecurity.com/2026/10/05/malwarebytes-scam-link-check/) | 28.0 | 20.0 | 42.0 |
| [Ploutus ATMマルウェア開発者とされる人物、逮捕後に米国で出廷](https://www.bleepingcomputer.com/news/security/suspected-dev-of-ploutus-atm-malware-appears-in-us-court-after-arrest/) | 28.0 | 20.0 | 42.0 |
| [Realtek Jungle SDKの脆弱性悪用でSTUNベースのC2を持つClingボットネットを配布する試行](https://thehackernews.com/2026/10/realtek-jungle-sdk-exploit-attempts.html) | 28.0 | 20.0 | 42.0 |
| [Pwn2Own Ireland 2026の全日程](https://www.thezdi.com/blog/2026/10/5/pwn2own-ireland-2026-the-full-schedule) | 27.0 | 20.0 | 42.0 |
| [Out-of-band Exchange Server更新で高深刻度のメールボックスアクセス脆弱性を修正（CVE-2026-96940）](https://thehackernews.com/2026/10/microsoft-exchange-flaw-lets.html) | 26.0 | 28.0 | 54.0 |
| [韓国の銀行6行にサイバー攻撃 計2万5000人超の個人情報流出──AIエージェントを使った可能性も 現地報道](https://www.itmedia.co.jp/news/article/2610/05/2000002009/) | 26.0 | 20.0 | 42.0 |
| [中国系ハッカーが米国政府関係者を装ってAIを悪用したサイバースパイ活動を実施](https://www.darkreading.com/cyberattacks-data-breaches/chinese-actor-impersonates-us-officials-cyber-espionage) | 25.0 | 20.0 | 42.0 |
| [Google、AI生成投稿の増加を受けオープンソース脆弱性報奨プログラムを一時停止](https://www.malwarebytes.com/blog/news/2026/10/google-pauses-open-source-bug-bounty-program-after-rise-in-ai-submissions) | 25.0 | 20.0 | 42.0 |
| [韓国、AIを悪用した攻撃の疑いの中で銀行への侵害を調査](https://www.bleepingcomputer.com/news/security/south-korea-probes-bank-breaches-amid-suspected-ai-powered-attacks/) | 25.0 | 20.0 | 42.0 |
| [LTM、AIエージェントの監視と意図しない動作の巻き戻しに向けてBlueVerse AgenTraceIQを発表](https://www.helpnetsecurity.com/2026/10/05/ltm-blueverse-agentraceiq/) | 25.0 | 20.0 | 42.0 |
| [AI駆動の攻撃が変えるセキュリティ戦略](https://www.darkreading.com/cyber-risk/ai-attacks-security-strategies) | 25.0 | 20.0 | 42.0 |
| [RemoveMacAIがmacOS 27でApple Intelligenceを無効化し、モデルを削除](https://www.helpnetsecurity.com/2026/10/05/removemacai-turn-off-apple-intelligence/) | 25.0 | 20.0 | 42.0 |
| [認証情報レイヤーの拡大がセキュリティチームの可視化を上回っている](https://thehackernews.com/2026/10/the-credential-layer-is-expanding.html) | 25.0 | 20.0 | 42.0 |
| [AIが発見したRejetto HFSの脆弱性が悪用される](https://www.securityweek.com/exploitation-hits-rejetto-hfs-vulnerability-discovered-by-ai/) | 25.0 | 20.0 | 42.0 |
| [Apple、macOSのAIエージェント向けデータアクセスに対するフルディスクアクセス制御を強化へ](https://thehackernews.com/2026/10/apple-plans-tighter-macos-full-disk.html) | 25.0 | 20.0 | 42.0 |
| [Google、AIによる脆弱性報告の増加でオープンソースバグバウンティを一時停止](https://www.infosecurity-magazine.com/news/google-suspends-opensource-bug/) | 25.0 | 20.0 | 42.0 |
| [ChatGPTで画像生成中にOpenAIが視覚広告を表示へ](https://www.bleepingcomputer.com/news/artificial-intelligence/openai-will-show-visual-ads-in-chatgpt-while-you-generate-images/) | 25.0 | 20.0 | 42.0 |
| [Google、AI生成の粗雑な報告増加でオープンソース脆弱性報奨制度を一時停止](https://www.itpro.com/software/open-source/this-pause-is-due-to-a-significant-rise-in-automated-submissions-the-vast-majority-of-which-are-not-valid-google-pauses-open-source-bug-bounty-scheme-over-ai-slop-submissions) | 25.0 | 20.0 | 42.0 |
| [DSPMとAIで実現するデータセキュリティの近代化とツール削減](https://www.cybersecuritydive.com/spons/modernizing-data-security-with-dspm-ai-and-fewer-tools/831578/) | 25.0 | 20.0 | 42.0 |
| [AIスパム急増を受けてGoogleがオープンソースバグバウンティプログラムを停止](https://www.bleepingcomputer.com/news/google/google-halts-open-source-bug-bounty-program-amid-ai-spam-surge/) | 25.0 | 20.0 | 42.0 |
| [Apple、AIエージェントの高度化に伴いmacOSのディスクアクセスを強化](https://www.helpnetsecurity.com/2026/10/05/macos-full-disk-access-updates/) | 25.0 | 20.0 | 42.0 |
| [Citrix NetScalerが新たなゼロデイで標的に](https://www.infosecurity-magazine.com/news/citrix-netscaler-zero-day/) | 22.0 | 20.0 | 43.0 |
| [重複する断片を用いたトークン制限の突破](https://portswigger.net/research/smashing-the-token-limit) | 22.0 | 20.0 | 42.0 |
| [複数サイトに不正アクセス、プラグイン脆弱性が標的に - ベネッセグループ会社](https://www.security-next.com/190961) | 22.0 | 20.0 | 42.0 |
| [米当局、脆弱性4件を「悪用脆弱性リスト」に追加 - 早期対応を要請](https://www.security-next.com/191054) | 22.0 | 20.0 | 42.0 |
| [「焼肉きんぐ」アプリの会員情報が流出 - 原因など詳細を調査](https://www.security-next.com/191040) | 22.0 | 20.0 | 42.0 |
| [未達で返戻の水道料金減免解除通知書が所在不明 - 横浜市](https://www.security-next.com/190448) | 22.0 | 20.0 | 42.0 |
| [ブロガー情報管理システムに不正アクセス、個人情報が流出 - 集英社](https://www.security-next.com/190800) | 22.0 | 20.0 | 42.0 |
| [Linuxカーネルの脆弱性が一挙1313件も報告される、AI普及で「個々の脆弱性を追う対策は限界」との指摘](https://gigazine.net/news/20261005-debian-security-advisory/) | 22.0 | 20.0 | 42.0 |
| [大和証券、委託先で11万人分の情報漏洩か 「被害は当社以外も」](https://xtech.nikkei.com/atcl/nxt/column/18/00001/12074/) | 21.0 | 20.0 | 42.0 |
| [ホワイトエッセンス、約105万アカウントの個人情報流出 8月発表の不正アクセス調査で判明](https://www.itmedia.co.jp/news/article/2610/05/2000002016/) | 21.0 | 20.0 | 42.0 |
| [「焼肉きんぐ」個人情報約1079万件が漏えい 公式アプリのシステムに不正アクセス ほぼ全会員分に相当](https://www.itmedia.co.jp/news/article/2610/05/2000002011/) | 21.0 | 20.0 | 42.0 |
| [タイムズカー、9月末で退会できなかった利用者が発生 アクセス集中が影響](https://xtech.nikkei.com/atcl/nxt/news/24/03407/) | 21.0 | 20.0 | 42.0 |
| [AttackersがRejetto HFSの管理者セッション偽造とRCEを可能にする脆弱性を標的にする](https://thehackernews.com/2026/10/attackers-target-rejetto-hfs-flaw-that.html) | 20.0 | 46.0 | 54.0 |
| [米国は水道システムを守るための実効的な計画が必要だ](https://cyberscoop.com/us-water-system-cybersecurity-ai-threats-op-ed/) | 20.0 | 20.0 | 48.0 |
| [ShinyHuntersメンバーとされる人物がヨルダンで拘束され、法執行機関に協力か](https://therecord.media/alleged-shinyhunters-member-detained-jordan-fbi) | 20.0 | 20.0 | 42.0 |
| [FBI、ShinyHuntersによるハッキング事件で複数人を逮捕と確認](https://www.theregister.com/security/2026/10/05/fbi-confirms-multiple-arrests-related-to-shinyhunters-hack/5301178) | 20.0 | 20.0 | 42.0 |
| [IQVIAが医療データの適切な匿名化に失敗し780万ドルの罰金を科される](https://www.bleepingcomputer.com/news/security/iqvia-fined-78-million-for-failing-to-properly-anonymize-health-data/) | 20.0 | 20.0 | 42.0 |
| [ウクライナの大手スーパーATB、サイバー攻撃を確認　ハッカーがデータ流出を警告](https://therecord.media/atb-ukraine-cyberattack-ransomware) | 20.0 | 20.0 | 42.0 |
| [Debianの最新カーネルセキュリティ更新で1,313件の修正を適用すべき理由](https://www.theregister.com/os-platforms/2026/10/05/debians-latest-kernel-security-update-has-1313-reasons-to-patch/5301124) | 20.0 | 20.0 | 42.0 |
| [デンマークの人口登録データ侵害、880万人に影響](https://www.bleepingcomputer.com/news/security/denmark-population-registry-data-breach-affects-88-million-people/) | 20.0 | 20.0 | 42.0 |
| [Dell System Updateの脆弱性により攻撃者がroot権限を取得可能に](https://www.bleepingcomputer.com/news/security/new-dell-system-update-flaw-lets-hackers-gain-root-privileges/) | 20.0 | 20.0 | 42.0 |
| [Google、無効な自動報告の急増を受けオープンソースのバグ報奨金を縮小](https://www.securityweek.com/google-narrows-open-source-bug-bounty-amid-wave-of-invalid-automated-reports/) | 20.0 | 20.0 | 42.0 |
| [提案中の反Flock法案、ナンバープレート自動読み取り装置に打撃の可能性](https://www.malwarebytes.com/blog/news/2026/10/proposed-anti-flock-bills-could-spell-trouble-for-license-plate-readers) | 20.0 | 20.0 | 42.0 |
| [HuntressがClickFix攻撃を検知し対応する方法](https://www.huntress.com/blog/fix-for-clickfix) | 20.0 | 20.0 | 42.0 |
| [SNS上の偽ブランド割引で消費者の「買い逃し不安」を悪用する手口](https://www.helpnetsecurity.com/2026/10/05/milk-dragon-phishing-fake-discounts/) | 20.0 | 20.0 | 42.0 |
| [日本経済新聞社、従業員と利用者を狙った侵入被害を公表](https://therecord.media/nikkei-cyberattack-japan-data) | 20.0 | 20.0 | 42.0 |
| [LinuxバックドアがSTUNプロトコルを悪用し、数十件の脆弱性を突く](https://www.securityweek.com/linux-backdoor-abuses-stun-protocol-exploits-dozens-of-flaws/) | 20.0 | 20.0 | 42.0 |
| [ニュージャージー州とテキサス州のヘルスケア企業でデータ侵害、25万人に影響](https://www.securityweek.com/250000-impacted-by-data-breaches-at-new-jersey-texas-healthcare-firms/) | 20.0 | 20.0 | 42.0 |
| [Executive Order 14421が示すゼロトラストによるグリッド保護](https://www.akamai.com/blog/security/2026/oct/secure-grid-executive-order-14421-zero-trust) | 20.0 | 20.0 | 42.0 |
| [デンマーク国民登録簿のデータ侵害で880万人の情報が流出](https://therecord.media/denmark-breach-register-cyberattack) | 20.0 | 20.0 | 42.0 |
| [米上院、医療分野のサイバーセキュリティ強化法案を可決](https://www.securityweek.com/senate-passes-bipartisan-bill-to-strengthen-healthcare-cybersecurity/) | 20.0 | 20.0 | 42.0 |
| [拘束されたShinyHuntersのハッカーがFBIによる他のメンバー追跡に協力していると報道](https://www.helpnetsecurity.com/2026/10/05/shinyhunters-member-rey-detained-jordan-fbi/) | 20.0 | 20.0 | 42.0 |
| [AWS CEO Matt Garman、データセンター増設への反発の中で方針を擁護](https://www.itpro.com/security/aws-ceo-matt-garman-says-hostile-nations-are-intentionally-seeding-misinformation-in-the-us-about-data-centers-to-trick-us-into-slowing-down) | 20.0 | 20.0 | 42.0 |
| [大和証券、問い合わせ管理サービスへの不正アクセスで約11万人の利用者情報漏えいの可能性 委託先のサーバーに不正アクセスが発生](https://internet.watch.impress.co.jp/docs/news/2145818.html) | 20.0 | 20.0 | 42.0 |
| [信頼する防御の裏側を支えるエンジニアたち](https://www.security.com/expert-perspectives/meet-engineers-behind-defenses-you-trust) | 20.0 | 20.0 | 42.0 |
| [MAKERphone 2：カメラ・スピーカー・プロトタイピングボードを差し替え可能なDIY 4Gスマホ](https://www.helpnetsecurity.com/2026/10/05/makerphone-2-diy-4g-phone/) | 20.0 | 20.0 | 42.0 |
| [「焼肉きんぐ」会員管理システムへの不正アクセスで約1079万件の個人情報漏えい](https://internet.watch.impress.co.jp/docs/news/2145813.html) | 20.0 | 20.0 | 42.0 |
| [学校向けソフトウェア提供企業Bromcomのレガシーサインオンサービスに起因する問題](https://www.theregister.com/security/2026/10/05/legacy-sign-on-service-comes-back-to-bite-school-software-provider-bromcom/5301156) | 20.0 | 20.0 | 42.0 |
| [英国の学校でサイバーインシデントからの復旧がさらに迅速に](https://www.infosecurity-magazine.com/news/uk-schools-recovering-faster/) | 20.0 | 20.0 | 42.0 |
| [Frontline Educationの侵害でK-12学校区職員に影響](https://www.infosecurity-magazine.com/news/frontline-education-breach-k12/) | 20.0 | 20.0 | 42.0 |
| [次世代アイデンティティセキュリティで権限が基盤であるべき理由](https://www.cybersecuritydive.com/spons/why-permissions-must-be-the-foundation-for-next-gen-identity-security/831732/) | 20.0 | 20.0 | 42.0 |
| [大阪公立大 サイバー攻撃受け障害](https://news.yahoo.co.jp/pickup/6597639?source=rss) | 20.0 | 20.0 | 42.0 |
| [大和証券、22万件情報漏えいか 顧客約11万人の口座番号も](https://www.itmedia.co.jp/news/article/2610/05/2000002005/) | 16.0 | 20.0 | 42.0 |

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
