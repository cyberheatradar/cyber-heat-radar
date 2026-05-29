# 📡 サイレーダー 2026-05-30 05:00 JST

このレポートは、2026-05-29 17:00 JST〜2026-05-30 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 181
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Attackers Use LLM Agent for Post-Exploitation After Marimo CVE-2026-39987 Exploit](#topic-600) | 48.0 | 96.0 | 84.0 | 音声 | 温度感上位枠 |
| 2 | [CVE-2026-0257: CISA KEV catalog addition](#topic-4247) | 43.0 | 67.0 | 59.0 | 音声 | 温度感上位枠 |
| 3 | [Gogs Zero-Day Exposes Servers to Remote Code Execution](#topic-12552) | 41.0 | 56.0 | 43.0 | 音声 | 温度感上位枠 |
| 4 | [Microsoft calls zero-day releases ‘never justifiable’ as researcher threatens to drop more](#topic-12547) | 37.0 | 38.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [AI-Generated npm Malware Leaks Its Own GitHub Token](#topic-12382) | 33.0 | 45.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [ChatGPT share links abused to host fake outage pages to deliver malware](#topic-12533) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [New Russian-Linked GREYVIBE Targets Ukraine with AI-Powered Cyberattacks](#topic-12557) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 8 | [New infostealer reaches enterprise devices through FortiClient EMS vulnerability](#topic-955) | 31.0 | 78.0 | 83.0 | GitHub | 音声枠上限によりGitHubのみ |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-600"></a>

### 1. Attackers Use LLM Agent for Post-Exploitation After Marimo CVE-2026-39987 Exploit

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>KEV</nobr> / <nobr>CVE</nobr> / <nobr>RCE</nobr> / <nobr>AI</nobr> / <nobr>脅威アクター</nobr> / <nobr>TTP</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 再燃 |
| <nobr>温度感</nobr> | 48.0 |
| <nobr>実務影響</nobr> | 96.0 |
| <nobr>確度</nobr> | 84.0 |

#### 概要

CISAは、Marimoに関するCVE-2026-39987をKnown Exploited Vulnerabilities（KEV）Catalogに追加し、実際の悪用が確認された脆弱性として扱っています。
公開情報では、初期侵入後にLLMエージェントがポストエクスプロイテーションに使われた可能性が示されていますが、詳細な手口は慎重に見る必要があります。
KEV入りは、当該脆弱性が机上のリスクではなく、優先的な対応が必要な状態であることを示します。
特にインターネットから到達可能なサービスでは、侵害後の横展開や情報窃取につながるおそれがあるため注目されています。

#### CISA KEV詳細

- **CVE**: CVE-2026-39987
- **Vendor / Project**: Marimo
- **Product**: Marimo
- **Vulnerability Name**: Marimo Remote Code Execution Vulnerability
- **Date Added**: 2026-04-23
- **Due Date**: 2026-05-07
- **Known Ransomware Use**: Unknown

**Required Action**

> Apply mitigations per vendor instructions, follow applicable BOD 22-01 guidance for cloud services, or discontinue use of the product if mitigations are unavailable.

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- CISA KEV関連。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
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

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Marimoを利用している環境は、CVE-2026-39987の適用状況と公開範囲を早急に確認する。
- インターネット露出した管理画面やノートブック環境の監視を強め、異常なログインや不審な操作の痕跡を点検する。
- 侵害が疑われる場合は、認証情報の再発行や関連アカウントの点検を含め、インシデント対応を優先する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-39987 | 主要CVE | 1.00 |
| ベンダー | Marimo | 影響ベンダー | 1.00 |
| 製品 | Marimo | 影響製品 | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-39987](https://nvd.nist.gov/vuln/detail/CVE-2026-39987) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>公的機関</nobr> | [CISA KEV: CVE-2026-39987](https://www.cisa.gov/known-exploited-vulnerabilities-catalog?field_cve=CVE-2026-39987) | <nobr>KEV掲載内容、Date Added、Due Date、Required Action</nobr> |
| <nobr>公的機関データ</nobr> | [CISA KEV JSON](https://www.cisa.gov/sites/default/files/feeds/known_exploited_vulnerabilities.json) | <nobr>CISA公式の機械可読データ。CVE IDで検索して確認</nobr> |
| <nobr>出典</nobr> | [Attackers Use LLM Agent for Post-Exploitation After Marimo CVE-2026-39987 Exploi](https://thehackernews.com/2026/05/attackers-use-llm-agent-for-post.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/04/23/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-4247"></a>

### 2. CVE-2026-0257: CISA KEV catalog addition

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>IoC</nobr> / <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>防御・運用</nobr> / <nobr>脅威アクター</nobr> / <nobr>KEV</nobr> / <nobr>認証バイパス</nobr> / <nobr>Windows</nobr> / <nobr>Linux</nobr> / <nobr>政策・規制</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 43.0 |
| <nobr>実務影響</nobr> | 67.0 |
| <nobr>確度</nobr> | 59.0 |

#### 概要

CISA は、Palo Alto Networks の PAN-OS / Prisma Access に影響する CVE-2026-0257 を Known Exploited Vulnerabilities（KEV）カタログに追加しました。
公開情報では、GlobalProtect 関連の認証回避として説明されており、条件がそろった環境では不正な VPN 接続につながる可能性があるとされています。
KEV 追加は、実際の悪用が確認された脆弱性として優先対応が求められることを意味します。
境界機器や VPN 装置に関わるため、影響範囲が広がると社内ネットワークへの入口になり得ます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 技術詳細・再現情報あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 技術詳細により影響確認が進みやすい。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 技術詳細・悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 技術詳細、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 対象製品と影響バージョンを確認し、ベンダーが案内する修正済み版へ速やかに更新する。
- 認証オーバーライド機能の有効化状況と、証明書の使い回し有無を点検する。
- 更新までの間は、関連ログを監視し、想定外の GlobalProtect 認証成功や不審な VPN 接続の有無を確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-0257 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |
| ベンダー | Palo Alto | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-0257](https://nvd.nist.gov/vuln/detail/CVE-2026-0257) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Rapid7 Observed Exploitation of PAN-OS GlobalProtect Authentication Bypass Vulne](https://www.rapid7.com/blog/post/etr-rapid7-observed-exploitation-of-pan-os-globalprotect-authentication-bypass-vulnerability-cve-2026-0257) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/05/29/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0257 PAN-OS: GlobalProtect Authentication Bypass Vulnerabilities (Sever](https://security.paloaltonetworks.com/CVE-2026-0257) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 技術詳細・悪用観測あり。

---

<a id="topic-12552"></a>

### 3. Gogs Zero-Day Exposes Servers to Remote Code Execution

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>RCE</nobr> / <nobr>ゼロデイ</nobr> / <nobr>CVE</nobr> / <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 41.0 |
| <nobr>実務影響</nobr> | 56.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

Gogsにゼロデイ脆弱性が見つかり、認証済み攻撃者によってリモートコード実行につながる可能性があると報じられています。
CVSS 9.4の高深刻度とされ、引数インジェクションの問題として説明されています。対象がGitサービスであるため、組織のソースコード管理基盤に影響し得ます。
認証後の悪用が想定されるため、単純な外部公開対策だけでは不十分な場合があります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Gogsの利用有無と影響範囲を確認し、該当バージョンの更新情報や修正版の有無を確認する。
- 認証済み操作でも不審なプルリクエストやブランチ名など、通常と異なる入力の監視を強化する。
- Gitリポジトリや連携サービスへのアクセス権限を見直し、必要最小限の権限に絞る。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Gogs Zero-Day Exposes Servers to Remote Code Execution](https://www.securityweek.com/gogs-zero-day-exposes-servers-to-remote-code-execution/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。

---

<a id="topic-12547"></a>

### 4. Microsoft calls zero-day releases ‘never justifiable’ as researcher threatens to drop more

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ゼロデイ</nobr> / <nobr>PoC</nobr> / <nobr>脆弱性</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 37.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Microsoftをめぐり、研究者がゼロデイ脆弱性の公開をさらに行う可能性を示唆していることが話題になっています。
公開された各脆弱性には動作確認用のコードが添えられており、攻撃者と防御側の双方にすぐ利用可能な状態だったとされています。
ゼロデイの公開は、修正前の脆弱性が広く認識されることで防御と悪用の両面に影響しやすく、関係製品の利用者にとって注意が必要です。
ベンダーと研究者の対応を含め、今後の公開範囲や修正状況が注目されます。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Microsoft関連製品の修正情報と更新適用状況を確認する。
- 外部公開された検証コードや解説記事に過度に依存せず、影響有無を自組織で点検する。
- 関連アカウントや資産の監視を強め、異常な挙動がないか確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft calls zero-day releases ‘never justifiable’ as researcher threatens to](https://therecord.media/microsoft-calls-zero-day-releases-never-justifiable-as-researcher-threatens-more) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-12382"></a>

### 5. AI-Generated npm Malware Leaks Its Own GitHub Token

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>マルウェア</nobr> / <nobr>AI</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 温度上昇中 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 45.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

AIで生成されたとみられるnpm向けのマルウェアが、自身のGitHubトークンを漏えいさせたと報じられています。
結果として、攻撃者側の運用痕跡や関連アカウントが露出した可能性がある点が注目されています。
npmのような開発者向けエコシステムで起きるサプライチェーン系の不正パッケージは、利用者やCI/CD環境に広く影響し得ます。
さらに、攻撃者側の設定ミスや痕跡露出は、調査・検知の手がかりになり得ます。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 依存パッケージの更新時は、公開レピュテーションやメンテナ情報だけでなく、異常な挙動や不自然な権限要求がないかを確認する。
- CI/CDや開発端末で使うトークンは最小権限にし、漏えい前提で定期ローテーションと失効手順を整備する。
- npm導入パッケージの監査、ソースコードレビュー、SBOM/ロックファイル管理を徹底し、不審な新規パッケージの混入を早期に検知する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [AI-Generated npm Malware Leaks Its Own GitHub Token](https://www.infosecurity-magazine.com/news/ai-npm-malware-leaks-github-token/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-12533"></a>

### 6. ChatGPT share links abused to host fake outage pages to deliver malware

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>AI</nobr> / <nobr>マルウェア</nobr> / <nobr>脅威アクター</nobr> |
| <nobr>分類理由</nobr> | AI×Security枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

ChatGPTのコンテンツ共有機能を悪用し、OpenAIの障害案内を装った偽ページへ誘導する事例が報告されています。
そこで、ChatGPTデスクトップアプリを装ったマルウェアのダウンロードに誘導する流れが確認されたとされています。
生成AIサービスの正規機能が悪用されると、利用者が「信頼できる共有リンク」と誤認しやすくなります。
AI関連サービスを起点にしたフィッシングやマルウェア誘導として、注意喚起の対象になりやすい事案です。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 共有リンク経由でも内容を鵜呑みにせず、障害情報は公式の告知経路で確認する。
- 社内で配布するアプリは、提供元・署名・入手元を確認し、未確認のインストーラを実行しない。
- AIサービスの共有機能を使った誘導があり得る前提で、URLの見え方だけで信頼しない運用を徹底する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ai_model_or_project | ChatGPT | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [ChatGPT share links abused to host fake outage pages to deliver malware](https://www.bleepingcomputer.com/news/security/chatgpt-share-links-abused-to-host-fake-outage-pages-to-deliver-malware/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="topic-12557"></a>

### 7. New Russian-Linked GREYVIBE Targets Ukraine with AI-Powered Cyberattacks

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>国家支援</nobr> / <nobr>地政学・サイバー紛争</nobr> / <nobr>AI</nobr> / <nobr>脅威アクター</nobr> |
| <nobr>分類理由</nobr> | AI×Security枠 |
| <nobr>温度状態</nobr> | 初出 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

WithSecureは、少なくとも2025年8月以降、ウクライナおよび関連組織を継続的に狙う新たな脅威アクター「GREYVIBE」を確認したとしています。
報道では、同グループはロシア語圏の活動者とみられ、AIを用いた攻撃手法が使われているとされていますが、詳細は公開情報の範囲での評価です。
地政学的な緊張が続く中で、AIを悪用した攻撃の実例として注目されています。
国家関与が疑われる脅威の動向は、地域関連組織だけでなく、支援先や周辺サプライチェーンにも影響しうるためです。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- ウクライナ関連の取引先・委託先・支援先を含め、関連組織の監視とアラート設定を見直す。
- AIを使った不自然な文面や誘導が含まれる可能性を前提に、メール・認証・端末操作の確認手順を強化する。
- 脅威インテリジェンスの更新を定期的に確認し、同種のキャンペーンが自組織に波及していないか点検する。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [New Russian-Linked GREYVIBE Targets Ukraine with AI-Powered Cyberattacks](https://thehackernews.com/2026/05/new-russian-linked-greyvibe-targets.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-955"></a>

### 1. New infostealer reaches enterprise devices through FortiClient EMS vulnerability

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>マルウェア</nobr> / <nobr>KEV</nobr> / <nobr>認証バイパス</nobr> |
| <nobr>温度状態</nobr> | 冷却中 |
| <nobr>温度感</nobr> | 31.0 |
| <nobr>実務影響</nobr> | 78.0 |
| <nobr>確度</nobr> | 83.0 |

#### 概要

CVE-2026-35616 は、Fortinet FortiClient EMS に関するCISA KEV掲載済みの脆弱性です。
CISA KEV上の名称は「Fortinet FortiClient EMS Improper Access Control Vulnerability」です。
CISA KEVでは実環境で悪用が確認された脆弱性として扱われています。
KEV掲載済みであるため、該当製品を利用している組織では、ベンダー公式情報とCISA KEVのRequired Actionを確認する価値があります。

#### CISA KEV詳細

- **CVE**: CVE-2026-35616
- **Vendor / Project**: Fortinet
- **Product**: FortiClient EMS
- **Vulnerability Name**: Fortinet FortiClient EMS Improper Access Control Vulnerability
- **Date Added**: 2026-04-06
- **Due Date**: 2026-04-09
- **Known Ransomware Use**: Unknown

**Required Action**

> Apply mitigations per vendor instructions, follow applicable BOD 22-01 guidance for cloud services, or discontinue use of the product if mitigations are unavailable.

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- CISA KEV関連。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用済み脆弱性として優先確認が必要。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- 公的機関情報あり。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 自組織で対象製品・関連資産を利用しているか確認する。
- ベンダー公式情報または公的機関情報を優先確認する。
- 対象バージョンか確認する。
- 修正版・緩和策の適用状況を確認する。
- インターネット露出の有無を確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-35616 | 主要CVE | 1.00 |
| ベンダー | Fortinet | 影響ベンダー | 1.00 |
| 製品 | FortiClient EMS | 影響製品 | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-35616](https://nvd.nist.gov/vuln/detail/CVE-2026-35616) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>公的機関</nobr> | [CISA KEV: CVE-2026-35616](https://www.cisa.gov/known-exploited-vulnerabilities-catalog?field_cve=CVE-2026-35616) | <nobr>KEV掲載内容、Date Added、Due Date、Required Action</nobr> |
| <nobr>公的機関データ</nobr> | [CISA KEV JSON](https://www.cisa.gov/sites/default/files/feeds/known_exploited_vulnerabilities.json) | <nobr>CISA公式の機械可読データ。CVE IDで検索して確認</nobr> |
| <nobr>出典</nobr> | [New infostealer reaches enterprise devices through FortiClient EMS vulnerability](https://www.helpnetsecurity.com/2026/05/29/forticlient-ems-vulnerability-infostealer/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers exploit FortiClient EMS flaw to push infostealer malware](https://www.bleepingcomputer.com/news/security/hackers-exploit-forticlient-ems-flaw-to-push-infostealer-malware/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [Lazarus、メモリ常駐型RemotePE RATで金融スパイ活動を拡大](https://blog.polyswarm.io/lazarus-expands-financial-espionage-operations-with-memory-resident-remotepe-rat) | 28.0 | 20.0 | 42.0 |
| [5ドルの攻撃からボットネット駆動のプラットフォームまで：DDoS as a Service市場の内実](https://www.bleepingcomputer.com/news/security/from-5-attacks-to-botnet-powered-platforms-inside-the-ddos-as-a-service-market/) | 28.0 | 20.0 | 42.0 |
| [オランダ政府、1700万台の感染端末を持つマルウェアボットネットを阻止](https://www.bleepingcomputer.com/news/security/dutch-govt-disrupts-malware-botnet-with-17-million-infected-devices/) | 28.0 | 20.0 | 42.0 |
| [オランダ警察、1700万台のデバイスで構成されたボットネットを摘発](https://www.helpnetsecurity.com/2026/05/29/dutch-police-disrupts-botnet-composed-of-17-million-devices/) | 28.0 | 20.0 | 42.0 |
| [Silent Ransom Groupが対面でIT担当者を装いシステム侵害](https://www.infosecurity-magazine.com/news/silent-ransom-group-it/) | 28.0 | 20.0 | 42.0 |
| [LinkedInを装ったフィッシング、AdobeのA/Bテスト基盤を悪用](https://www.helpnetsecurity.com/2026/05/29/linkedin-themed-phishing-adobe-a-b-testing-platform/) | 28.0 | 20.0 | 42.0 |
| [中国系ハッカーがイラン戦争を悪用し海運・エネルギー企業を標的にする](https://www.infosecurity-magazine.com/news/chinese-hackers-exploit-iran-war/) | 28.0 | 20.0 | 42.0 |
| [甘過ぎた“経営陣のAIリスク認識” 8割は「AI利用を可視化」と回答、なのに未承認AIが拡大](https://atmarkit.itmedia.co.jp/ait/articles/2605/29/news143.html) | 26.0 | 20.0 | 42.0 |
| [ChatGPTのWeb要約機能に脆弱性、フィッシングの新たな攻撃面に](https://thehackernews.com/2026/05/chatgphish-vulnerability-turns-chatgpt.html) | 25.0 | 20.0 | 42.0 |
| [Microsoft 365 Copilotの再設計で文脈と操作を1つのワークスペースに統合](https://www.helpnetsecurity.com/2026/05/29/microsoft-365-copilot-redesign/) | 25.0 | 20.0 | 42.0 |
| [Chrome 148アップデートで151件の脆弱性を修正](https://www.securityweek.com/chrome-148-update-patches-151-vulnerabilities/) | 24.0 | 38.0 | 42.0 |
| [Microsoft、2026年Gartner® Magic Quadrant™でエンドポイント保護のリーダーに選出](https://www.microsoft.com/en-us/security/blog/2026/05/29/microsoft-is-named-a-leader-in-the-2026-gartner-magic-quadrant-for-endpoint-protection/) | 22.0 | 20.0 | 42.0 |
| [Oracleが補完パッチ、5製品35件の脆弱性を修正 - クリティカル11件](https://www.security-next.com/185192) | 22.0 | 20.0 | 42.0 |
| [Windowsのゼロデイ脆弱性を投稿したセキュリティ研究者が「Microsoftの報復でGitHubから追放された」と主張](https://gigazine.net/news/20260529-nightmare-eclipse-github-banned/) | 22.0 | 20.0 | 42.0 |
| [日本政府と主要金融機関、OpenAI新モデルのアクセス権を取得 サイバー対策強化へ](https://www.itmedia.co.jp/news/articles/2605/29/news144.html) | 21.0 | 20.0 | 42.0 |
| [Microsoft、事前共有なしのゼロデイ脆弱性公表を批判 バグハンターと対立](https://www.itmedia.co.jp/news/articles/2605/29/news123.html) | 21.0 | 20.0 | 42.0 |
| [CISAがセキュリティチームにソフトウェア開発への侵害有無の確認を呼びかける](https://www.cybersecuritydive.com/news/cisa-security-software-supply-chain-compromises-GitHub/821487/) | 20.0 | 45.0 | 42.0 |
| [CVE-2026-46178 RDMA/mlx4: mlx4_ib_create_srq() のエラー時のリソースリーク修正](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-46178) | 20.0 | 28.0 | 38.0 |
| [CVE-2026-46181 RDMA/mlx4: mlx4_srq_event()におけるRCUの誤用を修正](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-46181) | 20.0 | 28.0 | 38.0 |
| [CVE-2026-46174 x86/CPU/AMD: Zen2のオペコードキャッシュにおける共有リソースの不適切な分離を防止](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-46174) | 20.0 | 28.0 | 38.0 |
| [CVE-2026-46193 xfrm: ah: 非同期コールバックでESNの高位ビットを考慮する](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-46193) | 20.0 | 28.0 | 38.0 |
| [CVE-2026-46184 sound: ua101におけるprobe時のゼロ除算の修正](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-46184) | 20.0 | 28.0 | 38.0 |
| [CVE-2026-46106 eventfs: remount時にevents走査でeventfs_mutexとSRCUを保持する](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-46106) | 20.0 | 28.0 | 38.0 |
| [CVE-2026-46121 mm/damon/sysfs-schemes: damon_sysfs_lockでmemcg_pathのkfree()を保護](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-46121) | 20.0 | 28.0 | 38.0 |

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
