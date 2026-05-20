# 📡 サイレーダー 2026-05-21 05:00 JST

このレポートは、2026-05-20 17:00 JST〜2026-05-21 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 114
- [音声で扱う想定のトピック](#audio-topics): 5
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [Microsoft Releases Mitigation for YellowKey BitLocker Bypass CVE-2026-45585 Exploit](#topic-7612) | 43.0 | 46.0 | 55.0 | 音声 | 温度感上位枠 |
| 2 | [CISA Adds Seven Known Exploited Vulnerabilities to Catalog](#topic-7417) | 38.0 | 38.0 | 47.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [Microsoft disrupts cybercrime operation that hid behind legitimate software](#topic-7907) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [Microsoft Takes Down Malware-Signing Service Behind Ransomware Attacks](#topic-7910) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Mini Shai Hulud: Compromised @antv npm packages enable CI/CD credential theft](#topic-7886) | 30.0 | 45.0 | 42.0 | 音声 | 温度感上位枠 |
| 6 | [ランサム被害が発生、一部サービスを停止 - システム開発会社](#topic-7915) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-7612"></a>

### 1. Microsoft Releases Mitigation for YellowKey BitLocker Bypass CVE-2026-45585 Exploit

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>防御・運用</nobr> / <nobr>Windows</nobr> / <nobr>ゼロデイ</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 43.0 |
| <nobr>実務影響</nobr> | 46.0 |
| <nobr>確度</nobr> | 55.0 |

#### 概要

Microsoftは、Windowsのフルディスク暗号化機能BitLockerを回避されるおそれがある脆弱性「YellowKey」（CVE-2026-45585）について、修正に向けて対応を進める一方、影響を受ける端末向けの緩和策を案内しています。
公開情報では、この問題はセキュリティ機能の回避に分類され、物理的なアクセスが前提となる可能性が示されています。
BitLockerは端末紛失や盗難時のデータ保護で重要なため、暗号化の回避につながる脆弱性は実運用への影響が大きいです。
緩和策が先に提示されている点からも、該当環境では早めの確認と適用が必要になります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 影響を受けるWindows端末があるかを確認し、Microsoftの案内に沿って緩和策を適用する。
- BitLocker依存の保護を前提にした運用を見直し、物理アクセス管理や端末持ち出し対策を強化する。
- 修正プログラムの提供状況を追い、適用可能になり次第速やかに更新する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-45585 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-45585](https://nvd.nist.gov/vuln/detail/CVE-2026-45585) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Microsoft provides mitigation for “YellowKey” BitLocker bypass flaw (CVE-2026-45](https://www.helpnetsecurity.com/2026/05/20/yellowkey-bitlocker-mitigation-cve-2026-45585/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Releases Mitigation for YellowKey BitLocker Bypass CVE-2026-45585 Expl](https://thehackernews.com/2026/05/microsoft-releases-mitigation-for.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 継続。

---

<a id="topic-7907"></a>

### 2. Microsoft disrupts cybercrime operation that hid behind legitimate software

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>攻撃キャンペーン</nobr> / <nobr>ランサムウェア</nobr> / <nobr>マルウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Microsoftが、正規ソフトウェアを装って活動していたサイバー犯罪組織に対する妨害措置を公表しました。
関連する「Fox Tempest」のマルウェア署名サービスは、複数のランサムウェア攻撃と結び付けられているとされています。
正規ソフトウェアを悪用したり、信頼性を装って検知を回避しようとする手口は、組織の防御をすり抜けやすいため注目されています。
ランサムウェア被害の前段にある支援インフラが断たれるかどうかは、今後の攻撃継続性にも影響します。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 正規ソフトウェアや署名済みファイルを前提にしない検知・検証を見直す。
- ランサムウェア本体だけでなく、配布や署名、運用支援など周辺インフラの変化も監視する。
- Microsoftなどベンダーの公表情報を確認し、関連するIOCや防御策が出た場合は速やかに反映する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft disrupts cybercrime operation that hid behind legitimate software](https://www.cybersecuritydive.com/news/microsoft-disrupts-cybercrime-hid-legitimate-software/820724/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-7910"></a>

### 3. Microsoft Takes Down Malware-Signing Service Behind Ransomware Attacks

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>マルウェア</nobr> / <nobr>ランサムウェア</nobr> / <nobr>脅威アクター</nobr> / <nobr>攻撃キャンペーン</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Microsoftは、同社のArtifact Signingシステムを悪用して不正なコードに署名し、ランサムウェアを含む攻撃を支援していたとされるmalware-signing-as-a-service（MSaaS）運用を妨害したと発表しました。
報道によれば、この活動は世界中の多数の端末やネットワークに影響した可能性があり、Microsoftは関連する脅威アクターをFox Tempestと呼んでいます。
正規の署名仕組みを悪用する手口は、悪意あるファイルの信頼性を見せかけるため、検知や利用者の見分けを難しくします。
ランサムウェアを含む複数の攻撃に関わるため、署名や配布経路の信頼確認がより重要になります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Microsoft製品や署名関連の通知・更新情報を確認し、影響の有無を把握する。
- 署名付きファイルであっても、配布元や実体の整合性を検証する運用を徹底する。
- ランサムウェア対策として、バックアップ、権限管理、EDRの検知ルールを再点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft Takes Down Malware-Signing Service Behind Ransomware Attacks](https://thehackernews.com/2026/05/microsoft-takes-down-malware-signing.html) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-7886"></a>

### 4. Mini Shai Hulud: Compromised @antv npm packages enable CI/CD credential theft

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>クラウド</nobr> / <nobr>Linux</nobr> / <nobr>マルウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 45.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Microsoft Security Blogによると、@antvのnpmパッケージが侵害され、CI/CD環境から認証情報を窃取しようとする「Mini Shai-Hulud」系のペイロードが配布されたとされています。
対象はLinuxベースの自動化環境で、npm install時に動作し、GitHub、AWS、Kubernetes、Vault、npm、1Passwordなどの資格情報が狙われたと説明されています。
ソフトウェアサプライチェーン経由で、開発・運用基盤の秘密情報がまとめて漏えいするおそれがあるためです。
CI/CDの認証情報が影響を受けると、コード改ざんやクラウド資源への不正アクセスにつながる可能性があります。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 依存しているnpmパッケージに@antv関連が含まれていないか確認し、該当版の利用有無を点検する。
- CI/CDで使用するトークンや鍵の棚卸しを行い、必要に応じてローテーションや失効を検討する。
- ビルド環境での外部通信や秘密情報の扱いを見直し、パッケージ導入時の監視と検知を強化する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Mini Shai Hulud: Compromised @antv npm packages enable CI/CD credential theft](https://www.microsoft.com/en-us/security/blog/2026/05/20/mini-shai-hulud-compromised-antv-npm-packages-enable-ci-cd-credential-theft/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="topic-7915"></a>

### 5. ランサム被害が発生、一部サービスを停止 - システム開発会社

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>ランサムウェア</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

スマートフォンアプリやウェブシステムの開発を手がけるノストラムが、ランサムウェアによるサイバー攻撃を受けたと公表しました。
影響を受けた学習支援サービスは一時停止されており、同社は対応を進めている状況です。
ランサムウェア被害は、単なる情報漏えいにとどまらず、サービス停止など業務継続への影響が出やすい点が重要です。
開発・運用を担う企業での公表は、委託先や周辺サービスを含めた影響確認の必要性を示します。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 関連するサービスの稼働状況と復旧案内を継続的に確認する。
- 委託先や外部連携先を含め、影響範囲の把握と連絡体制の確認を行う。
- バックアップ、アカウント管理、ログ保全など、初動対応と再発防止策の点検を進める。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [ランサム被害が発生、一部サービスを停止 - システム開発会社](https://www.security-next.com/184422) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 反応未確認。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-7417"></a>

### 1. CISA Adds Seven Known Exploited Vulnerabilities to Catalog

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>KEV</nobr> / <nobr>Windows</nobr> / <nobr>DDoS</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 38.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 47.0 |

#### 概要

CISAは、実際の悪用が確認されたとして、Known Exploited Vulnerabilities（KEV）カタログに7件の脆弱性を追加しました。
対象にはMicrosoftやAdobe関連の古い脆弱性に加え、比較的新しいとみられるCVEも含まれています。
KEVへの追加は、実環境で悪用が観測されていることを示すため、組織の優先対応対象として扱う必要があります。
特に古い脆弱性が含まれている場合、未管理資産や更新漏れが攻撃面として残っている可能性があります。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- 対象CVEが自組織の資産や利用製品に該当するかを確認し、優先度を上げて修正状況を点検する。
- パッチ適用済みでも、脆弱な旧バージョンの残存や例外設定、未把握端末がないか棚卸しする。
- 関連製品の監視を強め、異常な挙動や不審なアクセスがないかを確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2008-4250 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2009-1537 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2009-3459 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2010-0249 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2010-0806 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-41091 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-45498 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Seven Known Exploited Vulnerabilities to Catalog](https://www.cisa.gov/news-events/alerts/2026/05/20/cisa-adds-seven-known-exploited-vulnerabilities-catalog) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers hit vulnerabilities hard last year, making exploits the top entry poin](https://cyberscoop.com/verizon-data-breach-investigations-report-2026/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり・低信頼。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 継続。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [Microsoftが偽マルウェア署名サービス「Fox Tempest」を解体](https://www.malwarebytes.com/blog/news/2026/05/fake-malware-signing-service-fox-tempest-dismantled-by-microsoft) | 28.0 | 20.0 | 42.0 |
| [Androidマルウェアキャンペーン、数百の偽アプリで利用者に気づかれず課金](https://www.infosecurity-magazine.com/news/android-carrier-billing-fraud-four/) | 28.0 | 20.0 | 42.0 |
| [Webworm APTが新たなバックドアで欧州政府機関を標的にする](https://www.helpnetsecurity.com/2026/05/20/webworm-apt-campaign-targets-europe/) | 28.0 | 20.0 | 42.0 |
| [Drupalの高リスク悪用可能性のある不具合を修正する重要アップデート](https://www.bleepingcomputer.com/news/security/drupal-critical-update-to-fix-bug-with-high-exploitation-risk/) | 28.0 | 20.0 | 42.0 |
| [Webworm、DiscordとMS Graph APIを利用してEchoCreepとGraphWormバックドアを展開](https://thehackernews.com/2026/05/webworm-deploys-echocreep-and-graphworm.html) | 28.0 | 20.0 | 42.0 |
| [中国系Webworm APTが戦術を進化させ、欧州の標的へ拡大](https://www.infosecurity-magazine.com/news/webworm-apt-evolves-tactics/) | 28.0 | 20.0 | 42.0 |
| [Certificateとコードの再利用で追跡するTamperedChefクラスター](https://unit42.paloaltonetworks.com/tracking-tampered-chef-clusters/) | 28.0 | 20.0 | 42.0 |
| [NTTドコモビジネス、AIでSOC分析を10分化 対応稼働95%削減](https://news.mynavi.jp/techplus/article/20260520-4478686/) | 26.0 | 20.0 | 42.0 |
| [セールスフォース・ジャパン、「Slack」のAIエージェント新機能を日本で提供開始](https://japan.zdnet.com/article/35247771/) | 26.0 | 20.0 | 42.0 |
| [TaskhostのWindowsタスクにおけるローカル権限昇格の脆弱性（CVE-2025-60710）](https://nvd.nist.gov/vuln/detail/CVE-2025-60710) | 25.0 | 82.0 | 81.0 |
| [MicrosoftがRAMPARTとClarityをオープンソース化し、AIエージェントの開発時保護を強化](https://thehackernews.com/2026/05/microsoft-open-sources-rampart-and.html) | 25.0 | 20.0 | 42.0 |
| [AI搭載アプリ攻撃はより高速化・高頻度化し、阻止も困難に](https://www.securityweek.com/ai-powered-app-attacks-are-faster-more-frequent-and-harder-to-stop/) | 25.0 | 20.0 | 42.0 |
| [1Password、OpenAIと連携しAIコーディングエージェントによる認証情報漏えいを防止](https://www.securityweek.com/1password-teams-with-openai-to-stop-ai-coding-agents-from-leaking-credentials/) | 25.0 | 20.0 | 42.0 |
| [Agent AIの時代は来るか？準備はできているか？](https://thehackernews.com/2026/05/agent-ai-is-coming-are-you-ready.html) | 25.0 | 20.0 | 42.0 |
| [ArmorCode、露出管理と修復のためのAIワーカーをセキュリティチームに提供](https://www.helpnetsecurity.com/2026/05/20/armorcode-anya-agents/) | 25.0 | 20.0 | 42.0 |
| [Novata、AIでポートフォリオとサプライチェーン全体のリスクを可視化](https://www.helpnetsecurity.com/2026/05/20/novata-risk-atlas/) | 25.0 | 20.0 | 42.0 |
| [本番稼働後のAIを守る：想定外のリスクへの備え](https://www.securityweek.com/caught-off-guard-securing-ai-after-it-hits-production/) | 25.0 | 20.0 | 42.0 |
| [Trust3 AI、AIエージェントのリスクに対処するMCP Securityレイヤーに注力](https://www.helpnetsecurity.com/2026/05/20/trust3-mcp-security/) | 25.0 | 20.0 | 42.0 |
| [Typosquattingはもはやユーザーの問題ではなくサプライチェーンの問題である](https://thehackernews.com/2026/05/typosquatting-is-no-longer-user-problem.html) | 25.0 | 20.0 | 42.0 |
| [Threat DetectionとIncident Responseサミット、本日開催](https://www.securityweek.com/virtual-event-today-threat-detection-incident-response-summit/) | 25.0 | 20.0 | 42.0 |
| [Cisco ThousandEyes Enterprise Agent BrowserBotのコマンドインジェクション脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-tebbot-cmdinj-wN3yQ5gn) | 24.0 | 46.0 | 50.0 |
| [Cisco Nexus 3000および9000シリーズスイッチのBorder Gateway Protocolにおけるサービス拒否の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-bgp-iefab-3hb2pwtx) | 24.0 | 46.0 | 50.0 |
| [Cisco Secure Workloadの不正なAPIアクセス脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-csw-pnbsa-g8WEnuy) | 24.0 | 46.0 | 50.0 |
| [Cisco ThousandEyes Virtual Applianceの認証済みリモートコード実行の脆弱性](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-tevacert-rce-RMJVEym5) | 24.0 | 46.0 | 50.0 |

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
