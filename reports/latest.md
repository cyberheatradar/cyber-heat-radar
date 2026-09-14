# 📡 サイレーダー 2026-09-15 05:00 JST

このレポートは、2026-09-14 17:00 JST〜2026-09-15 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 83
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 53

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-85706: CISA KEV catalog addition](#topic-32206) | 37.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [CVE-2026-75650: StyleSmuggler — Critical RCE in Adobe Commerce and Magento](#topic-31503) | 37.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 3 | [Cisco Secure Email Gateway and Secure Email and Web Manager Security Hardening Release: September 2026](#topic-32498) | 37.0 | 46.0 | 51.0 | 音声 | 温度感上位枠 |
| 4 | [ENISA launched the CRA Single Reporting Platform for actively exploited vulnerabilities](#topic-32523) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [Red Heron Exploits Gitea RCE to Compromise 13 Organizations Across Six Countries](#topic-32490) | 32.0 | 38.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-32206"></a>

### 1. CVE-2026-85706: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

CVE-2026-85706 は、GitLab CE/EE に関する深刻な脆弱性として CISA の KEV カタログに追加されています。
公開情報では、認証なしでサーバー上のファイルを読み取られるおそれがあり、修正公開後まもなく外部からの探索や試行が観測されたとされています。
KEV への追加は、実際の悪用リスクが高く、優先対応が求められる脆弱性であることを示します。
特に self-managed の GitLab 環境では、放置すると情報漏えいにつながる可能性があるため注意が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
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

- GitLab CE/EE の自己管理環境で、該当する修正版への更新状況を確認する。
- 外部公開された GitLab インスタンスについて、不要な露出やアクセス制御の不備がないか見直す。
- 関連する監査ログを確認し、ファイル参照の不審な挙動や普段と異なるアクセスの有無を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-85706 | 関連CVE | 1.00 | 候補あり（URL 9件以上） |
| 脆弱性 | CVE-2026-87719 | 関連CVE | 1.00 | 未確認 |
| ベンダー | GitLab | 言及あり | 0.80 | — |
| ベンダー | watchTowr | 言及あり | 0.80 | — |
| 製品 | GitLab CE/EE | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-85706](https://nvd.nist.gov/vuln/detail/CVE-2026-85706) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Perfect-10 GitLab bug under attack days after patch lands](https://www.theregister.com/security/2026/09/14/perfect-10-gitlab-bug-under-attack-days-after-patch-lands/5296176) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-85706: Critical GitLab Path Traversal Exploited in the Wild](https://www.rapid7.com/blog/post/etr-cve-2026-85706-critical-gitlab-path-traversal-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [GitLab’s critical flaw is already drawing internet-wide probes](https://cyberscoop.com/gitlab-critical-flaws-path-traversal-scans/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [GitLab CVSS 10 File-Read Flaw Draws In-the-Wild Probes After Disclosure](https://thehackernews.com/2026/09/gitlab-cvss-10-file-read-flaw-draws-in.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [GitLab urges users to patch max severity path traversal flaw](https://www.bleepingcomputer.com/news/security/gitlab-urges-users-to-patch-max-severity-path-traversal-flaw/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers Exploit Maximum Severity Flaw in GitLab](https://www.infosecurity-magazine.com/news/hackers-exploit-maximum-severity/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Malicious actors already using critical GitLab flaw, CISA and others warn](https://www.cybersecuritydive.com/news/gitlab-vulnerability-exploitation-cisa-kev/830278/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-31503"></a>

### 2. CVE-2026-75650: StyleSmuggler — Critical RCE in Adobe Commerce and Magento

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Adobe Commerce と Magento Open Source に影響する CVE-2026-75650（StyleSmuggler）について、複数の公開情報で悪用の観測が報告されています。
記載情報では、未認証の攻撃者による任意コード実行につながる重大な脆弱性として扱われています。
ECサイト基盤に広く使われる製品のため、影響を受ける環境ではサーバー侵害や不正なバックドア設置につながるおそれがあります。
すでに悪用が示唆されている点から、単なる理論上の脅威ではなく、優先度の高い対応対象として注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
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

- 影響を受ける Adobe Commerce / Magento Open Source のバージョンと稼働状況を確認し、提供済みの修正を速やかに適用する。
- 管理画面や公開サーバーで不審な改変、未知のファイル、想定外のプロセス起動など侵害痕跡の有無を点検する。
- Web アプリケーション保護、監視、バックアップの復旧手順を見直し、侵害が疑われる場合の初動対応を準備する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-75650 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Adobe | 言及あり | 0.80 | — |
| 製品 | Adobe Commerce | 言及あり | 0.80 | — |
| マルウェア | Webshell | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-75650](https://nvd.nist.gov/vuln/detail/CVE-2026-75650) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-75650: StyleSmuggler — Critical RCE in Adobe Commerce and Magento](https://www.akamai.com/blog/security-research/2026/sep/cve-2026-75650-stylesmuggler-adobe-commerce-magento) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Adobe Patches Over 170 Vulnerabilities, Including Commerce Zero-Day](https://www.securityweek.com/adobe-patches-over-170-vulnerabilities-including-commerce-zero-day/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Adobe fixes critical Magento zero-day exploited to backdoor servers](https://www.bleepingcomputer.com/news/security/adobe-fixes-critical-magento-zero-day-exploited-to-backdoor-servers/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Adobe Patches Magento Zero-Day Exploited to Deploy Rust Backdoor and PHP Web She](https://thehackernews.com/2026/09/adobe-patches-magento-zero-day.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-32498"></a>

### 3. Cisco Secure Email Gateway and Secure Email and Web Manager Security Hardening Release: September 2026

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

Ciscoは、Secure Email GatewayとSecure Email and Web Manager向けに、内部レビューで見つかった複数の脆弱性を修正するハードニング更新を公開しました。
対象のうち少なくとも1件は実際に悪用が確認されているとされ、CVE-2026-20353を含む複数のCVEが割り当てられています。
メールセキュリティ製品は組織の入口に近く、影響が広がると受信メールの保護や運用に直結します。
特に悪用観測がある場合は、通常の脆弱性対応よりも優先度を上げて確認されやすい点が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Ciscoの該当製品を利用しているかを確認し、公開済みの更新適用状況を点検する。
- 修正対象に複数のCVEが含まれるため、個別の1件だけでなく関連する更新一式を確認する。
- 回避策がないとされているため、パッチ適用と併せて監視強化や設定点検を早めに進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20353](https://nvd.nist.gov/vuln/detail/CVE-2026-20353) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Email Gateway and Secure Email and Web Manager Security Hardening R](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-hardening-esa-dfCrfXkm) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32523"></a>

### 4. ENISA launched the CRA Single Reporting Platform for actively exploited vulnerabilities

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

ENISAが、EUのサイバーレジリエンス法（CRA）に基づく「Single Reporting Platform」の運用を開始したとされています。
製品に関わる活動中の脆弱性や重大インシデントの報告を、この単一の窓口で受け付ける仕組みです。
CRAの報告義務が実運用に入ることで、EU市場向け製品を扱う事業者は対応フローの整備がより重要になります。
脆弱性や重大インシデントの把握と報告を一元化するため、社内のCSIRTや法務、製品部門の連携が求められます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- EU市場向け製品の報告対象になりうる事象を社内で整理し、初動手順を確認する。
- 脆弱性受付、重大インシデント判定、対外報告の責任分担を明確にする。
- 製品セキュリティと法令対応の両面で、報告期限や記録保持の運用を見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ENISA launched the CRA Single Reporting Platform for actively exploited vulnerab](https://www.helpnetsecurity.com/2026/09/14/enisa-cra-single-reporting-platform/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-32490"></a>

### 5. Red Heron Exploits Gitea RCE to Compromise 13 Organizations Across Six Countries

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>R⁠C⁠E</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 32.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

脅威アクター「Red Heron」が、Giteaの最近公表された脆弱性を悪用し、複数国にまたがるキャンペーンで公開インターネット上のインスタンスを侵害したと報告されています。
公開情報では、少なくとも13組織が影響を受けたとされ、対象は6か国に及ぶとされています。
Giteaは開発者向けに広く使われるため、公開環境での脆弱性悪用は組織のソースコードや運用情報に波及する可能性があります。
短期間での悪用が示唆されており、パッチ適用や露出資産の確認が重要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Giteaの利用有無を確認し、公開インスタンスがある場合は優先的に更新状況を点検する。
- インターネット公開された管理画面や不要な露出を見直し、アクセス制御を強化する。
- 異常なログイン、設定変更、リポジトリ操作など、侵害を示す兆候がないか監視を強める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | Gitea | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Red Heron Exploits Gitea RCE to Compromise 13 Organizations Across Six Countries](https://thehackernews.com/2026/09/red-heron-exploits-gitea-rce-to.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

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
| [HackersがHBO MaxのRedditアカウントを乗っ取り、ClickFix広告でマルウェアを拡散](https://www.bleepingcomputer.com/news/security/hackers-hijack-hbo-max-reddit-account-to-push-malware-in-clickfix-ads/) | 28.0 | 20.0 | 42.0 |
| [GTA6の偽リークに便乗したマルウェア配布の実態](https://blog.polyswarm.io/gamers-get-played-fake-gta6-leaks-deliver-a-grab-bag-of-malware) | 28.0 | 20.0 | 42.0 |
| [公開されたVite開発サーバーを狙うハッカー、AWSとAzureの認証情報を窃取](https://www.bleepingcomputer.com/news/security/hackers-target-exposed-vite-dev-servers-to-steal-aws-azure-secrets/) | 28.0 | 20.0 | 42.0 |
| [親ウクライナ派のハッキング集団「Cat」がロシア標的に新たなマルウェアを展開](https://therecord.media/ukraine-malware-russia-ransomware) | 28.0 | 20.0 | 42.0 |
| [Telus、顧客にアカウント侵害を警告](https://www.securityweek.com/telus-warns-customers-of-account-breaches/) | 28.0 | 20.0 | 42.0 |
| [Revolut、金融情報とパスポート情報の漏えいを公表](https://www.bleepingcomputer.com/news/security/revolut-discloses-data-breach-exposing-financial-info-passports/) | 28.0 | 20.0 | 42.0 |
| [なぜAIエージェントはウソをつき不正行為を行い協調するのか？](https://gigazine.net/news/20260914-why-ai-agents-lying-cheating-coordinating/) | 27.0 | 20.0 | 42.0 |
| [古坂大魔王が8歳娘の手描きキャラをAIアニメ化→「良いパパ」「子どもの創造性損ねる」と賛否両論](https://www.itmedia.co.jp/news/article/2609/14/2000001458/) | 26.0 | 20.0 | 42.0 |
| [OpenAIの悪意あるボット群がRubyGemsを攻撃](https://www.theregister.com/security/2026/09/14/openais-malicious-bot-swarm-attacked-rubygems/5296356) | 25.0 | 20.0 | 42.0 |
| [Anthropic CEOが語る、AIの改善から制御への転換の必要性](https://www.darkreading.com/cyber-risk/anthropic-ceo-shift-from-improving-to-controlling-ai) | 25.0 | 20.0 | 42.0 |
| [AIエージェントによりセキュリティチームがますます後手に回る](https://www.cybersecuritydive.com/news/security-teams-increasingly-outflanked-by-ai-agents/830290/) | 25.0 | 20.0 | 42.0 |
| [Rapid7がForresterのMDRランドスケープで注目ベンダーに選出：将来はExposure-informedで予防的なMDRへ](https://www.rapid7.com/blog/post/dr-forrester-mdr-landscape-notable-vendor-preemptive) | 25.0 | 20.0 | 42.0 |
| [⚡ 週刊まとめ：Rogue AI Agents、WeChatワーム、PaperCut攻撃、AIスパイ活動、ルートキット](https://thehackernews.com/2026/09/weekly-recap-rogue-ai-agents-wechat.html) | 25.0 | 20.0 | 42.0 |
| [Anthropic CEOの中国AI開発抑制発言に対する北京の反発](https://www.securityweek.com/beijing-hits-back-at-anthropic-ceos-call-to-curb-chinas-ai-development/) | 25.0 | 20.0 | 42.0 |
| [Bitsight、サプライチェーン全体で脅威インテリジェンスと露出監視を連携](https://www.helpnetsecurity.com/2026/09/14/bitsight-beacon/) | 25.0 | 20.0 | 42.0 |
| [AIが人類にもたらすリスクへの新たな警告が長年の論争を再燃させる](https://www.securityweek.com/new-warnings-about-the-risks-of-ai-to-humanity-revive-a-long-running-debate/) | 25.0 | 20.0 | 42.0 |
| [Dataminrがエージェント型AIでセキュリティ脅威を予測・検証](https://www.helpnetsecurity.com/2026/09/14/dataminr-uses-agentic-ai-to-predict-and-verify-security-threats/) | 25.0 | 20.0 | 42.0 |
| [AIを制御する競争と、人間らしさを守るために](https://www.securityweek.com/the-race-to-control-ai-and-protect-what-makes-us-human/) | 25.0 | 20.0 | 42.0 |
| [AIが露出問題を変えた。検証もそれに合わせて変わる必要がある。](https://thehackernews.com/2026/09/ai-changed-exposure-problem-validation.html) | 25.0 | 20.0 | 42.0 |
| [Airrived、AIエージェントの行動とリスクを追跡するAgentic Observabilityを追加](https://www.helpnetsecurity.com/2026/09/14/airrived-agentic-observability-expansion/) | 25.0 | 20.0 | 42.0 |
| [CISOsがAIエージェントの価値を損なわずに制御へ急ぐ](https://www.securityweek.com/cisos-race-to-control-ai-agents-without-destroying-their-value/) | 25.0 | 20.0 | 42.0 |
| [セキュリティチームはAIの信頼確立より先にAI導入を進めている](https://www.cybersecuritydive.com/spons/security-teams-are-adopting-ai-faster-than-they-trust-it/829748/) | 25.0 | 20.0 | 42.0 |
| [OpenAI Agent SwarmがRubyGemsパッケージマネージャーをハッキング](https://www.infosecurity-magazine.com/news/openai-agent-swarm-hacks-rubygems/) | 25.0 | 20.0 | 42.0 |
| [Cisco Secure Email GatewayのSQLインジェクション脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-esa-inj-2bLVGmhX) | 24.0 | 46.0 | 50.0 |
| [Human AttackerがMarimoのRCEをマシンスピードで悪用](https://www.infosecurity-magazine.com/news/human-attacker-machine-speed/) | 24.0 | 38.0 | 42.0 |
| [個人情報含むファイルを誤送信、前年同様と勘違い - 沖縄県](https://www.security-next.com/189735) | 22.0 | 20.0 | 42.0 |
| [市デジタルアーカイブサイトが改ざん、無関係サイトへ誘導 - 大町市](https://www.security-next.com/190193) | 22.0 | 20.0 | 42.0 |
| [生徒寮でサポート詐欺、入寮者の個人情報が流出か - 宮崎県](https://www.security-next.com/189985) | 22.0 | 20.0 | 42.0 |
| [iOS 26.6.2配信中、iPhoneをモバイル通信で更新できない不具合修正](https://news.mynavi.jp/techplus/article/20260914-4967067/) | 21.0 | 20.0 | 42.0 |
| [30,000件インストールのTwitch拡張機能でユーザーのOAuthトークンが露出](https://www.bleepingcomputer.com/news/security/twitch-extension-with-30k-installs-exposes-users-oauth-tokens/) | 20.0 | 20.0 | 42.0 |
| [Black Axeの南アフリカでの活動に関与したとされる5人の指導者が米国へ身柄送還](https://cyberscoop.com/black-axe-south-africa-leaders-extradited/) | 20.0 | 20.0 | 42.0 |
| [新しいハードウェアデバイスが暗号化メモリにRAM攻撃し、データを露出させる](https://www.theregister.com/security/2026/09/14/new-hardware-device-can-ram-into-encrypted-memory-expose-your-data/5296377) | 20.0 | 20.0 | 42.0 |
| [Intel TDXとAMD SEV-SNPの機密コンピューティングを突破する新たなDDRop攻撃](https://thehackernews.com/2026/09/new-ddrop-attack-breaks-intel-tdx-and.html) | 20.0 | 20.0 | 42.0 |
| [WordPressが高リスクな更新の配布前にブロックする自動プラグインレビューを追加](https://thehackernews.com/2026/09/wordpress-adds-automated-plugin-reviews.html) | 20.0 | 20.0 | 42.0 |
| [悪意のあるTwitch拡張機能が31,000人のOAuthトークンを漏えいさせる](https://www.infosecurity-magazine.com/news/malicious-twitch-extension-oauth/) | 20.0 | 20.0 | 42.0 |
| [Googleの新しい検索リダイレクトにより、クリック前のリンク確認が難しくなる](https://www.malwarebytes.com/blog/news/2026/09/googles-new-search-redirects-make-links-harder-to-check-before-you-click) | 20.0 | 20.0 | 42.0 |
| [パッチ自動化にはアクセルだけでなくブレーキも必要な理由](https://www.bleepingcomputer.com/news/security/why-patch-automation-needs-brakes-not-just-an-accelerator/) | 20.0 | 20.0 | 42.0 |
| [Entrustが暗号資産インベントリデータをセキュリティ対策へ活用](https://www.helpnetsecurity.com/2026/09/14/entrust-cbom-capabilities/) | 20.0 | 20.0 | 42.0 |
| [Revolutのデータ侵害で個人情報と金融情報が流出](https://www.securityweek.com/personal-financial-info-exposed-in-revolut-data-breach/) | 20.0 | 20.0 | 42.0 |
| [軍事システムへの攻撃増加を受け、防衛サイバー予算が急増へ](https://www.infosecurity-magazine.com/news/defense-cyber-spending-attacks/) | 20.0 | 20.0 | 42.0 |
| [Revolut、政府メールアカウントを使う詐欺師に顧客データを提供](https://therecord.media/revolut-scam-crypto-impersonation) | 20.0 | 20.0 | 42.0 |
| [Chinese HackersがTencent Softwareの重大な脆弱性を悪用しワンクリックでコード実行](https://www.securityweek.com/chinese-hackers-exploit-critical-tencent-software-flaw-for-one-click-code-execution/) | 20.0 | 20.0 | 42.0 |
| [Revolut、偽の政府要請によるデータ侵害を確認](https://www.infosecurity-magazine.com/news/revolut-data-breach-fake-government/) | 20.0 | 20.0 | 42.0 |
| [Revolutが顧客IDと財務データを政府関係者を装った相手に提供](https://www.malwarebytes.com/blog/news/2026/09/revolut-gave-customer-ids-and-financial-data-to-a-government-impostor) | 20.0 | 20.0 | 42.0 |
| [コンテックの法人向けWi-Fi機器「FLEXLAN」シリーズに複数の脆弱性、最新版ファームウェアに更新を](https://internet.watch.impress.co.jp/docs/news/2140840.html) | 20.0 | 20.0 | 42.0 |
| [Revolutが偽の政府要請で顧客データを提供](https://www.itpro.com/security/data-breaches/revolut-hands-over-customer-data-after-fake-government-request) | 20.0 | 20.0 | 42.0 |
| [2026年に知っておくべきサイバーセキュリティ統計13選](https://www.security.com/expert-perspectives/13-cybersecurity-stats-you-should-know-2026) | 20.0 | 20.0 | 42.0 |
| [Microsoft：9月の更新プログラムでWindows ServerのRDSに障害が発生](https://www.bleepingcomputer.com/news/microsoft/microsoft-september-updates-cause-rds-failures-on-windows-server/) | 20.0 | 20.0 | 42.0 |
| [JFrog Artifactoryの3件の脆弱性を悪用したバックドア展開](https://www.securityweek.com/three-jfrog-artifactory-flaws-exploited-for-backdoor-deployment/) | 20.0 | 20.0 | 42.0 |
| [UK政府、2300万人のユーザー向けにパスワード廃止を開始](https://www.theregister.com/security/2026/09/14/ukgov-begins-killing-off-passwords-for-23-million-users/5296088) | 20.0 | 20.0 | 42.0 |
| [ゼロトラストは未来だが、企業にはなおVPNが必要だ](https://www.cybersecuritydive.com/spons/zero-trust-is-the-future-but-enterprises-still-need-their-vpns/829864/) | 20.0 | 20.0 | 42.0 |
| [ConnectWiseがScreenConnectの脆弱性を修正、ワーム型攻撃で悪用される](https://www.securityweek.com/connectwise-patches-screenconnect-vulnerability-exploited-in-worm-like-attacks/) | 20.0 | 20.0 | 42.0 |
| [Microsoft: 9月の更新プログラムで一部のWindows PCの音声が利用不可に](https://www.bleepingcomputer.com/news/microsoft/microsoft-september-updates-break-audio-on-some-windows-pcs/) | 20.0 | 20.0 | 42.0 |

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
