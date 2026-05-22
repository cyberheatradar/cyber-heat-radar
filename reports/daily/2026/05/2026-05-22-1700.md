# 📡 サイレーダー 2026-05-22 17:00 JST

このレポートは、2026-05-22 11:00 JST〜2026-05-22 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 66
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 2
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [注意喚起: Palo Alto Networks製PAN-OSにおける認証回避の脆弱性（CVE-2026-0265）に関する注意喚起 (公開)](#topic-4257) | 47.0 | 74.0 | 60.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [CISA Adds Exploited Langflow and Trend Micro Apex One Vulnerabilities to KEV](#topic-8595) | 38.0 | 38.0 | 47.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 3 | [ランサム攻撃で障害発生、情報流出の可能性も - 東京鋪装工業](#topic-8947) | 30.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-8947"></a>

### 1. ランサム攻撃で障害発生、情報流出の可能性も - 東京鋪装工業

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | - |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 30.0 |
| <nobr>実務影響</nobr> | 30.0 |
| <nobr>確度</nobr> | 42.0 |

#### 概要

東京鋪装工業はサイバー攻撃を受け、障害が発生したことを公表しました。取引先や従業員の個人情報が流出した可能性も示されており、影響範囲の確認が進められている状況です。
業務停止と個人情報の流出可能性が同時に示されており、被害が運用面と情報管理の両方に及ぶおそれがあります。
取引先を含む関係者への影響が想定されるため、類似事案として注意が必要です。

#### 温度感の理由

##### 温度感
- 脅威・インシデント関連の公開情報として観測しています。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 個人情報や取引先情報を含むデータの保全状況と流出有無を早期に確認する。
- 障害の影響範囲を整理し、業務継続手順や代替運用を速やかに見直す。
- 関係先への連絡体制と、必要に応じた公表・通知の準備を進める。

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [ランサム攻撃で障害発生、情報流出の可能性も - 東京鋪装工業](https://www.security-next.com/184425) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: なし。
- 継続観測: 初出。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-4257"></a>

### 1. 注意喚起: Palo Alto Networks製PAN-OSにおける認証回避の脆弱性（CVE-2026-0265）に関する注意喚起 (公開)

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>CVE</nobr> / <nobr>脆弱性</nobr> / <nobr>認証バイパス</nobr> / <nobr>KEV</nobr> / <nobr>防御・運用</nobr> / <nobr>脅威アクター</nobr> / <nobr>政策・規制</nobr> / <nobr>PoC</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 47.0 |
| <nobr>実務影響</nobr> | 74.0 |
| <nobr>確度</nobr> | 60.0 |

#### 概要

Palo Alto NetworksのPAN-OSに、Cloud Authentication Service（CAS）が有効な構成で認証を回避されるおそれのある脆弱性（CVE-2026-0265）が公表されました。
影響範囲はPA-Series、VM-Series、Panoramaの一部で、Cloud NGFWとPrisma Accessは対象外とされています。
認証回避は、外部からの不正アクセスや管理系ポータルへの侵入につながる可能性があるため、境界防御製品では特に注意が必要です。
加えて、該当構成が非デフォルトでも一般的とされており、棚卸しと早期更新の優先度が高い話題です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 公開PoC・検証コード言及あり。
- 脅威・攻撃キャンペーン文脈。
- 技術者コミュニティ反応: 弱。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 公開PoCにより再現・悪用可能性が上がる。
- RCEまたは認証バイパス系。

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

- CASを使っているPAN-OS環境がないか確認し、該当する場合はベンダーが案内する修正版への更新を優先する。
- PA-Series、VM-Series、Panoramaのどれが影響対象か、利用中のバージョンが修正版に含まれるかを点検する。
- 管理画面やログイン用インターフェースの公開状況を見直し、不要な外部到達性があれば縮小する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-0265 | 主要CVE | 1.00 |
| 脆弱性 | CVE-2026-0300 | 主要CVE | 1.00 |
| ベンダー | Palo Alto | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-0265](https://nvd.nist.gov/vuln/detail/CVE-2026-0265) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>公的・一次情報</nobr> | [注意喚起: Palo Alto Networks製PAN-OSにおける認証回避の脆弱性（CVE-2026-0265）に関する注意喚起  (公開)](https://www.jpcert.or.jp/at/2026/at260015.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0265: Authentication Bypass in Palo Alto Networks PAN-OS](https://www.rapid7.com/blog/post/etr-cve-2026-0265-authentication-bypass-in-palo-alto-networks-pan-os) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-0265 PAN-OS: Authentication Bypass with Cloud Authentication Service (C](https://security.paloaltonetworks.com/CVE-2026-0265) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・高信頼。
- 日本語圏一次情報: あり。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 公開PoC・検証コード言及あり。
- 継続観測: 継続。

---

<a id="topic-8595"></a>

### 2. CISA Adds Exploited Langflow and Trend Micro Apex One Vulnerabilities to KEV

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | GitHub |
| <nobr>タグ</nobr> | <nobr>KEV</nobr> / <nobr>脆弱性</nobr> / <nobr>CVE</nobr> |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 38.0 |
| <nobr>実務影響</nobr> | 38.0 |
| <nobr>確度</nobr> | 47.0 |

#### 概要

CISAは、実際に悪用が確認された脆弱性として、LangflowとTrend Micro Apex Oneに関する脆弱性をKEVカタログに追加しました。
あわせて、別の資料ではMicrosoft Defenderに関する脆弱性を含む複数件の追加も示されています。
KEV入りは、当該脆弱性が現実に攻撃へ使われていることを示す重要なシグナルです。対象製品を使う組織では、優先度を上げて影響確認と更新対応を進める必要があります。

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

- CISAのKEVに追加された対象を確認し、自組織の利用有無と影響範囲を点検する。
- 該当製品・関連コンポーネントの修正パッチやベンダー案内を確認し、適用計画を前倒しする。
- 検知・監視ルールを見直し、関連する不審な挙動がないかログを確認する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-34291 | 主要CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>出典</nobr> | [CISA Adds Exploited Langflow and Trend Micro Apex One Vulnerabilities to KEV](https://thehackernews.com/2026/05/cisa-adds-exploited-langflow-and-trend.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Microsoft Defender vulnerabilities are being exploited in the wild](https://www.malwarebytes.com/blog/bugs/2026/05/microsoft-defender-vulnerabilities-are-being-exploited-in-the-wild) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応あり・低信頼。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 未評価。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 未評価。
- 開発者コミュニティ反応: 反応未確認。
- 攻撃・悪用観測シグナル: 悪用観測あり。
- 継続観測: 継続。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| <nobr>Topic</nobr> | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> |
|---|---:|---:|---:|
| [建設現場の知見共有をAIで効率化--「Google Workspace」「Gemini」活用でブログ作成も](https://japan.zdnet.com/article/35247877/) | 27.0 | 20.0 | 42.0 |
| [CapCut、GoogleのGeminiと提携 生成AIから直接動画・画像編集が可能に](https://www.itmedia.co.jp/news/articles/2605/22/news097.html) | 26.0 | 20.0 | 42.0 |
| [「Google AI Pro」ユーザーはYouTube広告ほぼ非表示 「Premium Lite」無料付与](https://www.itmedia.co.jp/news/articles/2605/22/news107.html) | 26.0 | 20.0 | 42.0 |
| [AIエージェントが10分で脅威特定、NTTドコモビジネスが新提供](https://xtech.nikkei.com/atcl/nxt/news/24/03238/) | 26.0 | 20.0 | 42.0 |
| [新しい詐欺の経済学：より安く、より速く、より説得力のある手口](https://www.helpnetsecurity.com/2026/05/22/visa-consumer-payment-fraud-report/) | 25.0 | 20.0 | 42.0 |
| [ふるさと納税寄付者の非公開氏名をサイトに誤掲載 - 八重瀬町](https://www.security-next.com/184586) | 22.0 | 20.0 | 42.0 |
| [Cross-Platform NPM Stealerの脅威拡大](https://isc.sans.edu/diary/rss/33006) | 22.0 | 20.0 | 42.0 |
| [Android版「ロボフォーム」に脆弱性 - 意図しないファイルDLのおそれ](https://www.security-next.com/184747) | 22.0 | 20.0 | 42.0 |
| [SNS公開のインタビュー動画に患者が映り込み - 大田記念病院](https://www.security-next.com/184742) | 22.0 | 20.0 | 42.0 |
| [度重なるサプライチェーン攻撃を受けnpmが「段階的リリース」を導入、流出したトークンだけではパッケージを公開できない仕組みを追加](https://gigazine.net/news/20260522-npm-staged-publishing/) | 22.0 | 20.0 | 42.0 |
| [VAIO、個人向けPCを「指定価格」に どの店でも同じ価格](https://www.itmedia.co.jp/news/articles/2605/22/news117.html) | 21.0 | 20.0 | 42.0 |
| [「とらのあな」電子書籍サービスに“不正な自動アクセス” 一部サービスを停止中](https://www.itmedia.co.jp/news/articles/2605/22/news116.html) | 21.0 | 20.0 | 42.0 |
| [マイナンバーカード取得義務化の提言に「法的必要性の議論必要」 松本デジタル相](https://xtech.nikkei.com/atcl/nxt/news/24/03239/) | 21.0 | 20.0 | 42.0 |
| [ファミマが楽天SPUに参加、グループ外で初 月3000円利用でポイント+0.5倍に](https://www.itmedia.co.jp/news/articles/2605/22/news108.html) | 21.0 | 20.0 | 42.0 |
| [「銀行をかたる」はもう古い クレカ13社共同のフィッシングサイト閉鎖、その成果は](https://atmarkit.itmedia.co.jp/ait/articles/2605/22/news048.html) | 21.0 | 20.0 | 42.0 |
| [NHK技研、目が疲れにくいVRゴーグルを“薄型化” 厚みを79％削減した新しい光学系を開発](https://www.itmedia.co.jp/news/articles/2605/22/news074.html) | 21.0 | 20.0 | 42.0 |
| [拘束しない認知症ケアを目指す、現場に寄り添った行動検知システムを開発](https://ascii.jp/elem/000/004/400/4400095/?rss=) | 21.0 | 20.0 | 42.0 |
| [物言う株主、KADOKAWA夏野CEO解任に賛同呼びかけ 在任5年で業績悪化、「ELDEN RING」「ニコニコ」への姿勢も疑問視](https://www.itmedia.co.jp/news/articles/2605/22/news086.html) | 21.0 | 20.0 | 42.0 |
| [ソフトバンクが「みまもりGPS」で声明 「日々の位置情報を中国と共有することない」──SNS上の噂に対応か](https://www.itmedia.co.jp/news/articles/2605/22/news080.html) | 21.0 | 20.0 | 42.0 |
| [国民年金の未納通知を装うフィッシングに注意　PayPayで送金要求](https://news.mynavi.jp/techplus/article/20260522-4482827/) | 21.0 | 20.0 | 42.0 |
| [久米商船、船舶管理プラットフォーム「MARITIME 7」船員労務管理を導入](https://japan.zdnet.com/article/35247873/) | 21.0 | 20.0 | 42.0 |
| [EIZO、JR西日本と共創したAIエッジコンピュータ--画像認識AIで異常を即時通知](https://japan.zdnet.com/article/35247869/) | 21.0 | 20.0 | 42.0 |
| [Cisco、Secure WorkloadのREST API脆弱性を修正しデータアクセスを可能にしたCVSS 10.0の問題](https://thehackernews.com/2026/05/cisco-patches-cvss-100-secure-workload.html) | 20.0 | 46.0 | 54.0 |
| [Unifi Accessにおけるリモートコード実行の脆弱性（CVE-2025-52665）](https://www.catchify.sa/post/cve-2025-52665-rce-in-unifi-os-25-000) | 20.0 | 46.0 | 50.0 |

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
