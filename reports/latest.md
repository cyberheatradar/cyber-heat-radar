# 📡 サイレーダー 2026-10-22 11:00 JST

このレポートは、2026-10-22 05:00 JST〜2026-10-22 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 57
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 31

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Critical PHP Vulnerability (CVE-2026-109618, CVE-2026-109619) \[infocon yellow\], (Wed, Oct 21st)](#topic-38753) | 67.0 | 64.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [「まさかそこから」大阪公立大のランサム被害、NEC委託先への攻撃が発端と判明](#topic-38963) | 31.0 | 38.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-38963"></a>

### 1. 「まさかそこから」大阪公立大のランサム被害、NEC委託先への攻撃が発端と判明

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 31.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

NECは、システム開発・保守を委託していた先がサイバー攻撃を受けたことで、複数の顧客にシステム障害や情報漏えいが発生したと公表しました。
大阪公立大学で公表されていたランサムウェア被害についても、この事案の影響だったことが判明しています。
委託先を起点に複数組織へ影響が及ぶ事例であり、サプライチェーン経由のリスクを改めて示しています。自組織だけでなく、外部委託先のセキュリティ管理が被害拡大の分岐点になり得ます。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- 情報漏えい系。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 委託先・再委託先を含むアクセス権限、接続経路、保守運用の管理状況を再点検する。
- 障害時の影響範囲を素早く把握できるよう、委託先関連の資産・連携先の棚卸しを行う。
- 情報漏えいの可能性を前提に、通知・報告・初動対応の手順が機能するか確認する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [「まさかそこから」大阪公立大のランサム被害、NEC委託先への攻撃が発端と判明](https://atmarkit.itmedia.co.jp/ait/articles/2610/22/news019.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-38753"></a>

### 1. Critical PHP Vulnerability (CVE-2026-109618, CVE-2026-109619) [infocon yellow], (Wed, Oct 21st)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 67.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

PHPに関する2件の深刻な脆弱性（CVE-2026-109618、CVE-2026-109619）が公表され、認証なしのリモートコード実行につながる可能性があるとされています。
複数のセキュリティ関連ソースで注目されており、修正情報とあわせて対応が進んでいます。PHPは利用範囲が広いため、影響を受ける環境が多い可能性があります。
さらに、公開直後から悪用観測やPoCの言及があり、迅速な確認と更新が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 21 sources。
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

- PHPの利用有無と対象バージョンを確認し、該当する場合は修正版の適用を急ぐ。
- Web公開サービスや関連製品で、異常な挙動や不審なリクエストの有無を点検する。
- 影響範囲の大きい環境では、暫定的なアクセス制御や露出面の縮小を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-109618 | 関連CVE | 1.00 | 候補あり（URL 46件以上） |
| 脆弱性 | CVE-2026-109619 | 関連CVE | 1.00 | 候補あり（URL 7件以上） |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-109618](https://nvd.nist.gov/vuln/detail/CVE-2026-109618) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [PHPにおける複数の任意のコードが実行可能な脆弱性（CVE-2026-109618、CVE-2026-109619）](https://jvn.jp/vu/JVNVU99905564/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in PHP Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-php-october26-Jj384Daq) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [多くのサイトが予防的に公開停止、高市総理が対応呼びかけ―「PHPの深刻な脆弱性」対応で何が起きた？](https://internet.watch.impress.co.jp/docs/news/2150203.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-](https://security.paloaltonetworks.com/CVE-2026-109618) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical PHP Vulnerability (CVE-2026-109618, CVE-2026-109619) [infocon yellow], ](https://isc.sans.edu/diary/rss/33440) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP2Shell Patches Land as First Exploitation Attempts Hit Sensors](https://www.securityweek.com/php2shell-patches-land-as-first-exploitation-attempts-hit-sensors/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: Critical Vulnerabilities in PHP: CVE-2026-109618, CVE-2026-109619](https://unit42.paloaltonetworks.com/cve-2026-109618-cve-2026-109619/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（24件）。
- 国内開発者記事: 採用あり（2件）。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Smashing Security podcast #489: 新しい暗号資産ウォレットにスパイが潜んでいた理由](https://grahamcluley.com/smashing-security-podcast-489/) | 28.0 | 20.0 | 42.0 |
| [Chrome、非安全サイトを許可プロンプトの背後に配置](https://www.helpnetsecurity.com/2026/10/22/google-chrome-https-protection/) | 28.0 | 20.0 | 42.0 |
| [Onamae Desktop Cloudが不正アクセス被害、最大2万7000台のサーバーに影響](https://www.bleepingcomputer.com/news/security/japans-onamae-desktop-cloud-hacked-up-to-27-000-servers-affected/) | 28.0 | 20.0 | 42.0 |
| [Lazarusがマルウェア配布にポスト量子暗号を利用](https://www.bleepingcomputer.com/news/security/lazarus-hackers-use-post-quantum-cryptography-for-malware-delivery/) | 28.0 | 20.0 | 42.0 |
| [人間の指示なしでAIが自発的にタスクを実行するClaudeのエージェントアプリ「Claude Duet」が発表される](https://gigazine.net/news/20261022-claude-duet/) | 27.0 | 20.0 | 42.0 |
| [AIエージェントが攻撃者なしでデータを露出する場合](https://www.f5.com/labs/articles/unprompted-when-ai-agents-expose-data-without-an-attacker) | 27.0 | 20.0 | 42.0 |
| [Meta決算、売上高26％増も営業益37％減 AIエージェント「Muse」は1000万人超が利用開始](https://www.itmedia.co.jp/news/article/2610/22/2000002489/) | 26.0 | 20.0 | 42.0 |
| [Microsoftが社内AIエージェントを「内部脅威」と呼ぶ理由は？ 「3つの封じ込め策」とともに紹介](https://www.itmedia.co.jp/enterprise/articles/2610/21/news070.html) | 26.0 | 20.0 | 42.0 |
| [攻撃者のAIは「人間超え、寝ない」 それでも専門家が"最優先の脅威ではない"と言う理由](https://www.itmedia.co.jp/enterprise/articles/2610/15/news025.html) | 26.0 | 20.0 | 42.0 |
| [Google Chrome、Gemini搭載の詐欺検知機能を追加し、ClickFix攻撃に警告](https://www.bleepingcomputer.com/news/google/google-chrome-adds-gemini-powered-scam-detection-warns-users-of-clickfix-attacks/) | 25.0 | 20.0 | 42.0 |
| [Microsoft、ConnectWiseへのサプライチェーン攻撃を中国の国家関与型脅威グループに帰属と発表](https://cyberscoop.com/microsoft-attributes-connectwise-supply-chain-attack-china-storm-0940/) | 25.0 | 20.0 | 42.0 |
| [「Gemini Notebook」で名刺を文字起こしして管理！ PFUの小型スキャナー「ScanSnap iX110」活用【自宅Wi-Fiの“わからない”をスッキリ！】](https://internet.watch.impress.co.jp/docs/column/homewifi/2149233.html) | 25.0 | 20.0 | 42.0 |
| [ClaudeがOpenSSHなど25のOSSを解析、493件のセキュリティ問題を発見](https://news.mynavi.jp/techplus/article/20261022-5172686/) | 24.0 | 20.0 | 43.0 |
| [米当局、「PHP脆弱性」の即修正を勧告 - 困難ならオフラインに](https://www.security-next.com/191766) | 22.0 | 20.0 | 42.0 |
| [「GitLab」に深刻な脆弱性 - 旧ブランチにも修正を提供](https://www.security-next.com/191760) | 22.0 | 20.0 | 42.0 |
| [eMudhraで侵害された8つの認証局すべての秘密鍵はなんとたった「1バイト」で秘密鍵の1つは「4」、Mozilla・Microsoft・Apple・Chromeのルートプログラムや多くの下流トラストストアによって信頼されているルート証明書に連鎖](https://gigazine.net/news/20261022-emudhra-problem/) | 22.0 | 20.0 | 42.0 |
| [eMudhraの中間証明書の侵害](https://blog.talosintelligence.com/compromised-intermediate-certificates/) | 22.0 | 20.0 | 42.0 |
| [大阪大、学生など7.8万人の情報漏えい NECが無断で協力会社とデータ共有](https://www.itmedia.co.jp/news/article/2610/22/2000002491/) | 21.0 | 20.0 | 42.0 |
| [AIを悪用しながら進化するサイバー脅威に対する、防御の4つの基本方針とその実践方法に迫る](https://news.mynavi.jp/techplus/kikaku/20261022-5133861/) | 21.0 | 20.0 | 42.0 |
| [氏名入りフィッシングメールを確認、9月の報告件数は約15%増](https://news.mynavi.jp/techplus/article/20261022-5161358/) | 21.0 | 20.0 | 42.0 |
| [Tesla決算、営業益56％減 FSD契約は67％増の174万件 SpaceX合併は「昨日すべて話した」とマスク氏](https://www.itmedia.co.jp/news/article/2610/22/2000002488/) | 21.0 | 20.0 | 42.0 |
| [PHPの「重大」脆弱性はAIが見つけた 「GPT-5.6 Solで発見」とOpenAI 「今後、AIによる脆弱性発見が急増」](https://www.itmedia.co.jp/news/article/2610/22/2000002486/) | 21.0 | 20.0 | 42.0 |
| [Meta、Cambridge Analytica問題巡る訴訟で250億ドルの支払い命令](https://www.itmedia.co.jp/news/article/2610/22/2000002484/) | 21.0 | 20.0 | 42.0 |
| [高市総理「大至急、PHPパッチ適用を」Xで異例の要請 エンジニアは評価「経営層に伝わる」](https://www.itmedia.co.jp/news/article/2610/22/2000002483/) | 21.0 | 20.0 | 42.0 |
| [LIFF SDKにおけるクロスサイトスクリプティングの脆弱性](https://jvn.jp/vu/JVNVU91023667/) | 20.0 | 20.0 | 42.0 |
| [ISC BINDにおける複数の脆弱性（2026年10月）](https://jvn.jp/vu/JVNVU91196958/) | 20.0 | 20.0 | 42.0 |
| [PHP、サプライチェーンセキュリティ企業Chainguardをウェブの大部分を危険にさらしたとして非難](https://www.theregister.com/security/2026/10/22/php-blames-supply-chain-security-biz-chainguard-for-putting-huge-chunks-of-the-web-at-risk/5304611) | 20.0 | 20.0 | 42.0 |
| [PHPの脆弱性 米OpenAIのAIで発見](https://news.yahoo.co.jp/pickup/6599651?source=rss) | 20.0 | 20.0 | 42.0 |
| [TiDB侵害で露呈したクラウドセキュリティの誤った前提](https://www.darkreading.com/cloud-security/tidb-breach-flawed-cloud-security) | 20.0 | 20.0 | 42.0 |
| [Marvell、Microsoft、Oracleがデータセンター・ハードウェアセキュリティの標準化に取り組む](https://www.darkreading.com/cloud-security/marvell-microsoft-oracle-standardize-data-center-hardware-security) | 20.0 | 20.0 | 42.0 |
| [Cloud Security Allianceの調査、Data Loss Preventionはデータ漏えい発生後に検知することが多いと判明](https://www.darkreading.com/cloud-security/cloud-security-alliance-survey-data-loss-prevention-detects-data-loss) | 20.0 | 20.0 | 42.0 |

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
