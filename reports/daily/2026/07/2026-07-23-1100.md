# 📡 サイレーダー 2026-07-23 11:00 JST

このレポートは、2026-07-23 05:00 JST〜2026-07-23 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 59
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 30

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks](#topic-216) | 72.0 | 99.0 | 92.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [wp2shell hits WordPress: detecting pre-auth RCE from plugin drop to command execution](#topic-23164) | 47.0 | 74.0 | 67.0 | 音声 | 温度感上位枠 |
| 3 | [AI作成メールのクリック率は人間と同等に 年1回のセキュリティ教育では防御困難か](#topic-23840) | 34.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Attackers Are Learning to Live Off the AI Toolchain](#topic-23889) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-23164"></a>

### 1. wp2shell hits WordPress: detecting pre-auth RCE from plugin drop to command execution

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>Exploit Kit</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 47.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

WordPress Coreに関連するCVE-2026-63030について、複数のセキュリティ情報で検証・悪用の文脈が報告されています。
公開情報では、認証前のリモートコード実行につながりうる脆弱性として扱われ、影響版には修正版が案内されています。
WordPressは広く使われているため、公開サイトへの影響が大きくなりやすい点が注目されています。公開PoCや実運用での悪用を示す情報がある場合、修正の優先度は高くなります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
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

- WordPress Coreを利用しているインターネット公開環境は、該当バージョンかどうかを確認し、修正版への更新を優先する。
- 自動更新の有無にかかわらず、実際に最新の修正版へ更新できているかを各サイト単位で点検する。
- WAFや監視で不審な管理操作・ファイル生成・Webシェル設置の兆候を確認し、侵害の有無を併せて点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-60137 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-63030 | 関連CVE | 1.00 | 候補あり（URL 23件以上） |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| 製品 | WordPress | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-63030](https://nvd.nist.gov/vuln/detail/CVE-2026-63030) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [wp2shell hits WordPress: detecting pre-auth RCE from plugin drop to command exec](https://www.elastic.co/security-labs/wp2shell-wordpress-rce-detection-elastic-defend) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical wp2shell WordPress flaws exploited to install webshells](https://www.bleepingcomputer.com/news/security/critical-wp2shell-wordpress-flaws-exploited-to-install-webshells/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [WordPress wp2shell Exploitation Grows as Public Exploit Fuels Mass Scanning](https://thehackernews.com/2026/07/wordpress-wp2shell-exploitation-grows.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [WordPress Exploitation Underway (CVE-2026-63030), (Mon, Jul 20th)](https://isc.sans.edu/diary/rss/33168) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Exploitation in the Wild of wp2shell](https://www.wiz.io/blog/wp2shell-cve-2026-63030-cve-2026-60137) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-63030: wp2shell a Critical Remote Code Execution Vulnerability in WordP](https://www.rapid7.com/blog/post/etr-cve-2026-63030-wp2shell-a-critical-remote-code-execution-vulnerability-in-wordpress-core) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-23840"></a>

### 2. AI作成メールのクリック率は人間と同等に 年1回のセキュリティ教育では防御困難か

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 34.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

生成AIの普及により、メールを使ったフィッシングやビジネスメール詐欺の手口がより精巧になっていると報じられました。
AIで作成されたメールは、受信者のクリック率が人間作成のものと同程度になり得るとされ、従来の年1回の教育だけでは十分に防ぎにくい可能性が示されています。
メール攻撃は依然として侵入の入口になりやすく、AIによって見分けにくさが増すと、人的な注意だけではリスクを抑えにくくなります。
技術対策に加えて、継続的な訓練や人の行動リスクを前提にした対策が重要になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 年次一回の研修に依存せず、継続的な訓練や注意喚起の仕組みを見直す。
- メールの真正性確認を補強するため、送信元確認や承認フローなど業務手順を再点検する。
- フィッシング対策製品だけでなく、ビジネスメール詐欺やディープフェイクを含む人的リスク管理を組み合わせる。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [AI作成メールのクリック率は人間と同等に　年1回のセキュリティ教育では防御困難か](https://www.itmedia.co.jp/enterprise/articles/2607/23/news043.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23889"></a>

### 3. Attackers Are Learning to Live Off the AI Toolchain

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

攻撃者が、AIツールやその周辺のワークフローを悪用して、通常の利用と見分けにくい形で不正活動を行う動きが指摘されています。
材料では、信頼されているAIツール群を前提にしたマルウェアの例として Sandworm_Mode が言及されています。現時点では初期的な事例として扱うのが適切です。
AI開発・運用の中に攻撃が紛れ込むと、従来の検知や監査だけでは異常を見つけにくくなる可能性があります。
AI導入が進む組織ほど、ツール連携や権限管理を含めた見直しが重要になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AIツール、API、補助ワークフローの権限を最小化し、不要な連携を整理する。
- 通常の利用パターンに紛れる挙動を想定し、ログの相関監視や監査証跡の保全を強化する。
- AI関連資産を資産台帳に含め、更新・接続先・第三者連携の変更管理を明確にする。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Attackers Are Learning to Live Off the AI Toolchain](https://www.darkreading.com/cyber-risk/attackers-live-off-ai-toolchain) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-216"></a>

### 1. CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> / <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 72.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 99.0 |
| <nobr>確⁠度</nobr> | 92.0 |

#### 概要

cPanel & WHMに存在する認証回避の脆弱性「CVE-2026-41940」について、実際の悪用が確認されているとする複数の報道や分析が出ています。
関連情報では、攻撃者が侵害した環境で管理権限に近い操作を狙い、ランサムウェア攻撃やバックドア設置につながった可能性が示されています。
cPanel & WHMはホスティング環境で広く使われるため、影響を受けると複数のサイトや顧客環境に波及し得ます。
公開PoCや悪用報告がある状況では、未対応環境が短期間で攻撃対象になりやすく、優先度の高い確認が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 10 sources。
- CISA KEV関連。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- cPanel & WHMの利用有無を確認し、該当バージョンが影響範囲に入るか早急に洗い出す。
- ベンダー提供の修正情報を確認し、適用状況と未適用ホストを優先的に是正する。
- 管理画面への不審なログインや設定変更、予期しないファイル配置などの痕跡を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2023-1389 | 関連CVE | 1.00 | 候補あり（URL 5件以上） |
| 脆弱性 | CVE-2026-0265 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-10520 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-10523 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-26268 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-33032 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-35273 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-41940 | 関連CVE | 1.00 | 候補あり（URL 14件以上） |
| 脆弱性 | CVE-2026-42208 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-50751 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-41940](https://nvd.nist.gov/vuln/detail/CVE-2026-41940) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Large-Scale GitHub Actions Abuse Powers a Distributed cPanel and WHM Exploitatio](https://socket.dev/blog/github-actions-abuse-powers-cpanel-and-whm-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [What’s New in Rapid7 Products and Services: Q2 2026 in Review](https://www.rapid7.com/blog/post/pt-new-products-services-q2-2026-mdr) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Weekly Report: Apache Camelに複数の脆弱性](https://www.jpcert.or.jp/wr/2026/wr260513.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Stealthy hackers exploit cPanel flaw in active backdoor campaign (CVE-2026-41940](https://www.helpnetsecurity.com/2026/05/12/cpanel-vulnerability-exploited-backdoor-cve-2026-41940/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [cPanel CVE-2026-41940 Under Active Exploitation to Deploy Filemanager Backdoor](https://thehackernews.com/2026/05/cpanel-cve-2026-41940-under-active.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Week in review: cPanel vulnerability actively exploited, DigiCert breach, Linked](https://www.helpnetsecurity.com/2026/05/10/week-in-review-cpanel-vulnerability-actively-exploited-digicert-breach-linkedin-job-scams/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [4th May – Threat Intelligence Report](https://research.checkpoint.com/2026/4th-may-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 採用あり（1件）。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [一般社団法人日本ご当地キャラクター協会の NAS がランサムウェア感染](https://scan.netsecurity.ne.jp/article/2026/07/23/55763.html) | 29.0 | 30.0 | 42.0 |
| [“交渉人”なのに犯人と内通、計120億円超の身代金吊り上げ セキュリティ企業の元従業員に禁錮刑 米国](https://www.itmedia.co.jp/news/articles/2607/22/news038.html) | 29.0 | 30.0 | 42.0 |
| [日本の冷凍食品チェーンを襲ったランサムウェア攻撃](https://www.darkreading.com/cyberattacks-data-breaches/ransomware-attack-japanese-frozen-food-chain) | 28.0 | 30.0 | 42.0 |
| [Weekly Report: JPCERT/CCが「APT-C-60による2026年の攻撃」を公開](https://www.jpcert.or.jp/wr/2026/wr260723.html) | 28.0 | 20.0 | 42.0 |
| [AIは何度も話しかけると“落ちる” ガードレール突破検証で分かった最も安全なLLM](https://atmarkit.itmedia.co.jp/ait/articles/2607/23/news056.html) | 28.0 | 20.0 | 42.0 |
| [Upbound、侵害によりAcimaのリース契約で1,300万ドルの不正発生と発表](https://www.bleepingcomputer.com/news/security/upbound-says-hack-caused-13-million-in-fraudulent-acima-leases/) | 28.0 | 20.0 | 42.0 |
| [AI エージェントのセキュリティをどう担保するか？ Okta Japan が 8 / 5 に最新アップデート公開](https://scan.netsecurity.ne.jp/article/2026/07/23/55766.html) | 26.0 | 20.0 | 42.0 |
| [Drupal プラグイン「AI Agents」に不正な認証の脆弱性](https://scan.netsecurity.ne.jp/article/2026/07/23/55761.html) | 26.0 | 20.0 | 42.0 |
| [AI ツールの脆弱性登録が増加傾向、OpenClaw や Open WebUI もランクイン ～ 2026年 第2四半期「JVN iPedia」登録状況](https://scan.netsecurity.ne.jp/article/2026/07/23/55756.html) | 26.0 | 20.0 | 42.0 |
| [Umiosが販売計画をAIで自動化 時系列基盤モデル採用で精度95％](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/071301465/) | 26.0 | 20.0 | 42.0 |
| [JR九州、故障検知システムを構築 車両検査のAIエージェントと一体運用](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/071301470/) | 26.0 | 20.0 | 42.0 |
| [OpenAIがHugging Face攻撃で自滅、中国製オープンモデルの優位を示す](https://www.theregister.com/ai-and-ml/2026/07/23/openai-scored-an-own-goal-with-huggingface-attack-showing-how-open-chinese-models-are-winning/5276699) | 25.0 | 20.0 | 42.0 |
| [Check Point製品の管理機能に脆弱性 - すでに悪用も、侵害調査を](https://www.security-next.com/187730) | 22.0 | 20.0 | 42.0 |
| [富山県立大学の Microsoft 365 学生アカウントから大量の迷惑メール送信](https://scan.netsecurity.ne.jp/article/2026/07/23/55765.html) | 21.0 | 20.0 | 42.0 |
| [日本大学の学生・卒業生 9 名のアカウントに不正アクセス、スパムメール送信の踏み台に](https://scan.netsecurity.ne.jp/article/2026/07/23/55764.html) | 21.0 | 20.0 | 42.0 |
| [取引先装うフィッシングメール受信、偽サイトでメールアカウントの認証情報入力](https://scan.netsecurity.ne.jp/article/2026/07/23/55762.html) | 21.0 | 20.0 | 42.0 |
| [非接触型ICカード技術 FeliCa の一部のICチップに脆弱性](https://scan.netsecurity.ne.jp/article/2026/07/23/55760.html) | 21.0 | 20.0 | 42.0 |
| [WordPress の深刻度「緊急」脆弱性「wp2shell 」の概要と対応指針 ～ GMO Flatt Security 解説](https://scan.netsecurity.ne.jp/article/2026/07/23/55759.html) | 21.0 | 20.0 | 42.0 |
| [日立システムズと MBSD が協業「Fusion SOCサービス」立ち上げ](https://scan.netsecurity.ne.jp/article/2026/07/23/55758.html) | 21.0 | 20.0 | 42.0 |
| [HENNGE、コーポレートエンジニア向けコミュニティ「情シスSlack（corp-engr）」のスポンサーに](https://scan.netsecurity.ne.jp/article/2026/07/23/55757.html) | 21.0 | 20.0 | 42.0 |
| [千葉県市原市の児童生徒に「i-フィルター 10 小中学生版」を無償提供](https://scan.netsecurity.ne.jp/article/2026/07/23/55755.html) | 21.0 | 20.0 | 42.0 |
| [仙台市で「東北サイバーセキュリティシンポジウム2026」を 11 / 25 ～ 26 開催](https://scan.netsecurity.ne.jp/article/2026/07/23/55754.html) | 21.0 | 20.0 | 42.0 |
| [26年度末開始「SCS評価制度」に脚光 供給網のサイバー対策を客観評価](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/020800017/071301466/) | 21.0 | 20.0 | 42.0 |
| [Linuxカーネルで432件のCVEが一斉公開 「重要な脆弱性だけ直す」運用は限界か](https://atmarkit.itmedia.co.jp/ait/articles/2607/23/news032.html) | 21.0 | 20.0 | 42.0 |
| [VLANでホームネットワークのセキュリティを強化するには--仕組みと導入手順を解説](https://japan.zdnet.com/article/35250843/) | 21.0 | 20.0 | 42.0 |
| [予定表招待「はい」で情報流出 Geminiを狙う攻撃の手口](https://www.itmedia.co.jp/enterprise/articles/2607/23/news045.html) | 21.0 | 20.0 | 42.0 |
| [高2が700万件漏えいに関与も……目立つ若年層のサイバー犯罪に「ホワイトハッカーにすれば」が安直なワケ](https://www.itmedia.co.jp/news/articles/2607/23/news021.html) | 21.0 | 20.0 | 42.0 |
| [Smashing Security podcast #477: 14件のチキンマックナゲット注文がロシア人ハッカー容疑者逮捕の手がかりに](https://grahamcluley.com/smashing-security-podcast-477/) | 20.0 | 20.0 | 42.0 |
| [連邦政府のサイバーセキュリティ報告ルールの多くは重複していると調査で判明](https://cyberscoop.com/gao-report-duplicate-cybersecurity-regulations-harmonization/) | 20.0 | 20.0 | 42.0 |
| [世界の外交官に影響したデータ侵害を韓国が公表](https://www.bleepingcomputer.com/news/security/south-korea-discloses-data-breach-impacting-diplomats-worldwide/) | 20.0 | 20.0 | 42.0 |

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
