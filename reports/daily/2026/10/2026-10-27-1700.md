# 📡 サイレーダー 2026-10-27 17:00 JST

このレポートは、2026-10-27 11:00 JST〜2026-10-27 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 58
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 2
- [低温だが記録しておくトピック](#low-record-topics): 30

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-2026-109619) on Palo Alto Networks Products (Severity: HIGH)](#topic-38753) | 56.0 | 74.0 | 67.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [GMO、ランサム被害にあった顧客に新しいPC提供へ 犯行グループは1人の顧客情報公開か](#topic-39817) | 42.0 | 33.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [CVE-2026-111497 Portfolio Status: Impact of Brotli Vulnerability (CVE-2026-111497) on Palo Alto Networks Products (Severity: CRITICAL)](#topic-39379) | 39.0 | 64.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 4 | [GMOに身代金要求 - ランサム攻撃や情報公開を行うと脅迫](#topic-39832) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-39817"></a>

### 1. GMO、ランサム被害にあった顧客に新しいPC提供へ 犯行グループは1人の顧客情報公開か

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 42.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 33.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

GMOは、ランサムウェア被害にあった顧客に対して新しいPCを提供する方針を示しました。
あわせて、犯行グループが顧客情報の一部を公開した可能性が報じられていますが、現時点で端末からランサムウェアを含むマルウェアは確認されていないとされています。
顧客端末の再提供や復旧支援は、被害拡大の抑制と業務継続に直結するため注目されています。情報公開の有無は、漏えい範囲や二次被害の見極めに関わるため、今後の続報が重要です。

#### 温度感の理由

##### 温度感
- 技術詳細・再現情報あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 技術詳細により影響確認が進みやすい。
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 被害端末の再配布・再セットアップ時は、初期化だけでなく設定や認証情報の見直しも含めて対応する。
- 公開情報で自社名や個人情報が言及されていないかを継続監視し、該当する場合は影響範囲を速やかに確認する。
- ランサムウェア事案では、端末の安全確認と並行して、バックアップ・アカウント・通信経路の点検を進める。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [GMO、ランサム被害にあった顧客に新しいPC提供へ　犯行グループは1人の顧客情報公開か](https://www.itmedia.co.jp/news/article/2610/27/2000002624/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-39832"></a>

### 2. GMOに身代金要求 - ランサム攻撃や情報公開を行うと脅迫

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | - |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

GMOインターネットの仮想デスクトップサービスをめぐり、侵害後に身代金を要求する脅迫が行われていると伝えられています。
同社は対応を進めつつ、利用者に注意を呼びかけているとされています。
ランサムウェアに関連する脅迫は、サービス停止や情報流出の懸念につながるため、利用者・運用者の両方に影響が及ぶ可能性があります。
国内で報じられている点からも、同種事案への備えや初動対応の重要性が改めて注目されます。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象サービスや周辺システムの影響範囲を確認し、異常なアクセスや設定変更の有無を点検する。
- 利用者向けの案内や問い合わせ対応を整え、不要な混乱を避けるため情報発信を一本化する。
- 関連する認証情報や接続経路について見直し、必要に応じて監視強化と追加の保護措置を講じる。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [GMOに身代金要求 - ランサム攻撃や情報公開を行うと脅迫](https://www.security-next.com/191999) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-38753"></a>

### 1. CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-2026-109619) on Palo Alto Networks Products (Severity: HIGH)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 56.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

PHPの2件の脆弱性（CVE-2026-109618、CVE-2026-109619）は、認証なしのリモートコード実行につながる可能性があるとされ、関連するベンダー各社の製品影響も案内されています。
公開情報では、実際の悪用や検証コードの言及があり、対応の緊急性が高い話題として扱われています。
Webサーバーやその上で動くアプリケーションに広く影響しうるため、対象環境がある組織では優先的な確認が必要です。
実際の悪用が示唆されている点から、未対応のまま放置すると被害につながるリスクが高まります。

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

- PHPの導入有無とバージョン、関連ベンダーの影響範囲を早急に棚卸しする。
- 各ベンダーの修正情報を確認し、該当環境は速やかにアップデートや緩和策を適用する。
- 外部公開しているPHPベースのサービスは、アクセスログや異常な挙動を重点的に監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-109618 | 関連CVE | 1.00 | 候補あり（URL 101件以上） |
| 脆弱性 | CVE-2026-109619 | 関連CVE | 1.00 | 候補あり（URL 14件以上） |
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
| <nobr>出典</nobr> | [CISA Confirms Active Exploitation of Two PHP2Shell Flaws Enabling Remote Code Ex](https://thehackernews.com/2026/10/cisa-confirms-active-exploitation-of.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-109618 Impact of Critical Vulnerabilities in PHP (CVE-2026-109618, CVE-](https://security.paloaltonetworks.com/CVE-2026-109618) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Vulnerabilities in PHP Affecting Cisco Products: October 2026](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-php-october26-Jj384Daq) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Millions of PHP Servers Face RCE Risk as PHP2Shell Exploitation Attempts Emerge](https://blog.polyswarm.io/millions-of-php-servers-face-rce-risk-as-php2shell-exploitation-attempts-emerge) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [26th October – Threat Intelligence Report](https://research.checkpoint.com/2026/26th-october-threat-intelligence-report/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP2Shell security flaws now sucessfully exploited in the wild](https://www.bleepingcomputer.com/news/security/php2shell-security-flaws-now-sucessfully-exploited-in-the-wild/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: PHPにおける複数の脆弱性（CVE-2026-109618、CVE-2026-109619）に関する注意喚起  (更新)](https://www.jpcert.or.jp/at/2026/at260033.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（36件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-39379"></a>

### 2. CVE-2026-111497 Portfolio Status: Impact of Brotli Vulnerability (CVE-2026-111497) on Palo Alto Networks Products (Severity: CRITICAL)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

CVE-2026-111497は、Brotli圧縮データの処理に関わる脆弱性で、Node.<wbr>jsやそれを組み込む各種製品に影響する可能性があるとされています。
公開情報では、Node.<wbr>jsの一部版に影響し、ベンダー各社が関連コンポーネントの修正や更新対応を進めていることが確認できます。
圧縮ライブラリの脆弱性は、単体のアプリではなく同梱ライブラリや派生製品にも波及しやすく、影響範囲の把握が難しくなりがちです。
実務では、直接利用していない製品でも、組み込みコンポーネント経由で影響を受ける可能性がある点が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 9 sources。
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

- Node.<wbr>jsや関連ランタイムを使うシステムで、ベンダーの修正版・影響範囲の案内を確認する。
- OSやアプリ単体だけでなく、同梱されたBrotliライブラリや再配布パッケージの更新有無を点検する。
- HTTPレスポンス解凍など、外部入力を圧縮展開する経路があるサービスは優先的に棚卸しする。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-111497 | 関連CVE | 1.00 | 候補あり（URL 24件以上） |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Palo Alto Networks | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| ベンダー | Wiz | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| マルウェア | ZLib | 主題 | 0.80 | — |
| ベンダー | watchTowr | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-111497](https://nvd.nist.gov/vuln/detail/CVE-2026-111497) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-111497 Portfolio Status: Impact of Brotli Vulnerability (CVE-2026-11149](https://security.paloaltonetworks.com/CVE-2026-111497) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Experts temper emergency-level alarms over critical Brotli defect](https://cyberscoop.com/brotli-critical-vulnerability-decompression-library-node2shell-broccoli2shell/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [eMudhra, Brotli, and the Long Tail of a Security Fix](https://socket.dev/blog/emudhra-brotli-security-fix) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft releases emergency .<wbr>NET security fixes for Google Brotli bug](https://www.theregister.com/security/2026/10/26/microsoft-releases-emergency-net-security-fixes-for-google-brotli-bug/5305515) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [PHP Issues Second Windows Security Update in Five Days to Fix Brotli Code Execut](https://thehackernews.com/2026/10/php-issues-second-windows-security.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-111497: Critical out-of-bounds write in the Node.<wbr>js Brotli decoder](https://www.rapid7.com/blog/post/etr-cve-2026-111497-critical-out-of-bounds-write-in-the-node-js-brotli-decoder) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Inside Node2Shell: A Closer Look at CVE-2026-111497](https://www.akamai.com/blog/security-research/2026/oct/inside-node2shell-closer-look-cve-2026-111497) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（4件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [GMO、PCのバックアップと電源オフ呼びかけ VPS利用者に きょう正午の攻撃予告受け](https://www.itmedia.co.jp/news/article/2610/27/2000002616/) | 29.0 | 30.0 | 42.0 |
| [専門AIで肌カウンセリング、ファンケルが新サービス チャットと顔画像解析で](https://www.itmedia.co.jp/news/article/2610/27/2000002629/) | 28.0 | 20.0 | 42.0 |
| [メアドを検索→AIで“その人専用フィッシングメール”を生成する手法、クリック率が約2.7倍に 7000人以上で実験](https://www.itmedia.co.jp/news/article/2610/27/2000002550/) | 28.0 | 20.0 | 42.0 |
| [サイバーコマンド、SCS評価制度の★3取得を支援する「KUMIHIMO AI.security」を提供](https://news.mynavi.jp/techplus/article/20261027-5203692/) | 26.0 | 20.0 | 42.0 |
| [ベイブレードXの「ベイバトルパス」をリバースエンジニアリングして独自アプリを開発、AIがシュートの強さを評価してアドバイス](https://gigazine.net/news/20261027-bayblade-x-reverse-engineering/) | 25.0 | 20.0 | 43.0 |
| [AIセキュリティ市場の複数分野が大規模プラットフォームへ向かう](https://www.helpnetsecurity.com/2026/10/27/jonathan-care-kuppingercole-analysts-ai-security-market/) | 25.0 | 20.0 | 42.0 |
| [LLMエージェントのセキュリティにはガードレール以上が必要です](https://www.helpnetsecurity.com/2026/10/27/llm-agent-security-video/) | 25.0 | 20.0 | 42.0 |
| [今すぐ応募できるサイバーセキュリティ求人：2026年10月27日](https://www.helpnetsecurity.com/2026/10/27/cybersecurity-jobs-available-right-now-october-27-2026/) | 25.0 | 20.0 | 42.0 |
| [GPT-6.1 TerraがOpenAIの重要なサイバー基準を満たし、GPT-5.6 Terraより安価に提供される](https://www.helpnetsecurity.com/2026/10/27/gpt-6-1-terra-released/) | 25.0 | 20.0 | 42.0 |
| [「PHP2Shell」「HTTP2Shell」のいずれも影響 - 「PAN-OS」の修正版が順次公開](https://www.security-next.com/192013) | 22.0 | 20.0 | 42.0 |
| [GMOとその利用者に向けた脅迫文が読める「GMO不正アクセス犯の犯行声明文ビュアー」](https://gigazine.net/news/20261027-gmo-hacker-seimei-viewer/) | 22.0 | 20.0 | 42.0 |
| [「PowerShell」に「Brotli」脆弱性を解消するアップデート](https://www.security-next.com/192008) | 22.0 | 20.0 | 42.0 |
| [中国製AI「Qwen3.8」にセキュリティ対策を命じたら勝手に北京のサーバーへデータ送信を試みたことが判明](https://gigazine.net/news/20261027-concerning-behaviour-open-weight-ai-model/) | 22.0 | 20.0 | 42.0 |
| [英語以外の言語を使うとAIモデルのコストは高くなる](https://gigazine.net/news/20261027-tokenizer-tax/) | 22.0 | 20.0 | 42.0 |
| [Appleの2026年10月のセキュリティアップデート](https://isc.sans.edu/diary/rss/33458) | 22.0 | 20.0 | 42.0 |
| [タイムズカー、お見舞金3000円の算定基準は？ 支払い時期や対象かの確認方法をパーク24に聞いた](https://www.itmedia.co.jp/news/article/2610/27/2000002627/) | 21.0 | 20.0 | 42.0 |
| [政府、サイバー攻撃の「緊急対策パッケージ」来週中に策定へ 高市首相がサイバー閣僚会議の初会合で指示](https://www.itmedia.co.jp/news/article/2610/27/2000002620/) | 21.0 | 20.0 | 42.0 |
| [「自分の個人情報が漏えいした……どうすれば？」 IPAが対処法公開](https://www.itmedia.co.jp/news/article/2610/27/2000002617/) | 21.0 | 20.0 | 42.0 |
| [JR「スマートEX」会員メアドなど漏えい、約17万件か ユミルリンクへの不正アクセスで](https://www.itmedia.co.jp/news/article/2610/27/2000002615/) | 21.0 | 20.0 | 42.0 |
| [船舶・港湾システム向けの無料脆弱性データベースを海事連合が公開](https://www.securityweek.com/maritime-coalition-launches-free-vulnerability-database-for-ship-and-port-systems/) | 20.0 | 20.0 | 42.0 |
| [P2Pアクセスと認証の脆弱性を悪用してUkraineのDahua IPカメラを乗っ取る攻撃者](https://thehackernews.com/2026/10/attackers-hijack-dahua-ip-cameras-in.html) | 20.0 | 20.0 | 42.0 |
| [Microsoft Authenticatorの脆弱性により悪意あるAndroidアプリが業務アカウントへのアクセスを窃取可能に](https://www.helpnetsecurity.com/2026/10/27/microsoft-authenticator-vulnerability-patchedcve-2026-80097/) | 20.0 | 20.0 | 42.0 |
| [GROWIにおける複数の脆弱性](https://jvn.jp/jp/JVN51223238/) | 20.0 | 20.0 | 42.0 |
| [SSHもパッケージマネージャーもないLinuxシステム「Amutable Foundations」](https://www.helpnetsecurity.com/2026/10/27/amutable-foundations-linux-system/) | 20.0 | 20.0 | 42.0 |
| [GMO攻撃者「個人情報毎日公開」](https://news.yahoo.co.jp/pickup/6600302?source=rss) | 20.0 | 20.0 | 42.0 |
| [脆弱性の悪用の71%は公開後1週間以内に始まる](https://www.helpnetsecurity.com/2026/10/27/rapid7-vulnerability-exploitation-trends-q3-2026-report/) | 20.0 | 20.0 | 42.0 |
| [ギフティグループ、不正アクセスでeギフトが不正に発行、約5.5億円の損失見込み](https://internet.watch.impress.co.jp/docs/news/2151480.html) | 20.0 | 20.0 | 42.0 |
| [FX不正アクセス 5社で顧客被害](https://news.yahoo.co.jp/pickup/6600277?source=rss) | 20.0 | 20.0 | 42.0 |
| [GMO攻撃者 個人情報1件を公開か](https://news.yahoo.co.jp/pickup/6600296?source=rss) | 20.0 | 20.0 | 42.0 |
| [Sleipnir Mobile for Androidのユーザーインターフェースにおいて偽のアドレスバーなどを表示される脆弱性](https://jvn.jp/jp/JVN90463048/) | 20.0 | 20.0 | 42.0 |

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
