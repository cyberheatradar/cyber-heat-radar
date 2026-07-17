# 📡 サイレーダー 2026-07-18 05:00 JST

このレポートは、2026-07-17 17:00 JST〜2026-07-18 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 79
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 2
- [低温だが記録しておくトピック](#low-record-topics): 46

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-58644: CISA KEV catalog addition](#topic-23002) | 50.0 | 64.0 | 55.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [Microsoft 2026年7月 Patch Tuesday 関連まとめ](#topic-22358) | 36.0 | 48.0 | 57.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [In Other News: Iran Tracks US Military Phones, CrashStealer macOS Malware, CVD Blueprint](#topic-23145) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [New NadMesh Botnet Hunts Exposed AI Services for Cloud Keys and Kubernetes Tokens](#topic-23130) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-23145"></a>

### 1. In Other News: Iran Tracks US Military Phones, CrashStealer macOS Malware, CVD Blueprint

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

SecurityWeekは、見逃されがちな複数のサイバー関連ニュースをまとめて取り上げ、その中でmacOS向けマルウェア「CrashStealer」に言及しています。
あわせて、脅威インテリジェンスやランサムウェア関連の話題も含まれており、複数のトピックを横断して注目される内容です。
macOSを含む複数の環境や組織に関わる話題が混在しており、実務上は自組織への影響有無を広く確認する必要があります。
単独の脆弱性情報ではなく、脅威動向として把握しておく価値があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- macOS端末の保護状況やEDR検知、許可されていないソフトウェアの導入状況を確認する。
- ランサムウェアや関連する攻撃動向について、社内の監視・アラート設定が現状に合っているか見直す。
- 関連情報が断片的に出やすいため、公式発表や信頼できる一次情報で続報を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | Apple macOS | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [In Other News: Iran Tracks US Military Phones, CrashStealer macOS Malware, CVD B](https://www.securityweek.com/in-other-news-iran-tracks-us-military-phones-crashstealer-macos-malware-cvd-blueprint/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23130"></a>

### 2. New NadMesh Botnet Hunts Exposed AI Services for Cloud Keys and Kubernetes Tokens

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>A⁠I</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、NadMeshと呼ばれるボットネットが、外部公開されたAI関連サービスを探してクラウド鍵やKubernetesトークンを狙っているとされています。
対象には、ComfyUI、Ollama、n8n、Open WebUI、Langflow、Gradioなどの運用環境が含まれると報じられています。
AI関連サービスは迅速に立ち上がる一方で、公開設定や認証の不備が見落とされやすく、重要な認証情報の流出につながるおそれがあります。
特にクラウド鍵やKubernetesトークンが関わる場合、単一サービスの問題が広い環境に波及する可能性があります。

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

- 外部公開しているAI/ワークフロー系サービスの露出範囲と認証設定を点検する。
- クラウド鍵やKubernetesトークンの扱いを見直し、不要な権限や長期利用の資格情報を減らす。
- 対象サービスのアクセスログと異常なスキャン兆候を確認し、公開面の監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | Langflow | 言及あり | 0.80 | — |
| 製品 | n8n | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New NadMesh Botnet Hunts Exposed AI Services for Cloud Keys and Kubernetes Token](https://thehackernews.com/2026/07/new-nadmesh-botnet-hunts-exposed-ai.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-23002"></a>

### 1. CVE-2026-58644: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 50.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

CISAは、Microsoft SharePoint Serverに影響するCVE-2026-58644をKnown Exploited Vulnerabilities（KEV）カタログに追加しました。
公開情報では、これは重大度の高い脆弱性で、Microsoftは修正を案内しており、実際に悪用が確認されたとされています。
KEVへの追加は、単なる脆弱性情報ではなく、実際に攻撃で使われている可能性が高いことを示すため、優先的な対応が必要になります。
特にSharePointを運用している組織では、影響範囲の確認と適用状況の点検が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
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

- SharePoint Serverの導入有無を確認し、該当製品・該当バージョンに修正が適用済みか点検する。
- 公開情報で示される高リスク脆弱性として扱い、パッチ適用や緩和策を優先度高く進める。
- 関連する認証ログや異常な動作を確認し、侵害の兆候がないか監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-58644 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-58644](https://nvd.nist.gov/vuln/detail/CVE-2026-58644) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-58644: Microsoft SharePoint Server Unauthenticated Remote Code Executio](https://www.rapid7.com/blog/post/etr-cve-2026-58644-microsoft-sharepoint-server-unauthenticated-remote-code-execution-vulnerability-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds Exploited SharePoint RCE Zero-Day CVE-2026-58644 to KEV](https://thehackernews.com/2026/07/cisa-adds-exploited-sharepoint-rce-zero.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-22358"></a>

### 2. Microsoft 2026年7月 Patch Tuesday 関連まとめ

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>A⁠I</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 冷却中 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 48.0 |
| <nobr>確⁠度</nobr> | 57.0 |

#### 概要

Microsoftの2026年7月 Patch Tuesdayでは、622件の脆弱性修正が公表され、Edge向けChromium由来の脆弱性は別途427件含まれているとされています。
重大度の高い脆弱性が62件あり、公開前に知られていたものや、すでに悪用が確認されているものも含まれるため、対応の優先度が高い状況です。
修正件数が非常に多く、重要度の高い脆弱性や既知の悪用が含まれるため、組織の更新計画やリスク評価に直結します。
特に広く使われるWindowsやEdgeの更新は、適用遅延が影響範囲を広げやすい点で注目されます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 13 sources。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 悪用済みとされる脆弱性、公開済みの脆弱性、Critical判定の項目を優先して影響確認する。
- Windows本体だけでなく、EdgeのChromium由来修正も含めて更新状況を確認する。
- 一部環境で更新後の不具合報告もあるため、段階的展開や事前検証の有無を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-26145 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-27690 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-33842 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34328 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34346 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34348 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-34349 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-40378 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-40400 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-40422 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Why Microsoft paused Patch Tuesday updates for some Dell devices](https://www.itpro.com/security/why-microsoft-paused-patch-tuesday-updates-for-some-dell-devices) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft cancels Patch Tuesday for some Dell users over surprise shutdowns, ove](https://www.theregister.com/os-platforms/2026/07/15/microsoft-cancels-patch-tuesday-for-some-dell-users-over-surprise-shutdowns-overheating-devices/5271691) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [July 2026 Patch Tuesday fixes 622 Microsoft CVEs, including three zero-days](https://www.malwarebytes.com/blog/bugs/2026/07/july-2026-patch-tuesday-fixes-622-microsoft-cves-including-three-zero-days) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft smashes Patch Tuesday record for second successive month](https://therecord.media/microsoft-vulnerabilities-patch-tuesday-release) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Researcher Drops New Windows Zero-Day PoC Hours After Microsoft Patch Tuesday](https://thehackernews.com/2026/07/researcher-drops-new-windows-zero-day.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [AI-driven bug hunting fuels record Microsoft Patch Tuesday](https://www.helpnetsecurity.com/2026/07/15/microsoft-patch-tuesday-sharepoint-cve-2026-56164/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches 570 CVEs in Record Patch Tuesday](https://www.infosecurity-magazine.com/news/microsoft-570-cves-patch-tuesday/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Patch Tuesday - July 2026](https://www.rapid7.com/blog/post/em-patch-tuesday-july-2026) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: あり（1件）。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [ランサム被害のアサヒ、漏えいの可能性229万件に拡大 当初は191万件](https://www.itmedia.co.jp/news/articles/2607/17/news107.html) | 29.0 | 30.0 | 42.0 |
| [Seven Malicious Vite npm PackagesがブロックチェーンC2を使ってRATを配布](https://thehackernews.com/2026/07/seven-malicious-vite-npm-packages-use.html) | 28.0 | 45.0 | 42.0 |
| [政府機関がランサムウェアの被害に毎日遭っていると調査が警告](https://www.infosecurity-magazine.com/news/government-ransomware-daily/) | 28.0 | 30.0 | 42.0 |
| [ランサムウェア攻撃によりCoca-Colaが米国の乳業部門で生産停止](https://www.cybersecuritydive.com/news/ransomware-attack-coca-cola-suspend-production-dairy/825540/) | 28.0 | 30.0 | 42.0 |
| [Spiralsランサムウェアが24時間以内に被害システムをロックダウン](https://www.helpnetsecurity.com/2026/07/17/spirals-ransomware-south-asia/) | 28.0 | 30.0 | 42.0 |
| [ArmeniaでREvilハッカーとして米国の逮捕状が出ていたロシア人観光客を拘束、弁護士は別人だと主張](https://thehackernews.com/2026/07/armenia-detains-russian-tourist-on-us.html) | 28.0 | 30.0 | 42.0 |
| [The GentlemenがQilinを上回り最も活発なランサムウェア脅威に](https://www.infosecurity-magazine.com/news/the-gentlemen-most-prolific/) | 28.0 | 30.0 | 42.0 |
| [Ransomware攻撃によりCoca-ColaのFairlife米国乳製品生産が停止](https://www.helpnetsecurity.com/2026/07/17/coca-cola-fairlife-ransomware-attack/) | 28.0 | 30.0 | 42.0 |
| [GigaWiper：モジュール型サイバー兵器の内部構造](https://blog.polyswarm.io/gigawiper-inside-a-modular-cyberweapon) | 28.0 | 20.0 | 42.0 |
| [GoldenEyeDogサブグループに関連するDigiCert侵害とコード署名証明書窃取](https://thehackernews.com/2026/07/goldeneyedog-subgroup-linked-to.html) | 28.0 | 20.0 | 42.0 |
| [Ciscoが警鐘を鳴らす、米欧企業を標的とした新たなロシア系マルウェアキャンペーン](https://www.itpro.com/security/cyber-crime/cisco-sounds-alarm-over-new-russian-malware-campaign-hitting-firms-in-us-and-europe) | 28.0 | 20.0 | 42.0 |
| [SVG旗画像に隠されたOtterCookie連携マルウェアを配布する偽のコーディングテスト](https://thehackernews.com/2026/07/north-korea-linked-hackers-hide.html) | 28.0 | 20.0 | 42.0 |
| [GitHubを安全に使う方法](https://www.malwarebytes.com/blog/how-to/2026/07/how-to-use-github-safely) | 28.0 | 20.0 | 42.0 |
| [GoSerpentマルウェアが東南アジアの政府機関と外交官を標的にしたスパイ活動](https://thehackernews.com/2026/07/new-goserpent-malware-targets-southeast.html) | 28.0 | 20.0 | 42.0 |
| [Black Hat USA 2026でのMicrosoft：AI時代とサプライチェーン攻撃における信頼の防御](https://www.microsoft.com/en-us/security/blog/2026/07/17/microsoft-at-black-hat-usa-2026-defending-trust-in-the-age-of-ai-and-supply-chain-attacks/) | 27.0 | 20.0 | 42.0 |
| [AIの本当の脅威は盲目的な信頼です](https://www.darkreading.com/application-security/real-ai-threat-blind-trust) | 25.0 | 20.0 | 42.0 |
| [AIスパムフィルターが古典的なテキストサルティングにだまされる](https://www.theregister.com/security/2026/07/17/ai-spam-filters-are-getting-suckered-by-old-school-text-salting/5274434) | 25.0 | 20.0 | 42.0 |
| [Googleが「Agentic Defense」戦略で攻撃者を上回ると期待](https://www.darkreading.com/cloud-security/google-bets-agentic-defense-strategy-outpace-attackers) | 25.0 | 20.0 | 42.0 |
| [EU、GoogleにAndroidのマイク・カメラ・画面を競合AIアシスタントに開放するよう命令](https://thehackernews.com/2026/07/eu-orders-google-to-open-android-mic.html) | 25.0 | 20.0 | 42.0 |
| [Claudeが1Passwordで資格情報を公開せずにWebサイトへサインイン可能に](https://www.helpnetsecurity.com/2026/07/17/1password-anthropic-claude-integration/) | 25.0 | 20.0 | 42.0 |
| [Googleが修正する、PINなしでGeminiがSMSを送信できるAndroidロック画面の不具合](https://www.theregister.com/security/2026/07/17/google-fixing-android-lock-screen-bug-that-lets-gemini-send-sms-without-a-pin/5273027) | 25.0 | 20.0 | 42.0 |
| [OpenSSLサーバーのメモリを11バイトのペイロードで枯渇させるHollowByteのDDoS脆弱性](https://www.bleepingcomputer.com/news/security/hollowbyte-ddos-flaw-bloats-openssl-server-memory-with-11-byte-payload/) | 24.0 | 38.0 | 42.0 |
| [攻撃者がFortiSandboxの重大な脆弱性を狙う中、CISAがパッチ適用命令を発出](https://www.theregister.com/security/2026/07/17/attackers-target-critical-fortisandbox-flaws-as-cisa-issues-patch-order/5274287) | 24.0 | 38.0 | 42.0 |
| [「SharePoint Server」の複数脆弱性悪用で対策呼びかけ - 米当局](https://www.security-next.com/187553) | 24.0 | 20.0 | 43.0 |
| [公開講座申込者向けの事前メールで誤送信 - 島根県立大](https://www.security-next.com/187476) | 22.0 | 20.0 | 42.0 |
| [システムにサイバー攻撃か、影響範囲を調査 - 日産化学](https://www.security-next.com/187519) | 22.0 | 20.0 | 42.0 |
| [小学校で児童の個人情報含む絵画作品を紛失 - 大阪市](https://www.security-next.com/186819) | 22.0 | 20.0 | 42.0 |
| [Scattered Spiderの主要メンバー、英国で66か月の禁錮刑に判決](https://cyberscoop.com/scattered-spider-leaders-sentenced-united-kingdom/) | 20.0 | 20.0 | 48.0 |
| [州当局者と選挙専門家、Trump演説を非難「これが切迫の表れだ」](https://cyberscoop.com/state-officials-election-experts-pan-trump-voter-fraud-speech-call-it-desperation/) | 20.0 | 20.0 | 42.0 |
| [Abbott、がん診断事業へのサイバー攻撃を公表](https://www.cybersecuritydive.com/news/abbott-discloses-cyberattack-on-cancer-diagnostics-business/825552/) | 20.0 | 20.0 | 42.0 |
| [Ernst & Young、サポートシステムの侵害でデータ漏えいを公表](https://www.bleepingcomputer.com/news/security/ernst-and-young-discloses-data-breach-after-support-system-hack/) | 20.0 | 20.0 | 42.0 |
| [23andMe、1800万ドルのデータ侵害和解で新たなセキュリティ義務に直面](https://www.infosecurity-magazine.com/news/23andme-18m-data-breach-settlement/) | 20.0 | 20.0 | 42.0 |
| [Carding用の「クリーン」な住宅用プロキシを探る内部事情](https://www.bleepingcomputer.com/news/security/inside-the-search-for-clean-residential-proxies-for-carding/) | 20.0 | 20.0 | 42.0 |
| [米国の乳業企業Fairlifeがサイバーインシデント後に生産を停止](https://therecord.media/dairy-company-fairlife-suspends-production-us-cyber-incident) | 20.0 | 20.0 | 42.0 |
| [Gold Eagle Clearinghouseがセキュリティの隙間を狙う、ただし手口は不明](https://www.darkreading.com/vulnerabilities-threats/gold-eagle-clearinghouse-targets-security-gap) | 20.0 | 20.0 | 42.0 |
| [ゼレンスキー氏、ウクライナの治安庁長官代行を国防相代行に任命](https://therecord.media/ukraine-acting-defense-minister-yevhenii-khmara) | 20.0 | 20.0 | 42.0 |
| [Shark掃除機の脆弱性でカメラ、家の地図、Wi-Fiパスワードが露出](https://www.malwarebytes.com/blog/news/2026/07/shark-vacuum-flaw-exposes-cameras-home-maps-and-wi-fi-passwords) | 20.0 | 20.0 | 42.0 |
| [Podcast: Broken Governance、Agentic AI、MindStone Agentに関する独占公開](https://www.securityweek.com/podcast-broken-governance-agentic-ai-and-the-mindstone-agent-exclusive/) | 20.0 | 20.0 | 42.0 |
| [Beacon Securityがセキュリティデータプラットフォーム向けに1300万ドルを調達](https://www.securityweek.com/beacon-security-raises-13-million-for-security-data-platform/) | 20.0 | 20.0 | 42.0 |
| [PentagonによるCMMC Phase 2停止への業界の反応：Feedback Friday](https://www.securityweek.com/industry-reactions-to-pentagon-suspending-cmmc-phase-2-feedback-friday/) | 20.0 | 20.0 | 42.0 |
| [詐欺師がFaceTimeを悪用して銀行口座を不正送金させる手口](https://www.helpnetsecurity.com/2026/07/17/apple-facetime-calls-scams/) | 20.0 | 20.0 | 42.0 |
| [日本の冷凍食品大手ニチレイの業務を妨害したサイバー攻撃](https://www.securityweek.com/cyberattack-disrupts-operations-of-japanese-frozen-food-giant-nichirei/) | 20.0 | 20.0 | 42.0 |
| [ACR StealerがClickFixの誘導を悪用してブラウザトークンとMicrosoft 365ファイルを窃取](https://thehackernews.com/2026/07/acr-stealer-uses-clickfix-lures-to.html) | 20.0 | 20.0 | 42.0 |
| [Risk Ledger、シリーズBで3200万ドルを調達](https://www.securityweek.com/risk-ledger-raises-32-million-in-series-b-funding/) | 20.0 | 20.0 | 42.0 |
| [アサヒグループHD、新たに取引先の役員や従業員などの個人情報約37.8万件を「漏えいのおそれがある個人情報」として発表](https://internet.watch.impress.co.jp/docs/news/2126189.html) | 20.0 | 20.0 | 42.0 |
| [米国、投資詐欺による4300万ドルの資金洗浄で2人を起訴](https://www.bleepingcomputer.com/news/security/us-charges-two-over-laundering-43-million-from-investment-fraud/) | 20.0 | 20.0 | 42.0 |

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
