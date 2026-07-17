# 📡 サイレーダー 2026-07-17 17:00 JST

このレポートは、2026-07-17 11:00 JST〜2026-07-17 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 53
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 26

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-58644: CISA KEV catalog addition](#topic-23002) | 41.0 | 64.0 | 51.0 | 音声 | 温度感上位枠 |
| 2 | [CISA urges immediate action on actively exploited Fortinet flaws](#topic-22999) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-23002"></a>

### 1. CVE-2026-58644: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 51.0 |

#### 概要

CISAは、Microsoft SharePoint Serverに影響するCVE-2026-58644をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
材料によると、この問題は重要度の高い脆弱性として扱われており、米連邦民間行政機関には2026年7月19日までの対応が求められています。
KEVへの追加は、実際に悪用が確認されている、または少なくとも優先対応が必要な脆弱性であることを示します。
SharePointは組織内で広く使われるため、影響範囲が大きくなりやすい点が注目されます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象のSharePoint ServerがCVE-2026-58644の修正適用済みか確認する。
- 資産管理上、公開・社内向けのSharePointインスタンスを洗い出し、未対応のものを優先する。
- CISA KEV対象であることを踏まえ、通常より早い期限でパッチ適用と状況確認を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-58644 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-58644](https://nvd.nist.gov/vuln/detail/CVE-2026-58644) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds Exploited SharePoint RCE Zero-Day CVE-2026-58644 to KEV](https://thehackernews.com/2026/07/cisa-adds-exploited-sharepoint-rce-zero.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-22999"></a>

### 2. CISA urges immediate action on actively exploited Fortinet flaws

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAが、FortinetのFortiSandboxに存在する2件の脆弱性について、政府機関に対して早急な対応を求めたと報じられています。
これらはすでに悪用が観測されているとされ、対象環境では優先的な修正が必要な状況です。セキュリティ製品そのものの脆弱性は、保護の起点が崩れるため影響が大きくなりやすいです。
特に悪用が確認されている場合、対応の遅れが侵害リスクの増大につながります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- FortiSandboxを利用している場合は、ベンダー情報とCISAの勧告を確認し、優先度を上げて更新・修正を適用する。
- 公開されている影響範囲と自組織の構成を照らし合わせ、該当有無を速やかに確認する。
- 関連機器や管理経路について、通常より厳しめに監視し、不審な挙動や設定変更の兆候を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2025-61624 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-21643 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-25089 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-39808 | 関連CVE | 1.00 | 候補あり（URL 3件以上） |
| 脆弱性 | CVE-2026-39813 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Fortinet | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA urges immediate action on actively exploited Fortinet flaws](https://www.bleepingcomputer.com/news/security/cisa-warns-feds-to-patch-exploited-fortinet-fortisandbox-flaws-by-sunday/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

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
| [Coca-Cola、ランサムウェア攻撃を受けて米国のFairlife生産を停止](https://www.securityweek.com/coca-cola-suspends-us-fairlife-production-due-to-ransomware-attack/) | 28.0 | 30.0 | 42.0 |
| [NECがTNFD対応のAIサービスを26年9月に提供開始、調査の作業時間を9割削減](https://xtech.nikkei.com/atcl/nxt/column/18/03682/071500009/) | 28.0 | 20.0 | 42.0 |
| [OpenAIのAIエージェントで中古車売買の顧客対応を自動化、サポート解決率50％向上・業務時間80％短縮・離脱顧客12％復帰などを達成した事例](https://gigazine.net/news/20260717-openai-cars24-agent/) | 27.0 | 20.0 | 42.0 |
| [Grokを悪用して児童性的虐待画像を作成した男性をSpaceXAIが提訴](https://gigazine.net/news/20260717-grok-csam-sue/) | 27.0 | 20.0 | 42.0 |
| [ローカルAIモデルをAIエージェントとして使える「LM Studio Bionic」が登場、コーディングやスライド作成に対応しクラウドモデルも使用可能](https://gigazine.net/news/20260717-lm-studio-bionic/) | 27.0 | 20.0 | 42.0 |
| [GoogleのAIまとめサービス・NotebookLMが「Gemini Notebook」に改名、GoogleサービスやGeminiとの連携も強化](https://gigazine.net/news/20260717-gemini-notebook/) | 27.0 | 20.0 | 42.0 |
| [Netflixでは生成AIが300作品でポスプロ工程などに活用されている](https://gigazine.net/news/20260717-netflix-gen-ai-title/) | 27.0 | 20.0 | 42.0 |
| [自律するAIエージェントの本番投入に潜むリスク、PwCが示す統制保証水準「AI-CAL」](https://japan.zdnet.com/article/35250726/) | 26.0 | 20.0 | 42.0 |
| [みずほFGがAIエージェント3000体構想、銀行業務全体をAI前提で再設計へ](https://xtech.nikkei.com/atcl/nxt/column/18/00001/11900/) | 26.0 | 20.0 | 42.0 |
| [中国AIも“ミュトス級”に到達か Moonshot AIが「Kimi K3」発表、一部ベンチでFable 5抜き首位](https://www.itmedia.co.jp/news/articles/2607/17/news079.html) | 26.0 | 20.0 | 42.0 |
| [AI音声フィッシングを成立させるのは声ではなくスクリプトです](https://www.helpnetsecurity.com/2026/07/17/research-ai-voice-phishing/) | 25.0 | 20.0 | 42.0 |
| [今週の新しい情報セキュリティ製品：2026年7月17日](https://www.helpnetsecurity.com/2026/07/17/new-infosec-products-of-the-week-july-17-2026/) | 25.0 | 20.0 | 42.0 |
| [データ分析可視化製品「Ivanti Xtraction」に複数脆弱性](https://www.security-next.com/187544) | 22.0 | 20.0 | 42.0 |
| [「FortiOS」に複数脆弱性 - アップデートで修正](https://www.security-next.com/187537) | 22.0 | 20.0 | 42.0 |
| [Microsoftが乗っ取られたアカウントをデータ保護のため永久停止、その後反発を受け復旧](https://gigazine.net/news/20260717-microsoft-restore-hacked-account/) | 22.0 | 20.0 | 42.0 |
| [「Dell PowerFlex」に深刻な脆弱性 - 6月の更新で修正済み](https://www.security-next.com/187531) | 22.0 | 20.0 | 42.0 |
| [社交不安を抱える人は「歩く人が自分の方に向かってきている」と感じやすいとの研究結果](https://gigazine.net/news/20260717-social-anxiety-perception-nearing-crowds/) | 22.0 | 20.0 | 42.0 |
| [Webエージェント時代のXSSとなりつつあるプロンプトインジェクション](https://www.helpnetsecurity.com/2026/07/17/xss-web-agent-prompt-injection/) | 21.0 | 26.0 | 42.0 |
| [キオクシア、約370億円の支払い命令に「到底容認できない」 控訴含む法的手段へ 米特許訴訟で](https://www.itmedia.co.jp/news/articles/2607/17/news097.html) | 21.0 | 20.0 | 42.0 |
| [2030年代の対応では手遅れ？ 暗号化されたデータを将来暴くサイバー攻撃、対策の道筋](https://atmarkit.itmedia.co.jp/ait/articles/2607/17/news057.html) | 21.0 | 20.0 | 42.0 |
| [公開直後に悪用された新たなSharePoint脆弱性](https://www.securityweek.com/fresh-sharepoint-vulnerability-exploited-soon-after-disclosure/) | 20.0 | 20.0 | 42.0 |
| [アジア太平洋地域で、EC・予約サービスを狙うAIボットの攻撃が急増、Akamaiが警告](https://internet.watch.impress.co.jp/docs/news/2126090.html) | 20.0 | 20.0 | 42.0 |
| [セキュリティ予算の無駄を削減する5つのステップ](https://www.helpnetsecurity.com/2026/07/17/security-budget-waste-video/) | 20.0 | 20.0 | 42.0 |
| [341,263台のハードドライブを対象にした、4TBから20TB超までの信頼性調査](https://www.helpnetsecurity.com/2026/07/17/hard-drive-reliability-2026-4tb-20tb/) | 20.0 | 20.0 | 42.0 |
| [CISA ICS Advisory / ICS Medical Advisory（2026年07月16日）](https://jvn.jp/vu/JVNVU95874748/) | 20.0 | 20.0 | 42.0 |
| [一部のHTTP/2サーバーにおけるフロー制御に起因したサービス拒否（DoS）の脆弱性](https://jvn.jp/vu/JVNVU90338324/) | 20.0 | 20.0 | 42.0 |

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
