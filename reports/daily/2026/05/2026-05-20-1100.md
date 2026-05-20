# 📡 サイレーダー 2026-05-20 11:00 JST

このレポートは、2026-05-20 05:00 JST〜2026-05-20 11:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 79
- [音声で扱う想定のトピック](#audio-topics): 3
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [Microsoft 2026年5月 Patch Tuesday 関連まとめ](#topic-3472) | 52.0 | 56.0 | 58.0 | 音声 | 温度感上位枠 |
| 2 | [Cybercrime service disrupted for abusing Microsoft platform to sign malware](#topic-7415) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [Microsoft Exchange ProxyShell Scanning Doubles in April 2026 as Two Distinct Campaign Clusters Emerge](#topic-7405) | 30.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-3472"></a>

### 1. Microsoft 2026年5月 Patch Tuesday 関連まとめ

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>AI</nobr> / <nobr>Windows</nobr> / <nobr>RCE</nobr> / <nobr>ゼロデイ</nobr> / <nobr>AIエージェント</nobr> / <nobr>脅威レポート</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 52.0 |
| <nobr>実務影響</nobr> | 56.0 |
| <nobr>確度</nobr> | 58.0 |

#### 概要

Microsoftは2026年5月のPatch Tuesdayで、120件超のCVEに対応する修正を公開しました。
現時点では、少なくとも公開情報ベースで広く悪用中のゼロデイは確認されていない一方、Microsoft Word関連の複数の重要なRCE脆弱性を含め、優先度の高い修正が含まれています。
件数が多く、影響範囲も広いため、通常の月例更新として見過ごしにくい内容です。特に文書ファイルを起点とする脆弱性は利用機会が多く、組織内の端末保護や更新計画に直結します。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 14 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 強。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- RCEまたは認証バイパス系。

##### 確度
- 複数ソース確認。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認または未評価。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Wordを含むOffice系の修正を優先的に適用する。
- 通常の月例より件数が多いため、検証環境での確認と段階的展開を意識する。
- OSだけでなく、利用中のMicrosoft製品全体の適用漏れがないか確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-40364 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40361 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-41096 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-41089 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-42898 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-40415 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-35435 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-35428 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-42826 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-32207 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Windows Zero-Day Barrage Continues After Patch Tuesday](https://www.darkreading.com/cyberattacks-data-breaches/windows-zero-day-barrage-continues-after-patch-tuesday) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [A week in security (May 11 – May 17)](https://www.malwarebytes.com/blog/news/2026/05/a-week-in-security-may-11-may-17-2) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft, Palo Alto Networks Find Many Vulnerabilities by Using AI on Their Own](https://www.securityweek.com/microsoft-palo-alto-networks-find-many-vulnerabilities-by-using-ai-on-their-own-code/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft's MDASH AI System Finds 16 Windows Flaws Fixed in Patch Tuesday](https://thehackernews.com/2026/05/microsofts-mdash-ai-system-finds-16.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [May 2026 Patch Tuesday: no zero-days but plenty to fix](https://www.malwarebytes.com/blog/news/2026/05/may-2026-patch-tuesday-no-zero-days-but-plenty-to-fix) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Chipmaker Patch Tuesday: Intel and AMD Patch 70 Vulnerabilities](https://www.securityweek.com/chipmaker-patch-tuesday-intel-and-amd-patch-70-vulnerabilities/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Fixes 17 Critical Flaws in May Patch Tuesday](https://www.infosecurity-magazine.com/news/microsoft-17-critical-flaws-may/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [ICS Patch Tuesday: New Security Advisories From Siemens, Schneider, CISA](https://www.securityweek.com/ics-patch-tuesday-new-security-advisories-from-siemens-schneider-cisa/) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 強。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 継続。

---

<a id="topic-7415"></a>

### 2. Cybercrime service disrupted for abusing Microsoft platform to sign malware

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>マルウェア</nobr> / <nobr>ランサムウェア</nobr> / <nobr>攻撃キャンペーン</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 36.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

Microsoftは、自社のArtifact Signingサービスを悪用して不正なコード署名証明書を生成し、マルウェアに署名させる「malware-signing-as-a-service」運用を阻止したとしています。
こうした証明書は、ランサムウェア関係者を含むサイバー犯罪者に利用されていたと説明されています。
正規の署名に見せかけられると、マルウェアの信頼性が不当に高まり、検知や利用者の判断を難しくするおそれがあります。
クラウド/署名基盤そのものの悪用は、攻撃対象が端末だけでなく認証・配布の仕組みに及ぶことを示しています。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- コード署名証明書の信頼性確認と、発行元・失効状況の監視を強化する。
- 署名付きだからといって安全とみなさず、配布経路や挙動ベースの検知も併用する。
- Microsoft側の関連通知や失効情報があれば、社内の検知ルールやブロックリストに反映する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Cybercrime service disrupted for abusing Microsoft platform to sign malware](https://www.bleepingcomputer.com/news/security/cybercrime-service-disrupted-for-abusing-microsoft-platform-to-sign-malware/) | <nobr>内容確認・補足情報</nobr> |

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

<a id="topic-7405"></a>

### 3. Microsoft Exchange ProxyShell Scanning Doubles in April 2026 as Two Distinct Campaign Clusters Emerge

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>攻撃キャンペーン</nobr> / <nobr>CVE</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 20.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

F5 Labsの分析によると、2026年4月にMicrosoft ExchangeのProxyShell関連のスキャン活動が増加したとされています。
あわせて、活動は性質の異なる2つのキャンペーンクラスターに分かれている可能性が示されています。
Exchangeは組織内の重要な業務システムで使われることが多く、関連するスキャンの増加は防御側にとって無視できません。
攻撃の兆候が複数のグループに分かれている可能性があるため、単一の動きとして見ない監視が必要です。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。

##### 実務影響
- 影響範囲、標的、TTP、検知観点を確認する価値があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Exchange公開系の露出状況や不要な外部公開設定を再確認する。
- ProxyShell関連の検知ルールやログ監視を見直し、急なスキャン増加を追えるようにする。
- 侵害の有無にかかわらず、パッチ適用状況と管理系アカウントの保護を点検する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [Microsoft Exchange ProxyShell Scanning Doubles in April 2026 as Two Distinct Cam](https://www.f5.com/labs/articles/microsoft-exchange-proxyshell-scanning-doubles-in-april-2026-as-two-distinct-campaign-clusters) | <nobr>内容確認・補足情報</nobr> |

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

今回はGitHubのみ掲載の注目トピックはありません。

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [Verizon DBIR 2026：脆弱性の悪用が認証情報窃取を上回り主要な侵害経路に](https://www.securityweek.com/verizon-dbir-2026-vulnerability-exploitation-overtakes-credential-theft-as-top-breach-vector/) | 28.0 | 30.0 | 42.0 |
| [Claude Mythosのヤバすぎる実力を検証 脆弱性を連結して攻撃経路を生成](https://atmarkit.itmedia.co.jp/ait/articles/2605/20/news042.html) | 28.0 | 20.0 | 42.0 |
| [グーグル、AIプランを刷新--これから選ぶべきプランは？](https://japan.zdnet.com/article/35247708/) | 26.0 | 20.0 | 42.0 |
| [AWSのワークショップで「旅行プランナー」のAIエージェントを開発した](https://ascii.jp/elem/000/004/402/4402705/?rss=) | 26.0 | 20.0 | 42.0 |
| [攻撃・防御それぞれで AI に向き合うエンジニアが語る ～ GMO IERAE HackNight #4 が 6 / 2 開催](https://scan.netsecurity.ne.jp/article/2026/05/20/55311.html) | 26.0 | 20.0 | 42.0 |
| [Okta for AI Agents と「Amazon Bedrock AgentCore」が統合](https://scan.netsecurity.ne.jp/article/2026/05/20/55306.html) | 26.0 | 20.0 | 42.0 |
| [Google、パーソナルAIエージェント「Gemini Spark」発表――デバイスを閉じても自律で働く](https://www.itmedia.co.jp/news/articles/2605/20/news068.html) | 26.0 | 20.0 | 42.0 |
| [Google検索が「AI検索」に──エージェント機能やマルチモーダル入力に対応](https://www.itmedia.co.jp/news/articles/2605/20/news067.html) | 26.0 | 20.0 | 42.0 |
| [現実世界を基に"動き回れる"仮想空間を生成　Googleの世界生成AI「Project Genie」にストリートビュー連携機能](https://www.itmedia.co.jp/news/articles/2605/20/news065.html) | 26.0 | 20.0 | 42.0 |
| [TaskhostのWindowsタスクにおけるローカル権限昇格の脆弱性（CVE-2025-60710）](https://nvd.nist.gov/vuln/detail/CVE-2025-60710) | 25.0 | 82.0 | 81.0 |
| [Netskope、SASEプラットフォーム「Netskope One」に、AIエージェントにも対応するセキュリティ機能群を統合](https://internet.watch.impress.co.jp/docs/news/2109912.html) | 25.0 | 20.0 | 42.0 |
| [AIアプリ向けChromaDBの最高深刻度の脆弱性によりサーバーが乗っ取られる](https://www.bleepingcomputer.com/news/security/max-severity-flaw-in-chromadb-for-ai-apps-allows-server-hijacking/) | 25.0 | 20.0 | 42.0 |
| [Androidアプリ「パスワード管理 ロボフォーム」のintent処理における検証不備の脆弱性](https://jvn.jp/vu/JVNVU93461473/) | 23.0 | 20.0 | 43.0 |
| [Cloudflareが明かす「Mythos Preview」の実力 AIが脆弱性発見から攻撃実証まで自律実行](https://www.itmedia.co.jp/enterprise/articles/2605/20/news035.html) | 23.0 | 20.0 | 42.0 |
| [推論サーバ「NVIDIA Triton Inference Server」に複数脆弱性](https://www.security-next.com/184657) | 22.0 | 20.0 | 42.0 |
| [「Firefox 151」がリリース - 脆弱性31件に対応](https://www.security-next.com/184650) | 22.0 | 20.0 | 42.0 |
| [「Drupal」が緊急更新を予定 - 数時間で脆弱性悪用の可能性](https://www.security-next.com/184640) | 22.0 | 20.0 | 42.0 |
| [PR： ネットワークのブラックボックス化が招く致命的な被害とは 有線・無線を一括制御して、トラブル復旧を速める秘策](https://atmarkit.itmedia.co.jp/ait/articles/2605/20/news003.html) | 21.0 | 20.0 | 42.0 |
| [アメリカ人「近所にデータセンターが建設されるくらいなら原子力発電所が建つ方がまだまし」世論調査結果](https://scan.netsecurity.ne.jp/article/2026/05/20/55312.html) | 21.0 | 20.0 | 42.0 |
| [はてな資金流出、特別調査委員会設置](https://scan.netsecurity.ne.jp/article/2026/05/20/55310.html) | 21.0 | 20.0 | 42.0 |
| [東邦大学医療センター大森病院の業務委託先がペースメーカープログラマを紛失、個人情報が不正に閲覧される可能性が否定できない状況](https://scan.netsecurity.ne.jp/article/2026/05/20/55309.html) | 21.0 | 20.0 | 42.0 |
| [東北大学に不正アクセス、大学病院のNASに保存されていた個人情報が漏えいした可能性](https://scan.netsecurity.ne.jp/article/2026/05/20/55308.html) | 21.0 | 20.0 | 42.0 |
| [「E/SASV Games公式サイト」に不正アクセス、ファイル改ざんと不正なプログラムの設置を確認](https://scan.netsecurity.ne.jp/article/2026/05/20/55307.html) | 21.0 | 20.0 | 42.0 |
| [TSS LINK「トランセーファー BASIC」Ver.4.7リリース、Adobe Acrobat・Adobe Acrobat Reader バージョン2026 に対応](https://scan.netsecurity.ne.jp/article/2026/05/20/55305.html) | 21.0 | 20.0 | 42.0 |

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
