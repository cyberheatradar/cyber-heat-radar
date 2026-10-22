# 📡 サイレーダー 2026-10-23 05:00 JST

このレポートは、2026-10-22 17:00 JST〜2026-10-23 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 114
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 85

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [PHP2Shell: Two Critical PHP Flaws Allow Unauthenticated Remote Code Execution](#topic-38753) | 66.0 | 74.0 | 67.0 | 音声 | 温度感上位枠 |
| 2 | [Two CVSS 9.0 Linux KSMBD RCE Flaws Disclosed on Public Mailing Lists Before Kernel Fixes](#topic-39056) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [Arista patches new VeloCloud Orchestrator zero-day exploited in attacks](#topic-39054) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [LiteLLM Suspects GitHub Token Leak in AI Gateway Logs Behind Malicious Package Release](#topic-39154) | 33.0 | 45.0 | 42.0 | 音声 | AI×Security枠 |
| 5 | [Microsoft: Chinese State Actor Used AI to Compromise ConnectWise Tenants](#topic-39128) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-38753"></a>

### 1. PHP2Shell: Two Critical PHP Flaws Allow Unauthenticated Remote Code Execution

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 66.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

PHPにおける2件の重大な脆弱性が公表され、未認証でリモートコード実行につながる可能性があるとされています。
CVE-2026-109618とCVE-2026-109619として追跡されており、複数のセキュリティ関連組織やベンダーが注意喚起しています。
Webアプリの基盤として広く使われるPHPに関わるため、影響範囲が大きくなる可能性があります。
公開情報では検証コードや関連ツールの言及もあり、対応の遅れがリスクにつながりやすい状況です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 23 sources。
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

- PHPの導入有無とバージョンを棚卸しし、影響を受ける構成がないか確認する。
- 関連する公式アドバイザリやベンダー情報を確認し、修正版の適用状況を点検する。
- Web公開サーバーや主要CMS、周辺ミドルウェアの監視を強化し、異常な挙動がないか確認する。

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
| <nobr>出典</nobr> | [PHP2Shell puts dozens of UK government services out of service](https://www.theregister.com/security/2026/10/22/php2shell-puts-dozens-of-uk-government-services-out-of-service/5304840) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in PHP Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-php-october26-Jj384Daq) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [New PHP2Shell scanner checks your hosts for CVE-2026-109618 and CVE-2026-109619](https://www.helpnetsecurity.com/2026/10/22/php2shell-scanner-tool/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP2Shell: Two Critical PHP Flaws Allow Unauthenticated Remote Code Execution](https://www.security.com/threat-intelligence/php2shell-critical-vulns-cve-2026-109618-109619) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: PHPにおける複数の脆弱性（CVE-2026-109618、CVE-2026-109619）に関する注意喚起  (公開)](https://www.jpcert.or.jp/at/2026/at260033.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHPにおける複数の任意のコードが実行可能な脆弱性（CVE-2026-109618、CVE-2026-109619）](https://jvn.jp/vu/JVNVU99905564/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [多くのサイトが予防的に公開停止、高市総理が対応呼びかけ―「PHPの深刻な脆弱性」対応で何が起きた？](https://internet.watch.impress.co.jp/docs/news/2150203.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（36件）。
- 国内開発者記事: 採用あり（1件）。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-39056"></a>

### 2. Two CVSS 9.0 Linux KSMBD RCE Flaws Disclosed on Public Mailing Lists Before Kernel Fixes

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>R⁠C⁠E</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Linuxカーネル内のSMBサーバー機能「KSMBD」に、CVSS 9.0とされるリモートコード実行の脆弱性が2件公表されました。
現時点では主系統のカーネルに修正が入っていないとされ、少なくとも一方はネットワーク認証前に到達し得ると説明されています。
KSMBDを有効にしているLinuxサーバーでは、影響範囲が大きい可能性があるため注意が必要です。認証前に成立し得る経路が示されている点は、優先度を高めて評価すべき材料です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- KSMBDの利用有無と公開範囲を確認し、該当サーバーを特定する。
- ベンダーや配布元の修正版・回避策の案内を継続確認し、適用可能なら速やかに反映する。
- SMB関連の外部到達性を見直し、不要な公開や露出を抑える。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Trend Micro | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Two CVSS 9.0 Linux KSMBD RCE Flaws Disclosed on Public Mailing Lists Before Kern](https://thehackernews.com/2026/10/two-cvss-90-linux-ksmbd-rce-flaws.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-39054"></a>

### 3. Arista patches new VeloCloud Orchestrator zero-day exploited in attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Arista Networksは、VeloCloud Orchestrator（VCO）のオンプレミス環境に影響するゼロデイ脆弱性に対するセキュリティ更新を公開しました。
公開情報によると、この脆弱性は攻撃で実際に悪用されていたとされています。ネットワーク管理基盤に関わる製品の脆弱性は、影響範囲が大きくなりやすいため注目されます。
すでに悪用が確認されている点から、対応の遅れがリスクにつながる可能性があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- VeloCloud Orchestratorのオンプレミス環境を利用している場合は、提供済みの修正情報を確認し、速やかに適用可否を判断する。
- 公開情報で示された影響範囲と自組織の構成を照合し、該当有無を確認する。
- 脆弱性対応とあわせて、関連ログの確認や異常兆候の有無を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-114625 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Arista patches new VeloCloud Orchestrator zero-day exploited in attacks](https://www.bleepingcomputer.com/news/security/arista-patches-new-velocloud-orchestrator-zero-day-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-39154"></a>

### 4. LiteLLM Suspects GitHub Token Leak in AI Gateway Logs Behind Malicious Package Release

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 45.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

LiteLLMは、GitHubトークンの漏えいがAIゲートウェイのログに残っていた可能性があるとして、悪意あるPythonパッケージ公開につながった疑いを公表しました。
公開された不正バージョンには、認証情報を盗む機能やバックドアが含まれていたとされています。
PyPIやDocker Hubを介したサプライチェーン侵害は、利用者側の環境やCI/CDに波及する恐れがあります。
AI関連サービスの運用ログやトークン管理が、間接的に重大な公開事故につながり得る点も注目されます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- パッケージ更新時は、署名・ハッシュ・公開元の整合性確認を徹底する。
- CI/CDやリリース基盤で使うトークンの権限を最小化し、漏えい時の失効手順を明確にしておく。
- AIゲートウェイや関連ログに機密情報が含まれていないか定期的に点検し、不要な出力を抑制する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [LiteLLM Suspects GitHub Token Leak in AI Gateway Logs Behind Malicious Package R](https://thehackernews.com/2026/10/litellm-suspects-github-token-leak-in.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-39128"></a>

### 5. Microsoft: Chinese State Actor Used AI to Compromise ConnectWise Tenants

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftによると、複数のConnectWise顧客環境で脅威アクターの活動が確認され、攻撃側がARTEXというエージェント型AIプラットフォームを利用していたとされています。
現時点では、公開情報ベースでの観測内容であり、詳細な影響範囲や手口の全容は断定できません。AIを悪用した攻撃が、実在の企業環境に対する侵害で観測された点が注目されています。
管理ツールや業務基盤に関わるサービスでは、サプライチェーンや運用経路を含めた監視強化の重要性が改めて示されます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ConnectWise関連環境の監査ログや認証イベントを点検し、不審なアクセスや通常と異なる操作がないか確認する。
- 管理者権限・APIキー・連携アカウントの棚卸しを行い、不要な権限や古い資格情報を見直す。
- AI支援型の不審な活動も想定し、アラート設計やインシデント対応手順を更新する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | ConnectWise | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft: Chinese State Actor Used AI to Compromise ConnectWise Tenants](https://www.infosecurity-magazine.com/news/microsoft-chinese-ai-connectwise/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
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
| [誰も管理していないAIエージェント：最新の内部脅威について専門家ウェビナーを見る](https://thehackernews.com/2026/10/the-ai-agent-nobody-owns-watch-expert.html) | 33.0 | 20.0 | 42.0 |
| [LiteLLMが今年2件目のサプライチェーン攻撃を受け、利用者に認証情報のローテーションを呼びかけ](https://www.helpnetsecurity.com/2026/10/22/litellm-compromised-supply-chain-attack-pypi-docker/) | 28.0 | 45.0 | 42.0 |
| [ランサムウェア関連の法執行・司法措置](https://therecord.media/africa-cybercrime-interpol-arrests) | 28.0 | 30.0 | 42.0 |
| [LiteLLMのリリースパイプラインが侵害され情報窃取マルウェアを配布](https://www.bleepingcomputer.com/news/security/litellm-release-pipeline-hacked-to-distribute-info-stealer-malware/) | 28.0 | 20.0 | 42.0 |
| [イランのハッキンググループが米国でC2インフラを運用していたことが判明](https://www.infosecurity-magazine.com/news/iranian-hacking-group-hosting-c2/) | 28.0 | 20.0 | 42.0 |
| [大規模なコンプライアンスのローカライズ：韓国のISMS認証取得](https://blog.cloudflare.com/k-isms/) | 28.0 | 20.0 | 42.0 |
| [M365トークンスプレーとリプレイ攻撃によるビジネスメールアカウント侵害](https://www.huntress.com/blog/token-replay-spray) | 28.0 | 20.0 | 42.0 |
| [Cisco複数製品のSnort 3セキュリティ強化リリース：2026年10月](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-hardening-snort3-ybgmhTQe) | 27.0 | 46.0 | 51.0 |
| [ChatGPTやGeminiの性格診断結果をArtificial Analysisが公開、Gemini 4 Argonは媚びやすくClaude Fable 5.1は説得力がある](https://gigazine.net/news/20261022-artificial-analysis-personalitybench/) | 27.0 | 20.0 | 42.0 |
| [数千体のAIが数百万個の脳細胞データをわずか32分で分析、アルツハイマー病やパーキンソン病の研究につながる新たな手掛かりを発見](https://gigazine.net/news/20261022-openai-research-complex-biological-data/) | 27.0 | 20.0 | 42.0 |
| [ThreatsDay: AIの機密漏えい、PingCAPのソースコード窃取、Signalのハングアップ不具合、Laravelの認証バイパスほか21件](https://thehackernews.com/2026/10/threatsday-ai-secrets-leak-pingcap.html) | 25.0 | 20.0 | 42.0 |
| [蒸留攻撃に関する連邦ガイダンス策定と防御的サイバー対策のための業界招集を目指す超党派法案](https://cyberscoop.com/bipartisan-bill-combat-ai-distillation-attacks-nist/) | 25.0 | 20.0 | 42.0 |
| [Microsoft、ConnectWiseへの攻撃を中国国家系ハッカーによるARTEX AIエージェント使用と断定](https://therecord.media/china-cyber-connectwise-ai) | 25.0 | 20.0 | 42.0 |
| [Agentic AIがハッカーの攻撃力を高める、詳細な指示がなくても](https://www.cybersecuritydive.com/news/agentic-ai-cyberattacks-harnesses-crowdstrike/833714/) | 25.0 | 20.0 | 42.0 |
| [機械速度の攻撃には機械速度の検知と対応が必要です](https://www.bleepingcomputer.com/news/security/machine-speed-attacks-require-machine-speed-detection-and-response/) | 25.0 | 20.0 | 42.0 |
| [OpenAIのコーディングエージェントが監視を回避していたことが判明](https://www.helpnetsecurity.com/2026/10/22/openai-agents-disabled-safety-monitoring/) | 25.0 | 20.0 | 42.0 |
| [運用レジリエンスのためのAIトークン消費管理](https://www.cisa.gov/resources-tools/resources/managing-ai-token-consumption-operational-resilience) | 25.0 | 20.0 | 42.0 |
| [XTIUM、XTAIを拡張し中央集権的なAIガバナンスとコスト管理を提供](https://www.helpnetsecurity.com/2026/10/22/xtium-xtai-orchestrator/) | 25.0 | 20.0 | 42.0 |
| [SentinelOne、AIエージェントに実行時の脅威検知と対応機能を提供](https://www.helpnetsecurity.com/2026/10/22/sentinelone-singularity-agentic-detection-and-response/) | 25.0 | 20.0 | 42.0 |
| [Broadcom、3-D Secure認証にリアルタイム詐欺検知を追加](https://www.helpnetsecurity.com/2026/10/22/broadcom-arcot-scam-defense/) | 25.0 | 20.0 | 42.0 |
| [Claude Securityがコード内で再発する脆弱性を検出可能に](https://www.helpnetsecurity.com/2026/10/22/claude-security-continuous-scanning-update/) | 25.0 | 20.0 | 42.0 |
| [OpenCodeの脆弱性により、WindowsとWSLで悪意あるMCPサーバーがサインイン中にコード実行可能に](https://thehackernews.com/2026/10/opencode-flaw-lets-malicious-mcp.html) | 25.0 | 20.0 | 42.0 |
| [Kiloview E3 NDI Encoderの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-295-01) | 24.0 | 46.0 | 50.0 |
| [Siemens APOGEE、TALONおよびDesigo PXC/PXM製品](https://www.cisa.gov/news-events/ics-advisories/icsa-26-295-08) | 24.0 | 46.0 | 50.0 |
| [Cisco、複数製品にまたがる34件の脆弱性を修正](https://www.securityweek.com/cisco-patches-34-vulnerabilities-across-multiple-products/) | 24.0 | 38.0 | 42.0 |
| [GitLab Community EditionおよびEnterprise Editionにおける重大な脆弱性](https://cert.europa.eu/publications/security-advisories/2026-019/) | 24.0 | 38.0 | 42.0 |
| [Anthropicが警告なしにセキュリティ対策を削除した94件のオープンソース事例を発見](https://www.helpnetsecurity.com/2026/10/22/anthropic-attack-surface-reduction-open-source/) | 24.0 | 38.0 | 42.0 |
| [PHP脆弱性“PoCフライング公開”の経緯、支援財団が公表 混乱広げた企業を名指しで批判](https://www.itmedia.co.jp/news/article/2610/22/2000002525/) | 23.0 | 20.0 | 42.0 |
| [Siemens SIMATIC S7-1500 CPU 1518(F)-4 PN/DP MFPの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-295-11) | 22.0 | 40.0 | 50.0 |
| [あの2回目の機会を狙っていた](https://blog.talosintelligence.com/i-had-plans-for-that-second/) | 22.0 | 20.0 | 42.0 |
| [リクルートの中古車情報サービスで個人情報など流出か](https://www.security-next.com/191773) | 22.0 | 20.0 | 42.0 |
| [番組宣伝システムでメディア関係者情報が流出か - フジテレビ](https://www.security-next.com/191719) | 22.0 | 20.0 | 42.0 |
| [Signalの欠陥により通話終了後も音声と映像が漏えいする可能性](https://www.helpnetsecurity.com/2026/10/22/signal-ringrtc-vulnerability-cve-2026-113380/) | 21.0 | 28.0 | 58.0 |
| [PHP脆弱性でいち早くサービス停止したコドモン 背景に「被害が出てからでは取り消せない」](https://www.itmedia.co.jp/news/article/2610/22/2000002528/) | 21.0 | 20.0 | 42.0 |
| [PHP脆弱性ショック、次の脅威に備えよ 被害連鎖の死角は「委託先」](https://xtech.nikkei.com/atcl/nxt/column/18/03671/102200005/) | 21.0 | 20.0 | 42.0 |
| [カプコン、1177万件漏えい 不正アクセスで](https://www.itmedia.co.jp/news/article/2610/22/2000002523/) | 21.0 | 20.0 | 42.0 |
| [高市総理、サイバーセキュリティの本を出していた しかも“PHP”から](https://www.itmedia.co.jp/news/article/2610/22/2000002522/) | 21.0 | 20.0 | 42.0 |
| [Cisco複数製品のSnort 3 SMTP MIMEにおけるサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-snort3-mime-vulns-bkXjcKkt) | 20.0 | 46.0 | 50.0 |
| [複数のCisco製品におけるSnort 3のサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-snort3-misc-dos-6mB22qAK) | 20.0 | 46.0 | 50.0 |
| [Cisco複数製品のSnort 3 Generic Routing Encapsulationにおけるサービス拒否脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-snort3-gre-JNpMHrTv) | 20.0 | 46.0 | 50.0 |
| [複数のCisco製品におけるSnort 3のサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-snort3-gtpcodec-dos-Rmecfepz) | 20.0 | 46.0 | 50.0 |
| [Cisco製品複数におけるSnort 3のVisual Basic for Applicationsバッファオーバーフローによるサービス拒否脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-snort3-vba-bufdos-jAuFdvn9) | 20.0 | 46.0 | 50.0 |
| [InterSystems IRIS for Healthの脆弱性情報](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-295-01) | 20.0 | 28.0 | 50.0 |
| [Siemens PSS(R)SINCALの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-295-06) | 20.0 | 28.0 | 50.0 |
| [詐欺師が電話を狙う新たな手口と身を守る5つの方法](https://www.malwarebytes.com/blog/scams/2026/10/scammers-are-finding-new-ways-to-target-your-phone-here-are-5-ways-to-protect-yourself) | 20.0 | 20.0 | 48.0 |
| [配送ロボットが顧客を違法にスキャンした疑い](https://www.malwarebytes.com/blog/privacy/2026/10/delivery-bots-accused-of-illegally-scanning-customers) | 20.0 | 20.0 | 48.0 |
| [インドのIT企業eMudhra、セキュリティインシデントを受け証明書事業から撤退を発表](https://therecord.media/indian-tech-company-announces-withdrawal-certificate-business-incident) | 20.0 | 20.0 | 42.0 |
| [eMudhra、8つの中間CA鍵が容易に推測可能だったためグローバルSSL/TLS事業から撤退へ](https://thehackernews.com/2026/10/emudhra-to-exit-global-ssltls-business.html) | 20.0 | 20.0 | 42.0 |
| [12年分のリリースに影響するGitLabの最高危険度脆弱性でリモートコード実行が可能に](https://www.theregister.com/security/2026/10/22/max-severity-gitlab-bug-allows-remote-code-execution-over-12-years-of-releases/5304854) | 20.0 | 20.0 | 42.0 |
| [bug bountyが1人の研究者のセキュリティスキルを磨く方法](https://github.blog/security/how-bug-bounty-sharpens-one-researchers-security-skills/) | 20.0 | 20.0 | 42.0 |
| [eMudhra中間CA証明書の侵害](https://unit42.paloaltonetworks.com/emudhra-certificate-compromise/) | 20.0 | 20.0 | 42.0 |
| [OAuth攻撃の現状と動向](https://unit42.paloaltonetworks.com/current-landscape-oauth-attacks/) | 20.0 | 20.0 | 42.0 |
| [Facebookの誤解を招くプライバシー主張でMetaに250億ドルの制裁金](https://www.malwarebytes.com/blog/news/2026/10/facebooks-misleading-privacy-claims-land-meta-a-25-billion-penalty) | 20.0 | 20.0 | 42.0 |
| [失墜したインドの認証局、証明書発行事業から撤退](https://www.theregister.com/security/2026/10/22/disgraced-indian-cert-issuer-leaves-the-cert-issuing-business/5304848) | 20.0 | 20.0 | 42.0 |
| [DNSの信頼が崩れるとき：偽造Google証明書が明らかにするもの](https://www.akamai.com/blog/security/2026/oct/dns-trust-breaks-counterfeit-google-certificates-reveal) | 20.0 | 20.0 | 42.0 |
| [China系攻撃者によるConnectWise Cloud Backupへの攻撃に関連する事案](https://www.cybersecuritydive.com/news/china-nexus-actor-attack-connectwise-cloud-backup/833727/) | 20.0 | 20.0 | 42.0 |
| [攻撃者がユーザーになるとき：アカウント乗っ取りの再考](https://www.theregister.com/security/2026/10/22/sponsored-when-the-attacker-becomes-the-user-rethinking-account-takeover/5303913) | 20.0 | 20.0 | 42.0 |
| [Unboxing Phishing Kit：Huntressが3つの実在キットを分析](https://www.huntress.com/blog/unboxing-phishing-kits) | 20.0 | 20.0 | 42.0 |
| [研究者が秘密鍵を1秒未満で解析したことを受け、eMudhraが証明書事業を終了](https://cyberscoop.com/emudhra-shuts-down-certificate-business-weak-private-keys/) | 20.0 | 20.0 | 42.0 |
| [PHPの脆弱性で世界的な対応が発生、Webサイトが停止](https://www.itpro.com/security/cyber-attacks/ive-not-seen-anything-like-this-in-a-long-long-time-millions-of-hacking-attempts-recorded-and-websites-taken-down-as-organizations-scramble-to-patch-critical-php-vulnerabilities) | 20.0 | 20.0 | 42.0 |
| [Hacker Conversations: Corey ThuenとEvil Bitの対話](https://www.securityweek.com/hacker-conversations-corey-thuen-and-the-evil-bit/) | 20.0 | 20.0 | 42.0 |
| [EU規制当局、Booking.comの詐欺リスクを調査へ](https://www.infosecurity-magazine.com/news/eu-bookingcom-scam-risks/) | 20.0 | 20.0 | 42.0 |
| [PHP2Shellの理解：知っておくべきすべて](https://www.akamai.com/blog/security-research/2026/oct/understanding-php2shell-everything-you-need-to-know) | 20.0 | 20.0 | 42.0 |
| [INTERPOL、世界的な一斉摘発で1,462人を逮捕、10,909件のサイバー犯罪ネットワークを摘発](https://thehackernews.com/2026/10/interpol-arrests-1462-suspects-disrupts.html) | 20.0 | 20.0 | 42.0 |
| [Amazon、PHP2Shellの悪用はパッチ公開4日前に始まっていた](https://www.bleepingcomputer.com/news/security/amazon-says-php2shell-exploitation-began-4-days-before-patches/) | 20.0 | 20.0 | 42.0 |
| [Indurex、産業向けサイバーセキュリティプラットフォーム拡大へ800万ドルを調達](https://www.securityweek.com/indurex-raises-8-million-to-expand-industrial-cybersecurity-platform/) | 20.0 | 20.0 | 42.0 |
| [16,000組織からのリアルタイム脅威インテリジェンスでSOCテレメトリを強化する早期対応のためのサイバー脅威コンテキスト](https://any.run/cybersecurity-blog/cyber-threat-context-for-early-soc-triage-response/) | 20.0 | 20.0 | 42.0 |
| [Tech企業とセキュリティ企業がPHP2Shellの脆弱性に対応](https://www.securityweek.com/tech-and-security-companies-respond-to-php2shell-vulnerabilities/) | 20.0 | 20.0 | 42.0 |
| [AWSの公表で判明、開示前から始まっていたPHP2Shellを狙う攻撃](https://www.theregister.com/cyber-crime/2026/10/22/hackers-pile-on-php2shell-as-aws-reveals-attacks-began-before-disclosure/5304749) | 20.0 | 20.0 | 42.0 |
| [サウスカロライナ州、州都へのサイバー攻撃後に支援を申し出る](https://therecord.media/south-carolina-officials-offer-assistance-cyber-incident) | 20.0 | 20.0 | 42.0 |
| [現代の非人間的なやり取りを把握するには、より優れた監視手段が必要です](https://www.akamai.com/blog/security/2026/oct/mapping-todays-nonhuman-interactions-requires-better-radar) | 20.0 | 20.0 | 42.0 |
| [Microsoft、ConnectWise侵害で中国系スパイが2,250のクラウドテナントに侵入可能に](https://www.theregister.com/security/2026/10/22/microsoft-says-connectwise-breach-let-chinese-spies-loose-on-2250-cloud-tenants/5304687) | 20.0 | 20.0 | 42.0 |
| [Cash Appアカウントを開設していないと主張する女性に懲役刑の可能性](https://www.malwarebytes.com/blog/news/2026/10/woman-faces-years-in-prison-over-a-cash-app-account-she-says-she-never-opened) | 20.0 | 20.0 | 42.0 |
| [Railway、侵入者が顧客の機密情報にアクセスした可能性があるとして認証情報のローテーションを呼びかけ](https://thehackernews.com/2026/10/railway-says-intruder-may-have-accessed.html) | 20.0 | 20.0 | 42.0 |
| [正規プラットフォームを悪用し、認証を通過するフィッシングメールを配信する攻撃](https://www.helpnetsecurity.com/2026/10/22/legitimate-platforms-abused-phishing-emails/) | 20.0 | 20.0 | 42.0 |
| [SplunkとSolarWindsが新たなセキュリティアップデートを公開](https://www.securityweek.com/splunk-solarwinds-release-fresh-security-updates/) | 20.0 | 20.0 | 42.0 |
| [PHP2Shell脆弱性がFortinet、Cisco、Palo Altoの顧客に与える影響](https://www.helpnetsecurity.com/2026/10/22/php2shell-vulnerability-fortinet-cisco-palo-alto-networks/) | 20.0 | 20.0 | 42.0 |
| [カプコンのオンラインサービスで約1177万件のユーザー情報漏えい、パスワードの不正な変更も](https://internet.watch.impress.co.jp/docs/news/2150509.html) | 20.0 | 20.0 | 42.0 |
| [Amazonが脆弱性公開の4日前に検知したPHP2Shellの悪用試行](https://www.infosecurity-magazine.com/news/php2shell-exploitation-attempt/) | 20.0 | 20.0 | 42.0 |
| [暗号化だけではデータの保護は不十分、移動先でも守るには](https://cyberscoop.com/vaultless-keyless-pseudonymization-cybersecurity-policy-op-ed/) | 20.0 | 20.0 | 42.0 |
| [大手薬局チェーンのIT部門と監査担当者がCiscoファイアウォールで「password」の使用を巡り激しい対立](https://www.theregister.com/security/2026/10/22/it-department-and-auditors-at-major-pharmacy-chain-got-into-a-rip-roaring-fight-about-using-password-on-cisco-firewall/5304592) | 20.0 | 20.0 | 42.0 |
| [カプコン 1177万件の情報漏えい](https://news.yahoo.co.jp/pickup/6599723?source=rss) | 20.0 | 20.0 | 42.0 |
| [PHP2Shellの悪用は修正パッチ公開の数日前から始まっていた](https://www.securityweek.com/php2shell-exploitation-started-days-before-patches/) | 20.0 | 20.0 | 42.0 |
| [NTTソルマーレの「コミックシーモア」、不正アクセスで最大約420万件の情報流出を発表 安全性が確保された機能から段階的にサービス再開へ](https://internet.watch.impress.co.jp/docs/news/2150465.html) | 20.0 | 20.0 | 42.0 |
| [クラウドセキュリティの成熟度は普及に追いつかず、SANSが警鐘](https://www.infosecurity-magazine.com/news/cloud-security-maturity-lags-sans/) | 20.0 | 20.0 | 42.0 |

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
