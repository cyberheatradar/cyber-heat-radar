# 📡 サイレーダー 2026-10-03 11:00 JST

このレポートは、2026-10-03 05:00 JST〜2026-10-03 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 30
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 5

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Cisco Catalyst SD-WAN Manager API Authentication Bypass Vulnerability](#topic-35199) | 50.0 | 64.0 | 66.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-35199"></a>

### 1. Cisco Catalyst SD-WAN Manager API Authentication Bypass Vulnerability

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 冷却中 |
| <nobr>温⁠度⁠感</nobr> | 50.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 64.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Cisco Catalyst SD-WAN Managerに存在する認証バイパス脆弱性（CVE-2026-76504）について、Ciscoは実際の悪用を確認したとしています。
影響を受ける環境では、認証されていないリモート攻撃者が管理者権限でAPIにアクセスできる可能性があるため、修正済みリリースへの更新が重要です。
SD-WANの管理基盤に関わるため、侵害されると広範囲のネットワーク運用や設定変更に影響し得ます。既に悪用観測があるとされ、優先度の高い対応が求められます。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 6 sources。
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

- 影響を受けるCisco Catalyst SD-WAN Managerのバージョンを確認し、修正済みリリースへ早急に更新する。
- 公開APIや管理系インターフェースへの不要な露出を見直し、アクセス元を最小限に制限する。
- Ciscoが案内する侵害痕跡や異常なAPI利用の有無を確認し、管理者権限の不審な操作を監視する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-76504 | 関連CVE | 1.00 | 未確認 |
| ベンダー | Cisco | 言及あり | 0.80 | — |
| 製品 | Cisco Catalyst SD-WAN Manager | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-76504](https://nvd.nist.gov/vuln/detail/CVE-2026-76504) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Cisco Catalyst SD-WAN Manager API Authentication Bypass Vulnerability](https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-sdwan-webauth-xr8beuuU) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds Exploited Cisco Catalyst SD-WAN Manager Auth Bypass to KEV](https://thehackernews.com/2026/10/cisa-adds-exploited-cisco-catalyst-sd.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [New Cisco SD-WAN zero-day exploited in-the-wild (CVE-2026-76504)](https://www.helpnetsecurity.com/2026/10/01/new-cisco-sd-wan-zero-day-exploited-in-the-wild-cve-2026-76504/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco Warns of Attackers Exploiting Critical Authentication Bypass in SD-WAN Man](https://thehackernews.com/2026/09/cisco-warns-of-attackers-exploiting.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Cisco Catalyst SD-WAN Manager API authentication bypass exploited in th](https://www.rapid7.com/blog/post/etr-critical-cisco-catalyst-sd-wan-manager-api-authentication-bypass-exploited-in-the-wild-cve-2026-76504) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Cisco warns of new SD-WAN zero-day exploited in attacks](https://www.bleepingcomputer.com/news/security/cisco-warns-of-new-sd-wan-authentication-bypass-zero-day-exploited-in-attacks/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Adds One Known Exploited Vulnerability to Catalog](https://www.cisa.gov/news-events/alerts/2026/09/30/cisa-adds-one-known-exploited-vulnerability-catalog) | <nobr>内容確認・補足情報</nobr> |

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
| [Apple、macOSの「フルディスクアクセス」に追加の制御を導入へ 「AIエージェントの進化でリスクが大幅に増大」](https://www.itmedia.co.jp/news/article/2610/03/2000001983/) | 26.0 | 20.0 | 42.0 |
| [「アバハウス」全顧客の情報漏えいか 会員・受注DBに不正アクセス 「不審な返金メール届いた」報告で判明](https://www.itmedia.co.jp/news/article/2610/03/2000001981/) | 21.0 | 20.0 | 42.0 |
| [靴のムーンスター、顧客情報漏えいの可能性 氏名や住所、注文情報など](https://www.itmedia.co.jp/news/article/2610/03/2000001982/) | 21.0 | 20.0 | 42.0 |
| [ABAHOUSE 全顧客の情報漏えいか](https://news.yahoo.co.jp/pickup/6597358?source=rss) | 20.0 | 20.0 | 42.0 |
| [RemoteThreatが警告する、対策失敗後に備えるための検証の必要性](https://www.darkreading.com/cybersecurity-operations/remotethreat-bets-security-teams-need-to-test-what-happens-after-defenses-fail) | 20.0 | 20.0 | 42.0 |

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
