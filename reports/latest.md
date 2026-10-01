# 📡 サイレーダー 2026-10-01 17:00 JST

このレポートは、2026-10-01 11:00 JST〜2026-10-01 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 61
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 31

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Apple CoreGraphics PoC Emerges as WhatsApp PDF Checks Hint at Possible Delivery Path](#topic-34785) | 48.0 | 56.0 | 67.0 | 音声 | 温度感上位枠 |
| 2 | [Bitget Confirms Third-Party Zero-Day Behind $387.5 Million Cryptocurrency Theft](#topic-35360) | 37.0 | 38.0 | 43.0 | 音声 | AI×Security枠 |
| 3 | [Many expect AI in the SOC to make entry jobs harder to get](#topic-35357) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 4 | [Citrix NetScaler Post-Exploitation Payload Creates Superuser, Maps Web Shell to CSS-Like URLs](#topic-35371) | 32.0 | 38.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [ChatGPTの「カスタムGPT」を悪用してマルウェア感染へ誘導する攻撃、正規のChatGPTページを入口に利用](#topic-35350) | 30.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 6 | [ScreenConnect Client (Ab)used by Attackers, (Thu, Oct 1st)](#topic-35356) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-34785"></a>

### 1. Apple CoreGraphics PoC Emerges as WhatsApp PDF Checks Hint at Possible Delivery Path

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>i⁠O⁠S</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 温度上昇中 |
| <nobr>温⁠度⁠感</nobr> | 48.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

AppleのCoreGraphicsに関する脆弱性CVE-2026-86950について、公開PoCの存在が確認され、標的型攻撃で悪用された可能性があるとされています。
関連報道では、細工されたPDFや埋め込みフォントを含むファイルがきっかけになり得るとみられていますが、詳細な悪用経路は未確定です。
すでに実際の攻撃文脈で語られている脆弱性であり、公開PoCによって検証や再現のハードルが下がるため、優先度は高めです。
Apple製端末は利用者が多く、対象が限定的でも影響範囲の見極めと更新対応が重要になります。

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

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Appleの修正版適用状況を確認し、対象OS・対象端末の更新を急ぐ。
- PDFや不審なファイルの取り扱いを見直し、受信経路や閲覧環境の監視を強化する。
- 標的型攻撃の可能性を踏まえ、端末の異常クラッシュや不審なアプリ挙動を確認する。

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
| <nobr>出典</nobr> | [Apple CoreGraphics PoC Emerges as WhatsApp PDF Checks Hint at Possible Delivery ](https://thehackernews.com/2026/10/apple-coregraphics-poc-emerges-as.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Patches CoreGraphics Zero Day Exploited in Attacks](https://www.infosecurity-magazine.com/news/apple-patches-coregraphics-zero/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Zero-Day Vulnerability Weaponized in Targeted Attacks](https://www.darkreading.com/cyberattacks-data-breaches/apple-zero-day-vulnerability-weaponized-targeted-attacks) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple patches CoreGraphics zero-day already exploited in targeted attacks](https://www.theregister.com/security/2026/09/29/apple-patches-coregraphics-zero-day-already-exploited-in-targeted-attacks/5299721) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Update your iPhone, iPad, or Mac: Flaw could run attackers’ code](https://www.malwarebytes.com/blog/bugs/2026/09/update-your-iphone-ipad-or-mac-flaw-could-run-attackers-code) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple squashes zero-day bug exploited in “extremely sophisticated” attack (CVE-2](https://www.helpnetsecurity.com/2026/09/29/apple-core-graphics-zero-day-cve-2026-86950-fixed/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Apple Patches Zero-Day Linked to ‘Extremely Sophisticated Attack’](https://www.securityweek.com/apple-patches-meta-reported-zero-day-linked-to-extremely-sophisticated-attack/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-35360"></a>

### 2. Bitget Confirms Third-Party Zero-Day Behind $387.5 Million Cryptocurrency Theft

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>A⁠I⁠エ⁠ー⁠ジ⁠ェ⁠ン⁠ト</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

暗号資産取引所Bitgetは、約3億8750万ドル相当の資産流出について、第三者製セキュリティ製品のゼロデイ脆弱性が悪用されたと確認しました。
調査は継続中とされており、現時点では第三者製品を起点とした侵害の可能性が示されています。
暗号資産関連の大規模被害であり、単一サービスの問題にとどまらず、周辺で利用する第三者製品のリスクも改めて注目されています。
ゼロデイが関与した可能性があるため、同種製品を使う組織は影響有無の確認を急ぐ必要があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 第三者製セキュリティ製品の利用有無と、ベンダーからの注意喚起・更新情報を確認する。
- 資産管理や認証、運用端末など重要領域で、侵害の兆候がないか監視とログ確認を強化する。
- 関連製品について、既知の不審挙動や未修正の脆弱性がないか、インベントリ単位で点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | Exchange | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Bitget Confirms Third-Party Zero-Day Behind $387.5 Million Cryptocurrency Theft](https://thehackernews.com/2026/10/bitget-confirms-third-party-zero-day.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35357"></a>

### 3. Many expect AI in the SOC to make entry jobs harder to get

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>A⁠I</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

SOCの初級業務では、これまで反復的な調査や記録作業を通じて経験を積むことが一般的でした。
この記事は、AIツールがそうした定型業務を担うことで、SOCのエントリーレベル職の入り口が狭くなるのではないかという見方を紹介しています。
AIの導入は、検知や仕分けなどの効率化を進める一方で、現場の育成や経験の積み方にも影響し得ます。
採用や教育の設計を見直さないと、将来の運用人材の育成に偏りが出る可能性があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 初級者が担当してきた定型業務のどこをAIで置き換え、どこを教育機会として残すか整理する。
- AI導入後も、判断根拠の確認や例外対応を学べる運用フローを設計する。
- 採用要件を見直し、ツール操作だけでなく分析力や説明力を評価する基準を用意する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Many expect AI in the SOC to make entry jobs harder to get](https://www.helpnetsecurity.com/2026/10/01/ai-soc-entry-jobs/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35371"></a>

### 4. Citrix NetScaler Post-Exploitation Payload Creates Superuser, Maps Web Shell to CSS-Like URLs

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 32.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Citrix NetScaler ADC および NetScaler Gateway を狙う攻撃活動が観測され、事後に利用されるペイロードが管理者権限の作成やウェブシェル関連の挙動に関与していた可能性が示されています。
公開情報では、設定情報の窃取を狙う動きも報告されていますが、確認できる範囲の事実として扱う必要があります。
境界装置が侵害されると、認証や通信の起点として使われるため影響範囲が大きくなりやすい点が重要です。設定情報の流出は、追加侵害や横展開の足がかりになり得るため注意が必要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Citrix NetScaler ADC / Gateway の公開状況と、関連するセキュリティ更新の適用状況を確認する。
- 管理者権限の不審な追加や、想定外のウェブシェル痕跡、設定取得に関する異常なアクセスログを点検する。
- 侵害の可能性がある場合は、認証情報の再評価と構成情報の保全・再点検を優先する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler Gateway | 言及あり | 0.80 | — |
| マルウェア | Webshell | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Citrix NetScaler Post-Exploitation Payload Creates Superuser, Maps Web Shell to ](https://thehackernews.com/2026/10/citrix-netscaler-post-exploitation.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-35350"></a>

### 5. ChatGPTの「カスタムGPT」を悪用してマルウェア感染へ誘導する攻撃、正規のChatGPTページを入口に利用

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

セキュリティ企業Huntressが、ChatGPTのカスタムGPTを悪用して、ユーザーをマルウェア感染につながる外部サイトへ誘導する手口を確認したと報告しました。
正規のchatgpt.com上の機能を入口として見せかけるため、利用者が本物のChatGPTだと誤認しやすい点が特徴とされています。
信頼されやすい正規サービスの画面や機能が悪用されるため、単純なドメイン確認だけでは見抜きにくい点が注目されています。
生成AIの利用拡大に伴い、ユーザー誘導型の攻撃が既存のフィッシング対策だけでは十分でないことを示しています。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 実務影響の詳細は限定的ですが、関連する利用環境・配布経路・検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 正規サービス上の機能であっても、外部サイトへの誘導や不自然な指示には注意する。
- 利用者向けに、ブラウザ上の表示や案内文だけでなく、実行前にURLや操作内容を確認するよう周知する。
- 生成AI関連の案内や自動応答に紛れた不審なダウンロード・コマンド実行要求を、検知ルールや教育の対象に含める。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| AIモデル/プロジェクト | ChatGPT | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ChatGPTの「カスタムGPT」を悪用してマルウェア感染へ誘導する攻撃、正規のChatGPTページを入口に利用](https://gigazine.net/news/20261001-custom-gpt-clickfix-rat/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-35356"></a>

### 6. ScreenConnect Client (Ab)used by Attackers, (Thu, Oct 1st)

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 30.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

公開情報では、ConnectWise ScreenConnect のクライアントが攻撃者に悪用されている可能性が取り上げられています。
高度なマルウェアに頼らず、既存の正規ツールを不正利用する手口が注目点です。リモート管理ツールの悪用は、正規通信に紛れて見えにくく、検知や切り分けを難しくすることがあります。
製品そのものの脆弱性が確認されたとは限りませんが、運用上の監視やアクセス制御の重要性を示す話題です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ScreenConnect の利用実態を確認し、許可された端末・アカウント以外の接続がないか点検する。
- リモート管理ツールの管理者権限、認証方式、多要素認証の有無を見直す。
- 通常業務で使う正規ツールの通信・実行ログを収集し、想定外の操作や新規導入の痕跡を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 製品 | ConnectWise ScreenConnect | 言及あり | 0.80 | — |
| 遠隔管理/RMMツール | ScreenConnect Client | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ScreenConnect Client (Ab)used by Attackers, (Thu, Oct 1st)](https://isc.sans.edu/diary/rss/33388) | <nobr>内容確認・補足情報</nobr> |

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
| [Amazonの配達員向けスマートグラスは生成AIマッピング用に配送先の私有地でも静止画を撮影、2027年までに2万人以上の配達員が着用へ](https://gigazine.net/news/20261001-amazon-smart-glasses-privacy/) | 27.0 | 20.0 | 42.0 |
| [Google、「Gemini 4 Pro」ではなく「Gemini 4 Agron」発表 まずはサイバー防御組織に限定提供、出力上限は100万トークンに](https://www.itmedia.co.jp/news/article/2610/01/2000001912/) | 27.0 | 20.0 | 42.0 |
| [VRAM 32GBの「Intel Arc Pro B70」で「Hermes Agent」のローカルAIを実行、4ビット量子化したQwen3.8-27Bを動かしてみた](https://gigazine.net/news/20261001-hermes-agent-arc-pro-b70/) | 27.0 | 20.0 | 42.0 |
| [米連邦取引委がAI大手の調査開始 AnthropicやOpenAIなど、暴走や悪用の懸念](https://www.itmedia.co.jp/news/article/2610/01/2000001931/) | 26.0 | 20.0 | 42.0 |
| [OpenAI、推論過程を狙った組織的な“蒸留”行為を阻止 「Kimi」開発元の関係者が関与と主張](https://www.itmedia.co.jp/news/article/2610/01/2000001929/) | 26.0 | 20.0 | 42.0 |
| [リコー、Difyアプリを企業間で共有する「RICOH AI App Mall」を提供開始](https://japan.zdnet.com/article/35253152/) | 26.0 | 20.0 | 42.0 |
| [TikTok「広告制作をより速く」 生成AI「Seedance」のビジネス活用進む](https://www.itmedia.co.jp/news/article/2610/01/2000001920/) | 26.0 | 20.0 | 42.0 |
| [BlackFog、エージェント型AI向けにプロンプト保護とガバナンスを追加](https://www.helpnetsecurity.com/2026/10/01/blackfog-adx-vision-2-0/) | 25.0 | 20.0 | 42.0 |
| [AIが見つける脆弱性は攻撃者が狙うもの](https://www.helpnetsecurity.com/2026/10/01/google-ai-discovered-vulnerabilities-remote-code-execution/) | 25.0 | 20.0 | 42.0 |
| [Google、Gemini 4 Argonで重大なソフトウェア脆弱性の発見と修正が可能と発表](https://www.helpnetsecurity.com/2026/10/01/google-gemini-4-argon/) | 25.0 | 20.0 | 42.0 |
| [GoogleのSynthID BioがAI設計タンパク質結合体を損なわずに電子透かしを付与できる話](https://www.helpnetsecurity.com/2026/10/01/synthid-bio-watermark/) | 25.0 | 20.0 | 42.0 |
| [Cisco、10月7日に複数製品のセキュリティアドバイザリを公開予定](https://www.security-next.com/190900) | 22.0 | 20.0 | 42.0 |
| [Insecure Agents Podcast: AIエージェントがセキュリティ制御を回避しないようにする方法](https://socket.dev/blog/insecure-agents-security-controls) | 22.0 | 20.0 | 42.0 |
| [NVIDIA製GPU関連ソフトに脆弱性 - 重要度「クリティカル」も](https://www.security-next.com/190906) | 22.0 | 20.0 | 42.0 |
| [OpenAIが「中国のAI企業が1万5000以上のユーザーを使ってモデルの思考を盗み取る蒸留攻撃を実行していた」と報告](https://gigazine.net/news/20261001-openai-model-distillation-campaign/) | 22.0 | 20.0 | 42.0 |
| [佐川急便、不正アクセスで個人情報流出か 送り主・届け先の氏名や住所など、約100日分の荷物データ対象](https://www.itmedia.co.jp/news/article/2610/01/2000001933/) | 21.0 | 20.0 | 42.0 |
| [中古アニメグッズ「らしんばん」に不正アクセス 口座情報や本人確認書類の番号など漏えいの恐れ](https://www.itmedia.co.jp/news/article/2610/01/2000001927/) | 21.0 | 20.0 | 42.0 |
| [吉野家HD、バイト応募者の個人情報5366件漏えい 元委託先に不正アクセス 契約終了もデータ残存](https://www.itmedia.co.jp/news/article/2610/01/2000001928/) | 21.0 | 20.0 | 42.0 |
| [能動的サイバー防御のカギは「情報」、NECが説くサイバーインテリジェンス](https://news.mynavi.jp/techplus/article/20261001-5056494/) | 21.0 | 20.0 | 42.0 |
| [社内業務のニーズに応じた「企業向けAI」選び](https://ascii.jp/elem/000/004/437/4437503/?rss=) | 21.0 | 20.0 | 42.0 |
| [NTTデータ、地銀13行と脆弱性対応を共同化 - 運用作業時間を約9割削減と試算](https://news.mynavi.jp/techplus/article/20261001-5055845/) | 21.0 | 20.0 | 42.0 |
| [「能動的サイバー防御」きょう開始 警察・自衛隊などが攻撃元サーバを無害化 高市首相も狙いを説明](https://www.itmedia.co.jp/news/article/2610/01/2000001918/) | 21.0 | 20.0 | 42.0 |
| [ソフトクリエイト、SOCサービス「Security FREE」を拡充しCrowdStrike・Cato・Zscalerに対応](https://ascii.jp/elem/000/004/438/4438885/?rss=) | 21.0 | 20.0 | 42.0 |
| [KMユナイテッド、Salesforceの「Agentforce」を導入--人事・労務の問い合わせ対応を効率化](https://japan.zdnet.com/article/35253142/) | 21.0 | 20.0 | 42.0 |
| [Metamaskがインフラに影響するセキュリティインシデントを公表](https://www.bleepingcomputer.com/news/security/metamask-discloses-security-incident-affecting-its-infrastructure/) | 20.0 | 20.0 | 42.0 |
| [MetaMaskのセキュリティインシデントで影響を受けたEthereumバリデータが退出](https://thehackernews.com/2026/10/metamask-security-incident-prompts-exit.html) | 20.0 | 20.0 | 42.0 |
| [21か国の金融機関で雇用詐欺の被害が3倍に増加](https://www.helpnetsecurity.com/2026/10/01/employment-scam-victims-research/) | 20.0 | 20.0 | 42.0 |
| [横浜国立大学、サイバーセキュリティの新拠点「SPIRAL」設立。大学発の国産サイバーインテリジェンス提供](https://internet.watch.impress.co.jp/docs/news/2144807.html) | 20.0 | 20.0 | 42.0 |
| [Proton Driveのエンドツーエンド暗号化クラウドストレージ紹介](https://www.helpnetsecurity.com/2026/10/01/product-showcase-proton-drive/) | 20.0 | 20.0 | 42.0 |
| [OpenSSLにおける脆弱性に対するアップデート（2026年9月29日）](https://jvn.jp/vu/JVNVU93468181/) | 20.0 | 20.0 | 42.0 |
| [佐川急便「お荷物問い合わせサービス」に不正アクセス、一部利用を制限中 ヤマト運輸でも「クロネコ代金後払いサービス」に不正アクセスで停止中](https://internet.watch.impress.co.jp/docs/news/2144755.html) | 20.0 | 20.0 | 42.0 |

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
