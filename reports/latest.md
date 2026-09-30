# 📡 サイレーダー 2026-09-30 17:00 JST

このレポートは、2026-09-30 11:00 JST〜2026-09-30 17:00 JST に収集・観測した公開情報をもとに、サイバーセキュリティ関連トピックの温度感を整理したものです。

## 🔥 今回の温度感サマリ

- 観測トピック数: 57
- [音声で扱う想定のトピック](#audio-topics): 1
- [GitHubのみ掲載想定のトピック](#github-only-topics): 1
- [低温だが記録しておくトピック](#low-record-topics): 30

| Rank | Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 | 区⁠分 | 分⁠類⁠理⁠由 |
|---:|---|---:|---:|---:|---|---|
| 1 | [Citrix NetScaler CVE-2026-88772 Exploit Details Show Pre-Auth Path to Shellcode Execution](#topic-34889) | 56.0 | 46.0 | 63.0 | GitHub | 直近音声掲載済み・新規材料ありのためGitHub継続掲載 |
| 2 | [Most open critical and high flaws are over 90 days old](#topic-35146) | 37.0 | 38.0 | 43.0 | 音声 | 温度感上位枠 |

---

<a id="audio-topics"></a>

## 🔊 音声で扱う想定のトピック

<a id="topic-35146"></a>

### 1. Most open critical and high flaws are over 90 days old

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | 音声 |
| <nobr>タ⁠グ</nobr> | <nobr>脆⁠弱⁠性</nobr> / <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> |
| <nobr>分⁠類⁠理⁠由</nobr> | 温度感上位枠 |
| <nobr>温⁠度⁠状⁠態</nobr> | 初出 |
| <nobr>温⁠度⁠感</nobr> | 37.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 38.0 |
| <nobr>確⁠度</nobr> | 43.0 |

#### 概要

Detectifyの分析では、米国・英国・北欧の顧客1,293社のインターネット公開資産に残る重大度の高い脆弱性の多くが、90日以上放置されていることが示されました。
時点観測では、北欧で97%、英国で92%、米国で86%が90日超の状態だったとされています。
重大・高リスクの脆弱性が長期未対応のままだと、攻撃対象として露出し続ける時間が長くなります。継続的な脆弱性管理や修正の優先順位付けが、実害の抑制に直結することを示す内容です。

#### 温度感の理由

##### 温度感
- 実悪用・ゼロデイ文脈。

##### 実務影響
- 悪用情報あり。

##### 確度
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- インターネット公開資産の重大・高リスク脆弱性について、年齢（放置期間）を含めて棚卸しする。
- 検出後の修正だけでなく、再検出・再発防止まで含めた運用フローを確認する。
- 修正待ちが長期化している項目を優先度順に見直し、例外扱いの妥当性を定期的に点検する。

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>出典</nobr> | [Most open critical and high flaws are over 90 days old](https://www.helpnetsecurity.com/2026/09/30/research-unpatched-vulnerabilities-backlog/) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="github-only-topics"></a>

## 📌 GitHubのみ掲載の注目トピック

<a id="topic-34889"></a>

### 1. Citrix NetScaler CVE-2026-88772 Exploit Details Show Pre-Auth Path to Shellcode Execution

#### スコアカード

| 項⁠目 | 値 |
|---|---:|
| <nobr>区⁠分</nobr> | GitHub |
| <nobr>タ⁠グ</nobr> | <nobr>ゼ⁠ロ⁠デ⁠イ</nobr> / <nobr>C⁠V⁠E</nobr> / <nobr>脆⁠弱⁠性</nobr> / <nobr>権⁠限⁠昇⁠格</nobr> / <nobr>マ⁠ル⁠ウ⁠ェ⁠ア</nobr> / <nobr>R⁠C⁠E</nobr> / <nobr>国⁠家⁠支⁠援</nobr> |
| <nobr>温⁠度⁠状⁠態</nobr> | 継続監視 |
| <nobr>温⁠度⁠感</nobr> | 56.0 |
| <nobr>実⁠務⁠影⁠響</nobr> | 46.0 |
| <nobr>確⁠度</nobr> | 63.0 |

#### 概要

Citrix NetScaler ADC/Gatewayの脆弱性CVE-2026-88772について、公開された技術情報から、事前認証での悪用につながる可能性が示されています。
複数の報道では、実際にゼロデイとして悪用され、Webシェルやトンネリング系マルウェアの展開、認証情報の窃取、内部ネットワークへの横展開が確認されたとされています。
境界機器であるNetScalerが影響を受けるため、外部公開資産への到達性が高く、侵入の起点になりやすい点が注目されています。
すでに悪用観測があるため、未対策環境では早急な確認と対応が重要です。

#### 温度感の理由

##### 温度感
- 複数ソースで確認: 4 sources。
- 実悪用・ゼロデイ文脈。
- 脅威・攻撃キャンペーン文脈。
- 現在の熱量に合わせた冷却補正。

##### 実務影響
- 悪用情報あり。

##### 確度
- 複数ソース確認。
- CVE IDあり。
- 一次・公的系ソースあり。

#### 担当者向け確認ポイント

- Citrix NetScaler ADC/Gatewayの該当バージョンと修正状況を確認し、適用可能な更新を優先して反映する。
- インターネット公開されている管理・VPN系インターフェースを点検し、想定外の改変や不審なファイル・プロセスの有無を確認する。
- 認証情報の不正利用や横展開の兆候に備え、関連ログの保全と監視強化を行う。

#### 関連する対象

| <nobr>種⁠類</nobr> | 名⁠称 | <nobr>関⁠係</nobr> | <nobr>確⁠度</nobr> | <nobr>P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t</nobr> |
|---|---|---|---:|---|
| 脆弱性 | CVE-2026-88772 | 関連CVE | 1.00 | 候補あり（URL 2件以上） |
| ベンダー | Citrix | 言及あり | 0.80 | — |
| 製品 | Citrix NetScaler ADC | 言及あり | 0.80 | — |

#### 参照リンク

| 種⁠別 | 参⁠照 | 確⁠認⁠す⁠べ⁠き⁠内⁠容 |
|---|---|---|
| <nobr>脆弱性DB</nobr> | [NVD: CVE-2026-88772](https://nvd.nist.gov/vuln/detail/CVE-2026-88772) | <nobr>CVE概要、CVSS、CWE、参⁠照情報</nobr> |
| <nobr>出典</nobr> | [Citrix NetScaler CVE-2026-88772 Exploit Details Show Pre-Auth Path to Shellcode ](https://thehackernews.com/2026/09/citrix-netscaler-cve-2026-88772-exploit.html) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Attackers exploited Citrix NetScaler zero-day for at least three weeks undetecte](https://cyberscoop.com/citrix-netscaler-zero-day-attacks-three-weeks-undetected/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Hackers exploit Citrix NetScaler zero-day to deploy web shells](https://www.bleepingcomputer.com/news/security/hackers-exploit-citrix-netscaler-zero-day-to-deploy-web-shells/) | <nobr>内容確認・補足情報</nobr> |
| <nobr>出典</nobr> | [Custom malware used in Citrix 0-day attacks targeting govt, banks, professional ](https://www.theregister.com/security/2026/09/29/custom-malware-used-in-citrix-0-day-attacks-targeting-govt-banks-professional-services/5299867) | <nobr>内容確認・補足情報</nobr> |

#### 外部反応・国内波及シグナル

- SNS反応: 観測あり・信頼度: 低。
- 国内ブックマーク反応: なし。
- 国内開発者記事: なし。
- 技術・開発者系ソース観測: 観測なし。

---

<a id="low-record-topics"></a>

## ❄️ 低温だが記録しておくトピック

音声や詳細解説には入れなかったものの、後から参照・検索・期間集計できるように残すアーカイブ枠です。
重大度が低いという意味ではなく、今回の配信枠では優先度が相対的に下がった話題を含みます。

| Topic | 温⁠度⁠感 | 実⁠務⁠影⁠響 | 確⁠度 |
|---|---:|---:|---:|
| [南アフリカ、航空管制を狙ったサイバー攻撃後に支援を要請](https://www.darkreading.com/cyberattacks-data-breaches/south-africa-help-cyberattack-air-traffic-control) | 28.0 | 30.0 | 42.0 |
| [WindowsでWSLコンテナが一般提供開始](https://www.helpnetsecurity.com/2026/09/30/microsoft-wsl-containers-available/) | 28.0 | 20.0 | 42.0 |
| [AIエージェントが「画像を貼れない」問題を勝手に解決、343組織の機密スクショ1万3000枚超をGitHubの公開リポジトリに保存していたことが判明](https://gigazine.net/news/20260930-pixelleak/) | 27.0 | 20.0 | 42.0 |
| [トランプ大統領とGoogle・Anthropic・Meta・OpenAI・SpaceXAI・NVIDIAがAIの安全管理を目指す「ホワイトハウス・超知能協定」に署名](https://gigazine.net/news/20260930-white-house-super-intelligence/) | 27.0 | 20.0 | 42.0 |
| [トランプ大統領が連邦政府内で「AI(人工知能)」表記の代わりに「SI(超知能)」表記を義務化する大統領令に署名](https://gigazine.net/news/20260930-trump-says-ai-renamed-super-intelligence/) | 27.0 | 20.0 | 42.0 |
| [OpenAIが常時稼働型のAIアシスタント「Dots」を公開、GPT‑6 Astra を搭載して専用のクラウドコンピューターで稼働](https://gigazine.net/news/20260930-openai-dots/) | 27.0 | 20.0 | 42.0 |
| [OpenAIがゲームボーイカラーっぽいゲーム機「Chromatic」とコラボしてCodexでレトロゲームを作成可能に](https://gigazine.net/news/20260930-chromatic-codex/) | 27.0 | 20.0 | 42.0 |
| [「声」もパブリシティー権の保護対象に 津田健次郎さんのAI声模倣訴訟で東京地裁が判断──削除請求自体は棄却](https://www.itmedia.co.jp/news/article/2609/30/2000001892/) | 26.0 | 20.0 | 42.0 |
| [たった4人で10カ国超を担当、飲食チェーンの海外進出を支える生成AI活用](https://www.itmedia.co.jp/news/article/2609/30/2000001789/) | 26.0 | 20.0 | 42.0 |
| [マネーフォワード、「Notion」と「Notion AI」を導入--AIネイティブな組織体制の構築と働き⽅を推進](https://japan.zdnet.com/article/35253101/) | 26.0 | 20.0 | 42.0 |
| [NTTドコモビジネス、「Oracle Autonomous AI Database」を導入--ライセンス費を43％削減](https://japan.zdnet.com/article/35253106/) | 26.0 | 20.0 | 42.0 |
| [生成AI動画巡り 声優の請求棄却](https://news.yahoo.co.jp/pickup/6597056?source=rss) | 25.0 | 20.0 | 42.0 |
| [新しい中小企業向けサイバーセキュリティサービスでAIが支援しコンサルタントが判断する仕組み](https://www.helpnetsecurity.com/2026/09/30/bh-haven-sme-cybersecurity-service/) | 25.0 | 20.0 | 42.0 |
| [税務署やe-Tax装うフィッシング、控除や還付など口実 - アプリへ不正誘導](https://www.security-next.com/190860) | 22.0 | 20.0 | 42.0 |
| [GitLab、旧ブランチ向けにセキュリティ更新 - クリティカル脆弱性を修正](https://www.security-next.com/190854) | 22.0 | 20.0 | 42.0 |
| [Mozilla、ブラウザ最新版「Firefox 157」を公開 - 脆弱性76件を解消](https://www.security-next.com/190850) | 22.0 | 20.0 | 42.0 |
| [「中国のGLM-5.3はClaude Mythos Preview級のサイバー攻撃能力を持つ一方で安全対策が不十分」とAnthropicが警告](https://gigazine.net/news/20260930-anthropic-warned-about-glm-5-3-risk/) | 22.0 | 20.0 | 42.0 |
| [GPT-6 Astraを8倍速で動かすUltrafastモードが登場＆トークン上限を引き上げた月額8万4000円のPro 500プランも登場](https://gigazine.net/news/20260930-gpt-6-astra-ultrafast/) | 22.0 | 20.0 | 42.0 |
| [アイデンティティ管理製品「SailPoint IdentityIQ」に深刻な脆弱性](https://www.security-next.com/190833) | 22.0 | 20.0 | 42.0 |
| [トークン消費85％減 Googleが脆弱性を自動修正するオープンソースハーネス「Mantis」公開](https://atmarkit.itmedia.co.jp/ait/articles/2609/30/news056.html) | 21.0 | 20.0 | 42.0 |
| [クオカードのLINEキャンペーンシステムに不正アクセス 当選情報など流出の恐れ](https://www.itmedia.co.jp/news/article/2609/30/2000001878/) | 21.0 | 20.0 | 42.0 |
| [「郵便局アプリ」に不正アクセス 氏名や送り先住所など漏えい 19人分・69件](https://www.itmedia.co.jp/news/article/2609/30/2000001881/) | 21.0 | 20.0 | 42.0 |
| [Spectreバグが再来、今度はJITエンジンを悩ませる](https://www.theregister.com/security/2026/09/30/spectre-bug-is-back-this-time-to-haunt-jit-engines/5299937) | 20.0 | 28.0 | 50.0 |
| [OpenSSLとwolfSSLで修正された高深刻度の脆弱性](https://www.securityweek.com/high-severity-vulnerabilities-patched-in-openssl-wolfssl/) | 20.0 | 20.0 | 42.0 |
| [Security toolsがClaude Enterpriseのチャットとアップロードを機密データ向けにスキャン可能に](https://www.helpnetsecurity.com/2026/09/30/claude-compliance-api-integrations/) | 20.0 | 20.0 | 42.0 |
| [OWASP Noir：オープンソースの静的解析ツール](https://www.helpnetsecurity.com/2026/09/30/owasp-noir-open-source-static-analysis-tool/) | 20.0 | 20.0 | 42.0 |
| [EU Cyber Resilience ActにおけるコンテナとKubernetesの要件](https://www.helpnetsecurity.com/2026/09/30/rapidfort-cra-container-compliance/) | 20.0 | 20.0 | 42.0 |
| [多くの組織は新たなセキュリティ対策の展開に6カ月以上を要する](https://www.helpnetsecurity.com/2026/09/30/relentless-defense-cisco-cybersecurity-survey/) | 20.0 | 20.0 | 42.0 |
| [富士フイルムビジネスイノベーション製およびシャープ製複合機（MFP）におけるパストラバーサルの脆弱性](https://jvn.jp/vu/JVNVU90160989/) | 20.0 | 20.0 | 42.0 |
| [Cloudflareの耐量子ウェブサイト証明書は2027年初頭に提供予定](https://www.helpnetsecurity.com/2026/09/30/cloudflare-certificate-authority-2027/) | 20.0 | 20.0 | 42.0 |

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
