# 📡 サイレーダー 2026-10-15 05:00 JST

このレポートは、2026-10-14 17:00 JST〜2026-10-15 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 114
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 2
- [低温だが記録しておくトピック](#low-record-topics): 77

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [From One Account to Every Mailbox: Breaking Zimbra's Identity Boundaries (Part 1)](#topic-37542) | 56.0 | 74.0 | 52.0 | 音声 | 温度感上位枠 |
| 2 | [Ivanti patches Connect Secure zero-day after researchers confirm in-the-wild attacks](#topic-37222) | 55.0 | 64.0 | 63.0 | 音声 | 温度感上位枠 |
| 3 | [Microsoft 2026年10月 Patch Tuesday 関連まとめ](#topic-36757) | 50.0 | 56.0 | 58.0 | GitHub | audio_eligible_by_public_rules_false |
| 4 | [Microsoft drops an actively exploited zero-day among record high of 1,413 vulnerabilities](#topic-37349) | 43.0 | 46.0 | 59.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 5 | [EGセキュアソリューションズのホスト型WAF「SiteGuard Server Edition」に脆弱性、最新バージョンに更新を 当該の脆弱性はすでに悪用を確認](#topic-37429) | 42.0 | 64.0 | 55.0 | 音声 | 温度感上位枠 |
| 6 | [Cisco patches new Secure Email Gateway zero-day exploited in attacks](#topic-37483) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 7 | [CISA Urges Immediate Ivanti Connect Secure Updates as Honeypots Log 105 Exploit Attempts](#topic-37547) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 8 | [Fake AI Tools Put US Companies at Risk: Inside Counterfeit Claude, ChatGPT, and Copilot](#topic-37585) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 9 | [FBI raids 40+ laptop farms helping North Korea pocket US tech salaries](#topic-37536) | 30.0 | 20.0 | 48.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-37542"></a>

### 1. From One Account to Every Mailbox: Breaking Zimbra's Identity Boundaries (Part 1)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>R⁠C⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 56.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 52.0 |

#### 概要

Zimbra Collaboration Suite（ZCS）で、認証関連の不備によりGraphQL経由のログイン試行が失敗回数の制限に反映されない問題が報告されています。
あわせて、同じ調査ではメールのなりすまし、他ユーザーのメールボックス閲覧、フィルタによる外部転送の制限回避など、アカウント境界に関わる複数の脆弱性も確認されています。
メールサーバーは社内外の信頼の起点になりやすく、認証や権限の不備はメール本文、添付ファイル、カレンダー情報など広い範囲の漏えいにつながる可能性があります。
特に公開PoCが言及されているため、弱いパスワードの試行や設定不備を前提にしたリスク評価が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- XSS系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ZCSの公開GraphQL/EWS/フィルタ設定が意図どおり制御されているか確認し、可能なら最新の修正版へ更新する。
- 外部LDAP連携やメール転送制限を使っている場合は、関連するアカウントポリシーと保存済みフィルタルールを点検する。
- 不審な認証失敗の増加、複数候補を含むGraphQLリクエスト、見覚えのない送信済みメールやフィルタ変更の痕跡を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Zimbra | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-93637](https://nvd.nist.gov/vuln/detail/CVE-2026-93637) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [From One Account to Every Mailbox: Breaking Zimbra's Identity Boundaries (Part 1](https://www.rapid7.com/blog/post/ve-breaking-zimbra-identity-boundaries-part-1) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-37222"></a>

### 2. Ivanti patches Connect Secure zero-day after researchers confirm in-the-wild attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>Exploit Kit</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 55.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Ivanti Connect Secureに影響するCVE-2026-104935について、実際の攻撃で悪用されていたことが複数の情報源で確認され、Ivantiが修正を公開しました。
報告では、未認証での遠隔操作につながる可能性がある重大な脆弱性として扱われています。
VPN製品は社内ネットワークの入口になりやすく、悪用されると広範な侵害につながるおそれがあります。ゼロデイとして実際に使われていた点から、早急な対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Ivanti Connect Secureの該当バージョンと適用状況を確認し、ベンダーの修正情報に沿って更新する。
- VPN装置の認証失敗、想定外の管理操作、設定変更などのログを重点的に点検する。
- 関連インシデントの可能性を踏まえ、周辺の認証基盤や内部サーバーにも異常がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-104935 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Ivanti | 言及あり | 0.80 | — |
| 製品 | Ivanti Connect Secure | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| ベンダー | watchTowr | 言及あり | 0.80 | — |
| 製品 | Active Directory | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-104935](https://nvd.nist.gov/vuln/detail/CVE-2026-104935) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Ivanti patches Connect Secure zero-day after researchers confirm in-the-wild att](https://www.theregister.com/security/2026/10/14/ivanti-patches-connect-secure-zero-day-after-researchers-confirm-in-the-wild-attacks/5303095) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Ivanti misses opportunity to fix vulnerability before attackers got to work and ](https://cyberscoop.com/ivanti-connect-secure-zero-day-actively-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Ivanti Zero-Day Chain Gave Attackers Root Access to Fully Patched VPN](https://www.securityweek.com/ivanti-zero-day-chain-gave-attackers-root-access-to-fully-patched-vpn/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Ivanti Connect Secure zero-day exploited in the wild (CVE-2026-104935)](https://www.rapid7.com/blog/post/etr-ivanti-connect-secure-zero-day-exploited-in-the-wild-cve-2026-104935) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers chained three Ivanti zero-days to gain root on fully patched VPN appli](https://www.helpnetsecurity.com/2026/10/14/ivanti-zero-days-gain-root-patched-vpn-appliances/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA warns admins to immediately fix Ivanti flaw exploited as zero-day](https://www.bleepingcomputer.com/news/security/cisa-warns-admins-to-immediately-fix-ivanti-flaw-exploited-as-zero-day/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-37429"></a>

### 3. EGセキュアソリューションズのホスト型WAF「SiteGuard Server Edition」に脆弱性、最新バージョンに更新を 当該の脆弱性はすでに悪用を確認

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 42.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

EGセキュアソリューションズのホスト型WAF「SiteGuard Server Edition」に、OSコマンドインジェクションの脆弱性（CVE-2026-106931）が確認されたとされています。
公開情報では、すでに悪用が確認されており、同社や関係機関が最新バージョンへの更新を含む対応を呼びかけています。
WAFはWeb防御の要となるため、そこに深刻な脆弱性があると保護対象の広い範囲に影響し得ます。
悪用が確認されている点から、単なる注意喚起ではなく、早急な対処が必要な案件として注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 対象製品の利用有無とバージョンを確認し、案内されている最新版へ速やかに更新する。
- 更新までの間は、関連する管理画面や運用経路へのアクセス制御を見直し、不要な公開を避ける。
- 更新後もログを確認し、不審な操作や想定外のコマンド実行の痕跡がないか点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-106931 | 関連CVE | 1.00 | 未確認 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-106931](https://nvd.nist.gov/vuln/detail/CVE-2026-106931) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [EGセキュアソリューションズのホスト型WAF「SiteGuard Server Edition」に脆弱性、最新バージョンに更新を　当該の脆弱性はすでに悪用を確認](https://internet.watch.impress.co.jp/docs/news/2148151.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: SiteGuard Server EditionにおけるOSコマンドインジェクションの脆弱性（CVE-2026-106931）に関する注意喚起  (](https://www.jpcert.or.jp/at/2026/at260032.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（2件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-37483"></a>

### 4. Cisco patches new Secure Email Gateway zero-day exploited in attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CiscoのSecure Email Gateway（SEG）において、攻撃で悪用されたとされるゼロデイ脆弱性が修正されたとされています。
公開情報では、遠隔の未認証攻撃者が高権限のコマンド実行につながる可能性が示されており、管理対象環境での対応状況確認が重要です。
メールゲートウェイは組織の対外通信の入口に当たるため、影響がある場合は広範囲に及ぶおそれがあります。
ゼロデイかつ悪用観測ありとされる点から、通常の定期更新よりも優先度を上げて確認すべき話題です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Ciscoの修正内容と影響範囲を確認し、該当SEGのバージョンを速やかに点検する。
- 公開済みの緩和策やベンダー案内があれば適用し、管理インターフェースや関連ログを監視する。
- 侵害の兆候がないか、メール配送の異常や不審な設定変更の有無を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-76519 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Cisco patches new Secure Email Gateway zero-day exploited in attacks](https://www.bleepingcomputer.com/news/security/cisco-patches-actively-exploited-secure-email-gateway-zero-day/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Email Gateway Arbitrary File Write Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-esa-afw-zqYJkjxp) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-37547"></a>

### 5. CISA Urges Immediate Ivanti Connect Secure Updates as Honeypots Log 105 Exploit Attempts

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、Ivanti Connect Secureの脆弱性に対して、最新版への速やかな更新を組織に呼びかけました。
対象の不具合は認証バイパスに関係するとされ、公開情報では悪用が観測されていると報告されています。
境界装置は組織の外部公開面に置かれることが多く、悪用が確認された脆弱性は侵入の起点になりやすいため注意が必要です。
CISAが迅速な更新を求めている点からも、優先度の高い対応対象と考えられます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Ivanti Connect Secureの該当版を利用していないか確認し、ベンダーの最新修正版への更新を優先する。
- 更新までの間は、公開範囲や管理アクセス経路を見直し、不要な露出を減らす。
- 対象機器の認証失敗や不審なアクセスの有無を確認し、ログ監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Ivanti | 言及あり | 0.80 | — |
| 製品 | Ivanti Connect Secure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA Urges Immediate Ivanti Connect Secure Updates as Honeypots Log 105 Exploit ](https://thehackernews.com/2026/10/cisa-urges-immediate-ivanti-connect.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-37585"></a>

### 6. Fake AI Tools Put US Companies at Risk: Inside Counterfeit Claude, ChatGPT, and Copilot

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

ANY.RUNの分析によると、Claude、ChatGPT、GitHub Copilot、Geminiなどの生成AIブランドを装う偽ツールを使ったキャンペーンが確認されています。
これらは情報窃取型マルウェアの配布やブラウザセッションの乗っ取り、業務アカウントへのフィッシングに悪用されているとされています。
生成AIの利用拡大に便乗したなりすましは、従業員の警戒をすり抜けやすく、企業アカウントや端末への被害につながるおそれがあります。
正規サービスに見せかけた配布経路が使われるため、利用者教育と検知の両面で注意が必要です。

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

- 公式配布元以外から入手したAI関連ツールや拡張機能を安易に実行しない運用を徹底する。
- ブラウザセッションの不審な挙動や、業務アカウントへの不自然な認証要求を重点的に監視する。
- 情報窃取型マルウェア対策として、EDRや多要素認証、アカウント保護設定を見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Cloudflare | 言及あり | 0.80 | — |
| ベンダー | Anthropic | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | DeepSeek | 言及あり | 0.80 | — |
| ベンダー | GitLab | 言及あり | 0.80 | — |
| ベンダー | Google | 言及あり | 0.80 | — |
| ベンダー | OpenAI | 言及あり | 0.80 | — |
| ベンダー | Meta | 言及あり | 0.80 | — |
| 製品 | Apple macOS | 言及あり | 0.80 | — |
| 製品 | Ivanti Policy Secure | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Fake AI Tools Put US Companies at Risk: Inside Counterfeit Claude, ChatGPT, and ](https://any.run/cybersecurity-blog/fake-ai-tools-us-companies/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-37536"></a>

### 7. FBI raids 40+ laptop farms helping North Korea pocket US tech salaries

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>国⁠家⁠支⁠援</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 48.0 |

#### 概要

米司法省の発表を受け、北朝鮮関連とされるIT労働者が米国企業のリモート雇用を得るために、盗用・偽造された身元情報を使っていたと報じられています。
あわせて、米国内で会社支給のノートPCを稼働させ続ける「ラップトップファーム」に関与したとされる人物への家宅捜索や逮捕が行われました。
遠隔採用や端末持ち出しを悪用したなりすましは、企業の境界防御だけでは見抜きにくく、本人確認と端末管理の重要性を改めて示します。
対象企業は、雇用・委託・資産管理の各プロセスが連携しているか確認する必要があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 採用時の本人確認、経歴確認、口座・住所・連絡先の整合性を再点検する。
- 会社支給端末の所在監視、遠隔操作・常時稼働の不自然なパターン検知を強化する。
- 委託先やリモート人材を含め、アクセス権限の最小化と定期的な再確認を行う。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [FBI raids 40+ laptop farms helping North Korea pocket US tech salaries](https://www.helpnetsecurity.com/2026/10/14/north-korean-it-workers-laptop-farms-arrests/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-36757"></a>

### 1. Microsoft 2026年10月 Patch Tuesday 関連まとめ

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>脅⁠威⁠レ⁠ポ⁠ー⁠ト</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 50.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 58.0 |

#### 概要

Microsoftの2026年10月のPatch Tuesdayでは、1,400件超の脆弱性修正が行われたとされ、過去最大級の規模として注目されています。
公開材料では、少なくとも一部に悪用観測がある脆弱性やゼロデイ文脈が含まれる一方、影響の中心は通常どおりWindowsやOffice関連の修正にあります。
大量の修正が一度に出るため、組織側では優先度付けを誤ると、重要な脆弱性の見落としにつながりやすい状況です。
とくに悪用観測がある項目は、公開後の適用遅れがリスクになりやすいため注意が必要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 7 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 悪用観測が示されている項目を最優先で確認し、対象製品の適用状況を早めに点検する。
- WindowsとOfficeを含む広範な修正のため、通常月よりも資産台帳ベースで影響範囲の洗い出しを丁寧に行う。
- 検知・監視ルールは、既知の悪用兆候や関連する挙動に対して更新漏れがないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Ivanti | 言及あり | 0.80 | — |
| ベンダー | Rapid7 | 言及あり | 0.80 | — |
| 製品 | Microsoft Defender | 言及あり | 0.80 | — |
| 製品 | Microsoft Exchange Server | 言及あり | 0.80 | — |
| 製品 | Microsoft Windows | 言及あり | 0.80 | — |
| 製品 | Chromium | 言及あり | 0.80 | — |
| 製品 | Exchange | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [CISA warns of new Ivanti bug being exploited as latest Patch Tuesday breaks reco](https://therecord.media/new-ivanti-microsoft-bugs-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Update Windows: Record Patch Tuesday fixes flaw already under attack](https://www.malwarebytes.com/blog/bugs/2026/10/update-windows-record-patch-tuesday-fixes-flaw-already-under-attack) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Breaks Patch Tuesday Record Again with 1400+ CVEs](https://www.infosecurity-magazine.com/news/microsoft-patch-tuesday-record-1/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Zero-Days Lurk in Microsoft's Overgrown October Patch Tuesday](https://www.darkreading.com/vulnerabilities-threats/zero-days-microsoft-october-patch-tuesday) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Patch Tuesday - October 2026](https://www.rapid7.com/blog/post/em-patch-tuesday-october-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patch Tuesday for October 2026 — Snort rules and prominent vulnerabili](https://blog.talosintelligence.com/microsoft-patch-tuesday-for-october-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [October 2026 Patch Tuesday forecast: Time for an Office cleanup](https://www.helpnetsecurity.com/2026/10/09/october-2026-patch-tuesday-forecast/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-37349"></a>

### 2. Microsoft drops an actively exploited zero-day among record high of 1,413 vulnerabilities

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 43.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

Microsoftは、Windowsや関連ソフトウェア向けに1,400件超の脆弱性修正を公開しました。
報道によると、その中には実際に悪用が確認されたWindowsのゼロデイ脆弱性CVE-2026-96951も含まれています。
修正件数が非常に多く、通常月を大きく上回る規模であるため、運用現場では優先順位付けが重要になります。
加えて、既に悪用が観測されている脆弱性が含まれるため、影響範囲の確認と迅速な適用が求められます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- WindowsおよびMicrosoft製品の更新適用状況を早急に確認し、優先度を上げて対応する。
- CVE-2026-96951の影響有無を資産管理情報と照合し、該当環境を重点的に監視する。
- 大規模パッチ適用に伴う業務影響を見込み、検証後の段階的展開とロールバック手順を確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-96951 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | Tenable | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-96951](https://nvd.nist.gov/vuln/detail/CVE-2026-96951) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Microsoft drops an actively exploited zero-day among record high of 1,413 vulner](https://cyberscoop.com/microsoft-patch-tuesday-october-2026/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches Record 1,413 Vulnerabilities, Including Exploited Windows Zero](https://www.securityweek.com/microsoft-patches-record-1413-vulnerabilities-including-exploited-windows-zero-day/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Patches More Than 1,400 Security Flaws](https://krebsonsecurity.com/2026/10/microsoft-patches-more-than-1400-security-flaws/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Channel Software WebAlliance eCommerceの認証不要SQLインジェクション脆弱性](https://www.rapid7.com/blog/post/ve-unauthenticated-sql-injection-in-channel-software-weballiance-ecommerce) | 29.0 | 49.0 | 51.0 |
| [2027年に向けた製造業サイバーセキュリティの7つの重要トレンド](https://www.huntress.com/blog/manufacturing-cybersecurity-trends) | 28.0 | 30.0 | 42.0 |
| [英国、暗号資産サービスのCryptomusをロシア資金洗浄で制裁](https://krebsonsecurity.com/2026/10/u-k-sanctions-cryptomus-for-ru-money-laundering/) | 28.0 | 30.0 | 42.0 |
| [「IDCFクラウド」への不正アクセスについて調査の進捗を公開、外部へのデータ流出を裏付ける事実は確認されず 一部利用者のバックアップ取り出しも可能だと判明](https://internet.watch.impress.co.jp/docs/news/2148166.html) | 28.0 | 30.0 | 42.0 |
| [FBI、テキサス州の北朝鮮IT労働者向けラップトップファームを摘発　米国人も逮捕](https://www.bleepingcomputer.com/news/security/fbi-raids-dprk-it-worker-laptop-farms-in-texas-us-nationals-arrested/) | 28.0 | 20.0 | 48.0 |
| [Ciscoが警告する新たな深刻なSecure Email Gateway脆弱性を悪用した活発な攻撃](https://thehackernews.com/2026/10/cisco-warns-of-active-attacks.html) | 28.0 | 20.0 | 42.0 |
| [Microsoftが10億件超の詐欺メッセージに関与する3つのフィッシングキットを無効化](https://thehackernews.com/2026/10/microsoft-disrupts-3-phishing-kits.html) | 28.0 | 20.0 | 42.0 |
| [米国、北朝鮮IT労働者詐欺に関連する40以上のラップトップファームを閉鎖し14人を起訴](https://thehackernews.com/2026/10/us-shuts-down-over-40-laptop-farms.html) | 28.0 | 20.0 | 42.0 |
| [北朝鮮系IT労働者スキームへの新たな家宅捜索・起訴・逮捕を米当局が取り締まり強化](https://www.cybersecuritydive.com/news/north-korea-it-worker-raids-arrests-charges/832968/) | 28.0 | 20.0 | 42.0 |
| [ROMULUSマルウェアサーバーがClickFixを悪用して複数のペイロードを配布](https://www.infosecurity-magazine.com/news/romulus-malware-clickfix-deliver/) | 28.0 | 20.0 | 42.0 |
| [Hirudo Androidマルウェアが銀行アプリを置き換えてセキュリティチェックを回避](https://www.bleepingcomputer.com/news/security/hirudo-android-malware-replaces-banking-apps-to-evade-security-checks/) | 28.0 | 20.0 | 42.0 |
| [米国、北朝鮮IT労働者のラップトップ農場摘発で2人を逮捕](https://www.securityweek.com/us-arrests-two-in-crackdown-on-north-korean-it-worker-laptop-farms/) | 28.0 | 20.0 | 42.0 |
| [米国、北朝鮮への300万ドル送金に使われたノートPC工場を摘発した偽候補者詐欺](https://www.itpro.com/security/us-raids-laptop-farms-used-to-funnel-usd3-million-to-north-korea-in-fake-candidate-scam) | 28.0 | 20.0 | 42.0 |
| [Google、待望の新AIモデル「Gemini 4 Argon」一般提供を開始 推論の継続力を強化 一部ベンチでトップに](https://www.itmedia.co.jp/news/article/2610/14/2000002265/) | 26.0 | 20.0 | 42.0 |
| [デジハリ大、「Claude」を全学導入へ──国内初、“回数気にせず”使い放題に](https://www.itmedia.co.jp/news/article/2610/14/2000002278/) | 26.0 | 20.0 | 42.0 |
| [AIワームがスマートデバイス全体に拡散する可能性、Anthropicが警告](https://www.malwarebytes.com/blog/ai/2026/10/ai-worms-could-spread-across-your-smart-devices-anthropic-warns) | 25.0 | 20.0 | 42.0 |
| [2026年10月21日公開予定のCiscoセキュリティアドバイザリ事前通知](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-notice-QGwHnJ6k) | 25.0 | 20.0 | 42.0 |
| [AI Agentsが未知のOTシステムを短時間で操作し機器を移動、Booz Allenが確認](https://www.securityweek.com/ai-agents-navigate-unfamiliar-ot-systems-and-move-equipment-in-minutes-booz-allen-finds/) | 25.0 | 20.0 | 42.0 |
| [2027年に向けた10のエンドポイントセキュリティ動向と対策のヒント](https://www.huntress.com/blog/endpoint-security-trends) | 25.0 | 20.0 | 42.0 |
| [Texas HB 3834におけるサイバーセキュリティとAI研修要件](https://www.huntress.com/blog/texas-hb-3834-cyber-security-awareness-training-requirements) | 25.0 | 20.0 | 42.0 |
| [上院議員らがトランプ政権にAIの安全性とセキュリティを巡る連邦政府の連携強化を要請](https://cyberscoop.com/congress-presses-trump-administration-ai-safety-cybersecurity/) | 25.0 | 20.0 | 42.0 |
| [Harmonic Security、ワークフォース向けAI保護で5000万ドルを調達](https://www.securityweek.com/harmonic-security-raises-50-million-for-workforce-ai-protection/) | 25.0 | 20.0 | 42.0 |
| [Agentic Pentestingの盲点とその解消策](https://www.bleepingcomputer.com/news/security/the-blind-spots-of-agentic-pentesting-and-how-to-close-them/) | 25.0 | 20.0 | 42.0 |
| [公開OpenAIモデルを使って6日で25万ドル規模のChromeフルチェーン攻撃コードを構築](https://thehackernews.com/2026/10/researchers-used-public-openai-model-to.html) | 25.0 | 20.0 | 42.0 |
| [Wiz for GovにWiz AI Agentsが登場、ミッションを機械速度で保護](https://www.wiz.io/blog/wiz-for-gov-agents-fedramp) | 25.0 | 20.0 | 42.0 |
| [AIエージェントが本番環境で重大なOTPバイパスを発見、攻撃はむしろ容易だった](https://thehackernews.com/2026/10/an-ai-agent-found-critical-otp-bypass.html) | 25.0 | 20.0 | 42.0 |
| [AIエージェントは自律的に動き、それが企業にとって問題になる](https://www.itpro.com/security/ai-agents-have-a-mind-of-their-own-and-thats-a-problem-for-businesses) | 25.0 | 20.0 | 42.0 |
| [AnthropicのClaude AIが偽の殺人通報を生成、警察が受理](https://www.malwarebytes.com/blog/ai/2026/10/police-receive-fake-murder-tip-from-anthropics-claude-ai) | 25.0 | 20.0 | 42.0 |
| [Radware MCP Server Protectionがエージェントの活動を監視し、プロトコル悪用を防止する仕組み](https://www.helpnetsecurity.com/2026/10/14/radware-mcp-server-protection/) | 25.0 | 20.0 | 42.0 |
| [SolarWinds Avior、IT自動化と人による承認・監査証跡を両立](https://www.helpnetsecurity.com/2026/10/14/solarwinds-avior/) | 25.0 | 20.0 | 42.0 |
| [Chainguard HarnessがフロンティアAIを活用して稼働中アプリケーションの脆弱性を検証](https://www.helpnetsecurity.com/2026/10/14/chainguard-harness/) | 25.0 | 20.0 | 42.0 |
| [OpenAIのエンジニア、役員会議室で発見されたトイレットペーパーに包まれた盗聴器で起訴](https://www.theregister.com/security/2026/10/14/openai-engineer-charged-after-boardroom-bug-found-wrapped-in-toilet-paper/5303000) | 25.0 | 20.0 | 42.0 |
| [GitHubがコード内に残された機密情報を検出するために低コストのAIモデルを採用](https://www.helpnetsecurity.com/2026/10/14/github-secret-detection-model/) | 25.0 | 20.0 | 42.0 |
| [OpenAIエンジニア、幹部会議を盗聴しようとした疑いで逮捕](https://www.helpnetsecurity.com/2026/10/14/openai-engineer-arrested-hidden-recording-device/) | 25.0 | 20.0 | 42.0 |
| [CVE-2026-0322 PAN-OS 管理インターフェースにおける認証済みリモートコード実行の脆弱性](https://security.paloaltonetworks.com/CVE-2026-0322) | 24.0 | 46.0 | 50.0 |
| [CVE-2026-0313 Cortex XSOARのOSコマンドインジェクション脆弱性（重要度：中）](https://security.paloaltonetworks.com/CVE-2026-0313) | 24.0 | 46.0 | 50.0 |
| [CVE-2026-0320 PAN-OSの認証済み管理者向けコマンドインジェクション脆弱性（重要度：中）](https://security.paloaltonetworks.com/CVE-2026-0320) | 24.0 | 46.0 | 50.0 |
| [情報漏洩の裏に「A2B攻撃」、スマホアプリの接続先サーバーに不正アクセス](https://xtech.nikkei.com/atcl/nxt/column/18/03790/101400005/) | 24.0 | 20.0 | 43.0 |
| [CVE-2026-0315 GlobalProtect AppのmacOSにおけるローカル権限昇格の脆弱性（深刻度: MEDIUM）](https://security.paloaltonetworks.com/CVE-2026-0315) | 22.0 | 40.0 | 50.0 |
| [フィッシング基盤エコシステムの裏側：世界的サイバー犯罪を支える隠れたネットワーク](https://www.microsoft.com/en-us/security/blog/2026/10/14/the-hidden-network-inside-the-phishing-infrastructure-ecosystem-powering-global-cybercrime/) | 22.0 | 20.0 | 48.0 |
| [JPAAWG 9th General Meeting、11月に都内でハイブリッド開催](https://www.security-next.com/191446) | 22.0 | 20.0 | 42.0 |
| [データ移行に用いた記憶媒体を紛失、内容を調査 - 商船三井クルーズ](https://www.security-next.com/191197) | 22.0 | 20.0 | 42.0 |
| [curl、HTTP/2アップロードの脆弱性を修正　PoCでクライアント側コード実行を実証](https://thehackernews.com/2026/10/curl-patches-http2-upload-flaw-after.html) | 22.0 | 20.0 | 42.0 |
| [「EC-CUBE」の公式決済プラグインに緊急脆弱性 - すでに悪用も](https://www.security-next.com/191457) | 22.0 | 20.0 | 42.0 |
| [CVE-2026-0316 PAN-OSの保存型クロスサイトスクリプティング（XSS）脆弱性（深刻度：低）](https://security.paloaltonetworks.com/CVE-2026-0316) | 21.0 | 34.0 | 50.0 |
| [サイバーリーズン、2027年に「LevelBlue」へ統一--「EDRから撤退するわけではない」](https://japan.zdnet.com/article/35253540/) | 21.0 | 20.0 | 42.0 |
| [CVE-2026-0319 PAN-OSの不適切な入力処理の脆弱性](https://security.paloaltonetworks.com/CVE-2026-0319) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0314 GlobalProtect AppのWindowsにおけるローカルDoS脆弱性](https://security.paloaltonetworks.com/CVE-2026-0314) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0321 PAN-OSのネットワークサービスにおけるサービス妨害（DoS）脆弱性（深刻度：MEDIUM）](https://security.paloaltonetworks.com/CVE-2026-0321) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0312 Checkov by Prisma Cloudのパストラバーサル脆弱性（重要度: MEDIUM）](https://security.paloaltonetworks.com/CVE-2026-0312) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0318 PAN-OS: Panoramaにおけるサービス拒否（DoS）脆弱性](https://security.paloaltonetworks.com/CVE-2026-0318) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-0311: Prisma CloudのCheckovにおけるサーバーサイドリクエストフォージェリの脆弱性（重要度：低）](https://security.paloaltonetworks.com/CVE-2026-0311) | 20.0 | 28.0 | 50.0 |
| [Ledger、サプライチェーン攻撃後にアジア全域の販売業者へ販売停止を要請](https://www.bleepingcomputer.com/news/security/ledger-asks-sellers-across-asia-to-halt-sales-after-supply-chain-attack/) | 20.0 | 20.0 | 42.0 |
| [HackersがCollaboraの組み込みCODEアプリの重大な脆弱性を悪用してNextcloudサーバーにバックドアを設置](https://thehackernews.com/2026/10/hackers-backdoor-nextcloud-servers.html) | 20.0 | 20.0 | 42.0 |
| [Passkeyが普及しても攻撃者が侵入できるポイント](https://www.huntress.com/blog/passkeys-raise-the-bar-but-attackers-can-still-get-in) | 20.0 | 20.0 | 42.0 |
| [Business Email Compromise（BEC）攻撃を防ぐ方法](https://www.huntress.com/blog/what-is-business-email-compromise-bec) | 20.0 | 20.0 | 42.0 |
| [Chromiumの月例脆弱性アップデート（2026年10月、重要度：HIGH）](https://security.paloaltonetworks.com/PAN-SA-2026-0013) | 20.0 | 20.0 | 42.0 |
| [ICS向けPatch Tuesday：Siemensが17件のアドバイザリを公開、RockwellがArmorBlockの乗っ取り脆弱性を修正](https://www.securityweek.com/ics-patch-tuesday-siemens-issues-17-advisories-rockwell-fixes-armorblock-takeover-flaw/) | 20.0 | 20.0 | 42.0 |
| [HackerがIvanti Connect Secureを連鎖的な攻撃で標的にする](https://www.cybersecuritydive.com/news/hacker-ivanti-connect-secure-chained-exploitation/832983/) | 20.0 | 20.0 | 42.0 |
| [Ahold Delhaize USAのバナーサイトが引き続きオフラインに](https://www.cybersecuritydive.com/news/ahold-delhaize-usa-sites-still-down/832972/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、Health-ISAC、パートナーが人気のフィッシングキットサービスを停止](https://www.cybersecuritydive.com/news/phishing-marketplace-takedown-microsoft-health-isac/832965/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、9月のWindows更新で発生したVPN問題を修正](https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-vpn-issues-caused-by-september-windows-updates/) | 20.0 | 20.0 | 42.0 |
| [Microsoft、中国系サイバー犯罪者が利用した主要フィッシング基盤3件を停止](https://therecord.media/microsoft-takes-down-3-major-chinese-phishing-platforms) | 20.0 | 20.0 | 42.0 |
| [10億件のフィッシングメッセージを送信したネットワークを一斉摘発](https://www.bleepingcomputer.com/news/security/global-takedown-hits-network-behind-1-billion-phishing-messages/) | 20.0 | 20.0 | 42.0 |
| [Google Chromeの複数の脆弱性により任意コードが実行される可能性](https://www.cisecurity.org/advisory/multiple-vulnerabilities-in-google-chrome-could-allow-for-arbitrary-code-execution_2026-116) | 20.0 | 20.0 | 42.0 |
| [ロシアの旅行予約プラットフォーム、サイバー攻撃後に予約受付を停止](https://therecord.media/russia-anywayanyday-travel-website-cyberattack) | 20.0 | 20.0 | 42.0 |
| [ラテンアメリカを広く標的としたロシアの影響工作](https://www.darkreading.com/cyberattacks-data-breaches/russian-influence-operation-targeting-latin-america) | 20.0 | 20.0 | 42.0 |
| [Microsoftとパートナーが大規模な中国語フィッシングキット・エコシステムを壊滅](https://cyberscoop.com/microsoft-disrupts-chinese-language-phishing-kit-ecosystem/) | 20.0 | 20.0 | 42.0 |
| [Microsoftが1億件超のメッセージを送信した中国語フィッシング市場を妨害](https://www.securityweek.com/microsoft-disrupts-chinese-language-phishing-market-behind-1b-messages/) | 20.0 | 20.0 | 42.0 |
| [クローン音声による架空の通話に備えるディープフェイク対応訓練の実施方法](https://thehackernews.com/2026/10/how-to-run-deepfake-readiness-drill.html) | 20.0 | 20.0 | 42.0 |
| [Fake Calendlyを装った「Meta Careers」ページによるFacebookとGoogleログイン情報の窃取](https://www.malwarebytes.com/blog/threat-intel/2026/10/fake-calendly-meta-careers-pages-steal-facebook-and-google-logins) | 20.0 | 20.0 | 42.0 |
| [Hirudo Androidトロイの木馬、改ざん済み銀行アプリを悪用して内蔵セキュリティチェックを回避](https://thehackernews.com/2026/10/hirudo-android-trojan-uses-patched.html) | 20.0 | 20.0 | 42.0 |
| [Phase EightとHobbs、Whistlesの運営会社がハッカーの標的に、ファッション小売企業への攻撃が拡大](https://www.helpnetsecurity.com/2026/10/14/tfg-london-cyberattack-phase-eight-hobbs-whistles/) | 20.0 | 20.0 | 42.0 |
| [Microsoftの最近のWindows更新プログラムがRemote Desktop障害を引き起こす可能性](https://www.bleepingcomputer.com/news/security/microsoft-recent-windows-updates-may-trigger-remote-desktop-failures/) | 20.0 | 20.0 | 42.0 |
| [Passkey認証は倍増も、普及は依然として鈍い](https://www.infosecurity-magazine.com/news/passkey-authentications-double/) | 20.0 | 20.0 | 42.0 |
| [MITRE ATT&CK T1490における検知のギャップ](https://www.security.com/expert-perspectives/detection-gap-mitre-attck-t1490) | 20.0 | 20.0 | 42.0 |
| [フランスのスーパーマーケットへのサイバー攻撃が冷蔵コントローラに影響](https://www.infosecurity-magazine.com/news/french-supermarket-hack-more/) | 20.0 | 20.0 | 42.0 |

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
