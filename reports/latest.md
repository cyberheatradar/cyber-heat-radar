# 📡 サイレーダー 2026-06-20 05:01 JST

このレポートは、2026-06-19 17:00 JST〜2026-06-20 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 70
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 41

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-20253: CISA KEV catalog addition](#topic-17163) | 45.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 2 | [CISA: Splunk Enterprise flaw actively exploited, patch by Sunday](#topic-18393) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Operation Endgame Disrupts Malware Network Linked to Major Ransomware Gang](#topic-18397) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Rights groups brand Home Office's AI age guesser for asylum-seekers as biased and inaccurate](#topic-18386) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [CryptoBandits Malware Doubles as a Backdoor, Abuses Tor](#topic-18383) | 32.0 | 38.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-17163"></a>

### 1. CVE-2026-20253: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>I⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

CISAは、Splunk EnterpriseにおけるCVE-2026-20253をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
複数の報道では、同脆弱性は認証不要で悪用されうる重大な問題で、実際の攻撃での利用も確認されたとされています。
Splunkは修正版を公開しており、影響を受ける環境では迅速な対応が求められます。
KEV入りは、すでに実際の悪用が確認されている可能性を示すため、通常の脆弱性情報より優先度が高くなります。
特に基盤システムとしてSplunkを使う組織では、侵害や横展開の起点になり得る点が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Splunk Enterpriseの該当バージョンを使っていないか確認し、修正版の適用状況を点検する。
- CISAのKEV対象であるため、通常より高い優先度でパッチ適用や緩和策の実施計画を進める。
- 認証不要での悪用が報じられているため、ログや不審なリクエストの有無を含めて関連システムを確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20253 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20253](https://nvd.nist.gov/vuln/detail/CVE-2026-20253) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Unauthenticated RCE in Splunk Enterprise under active attack (CVE-2026-20253)](https://www.helpnetsecurity.com/2026/06/19/splunk-vulnerability-cve-2026-20253-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Splunk Enterprise Vulnerability Exploited in Attacks Days After Disclosure](https://www.securityweek.com/splunk-enterprise-vulnerability-exploited-in-attacks-days-after-disclosure/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/06/18/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Splunk Enterprise Flaw Lets Attackers Run Code Without Authentication](https://thehackernews.com/2026/06/critical-splunk-enterprise-flaw-lets.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補あり（URL 3件以上 / 該当CVE 1件）。

---

<a id="topic-18393"></a>

### 2. CISA: Splunk Enterprise flaw actively exploited, patch by Sunday

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

CISAが、Splunk Enterpriseに存在する重大な脆弱性について、攻撃で悪用されているとして米連邦機関に期限までの対処を促しています。
公開情報では詳細な手口までは示されていませんが、既に悪用が観測されている点が注目されています。
業務監視やログ管理で広く使われる製品に関するため、影響範囲が大きくなる可能性があります。悪用が確認されている脆弱性は、優先的な更新と緊急点検の対象になります。

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

- Splunk Enterpriseの該当バージョンや適用済みパッチ状況を確認する。
- ベンダーや公的機関の告知に基づき、更新・緩和策を早急に適用する。
- 認証ログや管理画面への不審なアクセスがないか、直近の監査を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20253 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA: Splunk Enterprise flaw actively exploited, patch by Sunday](https://www.bleepingcomputer.com/news/security/cisa-splunk-enterprise-flaw-actively-exploited-patch-by-sunday/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補あり（URL 3件以上 / 該当CVE 1件）。

---

<a id="topic-18397"></a>

### 3. Operation Endgame Disrupts Malware Network Linked to Major Ransomware Gang

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Operation Endgameの一環として、Evil Corpに関連するとされるマルウェア網に対する妨害が実施されたと報じられています。
あわせて、SocGholishマルウェアがEvil Corp関係の約15,000サイトから除去されたとされています。
ランサムウェア関連組織の活動基盤に打撃を与える動きとして注目されます。感染経路や誘導元の一部が減少した可能性があり、関連する防御・監視の見直しにつながります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SocGholishを含む初期侵入経路の監視を強化し、関連ドメインや不審なリダイレクトの検知を点検する。
- ランサムウェア関連の脅威情報を踏まえ、メール・Web・エンドポイントの多層防御設定を再確認する。
- 同種の妨害報道があっても残存インフラや派生活動はあり得るため、アラート運用とログ確認を継続する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Operation Endgame Disrupts Malware Network Linked to Major Ransomware Gang](https://www.infosecurity-magazine.com/news/operation-endgame-socgholish-evil/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-18386"></a>

### 4. Rights groups brand Home Office's AI age guesser for asylum-seekers as biased and inaccurate

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

英国の内務省が難民申請者の年齢推定に使うとされるAIについて、権利団体から偏りや精度への懸念が示されています。
特に、子どもと大人の境界にいる人を信頼して判別できないのではないか、という点が問題視されています。
年齢判定は保護や手続きの分岐に直結しやすく、誤判定が本人の権利や扱いに影響する可能性があります。AIを行政判断に使う際の公平性、説明責任、検証可能性が改めて問われる事例です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIの判断を単独で最終決定に使わず、人手による確認や異議申立ての流れを用意すること。
- 導入前後で、特定集団に不利な誤判定が出ていないかを継続的に点検すること。
- 判断の根拠、限界、運用条件を関係者に分かる形で明示し、記録を残すこと。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Rights groups brand Home Office's AI age guesser for asylum-seekers as biased an](https://www.theregister.com/security/2026/06/19/rights-groups-brand-home-offices-ai-age-guesser-for-asylum-seekers-as-biased-and-inaccurate/5258892) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-18383"></a>

### 5. CryptoBandits Malware Doubles as a Backdoor, Abuses Tor

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 32.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

CryptoBanditsと呼ばれるマルウェアが、情報窃取だけでなくバックドアとしても機能し、TorやローカルSOCKS5プロキシを使って通信を中継しているとされています。
公開情報では、遠隔操作につながる動きが示されており、単なる盗難型マルウェアよりも広い悪用可能性が示唆されています。
通信の秘匿性を高める仕組みが悪用されると、検知や追跡が難しくなるため、感染後の横展開や遠隔操作のリスクが上がります。
情報窃取とリモート実行の両面を持つ点は、被害の範囲が広がりやすいことを意味します。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Tor経由やSOCKS系の不審な中継通信がないか、ネットワーク監視とログで確認する。
- 情報窃取系の兆候だけでなく、バックドアとしての不正な継続接続や外向き通信も合わせて点検する。
- 既知IOCが少ない場合でも、EDRで不審なプロセス連携やプロキシ利用の挙動検知を優先する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CryptoBandits Malware Doubles as a Backdoor, Abuses Tor](https://www.securityweek.com/cryptobandits-malware-doubles-as-a-backdoor-abuses-tor/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
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
| [Gentlemen RaaSがGentleKiller EDRフレームワークを用いて400のセキュリティプロセスを標的に](https://thehackernews.com/2026/06/the-gentlemen-raas-uses-gentlekiller.html) | 28.0 | 30.0 | 42.0 |
| [GoogleのreCAPTCHAで手のジェスチャーを求められることがある問題](https://www.helpnetsecurity.com/2026/06/19/google-recaptcha-hand-gesture-verification/) | 28.0 | 20.0 | 48.0 |
| [SocGholish対策で約1万5000件の感染サイトをクリーンアップ](https://www.malwarebytes.com/blog/news/2026/06/nearly-15000-infected-websites-cleaned-in-socgholish-crackdown) | 28.0 | 20.0 | 42.0 |
| [AppleがBeatsの盗聴脆弱性を修正、DOTがDeltaのCrowdStrike調査を終了、AWS Continuum](https://www.securityweek.com/in-other-news-apple-patches-beats-eavesdropping-flaw-dot-closes-delta-crowdstrike-probe-aws-continuum/) | 28.0 | 20.0 | 42.0 |
| [CISA、FortiBleedにより86,644台のFortiGateデバイスが影響とFortinet顧客に警告](https://thehackernews.com/2026/06/cisa-warns-fortinet-customers-as.html) | 28.0 | 20.0 | 42.0 |
| [RussiaのEvil Corpハッカーグループに関連するマルウェアネットワークを警察が摘発](https://therecord.media/socgholish-botnet-disrupted) | 28.0 | 20.0 | 42.0 |
| [サイバー犯罪者がGitHub、YouTube、VirusTotalを悪用して暗号資産窃取マルウェアを拡散](https://www.helpnetsecurity.com/2026/06/19/fake-github-stars-crypto-stealing-malware/) | 28.0 | 20.0 | 42.0 |
| [FortiBleed: 8万6000件のFortinetデバイス認証情報が漏えい](https://www.securityweek.com/fortibleed-86000-fortinet-device-credentials-compromised/) | 28.0 | 20.0 | 42.0 |
| [The Hacker News、ANY.RUNを2026年の最優秀セキュリティ調査プラットフォームに認定](https://any.run/cybersecurity-blog/best-security-platform/) | 28.0 | 20.0 | 42.0 |
| [Weekly Metasploitアップデート: NTLM Relay権限昇格、MCP Server統合、Paperclip AIのRCEチェーンなど](https://www.rapid7.com/blog/post/pt-metasploit-wrap-up-19-06-2026) | 27.0 | 20.0 | 42.0 |
| [AIと話すだけで動画編集できる映像ソフト、オープンソースで登場 出力は「Premiere」「DaVinci」でも読み込み可](https://www.itmedia.co.jp/news/articles/2606/19/news119.html) | 26.0 | 20.0 | 42.0 |
| [AutoJack攻撃で1つのWebページがAIエージェントを乗っ取りホスト上でコード実行可能に](https://thehackernews.com/2026/06/autojack-attack-lets-one-web-page.html) | 25.0 | 20.0 | 42.0 |
| [すべてのAIエージェントはIDであるが、ほとんどの組織はそう扱っていない](https://www.bleepingcomputer.com/news/security/every-ai-agent-is-an-identity-most-organizations-dont-treat-them-that-way/) | 25.0 | 20.0 | 42.0 |
| [AIの進展とサイバーセキュリティチームに迫る変化の圧力](https://www.darkreading.com/cybersecurity-operations/stressors-ai-changes-cybersecurity-teams) | 25.0 | 20.0 | 42.0 |
| [支援型からエージェント型へ：脅威管理を再定義するAIの変革](https://thehackernews.com/2026/06/from-assistive-to-agentic-ai-shift.html) | 25.0 | 20.0 | 42.0 |
| [AWSがAI搭載の脆弱性管理プラットフォーム「Continuum」を発表](https://www.infosecurity-magazine.com/news/aws-continuum-ai-vulnerability/) | 25.0 | 20.0 | 42.0 |
| [Shadow AIの真の脅威はアクセス制御にある](https://thehackernews.com/2026/06/forget-data-leakage-shadow-ais-real.html) | 25.0 | 20.0 | 42.0 |
| [NY州の男性、AI生成のヌード画像で大学生を脅迫し起訴される](https://www.bleepingcomputer.com/news/security/new-york-man-faces-cyberstalking-charge-after-sharing-ai-generated-nudes-online/) | 25.0 | 20.0 | 42.0 |
| [Klueの侵害によりSalesforceのデータが窃取、Huntressも影響を受ける](https://www.helpnetsecurity.com/2026/06/19/klue-salesforce-data-breach-huntress/) | 23.0 | 23.0 | 43.0 |
| [学生向けのイベント当選通知でメール誤送信 - 兵庫県立大](https://www.security-next.com/186139) | 22.0 | 20.0 | 42.0 |
| [職員アカウントが侵害、スパムの踏み台に - 日中経済協会](https://www.security-next.com/185994) | 22.0 | 20.0 | 42.0 |
| [保護者の同意なく子どもの個人情報をPTAへ提供 - 小田原市](https://www.security-next.com/185935) | 22.0 | 20.0 | 42.0 |
| [「FortiOS」の「SSL VPN」脆弱性に関するアドバイザリを更新](https://www.security-next.com/186165) | 22.0 | 20.0 | 42.0 |
| [Apple、Beats Studio Budsの脆弱性を修正、イヤホンが盗聴器化する恐れ](https://www.malwarebytes.com/blog/bugs/2026/06/apple-patches-beats-studio-buds-flaw-that-could-turn-earbuds-into-a-wiretap) | 21.0 | 28.0 | 54.0 |
| [Cisco Identity Services Engine のリモートコード実行および情報漏えいの脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-ise-multi-G5WP8vv) | 20.0 | 46.0 | 50.0 |
| [修正不能な「usbliter8」エクスプロイトがApple A12およびA13のSecureROM起動チェーンを突破](https://thehackernews.com/2026/06/unpatchable-usbliter8-exploit-breaks.html) | 20.0 | 20.0 | 42.0 |
| [Texas州政府のデータ侵害で300万人超の運転免許証情報が流出](https://www.bleepingcomputer.com/news/security/texas-govt-data-breach-exposes-over-3-million-drivers-licenses/) | 20.0 | 20.0 | 42.0 |
| [checkm8型のBootROMエクスプロイトをA12・A13 iPhone向けに公開](https://www.theregister.com/security/2026/06/19/researchers-drop-checkm8-style-bootrom-exploit-for-a12-and-a13-iphones/5259028) | 20.0 | 20.0 | 42.0 |
| [Appleの「Hide My Email」変更にプライバシー重視派が反発](https://www.bitdefender.com/en-us/blog/hotforsecurity/apples-hide-my-email-tweak-leaves-privacy-fans-fuming) | 20.0 | 20.0 | 42.0 |
| [Operation Endgame、SocGholishサーバーを妨害し14,971件のWordPressサイトをクリーンアップ](https://thehackernews.com/2026/06/operation-endgame-disrupts-socgholish.html) | 20.0 | 20.0 | 42.0 |
| [テキサスではすべてが大きく、より良い――データ漏えいも例外ではない](https://www.theregister.com/security/2026/06/19/texas-gov-vendor-breach-exposes-data-of-3m-hunters-anglers/5258815) | 20.0 | 20.0 | 42.0 |
| [英国のプライバシー監督当局トップが「判断ミス」を認め辞任](https://www.theregister.com/security/2026/06/19/britains-privacy-watchdog-quits-after-poor-judgment-admission/5258926) | 20.0 | 20.0 | 42.0 |
| [公益事業へのサイバー攻撃の大半を占めるレガシーキット](https://www.itpro.com/security/legacy-kit-behind-vast-majority-of-cyber-attacks-on-utilities) | 20.0 | 20.0 | 42.0 |
| [展示会会場で聞いたXDRに関する8つの質問](https://www.security.com/product-insights/8-xdr-questions) | 20.0 | 20.0 | 42.0 |
| [Mastodon 4.6、プロフィールコレクションと二要素認証制御を追加](https://www.helpnetsecurity.com/2026/06/19/mastodon-4-6-released/) | 20.0 | 20.0 | 42.0 |
| [Klueのサプライチェーン攻撃の影響を受けたサイバーセキュリティ企業](https://www.securityweek.com/cybersecurity-firms-impacted-by-klue-supply-chain-attack/) | 20.0 | 20.0 | 42.0 |
| [GoogleがAndroid開発者認証の義務化に向けた実施時期を発表](https://www.helpnetsecurity.com/2026/06/19/android-developer-verification-rollout-markets/) | 20.0 | 20.0 | 42.0 |
| [AccentureがDragos、runZero、NetRiseを42億ドルで買収するサイバーセキュリティ取引](https://www.helpnetsecurity.com/2026/06/19/accenture-dragos-runzero-netrise-acquisition/) | 20.0 | 20.0 | 42.0 |
| [OAuthトークン悪用による顧客データ漏えいを受けSalesforceがKlueアプリ連携を停止](https://thehackernews.com/2026/06/salesforce-disables-klue-app.html) | 20.0 | 20.0 | 42.0 |
| [SlackやTeamsなどメール以外のチャネルにおける脅威検知への信頼不足](https://www.infosecurity-magazine.com/news/threat-detection-across-nonemail/) | 20.0 | 20.0 | 42.0 |
| [IPv4マップドIPv6アドレスを用いたeBankingフィッシング攻撃](https://isc.sans.edu/diary/rss/33090) | 17.0 | 20.0 | 42.0 |

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
