# Cyber Heat Radar 2026年度Q1 統計レポート

- 対象期間: 2026-04-01 00:00 JST 〜 2026-07-01 00:00 JST 未満
- 集計基準: Cyber Heat Radarで公開掲載されたレポート項目を対象に集計
- 除外: 低温記録のみの話題は集計対象外
- CVE集計: 公開掲載トピックに紐づく正規化済みCVEを対象に集計
- 集約トピック制御: 多数のCVEを束ねた集約トピックは、CVE件数の過大計上を避けるため個別CVE統計から除外
- KEV集計: CISA KEV公式カタログに2026-07-01より前に追加され、対象期間の登場CVEと一致したものを集計
- PoC/Exploit集計: 公開候補として確認済みのPoC/Exploit情報があるCVEを候補ありとして集計
- PoC/Exploit: URLは出さず、CVE単位の候補件数のみ
- 総括生成: 公開掲載ベースの集計結果と情報源材料を入力に生成AIで作成

---

## 1. サマリー

| 項⁠目 | 値 |
|---|---:|
| 生成レポート枠数 | 136 |
| 掲載ありレポート枠数 | 96 |
| ユニークトピック数 | 214 |
| 掲載延べ件数 | 283 |
| 平均最高温度 | 36.6 |
| 最高温度 | 73.0 |
| 登場CVE数 | 52 |
| KEV公式掲載CVE数 | 36 |
| PoC/Exploit候補ありCVE数 | 38 |

---

## 2. 温度分布

| 温⁠度⁠帯 | ユ⁠ニ⁠ー⁠ク⁠ト⁠ピ⁠ッ⁠ク⁠数 |
|---|---:|
| 90度以上 | 0 |
| 80〜89度 | 0 |
| 70〜79度 | 1 |
| 60〜69度 | 4 |
| 59度以下 | 209 |
| 未判定 | 0 |

---

## 3. カテゴリ別集計

| カ⁠テ⁠ゴ⁠リ | ユ⁠ニ⁠ー⁠ク⁠ト⁠ピ⁠ッ⁠ク⁠数 |
|---|---:|
| 脆弱性 | 86 |
| AI×Security | 69 |
| ランサムウェア | 26 |
| 脅威・攻撃 | 9 |
| サプライチェーン | 8 |
| インシデント | 1 |
| メディア/Podcast | 1 |
| その他 | 9 |
| defense_ops | 2 |
| threat_advisory | 2 |
| threat_report | 1 |

---

## 4. CVE統計

| 項⁠目 | 値 |
|---|---:|
| 登場CVE数 | 52 |
| KEV公式掲載CVE数 | 36 |
| PoC/Exploit候補ありCVE数 | 38 |

### 4.1 最頻出CVE Top10

| C⁠V⁠E | 関⁠連⁠ト⁠ピ⁠ッ⁠ク⁠数 | P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t⁠候⁠補⁠件⁠数 |
|---|---:|---:|
| CVE-2026-12569 | 4 | 0 |
| CVE-2025-67038 | 3 | 1 |
| CVE-2026-20182 | 3 | 3 |
| CVE-2026-20230 | 3 | 3 |
| CVE-2026-20245 | 3 | 3 |
| CVE-2026-34908 | 3 | 1 |
| CVE-2026-34909 | 3 | 0 |
| CVE-2026-34910 | 3 | 0 |
| CVE-2026-11645 | 2 | 3 |
| CVE-2026-20127 | 2 | 1 |

### 4.2 KEV公式掲載CVE

| C⁠V⁠E | K⁠E⁠V⁠追⁠加⁠日 | ベ⁠ン⁠ダ⁠ー⁠/⁠プ⁠ロ⁠ジ⁠ェ⁠ク⁠ト | 製⁠品 | 脆⁠弱⁠性⁠名 | P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t⁠候⁠補⁠件⁠数 |
|---|---|---|---|---|---:|
| CVE-2022-0492 | 2026-06-02 | Linux | Kernel | Linux Kernel Improper Authentication Vulnerability | 22 |
| CVE-2022-20775 | 2026-02-25 | Cisco | SD-WAN | Cisco SD-WAN Path Traversal Vulnerability | 0 |
| CVE-2024-21182 | 2026-06-01 | Oracle | WebLogic Server | Oracle WebLogic Server Unspecified Vulnerability | 5 |
| CVE-2024-24919 | 2024-05-30 | Check Point | Quantum Security Gateways | Check Point Quantum Security Gateways Information Disclosure Vulnerability | 73 |
| CVE-2025-48595 | 2026-06-02 | Android | Framework | Android Framework Integer Overflow Vulnerability | 2 |
| CVE-2025-67038 | 2026-06-23 | Lantronix | EDS5000 | Lantronix EDS5000 Code Injection Vulnerability | 1 |
| CVE-2025-8088 | 2025-08-12 | RARLAB | WinRAR | RARLAB WinRAR Path Traversal Vulnerability | 38 |
| CVE-2026-0257 | 2026-05-29 | Palo Alto Networks | PAN-OS | Palo Alto Networks PAN-OS Authentication Bypass Vulnerability | 10 |
| CVE-2026-10520 | 2026-06-11 | Ivanti | Sentry | Ivanti Sentry OS Command Injection Vulnerability | 6 |
| CVE-2026-11645 | 2026-06-09 | Google | Chromium V8 | Google Chromium V8 Out-of-Bounds Read and Write Vulnerability | 3 |
| CVE-2026-12569 | 2026-06-25 | PTC | Windchill and FlexPLM | PTC Windchill and FlexPLM Improper Input Validation Vulnerability | 0 |
| CVE-2026-20127 | 2026-02-25 | Cisco | Catalyst SD-WAN Controller and Manager | Cisco Catalyst SD-WAN Controller and Manager Authentication Bypass Vulnerability | 1 |
| CVE-2026-20182 | 2026-05-14 | Cisco | Catalyst SD-WAN | Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability | 3 |
| CVE-2026-20230 | 2026-06-25 | Cisco | Unified Communications Manager | Cisco Unified Communications Manager Server-Side Request Forgery (SSRF) Vulnerability | 3 |
| CVE-2026-20245 | 2026-06-09 | Cisco | Catalyst SD-WAN Manager | Cisco Catalyst SD-WAN Manager Improper Encoding or Escaping of Output Vulnerability | 3 |
| CVE-2026-20253 | 2026-06-18 | Splunk | Enterprise | Splunk Enterprise Missing Authentication for Critical Function Vulnerability | 5 |
| CVE-2026-20262 | 2026-06-15 | Cisco | Catalyst SD-WAN Manager | Cisco Catalyst SD-WAN Manager Directory or Path Traversal Vulnerability | 2 |
| CVE-2026-28318 | 2026-06-05 | SolarWinds | Serv-U | SolarWinds Serv-U Uncontrolled Resource Consumption Vulnerability | 3 |
| CVE-2026-33017 | 2026-03-25 | Langflow | Langflow | Langflow Code Injection Vulnerability | 1 |
| CVE-2026-33825 | 2026-04-22 | Microsoft | Defender | Microsoft Defender Insufficient Granularity of Access Control Vulnerability | 1 |
| CVE-2026-34908 | 2026-06-23 | Ubiquiti | UniFi OS | Ubiquiti UniFi OS Improper Access Control Vulnerability | 1 |
| CVE-2026-34909 | 2026-06-23 | Ubiquiti | UniFi OS | Ubiquiti UniFi OS Path Traversal Vulnerability | 0 |
| CVE-2026-34910 | 2026-06-23 | Ubiquiti | UniFi OS | Ubiquiti UniFi OS Improper Input Validation Vulnerability | 0 |
| CVE-2026-35273 | 2026-06-12 | Oracle |  PeopleSoft Enterprise PeopleTools | Oracle PeopleSoft Enterprise PeopleTools Missing Authentication for Critical Function Vulnerability | 3 |
| CVE-2026-35616 | 2026-04-06 | Fortinet | FortiClient EMS | Fortinet FortiClient EMS Improper Access Control Vulnerability | 2 |
| CVE-2026-39987 | 2026-04-23 | Marimo | Marimo | Marimo Remote Code Execution Vulnerability | 4 |
| CVE-2026-41091 | 2026-05-20 | Microsoft | Defender | Microsoft Defender Link Following Vulnerability | 2 |
| CVE-2026-42271 | 2026-06-08 | BerriAI | LiteLLM | BerriAI LiteLLM Command Injection Vulnerability | 2 |
| CVE-2026-42897 | 2026-05-15 | Microsoft | Microsoft | Microsoft Exchange Server Cross-Site Scripting Vulnerability | 1 |
| CVE-2026-45247 | 2026-06-03 | Mirasvit | Mirasvit Full Page Cache Warmer | Mirasvit Full Page Cache Warmer Deserialization of Untrusted Data Vulnerability | 2 |
| CVE-2026-45498 | 2026-05-20 | Microsoft | Defender | Microsoft Defender Denial of Service Vulnerability | 0 |
| CVE-2026-48558 | 2026-06-29 | SimpleHelp  | SimpleHelp | SimpleHelp Authentication Bypass Vulnerability | 0 |
| CVE-2026-48907 | 2026-06-16 | Widget Factory | Joomla Content Editor  | Widget Factory Joomla Content Editor Improper Access Control Vulnerability | 15 |
| CVE-2026-50751 | 2026-06-08 | Check Point | Security Gateway | Check Point Security Gateway Improper Authentication Vulnerability | 7 |
| CVE-2026-54420 | 2026-06-15 | LiteSpeed | cPanel Plugin | LiteSpeed cPanel Plugin UNIX Symbolic Link (Symlink) Following Vulnerability | 4 |
| CVE-2026-9082 | 2026-05-22 | Drupal | Core | Drupal Core SQL Injection Vulnerability | 13 |

---

## 5. 主要エンティティ

### 5.1 製品・ベンダー Top20

| 種⁠別 | 名⁠称 | 関⁠連⁠ト⁠ピ⁠ッ⁠ク⁠数 |
|---|---|---:|
| ベンダー | Microsoft | 42 |
| ベンダー | Cisco | 14 |
| ベンダー | cPanel | 5 |
| ベンダー | Ivanti | 3 |
| ベンダー | Fortinet | 2 |
| ベンダー | Palo Alto | 2 |
| ベンダー | Marimo | 1 |
| ベンダー | VMware | 1 |
| 製品 | Exchange | 10 |
| 製品 | cPanel | 5 |
| 製品 | Connect Secure | 1 |
| 製品 | FortiClient EMS | 1 |
| 製品 | Marimo | 1 |
| 製品 | Sentry | 1 |
| 製品 | Unified Communications Manager | 1 |
| 製品 | WHM | 1 |

### 5.2 技術・基盤 Top10

| 種⁠別 | 名⁠称 | 関⁠連⁠ト⁠ピ⁠ッ⁠ク⁠数 |
|---|---|---:|
| 技術・基盤 | Active Directory | 1 |

### 5.3 脅威アクター・ランサムウェア Top10

| 種⁠別 | 名⁠称 | 関⁠連⁠ト⁠ピ⁠ッ⁠ク⁠数 |
|---|---|---:|
| ランサムウェアグループ | Qilin | 7 |
| ランサムウェアグループ | Akira | 3 |
| ランサムウェアグループ | Clop | 2 |
| ランサムウェアグループ | BlackCat | 1 |
| ランサムウェアグループ | LockBit | 1 |

### 5.4 AIモデル・AIプロジェクト Top10

| 種⁠別 | 名⁠称 | 関⁠連⁠ト⁠ピ⁠ッ⁠ク⁠数 |
|---|---|---:|
| AIモデル/プロジェクト | Claude | 9 |
| AIモデル/プロジェクト | Anthropic | 6 |
| AIモデル/プロジェクト | ChatGPT | 5 |
| AIモデル/プロジェクト | OpenAI | 5 |
| AIモデル/プロジェクト | Claude Mythos | 2 |
| AIモデル/プロジェクト | Gemini | 2 |
| AIモデル/プロジェクト | Grok | 1 |

---

## 6. 重要トピック Top10

| 順⁠位 | 最⁠高⁠温⁠度 | 掲⁠載⁠回⁠数 | カ⁠テ⁠ゴ⁠リ | タ⁠イ⁠ト⁠ル | 関⁠連⁠C⁠V⁠E |
|---:|---:|---:|---|---|---|
| 1 | 73.0 | 4 | 脆弱性 | Why patch directives only go so far | CVE-2024-24919, CVE-2026-50751, CVE-2026-50752 |
| 2 | 67.0 | 2 | 脆弱性 | CVE-2026-10520: Ivanti Sentry | CVE-2026-10520 |
| 3 | 64.0 | 5 | 脆弱性 | Microsoft 2026年6月 Patch Tuesday 関連まとめ | 多数（261件、個別CVE統計から除外） |
| 4 | 63.0 | 15 | 脆弱性 | Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability | CVE-2026-20182 |
| 5 | 60.0 | 4 | 脆弱性 | ShinyHunters Targets Education Sector with Oracle PeopleSoft Exploit | CVE-2026-35273 |
| 6 | 53.0 | 2 | 脆弱性 | Microsoft working on a fix for RoguePlanet, a flaw that grants full PC control | CVE-2026-33825, CVE-2026-41091, CVE-2026-45498, CVE-2026-50656 |
| 7 | 49.0 | 1 | ランサムウェア | Check Point VPN Zero-Day Exploited in Qilin Ransomware Attacks | - |
| 8 | 48.0 | 14 | 脆弱性 | Threat Brief: Active Exploitation of PAN-OS CVE-2026-0257 | CVE-2026-0257 |
| 9 | 48.0 | 3 | 脆弱性 | Cisco discloses second exploited SD-WAN vulnerability in two weeks (CVE-2026-20262) | CVE-2026-20262 |
| 10 | 48.0 | 2 | 脆弱性 | Google Releases Patch for Chrome Vulnerability Exploited in the Wild | CVE-2026-11645 |

---

## 7. 2026年度Q1総括

### 7.1 全体傾向

公開件数は96、生成件数は136で、全214トピック・283件の掲載が確認できる。温度分布は59度以下が209トピックと大半を占め、70度以上は1トピックに限られる。平均最大温度は36.6、最大温度は73.0で、上位に位置する話題は限定的だった。カテゴリ別では「脆弱性」が86トピックで最多、次いで「AI×Security」が69、「ランサムウェア」が26となっており、全体として脆弱性関連とAI関連が大きな比重を占める構成だった。

### 7.2 CVEの傾向

登場CVEは52件、KEV公式掲載CVEは36件、PoC/Exploit候補ありCVEは38件で、KEVとPoC/Exploit候補の重なりは30件だった。上位の登場CVEではCVE-2026-12569が関連トピック数4で最多となり、CVE-2025-67038、CVE-2026-20182、CVE-2026-20230、CVE-2026-20245、CVE-2026-34908はいずれも関連トピック数3で続いた。PoC/Exploit候補ありCVEの件数がKEV公式掲載CVEを上回っており、観測範囲では実際の悪用が確認されたものと候補段階のものが並行して取り上げられていた。

### 7.3 悪用・PoC・KEVの観測

上位トピックには、実際の悪用やPoC公開に関する記述が複数含まれた。たとえばCVE-2026-50751は「Why patch directives only go so far」で最大温度73.0、登場回数4で最上位となり、CVE-2026-10520はKEV公式掲載CVEとして関連トピック数2、CVE-2026-0257は登場回数14、CVE-2026-20262は登場回数3、CVE-2026-11645は登場回数2だった。これらは、KEV公式掲載やPoC/Exploit候補、さらには「悪用された」「実際に悪用が観測された」といった観測が同一期間内に集中していることを示している。

### 7.4 脅威アクター・ランサムウェアの動向

ランサムウェアグループの関連トピック数はQilinが7で最多、次いでAkiraが3、Clopが2、BlackCatが1、LockBitが1だった。上位トピックでもQilinに関する話題が登場し、ランサムウェア関連の中では相対的にQilinの掲載が多い。一方で、全体カテゴリでは「ランサムウェア」は26トピックで、「脆弱性」や「AI×Security」より少なく、観測範囲ではランサムウェア単独よりも脆弱性起点の話題がより広く扱われていた。

### 7.5 AI×Securityの傾向

AI×Security関連ではClaudeが9件で最多、Anthropicが6件、ChatGPTとOpenAIが各5件、Claude MythosとGeminiが各2件、Grokが1件だった。カテゴリとしての「AI×Security」は69トピックで、ランサムウェアを上回り、全体でも大きな比重を占める。上位の対象が複数のAIモデル/プロジェクトに分散していることから、観測範囲では特定単独ではなく、複数のAI関連対象が並行して話題化していた。

### 7.6 観測上の留意事項

ここでの数値は、定められた期間内にCyber Heat Radarで掲載された話題、掲載回数、関連CVE、カテゴリ分類に基づく集計です。温度分布は話題単位の件数であり、掲載項目数や生成レポート数とは一致しません。CVE、KEV公式掲載CVE、PoC/Exploit候補ありCVEの各件数は、観測期間中に掲載対象となった話題との関連に基づいています。PoC/Exploit候補件数は、公開候補として確認された情報の件数であり、URLそのものは掲載していません。
