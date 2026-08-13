# 📡 サイレーダー 2026-08-13 17:00 JST

このレポートは、2026-08-13 11:00 JST〜2026-08-13 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 44
- [音声で扱う想定のトピック](#audio-topics): 2
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 18

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [CVE-2026-20349: CISA KEV catalog addition](#topic-27066) | 50.0 | 64.0 | 59.0 | 音声 | 温度感上位枠 |
| 2 | [Attackers Exploit SharePoint Authentication Bypass After Public PoC Release](#topic-27420) | 41.0 | 56.0 | 52.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-27066"></a>

### 1. CVE-2026-20349: CISA KEV catalog addition

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>D⁠D⁠o⁠S</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 50.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 59.0 |

#### 概要

CVE-2026-20349は、Cisco Secure Firewall ASA/FTDのRemote Access SSL VPNサービスに存在する脆弱性で、認証なしの遠隔攻撃により機器が予期せず再起動し、サービス不能に陥る可能性があるとされています。
Ciscoは修正版を案内しており、この問題はCISAのKEVカタログにも追加されています。
実際に悪用が観測されたとされており、境界防御機器の停止はネットワーク全体の可用性に直結します。
特にVPN経由のリモート接続基盤を使っている組織では、影響範囲が大きくなりやすい点が注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
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

- Ciscoの該当製品・該当ソフトウェア版が使われていないかを確認し、修正版の適用状況を点検する。
- 外部公開しているRemote Access SSL VPNの稼働状況と、予期しない再起動やサービス断の監視を強化する。
- CISA KEV掲載対象として扱い、脆弱性管理の優先順位を上げて対応計画に反映する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-20349 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Adaptive Security Appliance | 言及あり | 0.80 | — |
| 製品 | Cisco Firepower Threat Defense | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-20349](https://nvd.nist.gov/vuln/detail/CVE-2026-20349) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco fixes vulnerability exploited to DoS its firewalls (CVE-2026-20349)](https://www.helpnetsecurity.com/2026/08/13/cve-2026-20349-cisco-firewalls-dos/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Patches Firewall Zero-Day Exploited for DoS Attacks](https://www.securityweek.com/cisco-patches-firewall-zero-day-exploited-for-dos-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Secure Firewall Adaptive Security Appliance and Secure Firewall Threat Def](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-asaftd-vpn-dos-dzv4mQFF) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="topic-27420"></a>

### 2. Attackers Exploit SharePoint Authentication Bypass After Public PoC Release

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>P⁠o⁠C</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 41.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 56.0 |
| <nobr>確⁠度</nobr> | 52.0 |

#### 概要

Microsoft SharePointの脆弱性「CVE-2026-55040」について、公開されたPoCコードの後に攻撃での悪用が始まったと報じられています。
脆弱性は認証に関連する重要なセキュリティ機能の回避で、Microsoftは2026年7月の更新で修正済みとされています。
公開PoCの存在は、脆弱性の再現や悪用の敷居を下げるため、未対応環境へのリスクが高まります。SharePointは業務利用が多く、認証回避が成立すると影響範囲が広くなり得ます。

#### 温度感の理由

##### 温度感
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。

##### 実務影響
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

##### 確度
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 該当するSharePoint環境が7月2026の修正を適用済みか確認する。
- 外部公開されたSharePoint関連の認証・アクセス制御の設定を点検する。
- 脆弱性情報と検知ログを突き合わせ、異常な認証試行や不審なアクセスを監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-55040 | 関連CVE | 1.00 | 候補あり（URL 1件以上） |
| ベンダー | Microsoft | 言及あり | 0.80 | — |
| 製品 | Microsoft SharePoint | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-55040](https://nvd.nist.gov/vuln/detail/CVE-2026-55040) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Attackers Exploit SharePoint Authentication Bypass After Public PoC Release](https://thehackernews.com/2026/08/attackers-exploit-sharepoint.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
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
| [DDoS攻撃が過去最大規模に、1Tbps超のキャンペーンが一般化](https://www.helpnetsecurity.com/2026/08/13/cloudflare-h1-2026-ddos-trends-report/) | 28.0 | 20.0 | 42.0 |
| [Wireshark 4.6.8、ファイルパーサーを含む28件のセキュリティ脆弱性を修正](https://www.helpnetsecurity.com/2026/08/13/wireshark-4-6-8-patches-security-bugs/) | 28.0 | 20.0 | 42.0 |
| [AIエージェントで構築した「自律型ハッキングツール」がアジアの政府機関を攻撃、中国による台湾政府への攻撃か](https://gigazine.net/news/20260813-ai-government-cyberattack/) | 27.0 | 20.0 | 42.0 |
| [Product showcase：この画像は本物？ Slop or Notが検証する](https://www.helpnetsecurity.com/2026/08/13/product-showcase-slop-or-not-ai-image-detector/) | 25.0 | 20.0 | 42.0 |
| [ベルギーのeID認証で市民アカウントがRCEの脆弱性にさらされる](https://www.darkreading.com/application-security/belgium-eid-authentication-citizen-accounts-rce) | 24.0 | 38.0 | 42.0 |
| [健診名簿を会場に置き忘れ、8日後に拾得 - 長崎県健康事業団](https://www.security-next.com/188374) | 22.0 | 20.0 | 42.0 |
| [研修施設のサイトが改ざん被害、影響などを調査 - 東海大](https://www.security-next.com/188455) | 22.0 | 20.0 | 42.0 |
| [複数年度の傷病者情報含む救急活動記録票を誤廃棄 - 伊勢崎市](https://www.security-next.com/188151) | 22.0 | 20.0 | 42.0 |
| [「トランプ大統領が政府の公式発表にいち早くアクセスできる権限を1600万円で提供することは違法だ」と報道の自由財団とThe Interceptが訴える](https://gigazine.net/news/20260813-intercept-fpf-sues-trump-selling-premium-truth-social-access/) | 22.0 | 20.0 | 42.0 |
| [Adobe、パッチチューズデーに複数製品の脆弱性を修正](https://www.security-next.com/188742) | 22.0 | 20.0 | 42.0 |
| [ヨネックス、公式ECショップに不正ログイン 氏名や住所、購入履歴が閲覧された恐れ パスワード変更呼び掛け](https://www.itmedia.co.jp/news/article/2608/13/2000000527/) | 21.0 | 20.0 | 42.0 |
| [総務省のAIセキュリティガイドライン「知っているが生かせない」企業が7割 対策を阻む事情とは？](https://atmarkit.itmedia.co.jp/ait/articles/2608/13/news047.html) | 21.0 | 20.0 | 42.0 |
| [あのGoogleもFacebookも1.2億ドル詐取された 詐欺師が「受信トレイ」を真っ先に狙う理由](https://atmarkit.itmedia.co.jp/ait/articles/2608/13/news013.html) | 21.0 | 20.0 | 42.0 |
| [公開Googleドキュメントに保存されたパスワードが検索結果に表示された問題](https://www.theregister.com/security/2026/08/13/passwords-stored-in-public-google-doc-then-showed-up-in-search-results/5287028) | 20.0 | 20.0 | 42.0 |
| [サイバー攻撃から24時間で復旧する方法](https://www.itpro.com/security/cyber-attacks/24-hours-to-recover-from-a-cyber-attack) | 20.0 | 20.0 | 42.0 |
| [企業がプレッシャー下で犯しがちな4つの調査ミス](https://www.helpnetsecurity.com/2026/08/13/corporate-investigation-mistakes-video/) | 20.0 | 20.0 | 42.0 |
| [VoiceTraにおける接続先の制限が不適切な脆弱性](https://jvn.jp/jp/JVN00941257/) | 20.0 | 20.0 | 42.0 |
| [Chinese Loongsonプロセッサにキャッシュ情報漏えいの脆弱性、研究者が発見](https://www.theregister.com/security/2026/08/13/chinese-loongson-processors-have-leaky-caches-researchers-find/5287137) | 20.0 | 20.0 | 42.0 |

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
