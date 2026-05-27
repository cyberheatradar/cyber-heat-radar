# 📡 サイレーダー 2026-05-28 05:00 JST

このレポートは、2026-05-27 17:00 JST〜2026-05-28 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 126
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CISA Adds Three Known Exploited Vulnerabilities to Catalog](#topic-10948) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 2 | [CISA gives feds 4 days to patch actively exploited cPanel plugin flaw](#topic-10922) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [New ransomware threat group, The Gentlemen, has become one of the most active ransomware operators, accounting for 10% of all attacks](#topic-10927) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [AI chatbot recommendations lure users to cryptojacking malware sites](#topic-10940) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 5 | [Evidence at the Moment of Attack. Answers at AI Speed.](#topic-10946) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 6 | [eSentire launches new Atlas AI Operatives for autonomous threat detection and response](#topic-10893) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 7 | [Fake ChatGPT and Claude installers on GitHub are dropping Deno RAT malware](#topic-10905) | 33.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-10948"></a>

### 1. CISA Adds Three Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>KEV</nobr> / <nobr>CVE</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

CISAは、実際の悪用が確認されたとして、Known Exploited Vulnerabilities（KEV）カタログに3件の脆弱性を追加しました。
対象はCVE-2026-8398、CVE-2026-45321、CVE-2026-48027で、いずれも関連製品の利用環境では優先的な対応が求められます。
KEVカタログへの追加は、当該脆弱性が現実の攻撃対象になっていることを示すため、放置リスクが高いと見なす必要があります。
特に資産把握が不十分な環境では、影響範囲の特定と修正の優先順位付けが重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 対象製品の利用有無を確認し、該当環境を洗い出す。
- ベンダー情報と修正可否を確認し、優先度を上げて適用する。
- 関連ログや検知ルールを見直し、不審な挙動がないか確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-8398 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-45321 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-48027 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Three Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/05/27/cisa-adds-three-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-10922"></a>

### 2. CISA gives feds 4 days to patch actively exploited cPanel plugin flaw

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

米サイバーセキュリティ・社会基盤安全保障庁（CISA）が、cPanel向けLiteSpeedプラグインに関連する脆弱性について、米連邦機関に短期間での対応を求めました。
材料では、この問題がすでに攻撃で悪用されているとされており、サーバー管理者に早急な確認と更新が必要な状況です。
公的機関が期限を区切って対応を促している点から、実運用環境への影響が懸念されています。管理対象にcPanel環境が含まれる組織では、優先度を上げて影響確認を行うべき話題です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- cPanelおよびLiteSpeed関連コンポーネントの利用有無と、適用済みバージョンを確認する。
- ベンダーや公的機関の更新情報を確認し、利用中の環境に対して優先的にパッチ適用を検討する。
- 外部公開された管理画面や関連サービスについて、監視とアクセス制御を再点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | cPanel | 言及あり | 0.80 |
| 製品 | cPanel | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [CISA gives feds 4 days to patch actively exploited cPanel plugin flaw](https://www.bleepingcomputer.com/news/security/cisa-gives-feds-4-days-to-patch-actively-exploited-cpanel-plugin-flaw/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-10927"></a>

### 3. New ransomware threat group, The Gentlemen, has become one of the most active ransomware operators, accounting for 10% of all attacks

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> / <nobr>TTP</nobr> / <nobr>マルウェア</nobr> / <nobr>防御・運用</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

NTTの研究者によると、ランサムウェア・アズ・ア・サービス（RaaS）型の攻撃グループ「The Gentlemen」が活発化しており、全体の攻撃の一部で大きな存在感を示しているとされています。
報告では、SystemBCマルウェアを使って検知回避や組織内での横展開を支援している可能性が指摘されています。
ランサムウェアは業務停止や情報漏えいにつながりやすく、活動が活発なグループの動向は防御側の優先監視対象になります。
特に、検知を避けながら侵入後の展開を進める手口が示唆されるため、既存の監視だけでは見落としが起きるおそれがあります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SystemBCのような不審なトンネリングや中継通信の兆候を監視対象に含めること。
- 横展開を想定し、特権アカウントや内部通信の異常、認証イベントの連続失敗を確認すること。
- ランサムウェア対策として、バックアップの隔離保全と復旧手順の定期検証を優先すること。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [New ransomware threat group, The Gentlemen, has become one of the most active ra](https://www.itpro.com/security/new-ransomware-threat-group-the-gentlemen-has-become-one-of-the-most-active-ransomware-operators-accounting-for-10-percent-of-all-attacks) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-10940"></a>

### 4. AI chatbot recommendations lure users to cryptojacking malware sites

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>攻撃キャンペーン</nobr> / <nobr>マルウェア</nobr> |
| <nobr>分類理由</nobr> | AI×Security枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Microsoftによると、攻撃者がAIチャットボットでのやり取りと検索結果の汚染を組み合わせ、暗号資産採掘型マルウェアへ誘導するキャンペーンが確認されています。
正規のユーティリティや周辺ソフトに見せかけた名称が使われており、利用者が誤って不正サイトから入手してしまうリスクが指摘されています。
AIチャットボットの回答や検索結果が、ユーザーのダウンロード先選びに影響しうることを示す事例です。
正規ソフトの名称を悪用した誘導は、一般ユーザーだけでなくPC愛好家や管理者にも誤認を起こしやすい点が注意されます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ソフト配布先は、チャットボットの推薦や検索結果だけに依存せず、公式サイトや検証済みの入手経路で確認する。
- 社内向けには、正規ツール名を騙る不審なダウンロードサイトや広告経由の流入に対する注意喚起を行う。
- 端末側では、ダウンロード後の不審な挙動や不要な採掘負荷を検知できるよう、EDRや監視ルールを見直す。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [AI chatbot recommendations lure users to cryptojacking malware sites](https://www.helpnetsecurity.com/2026/05/27/ai-chatbot-cryptojacking-campaign/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-10946"></a>

### 5. Evidence at the Moment of Attack. Answers at AI Speed.

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>防御・運用</nobr> |
| <nobr>分類理由</nobr> | AI×Security枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Wizは、検知時点でフォレンジック用の情報を自動収集し、AIで調査を支援する「Wiz Sensor Forensics」を一般提供開始したとしています。
SOCやIRチームの初動調査を速めることを狙った機能で、アラート対応時の証跡確保を補助する位置づけです。
クラウド環境では、検知後に必要な証跡が失われると調査が難しくなるため、検知時点での自動採取は実務上の価値があります。
AIを使った整理・要約が加わることで、限られた運用人員でも対応速度の改善が期待されます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- アラート発生時に何が自動で保存されるのか、対象範囲と保持条件を確認する。
- 既存のSIEM/SOARやインシデント対応手順と連携できるかを検証する。
- AIによる支援結果は補助情報として扱い、最終判断は生データと合わせて行う。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Evidence at the Moment of Attack. Answers at AI Speed.](https://www.wiz.io/blog/wiz-sensor-forensics-ga) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-10893"></a>

### 6. eSentire launches new Atlas AI Operatives for autonomous threat detection and response

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>防御・運用</nobr> / <nobr>AIエージェント</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

eSentireが、Atlas Platformにおいて自律的な脅威検知と対応を行う新機能群を発表しました。
AIオペラティブ同士が連携し、予防・検知・対応を継続的に回す設計だとされています。
AIを活用したセキュリティ運用の自動化は、SOCやMDRの効率化に直結するため注目されています。
攻撃対応の迅速化や運用負荷の軽減につながる可能性があり、ベンダー各社の実装動向を比較する材料にもなります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 自律化の範囲がどこまでか、検知・封じ込め・復旧のどの工程まで任せられるのかを確認する。
- 誤検知時の挙動や、人手による承認が必要な条件など、制御性と監査性を評価する。
- 既存のMDRやSIEM/SOARとの連携可否、導入後の運用設計への影響を見ておく。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [eSentire launches new Atlas AI Operatives for autonomous threat detection and re](https://www.helpnetsecurity.com/2026/05/27/esentire-atlas-platform-capabilities/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-10905"></a>

### 7. Fake ChatGPT and Claude installers on GitHub are dropping Deno RAT malware

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>マルウェア</nobr> / <nobr>AI</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

GitHubやSourceForge上で、ChatGPTやClaudeなどの人気ソフトを装った偽インストーラーやプラグインが確認されたと報じられています。
これらのダウンロードはバックドアを経由して、Deno JavaScript runtime を使ったRATにつながるとされています。
さらに、改ざんされたYouTubeチャンネルからこれらの不正なリポジトリへ誘導しているとされています。
生成AI関連の名前を悪用した配布手口は、利用者が正規の入手先と誤認しやすく、被害につながりやすい点が注意されます。
ソフトの入手経路が複数の公開プラットフォームにまたがるため、組織としての確認範囲も広がります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ソフト配布は公式サイトや信頼できる配布経路に限定し、GitHub等の第三者掲載物はそのまま信用しない。
- YouTubeやSNS経由の案内先URLを鵜呑みにせず、提供元・署名・ハッシュなどの確認を徹底する。
- 端末保護製品とログ監視で、未知のバックドアや不審な実行ファイルの起動を早期検知できるようにする。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ai_model_or_project | ChatGPT | 主題 | 0.80 |
| ai_model_or_project | Claude | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Fake ChatGPT and Claude installers on GitHub are dropping Deno RAT malware](https://www.helpnetsecurity.com/2026/05/27/deno-rat-malware-fake-chatgpt-claude-installers/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

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
| [連携作戦でGlasswormボットネットを摘発](https://www.cybersecuritydive.com/news/takedown-glassworm-botnet-crowdstrike-Google-Shadowserver/821227/) | 28.0 | 40.0 | 42.0 |
| [GlassWormマルウェアのテイクダウンで開発者向けサプライチェーン攻撃インフラが混乱](https://thehackernews.com/2026/05/glassworm-malware-takedown-disrupts.html) | 28.0 | 40.0 | 42.0 |
| [GrandoreiroマルウェアとBTMOB RATキャンペーンがWindowsおよびAndroidユーザーを標的にする](https://thehackernews.com/2026/05/grandoreiro-malware-and-btmob-rat.html) | 28.0 | 20.0 | 42.0 |
| [CrowdStrikeとGoogleがGlasswormボットネットを停止](https://www.infosecurity-magazine.com/news/crowdstrike-google-takedown/) | 28.0 | 20.0 | 42.0 |
| [Commit to Compromise：暗号資産業界のソフトウェア開発基盤を狙う新たな脅威アクター](https://www.wiz.io/blog/threat-actors-target-crypto-orgs) | 28.0 | 20.0 | 42.0 |
| [CrowdStrikeがオープンソースのサプライチェーンを狙うGlasswormボットネットを妨害](https://cyberscoop.com/crowdstrike-glassworm-botnet-takedown/) | 28.0 | 20.0 | 42.0 |
| [Glasswormボットネット、堅牢なC2インフラのテイクダウン後に停止](https://www.bleepingcomputer.com/news/security/glassworm-botnet-disrupted-after-resilient-c2-infrastructure-takedown/) | 28.0 | 20.0 | 42.0 |
| [ANY.RUNの10年にわたる進化：CEO Aleksey Lapshinへのインタビュー](https://any.run/cybersecurity-blog/ceo-interview-anyrun-10-years/) | 28.0 | 20.0 | 42.0 |
| [GlassWormボットネットが無力化される](https://www.securityweek.com/glassworm-botnet-disrupted/) | 28.0 | 20.0 | 42.0 |
| [LA Metroへのサイバー攻撃、イラン国家支援ハッカーと関連か](https://www.securityweek.com/la-metro-cyberattack-linked-to-iranian-state-sponsored-hackers/) | 28.0 | 20.0 | 42.0 |
| [Cogent、AI搭載の新たなセキュリティ機能で攻撃から修復までのギャップを狙う](https://www.helpnetsecurity.com/2026/05/27/cogent-zero-day-response-and-autonomous-remediation/) | 27.0 | 20.0 | 43.0 |
| [Stack OverflowのフォーラムはAIが原因で消滅しかけているが企業自体はまだAIのおかげで健在](https://gigazine.net/news/20260527-stack-overflow-ai/) | 27.0 | 20.0 | 42.0 |
| [悪意あるnpmパッケージがGitHub経由でClaude AIユーザーディレクトリからファイルを窃取](https://thehackernews.com/2026/05/malicious-npm-package-stole-files-from.html) | 25.0 | 30.0 | 42.0 |
| [英国のスパイ長官、AIを「止められない力」と位置づけサイバー空間における攻防両面の影響を指摘](https://cyberscoop.com/gchq-warns-ai-cyber-warfare-threats/) | 25.0 | 20.0 | 42.0 |
| [英国のサイバー諜報責任者、AIを「止められない力」と呼びロシアに警鐘](https://www.securityweek.com/uk-cyberspying-chief-calls-ai-an-unstoppable-force-and-warns-about-russia/) | 25.0 | 20.0 | 42.0 |
| [AI支援によるエクスプロイト開発がスキャナーの検知を上回る](https://www.darkreading.com/threat-intelligence/ai-assisted-exploit-development-scanner-detection) | 25.0 | 20.0 | 42.0 |
| [主要なAIモデルはベンダーの主張よりも悪意あるプロンプトに脆弱である](https://www.cybersecuritydive.com/news/cisco-ai-models-research-multi-turn-prompt-attacks/821211/) | 25.0 | 20.0 | 42.0 |
| [Google AI Threat Defense、AIを使って脆弱性を迅速に見つける攻撃者を標的にする](https://www.helpnetsecurity.com/2026/05/27/google-ai-threat-defense-released/) | 25.0 | 20.0 | 42.0 |
| [Ping IdentityがAIガバナンスと信頼できるアクセスでエージェント型セキュリティを強化](https://www.helpnetsecurity.com/2026/05/27/ping-identity-advances-agentic-security-with-ai-governance-and-trusted-access/) | 25.0 | 20.0 | 42.0 |
| [SecurityWeek、8月11日～12日にThe Ritz-Carlton Half Moon BayでAIリスクサミットを開催](https://www.securityweek.com/securityweek-to-host-ai-risk-summit-august-11-12-at-the-ritz-carlton-half-moon-bay/) | 25.0 | 20.0 | 42.0 |
| [Microsoft Entra Agent IDにおける不審なAIワークフローの調査：自律型エージェント](https://redcanary.com/blog/threat-detection/entra-id-ai-workflows/) | 25.0 | 20.0 | 42.0 |
| [サイバーセキュリティの進化：境界防御からAIネイティブセキュリティへ](https://www.darkreading.com/cybersecurity-operations/cybersecurity-evolution-perimeter-defense-to-ai-native-security) | 25.0 | 20.0 | 42.0 |
| [AI脅威に備えるためのWizによる機械速度での防御](https://www.wiz.io/blog/wiz-ai-threat-readiness-operating-model) | 25.0 | 20.0 | 42.0 |
| [RevEng.AIがソフトウェアバイナリの脆弱性とバックドア発見に1500万ドルを調達](https://www.securityweek.com/reveng-ai-raises-15-million-to-hunt-for-flaws-and-backdoors-in-software-binaries/) | 25.0 | 20.0 | 42.0 |

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
