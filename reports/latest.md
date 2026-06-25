# 📡 サイレーダー 2026-06-26 05:00 JST

このレポートは、2026-06-25 17:00 JST〜2026-06-26 05:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。



## 🔥 今回の温度感サマリ

- 観測トピック数: 111
- [音声で扱う想定のトピック](#audio-topics): 7
- [GitHubのみ掲載想定のトピック](#github-only-topics): 0
- [低温だが記録しておくトピック](#low-record-topics): 79

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Why patch directives only go so far](#topic-15996) | 56.0 | 77.0 | 66.0 | 音声 | 温度感上位枠 |
| 2 | [Stealthy new backdoor surfaces in attacks on multiple sectors](#topic-19311) | 36.0 | 30.0 | 42.0 | 音声 | 温度感上位枠 |
| 3 | [New macOS malware embeds fake errors to confuse AI analysis tools](#topic-19298) | 35.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 4 | [STOCKSTAY Another Day: The Latest Addition to Turla’s Intelligence Gathering Apparatus](#topic-19314) | 35.0 | 20.0 | 42.0 | 音声 | 温度感上位枠 |
| 5 | [Lantronix Serial-to-IP Converter Flaw Exploited in Attacks After OT Threat Warning](#topic-19075) | 33.0 | 46.0 | 55.0 | 音声 | 温度感上位枠 |
| 6 | [ANY.RUN & Torq Integration: Scale Triage & Respond with Confidence](#topic-19360) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |
| 7 | [New Gaslight macOS Malware Uses Prompt Injection to Disrupt AI-Assisted Analysis](#topic-19389) | 33.0 | 20.0 | 42.0 | 音声 | AI×Security枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-15996"></a>

### 1. Why patch directives only go so far

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>C⁠V⁠E</nobr> / <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>K⁠E⁠V</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>認⁠証⁠バ⁠イ⁠パ⁠ス</nobr> / <nobr>I⁠o⁠C</nobr> / <nobr>政⁠策⁠・⁠規⁠制</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 再燃 |
| <nobr>温⁠度⁠感</nobr> | 56.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 77.0 |
| <nobr>確⁠度</nobr> | 66.0 |

#### 概要

Check Point製品のVPN関連脆弱性CVE-2026-50751について、認証バイパスとして公開情報で注意喚起が続いています。
複数の報道やセキュリティ機関の案内では、すでに実際の悪用が観測されており、Qilin系ランサムウェア文脈でも言及されています。
脆弱性の修正だけでなく、既に侵入された環境では被害拡大や痕跡確認が重要になるためです。加えて、技術情報の公開により、今後は機会的な攻撃が増える可能性がある点が注目されています。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 7 sources。
- 実悪用・ゼロデイ文脈。
- 技術詳細・再現情報あり。
- 脅威・攻撃キャンペーン文脈。
- 技術・開発者系ソース観測: 観測あり。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。
- 技術詳細により影響確認が進みやすい。
- RCEまたは認証バイパス系。
- ランサムウェア文脈。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 技術詳細・悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 技術詳細、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Check Pointの公式対策状況とJPCERT/CC・IPAの注意喚起を確認し、該当製品の適用状況を点検する。
- VPN機器の認証関連ログや不審な接続履歴を確認し、既存侵害の兆候がないか調べる。
- 該当構成に該当するかを確認し、必要に応じて設定見直しや追加の監視を実施する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2024-24919 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-50751 | 関連CVE | 1.00 |
| 脆弱性 | CVE-2026-50752 | 関連CVE | 1.00 |
| 製品 | Exchange | 言及あり | 0.80 |
| ransomware_group | Qilin | 主題 | 0.80 |
| 製品 | Connect Secure | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-50751](https://nvd.nist.gov/vuln/detail/CVE-2026-50751) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Why patch directives only go so far](https://cyberscoop.com/why-security-patching-is-not-enough-cve-2026-50751-op-ed/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Researchers release details, PoC for exploited Check Point VPN flaw (CVE-2026-50](https://www.helpnetsecurity.com/2026/06/12/cve-2026-50751-poc-exploit/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [注意喚起: Check Point Software Technologies社製品における認証バイパスの脆弱性（CVE-2026-50751）に関する注意喚起](https://www.jpcert.or.jp/at/2026/at260016.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Check Point Software Technologies製品の脆弱性対策について(CVE-2026-50751)](https://www.ipa.go.jp/security/security-alert/2026/alert20260610.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Ransomware crims got a month-long head start on Check Point VPN 0-day that now h](https://www.theregister.com/cyber-crime/2026/06/08/attackers-had-month-long-head-start-on-patched-check-point-vpn-zero-day/5252438) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Check Point VPN Zero-Day Exploited in the Wild (CVE-2026-50751)](https://www.rapid7.com/blog/post/etr-critical-check-point-vpn-zero-day-exploited-in-the-wild-cve-2026-50751) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Critical Check Point VPN Flaw Exploited to Bypass Passwords in IKEv1 Setups](https://thehackernews.com/2026/06/critical-check-point-vpn-flaw-exploited.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: あり（1件）。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補あり（URL 79件以上 / 該当CVE 2件）。

---

<a id="topic-19311"></a>

### 2. Stealthy new backdoor surfaces in attacks on multiple sectors

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>ラ⁠ン⁠サ⁠ム⁠ウ⁠ェ⁠ア</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>T⁠T⁠P</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 36.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 30.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Symantecによると、比較的新しいバックドア「Mistic」が、保険、教育、IT、専門サービスなど複数業界への攻撃で2026年4月以降に使われているとされています。
関連が指摘されるWoodgnat（KongTuke）は、ランサムウェア関連の侵入足場提供者として複数の攻撃グループと結び付けられてきました。
初期侵入の段階で使われる可能性があるマルウェアは、後続の侵害やランサムウェア被害につながるおそれがあるため注意が必要です。
特定業界に限定されず複数分野で観測されている点も、監視対象を広げる必要性を示しています。

#### 温度感の理由

##### 温度感
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- ランサムウェア文脈。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 不審な初期侵入の兆候を前提に、認証情報の保護と多要素認証の徹底を見直す。
- 外部公開サービスやリモート接続経路の監視を強化し、異常なログインや永続化の痕跡を確認する。
- EDRやメール・Webフィルタリングの検知ルールを最新化し、関連する侵害指標の有無を点検する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| ransomware_group | Akira | 主題 | 0.80 |
| ransomware_group | Qilin | 主題 | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Stealthy new backdoor surfaces in attacks on multiple sectors](https://www.helpnetsecurity.com/2026/06/25/mistic-backdoor-woodgnat-attacks/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-19298"></a>

### 3. New macOS malware embeds fake errors to confuse AI analysis tools

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

macOS向けの新しいマルウェア「Gaslight」が、AI支援の解析ツールを混乱させることを狙って作られていると報告されています。
実行ファイル内に、プロンプトインジェクション文字列や偽のデバッグ情報を埋め込むことで、解析結果を誤らせる意図があるとされています。
AIを使ったマルウェア分析が広がる中、解析を妨害するためにAIの弱点を突く手口が確認された点が注目されます。
自動解析の出力だけに依存すると、見落としや誤判定につながる可能性があります。

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

- AI支援ツールの結果は参考情報として扱い、従来の静的・動的解析と突き合わせる。
- 不自然なエラー表示やデバッグ文字列があっても、実害や挙動を別途確認する。
- macOS向け検体の解析手順では、AIへの指示文混入やノイズ混入を前提にレビュープロセスを設計する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New macOS malware embeds fake errors to confuse AI analysis tools](https://www.bleepingcomputer.com/news/security/new-macos-malware-embeds-fake-errors-to-confuse-ai-analysis-tools/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-19314"></a>

### 4. STOCKSTAY Another Day: The Latest Addition to Turla’s Intelligence Gathering Apparatus

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>I⁠o⁠C</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>ボ⁠ッ⁠ト⁠ネ⁠ッ⁠ト</nobr> / <nobr>脅⁠威⁠ア⁠ク⁠タ⁠ー</nobr> / <nobr>W⁠i⁠n⁠d⁠o⁠w⁠s</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>攻⁠撃⁠キ⁠ャ⁠ン⁠ペ⁠ー⁠ン</nobr> / <nobr>ク⁠ラ⁠ウ⁠ド</nobr> / <nobr>地⁠政⁠学⁠・⁠サ⁠イ⁠バ⁠ー⁠紛⁠争</nobr> / <nobr>防⁠御⁠・⁠運⁠用</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 35.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

Google Threat Intelligence Groupは、ロシア系脅威グループTurlaが少なくとも2022年末から開発・運用してきたとみられる.<wbr>NETバックドア「STOCKSTAY」を分析し、その機能や運用の変化を公開しました。
STOCKSTAYは、WebSocketを使ったC2通信や複数コンポーネント構成、環境に応じた設定の切り替えなどを特徴とし、ウクライナの政府・軍関連組織や欧州の外交関連組織を狙った事例が報告されています。
Turlaは長期にわたり活動が確認されている諜報系グループで、今回の分析は同グループの新たなツール体系と運用パターンの理解に役立ちます。
攻撃で使われた誘導文書や配布経路が複数確認されており、防御側は初期侵入から横展開まで含めて監視を見直す必要があります。

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

- Windows環境での不審なRDPファイル、HTA、MSI、LNKの実行や、正規アプリを装ったファイル名に注意する。
- WebSocket通信や外部モジュール化された.<wbr>NETコンポーネント、レジストリ永続化の兆候を重点的に監視する。
- 外交・防衛・教育関連の業務文脈を装う誘導が見られるため、メールとダウンロード元の妥当性確認を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-8088 | 関連CVE | 1.00 |
| ベンダー | Microsoft | 言及あり | 0.80 |
| 製品 | Exchange | 言及あり | 0.80 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [STOCKSTAY Another Day: The Latest Addition to Turla’s Intelligence Gathering App](https://cloud.google.com/blog/topics/threat-intelligence/stockstay-turla-intelligence-gathering/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測あり。
- PoC/検証コード候補: 候補あり（URL 37件以上 / 該当CVE 1件）。

---

<a id="topic-19075"></a>

### 5. Lantronix Serial-to-IP Converter Flaw Exploited in Attacks After OT Threat Warning

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>C⁠V⁠E</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 55.0 |

#### 概要

CISAがLantronix EDS5000 Seriesに影響する深刻な脆弱性CVE-2025-67038について、実際の悪用が確認されているとして注意喚起しました。
対象はシリアル・トゥ・IP変換機器で、コードインジェクションにより不正なコード実行につながるおそれがあるとされています。
OT環境やネットワーク機器は一度影響を受けると、周辺システムにも広く波及する可能性があります。
すでに悪用が観測されているため、未対策機器の有無確認と修正適用の優先度が高い事案です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 2 sources。
- 実悪用・ゼロデイ文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 攻撃・悪用観測シグナル

- シグナル種別: 悪用観測あり。
- 公開PoC/Exploitコード: 未確認。
- 確認方針: 公開PoCの有無とは分けて、悪用観測、IoC、緩和策、ベンダー公式情報を確認します。

#### 担当者向け確認ポイント

- Lantronix EDS5000 Seriesの利用有無を棚卸しし、影響範囲を特定する。
- メーカー提供の修正や回避策の適用状況を確認し、優先的に更新する。
- 外部公開状況や不審な通信・設定変更がないか、機器周辺の監視を強化する。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> |
|---|---|---|---:|
| 脆弱性 | CVE-2025-67038 | 関連CVE | 1.00 |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2025-67038](https://nvd.nist.gov/vuln/detail/CVE-2025-67038) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Lantronix Serial-to-IP Converter Flaw Exploited in Attacks After OT Threat Warni](https://www.securityweek.com/lantronix-serial-to-ip-converter-flaw-exploited-in-attacks-after-ot-threat-warning/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [CISA Warns Critical Lantronix EDS5000 Flaw Is Being Actively Exploited](https://thehackernews.com/2026/06/cisa-warns-critical-lantronix-eds5000.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補あり（URL 1件以上 / 該当CVE 1件）。

---

<a id="topic-19360"></a>

### 6. ANY.RUN & Torq Integration: Scale Triage & Respond with Confidence

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>防⁠御⁠・⁠運⁠用</nobr> / <nobr>フ⁠ィ⁠ッ⁠シ⁠ン⁠グ</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

ANY.RUNが、TorqのAI SOCプラットフォームとの連携を紹介しました。
アラートの文脈不足で真偽判断が難しいSOC業務に対し、マルウェアやフィッシングの判定情報と実用的なインテリジェンスを提供し、トリアージと対応の効率化を狙う内容です。
アラート疲れや誤検知対応の負担が大きいSOCにとって、初動判断を速める連携として注目されます。
脅威の切り分け精度が上がれば、対応の優先順位付けや運用の平準化に役立つ可能性があります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- 既存のSOC自動化基盤に、判定結果やコンテキスト情報をどう取り込むか確認する。
- マルウェア・フィッシング判定を他の検知結果と突き合わせ、誤検知低減に使えるか評価する。
- 連携で得られる情報を、アラートの優先順位付けや封じ込め判断の補助にどう反映するか整理する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [ANY.RUN & Torq Integration: Scale Triage & Respond with Confidence](https://any.run/cybersecurity-blog/torq-integration/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 高。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

---

<a id="topic-19389"></a>

### 7. New Gaslight macOS Malware Uses Prompt Injection to Disrupt AI-Assisted Analysis

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>A⁠I</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | AI×Security枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 33.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 20.0 |
| <nobr>確⁠度</nobr> | 42.0 |

#### 概要

macOS向けの新たなマルウェア「Gaslight」が確認され、解析に使うAIツールを混乱させることを狙ったプロンプト注入の文字列を含んでいると報告されています。
Rustで実装された情報窃取系の不正プログラムとみられ、AI支援の分析を妨げることを目的とした珍しい手口として注目されています。
脅威側がAI支援の解析環境そのものを意識して対策を組み込んでいる可能性があり、分析フローへの影響が懸念されます。
AIを使った初動調査では、モデルの出力をそのまま信頼せず、従来の静的・動的解析と併用する重要性が高まります。

#### 温度感の理由

##### 温度感
- AI×Security文脈。
- 脅威・攻撃キャンペーン文脈。

##### 実務影響
- データ分類、権限管理、監査、外部接続管理などの確認観点があります。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- AI支援分析では、入力文字列に誘導的な文言が含まれていないかを前提に、出力の妥当性を人手で確認する。
- macOS端末の情報窃取系マルウェアとして、通常のEDR検知に加え、未知のRust系実行ファイルや不審な挙動の監視を強化する。
- 解析担当者向けに、AIツールが分析中断や拒否を返した場合の再検証手順をあらかじめ用意する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [New Gaslight macOS Malware Uses Prompt Injection to Disrupt AI-Assisted Analysis](https://thehackernews.com/2026/06/new-gaslight-macos-malware-uses-prompt.html) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。
- PoC/検証コード候補: 候補なし。

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
| [Windows脅威によるCOMの利用入門](https://blog.talosintelligence.com/introduction-to-com-usage-by-windows-threats/) | 30.0 | 20.0 | 42.0 |
| [欧州を標的としたランサムウェア攻撃の大幅増加、新報告書が警告](https://www.infosecurity-magazine.com/news/increase-ransomware-europe/) | 28.0 | 30.0 | 42.0 |
| [欧州がランサムウェアの標的として最も狙われる地域に変化](https://www.darkreading.com/cybersecurity-analytics/europe-evolves-ransomware-favorite-region) | 28.0 | 30.0 | 42.0 |
| [RICO法を用いて3つの悪名高いマルウェアネットワークが摘発され、戦略転換が示された](https://www.itpro.com/security/malware/this-operation-marked-a-shift-in-strategy-three-notorious-malware-networks-have-been-taken-down-using-rico-legislation) | 28.0 | 20.0 | 42.0 |
| [ClickFixおよびModeloRATキャンペーンでKongTukeに関連する新たなMisticバックドア](https://thehackernews.com/2026/06/new-mistic-backdoor-linked-to-kongtuke.html) | 28.0 | 20.0 | 42.0 |
| [IOCを超えて：AIを活用した脅威インテリジェンス](https://blog.talosintelligence.com/beyond-iocs-ai-enabled-threat-intelligence/) | 27.0 | 20.0 | 42.0 |
| [AWS Summit Japan セッションの約半数がAIエージェント、「最も強い力に」](https://xtech.nikkei.com/atcl/nxt/column/18/03664/062500001/) | 26.0 | 20.0 | 42.0 |
| [番狂わせ続きのサッカーW杯、その背景に“AI参謀”あり？ すべての参加チームが使う「FIFA AI Pro」とは](https://ascii.jp/elem/000/004/413/4413350/?rss=) | 26.0 | 20.0 | 42.0 |
| [公取委のとあるポスターが物議 「アニメ取引適正化」訴えるもイラストに生成AI 採用した理由とは？](https://www.itmedia.co.jp/news/articles/2606/25/news117.html) | 26.0 | 20.0 | 42.0 |
| [pydicomとpynetdicomライブラリ](https://www.cisa.gov/news-events/ics-advisories/icsma-26-176-01) | 25.0 | 46.0 | 50.0 |
| [Checksum API AgentがステートフルなAPIテストを生成・維持](https://www.helpnetsecurity.com/2026/06/25/checksum-api-agent-generates-and-maintains-stateful-api-tests/) | 25.0 | 20.0 | 42.0 |
| [Reco Agent SecurityでAIエージェントの管理を強化し、リスクを低減](https://www.helpnetsecurity.com/2026/06/25/reco-agent-security-helps-organizations-govern-ai-agents-and-reduce-exposure/) | 25.0 | 20.0 | 42.0 |
| [Mitigaがクラウド、SaaS、ID、AI保護向けのAgentic Runtime Securityを発表](https://www.helpnetsecurity.com/2026/06/25/mitiga-agentic-runtime-security/) | 25.0 | 20.0 | 42.0 |
| [AIコストモデルはトークン単価で止まるが、請求額は止まらない](https://www.akamai.com/blog/ai/2026/jun/ai-cost-model-stops-token-price-bill-doesnt) | 25.0 | 20.0 | 42.0 |
| [AIとコンプライアンスが新たなセキュリティ運用モデルを迫る理由](https://www.rapid7.com/blog/post/it-experts-video-series-ai-compliance-force-new-security-operating-models) | 25.0 | 20.0 | 42.0 |
| [Runlayer、シリーズAで3000万ドルを調達](https://www.securityweek.com/runlayer-raises-30-million-in-series-a-funding/) | 25.0 | 20.0 | 42.0 |
| [ThreatsDay Bulletin: Smart TV Proxyware、24年越しのcurlバグ、AI犯罪フォーラムほか13件の話題](https://thehackernews.com/2026/06/threatsday-bulletin-smart-tv-proxyware.html) | 25.0 | 20.0 | 42.0 |
| [runZero 5.0、露出管理を統合してリスク低減を加速](https://www.helpnetsecurity.com/2026/06/25/runzero-5-0/) | 25.0 | 20.0 | 42.0 |
| [BlackLine、CFO向けAI監視機能を備えたAgentic Financial Operations Platformを強化](https://www.helpnetsecurity.com/2026/06/25/blackline-agentic-financial-operations-platform/) | 25.0 | 20.0 | 42.0 |
| [自動化されたAI脆弱性スキャンへの信頼が9%まで低下、新調査で判明](https://www.infosecurity-magazine.com/news/trust-ai-vulnerability-scanning/) | 25.0 | 20.0 | 42.0 |
| [2026年のSMB脅威動向の内側：フィッシングや詐欺から偽AIツールまで](https://securelist.com/smb-threat-report-2026/120357/) | 25.0 | 20.0 | 42.0 |
| [Seemplicity AI Analystsが修復対応を実行可能なリスクに集中させる](https://www.helpnetsecurity.com/2026/06/25/seemplicity-ai-analysts-focus-remediation-on-exploitable-risks/) | 25.0 | 20.0 | 42.0 |
| [YesWeHack、AI搭載エージェントでペネトレーションテストを自動化](https://www.helpnetsecurity.com/2026/06/25/yeswehack-automates-penetration-testing-with-ai-powered-agents/) | 25.0 | 20.0 | 42.0 |
| [Schneider Electric PowerLogic P7の脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-176-07) | 24.0 | 46.0 | 50.0 |
| [H.VIEW HV-500S6 IPカメラ](https://www.cisa.gov/news-events/ics-advisories/icsa-26-176-05) | 24.0 | 46.0 | 50.0 |
| [Daktronicsコントローラーファームウェア](https://www.cisa.gov/news-events/ics-advisories/icsa-26-176-04) | 24.0 | 46.0 | 50.0 |
| [EVoke Systems Charging Station Management Systemの脆弱性情報](https://www.cisa.gov/news-events/ics-advisories/icsa-26-176-02) | 24.0 | 46.0 | 50.0 |
| [GitLabのコード実行および情報漏えい脆弱性を修正](https://www.securityweek.com/gitlab-patches-code-execution-information-disclosure-vulnerabilities/) | 22.0 | 28.0 | 42.0 |
| [Forrester WaveでMicrosoftがエンドポイント管理プラットフォームのリーダーに選出](https://www.microsoft.com/en-us/security/blog/2026/06/25/microsoft-a-leader-in-the-forrester-wave-for-endpoint-management-platforms/) | 22.0 | 20.0 | 42.0 |
| [関連7サイトで障害、原因調査や復旧急ぐ - 名鉄協商](https://www.security-next.com/186390) | 22.0 | 20.0 | 42.0 |
| [サーバから個人情報が流出した可能性 - 現代仏壇](https://www.security-next.com/186268) | 22.0 | 20.0 | 42.0 |
| [中学校の生徒情報含む修学旅行しおりを紛失 - 名古屋市](https://www.security-next.com/186334) | 22.0 | 20.0 | 42.0 |
| [県内中高校向けのメールで誤送信 - 香川県](https://www.security-next.com/186338) | 22.0 | 20.0 | 42.0 |
| [インドネシア子会社でデータ外部送信が判明 - ダイキョーニシカワ](https://www.security-next.com/186263) | 22.0 | 20.0 | 42.0 |
| [OHIF ViewerのDICOM関連セキュリティ問題](https://www.cisa.gov/news-events/ics-advisories/icsma-26-176-02) | 21.0 | 28.0 | 50.0 |
| [DAZN、W杯日本×スウェーデン戦で「映像の乱れ」に注意喚起 朝8時キックオフ、通勤時間帯を直撃](https://www.itmedia.co.jp/news/articles/2606/25/news136.html) | 21.0 | 20.0 | 42.0 |
| [押さえておきたい脅威アクター - 敵を知って攻撃をブロック 第4回 【脅威アクター解説】Lazarusとは？日本も標的とする攻撃手法と最新動向](https://news.mynavi.jp/techplus/article/threatactors-4/) | 21.0 | 20.0 | 42.0 |
| [Delta Electronics DTM Softの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-176-06) | 20.0 | 28.0 | 50.0 |
| [Yokogawa FAST/TOOLSおよびCI Server](https://www.cisa.gov/news-events/ics-advisories/icsa-26-176-01) | 20.0 | 28.0 | 50.0 |
| [Horner Automation Cscapeの脆弱性](https://www.cisa.gov/news-events/ics-advisories/icsa-26-176-03) | 20.0 | 28.0 | 50.0 |
| [Chromeを更新して重大なブラウザーのセキュリティ脆弱性を修正する](https://www.malwarebytes.com/blog/news/2026/06/update-chrome-to-patch-critical-browser-security-flaws) | 20.0 | 28.0 | 50.0 |
| [偽のドメイン更新メールでサイト運営者をだまして詐欺師に支払わせる手口](https://www.malwarebytes.com/blog/threat-intel/2026/06/fake-domain-renewal-emails-trick-website-owners-into-paying-scammers) | 20.0 | 20.0 | 48.0 |
| [地元警察の癒着でアジアの詐欺拠点への取り締まりが妨げられる](https://www.darkreading.com/threat-intelligence/police-collusion-crackdown-asian-scam-centers) | 20.0 | 20.0 | 42.0 |
| [DHS長官、CISA候補者と大統領が面会したと明かす　同庁は600人採用を計画](https://therecord.media/cisa-director-nominee-workforce-hires-mullin-house-hearing) | 20.0 | 20.0 | 42.0 |
| [MicrosoftがWindows 10の無料ESUサポートを2027年10月まで延長](https://www.bleepingcomputer.com/news/microsoft/microsoft-quietly-extends-free-windows-10-esu-support-to-october-2027/) | 20.0 | 20.0 | 42.0 |
| [「Parcel Expert」を名乗る求人に注意：それはパーセル・ミュール詐欺です](https://www.malwarebytes.com/blog/scams/2026/06/beware-of-parcel-expert-job-offers-theyre-parcel-mule-scams) | 20.0 | 20.0 | 42.0 |
| [米連邦裁判所、トランプ氏の選挙対策重視の大統領令を違法と判断](https://cyberscoop.com/judge-strikes-down-trump-election-executive-order/) | 20.0 | 20.0 | 42.0 |
| [新しいMCP仕様：セキュリティチームが備えるべきこと](https://www.akamai.com/blog/security-research/2026/jun/new-mcp-specification-security-teams-must-prepare) | 20.0 | 20.0 | 42.0 |
| [PirloTVのスポーツ海賊版ネットワークが44ドメイン押収で阻止される](https://www.bleepingcomputer.com/news/security/pirlotv-sports-piracy-network-disrupted-as-44-domains-seized/) | 20.0 | 20.0 | 42.0 |
| [NIST、リモートアクセスツールを利用する水道事業者向けにセキュリティガイダンスを提供](https://www.cybersecuritydive.com/news/water-utilities-remote-access-nist-guidance/823776/) | 20.0 | 20.0 | 42.0 |
| [Bluekitフィッシングキットがブラウザ中間者攻撃を採用しログイン情報を窃取](https://www.bleepingcomputer.com/news/security/bluekit-phishing-kit-adopts-browser-in-the-middle-for-login-theft/) | 20.0 | 20.0 | 42.0 |
| [ロシアが契約解除後もCellebriteで人権活動家のスマートフォンに侵入](https://cyberscoop.com/russia-cellebrite-activist-phone-hacking/) | 20.0 | 20.0 | 42.0 |
| [ロシアの乳業会社がサイバー攻撃で業務妨害か](https://therecord.media/russia-dairy-producter-cyberattack-ufa) | 20.0 | 20.0 | 42.0 |
| [サイバーリスクの進化に伴い、保険業界が防御策を強化](https://www.cybersecuritydive.com/news/cyber-risk-insurance-industry-guardrails/823762/) | 20.0 | 20.0 | 42.0 |
| [DraftKingsハック事件で「Snoopy」として知られるミネソタ州の男に判決](https://cyberscoop.com/draftkings-hack-sentencing-nathan-austad-snoopy/) | 20.0 | 20.0 | 42.0 |
| [Ciscoの脆弱性、公開数か月前に悪用かとGoogleが警告](https://www.infosecurity-magazine.com/news/cisco-vulnerability-exploited/) | 20.0 | 20.0 | 42.0 |
| [効果的な不正防止の4つの高度化](https://www.bleepingcomputer.com/news/security/the-four-elevations-of-effective-fraud-prevention/) | 20.0 | 20.0 | 42.0 |
| [ControlMonkeyがバックアップ可視化とクラウド復旧準備態勢を連携](https://www.helpnetsecurity.com/2026/06/25/controlmonkey-connects-backup-visibility-with-cloud-recovery-readiness/) | 20.0 | 20.0 | 42.0 |
| [Proxyサービスに利用された2,000万件の米国IP接続](https://www.infosecurity-magazine.com/news/twenty-million-us-ip-connections/) | 20.0 | 20.0 | 42.0 |
| [Veritoneが証拠分析とコンプライアンスレビューを効率化するAssessを発表](https://www.helpnetsecurity.com/2026/06/25/veritone-introduces-assess-to-streamline-evidence-analysis-and-compliance-reviews/) | 20.0 | 20.0 | 42.0 |
| [ウクライナ国営郵便事業者、サイバー攻撃後にアプリ障害を報告](https://therecord.media/ukraine-state-postal-operator-reports-disruption) | 20.0 | 20.0 | 42.0 |
| [Cal Water、イランのHandalaによるサイバー攻撃でOTシステム侵害なしと発表](https://www.securityweek.com/cal-water-finds-no-evidence-of-ot-activity-after-hackers-claimed-they-could-disrupt-water-supply/) | 20.0 | 20.0 | 42.0 |
| [ハッカーは企業が公表するよりも速く脆弱性を悪用している](https://www.itpro.com/security/hackers-are-exploiting-flaws-faster-than-companies-can-disclose-them) | 20.0 | 20.0 | 42.0 |
| [ランタイムシグナルを用いたクラウド環境における隠れた攻撃経路の解明](https://www.wiz.io/blog/runtime-signals-in-security-graph) | 20.0 | 20.0 | 42.0 |
| [CISAの新ガイド、政府機関のゼロトラスト導入に向けたSASE採用を支援](https://www.infosecurity-magazine.com/news/cisa-sase-tic-3-0-zero-trust/) | 20.0 | 20.0 | 42.0 |
| [NDRの有効性をRichard Bejtlichが語る：神話の時代を生き抜くために](https://thehackernews.com/2026/06/surviving-mythos-era-richard-bejtlich.html) | 20.0 | 20.0 | 42.0 |
| [macOSの脆弱性で標準ユーザーがEDRとMDMを無効化可能に](https://www.infosecurity-magazine.com/news/macos-xpc-flaw-disable-edr-mdm/) | 20.0 | 20.0 | 42.0 |
| [ハッカー、6万件の賭けアカウント侵害攻撃で懲役18か月](https://www.helpnetsecurity.com/2026/06/25/hacker-sentenced-draftkings-credential-stuffing-attac/) | 20.0 | 20.0 | 42.0 |
| [DLPインシデントの滞留は解消すべき課題です](https://www.security.com/product-insights/dlp-incident-backlog) | 20.0 | 20.0 | 42.0 |
| [Flareが新たなCTI機能とOktaサポートを発表](https://www.helpnetsecurity.com/2026/06/25/flare-cti-okta/) | 20.0 | 20.0 | 42.0 |
| [Curlで修正された25年前の脆弱性](https://www.securityweek.com/25-year-old-vulnerability-patched-in-curl/) | 20.0 | 20.0 | 42.0 |
| [Entrust、ハイリスク取引時のユーザー確認に生体認証を活用](https://www.helpnetsecurity.com/2026/06/25/entrust-biometric-authentication/) | 20.0 | 20.0 | 42.0 |
| [Elite Network、会員の個人データ露出後にハッキング被害を公表](https://www.malwarebytes.com/blog/privacy/2026/06/elite-network-says-it-was-hacked-after-members-personal-data-was-left-exposed) | 20.0 | 20.0 | 42.0 |
| [SecurityWeek ICS Cybersecurity Conference、25周年記念の特別版としてナッシュビルで開催](https://www.securityweek.com/securityweek-ics-cybersecurity-conference-heads-to-nashville-for-special-25-year-anniversary-edition/) | 20.0 | 20.0 | 42.0 |
| [Alert Enrichmentから確信ある対応へ：ANY.RUNがSOCの全ワークフローを支える方法](https://any.run/cybersecurity-blog/streamline-your-soc/) | 20.0 | 20.0 | 42.0 |
| [Bitdefender RealCheckが動画を解析し、ディープフェイクや詐欺を検出する機能](https://www.helpnetsecurity.com/2026/06/25/bitdefender-realcheck-analyzes-videos-for-deepfakes-and-fraud/) | 20.0 | 20.0 | 42.0 |
| [NIST、更新版IoTセキュリティガイダンスを公開レビューに付す](https://www.securityweek.com/nist-opens-updated-iot-security-guidance-to-public-review/) | 20.0 | 20.0 | 42.0 |
| [Google WalletにTSA Touchless IDを追加、空港保安検査を迅速化](https://www.helpnetsecurity.com/2026/06/25/google-wallet-joins-tsa-precheck-touchless-id-program/) | 20.0 | 20.0 | 42.0 |
| [誰も聞いていないとき、ポートは何を聞くのか？ 自動化されたサイバー犯罪の評価［ゲスト日誌］](https://isc.sans.edu/diary/rss/33104) | 17.0 | 20.0 | 42.0 |

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
