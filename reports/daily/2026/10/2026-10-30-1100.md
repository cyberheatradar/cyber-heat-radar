# 📡 サイレーダー 2026-10-30 11:00 JST

このレポートは、2026-10-30 05:00 JST〜2026-10-30 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 73
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 46

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-2026-109619) on Palo Alto Networks Products (Severity: CRITICAL)](#topic-38753) | 56.0 | 74.0 | 67.0 | 音声 | 温度感上位枠 |
| 2 | [Vulnerabilities in Node.<wbr>js Affecting Cisco Products: October 2026](#topic-39379) | 39.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [Hugging Face malware campaign returns to hijack GPUs for crypto mining](#topic-40512) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-38753"></a>

### 1. CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-2026-109619) on Palo Alto Networks Products (Severity: CRITICAL)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 56.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

PHPに存在する複数の重大な脆弱性（CVE-2026-109618、CVE-2026-109619）について、Palo Alto NetworksやJPCERT/CCなどが注意喚起しています。
公表情報では、認証なしのリモートコード実行につながる可能性が示されており、公開PoCや検証コードの言及も見られます。
WebサーバーやCMS基盤で広く使われるPHPに関わるため、影響範囲が広くなるおそれがあります。関連製品や周辺システムでの迅速な確認と更新対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 27 sources。
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

- 利用中のPHPバージョンと依存製品が影響対象かを確認する。
- ベンダー提供の修正版・緩和策の適用状況を点検する。
- 外部公開サービスで不審な挙動や異常なエラーがないか監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-109618 | 関連CVE | 1.00 | 候補あり（URL 106件以上） |
| 脆弱性 | CVE-2026-109619 | 関連CVE | 1.00 | 候補あり（URL 13件以上） |
| 脆弱性 | CVE-2026-110264 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-114625 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-115560 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| ベンダー | Cloudflare | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-109618](https://nvd.nist.gov/vuln/detail/CVE-2026-109618) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-](https://security.paloaltonetworks.com/CVE-2026-109618) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: Critical Vulnerabilities in PHP: CVE-2026-109618, CVE-2026-109619 ](https://unit42.paloaltonetworks.com/cve-2026-109618-cve-2026-109619/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: PHPにおける複数の脆弱性（CVE-2026-109618、CVE-2026-109619）に関する注意喚起  (更新)](https://www.jpcert.or.jp/at/2026/at260033.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in PHP Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-php-october26-Jj384Daq) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Weekly Report: PHPにおける複数の脆弱性（CVE-2026-109618、CVE-2026-109619）に関する注意喚起](https://www.jpcert.or.jp/wr/2026/wr261028.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Introducing the Cloudflare PHP Capture the Flag challenge](https://blog.cloudflare.com/php-ctf/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Confirms Active Exploitation of Two PHP2Shell Flaws Enabling Remote Code Ex](https://thehackernews.com/2026/10/cisa-confirms-active-exploitation-of.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（44件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-39379"></a>

### 2. Vulnerabilities in Node.<wbr>js Affecting Cisco Products: October 2026

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Node.<wbr>jsのBrotliデコーダに関する脆弱性「CVE-2026-111497」について、Ciscoを含む複数ベンダーが影響を案内しています。
公開情報では、悪意あるBrotliデータにより、Node.<wbr>js環境で意図しないコード実行につながる可能性が示されています。
Node.<wbr>jsは多くの製品やサービスの基盤として使われているため、影響範囲が広がりやすい点が注目されています。
加えて、関連情報では実悪用の文脈にも触れられており、対応の優先度を上げる理由になります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 11 sources。
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

- Node.<wbr>jsの該当サポート系統を利用している製品・サービスを洗い出し、ベンダーの修正版や案内を確認する。
- Brotliを扱う機能や外部入力を受ける経路があるシステムは、更新の適用状況と影響範囲を優先確認する。
- Ciscoや各ベンダーのアドバイザリを参照し、関連コンポーネントを含めた脆弱性管理と監視を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-105482 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-105483 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-106069 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-111497 | 関連CVE | 1.00 | 候補あり（URL 29件以上） |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| ベンダー | Wiz | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-111497](https://nvd.nist.gov/vuln/detail/CVE-2026-111497) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in Node.<wbr>js Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-oct2026-node-js-Jj3SQ19u) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-111497 Portfolio Status: Impact of Brotli Vulnerability (CVE-2026-11149](https://security.paloaltonetworks.com/CVE-2026-111497) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Adobe Commerce PolyShell Attacks Breach Hundreds of Stores as Brotli Exploit Tra](https://thehackernews.com/2026/10/adobe-commerce-polyshell-attacks-breach.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Brotli bug reaches far beyond Node.<wbr>js (CVE-2026-111497)](https://www.helpnetsecurity.com/2026/10/27/node2shell-broccoli2shell-vulnerability-cve-2026-111497/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Experts temper emergency-level alarms over critical Brotli defect](https://cyberscoop.com/brotli-critical-vulnerability-decompression-library-node2shell-broccoli2shell/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [eMudhra, Brotli, and the Long Tail of a Security Fix](https://socket.dev/blog/emudhra-brotli-security-fix) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft releases emergency .<wbr>NET security fixes for Google Brotli bug](https://www.theregister.com/security/2026/10/26/microsoft-releases-emergency-net-security-fixes-for-google-brotli-bug/5305515) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（5件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-40512"></a>

### 3. Hugging Face malware campaign returns to hijack GPUs for crypto mining

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Hugging Face上のモデルを悪用した仮想通貨マイニングのキャンペーンが、削除対応の後に再び確認されたとされています。
GPUサーバーを乗っ取ってマイニングやバックドア設置に使う手口が報じられており、別件ではAIコーディング支援を悪用してRATを入れさせようとする偽プロジェクトの存在も示されています。
AI開発・実行環境が、単なるモデル利用の場から攻撃の足場に変わる可能性があるため注目されます。
特にGPU資源の不正利用は、計算コストの増大だけでなく、環境侵害や継続的な不正アクセスにつながるおそれがあります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 公開モデルや依存コードを取り込む前に、提供元の信頼性と更新履歴を確認する。
- GPUサーバーやAI基盤で、想定外のプロセス起動や外向き通信を監視する。
- AI支援ツールの提案を鵜呑みにせず、導入前のレビューと権限管理を徹底する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 遠隔管理/RMMツール | NetSupport RAT | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Hugging Face malware campaign returns to hijack GPUs for crypto mining](https://www.bleepingcomputer.com/news/security/hugging-face-malware-campaign-returns-to-hijack-gpus-for-crypto-mining/) | <nobr>内容確認・補足情報</nobr> |

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
| [「3年以内に車はランサムウェアに狙われる」 9割の開発者が回答](https://atmarkit.itmedia.co.jp/ait/articles/2610/30/news023.html) | 29.0 | 30.0 | 42.0 |
| [リモートディテーリング事業等を行うエンタッチにランサムウェア攻撃](https://scan.netsecurity.ne.jp/article/2026/10/30/56630.html) | 29.0 | 30.0 | 42.0 |
| [エンタッチにランサムウェア攻撃、データベース内の情報が流出](https://scan.netsecurity.ne.jp/article/2026/10/30/56627.html) | 29.0 | 30.0 | 42.0 |
| [「Dire Wolf」の攻撃が急増 ファイルの一部を暗号化し高速化](https://xtech.nikkei.com/atcl/nxt/mag/nnw/18/041600214/101900021/) | 29.0 | 30.0 | 42.0 |
| [大塚商会、アクロニス「Acronis Cyber Protect Cloud」を基盤とした自動バックアップソリューション提供 ランサムウェアや災害などによるデータ消失を対策](https://internet.watch.impress.co.jp/docs/news/2152388.html) | 28.0 | 30.0 | 42.0 |
| [【緊急対応】バックアップするも8割超が復旧できず…ガートナー流「データ保護術3選」](https://www.sbbit.jp/article/cont1/187823?ref=rss) | 28.0 | 30.0 | 42.0 |
| [PHPの脆弱性悪用に関する限定的な報告が浮上](https://therecord.media/php2shell-successful-exploitation-reports-emerge) | 28.0 | 20.0 | 42.0 |
| [OpenAI、AIの行動指針「Model Spec」を改定 “記憶”の使い方や人間による監督を明記](https://www.itmedia.co.jp/news/article/2610/30/2000002735/) | 26.0 | 20.0 | 42.0 |
| [徳丸浩氏 登壇 ～ 日銀金融研究所、オンラインセミナー「AIエージェント時代に求められるセキュリティ戦略と課題」を 11/30 開催](https://scan.netsecurity.ne.jp/article/2026/10/30/56623.html) | 26.0 | 20.0 | 42.0 |
| [OpenAI、批判を受けChatGPT Proの利用上限を倍増し予定していた50%削減を撤回](https://www.bleepingcomputer.com/news/artificial-intelligence/openai-doubles-chatgpt-pro-usage-limits-after-backlash-over-planned-50-percent-cut/) | 25.0 | 20.0 | 42.0 |
| [SAPとNTT、ソブリンクラウドとSAP Business AIの機能提供に向けて連携](https://internet.watch.impress.co.jp/docs/news/2152433.html) | 25.0 | 20.0 | 42.0 |
| [研究者がOpenAIやMicrosoftの脆弱性を含む5つのAI開発ツールのバグを発見](https://www.theregister.com/security/2026/10/29/researchers-find-bugs-in-5-ai-developer-tools-with-openai-and-microsoft-flaws-still-unpatched/5306508) | 25.0 | 20.0 | 42.0 |
| [【緊急】全システム担当者が知っておくべき「AI防御特化スキル」、主要5社の使い方](https://www.sbbit.jp/article/cont1/187920?ref=rss) | 25.0 | 20.0 | 42.0 |
| [Anthropicを装ったフィッシングメールが主要セキュリティツールを回避](https://www.darkreading.com/cyberattacks-data-breaches/anthropic-phishing-emails-bypass-security-tools) | 25.0 | 20.0 | 42.0 |
| [981gの軽さにRyzen AIのパワー、さらにコスパも。マウスコンピューターの新モデル「mouse X2」は“ちょうどいい”を極めた優等生モバイルPCだった[Sponsored]](https://internet.watch.impress.co.jp/docs/topic/special/2149773.html) | 25.0 | 20.0 | 42.0 |
| [AI時代におけるサイバーセキュリティ啓発の再考](https://www.darkreading.com/cyber-risk/rethinking-cybersecurity-awareness-ai-era) | 25.0 | 20.0 | 42.0 |
| [米当局、Ciscoセキュリティ製品と「GitLab」の脆弱性悪用に警鐘](https://www.security-next.com/192196) | 24.0 | 20.0 | 43.0 |
| [AIが勝手に隔離環境を脱出した事件を受けてOpenAIが「AIを別のAIで監視する仕組み」を公開](https://gigazine.net/news/20261030-openai-detect-frontier-model-misalignment/) | 22.0 | 20.0 | 42.0 |
| [AndroidにSMSを送りつけるだけで通話を切断できる脆弱性が判明、緊急通報にも影響](https://gigazine.net/news/20261030-sms-of-death/) | 22.0 | 20.0 | 42.0 |
| [「Ivanti Connect Secure」に追加脆弱性2件 - 連鎖攻撃を確認](https://www.security-next.com/192205) | 22.0 | 20.0 | 42.0 |
| [「Chrome」で脆弱性21件を修正 - 「クリティカル」の脆弱性も](https://www.security-next.com/192200) | 22.0 | 20.0 | 42.0 |
| [Appleのgitは依然として侵害されたeMudhra証明書を信頼している](https://gigazine.net/news/20261030-apple-git-trusts-compromised-certificates/) | 22.0 | 20.0 | 42.0 |
| [ヤクルト本社、個人情報約4万件漏えい 公式サイトへの不正アクセスで](https://www.itmedia.co.jp/news/article/2610/30/2000002739/) | 21.0 | 20.0 | 42.0 |
| [AIで変わるセキュリティ運用--リソース不足や労苦の改善を探るセミナーを開催](https://japan.zdnet.com/article/35253579/) | 21.0 | 20.0 | 42.0 |
| [アイリスオーヤマの通販サイトに不正アクセス 情報漏えいは「調査中」](https://www.itmedia.co.jp/news/article/2610/30/2000002737/) | 21.0 | 20.0 | 42.0 |
| [今日もどこかで情報漏えい 第53回「2026年9月の情報漏えい」カメラが情報漏えいの瞬間を捉えた世紀の映像](https://scan.netsecurity.ne.jp/article/2026/10/30/56635.html) | 21.0 | 20.0 | 42.0 |
| [Gunosy の社内業務用アカウントの認証情報を用いた不正ログイン、取引先や役員・従業員等の情報が流出](https://scan.netsecurity.ne.jp/article/2026/10/30/56634.html) | 21.0 | 20.0 | 42.0 |
| [So-net 会員データベースに不正アクセス、会員情報214万1,986件が漏えい](https://scan.netsecurity.ne.jp/article/2026/10/30/56633.html) | 21.0 | 20.0 | 42.0 |
| [「お名前.com デスクトップクラウド」に不正アクセス、情報が公開された顧客に上限300万円の特別見舞金](https://scan.netsecurity.ne.jp/article/2026/10/30/56632.html) | 21.0 | 20.0 | 42.0 |
| [不正アクセスでチケット購入サービス「GETTIIS」会員情報が外部流出](https://scan.netsecurity.ne.jp/article/2026/10/30/56631.html) | 21.0 | 20.0 | 42.0 |
| [ニフティの回線申込・受付管理システムに不正アクセス、最大54万2,513件の会員情報に影響](https://scan.netsecurity.ne.jp/article/2026/10/30/56629.html) | 21.0 | 20.0 | 42.0 |
| [セカンドリテイリングに不正アクセス](https://scan.netsecurity.ne.jp/article/2026/10/30/56628.html) | 21.0 | 20.0 | 42.0 |
| [メディアサーバにディレクトリパストラバーサルが存在 ～ アルカディア運営の「SpeeCAN RAIDEN」に不正アクセス](https://scan.netsecurity.ne.jp/article/2026/10/30/56626.html) | 21.0 | 20.0 | 42.0 |
| [「阪急百貨店・阪神百貨店予約サイト」に不正アクセス、約126万件の「H2O ID」個人情報が漏えい](https://scan.netsecurity.ne.jp/article/2026/10/30/56625.html) | 21.0 | 20.0 | 42.0 |
| [経済産業省が中小企業・小規模事業者向け「サイバーセキュリティ特別相談窓口」を設置](https://scan.netsecurity.ne.jp/article/2026/10/30/56624.html) | 21.0 | 20.0 | 42.0 |
| [なぜ「更新できない」のか？ PHP騒動で見えた、パッチを先送りする企業の盲点](https://www.itmedia.co.jp/enterprise/articles/2610/30/news025.html) | 21.0 | 20.0 | 42.0 |
| [約3割のセキュリティ担当者、本番環境で「野良エージェント」に遭遇 ServiceNow調査](https://www.itmedia.co.jp/enterprise/articles/2610/29/news047.html) | 21.0 | 20.0 | 42.0 |
| [個人情報、漏れたらまず何する？ ID／PW、クレカ、免許証、メールアドレス、情報別やることまとめ](https://atmarkit.itmedia.co.jp/ait/articles/2610/30/news022.html) | 21.0 | 20.0 | 42.0 |
| [CISA ICS Advisory / ICS Medical Advisory（2026年10月29日）](https://jvn.jp/vu/JVNVU95856220/) | 20.0 | 20.0 | 42.0 |
| [情報漏えい 4月以降延べ2.6億人分](https://news.yahoo.co.jp/pickup/6600644?source=rss) | 20.0 | 20.0 | 42.0 |
| [TrendAI、損保ジャパンのサイバー保険契約者向けにIT資産管理・脆弱性管理サービス提供 アタックサーフェスマネジメント（ASM）「SOMPO Cyber Risk Scan」](https://internet.watch.impress.co.jp/docs/news/2152315.html) | 20.0 | 20.0 | 42.0 |
| [Binance、58億ドル相当の暗号資産窃取の可能性を調査](https://www.bleepingcomputer.com/news/security/binance-probes-potential-58-billion-crypto-theft-hack/) | 20.0 | 20.0 | 42.0 |
| [Japan Airlines、第三者によるデータ侵害で乗客情報が流出](https://www.bleepingcomputer.com/news/security/japan-airlines-suffers-third-party-data-breach-exposing-passenger-info/) | 20.0 | 20.0 | 42.0 |
| [Polymarket、暗号資産流出スクリプトの侵害を受け取引停止　250万ドルの追跡判明](https://www.bleepingcomputer.com/news/security/polymarket-halts-trading-after-crypto-draining-script-breach-25m-traced/) | 20.0 | 20.0 | 42.0 |
| [KDDI、リスクの診断と対処を効率化する「AI脆弱性管理ソリューション」の提供を開始](https://internet.watch.impress.co.jp/docs/news/2152201.html) | 20.0 | 20.0 | 42.0 |
| [漏えいしたDHS職員アーカイブ、Icepickがオンライン維持に苦戦](https://cyberscoop.com/dhs-employee-breach-icepick-database-takedown/) | 20.0 | 20.0 | 42.0 |

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
