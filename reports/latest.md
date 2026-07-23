# 📡 サイレーダー 2026-07-23 17:00 JST

このレポートは、2026-07-23 11:00 JST〜2026-07-23 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 51
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 22

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [2026-009: Critical Vulnerabilities in Microsoft SharePoint](#topic-23476) | 62.0 | 74.0 | 67.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [「SharePoint」「Check Point」の脆弱性悪用で警告 - 米当局](#topic-23931) | 39.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [「使ってはいけないリスト」の生成AI、マルウェア配布に使われるクラウドアプリ](#topic-23936) | 34.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Shadow AI is becoming enterprise security’s biggest blind spot](#topic-23906) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-23931"></a>

### 1. 「SharePoint」「Check Point」の脆弱性悪用で警告 - 米当局

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 39.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

米サイバーセキュリティインフラセキュリティ庁（CISA）が、Microsoft SharePointとCheck Point Software TechnologiesのSmartConsoleに関連する脆弱性について、悪用が確認されているとして注意喚起しました。
公開情報では、これらの脆弱性に関して実際の悪用が懸念されている段階とされています。広く使われる製品に関わるため、影響範囲が大きくなり得ます。
悪用観測がある場合、未対応環境は侵害リスクの上昇につながるため、早期の確認と対応が重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当するSharePointおよびSmartConsoleの利用有無とバージョンを確認し、ベンダーやCISAの案内に沿って修正・緩和策を適用する。
- 外部公開されている管理画面や関連サービスの露出を見直し、不要な公開を避ける。
- 監視ログや認証履歴を点検し、通常と異なるアクセスや操作の痕跡がないか確認する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-16232 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-50522 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Check Point | 言及あり | 0.80 | — |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [「SharePoint」「Check Point」の脆弱性悪用で警告 - 米当局](https://www.security-next.com/187752) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23936"></a>

### 2. 「使ってはいけないリスト」の生成AI、マルウェア配布に使われるクラウドアプリ

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 34.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Netskopeの調査として、組織内で利用が制限されている生成AIアプリケーションや、情報漏えいのリスクにさらされやすいデータ、マルウェア配布に悪用されやすいクラウドアプリケーションが挙げられています。
いずれも公開情報ベースの調査結果であり、特定の侵害事案を断定する内容ではありません。
生成AIとクラウド利用が広がる中で、業務利用の可否やデータ取り扱い、外部サービスのリスク評価を見直す材料になります。
セキュリティ部門だけでなく、利用部門のガバナンスにも関わる話題です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 社内で許可・制限している生成AI/クラウドアプリの一覧と運用基準を再確認する。
- データの投入可否、共有設定、保存先などの利用ルールが現状の業務実態に合っているか確認する。
- クラウドアプリ経由の不正配布リスクを踏まえ、外部サービスの監視・遮断・教育のバランスを見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [「使ってはいけないリスト」の生成AI、マルウェア配布に使われるクラウドアプリ](https://atmarkit.itmedia.co.jp/ait/articles/2607/23/news061.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-23906"></a>

### 3. Shadow AI is becoming enterprise security’s biggest blind spot

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

AIの業務利用が急速に広がる一方で、組織が把握・管理できない「Shadow AI」がセキュリティ上の盲点になりつつある、という指摘です。
文書要約やコード作成、業務自動化など日常業務にAIが入り込むことで、利用実態の可視化や統制が追いついていない状況が示されています。
未承認のAI利用は、機密情報の取り扱い、データ保護、ガバナンスの面で想定外のリスクを生みやすいためです。
生成AIの導入が進むほど、技術対策だけでなく利用ルールや管理の整備が重要になります。

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

- 社内で使われているAIサービスやAI機能を棚卸しし、利用実態を把握する。
- 機密情報や個人情報を入力しないためのガイドラインと承認手続きを明確にする。
- ログ管理、アクセス制御、データ保護の観点で既存のセキュリティ・ガバナンスにAI利用を組み込む。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| ベンダー | Microsoft | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Shadow AI is becoming enterprise security’s biggest blind spot](https://www.helpnetsecurity.com/2026/07/23/shadow-ai-security-risks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-23476"></a>

### 1. 2026-009: Critical Vulnerabilities in Microsoft SharePoint

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>P⁠o⁠C</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 高温 |
| <nobr>温⁠度⁠感</nobr> | 62.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 67.0 |

#### 概要

Microsoft SharePointの脆弱性CVE-2026-50522について、公開PoCの登場後に実際の悪用が観測されていると複数の情報源が伝えています。
対象はオンプレミスのSharePoint Serverで、未認証の攻撃者によるリモートコード実行につながるおそれがあるとされています。
SharePointは組織内の文書共有や業務基盤として使われることが多く、影響範囲が広くなりやすい点が重要です。
さらに、悪用者がサーバーの機微な鍵情報を狙う動きが報告されており、修正適用後も対応が必要になる可能性があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
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

- 対象バージョンのSharePoint Serverに対し、Microsoftの修正プログラム適用状況を確認する。
- 侵害の有無を確認するため、認証情報の不審な利用やサーバー上の異常な変更を点検する。
- 必要に応じて関連する機密情報や鍵のローテーション、アクセス権の見直しを検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-32201 | 関連CVE | 1.00 | 未確認 |
| 脆弱性 | CVE-2026-45659 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-50522 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-56164 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| 脆弱性 | CVE-2026-58644 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| ベンダー | watchTowr | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |
| 製品 | Microsoft Office | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-50522](https://nvd.nist.gov/vuln/detail/CVE-2026-50522) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [2026-009: Critical Vulnerabilities in Microsoft SharePoint](https://cert.europa.eu/publications/security-advisories/2026-009/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Another SharePoint RCE exploited: Patch, then rotate your machine keys (CVE-2026](https://www.helpnetsecurity.com/2026/07/22/sharepoint-cve-2026-50522-exploited/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Fourth SharePoint Vulnerability Exploited in Past Month’s Wave of Attacks](https://www.securityweek.com/fourth-sharepoint-vulnerability-exploited-in-past-months-wave-of-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical SharePoint RCE flaw exploited to steal machine keys](https://www.bleepingcomputer.com/news/security/critical-sharepoint-rce-flaw-exploited-to-steal-machine-keys/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical SharePoint RCE CVE-2026-50522 Under Active Exploitation After Public Po](https://thehackernews.com/2026/07/critical-sharepoint-rce-cve-2026-50522.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: 候補あり・採用なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [ランサムウェアの身代金の支払い、法律で禁止すべき？ 海外メディアによる賛否両論まとめ【やじうまWatch】](https://internet.watch.impress.co.jp/docs/yajiuma/2127168.html) | 28.0 | 30.0 | 42.0 |
| [OpenAIが報道機関の生成AI活用事例を公開、取材支援から読者向けサービスまで](https://gigazine.net/news/20260723-openai-news-organizations-using-ai/) | 27.0 | 20.0 | 42.0 |
| [米政府、中国AI「Kimi K3」開発元を批判 Anthropic「Fable」を蒸留したとして](https://www.itmedia.co.jp/news/articles/2607/23/news105.html) | 26.0 | 20.0 | 42.0 |
| [ソフトバンク、「GaranAI」ベータ版を提供--コンテンツ産業と生成AI開発の持続的な発展を支援](https://japan.zdnet.com/article/35250884/) | 26.0 | 20.0 | 42.0 |
| [AIエージェントの制御は「コンテンツレイヤー」で Boxが新AIセキュリティ機能群](https://ascii.jp/elem/000/004/421/4421637/?rss=) | 26.0 | 20.0 | 42.0 |
| [ビックリマン風キャラを“自分の顔”からAI生成→Tシャツや缶バッジに ロッテが新サービス公開へ](https://www.itmedia.co.jp/news/articles/2607/23/news086.html) | 26.0 | 20.0 | 42.0 |
| [OpenAI、サイバー攻撃能力テスト中のAIモデルがHugging Faceに不正アクセスしたと発表](https://internet.watch.impress.co.jp/docs/news/2127303.html) | 25.0 | 20.0 | 42.0 |
| [アプリの成長とともに増えるAIコードの脆弱性](https://www.helpnetsecurity.com/2026/07/23/report-ai-code-vulnerabilities/) | 25.0 | 20.0 | 42.0 |
| [Windows 11のログから“攻撃に使われたツール”が分かる？ JPCERT/CCの無料分析シート](https://atmarkit.itmedia.co.jp/ait/articles/2607/23/news059.html) | 21.0 | 20.0 | 42.0 |
| [ニチレイ「今週中に全拠点が通常稼働」 サイバー攻撃から復旧へ](https://www.itmedia.co.jp/news/articles/2607/23/news090.html) | 21.0 | 20.0 | 42.0 |
| [「クレカが使えない！」 16日朝の大規模障害を引き起こした「Cybersource」とは何者か](https://www.itmedia.co.jp/news/articles/2607/23/news053.html) | 21.0 | 20.0 | 42.0 |
| [Axonius、Asset Cloudを拡張しCyber AssetsとExposuresを強化](https://www.helpnetsecurity.com/2026/07/23/axonius-cyber-assets-exposures/) | 20.0 | 20.0 | 42.0 |
| [ポルトガルで拡散しているブラジル発のバンキングトロイの木馬](https://www.darkreading.com/cyberattacks-data-breaches/brazilian-banking-trojan-spreading-portugal) | 20.0 | 20.0 | 42.0 |
| [医師を誹謗中傷したことが私的な医療記録へのアクセスにつながった](https://www.theregister.com/security/2026/07/23/talking-smack-about-a-doctor-got-him-access-to-private-medical-files/5276604) | 20.0 | 20.0 | 42.0 |
| [ISC BINDにおける複数の脆弱性（2026年7月）](https://jvn.jp/vu/JVNVU97496543/) | 20.0 | 20.0 | 42.0 |
| [バックアップソフトウェア「Duplicati」における不適切な権限割り当てに関する脆弱性](https://jvn.jp/vu/JVNVU98636554/) | 20.0 | 20.0 | 42.0 |
| [Analog Way製メディアサーバー「Picturall Quad Compact Mark II」におけるローカル権限昇格の脆弱性](https://jvn.jp/vu/JVNVU98875819/) | 20.0 | 20.0 | 42.0 |
| [AppViewX Agent Identity Securityの製品紹介](https://www.helpnetsecurity.com/2026/07/23/product-showcase-appviewx-agent-identity-security/) | 20.0 | 20.0 | 42.0 |
| [米国がSiemens、Schneider、RockwellのICS機器を狙うイラン系ハッカーに警告](https://www.securityweek.com/us-warns-of-iranian-hackers-targeting-siemens-schneider-and-rockwell-ics-devices/) | 20.0 | 20.0 | 42.0 |
| [複数パッチの脆弱性修正でオープンソースが露出する可能性](https://www.helpnetsecurity.com/2026/07/23/research-multi-patch-vulnerability-fixes/) | 20.0 | 20.0 | 42.0 |
| [リコー製プリンターおよび複合機のSSH通信機能におけるアクセス制御不備の脆弱性](https://jvn.jp/jp/JVN32082029/) | 20.0 | 20.0 | 42.0 |
| [機密データを守るための多層防御戦略](https://www.helpnetsecurity.com/2026/07/23/defense-in-depth-strategy-video/) | 20.0 | 20.0 | 42.0 |

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
