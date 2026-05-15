# 📡 サイレーダー 2026-05-15 11:00 JST 試作版

このレポートは、2026-05-15 05:00 JST〜2026-05-15 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 101
- [音声で扱う想定のトピック](#audio-topics): 0
- [GitHubのみ掲載想定のトピック](#github-only-topics): 4
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cisco warns of new critical SD-WAN flaw exploited in zero-day attacks](#topic-4945) | 93.0 | 84.0 | 67.0 | GitHub | 直近掲載済み・再掲抑制 |
| 2 | [Hack: Local Privilege Escalation in Taskhost Windows Tasks (CVE-2025-60710).](#topic-12) | 54.0 | 82.0 | 81.0 | GitHub | 直近掲載済み・再掲抑制 |
| 3 | [Maximum Severity Cisco SD-WAN Bug Exploited in the Wild](#topic-5050) | 45.0 | 38.0 | 43.0 | GitHub | 直近掲載済み・再掲抑制 |
| 4 | [OpenAI asks macOS users to update after TanStack npm supply chain attack](#topic-5049) | 33.0 | 30.0 | 42.0 | GitHub | 直近掲載済み・再掲抑制 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

今回は音声で扱う想定のトピックはありません。

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-4945"></a>

### 1. Cisco warns of new critical SD-WAN flaw exploited in zero-day attacks

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>認証バイパス</nobr> / <nobr>KEV</nobr> / <nobr>政策・規制</nobr> / <nobr>防御・運用</nobr> / <nobr>IoC</nobr> / <nobr>ゼロデイ</nobr> / <nobr>PoC</nobr> / <nobr>国家支援</nobr> |
| <nobr>温度状態</nobr> | 高温 |
| <nobr>温度感</nobr> | 93.0 |
| <nobr>実務影響</nobr> | 84.0 |
| <nobr>確度</nobr> | 67.0 |

#### 概要

Ciscoは、Catalyst SD-WAN Controllerおよび関連製品に存在する認証バイパスの脆弱性CVE-2026-20182を修正する更新を公開し、限定的なゼロデイ攻撃で悪用されたと説明しています。
脆弱性の深刻度はCVSS 10.0とされ、影響を受ける環境では管理者権限の不正取得につながる可能性があるとされています。
SD-WANコントローラはネットワーク制御の中核に位置するため、侵害されると広範な影響が出やすい点が注目されています。
加えて、実際の悪用が示唆されているため、通常の脆弱性情報よりも早急な対応が求められます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 中。

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

- Ciscoの案内に沿って、該当製品の修正版適用状況を確認する。
- 自組織でCatalyst SD-WAN Controller / Managerの利用有無と対象バージョンを棚卸しする。
- 異常な制御接続や管理権限の変化など、ベンダーが示す確認観点に基づいて影響有無を点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-20182 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20133 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20128 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20122 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-20127 | 主要CVE | 1.00 |
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20182](https://nvd.nist.gov/vuln/detail/CVE-2026-20182) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of new critical SD-WAN flaw exploited in zero-day attacks](https://bleepingcomputer.com/news/security/cisco-warns-of-new-critical-sd-wan-flaw-exploited-in-zero-day-attacks) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Controller Auth Bypass Actively Exploited to Gain Admin Ac](https://thehackernews.com/2026/05/cisco-catalyst-sd-wan-controller-auth.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Ongoing exploitation of Cisco Catalyst SD-WAN vulnerabilities](https://blog.talosintelligence.com/sd-wan-ongoing-exploitation) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [The Dark Side of Efficiency: When Network Controllers Become "God Mode" for Atta](https://rapid7.com/blog/post/tr-efficiencys-dark-side-network-controllers-in-god-mode-attackers-sd-wan) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-20182: Critical authentication bypass in Cisco Catalyst SD-WAN Controll](https://rapid7.com/blog/post/ve-cve-2026-20182-critical-authentication-bypass-cisco-catalyst-sd-wan-controller-fixed) | <nobr>内容確認・補足情報</nobr> |
| <nobr>公的・一次情報</nobr> | [Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-rpa2-v69WY2SW) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://cisa.gov/news-events/alerts/2026/05/14/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

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

CVE-2025-60710は、Microsoft WindowsのTaskhost関連の処理におけるローカル権限昇格の脆弱性として整理されています。
CISAのKnown Exploited Vulnerabilitiesに掲載されており、公開PoCの存在も示されています。
権限昇格の脆弱性は、侵入後に被害を拡大させる足がかりになりやすいため注意が必要です。公開PoCの言及があることで、検証や悪用のハードルが下がる可能性があります。

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

- Windows環境での適用状況を確認し、関連する修正や緩和策の有無を点検する。
- 特にローカルでの権限上昇につながる挙動がないか、監査・検知ルールを見直す。
- CISA KEV掲載対象として、優先度を上げて資産棚卸しと対応計画を確認する。

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

<a id="topic-5050"></a>

### 3. Maximum Severity Cisco SD-WAN Bug Exploited in the Wild

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>KEV</nobr> / <nobr>脅威アクター</nobr> / <nobr>CVE</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 45.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 43.0 |

#### 概要

CiscoのSD-WAN関連の脆弱性が、現実の攻撃で悪用されたと報じられています。
報道では、今年に入ってCiscoのネットワーク制御システムに対するCVSS 10.0の脆弱性が再び攻撃者に利用されたとされています。
ネットワーク機器や制御系の脆弱性は、影響範囲が広く、侵害時の波及も大きくなりやすいため注目されています。
悪用観測がある場合は、単なる理論上のリスクではなく、迅速な確認と対応が必要になります。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Cisco SD-WAN環境で該当する製品・バージョンの有無を確認し、ベンダー告知に基づく修正適用を急ぐ。
- 外部公開されている管理画面や制御系インターフェースの露出状況を見直し、不要な公開を避ける。
- 関連ログや管理操作の履歴を確認し、異常な認証・設定変更・通信の兆候がないか点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Cisco | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Maximum Severity Cisco SD-WAN Bug Exploited in the Wild](https://darkreading.com/vulnerabilities-threats/maximum-severity-cisco-sd-wan-bug-exploited) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり・低信頼。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 初出。

---

<a id="topic-5049"></a>

### 4. OpenAI asks macOS users to update after TanStack npm supply chain attack

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>サプライチェーン</nobr> / <nobr>AI</nobr> / <nobr>攻撃キャンペーン</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

OpenAIが、TanStackを巡るnpmのサプライチェーン攻撃に関連して、macOS利用者に更新を促しているとされています。
公開情報では、この動きはTanStackだけでなく、複数のAI関連企業に結びつくnpmやPyPIパッケージへ影響が広がっている状況を受けたものとされています。
サプライチェーン攻撃は、直接の標的でなくても依存関係を通じて開発環境や利用者に影響が及ぶ点が重要です。
特にnpmやPyPIはソフトウェア供給網で広く使われており、影響範囲が拡大しやすいことが注目されています。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- npm/PyPI・侵害パッケージ・開発者/CI/CDへの影響を伴うサプライチェーン攻撃。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 利用中の依存パッケージに更新や異常がないか確認し、公式アナウンスに沿って対応する。
- 開発・CI/CD環境で、問題となる可能性のあるパッケージの固定化や再取得の有無を点検する。
- macOSを含む端末側でも、ベンダーや保守担当からの更新案内を優先して適用する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ai_model_or_project | OpenAI | 主題 | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [OpenAI asks macOS users to update after TanStack npm supply chain attack](https://therecord.media/openai-asks-macos-users-to-update-tanstack-npm) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [NGINXのrewrite機能に「緊急」の脆弱性 “見落とし設定”がRCEの入り口に](https://atmarkit.itmedia.co.jp/ait/articles/2605/15/news043.html) | 29.0 | 38.0 | 42.0 |
| [GMOサイバーセキュリティ byイエラエ、オンラインセミナー「増え続けるランサムウェア被害、限られた予算でどこまで守る？脆弱性対策優先順位の付け方」5 / 19 開催](https://scan.netsecurity.ne.jp/article/2026/05/15/55279.html) | 29.0 | 30.0 | 42.0 |
| [マルタケの一部サーバでのシステム障害、不正アクセス（ランサムウェア）による影響の可能性も含め調査](https://scan.netsecurity.ne.jp/article/2026/05/15/55278.html) | 29.0 | 30.0 | 42.0 |
| [公益財団法人B&G財団にマルウェア攻撃、サーバでシステム障害が発生](https://scan.netsecurity.ne.jp/article/2026/05/15/55276.html) | 29.0 | 20.0 | 42.0 |
| [Burst Statistics WordPressプラグインの認証バイパス脆弱性を悪用する攻撃者](https://bleepingcomputer.com/news/security/hackers-exploit-auth-bypass-flaw-in-burst-statistics-wordpress-plugin) | 28.0 | 38.0 | 42.0 |
| [セキュアな接続と強固なバックアップでランサムウェア被害の早期復旧を支援するサービス、KDDIアイレットが提供開始](https://internet.watch.impress.co.jp/docs/news/2108724.html) | 28.0 | 30.0 | 42.0 |
| [「Linux」カーネルに三たび重大な脆弱性が見つかる--AIツールの登場で加速](https://japan.zdnet.com/article/35247550) | 26.0 | 20.0 | 42.0 |
| [AI事業者が争う姿勢 朝日、日経の記事無断使用巡り](https://itmedia.co.jp/news/articles/2605/15/news068.html) | 26.0 | 20.0 | 42.0 |
| [Anthropicとゲイツ財団が提携 AIによる社会貢献に2億ドル拠出](https://itmedia.co.jp/news/articles/2605/15/news064.html) | 26.0 | 20.0 | 42.0 |
| [AppleがiOS 26.5公開 カーネルやWebKitなど多数の脆弱性を修正、早期更新を](https://itmedia.co.jp/enterprise/articles/2605/15/news042.html) | 25.0 | 28.0 | 42.0 |
| [TeamPCPハッカーがMistral AIのコードリポジトリを売りに出す](https://bleepingcomputer.com/news/security/teampcp-hackers-advertise-mistral-ai-code-repos-for-sale) | 25.0 | 20.0 | 42.0 |
| [国防総省のサイバー担当者、先進AIを「革命的な戦争」と呼ぶ](https://cyberscoop.com/pentagon-cyber-ai-revolutionary-warfare-mythos) | 25.0 | 20.0 | 42.0 |
| [ホワイトハウスのサイバー担当者、AI時代におけるIDセキュリティの重要性を強調](https://cyberscoop.com/white-house-federal-identity-security-ai-risks) | 25.0 | 20.0 | 42.0 |
| [日本人の頭蓋骨、100年間で大きく変化 “短頭化”し男女差も拡大 東大や科警研などが研究発表](https://itmedia.co.jp/news/articles/2605/15/news028.html) | 24.0 | 20.0 | 43.0 |
| [NVIDIA製「RTX5090」登場で記憶認証は崩壊？ GPU進化に負けないパスワードを作るコツ](https://atmarkit.itmedia.co.jp/ait/articles/2605/15/news041.html) | 24.0 | 20.0 | 43.0 |
| [OpenAIがAppleに対する法的措置も視野に法律事務所に相談中、加入者増加と知名度向上に不服](https://gigazine.net/news/20260515-openai-apple-partnership-frays) | 22.0 | 20.0 | 42.0 |
| [スマートグラス「Meta Ray-Ban Display」に指の動きだけで文字を入力できる手書き入力が搭載へ](https://gigazine.net/news/20260515-meta-ray-ban-display-neural-handwriting) | 22.0 | 20.0 | 42.0 |
| [AMD製AIチップで開発された拡散言語モデル「ZAYA1-8B-Diffusion-Preview」が登場、自己回帰モデルを拡散モデルに変換](https://gigazine.net/news/20260515-zaya1-8b-diffusion-preview) | 22.0 | 20.0 | 42.0 |
| [xAIがコーディングエージェントCLIツール「Grok Build」のベータ版をリリース](https://gigazine.net/news/20260515-grok-build-beta) | 22.0 | 20.0 | 42.0 |
| [未査読論文リポジトリのarXivが「論文にLLMによる間違いや架空の引用が含まれていたら1年間投稿禁止」の方針を示す](https://gigazine.net/news/20260515-arxiv-ai-paper-banned) | 22.0 | 20.0 | 42.0 |
| [「VMware Fusion」に権限昇格の脆弱性 - 修正版を公開](https://security-next.com/184463) | 22.0 | 20.0 | 42.0 |
| [ChatGPTのスマホアプリにCodexへの指示機能が追加される、PCを開かずともCodexでエージェントコーディングやPC自動操作を実行可能](https://gigazine.net/news/20260515-codex-mobile-app) | 22.0 | 20.0 | 42.0 |
| [「Chrome」で脆弱性79件を修正 - 14件が「クリティカル」](https://security-next.com/184460) | 22.0 | 20.0 | 42.0 |
| [自分の「好き」を記録しながら同じ趣味の人とゆるやかにつながりあえるSNS「コレクトピア」で自分の趣味をさくっとコレクションにまとめてみた](https://gigazine.net/news/20260515-collectopia) | 22.0 | 20.0 | 42.0 |

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
