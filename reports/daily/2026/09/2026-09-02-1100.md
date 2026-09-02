# 📡 サイレーダー 2026-09-02 11:00 JST

このレポートは、2026-09-02 05:00 JST〜2026-09-02 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 71
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 43

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Anthropic、「Claude」ユーザーを狙った情報窃取型マルウェアを警告](#topic-30468) | 34.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 2 | [AI Model Evaluator METR Hit by Credential Theft, Probing](#topic-30547) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [Counterfeit installers to system compromise: Tracking a deceptive software download campaign](#topic-30510) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-30468"></a>

### 1. Anthropic、「Claude」ユーザーを狙った情報窃取型マルウェアを警告

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 34.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Anthropicは、Claudeの一部ユーザーを狙う情報窃取型マルウェアについて注意を呼びかけています。
報道によれば、攻撃はセッションの乗っ取りを通じて利用クレジットの不正取得につながる可能性があるとされています。
AIサービスのアカウントやセッションが狙われると、個人情報や利用枠の損失だけでなく、業務利用への影響も出るおそれがあります。
生成AIの普及に伴い、モデルそのものだけでなく周辺の利用環境を守る重要性が増しています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Claudeなど外部AIサービスのセッション管理を見直し、多要素認証や端末保護を徹底する。
- 利用クレジットや請求の急増、不審なログインやセッション挙動を定期的に確認する。
- 従業員に対し、AIサービス名をかたる不審な案内や偽サイトへの注意喚起を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Anthropic | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | Anthropic | 主題 | 0.80 | — |
| AIモデル/プロジェクト | Claude | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Anthropic、「Claude」ユーザーを狙った情報窃取型マルウェアを警告](https://japan.zdnet.com/article/35252172/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-30547"></a>

### 2. AI Model Evaluator METR Hit by Credential Theft, Probing

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

AIモデル評価を手がける非営利組織METRが、認証情報の窃取とその後の調査対象になったとされています。
攻撃者がAPIキーを盗み、結果として公開AIモデルのクレジット約60万ドル分が消費されたと報じられています。
AI関連組織でも、APIキーやアクセス権限の管理不備が大きなコストや運用影響につながりうることを示す事例です。
AI利用の拡大に伴い、従来型の認証情報保護や権限管理の重要性が改めて注目されます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- APIキーやサービスアカウントの保管・ローテーション・失効手順を見直す。
- 異常なAPI利用量やクレジット消費を早期に検知できる監視を整える。
- 権限の最小化と、重要なアクセスに対する追加保護を徹底する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [AI Model Evaluator METR Hit by Credential Theft, Probing](https://www.darkreading.com/identity-access-management-security/ai-model-evaluator-metr-credential-theft-probing) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-30510"></a>

### 3. Counterfeit installers to system compromise: Tracking a deceptive software download campaign

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

正規ソフトウェアの配布元を装った偽のダウンロードページや、改変されたインストーラーアーカイブを通じてマルウェアを配布するキャンペーンが確認されています。
Microsoftは、観測された手口や検知情報、IOC、緩和策を公開し、組織に対して注意喚起しています。
信頼されやすい「ソフトの入手経路」を悪用するため、利用者や運用担当者が気づきにくく、初期侵入につながるおそれがあります。
正規ソフトの導入フローやダウンロード元の確認が、被害防止の重要なポイントになります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ソフトウェア入手先の正当性を再確認し、検索結果や広告経由の偽サイトに注意する。
- インストーラーの署名や配布元、ハッシュなどの整合性確認を運用に組み込む。
- EDR/XDRやメール・Web保護で不審なダウンロードや実行を検知・ブロックできるようにする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Kaspersky | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Qwen | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |
| 攻撃/検証ツール | Responder | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Counterfeit installers to system compromise: Tracking a deceptive software downl](https://www.microsoft.com/en-us/security/blog/2026/09/01/counterfeit-installers-system-compromise-tracking-deceptive-software-download-campaign/) | <nobr>内容確認・補足情報</nobr> |

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
| [赤武エンジニアリングでランサムウェア感染によるシステム障害が発生](https://scan.netsecurity.ne.jp/article/2026/09/02/56105.html) | 29.0 | 30.0 | 42.0 |
| [ランサム損失は28社 1年で倍の236億円に](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/082700567/082700003/) | 29.0 | 30.0 | 42.0 |
| [ランサムウェアグループが内部から人材を勧誘する動き、強化されるセキュリティが背景に](https://www.darkreading.com/cyber-risk/stronger-security-drives-ransomware-groups-to-recruit-from-within) | 28.0 | 30.0 | 42.0 |
| [古い未修正の脆弱性によりフィリピン原子力機関へのアクセスが可能に](https://www.darkreading.com/cyberattacks-data-breaches/old-unpatched-flaws-attackers-philippines-nuclear-agency) | 28.0 | 20.0 | 42.0 |
| [CopsとCrowdStrikeがSalityボットネットをシンクホールへ誘導し無力化](https://www.theregister.com/cyber-crime/2026/09/02/cops-crowdstrike-disrupt-sality-botnet-by-poisoning-the-network-and-diverting-into-sinkholes/5293795) | 28.0 | 20.0 | 42.0 |
| [FBIが著名人を狙う巧妙なフィッシングキャンペーンに警戒を呼びかけ](https://cyberscoop.com/fbi-alert-oauth-consent-phishing-campaign/) | 28.0 | 20.0 | 42.0 |
| [中国の「Fire Ant」キャンペーン、侵害したCiscoルーターを追加攻撃の踏み台として悪用](https://therecord.media/router-hacks-fire-ant-group-china) | 28.0 | 20.0 | 42.0 |
| [Okta、業界標準プロトコル「XAA」採用の「Agent SSO」提供開始 ～ AI エージェントと人間のアイデンティティを一元管理](https://scan.netsecurity.ne.jp/article/2026/09/02/56100.html) | 26.0 | 20.0 | 42.0 |
| [Anthropic、「Claude Fable 5.1」と「Claude Mythos 5.1」発表 「監視の難しさ」への懸念も開示](https://www.itmedia.co.jp/news/article/2609/02/2000001048/) | 26.0 | 20.0 | 42.0 |
| [AIを取り巻くサイバー脅威を整理する](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/111900071/081800082/) | 26.0 | 20.0 | 42.0 |
| [クラウドかローカルかの問いに終止符を打つ--「ハイブリッドAI」が切り拓く、AI活用の現実解](https://japan.zdnet.com/article/35251954/) | 26.0 | 20.0 | 42.0 |
| [従量課金で気付けば「AI貧乏」 1カ月で200万円超過の例も](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/092400133/082700202/) | 26.0 | 20.0 | 42.0 |
| [「ChatGPT Work」、ユーザーの許可不要でウェブログイン可能に--リスクになるか](https://japan.zdnet.com/article/35252044/) | 26.0 | 20.0 | 42.0 |
| [OpenAI、「高度で大規模なAIによるサイバー攻撃」の発生を警告--対策は？](https://japan.zdnet.com/article/35252117/) | 26.0 | 20.0 | 42.0 |
| [AIエージェントまたは人間による攻撃を受けるもう一つのArtifactoryのCVE](https://www.theregister.com/security/2026/09/01/another-artifactory-cve-under-attack-by-ai-agents-or-humans/5293769) | 25.0 | 20.0 | 42.0 |
| [AIプラットフォームへの攻撃が増加する中で悪用されるLangflowの深刻な脆弱性](https://www.darkreading.com/vulnerabilities-threats/critical-langflow-flaw-exploited-attacks-rise) | 25.0 | 20.0 | 42.0 |
| [Palo Alto Networks、AIエージェントプラットフォーム「Console」を買収](https://www.securityweek.com/palo-alto-networks-acquires-ai-agent-platform-console/) | 25.0 | 20.0 | 42.0 |
| [Mozilla、「Firefox 155」公開 - 脆弱性29件に対応](https://www.security-next.com/189716) | 22.0 | 20.0 | 42.0 |
| [「Chrome」にセキュリティ更新、脆弱性26件を修正 - 「Critical」2件](https://www.security-next.com/189711) | 22.0 | 20.0 | 42.0 |
| [「SonicWall SMA 1000」に深刻な脆弱性 - 悪用を示す事例も](https://www.security-next.com/189706) | 22.0 | 20.0 | 42.0 |
| [Omarchyで任意のユーザープロセスがルート権限に昇格可能の脆弱性、4.0.1へのアップデートで回避可能](https://gigazine.net/news/20260902-omarchy-root-creds/) | 22.0 | 20.0 | 42.0 |
| [まんだらけサーバに不正アクセス、「大オークション大会」の開催を延期](https://scan.netsecurity.ne.jp/article/2026/09/02/56109.html) | 21.0 | 20.0 | 42.0 |
| [イエローハットWEB作業予約システムへの不正プログラムによる攻撃、最大1,801,499名の会員情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/09/02/56108.html) | 21.0 | 20.0 | 42.0 |
| [「うんこミュージアム公式サイト」に不正アクセス、サイトの一部が改ざんされる被害](https://scan.netsecurity.ne.jp/article/2026/09/02/56107.html) | 21.0 | 20.0 | 42.0 |
| [不正アクセス関連損失として 1 億 8,100 万円を「その他の費用」に計上](https://scan.netsecurity.ne.jp/article/2026/09/02/56106.html) | 21.0 | 20.0 | 42.0 |
| [東京ガスネットワーク社員、飲酒して帰宅中に業務用パソコン紛失](https://scan.netsecurity.ne.jp/article/2026/09/02/56104.html) | 21.0 | 20.0 | 42.0 |
| [チャーム本店 1 号店及びチャーム本店 2 号店に不正アクセス、受注・出荷業務を停止](https://scan.netsecurity.ne.jp/article/2026/09/02/56103.html) | 21.0 | 20.0 | 42.0 |
| [ドライブレコーダーで紙片が飛ばされていく様子を確認 ～ 救急車の救急出場時に指令書を紛失](https://scan.netsecurity.ne.jp/article/2026/09/02/56102.html) | 21.0 | 20.0 | 42.0 |
| [NRIS、発注企業向け「SCS評価制度」対応支援 ～ Secure SketCH とコンサルの合わせ技](https://scan.netsecurity.ne.jp/article/2026/09/02/56101.html) | 21.0 | 20.0 | 42.0 |
| [スリーシェイク、Security Days Fall 2026 に「Securify」をブース出展 手塚卓也氏によるセッションも](https://scan.netsecurity.ne.jp/article/2026/09/02/56099.html) | 21.0 | 20.0 | 42.0 |
| [IPA、重要インフラ企業向けに「AIセキュリティトレーニング」10 / 26・27 開催](https://scan.netsecurity.ne.jp/article/2026/09/02/56098.html) | 21.0 | 20.0 | 42.0 |
| [被害企業の防止策 守りより「復旧力」へ](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/082700567/082700004/) | 21.0 | 20.0 | 42.0 |
| [18社が損失計上 海外拠点が標的に](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/082700567/082700002/) | 21.0 | 20.0 | 42.0 |
| [67％がSCS評価制度の取り組み進行 業務システムの共同利用は約9割](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020600010/082700232/) | 21.0 | 20.0 | 42.0 |
| [「社長の声」装い詐取 不正アクセスなき詐欺](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/082700567/082700001/) | 21.0 | 20.0 | 42.0 |
| [Weekly Report: Apache Tomcatに複数の脆弱性](https://www.jpcert.or.jp/wr/2026/wr260902.html) | 20.0 | 20.0 | 42.0 |
| [CISA ICS Advisory / ICS Medical Advisory（2026年09月01日）](https://jvn.jp/vu/JVNVU90253159/) | 20.0 | 20.0 | 42.0 |
| [FBI、1億5300万件超の運転免許証を販売するサービスを捜査](https://krebsonsecurity.com/2026/09/fbi-probes-service-selling-153m-drivers-licenses/) | 20.0 | 20.0 | 42.0 |
| [ブラジルポルトガル語のメールによるGuildma（Astaroth）マルウェア感染](https://isc.sans.edu/diary/rss/33300) | 20.0 | 20.0 | 42.0 |
| [HackersがFaronics Deploy管理ツールを悪用してScreenConnectをインストール](https://www.bleepingcomputer.com/news/security/hackers-abuse-faronics-deploy-admin-tool-to-install-screenconnect/) | 20.0 | 20.0 | 42.0 |
| [AttackerがMETR APIキーを盗み、60万ドル相当のクレジットを使用していたことに数週間誰も気づかなかった](https://www.theregister.com/security/2026/09/01/attacker-stole-a-metr-api-key-used-600k-worth-of-credits-and-no-one-noticed-for-weeks/5293730) | 20.0 | 20.0 | 42.0 |
| [Tina Peters、弁護士を通じてShasta County選挙での正式な役割を撤回](https://cyberscoop.com/tina-peters-shasta-county-election-role/) | 20.0 | 20.0 | 42.0 |
| [FirefoxがiPhoneユーザーのWeb広告を回避しつつ自社広告で収益化する仕組み](https://www.theregister.com/security/2026/09/01/firefox-helps-iphone-users-bypass-ads-on-web-sites-while-making-money-showing-its-own-ads/5293747) | 20.0 | 20.0 | 42.0 |

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
