# 📡 サイレーダー 2026-08-11 05:00 JST

このレポートは、2026-08-10 17:00 JST〜2026-08-11 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 91
- [音声で扱う想定のトピック](#audio-topics): 6
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 60

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2024-55591: CISA KEV catalog addition](#topic-3175) | 45.0 | 74.0 | 55.0 | 音声 | 温度感上位枠 |
| 2 | [N-able ships second N-central hotfix as attackers keep exploiting CVE-2026-18577](#topic-25667) | 45.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |
| 3 | [Metabase zero-day exploited to access Framework customer data](#topic-26950) | 45.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Metabase Patches Vulnerability Exploited as Zero-Day](#topic-26978) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 5 | [Critical Progress LoadMaster flaw now actively exploited in attacks](#topic-26990) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 6 | [Kimsuky Builds Offline AI Stack to Boost Phishing and Automate Malware Development](#topic-26954) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-3175"></a>

### 1. CVE-2024-55591: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>T⁠T⁠P</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>L⁠i⁠n⁠u⁠x</nobr> / <nobr>K⁠E⁠V</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 74.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

CVE-2024-55591がCISAのKEVカタログに追加され、既知の悪用対象として扱われています。
材料では、この脆弱性はランサムウェア関連の文脈でも言及されており、複数ソースで悪用観測が示されています。
KEV入りは、実際の攻撃で使われている可能性が高く、対応優先度を上げる目安になります。影響範囲が広い製品や周辺システムに波及しうるため、運用上の確認が必要です。

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
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- CVE-2024-55591を含む対象製品の利用有無を確認し、優先度高めでパッチ適用計画を見直す。
- 外部公開面や管理系アクセス経路を点検し、不要な露出がないか確認する。
- 関連する認証情報の保護、ログ監視、侵害兆候の点検を行い、既存の検知ルールを見直す。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2024-55591 | 関連CVE | 1.00 | 候補あり（URL 11件以上） |
| 脆弱性 | CVE-2025-33073 | 関連CVE | 1.00 | 候補あり（URL 42件以上） |
| 脆弱性 | CVE-2025-61882 | 関連CVE | 1.00 | 候補あり（URL 13件以上） |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2024-55591](https://nvd.nist.gov/vuln/detail/CVE-2024-55591) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [#StopRansomware: Gunra Ransomware](https://www.cisa.gov/news-events/cybersecurity-advisories/aa26-222a) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Thus Spoke…The Gentlemen](https://research.checkpoint.com/2026/thus-spoke-the-gentlemen/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [The State of Ransomware – Q1 2026](https://research.checkpoint.com/2026/the-state-of-ransomware-q1-2026/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-25667"></a>

### 2. N-able ships second N-central hotfix as attackers keep exploiting CVE-2026-18577

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>C⁠I⁠S⁠O⁠・⁠組⁠織⁠運⁠営</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

N-ableのRMM製品「N-central」に存在する認証バイパスの脆弱性（CVE-2026-18577）について、悪用が継続しているとして追加のホットフィックスが公開されました。
影響はホスト型・オンプレミス双方の環境に及ぶとされ、既に前回の修正を適用していても追加対応が必要と案内されています。
RMM製品は管理対象の端末や顧客環境への広い権限を持つため、ここが突破されると影響が大きくなりやすいです。
既存の修正だけでは不十分だった可能性が示されており、運用中の管理基盤の見直しが重要になります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 5 sources。
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

- N-centralの該当バージョンと適用済みホットフィックスを確認し、追加ホットフィックスの適用状況を点検する。
- 管理者権限の不審な作成・変更、認証回避を示すログ、ベンダーが示す侵害指標の有無を確認する。
- 影響範囲に応じて、外部公開の制限、管理者アカウントの棚卸し、関連資格情報の更新を検討する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-18577 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-18577](https://nvd.nist.gov/vuln/detail/CVE-2026-18577) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [N-able ships second N-central hotfix as attackers keep exploiting CVE-2026-18577](https://www.helpnetsecurity.com/2026/08/10/cve-2026-18577-n-central-hotfix-2-msps/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-18577: N-able N-central Authentication Bypass Exploited in the Wild](https://www.rapid7.com/blog/post/etr-cve-2026-18577-n-able-n-central-authentication-bypass-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit N-able Patch Bypass Flaw on RMM Servers](https://www.darkreading.com/vulnerabilities-threats/attackers-exploit-n-able-patch-bypass-flaw) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [N-able warns of N-central auth bypass flaw exploited in attacks](https://www.bleepingcomputer.com/news/security/n-able-warns-of-n-central-auth-bypass-flaw-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers exploit N-able N-central flaw to reach managed endpoints (CVE-2026-185](https://www.helpnetsecurity.com/2026/08/03/cve-2026-18577-n-able-n-central-vulnerability/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [N‑able Patches Vulnerability Exploited to Hack N-central Servers](https://www.securityweek.com/n-able-patches-vulnerability-exploited-to-hack-n-central-servers/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。

---

<a id="topic-26950"></a>

### 3. Metabase zero-day exploited to access Framework customer data

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 45.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Frameworkの顧客向け通知によると、Metabaseのゼロデイ脆弱性が悪用され、顧客データへの不正アクセスが発生したとされています。
現時点で、氏名、メールアドレス、電話番号、住所、ログインIPアドレスがアクセスされた一方、支払い情報や注文関連の記録は対象外だったと案内されています。
ゼロデイ脆弱性の悪用が実際の顧客情報流出につながった事例であり、SaaSや社内BIツールも重要な攻撃対象になり得ることを示しています。
直接の金銭情報が含まれなくても、連絡先や住所などの情報は二次被害やなりすましに悪用される可能性があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Metabaseなど社内向け分析基盤の外部公開範囲とアクセス制御を再点検する。
- 顧客通知に含まれた漏えい項目を確認し、該当する利用者への案内や監視を行う。
- ゼロデイや既知脆弱性への対応として、資産把握・更新適用・認証強化の運用を見直す。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Metabase zero-day exploited to access Framework customer data](https://www.helpnetsecurity.com/2026/08/10/metabase-zero-day-framework-tally-kilo-code/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-26978"></a>

### 4. Metabase Patches Vulnerability Exploited as Zero-Day

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Metabaseに存在する脆弱性が修正され、ゼロデイとして悪用されていたと報じられています。
公開情報によれば、認証されていない遠隔攻撃者がMetabaseインスタンスで管理者権限を得られる可能性がありました。
認証を必要とせずに管理者権限へ到達しうる点は、影響範囲が広く、侵害時の被害が大きくなりやすいため注目されています。
ゼロデイとしての悪用が示唆されているため、既存の対策状況にかかわらず早急な確認が必要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Metabaseを公開運用している場合は、最新版への更新状況とベンダーの修正内容を確認する。
- 管理画面への到達性、外部公開の有無、アクセス制御の設定を見直す。
- 不審な管理者権限付与や設定変更、ログイン履歴の異常がないか監査する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Metabase Patches Vulnerability Exploited as Zero-Day](https://www.securityweek.com/metabase-patches-vulnerability-exploited-as-zero-day/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-26990"></a>

### 5. Critical Progress LoadMaster flaw now actively exploited in attacks

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

CISAは、Progress Kemp LoadMasterに存在する重大なコマンドインジェクション脆弱性が攻撃で悪用されていると警告しました。
対象製品の管理環境が影響を受ける可能性があり、利用組織では早急な確認と対策が必要とされています。
実際の悪用が確認されているため、単なる脆弱性情報ではなく、被害につながるリスクが高い点が注目されています。
管理系機器は影響範囲が大きく、侵害されると可用性や機密性に波及しやすい点も重要です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Progress Kemp LoadMasterの該当バージョンや公開状況を確認し、ベンダー案内やCISA情報に沿って修正を適用する。
- 外部公開している管理インターフェースやアクセス制御を見直し、不要な露出がないか点検する。
- 監査ログや認証履歴を確認し、想定外の管理操作や不審な要求がないか監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-8037 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| 製品 | Progress Kemp LoadMaster | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Critical Progress LoadMaster flaw now actively exploited in attacks](https://www.bleepingcomputer.com/news/security/cisa-warns-of-critical-progress-loadmaster-flaw-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-26954"></a>

### 6. Kimsuky Builds Offline AI Stack to Boost Phishing and Automate Malware Development

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>A⁠I</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>国⁠家⁠支⁠援</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

北朝鮮系とされる脅威グループ「Kimsuky」が、公開AIサービスに頼らず、自前の環境でAIを動かす形に移行していると報じられました。
文書検索機能と手元の資料を組み合わせ、フィッシングの作成やマルウェア開発の補助にAIを使う動きが示唆されています。
攻撃側が外部サービス依存を減らし、運用を見えにくくする方向に進んでいる可能性があるため、検知や分析の前提が変わるおそれがあります。
特に、標的型メールやマルウェア関連の活動がより効率化される懸念が注目されています。

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

- フィッシング文面の品質向上や多言語化など、生成AIの悪用を前提にメール対策と利用者教育を見直す。
- 社内文書や機微情報の流出が、攻撃者側の検索・要約の精度向上につながり得るため、保管範囲とアクセス権限を再点検する。
- AI関連の挙動に限らず、標的型メール・不審な添付・認証情報窃取の兆候を従来どおり広く監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脅威アクター | Kimsuky | 主題 | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Kimsuky Builds Offline AI Stack to Boost Phishing and Automate Malware Developme](https://thehackernews.com/2026/08/kimsuky-builds-offline-ai-stack-that.html) | <nobr>内容確認・補足情報</nobr> |

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
| [Metabaseのゼロデイ攻撃でFrameworkが顧客データを失う](https://www.theregister.com/personal-tech/2026/08/10/framework-loses-customer-data-in-metabase-zero-day-attack/5285302) | 37.0 | 38.0 | 43.0 |
| [元Medusaの関係者が使用する新たなStormEncryptorランサムウェア](https://www.bleepingcomputer.com/news/security/new-stormencryptor-ransomware-used-by-former-medusa-affiliate/) | 36.0 | 30.0 | 42.0 |
| [中国関連のハッカーがN-centralの脆弱性を悪用して新型StormEncryptorランサムウェアを展開、攻撃の可能性が高い](https://thehackernews.com/2026/08/china-linked-hackers-deploy-new.html) | 36.0 | 30.0 | 42.0 |
| [China関連の攻撃者が人気のサイバーセキュリティツールをランサムウェアの足がかりに変えているとMicrosoftが警告](https://therecord.media/china-hackers-ransomware-microsoft) | 36.0 | 30.0 | 42.0 |
| [DeadLockランサムウェア：Rust製暗号化ツールと分散型復旧インフラの分析](https://www.microsoft.com/en-us/security/blog/2026/08/10/deadlock-ransomware-breaking-down-a-rust-based-encryptor-with-decentralized-recovery-infrastructure/) | 30.0 | 30.0 | 42.0 |
| [Lazarus APTのIT人材を偽のDeFiスタートアップで雇う手口の続編、監視下にあるあなたの笑顔](https://any.run/cybersecurity-blog/lazarus-group-it-workers-investigation-part-two/) | 30.0 | 20.0 | 48.0 |
| [MetabaseのSQLインジェクション：実際の攻撃で悪用された事例](https://www.wiz.io/blog/inside-the-metabase-sqli-exploited-in-the-wild) | 29.0 | 20.0 | 43.0 |
| [CISA、SonicWall SMA1000の脆弱性がランサムウェア攻撃グループに悪用されていると警告](https://www.bleepingcomputer.com/news/security/cisa-sonicwall-sma1000-flaws-now-exploited-by-ransomware-gangs/) | 28.0 | 30.0 | 42.0 |
| [新しいPasskey攻撃で同期済み秘密鍵の回復やフィッシング耐性MFAの回避が可能に](https://thehackernews.com/2026/08/new-passkey-attacks-can-recover-synced.html) | 28.0 | 20.0 | 42.0 |
| [TrueConf Serverの脆弱性を悪用し、クライアントインストーラーをPhantomCoreに置き換える攻撃](https://thehackernews.com/2026/08/head-mare-exploits-trueconf-flaws-to.html) | 28.0 | 20.0 | 42.0 |
| [2026年第2四半期のIT脅威の進化：モバイル以外の統計](https://securelist.com/malware-report-q2-2026-pc-iot-statistics/120960/) | 28.0 | 20.0 | 42.0 |
| [Go言語ベースのmacOSマルウェアが暗号資産と機密情報を窃取](https://www.infosecurity-magazine.com/news/gobased-macos-malware-crypto-and/) | 28.0 | 20.0 | 42.0 |
| [Levi Strauss社へのサイバー攻撃で企業データが窃取される](https://www.securityweek.com/corporate-data-stolen-in-levi-strauss-cyberattack/) | 28.0 | 20.0 | 42.0 |
| [Weekly Recap: AIの暴走、Metabaseのゼロデイ、MCPのサプライチェーン攻撃、ルーターのバックドア](https://thehackernews.com/2026/08/weekly-recap-ai-goes-rogue-metabase-0.html) | 27.0 | 20.0 | 43.0 |
| [Microsoft、2026年IDC MarketScapeのエンタープライズ向けMDR/MXDRでリーダーに選出](https://www.microsoft.com/en-us/security/blog/2026/08/10/microsoft-named-a-leader-in-the-2026-idc-marketscape-for-mdr-mxdr-for-the-enterprise/) | 27.0 | 20.0 | 42.0 |
| [Claude Fable 5で生物学の質問が過剰に制限される問題を改善、誤検出を減らして「フォールバック」を約85％削減](https://gigazine.net/news/20260810-claude-fable-5-biology-safeguard/) | 27.0 | 20.0 | 42.0 |
| [Ciscoが警告したClamAVの高深刻度脆弱性と公開PoC](https://www.securityweek.com/cisco-warns-of-high-severity-clamav-vulnerabilities-with-public-poc/) | 26.0 | 38.0 | 42.0 |
| [OpenAIがChatGPT 5.6 Cyberを公開、ただし承認ユーザー限定](https://www.bleepingcomputer.com/news/security/openai-releases-chatgpt-56-cyber-but-its-only-for-approved-users/) | 25.0 | 20.0 | 42.0 |
| [AI開発の高速化におけるセキュリティ確保に関するウェビナーのご案内](https://thehackernews.com/2026/08/shipping-1050-more-code-watch-this.html) | 25.0 | 20.0 | 42.0 |
| [北朝鮮のスパイがローカルLLMを悪用してAIによる悪事を働いている](https://www.theregister.com/security/2026/08/10/north-korean-spies-are-running-local-llms-to-cause-ai-mischief/5285632) | 25.0 | 20.0 | 42.0 |
| [AI対応PAM：IDセキュリティソリューションが応答する時](https://www.security.com/product-insights/ai-ready-pam-when-your-identity-security-solution-talks-back) | 25.0 | 20.0 | 42.0 |
| [AIエージェントにクラス予約を頼んだら、ウェイトリストAPIをハッキングして順番を繰り上げた件](https://www.theregister.com/ai-and-ml/2026/08/10/gym-rat-asks-ai-agent-to-book-him-a-class-it-hacks-a-waitlist-api-to-bump-him-up-the-list/5285591) | 25.0 | 20.0 | 42.0 |
| [AtlassianのAIアシスタント「Rovo」に見つかった脆弱性](https://www.infosecurity-magazine.com/news/rovoblast-atlassian-rovo-url/) | 25.0 | 20.0 | 42.0 |
| [OpenAIの新モデルAstraに高まる自律型サイバー攻撃の懸念](https://www.securityweek.com/openais-upcoming-astra-model-raises-autonomous-cyberattack-concerns/) | 25.0 | 20.0 | 42.0 |
| [透明なAIエージェントが想像以上に重要な理由](https://cyberscoop.com/transparent-ai-agent-security-op-ed/) | 25.0 | 20.0 | 42.0 |
| [AIアクセラレータとネオクラウドのセキュリティ盲点を狙うStealthium](https://www.securityweek.com/stealthium-targets-security-blind-spots-in-ai-accelerators-and-neo-clouds/) | 25.0 | 20.0 | 42.0 |
| [認証情報だけでは不十分：AI時代のデバイス信頼](https://www.bleepingcomputer.com/news/security/when-credentials-are-no-longer-enough-device-trust-in-the-ai-era/) | 25.0 | 20.0 | 42.0 |
| [Poisoned Logsを使ってAIエージェントを悪用する「Ghostjacking」攻撃](https://www.securityweek.com/ghostjacking-attack-uses-poisoned-logs-to-turn-ai-agents-bad/) | 25.0 | 20.0 | 42.0 |
| [AIエージェントは信頼できるのか？新研究が示す「メモリポイズニング」で偽情報を「記憶」させられる巨大なセキュリティリスク](https://www.itpro.com/security/trust-your-ai-agents-new-research-shows-memory-poisoning-can-dupe-them-into-remembering-fake-information-and-its-a-huge-security-risk) | 25.0 | 20.0 | 42.0 |
| [AIエージェントの信頼されたアクセスを悪用してファイアウォール制御を回避する「Ghostjacking」](https://www.infosecurity-magazine.com/news/ghostjacking-ai-gents-access/) | 25.0 | 20.0 | 42.0 |
| [Claude Codeが自動モードを主導するようにした](https://www.theregister.com/ai-and-ml/2026/08/10/claude-code-puts-auto-mode-in-the-drivers-seat/5285326) | 25.0 | 20.0 | 42.0 |
| [Anthropic、Claude Codeの操作レビューをデフォルトでAIに委ねる方針を導入](https://www.helpnetsecurity.com/2026/08/10/anthropic-claude-code-auto-mode/) | 25.0 | 20.0 | 42.0 |
| [CISA、悪用確認済みのProgress LoadMasterの脆弱性に即時パッチ適用を呼びかけ](https://www.securityweek.com/cisa-urges-immediate-patching-of-exploited-progress-loadmaster-vulnerability/) | 24.0 | 38.0 | 42.0 |
| [攻撃者がソーシャルエンジニアリング攻撃でLevi'sを標的にする](https://www.theregister.com/security/2026/08/10/attackers-pick-levis-pockets-in-social-engineering-attack/5285401) | 22.0 | 20.0 | 42.0 |
| [島根県が管理する共同研究サイトが改ざん - 外部サイトへ誘導](https://www.security-next.com/188193) | 22.0 | 20.0 | 42.0 |
| [MSPがブラウザを新たなセキュリティ制御ポイントとして再考すべき理由](https://www.itpro.com/security/why-msps-should-rethink-the-browser-as-the-new-security-control-point) | 20.0 | 20.0 | 42.0 |
| [パッチのギャップ：防御者がチェックリストではなくチェーンで考えるべき理由](https://www.darkreading.com/cybersecurity-operations/patch-gap-defenders-chains-not-checklists) | 20.0 | 20.0 | 42.0 |
| [データの足跡を偽装して価格を下げる方法（Lock and Code S07E16）](https://www.malwarebytes.com/blog/podcast/2026/08/how-to-fake-a-data-trail-and-maybe-lower-prices-lock-and-code-s07e16) | 20.0 | 20.0 | 42.0 |
| [CorunaとDarkSwordのiOSエクスプロイトが世界的に拡散](https://www.darkreading.com/vulnerabilities-threats/coruna-darksword-ios-exploits-proliferate-globally) | 20.0 | 20.0 | 42.0 |
| [古いサイバー犯罪法がセキュリティ研究者を危険にさらす](https://www.darkreading.com/application-security/outdated-cybercrime-laws-security-researchers-risk) | 20.0 | 20.0 | 42.0 |
| [Sherlock Holmesは“OG”ソーシャルエンジニアだった](https://www.darkreading.com/cyber-risk/sherlock-holmes-was-the-og-social-engineer) | 20.0 | 20.0 | 42.0 |
| [ポーランドで数か月隠れていた2件目の熱電併給施設へのサイバー攻撃が判明](https://therecord.media/poland-uncovers-critical-infrastructure-attack-hidden) | 20.0 | 20.0 | 42.0 |
| [上院民主党議員、水道システムのサイバーセキュリティ強化に年間3億ドルを配分する法案を提出](https://therecord.media/senate-water-cybersecurity-legislation) | 20.0 | 20.0 | 42.0 |
| [誰でも詐欺師になれる新たなターンキーキット](https://www.malwarebytes.com/blog/scams/2026/08/new-turnkey-kit-makes-it-easy-for-anyone-to-become-a-scammer) | 20.0 | 20.0 | 42.0 |
| [The Comに関与した英国人男性、117人への虐待で有罪判決](https://cyberscoop.com/uk-justin-swaddle-the-com-sentenced/) | 20.0 | 20.0 | 42.0 |
| [市民社会の取り組みが地方の水道システム保護のためにサイバーセキュリティベンダーへ報酬を支払う](https://www.cybersecuritydive.com/news/water-cybersecurity-mdr-services-def-con-franklin/827449/) | 20.0 | 20.0 | 42.0 |
| [Steamのハードウェア配送業者へのサイバー攻撃で氏名・住所・注文情報が流出](https://www.helpnetsecurity.com/2026/08/10/valve-data-breach-ceva-logistics-steam-hardware/) | 20.0 | 20.0 | 42.0 |
| [WordPressプラグインが単一ファイルの変更なしで侵害された件](https://www.infosecurity-magazine.com/news/bdthemes-wordpress-poisoned-api/) | 20.0 | 20.0 | 42.0 |
| [8月10日の脅威インテリジェンスレポート](https://research.checkpoint.com/2026/10th-august-threat-intelligence-report/) | 20.0 | 20.0 | 42.0 |
| [Microsoft Entra ID、Windows HelloとmacOS PSSOユーザー向けの追加MFA認証を廃止](https://www.helpnetsecurity.com/2026/08/10/entra-id-windows-hello-macos-psso-standalone-mfa/) | 20.0 | 20.0 | 42.0 |
| [The Comのメンバーが恐喝と性的脅迫で実刑判決を受ける](https://www.bleepingcomputer.com/news/security/member-of-the-com-sent-to-prison-for-blackmail-sextortion/) | 20.0 | 20.0 | 42.0 |
| [Edge、古い拡張機能のサポート終了で人気のプライバシーツールに影響](https://www.malwarebytes.com/blog/news/2026/08/edge-is-dropping-older-extensions-affecting-popular-privacy-tools) | 20.0 | 20.0 | 42.0 |
| [Royal Navyのドローンが中国へデータ送信していた脆弱性調査で判明](https://www.theregister.com/edge-and-iot/2026/08/10/cyber-vulnerability-sweep-picks-up-royal-navy-drones-sending-data-to-china/5285430) | 20.0 | 20.0 | 42.0 |
| [LexisNexisがサーバー上の不審な活動を受けてサービスを停止](https://www.bleepingcomputer.com/news/security/lexisnexis-shuts-down-services-after-suspicious-activity-on-servers/) | 20.0 | 20.0 | 42.0 |
| [Valve、Steamハードウェア利用者にデータ漏えいを通知](https://www.bleepingcomputer.com/news/security/valve-notifies-steam-hardware-customers-of-a-data-breach/) | 20.0 | 20.0 | 42.0 |
| [ニュージャージー州とアラバマ州が水道関連のサイバー攻撃の標的に追加される](https://www.securityweek.com/new-jersey-alabama-join-states-targeted-in-water-cyberattacks/) | 20.0 | 20.0 | 42.0 |
| [新たなPrivate APNの悪用によりハッカーがポーランドの2番目のエネルギー施設を妨害](https://www.securityweek.com/novel-private-apn-pivot-let-hackers-sabotage-second-polish-energy-facility/) | 20.0 | 20.0 | 42.0 |
| [2026年第2四半期のIT脅威動向：モバイル統計](https://securelist.com/malware-report-q2-2026-mobile-statistics/120948/) | 20.0 | 20.0 | 42.0 |
| [Swiss authorities、SharePointの認証情報漏えい懸念の中で冷静な対応を呼びかけ](https://www.itpro.com/security/data-breaches/swiss-authorities-urge-calm-amid-fears-over-sharepoint-credential-leak) | 20.0 | 20.0 | 42.0 |
| [米国、イランの60億ドル規模の暗号資産取引所Shelbitに制裁](https://www.infosecurity-magazine.com/news/us-sanctions-iranian-6bn-crypto/) | 20.0 | 20.0 | 42.0 |

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
