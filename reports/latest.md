# 📡 サイレーダー 2026-09-30 05:00 JST

このレポートは、2026-09-29 17:00 JST〜2026-09-30 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 119
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 88

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Custom malware used in Citrix 0-day attacks targeting govt, banks, professional services](#topic-34889) | 51.0 | 46.0 | 55.0 | 音声 | 温度感上位枠 |
| 2 | [Apple squashes zero-day bug exploited in “extremely sophisticated” attack (CVE-2026-86950)](#topic-34785) | 50.0 | 46.0 | 66.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [NetScaler zero-day exploitation escalates into mass attacks (CVE-2026-88771)](#topic-34525) | 49.0 | 74.0 | 67.0 | 音声 | 温度感上位枠 |
| 4 | [Dual NetScaler Zero-Days Trigger Chaos for Citrix Customers](#topic-34916) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [Citrix NetScaler vulnerabilities being actively exploited](#topic-34942) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [Malicious Custom GPT on chatgpt.com lures users into installing a RAT](#topic-34961) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [Star Blizzard refines phishing and malware delivery with the RedFlick technique](#topic-34908) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-34889"></a>

### 1. Custom malware used in Citrix 0-day attacks targeting govt, banks, professional services

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 51.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

Citrix NetScalerの脆弱性「CVE-2026-88772」を悪用したゼロデイ攻撃が観測され、カスタムのweb shellやトンネリング系マルウェアの投入につながったとされています。
攻撃者は認証情報の窃取やroot権限の取得、さらに内部ネットワークへの展開を狙った可能性が示されています。
政府機関、金融機関、専門サービス業などへの影響が示唆されており、境界機器の侵害がそのまま内部侵入につながるリスクがあるため注目されています。
ゼロデイ段階での悪用観測がある点も、迅速な対応の必要性を高めています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Citrix NetScalerの該当バージョンや公開済み修正情報を確認し、優先度高く適用状況を点検する。
- 外部公開面での異常な認証失敗、予期しないweb shell痕跡、トンネリング挙動などの有無を監視する。
- 侵害が疑われる場合は、認証情報の再発行やセッション無効化、内部横展開の有無を含めた広域調査を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-88772 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Citrix | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-88772](https://nvd.nist.gov/vuln/detail/CVE-2026-88772) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Hackers exploit Citrix NetScaler zero-day to deploy web shells](https://www.bleepingcomputer.com/news/security/hackers-exploit-citrix-netscaler-zero-day-to-deploy-web-shells/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Custom malware used in Citrix 0-day attacks targeting govt, banks, professional ](https://www.theregister.com/security/2026/09/29/custom-malware-used-in-citrix-0-day-attacks-targeting-govt-banks-professional-services/5299867) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34525"></a>

### 2. NetScaler zero-day exploitation escalates into mass attacks (CVE-2026-88771)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 49.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

CitrixのNetScaler ADCとNetScaler Gatewayに影響するCVE-2026-88771について、未修正環境への実際の悪用が確認され、攻撃が拡大していると報じられています。
関連情報では、公開された検証コードの存在も示されており、標的型の侵害から広範な攻撃へ移行している可能性が指摘されています。
NetScalerは外部公開されやすい境界機器として使われることが多く、侵害されると社内ネットワークへの影響が大きくなり得ます。
既知の悪用が確認されているため、単なる脆弱性情報ではなく、優先対応が必要な事案として注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
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

- NetScaler ADC / Gateway の該当バージョンと公開状況を確認し、ベンダー修正の適用可否を急いで点検する。
- インターネット公開している装置について、想定外の管理ポート露出や不要な公開範囲がないか見直す。
- 侵害の有無を前提に、認証情報の再点検や関連ログの確認など、周辺影響の調査を進める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-88771 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 脆弱性 | CVE-2026-88772 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-88771](https://nvd.nist.gov/vuln/detail/CVE-2026-88771) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [NetScaler zero-day exploitation escalates into mass attacks (CVE-2026-88771)](https://www.helpnetsecurity.com/2026/09/29/netscaler-zero-day-exploitation-escalates-into-mass-attacks-cve-2026-88771/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix patches actively exploited NetScaler zero-days after a weekend of unoffic](https://cyberscoop.com/citrix-zero-days-delayed-disclosure/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Threat Brief: NetScaler Zero Days CVE-2026-88771 and CVE-2026-88772 Exploited in](https://unit42.paloaltonetworks.com/netscaler-zero-days-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-88771 and CVE-2026-88772: Two Critical Citrix NetScaler Flaws Under Act](https://www.bitsight.com/blog/critical-vulnerability-alert-cve-2026-88771-cve-2026-88772-citrix-netscaler-flaws-under-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zero-Day Exploitation of Citrix NetScaler ADC and Gateway: CVE-2026-88771 and CV](https://www.rapid7.com/blog/post/etr-zero-day-exploitation-of-citrix-netscaler-adc-and-gateway-cve-2026-88771-and-cve-2026-88772) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Citrix NetScaler RCE zero-days exploited globally for weeks (CVE-2026-88771, CVE](https://www.helpnetsecurity.com/2026/09/28/citrix-netscaler-rce-zero-days-exploited-for-weeks-cve-2026-88771-cve-2026-88772/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: NetScaler ADCおよびNetScaler Gatewayにおける複数の脆弱性（CVE-2026-88771、CVE-2026-88772等](https://www.jpcert.or.jp/at/2026/at260029.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（2件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-34916"></a>

### 3. Dual NetScaler Zero-Days Trigger Chaos for Citrix Customers

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CitrixのNetScaler製品に関するゼロデイ脆弱性が報告され、既定設定で利用している環境に影響する可能性があるとされています。
公開材料では、攻撃者にネットワークへの広いアクセスを許し得る重大な問題として扱われており、悪用観測の文脈も示されています。
境界機器やリモートアクセス基盤に関わる脆弱性は、影響範囲が広くなりやすく、侵入の起点として狙われやすいため注目されます。
ゼロデイかつ悪用情報ありの状況では、パッチ適用や緩和策の優先度が高まります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- NetScalerの利用有無と適用バージョン、既定設定のまま使っていないかを確認する。
- ベンダーの修正情報や回避策を確認し、適用可能なものは速やかに反映する。
- 境界装置の認証ログ、管理ログ、異常なセッションや設定変更の有無を重点的に点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Citrix | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Dual NetScaler Zero-Days Trigger Chaos for Citrix Customers](https://www.darkreading.com/vulnerabilities-threats/netscaler-zero-days-chaos-citrix) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34942"></a>

### 4. Citrix NetScaler vulnerabilities being actively exploited

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Citrix NetScaler ADC と Gateway に影響する脆弱性について、実際に悪用が観測されているとされています。
現時点では細かな脆弱性番号は示されていませんが、早急な緩和対応が求められる状況です。
ネットワーク境界に置かれやすい製品が対象のため、影響範囲が広くなりやすい点が注目されています。悪用が確認されている場合、公開後すぐの対応遅れが侵害につながるおそれがあります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Citrix の案内やセキュリティ情報を確認し、該当バージョンの有無を点検する。
- 外部公開されている NetScaler ADC / Gateway の管理面・関連サービスを優先して監視する。
- パッチ適用がすぐに難しい場合は、ベンダー推奨の緩和策を適用し、ログを重点的に確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Citrix NetScaler vulnerabilities being actively exploited](https://www.itpro.com/cloud/cloud-security/citrix-netscaler-vulnerabilities-being-actively-exploited) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34961"></a>

### 5. Malicious Custom GPT on chatgpt.com lures users into installing a RAT

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報によると、ChatGPTのCustom GPTを悪用した誘導が確認され、ユーザーを偽のCloudflare CAPTCHA確認へ導いたうえで、RATの実行につながる流れが報告されています。
広告経由の検索結果を足がかりにした手口とされ、複数の被害相談があったとされていますが、詳細な被害範囲は現時点で断定できません。
AIサービスの利用画面や関連機能が、単なる情報収集だけでなく攻撃の誘導面として使われうる点が注目されています。
正規サービスに見える導線を悪用するため、利用者教育と検索・広告経由のリスク対策が重要です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI関連の正規UIやCustom GPTを起点にした誘導を前提に、利用者向け注意喚起を行う。
- 検索広告や外部サイトからの遷移先で、CAPTCHAやダウンロード要求が出た場合の確認手順を再点検する。
- エンドポイント側で不審な実行ファイルの起動や遠隔操作系マルウェアの兆候を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cloudflare | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| AIモデル/プロジェクト | ChatGPT | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Malicious Custom GPT on chatgpt.com lures users into installing a RAT](https://www.helpnetsecurity.com/2026/09/29/malicious-chatgpt-custom-gpt-malware-via-clickfix/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-34908"></a>

### 6. Star Blizzard refines phishing and malware delivery with the RedFlick technique

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>i⁠O⁠S</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Microsoftは、ロシア由来とされる脅威グループStar Blizzardが、フィッシング活動や検知回避の手法を進化させていると報告しました。
公開情報では、侵害されたWebサイト上のアカウントの悪用や、MicrosoftがRedFlickと呼ぶ新たなマルウェア配信手法が観測されたとされています。
標的型フィッシングとマルウェア配信の両面で手口が洗練されている可能性があり、受信者側の見分けが難しくなります。
特にクラウドや業務用アカウントを経由した誘導は、従来の注意喚起だけでは防ぎにくいため注視が必要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 不審なメールやリンクだけでなく、正規に見えるアカウントやWebサイト経由の誘導も前提に、認証強化と監視を見直す。
- メール・クラウド・端末の各層で、異常なログイン、転送設定、ファイル取得の兆候を継続的に確認する。
- ユーザー向けには、外部から送られた招待や共有要求をそのまま開かず、送信元確認を徹底する運用を周知する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脅威アクター | Star Blizzard | 主題 | 0.80 | — |
| ベンダー | Mandiant | 言及あり | 0.80 | — |
| ベンダー | Proofpoint | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | cPanel | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | Apple | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |
| 製品 | Microsoft 365 | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Star Blizzard refines phishing and malware delivery with the RedFlick technique](https://www.microsoft.com/en-us/security/blog/2026/09/29/star-blizzard-refines-phishing-and-malware-delivery-with-the-redflick-technique/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-34785"></a>

### 1. Apple squashes zero-day bug exploited in “extremely sophisticated” attack (CVE-2026-86950)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>i⁠O⁠S</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 50.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Appleは、CoreGraphicsに存在するゼロデイ脆弱性CVE-2026-86950を修正する更新を公開しました。
複数の情報源によれば、この問題は特定の対象に対する高度な攻撃で悪用されていた可能性があり、Appleも一部の古いOS系統向け更新にセキュリティ修正を含めています。
ゼロデイで既に悪用が確認されている、またはその可能性が示されている点が重要です。対象端末では機密情報の保護や被害拡大防止のため、早期適用の優先度が高いと考えられます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
- 実悪用・ゼロデイ文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- iOS/macOSの該当バージョンで提供されている最新アップデートを早急に適用する。
- Appleの案内に従い、影響を受ける旧系統と非対象の新系統を切り分けて更新状況を確認する。
- 高リスク端末や標的になりやすい利用者については、更新完了まで監視とインシデント対応手順を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-86950 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Apple | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Apple iOS | 言及あり | 0.80 | — |
| ベンダー | Meta | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-86950](https://nvd.nist.gov/vuln/detail/CVE-2026-86950) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Apple patches CoreGraphics zero-day already exploited in targeted attacks](https://www.theregister.com/security/2026/09/29/apple-patches-coregraphics-zero-day-already-exploited-in-targeted-attacks/5299721) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Update your iPhone, iPad, or Mac: Flaw could run attackers’ code](https://www.malwarebytes.com/blog/bugs/2026/09/update-your-iphone-ipad-or-mac-flaw-could-run-attackers-code) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple squashes zero-day bug exploited in “extremely sophisticated” attack (CVE-2](https://www.helpnetsecurity.com/2026/09/29/apple-core-graphics-zero-day-cve-2026-86950-fixed/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Patches Zero-Day Linked to ‘Extremely Sophisticated Attack’](https://www.securityweek.com/apple-patches-meta-reported-zero-day-linked-to-extremely-sophisticated-attack/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Emergency Patch for iOS 26, macOS26, macOS15 (CVE-2026-86950), (Mon, Sep 2](https://isc.sans.edu/diary/rss/33376) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [101個の悪意あるnpmパッケージが開発者のWhatsAppアカウントを同意なくグループに追加](https://thehackernews.com/2026/09/101-malicious-npm-packages-add.html) | 28.0 | 35.0 | 42.0 |
| [Arizona州最高裁判所、住民の個人情報が盗まれたと発表](https://therecord.media/arizona-supreme-court-says-hackers-stole-data) | 28.0 | 30.0 | 42.0 |
| [元米空軍関係者、BEC攻撃で実刑判決](https://www.bleepingcomputer.com/news/security/former-us-air-force-members-sent-to-prison-over-bec-attacks/) | 28.0 | 20.0 | 42.0 |
| [Star Blizzardが偽のイベント招待で100以上の組織を標的にバックドアを配布](https://thehackernews.com/2026/09/russias-star-blizzard-targets-100.html) | 28.0 | 20.0 | 42.0 |
| [NeedyMantisが侵害ネットワークへの長期アクセスを提供](https://www.darkreading.com/threat-intelligence/needymantis-long-term-access-compromised-networks) | 28.0 | 20.0 | 42.0 |
| [RatHatの進化するC2パネルが示すMalware-as-a-Serviceモデル](https://www.infosecurity-magazine.com/news/rathat-c2-panel-malware-as-a/) | 28.0 | 20.0 | 42.0 |
| [Microsoft、NeedyMantisマルウェアによる永続的なネットワークアクセスを警告](https://www.infosecurity-magazine.com/news/microsoft-needymantis-malware/) | 28.0 | 20.0 | 42.0 |
| [Microsoftが解析したDaemon Tools標的のNeedyMantisマルウェア](https://www.securityweek.com/daemon-tools-hackers-needymantis-malware-dissected-by-microsoft/) | 28.0 | 20.0 | 42.0 |
| [AIエージェント「Manus 2.0」リリース、さらにパーソナルAIエージェント向けアプリ「Cue」やプロフェッショナルなAIワークスペースを実現するデスクトップアプリ「Manus Studio」も](https://gigazine.net/news/20260929-manus-2-0/) | 27.0 | 20.0 | 42.0 |
| [MetaのAI「Muse」にFacebook Marketplaceの対応を任せたら勝手に値下げ＆住所公開、購入者が自宅に来る事態に](https://gigazine.net/news/20260929-meta-muse-give-home-address/) | 27.0 | 20.0 | 42.0 |
| [Anthropic、IPO目論見書でAIによる「人類存亡リスク」を警告 海外報道](https://www.itmedia.co.jp/news/article/2609/29/2000001860/) | 26.0 | 20.0 | 42.0 |
| [みんながAIを気軽に使うと、電力消費がものすごく上がる。じゃあどうすればいい？](https://ascii.jp/elem/000/004/437/4437295/?rss=) | 26.0 | 20.0 | 42.0 |
| [ワークスアプリ、大手企業向けローコード基盤をAIエージェントで強化](https://japan.zdnet.com/article/35253077/) | 26.0 | 20.0 | 42.0 |
| [IIJ、新人エンジニア向け研修教材を無料公開 Web技術の基礎から生成AI活用まで20講義超](https://www.itmedia.co.jp/news/article/2609/29/2000001854/) | 26.0 | 20.0 | 42.0 |
| [米国、サイバーセキュリティと国家のサイバー防衛に向けてAIを重要インフラに活用へ](https://cyberscoop.com/national-cyber-director-ai-critical-infrastructure-cybersecurity/) | 25.0 | 20.0 | 42.0 |
| [DARPAが軍用メッセージングアプリの保護にAI活用へXintを選定](https://www.securityweek.com/darpa-selects-xint-to-use-ai-in-securing-military-messaging-apps/) | 25.0 | 20.0 | 42.0 |
| [AIモデルがテック企業内部の機密情報を含むスクリーンショットを投稿し続ける問題](https://www.theregister.com/ai-and-ml/2026/09/29/ai-models-keep-posting-screenshots-showing-sensitive-data-from-inside-tech-companies/5299640) | 25.0 | 20.0 | 42.0 |
| [自動化AIエージェントを用いたサイバーセキュリティ非営利団体DIVDへの侵害](https://www.bleepingcomputer.com/news/security/automated-ai-agent-used-to-breach-cybersecurity-nonprofit-divd/) | 25.0 | 20.0 | 42.0 |
| [AI時代における建設業界のサイバーセキュリティ対策](https://www.cybersecuritydive.com/news/construction-cybersecurity-AI/831637/) | 25.0 | 20.0 | 42.0 |
| [LastPass、従業員にAIツールへの機密データ共有前の注意を喚起](https://www.helpnetsecurity.com/2026/09/29/lastpass-ai-monitoring-and-protect/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、GPT-6.1 Astraの逸脱挙動を評価しベンチに登録](https://www.theregister.com/ai-and-ml/2026/09/29/openai-benches-gpt-61-astra-for-overstepping-the-mark/5299743) | 25.0 | 20.0 | 42.0 |
| [ハッカーがClickFix攻撃でChatGPTのCustom GPTを悪用](https://www.securityweek.com/hackers-use-chatgpt-custom-gpts-in-clickfix-attacks/) | 25.0 | 20.0 | 42.0 |
| [AIを活用したポスト量子移行のロードマップ策定](https://blog.cloudflare.com/ai-driven-cryptography-discovery/) | 25.0 | 20.0 | 42.0 |
| [Metaが中小企業向けに業務を理解するAIエージェントを提供](https://www.helpnetsecurity.com/2026/09/29/meta-muse-for-small-business/) | 25.0 | 20.0 | 42.0 |
| [Vega IIがSOCにセキュリティ学習済みAIと長期記憶をもたらす](https://www.helpnetsecurity.com/2026/09/29/vega-ii-agentic-cyber-defense-platform/) | 25.0 | 20.0 | 42.0 |
| [Rig Security、Agentic AIのアイデンティティリスク対策に1,200万ドルを調達](https://www.securityweek.com/rig-security-emerges-from-stealth-with-12m-to-tackle-agentic-ai-identity-risks/) | 25.0 | 20.0 | 42.0 |
| [役員がディープフェイクの標的になると経営課題になる深刻化](https://www.helpnetsecurity.com/2026/09/29/pindrop-enterprise-deepfake-attacks-report/) | 25.0 | 20.0 | 42.0 |
| [OpenAIのGPT-6 Astraが指示に反してサプライチェーン攻撃を実行](https://www.helpnetsecurity.com/2026/09/29/openai-gpt-6-astra-supply-chain-attacks-test-simulations/) | 25.0 | 20.0 | 42.0 |
| [OpenAI、GPT-6.1 Astraの公開を中止し、フロンティア訓練の安全性事例を詳細化](https://www.securityweek.com/openai-calls-off-gpt-6-1-astra-launch-details-safety-cases-for-frontier-training/) | 25.0 | 20.0 | 42.0 |
| [Palo Alto NetworksとNVIDIA、AIエージェントの制御強化を目指す](https://www.helpnetsecurity.com/2026/09/29/palo-alto-networks-nvidia-ai-agent-security/) | 25.0 | 20.0 | 42.0 |
| [Copilotユーザーの奇妙で不適切な画像編集依頼を人間がレビューしている](https://www.malwarebytes.com/blog/ai/2026/09/humans-are-reviewing-copilot-users-bizarre-and-abusive-image-editing-requests) | 25.0 | 20.0 | 42.0 |
| [グーグル Gemini「Gems」終了へ](https://news.yahoo.co.jp/pickup/6596966?source=rss) | 25.0 | 20.0 | 42.0 |
| [Claude Sonnet 5.5が価格据え置きで高速化](https://www.helpnetsecurity.com/2026/09/29/anthropic-claude-sonnet-5-5/) | 25.0 | 20.0 | 42.0 |
| [MikroTik RouterOSの脆弱性とセキュリティ対策](https://www.cisa.gov/news-events/ics-advisories/icsa-26-272-06) | 24.0 | 46.0 | 50.0 |
| [Toptech TMS7およびTopHATの脆弱性問題](https://www.cisa.gov/news-events/ics-advisories/icsa-26-272-02) | 24.0 | 46.0 | 50.0 |
| [Anjvision YSSD-RTMP-H5の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-272-05) | 24.0 | 46.0 | 50.0 |
| [VIVOTEKカメラのファームウェア](https://www.cisa.gov/news-events/ics-advisories/icsa-26-272-03) | 24.0 | 46.0 | 50.0 |
| [Baicells Nova 430Hの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-272-04) | 24.0 | 46.0 | 50.0 |
| [ソースコードの先へ：王国への鍵に迫る道](https://www.microsoft.com/en-us/security/blog/2026/09/29/beyond-source-code-a-path-to-the-keys-to-the-kingdom/) | 22.0 | 20.0 | 42.0 |
| [オープンキャンパスの受付名簿が所在不明 - 三重大](https://www.security-next.com/190384) | 22.0 | 20.0 | 42.0 |
| [生徒の健康記録紛失、大規模改修時の移動で - 新潟市中学校](https://www.security-next.com/190689) | 22.0 | 20.0 | 42.0 |
| [アプリ経由で会員情報サーバに第三者アクセス- セイコーマート](https://www.security-next.com/190794) | 22.0 | 20.0 | 42.0 |
| [「GPT-6 Astraは旧世代モデルよりサイバー攻撃を実行しやすい傾向にある」というイギリス政府機関の分析結果が公開される](https://gigazine.net/news/20260929-gpt-6-astra-aisi-report/) | 22.0 | 20.0 | 42.0 |
| [WatchGuard製アクセスポイントに複数脆弱性 - 「クリティカル」も](https://www.security-next.com/190814) | 22.0 | 20.0 | 42.0 |
| [Lantronix G520 Series Cellular Gatewayの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-272-01) | 21.0 | 34.0 | 50.0 |
| [チケット販売サイト「イープラス」に不正アクセス、個人情報1463件漏えい 口座情報や住所なども一部流出](https://www.itmedia.co.jp/news/article/2609/29/2000001861/) | 21.0 | 20.0 | 42.0 |
| [ヤマト運輸「クロネコ代金後払い」、不正アクセスでサービス停止、宅急便などは通常通り](https://www.itmedia.co.jp/news/article/2609/29/2000001859/) | 21.0 | 20.0 | 42.0 |
| [AI活用企業の84.7%がセキュリティリスク増加を懸念、93.4%がエンドポイント対策重要と回答](https://news.mynavi.jp/techplus/article/20260929-5047108/) | 21.0 | 20.0 | 42.0 |
| [Viidure Dashcam Androidアプリケーション](https://www.cisa.gov/news-events/ics-advisories/icsa-26-272-07) | 20.0 | 28.0 | 50.0 |
| [ShinyHuntersのリーダーとされる人物がオランダで逮捕](https://cyberscoop.com/shinyhunters-alleged-leader-arrested-netherlands/) | 20.0 | 20.0 | 48.0 |
| [盗まれた職員パスワードを使ったフランス税務データ窃取が7週間にわたり発覚せず](https://thehackernews.com/2026/09/french-tax-data-theft-using-stolen.html) | 20.0 | 20.0 | 42.0 |
| [Spectre-v2の新たなBTR攻撃が既存の防御をすり抜けてLinuxメモリを漏えいさせる](https://thehackernews.com/2026/09/new-spectre-v2-btr-attack-leaks-linux.html) | 20.0 | 20.0 | 42.0 |
| [Spectre v2の新たな攻撃手法でLinuxのrootパスワードハッシュが数分で漏えいする問題](https://www.bleepingcomputer.com/news/security/new-spectre-v2-attack-variant-leaks-linux-root-password-hash-in-minutes/) | 20.0 | 20.0 | 42.0 |
| [Cloudflare、ポスト量子Web向けの公開証明書認証局を発表](https://www.darkreading.com/cloud-security/cloudflare-announces-public-certificate-authority-post-quantum-web) | 20.0 | 20.0 | 42.0 |
| [Spectre v2の新たな亜種によりIntel、AMD、Arm CPUでデータ漏えいの恐れ](https://www.securityweek.com/new-spectre-v2-variant-exposes-intel-amd-arm-cpus-to-data-leaks/) | 20.0 | 20.0 | 42.0 |
| [Citrix NetScalerの悪用は公表通知の数日前から始まっていた](https://www.cybersecuritydive.com/news/citrix-netscaler-exploitation-days-before-notification/831634/) | 20.0 | 20.0 | 42.0 |
| [Symantec PAMセカンダリサイトの実践ガイド](https://www.security.com/product-insights/part-2-why-less-more-symantec-pam-clustering) | 20.0 | 20.0 | 42.0 |
| [GAO報告書、重複するサイバーセキュリティ規制に対する業界の懸念を指摘](https://www.cybersecuritydive.com/news/cybersecurity-regulation-industry-feedback-harmonization-gao/831619/) | 20.0 | 20.0 | 42.0 |
| [RemoteThreatが攻撃運用プラットフォーム向けに700万ドルを調達](https://www.securityweek.com/remotethreat-launches-with-7-million-for-offensive-operations-platform/) | 20.0 | 20.0 | 42.0 |
| [Kiteworks、9時間の予防的停止中に見つかった重大な脆弱性を修正](https://thehackernews.com/2026/09/kiteworks-fixes-critical-flaw-found.html) | 20.0 | 20.0 | 42.0 |
| [Kiteworks、連邦当局からの「信頼できる脅威インテリジェンス」受け停止勧告を解除](https://cyberscoop.com/kiteworks-lifts-shutdown-advisory-after-credible-threat-intelligence-from-federal-authorities/) | 20.0 | 20.0 | 42.0 |
| [リアルタイムのIDテレメトリで脅威の深刻化を未然に防ぐ](https://www.bleepingcomputer.com/news/security/catch-threats-before-they-escalate-with-real-time-identity-telemetry/) | 20.0 | 20.0 | 42.0 |
| [Amazon Bedrock AgentCoreの欠陥によりAWS認証情報が漏えいする可能性](https://www.infosecurity-magazine.com/news/aws-agentcore-sdk-flaws-ai/) | 20.0 | 20.0 | 42.0 |
| [Reco、エージェンティック・セキュリティ向けに5500万ドルを調達](https://www.securityweek.com/reco-raises-55-million-for-agentic-security/) | 20.0 | 20.0 | 42.0 |
| [NvidiaがHugging Faceへの攻撃を防げた可能性のある安全性プラットフォームを発表](https://www.itpro.com/technology/artificial-intelligence/nvidia-unveils-safety-platform-that-could-have-stopped-hugging-face-attack) | 20.0 | 20.0 | 42.0 |
| [Merkle Tree Certificatesを用いたポスト量子証明機関の構築](https://blog.cloudflare.com/pq-ca-with-mtcs/) | 20.0 | 20.0 | 42.0 |
| [TrendAI™による自律的な脆弱性発見の紹介：機械速度で進む次世代の脅威修復](https://newsroom.trendmicro.com/2026-09-29-Introducing-TrendAI-TM-Autonomous-Vulnerability-Discovery-Next-Generation-Threat-Remediation-at-Machine-Speed) | 20.0 | 20.0 | 42.0 |
| [Cloudflare Application Profilesによるポジティブセキュリティの強制](https://blog.cloudflare.com/application-profiles/) | 20.0 | 20.0 | 42.0 |
| [Cloudflareアカウント向けのオープンソース脅威インテリジェンスを強化するThreat Signalsの導入](https://blog.cloudflare.com/threat-signals/) | 20.0 | 20.0 | 42.0 |
| [あなたのドメインは耐量子暗号を使用しているか？自分で確認できるようになった](https://blog.cloudflare.com/post-quantum-visibility/) | 20.0 | 20.0 | 42.0 |
| [MetaのMuseがFacebook Marketplaceの買い手を売り手の自宅へ案内した問題](https://www.malwarebytes.com/blog/news/2026/09/metas-muse-sent-a-facebook-marketplace-buyer-to-a-sellers-home) | 20.0 | 20.0 | 42.0 |
| [Blue Agentの視点：AWSとGitHubにまたがるマルチプラットフォームのデータ流出を調査する](https://www.wiz.io/blog/blue-agent-data-exfiltration-investigation) | 20.0 | 20.0 | 42.0 |
| [ロシアのピザチェーン、ハッカーの主張後にサイバー攻撃を確認](https://therecord.media/russian-pizza-chain-dodo-confirms-data-breach) | 20.0 | 20.0 | 42.0 |
| [Pentagon Personnel Agencyのデータ侵害、300万人に影響](https://www.securityweek.com/pentagon-personnel-agency-data-breach-impacts-3-million-people/) | 20.0 | 20.0 | 42.0 |
| [イープラス 個人情報1463件漏えい](https://news.yahoo.co.jp/pickup/6596987?source=rss) | 20.0 | 20.0 | 42.0 |
| [ベトナム人男性、1600万ドル規模の「豚の解体」暗号資産詐欺で起訴](https://www.bleepingcomputer.com/news/security/vietnamese-man-charged-in-16-million-pig-butchering-crypto-scam/) | 20.0 | 20.0 | 42.0 |
| [将来に向けて大きな計画を秘める4つのサイバー脅威](https://www.securityweek.com/four-cyber-threats-harboring-big-plans-for-the-future/) | 20.0 | 20.0 | 42.0 |
| [元X-Forceハッカーたちが追う攻撃的サイバー分野のゴールドラッシュ](https://www.theregister.com/security/2026/09/29/former-x-force-hackers-chase-the-offensive-cyber-gold-rush/5299662) | 20.0 | 20.0 | 42.0 |
| [ShinyHunters捜査でオランダ警察が有罪判決を受けたハッカーを逮捕](https://www.securityweek.com/dutch-police-arrest-convicted-hacker-in-shinyhunters-investigation/) | 20.0 | 20.0 | 42.0 |
| [サイバーセキュリティの採用慣行ではジュニア人材の活躍の余地が少ない](https://www.helpnetsecurity.com/2026/09/29/skillbit-cybersecurity-micro-training-trends-report/) | 20.0 | 20.0 | 42.0 |
| [OperTraitors: Kubernetes Operatorがセキュリティ体制を損なう仕組み](https://unit42.paloaltonetworks.com/agentic-ai-kubernetes-operator-risks/) | 20.0 | 20.0 | 42.0 |
| [偽のiPhone Duo予約販売詐欺がDarkSword攻撃を引き起こす](https://www.malwarebytes.com/blog/threat-intel/2026/09/fake-iphone-duo-preorder-scam-triggers-darksword-attack) | 20.0 | 20.0 | 42.0 |
| [日本の鉄道事業者が週末のサイバー攻撃を受ける](https://www.infosecurity-magazine.com/news/japanese-railway-operators-cyber/) | 20.0 | 20.0 | 42.0 |
| [Kiteworks、シャットダウン通知後にシステム再起動を顧客に要請](https://www.infosecurity-magazine.com/news/kiteworks-customers-restart/) | 20.0 | 20.0 | 42.0 |
| [ハッカーがSQLインジェクションの脆弱性を悪用し、ポーランドの医療ソフトウェア提供企業から患者データを窃取](https://www.helpnetsecurity.com/2026/09/29/qbusoft-medyc-data-breach-poland/) | 20.0 | 20.0 | 42.0 |
| [Kiteworksが重大な脆弱性を修正し、顧客システムをオンライン化](https://www.bleepingcomputer.com/news/security/kiteworks-lifts-shutdown-warning-after-patching-critical-flaw/) | 20.0 | 20.0 | 42.0 |
| [CloudflareのEmDash 1.0、サンドボックス化されたプラグインに事前のアクセス許可を要求させる](https://www.helpnetsecurity.com/2026/09/29/cloudflare-emdash-plugin-security/) | 20.0 | 20.0 | 42.0 |
| [2026年9月の主なサイバー攻撃：米国とEUでセッション乗っ取り、リモートアクセス、決済詐欺が発生](https://any.run/cybersecurity-blog/major-cyber-attacks-september-2026/) | 20.0 | 20.0 | 42.0 |

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
