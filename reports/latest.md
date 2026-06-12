# 📡 サイレーダー 2026-06-12 17:00 JST

このレポートは、2026-06-12 11:00 JST〜2026-06-12 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 43
- [音声で扱う想定のトピック](#audio-topics): 0
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 17

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Google Confirms Exploitation of Oracle PeopleSoft Zero-Day by ShinyHunters](#topic-16788) | 60.0 | 64.0 | 63.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

今回は音声で扱う想定のトピックはありません。

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-16788"></a>

### 1. Google Confirms Exploitation of Oracle PeopleSoft Zero-Day by ShinyHunters

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 60.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Oracle PeopleSoft Suiteの脆弱性「CVE-2026-35273」について、複数の報道でゼロデイとして扱われ、ShinyHuntersによるデータ窃取攻撃で悪用された可能性が伝えられています。
Oracleはこの問題への対処を進めているとされていますが、公開情報上では実地での悪用確認については報道ごとに表現差があります。
認証なしでのリモートコード実行につながる可能性があるとされ、影響範囲が広くなりやすい点が注目されています。
特に大学などの組織を含むデータ窃取型の攻撃文脈で語られており、早期の対処が重要です。

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

- PeopleSoft利用環境でCVE-2026-35273への対処状況を確認し、Oracleの案内に沿って修正や緩和策を適用する。
- 外部公開されたPeopleSoft関連の入口や不要な管理画面を見直し、アクセス制御と監視を強化する。
- 関連ログを点検し、想定外のアクセスやデータ取得の兆候がないかを確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-35273 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-35273](https://nvd.nist.gov/vuln/detail/CVE-2026-35273) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Google Confirms Exploitation of Oracle PeopleSoft Zero-Day by ShinyHunters](https://www.securityweek.com/google-confirms-exploitation-of-oracle-peoplesoft-zero-day-by-shinyhunters/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShinyHunters Exploits Oracle PeopleSoft Zero-Day (CVE-2026-35273) to Breach Univ](https://thehackernews.com/2026/06/shinyhunters-exploits-oracle-peoplesoft.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Oracle mitigates PeopleSoft zero-day exploited in data theft attacks](https://www.bleepingcomputer.com/news/security/oracle-mitigates-peoplesoft-zero-day-exploited-in-data-theft-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ShinyHunters hacked 100+ orgs by exploiting an Oracle PeopleSoft 0-day](https://www.theregister.com/cyber-crime/2026/06/11/shinyhunters-claims-oracle-peoplesoft-0-day-hit-100-orgs/5254443) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Oracle Addresses PeopleSoft Vulnerability Amid Reports of Zero-Day Attacks](https://www.securityweek.com/oracle-addresses-peoplesoft-vulnerability-amid-reports-of-zero-day-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内公式情報: なし。
- 国内メディア掲載: 未確認。
- 国内コミュニティ反応: 観測あり・信頼度: 低。
- 技術者コミュニティ反応: 観測あり・信頼度: 中。
- 開発者コミュニティ反応: 観測あり・信頼度: 中。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Googleが20億のWebを分析 AIを狙う「間接的プロンプトインジェクション」の実態](https://atmarkit.itmedia.co.jp/ait/articles/2606/12/news052.html) | 26.0 | 20.0 | 42.0 |
| [NISTとISOフレームワークを用いたAIエージェントのガバナンス方法](https://www.helpnetsecurity.com/2026/06/12/nist-iso-frameworks-govern-ai-agents/) | 25.0 | 20.0 | 42.0 |
| [ZeroFox、セキュリティチーム向けにAI Analyticsを提供開始](https://www.helpnetsecurity.com/2026/06/12/zerofox-ai-analytics-in-platform-security-reporting/) | 25.0 | 20.0 | 42.0 |
| [AI主権がデータセンターをサイバー作戦の戦略的標的にする](https://www.helpnetsecurity.com/2026/06/12/ai-sovereignty-data-centers/) | 25.0 | 20.0 | 42.0 |
| [OpenSSLに高危険度の脆弱性 発見にはClaudeが関与](https://atmarkit.itmedia.co.jp/ait/articles/2606/12/news055.html) | 24.0 | 20.0 | 43.0 |
| [crypton-x509-validationにおける不適切な証明書検証の脆弱性](https://jvn.jp/vu/JVNVU96130756/) | 23.0 | 20.0 | 43.0 |
| [5月下旬以降、「PeopleSoft」にゼロデイ攻撃 - 対策と侵害有無の調査を](https://www.security-next.com/185824) | 22.0 | 20.0 | 42.0 |
| [Homebrew 6.0.0が公開される、サードパーティーtapの信頼確認を導入しセキュリティ強化へ](https://gigazine.net/news/20260612-homebrew-6-0-0/) | 22.0 | 20.0 | 42.0 |
| [漏えい・脆弱なパスワードを1タップで自動更新 Appleが新機能を発表](https://atmarkit.itmedia.co.jp/ait/articles/2606/12/news057.html) | 21.0 | 20.0 | 42.0 |
| [AI活用のウイルス対策ソフトなど最新製品を展示、SCS評価制度の支援も](https://xtech.nikkei.com/atcl/nxt/column/18/03585/061200023/) | 21.0 | 20.0 | 42.0 |
| [MicrosoftのGitHubリポジトリ73件が侵害 AIコーディングツールにも拡大](https://news.mynavi.jp/techplus/article/20260612-4567579/) | 21.0 | 20.0 | 42.0 |
| [警視庁、メール受信者の注意力を逆手に取った「二段階式フィッシングメール」に注意喚起](https://internet.watch.impress.co.jp/docs/news/2116742.html) | 20.0 | 20.0 | 42.0 |
| [Tchapメッセンジャー侵害でフランス政府職員7万3000人超に影響](https://www.bleepingcomputer.com/news/security/french-govt-says-tchap-breach-affected-over-73-000-accounts/) | 20.0 | 20.0 | 42.0 |
| [Comcast Business SecurityEdge Preferred、小規模事業者向けのセキュリティを強化](https://www.helpnetsecurity.com/2026/06/12/comcast-business-securityedge-preferred-small-businesses/) | 20.0 | 20.0 | 42.0 |
| [150万件の悪性ドメインを支える製造ライン](https://www.helpnetsecurity.com/2026/06/12/malicious-domain-registration-research/) | 20.0 | 20.0 | 42.0 |
| [EuropeのデジタルIDウォレット、初の標準仕様を策定](https://www.helpnetsecurity.com/2026/06/12/etsi-eu-digital-identity-wallet/) | 20.0 | 20.0 | 42.0 |
| [今週の新しい情報セキュリティ製品：2026年6月12日](https://www.helpnetsecurity.com/2026/06/12/new-infosec-products-of-the-week-june-12-2026/) | 20.0 | 20.0 | 42.0 |

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
