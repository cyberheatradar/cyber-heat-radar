# 📡 サイレーダー 2026-05-26 18:16 JST

このレポートは、2026-05-26 12:15 JST〜2026-05-26 18:15 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 65
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [KnowledgeDeliver LMS Flaw Exploited to Deploy Godzilla and Cobalt Strike](#topic-9892) | 50.0 | 64.0 | 55.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [CISA orders feds to patch actively exploited Drupal vulnerability](#topic-10311) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 3 | [ランサムウェア攻撃が「持続可能なビジネス」に 侵入コスト6万6000円、復旧に2億3000万円](#topic-10211) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Microsoft 365 CopilotのAIエージェント機能「Cowork」が勝手にファイルを流出させる可能性があるとセキュリティ企業が指摘](#topic-10218) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-10311"></a>

### 1. CISA orders feds to patch actively exploited Drupal vulnerability

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

CISAは、Drupalのコンテンツ管理システムに存在するSQLインジェクションの脆弱性について、実際に悪用されているとして米政府機関に期限付きで対処を求めました。
公開情報では、対象の脆弱性が現に攻撃に使われている可能性が示されています。Drupalは広く使われているため、影響を受ける環境があれば被害が広がるおそれがあります。
公的機関が緊急対応を促している点からも、優先度の高いパッチ適用対象と考えられます。

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

- Drupalを利用するサーバーで、該当する修正版やベンダー案内が出ていないか早急に確認する。
- 外部公開中の管理画面や関連サービスを点検し、不要な露出や古い構成がないか確認する。
- ログ監視を強化し、異常なリクエストや不審なデータベース操作の兆候を確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [CISA orders feds to patch actively exploited Drupal vulnerability](https://www.bleepingcomputer.com/news/security/cisa-orders-feds-to-patch-actively-exploited-drupal-vulnerability/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-10211"></a>

### 2. ランサムウェア攻撃が「持続可能なビジネス」に 侵入コスト6万6000円、復旧に2億3000万円

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

ランサムウェア攻撃では、侵入にかかるコストが小さい一方で、被害企業側の復旧費用は非常に大きくなりうることが指摘されています。
今回の材料では、その差が約3500倍に達する例が示され、攻撃側にとって収益化しやすい構造が問題視されています。
被害復旧の負担が極端に大きいと、攻撃は継続的に成立しやすくなり、同種の被害が繰り返される懸念があります。
企業にとっては、侵入を防ぐ対策だけでなく、事業継続や復旧計画の実効性が改めて重要になります。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- バックアップ、復旧手順、権限管理など、被害後の回復力を定期的に点検する。
- 初期侵入を減らすため、認証強化や脆弱性管理、端末監視を継続する。
- 復旧費用の膨張を抑えるため、重要システムの優先順位と連絡体制を事前に整理しておく。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [ランサムウェア攻撃が「持続可能なビジネス」に　侵入コスト6万6000円、復旧に2億3000万円](https://www.itmedia.co.jp/news/articles/2605/26/news108.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 弱。
- 日本語圏反応: 反応あり。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-10218"></a>

### 3. Microsoft 365 CopilotのAIエージェント機能「Cowork」が勝手にファイルを流出させる可能性があるとセキュリティ企業が指摘

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>クラウド</nobr> / <nobr>AIエージェント</nobr> / <nobr>Windows</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Microsoft 365 CopilotのAIエージェント機能「Cowork」について、セキュリティ企業が間接プロンプト注入を通じてSharePointやOneDrive上のファイルが流出する可能性を指摘しています。
現時点では公開情報ベースの報告であり、詳細な影響範囲や再現性は追加確認が必要です。
Copilotのように業務データへ広くアクセスするAI機能では、従来の権限管理だけでは想定しにくい情報漏えい経路が生じうるためです。
利用部門・管理部門の双方で、AI機能の許可範囲やデータ保護設定を見直す契機になります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- SharePoint/OneDrive連携を含むCopilot系機能の権限設定とデータアクセス範囲を確認する。
- AIエージェントに入力される外部コンテンツや参照元の取り扱いを点検し、不要な自動応答を抑える。
- 監査ログやDLP設定を見直し、AI経由の情報持ち出し兆候を把握できるようにする。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| ai_model_or_project | Copilot | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft 365 CopilotのAIエージェント機能「Cowork」が勝手にファイルを流出させる可能性があるとセキュリティ企業が指摘](https://gigazine.net/news/20260526-microsoft-copilot-cowork-exfiltrates-files/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 反応あり。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-9892"></a>

### 1. KnowledgeDeliver LMS Flaw Exploited to Deploy Godzilla and Cobalt Strike

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>脅威アクター</nobr> / <nobr>Windows</nobr> / <nobr>ゼロデイ</nobr> / <nobr>IoC</nobr> / <nobr>iOS</nobr> / <nobr>RCE</nobr> / <nobr>CVE</nobr> / <nobr>防御・運用</nobr> / <nobr>政策・規制</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 50.0 |
| <nobr>実務影響</nobr> | 64.0 |
| <nobr>確度</nobr> | 55.0 |

#### 概要

KnowledgeDeliver LMS に存在した脆弱性が悪用され、認証なしでのリモートコード実行につながったと報告されています。
攻撃者は侵入後、Webシェルの配置やWebコンテンツの改ざんを行い、最終的に利用者端末へ追加の不正コードを誘導したとされています。
日本で広く使われるLMSに関わるため、影響範囲が単一組織にとどまらない可能性があります。
さらに、共有されたASP.<wbr>NET machine keyのような設定上の弱点は、個別環境の分離を前提にした運用でも横断的な侵害につながり得る点で重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
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

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- KnowledgeDeliver の該当バージョンを洗い出し、ベンダー案内に従って machine key が各環境で一意か確認する。
- IIS/ASP.<wbr>NET のイベントログ、Webルートの改ざん、w3wp.exe からの不審な子プロセス生成を重点的に確認する。
- LMS へのアクセス制御を見直し、不要な外部公開を避けるとともに、異常なリクエストやファイル変更を継続監視する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-5426 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-5426](https://nvd.nist.gov/vuln/detail/CVE-2026-5426) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [KnowledgeDeliver LMS Flaw Exploited to Deploy Godzilla and Cobalt Strike](https://thehackernews.com/2026/05/knowledgedeliver-lms-flaw-exploited-to.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Exploitation of KnowledgeDeliver via ViewState Deserialization Vulnerability](https://cloud.google.com/blog/topics/threat-intelligence/knowledgedeliver-viewstate-deserialization-vulnerability/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [F-Secure Internet Securityがフィッシングサイト、偽ストア、SMS詐欺をブロックする製品紹介](https://www.helpnetsecurity.com/2026/05/26/product-showcase-f-secure-internet-security-android/) | 36.0 | 30.0 | 42.0 |
| [Iranian HackersがフィッシングとSEOポイズニングでMiniFastとMiniJunk V2を展開](https://thehackernews.com/2026/05/iranian-hackers-deploy-minifast-and.html) | 28.0 | 20.0 | 42.0 |
| [AnthropicのAI「Claude Mythos」、1カ月で1万件超の脆弱性発見 修正作業追いつかず](https://news.mynavi.jp/techplus/article/20260526-4504331/) | 27.0 | 20.0 | 42.0 |
| [WordPressプラグイン・テーマの脆弱性最新情報 第29回 WordPress脆弱性13件、AI Engineの権限昇格や認証バイパスに注意【5月14日～5月20日】](https://news.mynavi.jp/techplus/article/wordpressvulnerability-29/) | 26.0 | 20.0 | 42.0 |
| [Microsoft: Windows Server 2016でドメインコントローラーの検索に失敗する可能性](https://www.bleepingcomputer.com/news/microsoft/microsoft-domain-controller-lookup-may-fail-on-windows-server-2016/) | 25.0 | 20.0 | 42.0 |
| [ソフトバンク、「AIデータセンター GPUクラウド」を10月に提供開始～運用負荷の軽減と柔軟性を実現するクラウドサービス](https://internet.watch.impress.co.jp/docs/news/2111560.html) | 25.0 | 20.0 | 42.0 |
| [NTTドコモが販売する「CM51FD」など、Atermの5Gモバイルルーター2製品に脆弱性。最新のファームウェアにアップデートを](https://internet.watch.impress.co.jp/docs/news/2111596.html) | 24.0 | 38.0 | 42.0 |
| [Linuxカーネルにおける複数の脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-016978.html) | 22.0 | 32.0 | 42.0 |
| [県内高校で生徒情報含む連携支援シートを紛失 - 新潟県](https://www.security-next.com/184953) | 22.0 | 20.0 | 42.0 |
| [元従業員が取引先情報を持ち出し - ロッキング・オン・ジャパン](https://www.security-next.com/184948) | 22.0 | 20.0 | 42.0 |
| [イランのネット接続が再開へ　大統領が承認、戦争後に海外サイトから3カ月遮断](https://www.itmedia.co.jp/news/articles/2605/26/news114.html) | 21.0 | 20.0 | 42.0 |
| [OpenAIの新しい画像透かし、AI生成の偽物を見分けやすく--その仕組みとは](https://japan.zdnet.com/article/35248024/) | 21.0 | 20.0 | 42.0 |
| [スカパー！、交流戦の一部試合でチャット機能を停止　巨人戦など](https://www.itmedia.co.jp/news/articles/2605/26/news113.html) | 21.0 | 20.0 | 42.0 |
| [薬局で受け取った薬の情報、マイナポータルで当日中に確認可能に 「薬」画面をリニューアル](https://www.itmedia.co.jp/news/articles/2605/26/news106.html) | 21.0 | 20.0 | 42.0 |
| [フェラーリ、初のEV「Ferrari Luce」発表 元Appleデザイナー、ジョニー・アイブ氏のLoveFromがデザイン担当](https://www.itmedia.co.jp/news/articles/2605/26/news096.html) | 21.0 | 20.0 | 42.0 |
| [松下幸之助氏の「AI偽動画」に注意 PHP研究所が再告知 津田健次郎さんによるTikTok提訴受け](https://www.itmedia.co.jp/news/articles/2605/26/news080.html) | 21.0 | 20.0 | 42.0 |
| [被害長女がChatGPTに相談→児相に通報か 巨人・阿部前監督の暴行事件](https://www.itmedia.co.jp/news/articles/2605/26/news081.html) | 21.0 | 20.0 | 42.0 |
| [CVE-2025-3198: GNU Binutilsのobjdumpにおけるbucomm.cのdisplay_infoメモリリーク](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2025-3198) | 20.0 | 28.0 | 38.0 |
| [あなたのビジネスにソフトウェア部品表は必要か](https://www.itpro.com/security/does-your-business-need-a-software-bill-of-materials) | 20.0 | 20.0 | 42.0 |
| [FBIがMicrosoft 365ユーザーに警告する新たなPhishing as a Service攻撃とその回避策](https://www.itpro.com/security/fbi-warns-microsoft-365-users-about-another-phishing-as-a-service-attack-heres-how-to-avoid-it) | 20.0 | 20.0 | 42.0 |
| [dnsmasqにおける複数の脆弱性](https://jvn.jp/vu/JVNVU90845089/) | 20.0 | 20.0 | 42.0 |
| [7-Elevenのデータ侵害で18万5,000人の個人情報が流出](https://www.bleepingcomputer.com/news/security/7-eleven-data-breach-exposes-personal-information-of-185-000-people/) | 20.0 | 20.0 | 42.0 |
| [マシンIDを管理する：管理すべき隠れた特権アクセス層](https://www.helpnetsecurity.com/2026/05/26/delinea-managing-managing-machine-identities-access/) | 20.0 | 20.0 | 42.0 |
| [今すぐ応募できるサイバーセキュリティ求人：2026年5月26日](https://www.helpnetsecurity.com/2026/05/26/cybersecurity-jobs-available-right-now-may-26-2026/) | 20.0 | 20.0 | 42.0 |

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
