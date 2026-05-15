# 📡 サイレーダー 2026-05-15 17:00 JST 試作版

このレポートは、2026-05-15 11:00 JST〜2026-05-15 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 138
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 3
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-20182: CISA KEV catalog addition](#topic-4945) | 88.0 | 84.0 | 67.0 | GitHub | 直近掲載済み・再掲抑制 |
| 2 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 54.0 | 82.0 | 81.0 | GitHub | 直近掲載済み・再掲抑制 |
| 3 | [NGINXでリモートコード実行の脆弱性が発見される、影響を受けるバージョンはこれ](#topic-4593) | 34.0 | 49.0 | 55.0 | GitHub | 直近掲載済み・再掲抑制 |
| 4 | [\[Guest Diary\] New Malware Libraries means New Signatures, (Fri, May 15th)](#topic-5333) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-5333"></a>

### 1. [Guest Diary] New Malware Libraries means New Signatures, (Fri, May 15th)

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>マルウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

SANS Internet Storm Centerの投稿として、新しいマルウェアライブラリの登場により新たなシグネチャ作成が必要になる、という趣旨の話題が取り上げられています。
公開情報上は詳細な攻撃キャンペーンや被害規模は確認できず、技術コミュニティでの反応は強くないものの、脅威インテリジェンス上の関心事として扱われています。
マルウェア側の実装が変わると、既存の検知ルールやシグネチャが追随を迫られるため、運用側の更新遅れが検知漏れにつながる可能性があります。
新しい検知材料の把握は、SOCや脅威ハンティングの精度維持に直結します。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 既存の検知ルールやシグネチャで、新しい亜種や派生に対する追従状況を確認する。
- EDR/AV/IDSの検知ログを見直し、類似挙動の未検知がないか点検する。
- 脅威情報の更新頻度を高め、ベンダー提供のルールやフィードの適用状況を確認する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [[Guest Diary]  New Malware Libraries means New Signatures, (Fri, May 15th)](https://isc.sans.edu/diary/rss/32986) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-4945"></a>

### 1. CVE-2026-20182: CISA KEV catalog addition

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>認証バイパス</nobr> / <nobr>ゼロデイ</nobr> / <nobr>KEV</nobr> / <nobr>IoC</nobr> / <nobr>PoC</nobr> / <nobr>政策・規制</nobr> / <nobr>防御・運用</nobr> / <nobr>国家支援</nobr> |
| <nobr>温度状態</nobr> | 高温 |
| <nobr>温度感</nobr> | 88.0 |
| <nobr>実務影響</nobr> | 84.0 |
| <nobr>確度</nobr> | 67.0 |

#### 概要

CISAは、Cisco Catalyst SD-WAN Controllerに関する認証バイパスの脆弱性CVE-2026-20182をKEVカタログに追加しました。
Ciscoはこの脆弱性への修正を公表しており、限定的な攻撃で悪用されたと説明しています。
KEV入りは、実際に悪用が確認されている、またはその可能性が高い脆弱性として優先対応が求められることを意味します。
SD-WAN基盤はネットワーク制御の要所であるため、影響範囲が大きくなりやすい点が注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 7 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 中。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 公開PoC・検証コード言及あり。
- 公開PoC/Exploitコード: 確認あり。
- 直接PoCリンク: 掲載しません。
- 確認方針: NVD、ベンダー公式、公的機関、信頼できる技術分析を優先し、GitHub等のコードは防御・検証目的で別途確認します。

#### 担当者向け確認ポイント

- 該当するCisco Catalyst SD-WAN Controller／Managerの利用有無を確認し、ベンダーの修正情報を基に早急に更新を適用する。
- KEV対象として優先度を上げ、外部公開状況や管理系インターフェースへの到達性を見直す。
- IOCや監視強化の案内があれば、管理者権限の異常操作や設定変更の兆候を重点的に点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20182 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20182](https://nvd.nist.gov/vuln/detail/CVE-2026-20182) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Patches Another SD-WAN Zero-Day, the Sixth Exploited in 2026](https://securityweek.com/cisco-patches-another-sd-wan-zero-day-the-sixth-exploited-in-2026) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds Cisco SD-WAN CVE-2026-20182 to KEV After Admin Access Exploits](https://thehackernews.com/2026/05/cisa-adds-cisco-sd-wan-cve-2026-20182.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of new critical SD-WAN flaw exploited in zero-day attacks](https://bleepingcomputer.com/news/security/cisco-warns-of-new-critical-sd-wan-flaw-exploited-in-zero-day-attacks) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller Auth Bypass Actively Exploited to Gain Admin Ac](https://thehackernews.com/2026/05/cisco-catalyst-sd-wan-controller-auth.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Ongoing exploitation of Cisco Catalyst SD-WAN vulnerabilities](https://blog.talosintelligence.com/sd-wan-ongoing-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>公的・一次情報</nobr> | [Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-rpa2-v69WY2SW) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-20182: Critical authentication bypass in Cisco Catalyst SD-WAN Controll](https://rapid7.com/blog/post/ve-cve-2026-20182-critical-authentication-bypass-cisco-catalyst-sd-wan-controller-fixed) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 中。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。
- 継続観測: 継続。

---

<a id="topic-12"></a>

### 2. Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>Windows</nobr> / <nobr>権限昇格</nobr> / <nobr>TTP</nobr> / <nobr>脆弱性</nobr> / <nobr>KEV</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 54.0 |
| <nobr>実務影響</nobr> | 82.0 |
| <nobr>確度</nobr> | 81.0 |

#### 概要

CVE-2025-60710は、Microsoft WindowsのTaskhost関連のタスク処理におけるローカル権限昇格の脆弱性として扱われています。
CISAのKnown Exploited Vulnerabilitiesに含まれており、公開PoCや検証コードへの言及もあるため、影響確認の優先度が高い案件です。
権限昇格の問題は、端末内での被害拡大や管理者権限の奪取につながる可能性があるため注目されます。
KEV掲載は、実際に悪用されている、または悪用が懸念される脆弱性として早急な対応が求められる目安になります。

#### CISA KEV詳細

- **CVE**: CVE-2025-60710
- **Vendor / Project**: Microsoft
- **Product**: Windows
- **Vulnerability Name**: Microsoft Windows Link Following Vulnerability
- **Date Added**: 2026-04-13
- **Due Date**: 2026-04-27
- **Known Ransomware Use**: Unknown

**Required Action**

> Apply mitigations per vendor instructions, follow applicable BOD 22-01 guidance for cloud services, or discontinue use of the product if mitigations are unavailable.

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- CISA KEV関連。
- 公開PoC・検証コード言及あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- 公開PoCにより再現・悪用可能性が上がる。
- 権限昇格系。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 公開PoC・検証コード言及あり。
- 公開PoC/Exploitコード: 確認あり。
- 直接PoCリンク: 掲載しません。
- 確認方針: NVD、ベンダー公式、公的機関、信頼できる技術分析を優先し、GitHub等のコードは防御・検証目的で別途確認します。

#### 担当者向け確認ポイント

- Windows環境でCVE-2025-60710の影響有無を確認し、関連する更新プログラムの適用状況を点検する。
- Taskhostを含むタスク関連の挙動や、通常と異なる権限昇格の兆候がないかを監視する。
- 社内の優先度付けでは、KEV掲載の有無と公開PoCの存在を踏まえて高めに扱う。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-60710 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 影響ベンダー | 1.00 |
| 製品 | Windows | 影響製品 | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-60710](https://nvd.nist.gov/vuln/detail/CVE-2025-60710) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>公的機関</nobr> | [CISA KEV: CVE-2025-60710](https://www.cisa.gov/known-exploited-vulnerabilities-catalog?field_cve=CVE-2025-60710) | <nobr>KEV掲載内容、Date Added、Due Date、Required Action</nobr> |
| <nobr>公的機関データ</nobr> | [CISA KEV JSON](https://www.cisa.gov/sites/default/files/feeds/known_exploited_vulnerabilities.json) | <nobr>CISA公式の機械可読データ。CVE IDで検索して確認</nobr> |
| <nobr>出典</nobr> | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](https://github.com/Wh04m1001/CVE-2025-60710) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。
- 継続観測: 継続。

---

<a id="topic-4593"></a>

### 3. NGINXでリモートコード実行の脆弱性が発見される、影響を受けるバージョンはこれ

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>RCE</nobr> / <nobr>CVE</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 34.0 |
| <nobr>実務影響</nobr> | 49.0 |
| <nobr>確度</nobr> | 55.0 |

#### 概要

NGINXのngx_http_rewrite_moduleに、CVE-2026-42945として追跡される深刻な脆弱性が公表されました。
報道では、ヒープバッファオーバーフローによりリモートコード実行につながる可能性があるとされ、影響範囲はNGINX Open SourceおよびNGINX Plusに及ぶ可能性があります。
Webサーバー基盤として広く使われる製品のため、該当環境がある場合は優先度高く確認すべき話題です。
技術詳細や再現情報が出ていることで、ベンダー告知や利用環境の影響確認が進みやすい点も注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 技術詳細・再現情報あり。
- 技術者コミュニティ反応: 弱。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 技術詳細により影響確認が進みやすい。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 技術詳細・再現情報あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 技術詳細、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 利用中のNGINXの版数と該当モジュールの利用有無を確認する。
- ベンダーの修正版・緩和策の案内を待たずに、適用可能な更新計画を前倒しで検討する。
- Webサーバーの異常終了や不審な挙動など、関連ログの監視を強化する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-42945 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-42945](https://nvd.nist.gov/vuln/detail/CVE-2026-42945) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [NGINXでリモートコード実行の脆弱性が発見される、影響を受けるバージョンはこれ](https://gigazine.net/news/20260515-nginx-remote-code-execution) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [18-Year-Old NGINX Rewrite Module Flaw Enables Unauthenticated RCE](https://thehackernews.com/2026/05/18-year-old-nginx-rewrite-module-flaw.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 反応あり。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 技術詳細・再現情報あり。
- 継続観測: 継続。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [アップルのiPadOS等の複数製品における複数の脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015732.html) | 27.0 | 23.0 | 43.0 |
| [アップルのiPadOS等の複数製品における整数オーバーフローの脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015734.html) | 27.0 | 23.0 | 43.0 |
| [アップルのiPadOS等の複数製品におけるNULL ポインタデリファレンスに関する脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015722.html) | 27.0 | 23.0 | 43.0 |
| [アップルのiPadOS等の複数製品におけるリソースの枯渇に関する脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015728.html) | 27.0 | 23.0 | 43.0 |
| [アップルのiPadOS等の複数製品における境界外書き込みに関する脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015726.html) | 27.0 | 23.0 | 43.0 |
| [アニメ・イラストに強い画像生成AI「Anima」の正式版がついに登場、タグ・自然言語両対応でSDXLやIllustrious系モデルが動作するPCなら余裕でローカル実行可能](https://gigazine.net/news/20260515-anima-image-generation-ai) | 27.0 | 20.0 | 42.0 |
| [動画生成AIのRunwayが日本に拠点を開設](https://gigazine.net/news/20260515-runway-comes-to-japan) | 27.0 | 20.0 | 42.0 |
| [画像生成AI「FLUX.2」によるアウトペインティングに特化した「FLUX Outpainting」が登場、実際に試してみた](https://gigazine.net/news/20260515-flux-outpainting) | 27.0 | 20.0 | 42.0 |
| [パナソニックHD、2032年への成長戦略--AIインフラに5000億円投資へ](https://japan.zdnet.com/article/35247569) | 26.0 | 20.0 | 42.0 |
| [AIエージェントをJava開発の“最強のチームメイト”に変えるイベント 「Microsoft Java Day」が5/28開催](https://ascii.jp/elem/000/004/401/4401900?rss=) | 26.0 | 20.0 | 42.0 |
| [「客先常駐」も、OpenAIがAI導入の新会社 問われるIT部門やSIerの存在意義](https://xtech.nikkei.com/atcl/nxt/column/18/00001/11746) | 26.0 | 20.0 | 42.0 |
| [Keycardが開発者に自律型AIエージェントのスコープ付きアクセスによる安全な保護を提供](https://helpnetsecurity.com/2026/05/15/keycard-for-multi-agent-apps) | 25.0 | 20.0 | 42.0 |
| [AI監視のパラドックス：その投資は見合うのか？](https://helpnetsecurity.com/2026/05/15/ai-workforce-impact-report) | 25.0 | 20.0 | 42.0 |
| [「Exchange Server」に脆弱性 - すでに悪用を確認、パッチは準備中](https://security-next.com/184486) | 24.0 | 20.0 | 43.0 |
| [アドビのAdobe Commerce等の複数製品におけるクロスサイトスクリプティングの脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015686.html) | 23.0 | 26.0 | 42.0 |
| [アップルのmacOSにおける複数の脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015725.html) | 23.0 | 20.0 | 43.0 |
| [The Go Projectのimageにおける不特定の脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015705.html) | 23.0 | 20.0 | 43.0 |
| [The Go Projectのimageにおける制限またはスロットリング無しのリソースの割り当てに関する脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015706.html) | 23.0 | 20.0 | 43.0 |
| [Pengutronix e.K.のbareboxにおける整数オーバーフローの脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015681.html) | 23.0 | 20.0 | 43.0 |
| [Pengutronix e.K.のbareboxにおける境界外読み取りに関する脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015683.html) | 23.0 | 20.0 | 43.0 |
| [Pengutronix e.K.のbareboxにおける無限ループに関する脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015682.html) | 23.0 | 20.0 | 43.0 |
| [PHPOfficeのPhpSpreadsheetにおける制限またはスロットリング無しのリソースの割り当てに関する脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015661.html) | 23.0 | 20.0 | 43.0 |
| [ZTEのZX297520V3 ファームウェアにおける境界外書き込みに関する脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015669.html) | 23.0 | 20.0 | 43.0 |
| [The Go ProjectのGoにおける不特定の脆弱性](https://jvndb.jvn.jp/ja/contents/2026/JVNDB-2026-015674.html) | 23.0 | 20.0 | 43.0 |

---

## 📊 スコアの見方

| <nobr>指標</nobr> | 意味 |
|---|---|
| <nobr>温度状態</nobr> | 話題のライフサイクルを示す補助ラベルです。例: 低温、継続監視、温度上昇中、高温、冷却中。 |
| <nobr>温度感</nobr> | 話題として今どれだけ注目・拡散・更新されているかを示します。 |
| <nobr>実務影響</nobr> | 対象組織・担当者にとって、対応優先度や被害可能性がどれだけ大きいかを示します。 |
| <nobr>確度</nobr> | 公的機関、ベンダー公式、複数ソース、CVE/KEV、一次資料などにより、情報をどれだけ確認できているかを示します。事件報道系は、複数報道があっても司法文書・当局発表などの一次資料が弱い場合、脆弱性KEV系より低く出ることがあります。 |

スコアは、公開情報から抽出した特徴量と事前定義した重み付けに基づく参考指標です。詳しい算出方針は [スコアリング方針](../docs/scoring.md) を参照してください。

## 🔒 公開しない内部情報について

サイレーダーでは、温度感の補助シグナルとして、公的機関・ベンダー公式・信頼できる報道機関・技術者コミュニティ・国内外の公開反応などを利用します。

これらのシグナルは、一次情報、報道波及、技術者反応、開発者反応、PoC・悪用観測などに分けて評価します。

ただし、ランキング操作、スパム的誘導、監視回避を防ぐため、個別の監視対象、取得手段、検索条件、評価対象サービス名、内部的な重み付けやしきい値は公開しません。

また、公開反応の多さだけで掲載順位を決めることはありません。重要度の判定では、ベンダー公式情報、公的機関、一次資料、信頼できる技術分析、実務影響を優先します。

## ⚠️ 注意事項

このレポートは、収集・観測できた公開情報をもとにした参考情報です。完全性、正確性、即時性を保証するものではありません。

重要な判断を行う場合は、必ずベンダー公式情報、公的機関、一次情報を確認してください。

サイレーダーは、広告・スポンサー・企業関係に基づいて掲載順位や温度感スコアを変更しません。
