# 📡 サイレーダー 2026-05-18 05:00 JST 試作版

このレポートは、2026-05-17 17:00 JST〜2026-05-18 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を試験的に整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 39
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 24

| Rank | Topic | <nobr>温度感</nobr> | <nobr>実務影響</nobr> | <nobr>確度</nobr> | <nobr>区分</nobr> | <nobr>分類理由</nobr> |
|---:|---|---:|---:|---:|---|---|
| 1 | [NGINX CVE-2026-42945 Exploited in the Wild, Causing Worker Crashes and Possible RCE](#topic-4593) | 33.0 | 67.0 | 57.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-4593"></a>

### 1. NGINX CVE-2026-42945 Exploited in the Wild, Causing Worker Crashes and Possible RCE

#### スコアカード

| 項目 | 値 |
|---|---:|
| <nobr>区分</nobr> | 音声 |
| <nobr>タグ</nobr> | <nobr>脆弱性</nobr> / <nobr>CVE</nobr> / <nobr>RCE</nobr> / <nobr>KEV</nobr> |
| <nobr>分類理由</nobr> | 温度感上位枠 |
| <nobr>温度状態</nobr> | 継続監視 |
| <nobr>温度感</nobr> | 33.0 |
| <nobr>実務影響</nobr> | 67.0 |
| <nobr>確度</nobr> | 57.0 |

#### 概要

NGINXのngx_http_rewrite_moduleに関する脆弱性CVE-2026-42945が公表され、公開後まもなく実際の悪用が観測されたと報告されています。
報道では、ワーカーのクラッシュにつながるほか、条件によってはリモートコード実行の可能性があるとされています。
広く使われるNGINX系製品に影響するため、サーバー運用への影響が大きい可能性があります。すでに悪用観測があるとされる点から、早期の確認と対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 3 sources。
- 実悪用・ゼロデイ文脈。
- 技術詳細・再現情報あり。
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

- 利用中のNGINX/OpenとNGINX Plusのバージョンを確認し、影響範囲を特定する。
- ベンダーや公的な案内を確認し、修正版や回避策が出ていれば速やかに適用する。
- 異常なワーカー停止や再起動、関連するログの増加がないか監視を強化する。

#### 関連する対象

| <nobr>種類</nobr> | 名称 | <nobr>関係</nobr> | <nobr>確度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2026-42945 | 主要CVE | 1.00 |

#### 参照リンク

| <nobr>種別</nobr> | 参照 | <nobr>確認すべき内容</nobr> |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-42945](https://nvd.nist.gov/vuln/detail/CVE-2026-42945) | <nobr>CVE概要、CVSS、CWE、参照情報</nobr> |
| <nobr>出典</nobr> | [NGINX CVE-2026-42945 Exploited in the Wild, Causing Worker Crashes and Possible ](https://thehackernews.com/2026/05/nginx-cve-2026-42945-exploited-in-wild.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [NGINXでリモートコード実行の脆弱性が発見される、影響を受けるバージョンはこれ](https://gigazine.net/news/20260515-nginx-remote-code-execution) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [18-Year-Old NGINX Rewrite Module Flaw Enables Unauthenticated RCE](https://thehackernews.com/2026/05/18-year-old-nginx-rewrite-module-flaw.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CVE-2026-42945 NGINX ngx_http_rewrite_module vulnerability](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-42945) | <nobr>内容確認・補足情報</nobr> |

#### 反応シグナル

- SNS反応: 反応未確認。
- 日本語圏一次情報: なし。
- 日本語圏メディア波及: 中。
- 日本語圏反応: 反応あり・低信頼。
- 技術者コミュニティ反応: 弱。
- 開発者コミュニティ反応: 反応あり。
- 攻撃・悪用観測シグナル: 技術詳細・悪用観測あり。
- 継続観測: 継続。

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
| [Week in review: CiscoがSD-WANの0-dayを修正、未修正のMicrosoft Exchange Serverの脆弱性が悪用される](https://helpnetsecurity.com/2026/05/17/week-in-review-cisco-patches-sd-wan-0-day-unpatched-microsoft-exchange-server-flaw-exploited) | 37.0 | 38.0 | 43.0 |
| [Taskhost Windows Tasksにおけるローカル権限昇格の脆弱性（CVE-2025-60710）](https://github.com/Wh04m1001/CVE-2025-60710) | 25.0 | 82.0 | 81.0 |
| [CVE-2026-46483 Vim: tar#Vimuntarにおけるshellescapeのspecialフラグ不足によるコマンドインジェクション](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-46483) | 24.0 | 46.0 | 38.0 |
| [UniFi Accessにおけるリモートコード実行の脆弱性（CVE-2025-52665）](https://catchify.sa/post/cve-2025-52665-rce-in-unifi-os-25-000) | 20.0 | 46.0 | 50.0 |
| [Netskopeにおけるクロステナント認証バイパスの脆弱性](https://blog.amberwolf.com/blog/2025/august/advisory---netskope-cross-tenant-authentication-bypass) | 20.0 | 38.0 | 42.0 |
| [Citrix NetScalerのメモリリークと反射型XSS（CVE-2025-12101）](https://bit.ly/48bPzCO) | 20.0 | 34.0 | 50.0 |
| [セキュリティ：4バイト、1つの嘘 - カーネルポインタに対するSMAP不要の信用詐欺（CVE-2025-50168）](https://oobs.io/posts/four-bytes-one-lie) | 20.0 | 28.0 | 50.0 |
| [Security: 低権限のCOMでBoot Configuration Data (BCD)を削除可能な脆弱性（CVE-2025-59253）](https://warpnet.nl/blog/deleting-the-bcd-through-com-as-low-privileged-user) | 20.0 | 28.0 | 50.0 |
| [Spring ELを用いて環境変数とシステムプロパティを露出させる攻撃（CVE-2025-41253）](https://psytester.github.io/CVE-2025-41253) | 20.0 | 28.0 | 50.0 |
| [CVE-2026-8328: FTP PASVのSSRF、ftpcp()が実際のピアアドレスを使わずサーバー提供のPASVホストアドレスを信頼する問題](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-8328) | 20.0 | 28.0 | 38.0 |
| [CVE-2026-8368: Perl向けLWP::UserAgent 6.83未満におけるクロスオリジンリダイレクト時のAuthorizationおよびProxy-Authorizationヘッダー漏えい](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-8368) | 20.0 | 28.0 | 38.0 |
| [CVE-2026-44283 etcd: etcdトランザクションのPrevKvによる読み取りアクセスがRBAC認可チェックを回避する可能性](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-44283) | 20.0 | 28.0 | 38.0 |
| [Tycoon2FAがデバイスコードフィッシングでMicrosoft 365アカウントを乗っ取る](https://bleepingcomputer.com/news/security/tycoon2fa-hijacks-microsoft-365-accounts-via-device-code-phishing) | 20.0 | 20.0 | 42.0 |
| [PLEASE_READ_ME：MySQLサーバーを破壊する機会主義的ランサムウェア](https://akamai.com/blog/security/please-read-me-opportunistic-ransomware-devastating-mysql-servers) | 10.0 | 30.0 | 42.0 |
| [Security: iBootログの難読化解除と再難読化](https://nyansatan.github.io/iboot-log-deobfuscation) | 10.0 | 20.0 | 48.0 |
| [サイバーリスクインテリジェンスの未来](https://bitsight.com/de/blog/die-zukunft-liegt-cyber-risk-intelligence) | 10.0 | 20.0 | 42.0 |
| [OpenAI Sora 2のセキュリティ分析：マルチモーダルLLMを動かすシステムプロンプトの解明](https://mindgard.ai/resources/openai-sora-system-prompts) | 10.0 | 20.0 | 42.0 |
| [Hack: Microsoft Windows向けの多目的リモートアクセスツール（オープンソース）](https://github.com/DarkCoderSc/OptixGate) | 10.0 | 20.0 | 42.0 |
| [MixMaster MMORPGのリバースエンジニアリング解析](https://3r4y.github.io/posts/mixmasterreverseengineering) | 10.0 | 20.0 | 42.0 |
| [Windowsセキュリティ研究向けカーネル脆弱性機能フレームワーク（KVC）への攻撃](https://github.com/wesmar/kvc) | 10.0 | 20.0 | 42.0 |
| [JDWP経由でデバッグ可能なAndroidプロセスにFridaを動的アタッチするハック（root不要）](https://github.com/frankheat/frida-jdwp-loader) | 10.0 | 20.0 | 42.0 |
| [Win FS minifilter driverで信頼されていないプロセスから機密データを保護する方法](https://github.com/KiExitDispatcher/NoMoreStealers) | 10.0 | 20.0 | 42.0 |
| [Hack: C/C++シェルコード生成用ツールキット「Extensible Position Independent Code」](https://github.com/Print3M/epic) | 10.0 | 20.0 | 42.0 |
| [Hack: .pdbファイルに記録されたデバッグ情報を視覚的に確認するツール](https://github.com/diversenok/DiaSymbolView) | 10.0 | 20.0 | 42.0 |

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
