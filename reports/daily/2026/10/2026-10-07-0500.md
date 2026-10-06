# 📡 サイレーダー 2026-10-07 05:00 JST

このレポートは、2026-10-06 17:00 JST〜2026-10-07 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 115
- [音声で扱う想定のトピック](#audio-topics): 4
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 85

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Atlassian urges immediate patching of critical Data Center file access vulnerability (CVE-2026-21589)](#topic-36029) | 37.0 | 46.0 | 65.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [Hackers exploit 32 zero-days on first day of Pwn2Own Ireland](#topic-36078) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Fake ChatGPT, Gemini Sites steal advertising accounts, MFA codes](#topic-36090) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 4 | [Hitachi Energy Asset Suite](#topic-36132) | 32.0 | 46.0 | 50.0 | 音声 | 温度感上位枠 |
| 5 | [More RMM Tools In the Wild, (Tue, Oct 6th)](#topic-36116) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-36078"></a>

### 1. Hackers exploit 32 zero-days on first day of Pwn2Own Ireland

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | - |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Pwn2Own Ireland 2026の初日には、競技の中で32件のゼロデイが悪用されたと報じられています。
公開情報では、Samsung Galaxy S26が2回攻略され、賞金獲得につながったことが示されています。
ゼロデイの悪用が実際に確認される場では、未修正の脆弱性が現実の製品にどの程度影響し得るかが可視化されます。端末や関連コンポーネントの防御・更新優先度を見直す材料になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象製品や関連ソフトの脆弱性情報、修正提供状況を継続確認する。
- 競技で実証された内容を踏まえ、同系統の機能を持つ製品・設定の点検を行う。
- ベンダー通知やセキュリティアドバイザリを監視し、必要な更新を迅速に適用する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Hackers exploit 32 zero-days on first day of Pwn2Own Ireland](https://www.bleepingcomputer.com/news/security/hackers-exploit-32-zero-days-on-first-day-of-pwn2own-ireland/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-36090"></a>

### 2. Fake ChatGPT, Gemini Sites steal advertising accounts, MFA codes

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

広告アカウント管理者を狙い、ChatGPT、Gemini、Claude、Perplexityを装った偽サイトで認証情報やMFAコードを盗み取るキャンペーンが報告されています。
ブラウザ上に本物らしく見せかける手口が使われているとされ、AI関連サービスの利用者を装った誘導が特徴です。
広告アカウントは不正利用されると、広告出稿の乗っ取りや金銭的被害につながるおそれがあります。
見た目だけでは判別しづらい偽サイトを使うため、利用者教育だけでなく認証周りの対策も重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIサービスを装うログイン画面への誘導に注意し、正規ドメイン確認を徹底する。
- MFAがあっても安心せず、フィッシング耐性の高い認証方式の採用を検討する。
- 広告運用アカウントの異常ログインや権限変更を監視し、被害拡大を早期に検知する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | Active Directory | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | ChatGPT | 主題 | 0.80 | — |
| AIモデル/プロジェクト | Gemini | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Fake ChatGPT, Gemini Sites steal advertising accounts, MFA codes](https://www.bleepingcomputer.com/news/security/fake-chatgpt-gemini-sites-steal-advertising-accounts-mfa-codes/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-36132"></a>

### 3. Hitachi Energy Asset Suite

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 32.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 50.0 |

#### 概要

Hitachi EnergyのAsset Suiteに、認証なしで特定のサーブレットへアクセスできる脆弱性が公表されました。
影響を受けるのはAsset Suite 9.9.0以前で、情報漏えい、改ざん、サービス停止につながる可能性があるとされています。
産業制御・エネルギー分野で使われる製品のため、影響が業務や設備運用に及ぶ可能性があります。ベンダーは修正版への更新や対象機能の無効化を案内しており、早めの対応が重要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 情報漏えい系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Asset Suite 9.9.0以前の利用有無を確認し、優先的に更新計画を立てる。
- 必要のないサーブレットが有効になっていないか点検し、運用上不要なら無効化を検討する。
- 制御系ネットワークの外部公開状況を見直し、アクセス経路や分離設定を再確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-11796 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-7395 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-7395](https://nvd.nist.gov/vuln/detail/CVE-2026-7395) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Hitachi Energy Asset Suite](https://www.cisa.gov/news-events/ics-advisories/icsa-26-279-03) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-36116"></a>

### 4. More RMM Tools In the Wild, (Tue, Oct 6th)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

SANS Internet Storm Centerは、RMM（Remote Management & Monitoring）ツールが脅威アクターに悪用されている動きについて報告しています。
今回の内容では、先に取り上げられたScreenConnectに続き、別のRMMツールが「実環境で見られた」とされています。
RMMツールは本来、正規の遠隔運用に使われるため、攻撃と通常運用の見分けが難しくなりやすい点が注目されています。
管理系ツールの悪用が広がると、検知や対応の難度が上がる可能性があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 検知、監視、SOC/CSIRT運用、環境への適用可否を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 社内で利用中のRMMツールの棚卸しと、想定外の導入有無の確認。
- RMM関連の通信・実行ログについて、正規運用のパターンと差分がないか点検。
- 管理ツールのアカウント保護や権限管理、監査ログの取得状況を再確認。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | ConnectWise ScreenConnect | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [More RMM Tools In the Wild, (Tue, Oct 6th)](https://isc.sans.edu/diary/rss/33400) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-36029"></a>

### 1. Atlassian urges immediate patching of critical Data Center file access vulnerability (CVE-2026-21589)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 65.0 |

#### 概要

Atlassianは、複数のData Center製品に影響する重大な脆弱性CVE-2026-21589について注意喚起し、速やかな対処を求めています。
認証なしで特定のファイルを読み取られる可能性があるとされており、対象製品を自己運用している組織は影響確認が必要です。
JiraやConfluenceなど業務で広く使われる製品群に関わるため、情報漏えいにつながるおそれがあります。
公開状況や設定次第では、外部からの不正アクセスリスクを早急に見直す必要があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 影響を受けるData Center製品とバージョンを棚卸しし、ベンダー案内に沿って修正済み版への更新可否を確認する。
- 公開経路にある対象システムのアクセス制御を見直し、不要な露出がないか点検する。
- 認証なしのファイル参照に関連する異常なアクセス履歴やエラーを確認し、必要に応じて監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-21589 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| ベンダー | Atlassian | 言及あり | 0.80 | — |
| 製品 | Atlassian Jira | 言及あり | 0.80 | — |
| 製品 | Atlassian Confluence | 言及あり | 0.80 | — |
| 製品 | Atlassian Bitbucket | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-21589](https://nvd.nist.gov/vuln/detail/CVE-2026-21589) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Atlassian warns of critical file-access flaw in Jira, Confluence](https://www.bleepingcomputer.com/news/security/atlassian-warns-of-critical-file-access-flaw-in-jira-confluence/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Atlassian urges immediate patching of critical Data Center file access vulnerabi](https://www.helpnetsecurity.com/2026/10/06/atlassian-data-center-cve-2026-21589/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Atlassian Flaw Lets Unauthenticated Attackers Read Known Files Across 8](https://thehackernews.com/2026/10/critical-atlassian-flaw-lets.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [複数のAtlassian製品が影響を受ける「クリティカル」脆弱性](https://www.security-next.com/191078) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Atlassian warns of critical file access flaw in its datacenter products](https://www.theregister.com/security/2026/10/06/atlassian-warns-of-critical-file-access-flaw-in-its-datacenter-products/5301284) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Pwn2Own Ireland 2026初日の結果](https://www.thezdi.com/blog/2026/10/6/pwn2own-ireland-2026-day-one-results) | 29.0 | 20.0 | 43.0 |
| [大阪公立大学、ランサムウェア攻撃の疑いで授業を休講に](https://therecord.media/osaka-university-cancels-classes-ransomware) | 28.0 | 30.0 | 42.0 |
| [IronChainランサムウェアが企業に永久的なデータ損失と高額な停止被害をもたらす](https://any.run/cybersecurity-blog/ironchain-analysis/) | 28.0 | 30.0 | 42.0 |
| [長期にわたるNPMマルウェアキャンペーン、4万件のダウンロードを獲得](https://www.securityweek.com/long-running-npm-malware-campaign-accumulates-40000-downloads/) | 28.0 | 30.0 | 42.0 |
| [RaaS運営者を裏切って被害者資金を横取りしたランサムウェアアフィリエイト](https://www.infosecurity-magazine.com/news/affiliate-doublecrosses-raas/) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア関連の法執行・司法措置](https://www.bleepingcomputer.com/news/security/engineer-sentenced-for-locking-thousands-of-devices-on-employer-network/) | 28.0 | 30.0 | 42.0 |
| [ATMマルウェア作成者とされる人物が逮捕後にネブラスカ州の法廷に出廷](https://therecord.media/atm-malware-creator-appears-in-nebraska-court) | 28.0 | 20.0 | 42.0 |
| [ウクライナで100以上のWebサイトが侵害されたClickFixキャンペーン、Lunexマルウェアを拡散](https://therecord.media/clickfix-campaign-ukraine-lunex-stealer) | 28.0 | 20.0 | 42.0 |
| [FBIがPloutus ATMマルウェア開発者を逮捕](https://www.securityweek.com/fbi-arrests-most-wanted-developer-of-ploutus-atm-malware/) | 28.0 | 20.0 | 42.0 |
| [Blinder Tunnelキャンペーンがイラクの重要インフラを標的にする](https://unit42.paloaltonetworks.com/blinder-tunnel-targets-critical-infrastructure/) | 28.0 | 20.0 | 42.0 |
| [AI時代における脆弱性リスク管理に関するCISOの視点](https://www.microsoft.com/en-us/security/blog/2026/10/06/ciso-perspectives-on-managing-vulnerability-risks-in-the-age-of-ai/) | 27.0 | 20.0 | 42.0 |
| [AIエージェントが暴走した記録をオンライン上で探し出し手がかりを追うコミュニティが発達しつつある](https://gigazine.net/news/20261006-ai-swarm-chasing-group/) | 27.0 | 20.0 | 42.0 |
| [ノルウェー、「AI眼鏡」規制法案提出へ 盗撮など高まる懸念……各国も対応加速](https://www.itmedia.co.jp/news/article/2610/06/2000002064/) | 26.0 | 20.0 | 42.0 |
| [GoogleのPageBreak AIエージェントがWebアプリで500件の脆弱性を発見](https://www.darkreading.com/application-security/google-pagebreak-ai-agent-500-flaws-web-apps) | 25.0 | 20.0 | 42.0 |
| [IANSのKakolowski氏が語る、AIがCISO予算とセキュリティチームをどう変えているか](https://www.darkreading.com/cybersecurity-operations/ai-reshaping-ciso-budgets-security-teams) | 25.0 | 20.0 | 42.0 |
| [韓国当局、複数の銀行へのハッキングにAIエージェントが使われたとみる](https://therecord.media/south-korean-bank-hacks-ai-agents) | 25.0 | 20.0 | 42.0 |
| [IBMのAI搭載脆弱性情報集約基盤が数百件のJava脆弱性を発見](https://www.cybersecuritydive.com/news/ibm-ai-vulnerability-java-lightwell/832249/) | 25.0 | 20.0 | 42.0 |
| [Agent-to-Agent通信のセキュリティ確保：次なるアイデンティティの最前線](https://www.rapid7.com/blog/post/ai-securing-agent-to-agent-communication-next-identity-frontier) | 25.0 | 20.0 | 42.0 |
| [Rogue OpenAIエージェントによるWikipediaへの不正編集とWikimediaへの大量リクエスト](https://www.helpnetsecurity.com/2026/10/06/openai-rogue-agents-wikimedia-wikipedia/) | 25.0 | 20.0 | 42.0 |
| [Wiz AI SASTの紹介：コードとインフラを理解するアプリケーションセキュリティ](https://www.wiz.io/blog/introducing-wiz-ai-sast) | 25.0 | 20.0 | 42.0 |
| [AppViewX、エージェントの発見と実行時制御でシャドーAIのリスクに対応](https://www.helpnetsecurity.com/2026/10/06/appviewx-shadow-ai-visibility/) | 25.0 | 20.0 | 42.0 |
| [New Relic、Ground Truth CLIでターミナルベースの調査と復旧チェックを追加](https://www.helpnetsecurity.com/2026/10/06/new-relic-ground-truth-cli/) | 25.0 | 20.0 | 42.0 |
| [SailPoint、AIエージェントの発見、臨時アクセス、コンプライアンス自動化を追加](https://www.helpnetsecurity.com/2026/10/06/sailpoint-agentic-fabric-innovation/) | 25.0 | 20.0 | 42.0 |
| [巧妙に作成されたWebページ上のゾンビ命令がGitHub Copilot CLIに秘密情報を漏えいさせる可能性](https://www.theregister.com/ai-and-ml/2026/10/06/zombie-instructions-on-carefully-constructed-web-pages-could-trick-github-copilot-cli-into-sharing-secrets/5301206) | 25.0 | 20.0 | 42.0 |
| [Intellias Agentic ServiceOpsがIT運用全体にガバナンスの効いたAIを適用](https://www.helpnetsecurity.com/2026/10/06/intellias-agentic-serviceops/) | 25.0 | 20.0 | 42.0 |
| [AXON DatumがAIシステムの動作前にデータアクセスポリシーを適用](https://www.helpnetsecurity.com/2026/10/06/axon-datum-enforces-data-access-policies-before-ai-systems-act/) | 25.0 | 20.0 | 42.0 |
| [macOSでAIリスクを受けAppleがフルディスクアクセス制御を強化へ](https://www.securityweek.com/apple-to-tighten-full-disk-access-controls-in-macos-amid-ai-risks/) | 25.0 | 20.0 | 42.0 |
| [Wikimedia：不正なOpenAIエージェントによるWikipediaの無断編集](https://www.bleepingcomputer.com/news/security/rogue-openai-agents-behind-potentially-malicious-wikipedia-edits/) | 25.0 | 20.0 | 42.0 |
| [Wikimediaが、OpenAIのエージェントがEtherpad侵害とWikiツールのプロキシ利用を試みたと警告](https://thehackernews.com/2026/10/wikimedia-says-openai-agents-tried-to.html) | 25.0 | 20.0 | 42.0 |
| [15,465件の公開MCPサーバー内部で見つかったもの：Welcome to the Jungle](https://thehackernews.com/2026/10/welcome-to-jungle-what-we-found-inside.html) | 25.0 | 20.0 | 42.0 |
| [Transcend RailsがAIエージェントにポリシー適用と支出管理を提供](https://www.helpnetsecurity.com/2026/10/06/transcend-rails-brings-policy-enforcement-and-spending-controls-to-ai-agents/) | 25.0 | 20.0 | 42.0 |
| [Hack The Box、サイバーセキュリティ分野でのAIエージェント評価を支援](https://www.helpnetsecurity.com/2026/10/06/hack-the-box-ai-range-enterprise-edition/) | 25.0 | 20.0 | 42.0 |
| [GitHubのReviewBenchがAIコードレビュアーを試す](https://www.helpnetsecurity.com/2026/10/06/github-reviewbench-ai-code-review-benchmark/) | 25.0 | 20.0 | 42.0 |
| [Hitachi Energy RTU500の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-279-06) | 24.0 | 46.0 | 50.0 |
| [SavannahにおけるlwIPのSMTPクライアント機能の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-279-02) | 24.0 | 46.0 | 50.0 |
| [Dell System Updateの脆弱性により攻撃者がroot権限を取得可能（CVE-2026-86360）](https://www.helpnetsecurity.com/2026/10/06/dell-system-update-vulnerability-cve-2026-86360/) | 24.0 | 46.0 | 50.0 |
| [VS Code Marketplace拡張機能向けSocketスキャンの導入](https://socket.dev/blog/vscode-extensions) | 22.0 | 20.0 | 42.0 |
| [BigDiskBusterがMicrosoft Defenderを稼働させたまま更新を妨害する](https://www.darkreading.com/application-security/bigdiskbuster-microsoft-defender-running-blocking-updates) | 22.0 | 20.0 | 42.0 |
| [同県サイトで公開した地区防災計画のPDFに個人情報 - 岡山県](https://www.security-next.com/190450) | 22.0 | 20.0 | 42.0 |
| [人事システムから従業員の個人情報が流出した可能性 - 第一ライフG](https://www.security-next.com/190994) | 22.0 | 20.0 | 42.0 |
| [介護事業者向けの報告書依頼メールで誤送信 - 鳥取県](https://www.security-next.com/190687) | 22.0 | 20.0 | 42.0 |
| [従業員アカウントに不正アクセス、取材先に大量なりすましメール - 日経](https://www.security-next.com/191072) | 22.0 | 20.0 | 42.0 |
| [アプリシステムが侵害、顧客情報流出の可能性 - 回転ずしチェーン](https://www.security-next.com/191070) | 22.0 | 20.0 | 42.0 |
| [シチズン時計、委託先への不正アクセスで約10万人分の個人情報漏えいか 大和証券と同じサービスが原因に](https://www.itmedia.co.jp/news/article/2610/06/2000002067/) | 21.0 | 20.0 | 42.0 |
| [相次ぐ不正アクセス受け、古川デジタル相がコメント 国民に3つのサイバー対策呼び掛け](https://www.itmedia.co.jp/news/article/2610/06/2000002060/) | 21.0 | 20.0 | 42.0 |
| [Google、無効な自動報告の急増を受けOSS製品のバグバウンティ報奨金を一時停止](https://thehackernews.com/2026/10/google-pauses-oss-product-bug-bounty.html) | 20.0 | 45.0 | 42.0 |
| [Johnson Controls EasyIO FGの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-279-01) | 20.0 | 28.0 | 50.0 |
| [Hitachi Energy REB500に関する脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-279-05) | 20.0 | 28.0 | 50.0 |
| [元NSA長官ナカソネ氏、NSAの組織改革は「おそらく必要」と発言](https://cyberscoop.com/nsa-reorganization-paul-nakasone-ai-cyberthreats/) | 20.0 | 20.0 | 48.0 |
| [Trump Mobile顧客のデータ流出、gold deviceを受け取っていない人もいる](https://www.theregister.com/security/2026/10/06/trump-mobile-customers-data-dumped-and-some-never-even-received-their-gold-device/5301433) | 20.0 | 20.0 | 42.0 |
| [ASOSがアプリ内通知の「HACKED」表示後にデータ侵害を確認](https://www.bleepingcomputer.com/news/security/asos-confirms-data-breach-after-hacked-in-app-notifications/) | 20.0 | 20.0 | 42.0 |
| [ClickFix攻撃、ブラウザキャッシュにVBScriptペイロードを隠蔽](https://www.infosecurity-magazine.com/news/clickfix-vbscript-browser-cache/) | 20.0 | 20.0 | 42.0 |
| [FBI、ShinyHunters侵害の原因を請負業者のパッチ適用漏れと指摘](https://www.securityweek.com/fbi-blames-contractors-missed-patch-for-shinyhunters-breach/) | 20.0 | 20.0 | 42.0 |
| [ASOSの「ハッカー」が顧客にプッシュ通知を送信](https://www.malwarebytes.com/blog/news/2026/10/asos-hackers-send-push-notifications-to-customers) | 20.0 | 20.0 | 42.0 |
| [米国のサイバー・レジリエンスと監督体制が一連の攻撃で試される](https://www.cybersecuritydive.com/news/us-cyber-resilience-oversight-attacks/832235/) | 20.0 | 20.0 | 42.0 |
| [RMMソフトウェアを保護する方法：MSPがテストすべき8つの管理策](https://www.bleepingcomputer.com/news/security/how-to-secure-rmm-software-8-controls-msps-should-test/) | 20.0 | 20.0 | 42.0 |
| [Nikkei、従業員2名のクラウドアカウント侵害を公表](https://www.infosecurity-magazine.com/news/nikkei-employee-cloud-account/) | 20.0 | 20.0 | 42.0 |
| [Anacondaがエージェント群と自律型セキュリティテストを組み合わせる仕組み](https://www.helpnetsecurity.com/2026/10/06/anaconda-platform/) | 20.0 | 20.0 | 42.0 |
| [Red HatのLightwell Projectが400件のオープンソース脆弱性を修正](https://www.infosecurity-magazine.com/news/red-hat-lightwell-remediates-400/) | 20.0 | 20.0 | 42.0 |
| [無題](https://www.huntress.com/blog/mapping-akira-ransomware-attack) | 20.0 | 20.0 | 42.0 |
| [重要医療機器がPQC移行に対応できない問題](https://www.infosecurity-magazine.com/news/medical-devices-pqc-transition/) | 20.0 | 20.0 | 42.0 |
| [Facebook Marketplace詐欺で氏名と電話番号が悪用される](https://www.malwarebytes.com/blog/threat-intel/2026/10/facebook-marketplace-phish-uses-your-name-and-number) | 20.0 | 20.0 | 42.0 |
| [ASOS顧客に影響したインシデント](https://www.ncsc.gov.uk/news/incident-affecting-asos-customers) | 20.0 | 20.0 | 42.0 |
| [LibreOfficeとOpenOfficeの脆弱性により、悪意あるスプレッドシートがマクロ警告なしでコード実行可能に](https://thehackernews.com/2026/10/libreoffice-and-openoffice-flaws-let.html) | 20.0 | 20.0 | 42.0 |
| [ASOSアプリでファストファッションではなくデータ漏えいの脅威が発生](https://www.theregister.com/security/2026/10/06/asos-app-delivers-a-data-leak-threat-instead-of-fast-fashion/5301332) | 20.0 | 20.0 | 42.0 |
| [デンマークのID登録簿で、住民数を上回る人数の詳細情報が漏えい](https://www.theregister.com/security/2026/10/06/denmarks-id-register-spills-more-peoples-details-than-the-country-has-residents/5301307) | 20.0 | 20.0 | 42.0 |
| [ASOS顧客に届いた奇妙な「ハッキングされた」メッセージ、Snowflake侵害の疑い](https://www.infosecurity-magazine.com/news/asos-customers-message-suspected/) | 20.0 | 20.0 | 42.0 |
| [専門家が考えるCISAのOT保護指針とは](https://cyberscoop.com/cisa-ot-cybersecurity-directive/) | 20.0 | 20.0 | 42.0 |
| [ASOSのユーザーがサイバー犯罪者からのプッシュ通知受信後に懸念を報告](https://www.itpro.com/security/cyber-crime/this-has-got-to-be-one-of-the-most-visible-hacks-in-history-asos-users-report-concerns-after-receiving-push-notification-from-cyber-criminals) | 20.0 | 20.0 | 42.0 |
| [Domino’s顧客を狙ったクレデンシャルスタッフィング攻撃](https://www.malwarebytes.com/blog/news/2026/10/dominos-customers-targeted-in-credential-stuffing-attacks) | 20.0 | 20.0 | 42.0 |
| [2026年9月に発表されたサイバーセキュリティM&A動向：39件の買収発表](https://www.securityweek.com/cybersecurity-ma-roundup-39-deals-announced-in-september-2026/) | 20.0 | 20.0 | 42.0 |
| [「楽天ドライブ」、不正アクセスにより約1.5万アカウントのデータなどが漏えい](https://internet.watch.impress.co.jp/docs/news/2146152.html) | 20.0 | 20.0 | 42.0 |
| [Ontinue、ION MXDRにマネージドダークウェブ監視を追加](https://www.helpnetsecurity.com/2026/10/06/ontinue-ion-dark-web-monitoring/) | 20.0 | 20.0 | 42.0 |
| [Symantec DLPをTetrate Agent Routerに拡張するエージェント実行環境でのDLP検査](https://www.security.com/product-insights/dlp-inspection-where-your-agents-run-extending-symantec-dlp-tetrate-agent-router) | 20.0 | 20.0 | 42.0 |
| [盗賊に仲間なし、ハッカーが自らの仲間を裏切る](https://www.itpro.com/security/cyber-crime/no-honor-amongst-thieves-as-hacker-betrays-his-own-gang) | 20.0 | 20.0 | 42.0 |
| [880万人のデンマーク人を襲ったサイバー攻撃で分かっていること](https://www.itpro.com/security/data-breaches/danish-data-breach-everything-we-know-about-the-cyber-attack-that-hit-8-8m-danes) | 20.0 | 20.0 | 42.0 |
| [デンマーク中央個人登録簿でのデータ侵害、880万人に影響](https://www.securityweek.com/8-8-million-impacted-by-data-breach-at-denmarks-central-person-register/) | 20.0 | 20.0 | 42.0 |
| [学校向けソフトウェア提供企業Bromcomでレガシーサインオンサービスの再利用が問題に](https://www.theregister.com/security/2026/10/06/legacy-sign-on-service-comes-back-to-bite-school-software-provider-bromcom/5301156) | 20.0 | 20.0 | 42.0 |
| [Nikkei、従業員のMicrosoftとGoogleメールアカウントへの侵害を公表](https://www.bleepingcomputer.com/news/security/nikkei-discloses-breaches-of-employees-microsoft-google-email-accounts/) | 20.0 | 20.0 | 42.0 |
| [サイバー犯罪収益の急増を受けて警察がパスキー利用を呼びかけ](https://www.infosecurity-magazine.com/news/police-urge-passkey-surge/) | 20.0 | 20.0 | 42.0 |
| [デンマークの人口登録簿でデータ漏えい、880万人の情報が流出](https://www.helpnetsecurity.com/2026/10/06/denmark-central-population-register-cpr-data-breach/) | 20.0 | 20.0 | 42.0 |
| [シチズン 約10万人分情報漏えいか](https://news.yahoo.co.jp/pickup/6597772?source=rss) | 20.0 | 20.0 | 42.0 |
| [日経BP、メールアカウントへの不正アクセスにより個人情報漏えいの疑い。日経新聞社への攻撃が影響](https://internet.watch.impress.co.jp/docs/news/2146104.html) | 20.0 | 20.0 | 42.0 |
| [ライブ会話で進化するソーシャルエンジニアリング検知](https://www.securityweek.com/social-engineering-detection-moves-into-the-live-conversation/) | 20.0 | 20.0 | 42.0 |
| [国内不正アクセス 過去最多ペース](https://news.yahoo.co.jp/pickup/6597763?source=rss) | 20.0 | 20.0 | 42.0 |

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
