# 📡 サイレーダー 2026-10-22 17:00 JST

このレポートは、2026-10-22 11:00 JST〜2026-10-22 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 65
- [音声で扱う想定のトピック](#audio-topics): 0
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 40

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [注意喚起: PHPにおける複数の脆弱性（CVE-2026-109618、CVE-2026-109619）に関する注意喚起 (公開)](#topic-38753) | 62.0 | 64.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

今回は音声で扱う想定のトピックはありません。

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-38753"></a>

### 1. 注意喚起: PHPにおける複数の脆弱性（CVE-2026-109618、CVE-2026-109619）に関する注意喚起 (公開)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 62.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

PHPにおける複数の脆弱性（CVE-2026-109618、CVE-2026-109619）について、JPCERT/CCやJVNが注意喚起を出しています。
報道や各種アドバイザリでは、任意コード実行につながる可能性が指摘されており、影響範囲の広さが懸念されています。
PHPは多くのWebサービスで使われているため、影響が出ると広範囲に及ぶ可能性があります。すでに関連する注意喚起や対策情報が出ていることから、早めの確認と更新対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 22 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
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

- 利用中のPHPバージョンと適用状況を確認し、修正版の有無を点検する。
- 公開中のWebアプリケーションについて、影響有無を優先的に洗い出す。
- ベンダーや公式アドバイザリの更新を継続監視し、必要に応じて緊急対応を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-109618 | 関連CVE | 1.00 | 候補あり（URL 47件以上） |
| 脆弱性 | CVE-2026-109619 | 関連CVE | 1.00 | 候補あり（URL 7件以上） |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-109618](https://nvd.nist.gov/vuln/detail/CVE-2026-109618) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: PHPにおける複数の脆弱性（CVE-2026-109618、CVE-2026-109619）に関する注意喚起  (公開)](https://www.jpcert.or.jp/at/2026/at260033.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHPにおける複数の任意のコードが実行可能な脆弱性（CVE-2026-109618、CVE-2026-109619）](https://jvn.jp/vu/JVNVU99905564/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in PHP Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-php-october26-Jj384Daq) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [多くのサイトが予防的に公開停止、高市総理が対応呼びかけ―「PHPの深刻な脆弱性」対応で何が起きた？](https://internet.watch.impress.co.jp/docs/news/2150203.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-](https://security.paloaltonetworks.com/CVE-2026-109618) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical PHP Vulnerability (CVE-2026-109618, CVE-2026-109619) [infocon yellow], ](https://isc.sans.edu/diary/rss/33440) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP2Shell Patches Land as First Exploitation Attempts Hit Sensors](https://www.securityweek.com/php2shell-patches-land-as-first-exploitation-attempts-hit-sensors/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（29件）。
- 国内開発者記事: 採用あり（2件）。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [「飲料メーカーA社」の被害事例を推察 ランサムウェア攻撃で今すぐ取り組むべき対策とは](https://atmarkit.itmedia.co.jp/ait/articles/2610/22/news031.html) | 29.0 | 30.0 | 42.0 |
| [APT41がBlackLotusブートキットを復活させ、中央アジアの外交機関を攻撃した件](https://securelist.com/uefi-bootkit-blackx/121539/) | 28.0 | 20.0 | 42.0 |
| [文化についてAIに質問すると日本が選ばれやすい傾向がある、8モデル・24言語で回答の偏りを調査](https://gigazine.net/news/20261022-llms-japanese-culture/) | 27.0 | 20.0 | 42.0 |
| [豪州でAI「Claude」に保育施設銃撃を予告したら逮捕 弁護側「耳感染症でストレス」](https://www.itmedia.co.jp/news/article/2610/22/2000002517/) | 26.0 | 20.0 | 42.0 |
| [Anthropic、Claudeでソフトウェアのアタックサーフェスを洗い出し・縮小する研究を公開 OpenSSHの修正にも貢献](https://www.itmedia.co.jp/news/article/2610/22/2000002498/) | 26.0 | 20.0 | 42.0 |
| [PHPに深刻な脆弱性 更新だけで対策は終わらない、企業が最初にやるべき2つのこと](https://www.itmedia.co.jp/enterprise/articles/2610/22/news054.html) | 25.0 | 38.0 | 42.0 |
| [月面で初のスーパーコンピューター性能テストをHPEとNASAが計画、AIによる地形解析やサイバー攻撃検知も実施へ](https://gigazine.net/news/20261022-hpt-nasa-moon-ai-benchmark/) | 25.0 | 20.0 | 43.0 |
| [AIエージェントの権限拡大がセキュリティ対策を上回っている](https://www.helpnetsecurity.com/2026/10/22/ai-agent-permissions-security/) | 25.0 | 20.0 | 42.0 |
| [少し話しかけただけで、仕組まれたAIが5000ドルを要求する](https://www.helpnetsecurity.com/2026/10/22/research-speech-model-backdoor/) | 25.0 | 20.0 | 42.0 |
| [UAE、政府サービスの50％をエージェント型AIに移行](https://www.darkreading.com/cybersecurity-operations/uae-transitions-50-government-services-agentic-ai) | 25.0 | 20.0 | 42.0 |
| [AIコーディングの急増がクラウド開発の脆弱性を露呈](https://www.helpnetsecurity.com/2026/10/22/localstack-ai-code-testing-report/) | 25.0 | 20.0 | 42.0 |
| [中国関連ハッカーがConnectWiseのサプライチェーン攻撃でARTEX AIエージェントを悪用](https://thehackernews.com/2026/10/china-linked-hackers-use-artex-ai.html) | 25.0 | 20.0 | 42.0 |
| [AIエージェントの可観測性はハルシネーションへの対応に苦戦している](https://www.helpnetsecurity.com/2026/10/22/ai-agent-observability-report/) | 25.0 | 20.0 | 42.0 |
| [PHPの「重大」脆弱性はAIが見つけた 「GPT-5.6 Solで発見」とOpenAI 「今後、AIによる脆弱性発見が急増」](https://www.itmedia.co.jp/news/article/2610/22/2000002486/) | 24.0 | 20.0 | 42.0 |
| [Node.<wbr>jsがセキュリティアップデートで「22.23.4」「24.22.1」「26.12.1」配信、全体で10件の脆弱性を修正](https://gigazine.net/news/20261022-node-js-security-releases/) | 22.0 | 20.0 | 42.0 |
| [「ロボットの赤ちゃん」で育児のシミュレーションをするだけでカップルのテストステロン値に変化が生じる](https://gigazine.net/news/20261022-couples-caregiving-robot-baby-testosterone/) | 22.0 | 20.0 | 42.0 |
| [Ciscoのビデオ会議製品に深刻な脆弱性 - 修正版が公開](https://www.security-next.com/191795) | 22.0 | 20.0 | 42.0 |
| [「PHP」の深刻なRCE脆弱性「PHP2Shell」 - 悪用試行を観測](https://www.security-next.com/191788) | 22.0 | 20.0 | 42.0 |
| [AIツール「LiteLLM」にパスワードを盗む不正プログラムが混入、インストールするだけで別のPythonプログラムにも影響](https://gigazine.net/news/20261022-litellm-backdoor/) | 22.0 | 20.0 | 42.0 |
| [GitLabが任意のコードを実行可能な危険度最大の脆弱性など12件に対するセキュリティパッチを公開](https://gigazine.net/news/20261022-gitlab-critical-patch/) | 22.0 | 20.0 | 42.0 |
| [「PHP脆弱性」が怖い理由 Webサイトの7割が利用、乗っ取られる恐れ](https://xtech.nikkei.com/atcl/nxt/column/18/00001/12118/) | 21.0 | 20.0 | 42.0 |
| [PHP「緊急」脆弱性悪用の試み、数百万件に CloudflareのCEOが報告](https://www.itmedia.co.jp/news/article/2610/22/2000002516/) | 21.0 | 20.0 | 42.0 |
| [PHP脆弱性、海外では“政府サイトごと停止”も オランダの電子認証やWikipedia関連サービスなどにも影響](https://www.itmedia.co.jp/news/article/2610/22/2000002514/) | 21.0 | 20.0 | 42.0 |
| [PHP脆弱性で高市総理「サイトを一時的に停止することも重要」](https://www.itmedia.co.jp/news/article/2610/22/2000002512/) | 21.0 | 20.0 | 42.0 |
| [PHPの重大脆弱性、情報流出と修正版の先行公開で混乱 - PHP財団が経緯公表](https://news.mynavi.jp/techplus/article/20261022-5173549/) | 21.0 | 20.0 | 42.0 |
| [Oracle Javaに55件の脆弱性 IPAが「早急に適用を」と促す対象は](https://www.itmedia.co.jp/enterprise/articles/2610/22/news058.html) | 21.0 | 20.0 | 42.0 |
| [PHPの重大脆弱性2件、1つはメモリー不足で悪用 増設だけでは防げず](https://xtech.nikkei.com/atcl/nxt/column/18/00001/12116/) | 21.0 | 20.0 | 42.0 |
| [PHP重大脆弱性、財団が「構造的な失敗」と認める 兆候は24年に把握](https://xtech.nikkei.com/atcl/nxt/column/18/00001/12115/) | 21.0 | 20.0 | 42.0 |
| [「GitLab」に深刻度“最大”の脆弱性 認証なしで任意のコード実行の恐れ、修正版適用を CVSS「10.0」](https://www.itmedia.co.jp/news/article/2610/22/2000002501/) | 21.0 | 20.0 | 42.0 |
| [コミックシーモア、流出は最大約420万件に メールアドレスや生年月日など 不正アクセスの経路特定・遮断は完了](https://www.itmedia.co.jp/news/article/2610/22/2000002500/) | 21.0 | 20.0 | 42.0 |
| [AKEY、Webサイト向け外部セキュリティ診断「SiteShield」を提供開始](https://news.mynavi.jp/techplus/article/20261022-5173138/) | 21.0 | 20.0 | 42.0 |
| [旅行ゲーム「ワールドクエスト」、PHP脆弱性で即日サービス終了 「古い仕組みのため対策とれず」](https://www.itmedia.co.jp/news/article/2610/22/2000002493/) | 21.0 | 20.0 | 42.0 |
| [認証局eMudhraの中間証明書、秘密鍵が「数ミリ秒」で復元可能な脆弱性 大手各社が緊急遮断](https://www.itmedia.co.jp/news/article/2610/21/2000002444/) | 20.0 | 20.0 | 43.0 |
| [Meta、Facebookのプライバシーに関して利用者を欺いたとしてニューメキシコ州に250億ドルの支払いを命じられる](https://www.securityweek.com/meta-ordered-to-pay-new-mexico-25-billion-for-deceiving-users-about-privacy-on-facebook/) | 20.0 | 20.0 | 42.0 |
| [認証局eMudhraが極めて弱い秘密鍵を擁護](https://www.theregister.com/security/2026/10/22/certification-authority-emudhra-defends-its-laughably-weak-private-keys/5304647) | 20.0 | 20.0 | 42.0 |
| [バルテック、「PHPの脆弱性を標的としたサイバー攻撃」によりサービス停止、情報流出の可能性](https://internet.watch.impress.co.jp/docs/news/2150396.html) | 20.0 | 20.0 | 42.0 |
| [主権とセキュリティをめぐる論点：MicrosoftのRoger Halbheer氏が指摘する問いのずれ](https://www.helpnetsecurity.com/2026/10/22/roger-halbheer-microsoft-data-sovereignty/) | 20.0 | 20.0 | 42.0 |
| [「2年前から兆候把握」も修正できず…AIが暴いたPHP重大欠陥、開発元の“構造的失敗”](https://www.sbbit.jp/article/cont1/187680?ref=rss) | 20.0 | 20.0 | 42.0 |
| [PHPの脆弱性 10年以上発見されず](https://news.yahoo.co.jp/pickup/6599674?source=rss) | 20.0 | 20.0 | 42.0 |
| [「侵入経路塞いだが、バックドアから……」不正アクセス105時間の攻防、分単位で報告 防災メールのアルカディア](https://www.itmedia.co.jp/news/article/2610/20/2000002426/) | 10.0 | 20.0 | 42.0 |

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
