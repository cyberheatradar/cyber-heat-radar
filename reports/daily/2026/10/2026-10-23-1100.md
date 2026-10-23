# 📡 サイレーダー 2026-10-23 11:00 JST

このレポートは、2026-10-23 05:00 JST〜2026-10-23 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 63
- [音声で扱う想定のトピック](#audio-topics): 0
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 38

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [PHP2Shell exploit bypasses protections designed to stop remote code execution](#topic-38753) | 66.0 | 74.0 | 67.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

今回は音声で扱う想定のトピックはありません。

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-38753"></a>

### 1. PHP2Shell exploit bypasses protections designed to stop remote code execution

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 66.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

PHPに存在するCVE-2026-109618を含む複数の脆弱性について、保護回避を伴うリモートコード実行の懸念が広がっています。
公開情報では、関連する検証コードやPoCの言及もあり、影響を受ける可能性のある環境では早急な対応が求められています。
認証なしでのコード実行につながる可能性があるため、サーバー侵害や情報漏えい、サービス停止に直結し得ます。
複数の製品・環境で影響が取り沙汰されており、広範な注意喚起が必要な事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 24 sources。
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

- PHP関連の修正版やベンダーの注意喚起を確認し、適用可能なものは速やかに更新する。
- 公開されている侵害痕跡や異常な挙動がないか、関連ログとWeb公開サービスを点検する。
- 影響範囲が大きい場合は、外部公開の縮小や一時的なアクセス制御など、暫定的なリスク低減策を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-109618 | 関連CVE | 1.00 | 候補あり（URL 77件以上） |
| 脆弱性 | CVE-2026-109619 | 関連CVE | 1.00 | 候補あり（URL 10件以上） |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-109618](https://nvd.nist.gov/vuln/detail/CVE-2026-109618) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-](https://security.paloaltonetworks.com/CVE-2026-109618) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [EOLのPHP 7.4、8.0、8.1にも異例のパッチ　JPCERT/CCが警告する「php2shell」の侵害痕跡3つと緊急対策](https://atmarkit.itmedia.co.jp/ait/articles/2610/23/news035.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in PHP Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-php-october26-Jj384Daq) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP2Shell exploit bypasses protections designed to stop remote code execution](https://www.theregister.com/security/2026/10/22/php2shell-exploit-bypasses-protections-designed-to-stop-remote-code-execution/5304883) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP2Shell puts dozens of UK government services out of service](https://www.theregister.com/security/2026/10/22/php2shell-puts-dozens-of-uk-government-services-out-of-service/5304840) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [New PHP2Shell scanner checks your hosts for CVE-2026-109618 and CVE-2026-109619](https://www.helpnetsecurity.com/2026/10/22/php2shell-scanner-tool/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP2Shell: Two Critical PHP Flaws Allow Unauthenticated Remote Code Execution](https://www.security.com/threat-intelligence/php2shell-critical-vulns-cve-2026-109618-109619) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（12件）。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Toronto crime tips org、データ侵害の詳細判明で業務停止](https://therecord.media/toronto-crime-tips-org-freezes-ops-after-breach) | 28.0 | 20.0 | 42.0 |
| [見逃されていたもの：連邦当局がテキサスのラップトップ農場を摘発](https://www.darkreading.com/insider-threats/texas-laptop-farms-north-korean-it-workers) | 28.0 | 20.0 | 42.0 |
| [「AIでエンジニア派遣は不要になる」のか？ 各社に肌感を聞いた 求められる人材、明確に変化](https://www.itmedia.co.jp/news/article/2610/23/2000002527/) | 26.0 | 20.0 | 42.0 |
| [OpenAIのAIエージェントが監視機能を無効化、指示を誤解して警告停止やコード削除](https://news.mynavi.jp/techplus/article/20261023-5175441/) | 26.0 | 20.0 | 42.0 |
| [大阪10/28・東京11/11・名古屋12/2開催 ネットワーク＆セキュリティ MeetUp! 2026 に「Cloudbase AI」を出展](https://scan.netsecurity.ne.jp/article/2026/10/23/56548.html) | 26.0 | 20.0 | 42.0 |
| [中国系攻撃者がAIエージェントで攻撃を自動化、「ConnectWise」のサプライチェーン攻撃に関与 Microsoftが警告](https://www.itmedia.co.jp/news/article/2610/23/2000002531/) | 26.0 | 20.0 | 42.0 |
| [Claude Coworkが仕様変更 企業の懸念は減るか増えるか？](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/052100111/102100189/) | 26.0 | 20.0 | 42.0 |
| [AIが「意思決定」まで担う時代に GitHubのプルリク承認機能](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/052100112/101600149/) | 26.0 | 20.0 | 42.0 |
| [国内で未曽有の情報漏洩事件 AIでサイバー攻撃にコスト革命](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/052100113/101600197/) | 26.0 | 20.0 | 42.0 |
| [AI時代のASPM 第2回：コードからクラウドまでの文脈で悪用可能なリスクを優先付けする](https://www.wiz.io/blog/aspm-ai-era-pt-2-prioritize-appsec-risk) | 25.0 | 20.0 | 42.0 |
| [「Node.<wbr>js」に脆弱性10件 - Brotli圧縮データの処理でRCEのおそれ](https://www.security-next.com/191807) | 22.0 | 20.0 | 42.0 |
| [HPEの無線LAN向けOSに多数の脆弱性 - クリティカルが33件](https://www.security-next.com/191821) | 22.0 | 20.0 | 42.0 |
| [NRIとNRIセキュア、AI駆動型サイバー攻撃に備える「サイバーレジリエンス経営支援」を開始](https://news.mynavi.jp/techplus/article/20261023-5178609/) | 21.0 | 20.0 | 42.0 |
| [証券口座で不正取引、金融サービスへのサイバー攻撃で何が起きている？](https://news.mynavi.jp/techplus/article/20261023-5178526/) | 21.0 | 20.0 | 42.0 |
| [PHP脆弱性「PHP2Shell」で2260万件に影響 情シスの緊急チェックリスト](https://techtarget.itmedia.co.jp/tt/article/2610/23/2000002526/) | 21.0 | 20.0 | 42.0 |
| [認証局eMudhra、SSL/TLS証明書事業から撤退へ 秘密鍵問題受け──既存顧客の証明書は無償で置き換え](https://www.itmedia.co.jp/news/article/2610/23/2000002534/) | 21.0 | 20.0 | 42.0 |
| [「お名前.com」 のFX自動売買VPS、不正アクセスで金銭被害か 「600万円の損失」「55万円なくなった」……報告相次ぐ](https://www.itmedia.co.jp/news/article/2610/23/2000002532/) | 21.0 | 20.0 | 42.0 |
| [AI時代のフィッシング詐欺に対する警告サインは何を重要とするべきか](https://ascii.jp/elem/000/004/443/4443596/?rss=) | 21.0 | 20.0 | 42.0 |
| [トホホすぎる「内製化率５０％」目標](https://scan.netsecurity.ne.jp/article/2026/10/23/56557.html) | 21.0 | 20.0 | 42.0 |
| [ふるさと納税ポータルサイト「ふるさとチョイス」に不正アクセス、泉大津市で寄附の受付ができない状況に](https://scan.netsecurity.ne.jp/article/2026/10/23/56556.html) | 21.0 | 20.0 | 42.0 |
| [中古車情報サイト「カーセンサーnet」と中古車販売店向け業務支援サービス「C-MATCH」への不正アクセス、最大3,709,551件の個人情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/10/23/56555.html) | 21.0 | 20.0 | 42.0 |
| [メール配信システム「ブラストメール」に不正アクセス、データ持ち出しを確認](https://scan.netsecurity.ne.jp/article/2026/10/23/56554.html) | 21.0 | 20.0 | 42.0 |
| [アバハウスインターナショナルに不正アクセス、複数の顧客からの問い合わせで発覚](https://scan.netsecurity.ne.jp/article/2026/10/23/56553.html) | 21.0 | 20.0 | 42.0 |
| [講談社BECK 従業員のメールアカウントに不正アクセス、50件の不審なメールを送信](https://scan.netsecurity.ne.jp/article/2026/10/23/56552.html) | 21.0 | 20.0 | 42.0 |
| [ムーンスターのサーバに不正アクセス、オンラインストアを利用した顧客情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/10/23/56551.html) | 21.0 | 20.0 | 42.0 |
| [セーファーインターネット協会が利用する「さくらのレンタルサーバ」に不正アクセス](https://scan.netsecurity.ne.jp/article/2026/10/23/56550.html) | 21.0 | 20.0 | 42.0 |
| [富士急ハイランド公式アプリ・会員サイト「CLUB フジQ」にリスト型攻撃、159名の会員情報が閲覧された可能性](https://scan.netsecurity.ne.jp/article/2026/10/23/56549.html) | 21.0 | 20.0 | 42.0 |
| [UnRTF に境界外書き込みの脆弱性](https://scan.netsecurity.ne.jp/article/2026/10/23/56547.html) | 21.0 | 20.0 | 42.0 |
| [複数の Lenovo 製タブレットの Android Verified Boot 機能に既知のテスト用鍵がそのまま使用されている問題](https://scan.netsecurity.ne.jp/article/2026/10/23/56546.html) | 21.0 | 20.0 | 42.0 |
| [アツミ電氣製 DVR に利用可能な非公開機能を悪用される問題](https://scan.netsecurity.ne.jp/article/2026/10/23/56545.html) | 21.0 | 20.0 | 42.0 |
| [GMOイエラエ 育休取得率 男性60％ 女性100％ ～ 厚労省「子育てサポート企業」に認定](https://scan.netsecurity.ne.jp/article/2026/10/23/56544.html) | 21.0 | 20.0 | 42.0 |
| [「自分たちの工場は自分たちで守る」 リコーが“リファレンス工場”から波及させたOTセキュリティ](https://ascii.jp/elem/000/004/443/4443693/?rss=) | 21.0 | 20.0 | 42.0 |
| [PHP脆弱性問題は“また起こる” 事件の裏にあったエンジニアの根深い課題](https://atmarkit.itmedia.co.jp/ait/articles/2610/23/news038.html) | 21.0 | 20.0 | 42.0 |
| [PHP2Shell、公表4日前に悪用の試み 「公表日より前にさかのぼって調査を」とAmazon](https://www.itmedia.co.jp/news/article/2610/23/2000002530/) | 21.0 | 20.0 | 42.0 |
| [Railway、潜在的な侵害を受け開発者にシークレットのローテーションを警告](https://www.bleepingcomputer.com/news/security/railway-warns-devs-to-rotate-secrets-after-potential-breach/) | 20.0 | 20.0 | 42.0 |
| [警視庁が個人情報漏えいに関する対策・啓発冊子を公開、都民向けと事業者向け](https://internet.watch.impress.co.jp/docs/news/2150370.html) | 20.0 | 20.0 | 42.0 |
| [Microsoft、ConnectWiseへのサプライチェーン攻撃にStorm-0940の関与を特定](https://www.darkreading.com/cyberattacks-data-breaches/microsoft-storm-0940-connectwise-supply-chain-attack) | 20.0 | 20.0 | 42.0 |
| [Capcom、1,170万アカウントに影響するデータ侵害を確認](https://www.bleepingcomputer.com/news/security/capcom-confirms-data-breach-affecting-117-million-accounts/) | 20.0 | 20.0 | 42.0 |

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
