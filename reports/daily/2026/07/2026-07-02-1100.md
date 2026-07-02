# 📡 サイレーダー 2026-07-02 11:00 JST

このレポートは、2026-07-02 05:00 JST〜2026-07-02 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 65
- [音声で扱う想定のトピック](#audio-topics): 4
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 35

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [「Cisco Unified CM」のSSRF脆弱性、悪用に注意](#topic-14652) | 57.0 | 96.0 | 91.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [米当局、「SharePoint Server」の脆弱性悪用に注意喚起](#topic-20474) | 39.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [FortiBleed credential-theft campaign linked to Lynx ransomware](#topic-20517) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [ChocoPoc malware delivered via trojanized exploits on GitHub](#topic-20529) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [New ChocoPoC malware targets researchers via trojanized PoC exploits](#topic-20528) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-20474"></a>

### 1. 米当局、「SharePoint Server」の脆弱性悪用に注意喚起

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

米当局は、Microsoft SharePoint Server の脆弱性が悪用されているとして注意を呼びかけています。
該当の問題は2026年5月の月例セキュリティ更新で修正されたもので、当初は十分な情報提供がないまま後からアドバイザリが出るなど、対応の経緯が通常と異なっていました。
業務で広く使われるSharePoint Serverが対象であり、未対策環境があると被害につながるおそれがあります。
公的機関が悪用を前提に警戒を促しているため、単なる脆弱性情報より優先度を上げて確認すべき案件です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- PoC/Exploit候補: 候補あり（該当CVE 1件 / URL 3件以上）。

#### 担当者向け確認ポイント

- 該当するSharePoint Serverの更新適用状況を確認し、未適用なら速やかにパッチを適用する。
- 外部公開しているSharePoint環境がある場合は、関連する監視・ログ確認を強化する。
- Microsoftや関係当局の追加情報を確認し、影響範囲や推奨対処を継続的に見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-45659 | 関連CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [米当局、「SharePoint Server」の脆弱性悪用に注意喚起](https://www.security-next.com/186688) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20517"></a>

### 2. FortiBleed credential-theft campaign linked to Lynx ransomware

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

FortiBleedと呼ばれるFortinet関連の認証情報窃取キャンペーンが、INCおよびLynxランサムウェアの活動と関連づけられています。
公開情報では、盗まれた認証情報が将来的なネットワーク侵入に利用される可能性が示唆されていますが、具体的な影響範囲や被害の全容はまだ明確ではありません。
Fortinet製品や関連アカウントの認証情報が狙われると、侵入後の横展開やランサムウェア被害につながるおそれがあります。
脅威アクター間の関連が示されているため、単発の漏えいではなく継続的な攻撃準備として注意が必要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Fortinet関連の管理者アカウントやVPN/認証基盤のログイン履歴を確認し、異常な利用がないか監視する。
- 多要素認証の有効化、認証情報の使い回し排除、不要アカウントの整理を優先する。
- 外部公開面の設定やパッチ適用状況を見直し、侵入経路になり得る箇所を継続的に点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ベンダー | Fortinet | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [FortiBleed credential-theft campaign linked to Lynx ransomware](https://www.bleepingcomputer.com/news/security/fortibleed-credential-theft-campaign-linked-to-lynx-ransomware/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-20529"></a>

### 3. ChocoPoc malware delivered via trojanized exploits on GitHub

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>P⁠o⁠C</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

GitHub上で公開されていた複数の武器化されたPoC exploitに、PythonベースのRAT「ChocoPoC」が仕込まれていたと報じられています。
報告によると、このマルウェアはコマンド実行や機密情報の窃取に悪用される可能性があります。
攻撃者が検証用コードやPoCを装ってマルウェアを配布する手口は、開発者や調査担当者が誤って実行してしまうリスクがあります。
公開リポジトリ経由の供給網リスクとして、日常的なコード取得・検証の運用に影響し得る点が注目されます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- PoCや検証用コードは、出所だけでなく内容差分や不審な依存関係も確認する。
- GitHub由来のアーカイブやスクリプトを扱う際は、隔離環境での検証を徹底する。
- 端末やリポジトリ監査で、想定外の外部通信・コマンド実行・情報収集の兆候を点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ChocoPoc malware delivered via trojanized exploits on GitHub](https://www.bleepingcomputer.com/news/security/chocopoc-malware-delivered-via-trojanized-exploits-on-github/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-20528"></a>

### 4. New ChocoPoC malware targets researchers via trojanized PoC exploits

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

GitHub上で配布されていた複数のPoC（概念実証）エクスプロイトに、PythonベースのRAT「ChocoPoC」が仕込まれていたと報じられています。
攻撃はサイバーセキュリティ研究者を狙ったものとみられており、コマンド実行や機微情報の窃取につながる可能性が指摘されています。
PoCや検証用コードは研究・調査の現場で利用されやすく、信頼して実行すると端末や認証情報を危険にさらすおそれがあります。
特に研究者や脆弱性検証を行う実務者は、入手したコードの真正性確認と実行環境の分離をより厳格に求められます。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- PoCや検証コードは、入手元だけでなく改変の有無も確認してから扱う。
- 研究・検証用の端末や環境は、業務ネットワークや重要な認証情報から切り離す。
- 不審な挙動があれば、実行前提の検証を止めて端末の監視・調査を優先する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New ChocoPoC malware targets researchers via trojanized PoC exploits](https://www.bleepingcomputer.com/news/security/new-chocopoc-malware-targets-researchers-via-trojanized-poc-exploits/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-14652"></a>

### 1. 「Cisco Unified CM」のSSRF脆弱性、悪用に注意

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 57.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 96.0 |
| <nobr>確⁠度</nobr> | 91.0 |

#### 概要

Cisco Unified Communications Manager（Unified CM）および Unified CM SME に、未認証のリモート攻撃者による SSRF につながる脆弱性（CVE-2026-20230）が報告されています。
Cisco は修正済みソフトウェアを公開しており、公開情報では悪用観測があるとされています。通信基盤として使われる製品のため、影響範囲が大きくなり得ます。
さらに、悪用されるとOS上でのファイル書き込みを起点に権限昇格へつながる可能性があるため、優先度の高い対応が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 8 sources。
- CISA KEV関連。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- PoC/Exploit候補: 候補あり（該当CVE 2件 / URL 6件以上）。

#### 担当者向け確認ポイント

- 対象製品のバージョンを確認し、Cisco の修正済みソフトウェア適用を急ぐ。
- WebDialer サービスの有効化状況を確認し、不要なら無効化を検討する。
- 関連ログや不審な HTTP リクエスト、想定外のファイル生成の有無を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20230 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-20245 | 関連CVE | 1.00 |
| ベンダー | Cisco | 影響ベンダー | 1.00 |
| 製品 | Unified Communications Manager | 影響製品 | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20230](https://nvd.nist.gov/vuln/detail/CVE-2026-20230) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [「Cisco Unified CM」のSSRF脆弱性、悪用に注意](https://www.security-next.com/186698) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified Communications Manager Server-Side Request Forgery Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-cucm-ssrf-cXPnHcW) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [The hits keep on coming for Cisco vulnerabilities](https://www.theregister.com/security/2026/06/24/the-hits-keep-on-coming-for-cisco-vulnerabilities/5261797) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified CM flaw actively exploited to drop webshells (CVE-2026-20230)](https://www.helpnetsecurity.com/2026/06/24/cisco-unified-cm-flaw-exploited-to-drop-webshells-cve-2026-20230/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified CM Flaw Exploited After PoC Reveals File-Write Path to Root](https://thehackernews.com/2026/06/cisco-unified-cm-flaw-exploited-after.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers Exploiting Cisco Unified CM Vulnerability](https://www.securityweek.com/hackers-exploiting-cisco-unified-cm-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Unified CM flaw CVE-2026-20230 now exploited in attacks](https://www.bleepingcomputer.com/news/security/cisco-unified-cm-sme-flaw-cve-2026-20230-now-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（1件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [「ランサムウェア」侵入手順を徹底解説 もう知ったかぶりからは卒業しよう](https://www.itmedia.co.jp/enterprise/articles/2607/02/news041.html) | 29.0 | 30.0 | 42.0 |
| [巧妙なフィッシングキャンペーンが被害者の端末とOSに自動適応](https://www.darkreading.com/application-security/phishing-campaigns-auto-adapt-victims-device-os) | 28.0 | 20.0 | 42.0 |
| [Proton、「Lumo 2.0」を発表--プライバシー重視のAIチャットボット](https://japan.zdnet.com/article/35249881/) | 26.0 | 20.0 | 42.0 |
| [現場主導の“AI業務改善”を当たり前に ジョイゾーが初期費用36万の伴走支援サービス](https://ascii.jp/elem/000/004/414/4414999/?rss=) | 26.0 | 20.0 | 42.0 |
| [Googleの「Gemini Spark」がmacOSに対応──Canvaなど外部アプリとの連携も](https://www.itmedia.co.jp/news/articles/2607/02/news058.html) | 26.0 | 20.0 | 42.0 |
| [AIビジネスは水平から垂直へ 「業界特化AI」が主戦場に](https://xtech.nikkei.com/atcl/nxt/mag/nc/18/063000556/063000001/) | 26.0 | 20.0 | 42.0 |
| [Anthropicの営業はAIエージェントをこう使う！ 日本法人メンバーが明かす手の内](https://www.itmedia.co.jp/news/articles/2607/02/news017.html) | 26.0 | 20.0 | 42.0 |
| [Claude Sonnet 5.0、論争を避けて中道を行く](https://www.theregister.com/devops/2026/07/01/claude-sonnet-50-heads-straight-down-the-middle-of-the-road-to-dodge-controversy/5265398) | 25.0 | 20.0 | 42.0 |
| [「macOS Tahoe 26.5.2」公開 - 脆弱性37件を修正](https://www.security-next.com/186684) | 22.0 | 20.0 | 42.0 |
| [「IBM Db2」に深刻な脆弱性 - 暫定的な修正を提供](https://www.security-next.com/186679) | 22.0 | 20.0 | 42.0 |
| [EUが推進するデジタル身分証明システム「デジタルIDウォレット」はGoogleやAppleの独占を強化するとの指摘](https://gigazine.net/news/20260702-european-digital-id-wallets-google-apple/) | 22.0 | 20.0 | 42.0 |
| [AIは新たな「内部脅威」なのか 企業が見直すべきデータ管理の課題](https://news.mynavi.jp/techplus/article/20260702-4646682/) | 21.0 | 20.0 | 42.0 |
| [セキュリティオペレーションを単一のプラットフォームとサービスモデルに統合する「FortiSOC」](https://ascii.jp/elem/000/004/414/4414187/?rss=) | 21.0 | 20.0 | 42.0 |
| [顔写真公開まで 2 週間のカウントダウン：オランダ警察のクラウドソーシング型犯罪者狩りゲーム「Game Over?!」](https://scan.netsecurity.ne.jp/article/2026/07/02/55621.html) | 21.0 | 20.0 | 42.0 |
| [個人情報漏えい等 4,602 件、大半は病院・薬局の「誤交付」～ 個人情報保護委員会、令和 7 年度 4Q 状況を公表](https://scan.netsecurity.ne.jp/article/2026/07/02/55620.html) | 21.0 | 20.0 | 42.0 |
| [メール配信システム「める配くん」の一部サーバに不正アクセス、情報漏えいと考えられる痕跡を確認](https://scan.netsecurity.ne.jp/article/2026/07/02/55619.html) | 21.0 | 20.0 | 42.0 |
| [ダイキョーニシカワのインドネシア連結子会社に不正アクセス、データの一部が外部送信された事実を確認](https://scan.netsecurity.ne.jp/article/2026/07/02/55618.html) | 21.0 | 20.0 | 42.0 |
| [「女の転職 type」にリスト型アカウントハッキング、フォレンジック調査と社内調査に内容の相違なし](https://scan.netsecurity.ne.jp/article/2026/07/02/55617.html) | 21.0 | 20.0 | 42.0 |
| [7 / 2 ～ 4 開催「Hardening Designers Conference 2026」にGMOサイバーセキュリティ byイエラエの熊坂駿吾氏が登壇](https://scan.netsecurity.ne.jp/article/2026/07/02/55616.html) | 21.0 | 20.0 | 42.0 |
| [RPGツクールMV および MZ に OSコマンドインジェクションの脆弱性](https://scan.netsecurity.ne.jp/article/2026/07/02/55615.html) | 21.0 | 20.0 | 42.0 |
| [DGM3103SCT に OSコマンドインジェクションの脆弱性](https://scan.netsecurity.ne.jp/article/2026/07/02/55614.html) | 21.0 | 20.0 | 42.0 |
| [前橋工科大学の長野寿城氏がパケット分類アルゴリズムの性能評価に関する研究で優秀研究賞を受賞](https://scan.netsecurity.ne.jp/article/2026/07/02/55613.html) | 21.0 | 20.0 | 42.0 |
| [日本の上場企業Webサイトの70.1%がサポート終了済PHPで稼働](https://scan.netsecurity.ne.jp/article/2026/07/02/55612.html) | 21.0 | 20.0 | 42.0 |
| [その製品、本当に"国産"？ セキュリティ製品を評価する新指標「日本度」が始動](https://atmarkit.itmedia.co.jp/ait/articles/2607/02/news040.html) | 21.0 | 20.0 | 42.0 |
| [「いつか」ではなく「いつ起きるか」--サイバーインシデントが事業継続を揺るがす時代のリスク実態](https://japan.zdnet.com/article/35249788/) | 21.0 | 20.0 | 42.0 |
| [ダークウェブ分析の韓国S2Wが日本法人設立、今日本で事業注力する理由](https://www.itmedia.co.jp/enterprise/articles/2607/01/news038.html) | 21.0 | 20.0 | 42.0 |
| [NISTのCVSSは本当に正しい？ 「全件分析断念」2カ月後に見えた意外な実態](https://atmarkit.itmedia.co.jp/ait/articles/2607/02/news037.html) | 21.0 | 20.0 | 42.0 |
| [社内Wi-Fiの認証にSIMが使える！ フルMVNO基盤を抱えるミソラコネクトならではの新提案](https://ascii.jp/elem/000/004/414/4414824/?rss=) | 21.0 | 20.0 | 42.0 |
| [謎解きゲームでサイバーセキュリティを学ぶ「CYBER ADVENTURE 2026」、7月5日に天空橋で開催〜日本青年会議所](https://internet.watch.impress.co.jp/docs/news/2121666.html) | 20.0 | 20.0 | 42.0 |
| [Smashing Security podcast #474: Polymarketは未来を予測できるのに、なぜこのハッキングを見逃したのか？](https://grahamcluley.com/smashing-security-podcast-474/) | 20.0 | 20.0 | 42.0 |
| [EvilTokensのdevice-codeフィッシングキットは想像以上に悪質だった](https://www.theregister.com/cyber-crime/2026/07/01/eviltokens-device-code-phishing-kit-totally-more-evil-than-we-all-thought/5265409) | 20.0 | 20.0 | 42.0 |
| [バッファロー、8ポート全てが10GbE対応の法人向けL2スマートスイッチ2機種を発売 セキュリティ評価制度「JC-STAR」★1に適合](https://internet.watch.impress.co.jp/docs/news/2121632.html) | 20.0 | 20.0 | 42.0 |
| [Kubota、ハッカーによるネットワークシステムへの1か月間の不正アクセスを公表](https://www.bleepingcomputer.com/news/security/kubota-says-hackers-had-month-long-access-to-network-systems/) | 20.0 | 20.0 | 42.0 |
| [Scattered Spiderのハッキング事件に関与した10代の容疑者が米国へ送還される](https://therecord.media/teen-suspect-in-scattered-spider-hacks-extradited-to-us) | 20.0 | 20.0 | 42.0 |
| [偽のPerplexity Chrome拡張機能が検索内容を監視する](https://www.malwarebytes.com/blog/privacy/2026/07/fake-perplexity-chrome-extension-spies-on-your-searches) | 20.0 | 20.0 | 42.0 |

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
