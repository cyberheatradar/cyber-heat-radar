# Cyber Heat Radar 2026年度Q2 統計レポート

- 対象期間: 2026-07-01 00:00 JST 〜 2026-10-01 00:00 JST 未満
- 集計基準: Cyber Heat Radarで公開掲載されたレポート項目を対象に集計
- 除外: 低温記録のみの話題は集計対象外
- CVE集計: 公開掲載トピックに紐づく正規化済みCVEを対象に集計
- 集約トピック制御: 多数のCVEを束ねた集約トピックは、CVE件数の過大計上を避けるため個別CVE統計から除外
- KEV集計: CISA KEV公式カタログに2026-10-01より前に追加され、対象期間の登場CVEと一致したものを集計
- PoC/Exploit集計: 公開候補として確認済みのPoC/Exploit情報があるCVEを候補ありとして集計
- PoC/Exploit: URLは出さず、CVE単位の候補件数のみ
- 総括生成: 公開掲載ベースの集計結果と情報源材料を入力に生成AIで作成

---

## 1. サマリー

| 項⁠目 | 値 |
|---|---:|
| 生成レポート枠数 | 278 |
| 掲載ありレポート枠数 | 190 |
| ユニークトピック数 | 527 |
| 掲載延べ件数 | 626 |
| 平均最高温度 | 37.6 |
| 最高温度 | 72.0 |
| 登場CVE数 | 203 |
| KEV公式掲載CVE数 | 116 |
| PoC/Exploit候補ありCVE数 | 113 |

---

## 2. 温度分布

| 温⁠度⁠帯 | ユ⁠ニ⁠ー⁠ク⁠ト⁠ピ⁠ッ⁠ク⁠数 |
|---|---:|
| 90度以上 | 0 |
| 80〜89度 | 0 |
| 70〜79度 | 1 |
| 60〜69度 | 7 |
| 59度以下 | 519 |
| 未判定 | 0 |

---

## 3. カテゴリ別集計

| カ⁠テ⁠ゴ⁠リ | ユ⁠ニ⁠ー⁠ク⁠ト⁠ピ⁠ッ⁠ク⁠数 |
|---|---:|
| 脆弱性 | 235 |
| AI×Security | 178 |
| ランサムウェア | 52 |
| 脅威・攻撃 | 24 |
| サプライチェーン | 12 |
| インシデント | 1 |
| メディア/Podcast | 1 |
| その他 | 17 |
| threat_advisory | 4 |
| threat_report | 3 |

---

## 4. CVE統計

| 項⁠目 | 値 |
|---|---:|
| 登場CVE数 | 203 |
| KEV公式掲載CVE数 | 116 |
| PoC/Exploit候補ありCVE数 | 113 |

### 4.1 最頻出CVE Top10

| C⁠V⁠E | 関⁠連⁠ト⁠ピ⁠ッ⁠ク⁠数 | P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t⁠候⁠補⁠件⁠数 |
|---|---:|---:|
| CVE-2026-45659 | 6 | 4 |
| CVE-2026-50656 | 5 | 4 |
| CVE-2026-56164 | 5 | 2 |
| CVE-2026-50522 | 4 | 4 |
| CVE-2026-55255 | 4 | 1 |
| CVE-2026-58644 | 4 | 0 |
| CVE-2026-73570 | 4 | 8 |
| CVE-2026-15409 | 3 | 5 |
| CVE-2026-15410 | 3 | 1 |
| CVE-2026-16232 | 3 | 2 |

### 4.2 KEV公式掲載CVE

| C⁠V⁠E | K⁠E⁠V⁠追⁠加⁠日 | ベ⁠ン⁠ダ⁠ー⁠/⁠プ⁠ロ⁠ジ⁠ェ⁠ク⁠ト | 製⁠品 | 脆⁠弱⁠性⁠名 | P⁠o⁠C⁠/⁠E⁠x⁠p⁠l⁠o⁠i⁠t⁠候⁠補⁠件⁠数 |
|---|---|---|---|---|---:|
| CVE-2008-4128 | 2026-07-13 | Cisco | IOS | Cisco IOS Cross-Site Request Forgery Vulnerability | 0 |
| CVE-2018-0171 | 2021-11-03 | Cisco | IOS and IOS XE | Cisco IOS and IOS XE Software Smart Install Remote Code Execution Vulnerability | 0 |
| CVE-2019-1068 | 2026-08-26 | Microsoft | SQL Server | Microsoft SQL Server Remote Code Execution Vulnerability | 2 |
| CVE-2021-23758 | 2026-08-26 | Ajax.NET Professional | Ajax.NET Professional | Ajax.NET Professional Deserialization of Untrusted Data Vulnerability | 2 |
| CVE-2021-27137 | 2026-07-21 | DD-WRT | DD-WRT | DD-WRT Stack-Based Buffer Overflow Vulnerability | 0 |
| CVE-2023-20198 | 2023-10-16 | Cisco | IOS XE Web UI | Cisco IOS XE Web UI Privilege Escalation Vulnerability | 41 |
| CVE-2023-27350 | 2023-04-21 | PaperCut | MF/NG | PaperCut MF/NG Improper Access Control Vulnerability | 21 |
| CVE-2023-4346 | 2026-07-15 | KNX Association | KNX Protocol Connection Authorization Option 1 | KNX Association KNX Protocol Connection Authorization Option 1 Overly Restrictive Account Lockout Mechanism Vulnerability | 0 |
| CVE-2024-21182 | 2026-06-01 | Oracle | WebLogic Server | Oracle WebLogic Server Unspecified Vulnerability | 5 |
| CVE-2024-42009 | 2025-06-09 | Roundcube | Webmail | RoundCube Webmail Cross-Site Scripting Vulnerability | 6 |
| CVE-2024-45519 | 2024-10-03 | Synacor | Zimbra Collaboration Suite (ZCS) | Synacor Zimbra Collaboration Suite (ZCS) Command Execution Vulnerability | 10 |
| CVE-2024-55591 | 2025-01-14 | Fortinet | FortiOS and FortiProxy | Fortinet FortiOS and FortiProxy Authentication Bypass Vulnerability | 12 |
| CVE-2025-14733 | 2025-12-19 | WatchGuard | Firebox | WatchGuard Firebox Out of Bounds Write Vulnerability | 1 |
| CVE-2025-20333 | 2025-09-25 | Cisco | Secure Firewall Adaptive Security Appliance and Secure Firewall Threat Defense | Cisco Secure Firewall Adaptive Security Appliance (ASA) and Secure Firewall Threat Defense (FTD) Buffer Overflow Vulnerability | 4 |
| CVE-2025-20362 | 2025-09-25 | Cisco | Secure Firewall Adaptive Security Appliance and Secure Firewall Threat Defense | Cisco Secure Firewall Adaptive Security (ASA) Appliance and Secure Firewall Threat Defense (FTD) Missing Authorization Vulnerability | 2 |
| CVE-2025-20393 | 2025-12-17 | Cisco | Multiple Products | Cisco Multiple Products Improper Input Validation Vulnerability | 4 |
| CVE-2025-24054 | 2025-04-17 | Microsoft | Windows | Microsoft Windows NTLM Hash Disclosure Spoofing Vulnerability | 14 |
| CVE-2025-3248 | 2025-05-05 | Langflow | Langflow | Langflow Missing Authentication Vulnerability | 34 |
| CVE-2025-33053 | 2025-06-10 | Microsoft | Windows |  Microsoft Windows External Control of File Name or Path Vulnerability | 6 |
| CVE-2025-33073 | 2025-10-20 | Microsoft | Windows | Microsoft Windows SMB Client Improper Access Control Vulnerability | 44 |
| CVE-2025-39964 | 2026-09-18 | Linux | Kernel | Linux Kernel Race Condition Vulnerability | 2 |
| CVE-2025-49113 | 2026-02-20 | Roundcube | Webmail | RoundCube Webmail Deserialization of Untrusted Data Vulnerability | 27 |
| CVE-2025-60710 | 2026-04-13 | Microsoft | Windows | Microsoft Windows Link Following Vulnerability | 2 |
| CVE-2025-61882 | 2025-10-06 | Oracle | E-Business Suite | Oracle E-Business Suite Unspecified Vulnerability | 16 |
| CVE-2025-61884 | 2025-10-20 | Oracle | E-Business Suite | Oracle E-Business Suite Server-Side Request Forgery (SSRF) Vulnerability | 3 |
| CVE-2025-62593 | 2026-08-17 | Ray-Project | Ray | Ray-Project Ray Code Injection Vulnerability | 1 |
| CVE-2025-66376 | 2026-03-18 | Synacor | Zimbra Collaboration Suite (ZCS) | Synacor Zimbra Collaboration Suite (ZCS) Cross-Site Scripting Vulnerability | 0 |
| CVE-2026-0257 | 2026-05-29 | Palo Alto Networks | PAN-OS | Palo Alto Networks PAN-OS Authentication Bypass Vulnerability | 10 |
| CVE-2026-0770 | 2026-07-21 | Langflow | Langflow | Langflow Inclusion of Functionality from Untrusted Control Sphere Vulnerability | 7 |
| CVE-2026-15409 | 2026-07-14 | SonicWall | SMA1000 Appliances | SonicWall SMA1000 Appliances Server-Side Request Forgery Vulnerability | 5 |
| CVE-2026-15410 | 2026-07-14 | SonicWall | SMA1000 Appliances | SonicWall SMA1000 Appliances Code Injection Vulnerability | 1 |
| CVE-2026-16232 | 2026-07-22 | Check Point | SmartConsole | Check Point SmartConsole Improper Authentication Vulnerability | 2 |
| CVE-2026-16812 | 2026-07-27 | Arista | VeloCloud Orchestrator | Arista VeloCloud Orchestrator On-Prem OS Command Injection Vulnerability | 0 |
| CVE-2026-18556 | 2026-08-04 | N-able | N-central | N-able N-central Authentication Bypass Using an Alternate Path or Channel Vulnerability | 0 |
| CVE-2026-18577 | 2026-08-03 | N-able | N-central | N-able N-central Authentication Bypass Using an Alternate Path or Channel Vulnerability | 1 |
| CVE-2026-19490 | 2026-09-09 | Citrix | NetScaler | Citrix NetScaler Authentication Bypass Using an Alternate Path or Channel Vulnerability | 2 |
| CVE-2026-20079 | 2026-09-09 | Cisco | Secure Firewall Management Center (FMC) and Security Cloud Control (SCC) Firewall Management | Cisco Firewall Management Center Authentication Bypass Using an Alternate Path or Channel Vulnerability | 3 |
| CVE-2026-20127 | 2026-02-25 | Cisco | Catalyst SD-WAN Controller and Manager | Cisco Catalyst SD-WAN Controller and Manager Authentication Bypass Vulnerability | 9 |
| CVE-2026-20182 | 2026-05-14 | Cisco | Catalyst SD-WAN | Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability | 3 |
| CVE-2026-20230 | 2026-06-25 | Cisco | Unified Communications Manager | Cisco Unified Communications Manager Server-Side Request Forgery (SSRF) Vulnerability | 3 |
| CVE-2026-20245 | 2026-06-09 | Cisco | Catalyst SD-WAN Manager | Cisco Catalyst SD-WAN Manager Improper Encoding or Escaping of Output Vulnerability | 3 |
| CVE-2026-20316 | 2026-07-29 | Cisco | Secure Firewall Management Center (FMC) | Cisco Secure Firewall Management Center Use of Hard-coded Password Vulnerability | 0 |
| CVE-2026-20349 | 2026-08-11 | Cisco | Secure Firewall Adaptive Security Appliance (ASA) and Secure Firewall Threat Defense (FTD)  | Cisco Secure Firewall Adaptive Security Appliance (ASA) and Secure Firewall Threat Defense (FTD) Heap Inspection Vulnerability | 0 |
| CVE-2026-21513 | 2026-02-10 | Microsoft | Windows | Microsoft MSHTML Framework Protection Mechanism Failure Vulnerability | 0 |
| CVE-2026-21643 | 2026-04-13 | Fortinet | FortiClient EMS | Fortinet FortiClient EMS SQL Injection Vulnerability | 2 |
| CVE-2026-21962 | 2026-08-24 | Oracle | HTTP Server and Oracle Weblogic Server Proxy Plug-in | Oracle HTTP Server and Oracle Weblogic Server Proxy Plug-in Improper Access Control Vulnerability | 10 |
| CVE-2026-25089 | 2026-07-16 | Fortinet | FortiSandbox | Fortinet FortiSandbox OS Command Injection Vulnerability | 2 |
| CVE-2026-32201 | 2026-04-14 | Microsoft | SharePoint Server | Microsoft SharePoint Server Improper Input Validation Vulnerability | 1 |
| CVE-2026-33017 | 2026-03-25 | Langflow | Langflow | Langflow Code Injection Vulnerability | 27 |
| CVE-2026-33824 | 2026-08-18 | Microsoft | Internet Key Exchange (IKE) Service Extensions | Microsoft Internet Key Exchange (IKE) Service Extensions Double Free Vulnerability | 1 |
| CVE-2026-33825 | 2026-04-22 | Microsoft | Defender | Microsoft Defender Insufficient Granularity of Access Control Vulnerability | 3 |
| CVE-2026-34486 | 2026-08-04 | Apache | Tomcat | Apache Tomcat Missing Encryption of Sensitive Data Vulnerability | 7 |
| CVE-2026-34621 | 2026-04-13 | Adobe | Acrobat and Reader | Adobe Acrobat and Reader Prototype Pollution Vulnerability | 4 |
| CVE-2026-34908 | 2026-06-23 | Ubiquiti | UniFi OS | Ubiquiti UniFi OS Improper Access Control Vulnerability | 1 |
| CVE-2026-34909 | 2026-06-23 | Ubiquiti | UniFi OS | Ubiquiti UniFi OS Path Traversal Vulnerability | 0 |
| CVE-2026-34910 | 2026-06-23 | Ubiquiti | UniFi OS | Ubiquiti UniFi OS Improper Input Validation Vulnerability | 2 |
| CVE-2026-35273 | 2026-06-12 | Oracle |  PeopleSoft Enterprise PeopleTools | Oracle PeopleSoft Enterprise PeopleTools Missing Authentication for Critical Function Vulnerability | 3 |
| CVE-2026-39808 | 2026-07-16 | Fortinet | FortiSandbox | Fortinet FortiSandbox OS Command Injection Vulnerability | 5 |
| CVE-2026-41091 | 2026-05-20 | Microsoft | Defender | Microsoft Defender Link Following Vulnerability | 2 |
| CVE-2026-41940 | 2026-04-30 | WebPros | cPanel & WHM and WP2 (WordPress Squared) | WebPros cPanel & WHM and WP2 (WordPress Squared) Missing Authentication for Critical Function Vulnerability | 66 |
| CVE-2026-42208 | 2026-05-08 | BerriAI | LiteLLM | BerriAI LiteLLM SQL Injection Vulnerability | 5 |
| CVE-2026-42897 | 2026-05-15 | Microsoft | Microsoft | Microsoft Exchange Server Cross-Site Scripting Vulnerability | 1 |
| CVE-2026-45498 | 2026-05-20 | Microsoft | Defender | Microsoft Defender Denial of Service Vulnerability | 0 |
| CVE-2026-45659 | 2026-07-01 | Microsoft | SharePoint Server | Microsoft SharePoint Server Deserialization of Untrusted Data Vulnerability | 4 |
| CVE-2026-46817 | 2026-07-15 | Oracle | E-Business Suite | Oracle E-Business Suite Improper Privilege Management Vulnerability | 2 |
| CVE-2026-48282 | 2026-07-07 | Adobe | ColdFusion | Adobe ColdFusion Path Traversal Vulnerability | 4 |
| CVE-2026-48558 | 2026-06-29 | SimpleHelp  | SimpleHelp | SimpleHelp Authentication Bypass Vulnerability | 1 |
| CVE-2026-48908 | 2026-07-07 | JoomShaper | SP Page Builder | JoomShaper SP Page Builder Unrestricted Upload of File with Dangerous Type Vulnerability | 12 |
| CVE-2026-48939 | 2026-07-10 | iCagenda | iCagenda | iCagenda Unrestricted Upload of File with Dangerous Type Vulnerability | 3 |
| CVE-2026-50522 | 2026-07-22 | Microsoft | SharePoint | Microsoft SharePoint Deserialization of Untrusted Data Vulnerability  | 4 |
| CVE-2026-53362 | 2026-08-27 | Linux | Kernel | Linux Kernel Unspecified Vulnerability | 0 |
| CVE-2026-55040 | 2026-08-18 | Microsoft | SharePoint | Microsoft SharePoint Weak Authentication Vulnerability | 4 |
| CVE-2026-55255 | 2026-07-07 | Langflow | Langflow | Langflow Authorization Bypass Through User-Controlled Key Vulnerability | 1 |
| CVE-2026-56155 | 2026-07-14 | Microsoft | Active Directory Federation Services | Microsoft Active Directory Federation Services Insufficient Granularity of Access Control Vulnerability  | 0 |
| CVE-2026-56164 | 2026-07-14 | Microsoft | SharePoint Server | Microsoft SharePoint Server Missing Authentication for Critical Function Vulnerability | 2 |
| CVE-2026-56290 | 2026-07-07 | Joomlack | Page Builder | Joomlack Page Builder Improper Access Control Vulnerability | 4 |
| CVE-2026-56291 | 2026-07-10 | Balbooa | Forms | Balbooa Forms Unrestricted Upload of File with Dangerous Type Vulnerability | 4 |
| CVE-2026-58644 | 2026-07-16 | Microsoft | SharePoint | Microsoft SharePoint Deserialization of Untrusted Data Vulnerability | 0 |
| CVE-2026-58704 | 2026-09-16 | Google | Pixel | Google Pixel Improper Authorization Vulnerability | 0 |
| CVE-2026-59310 | 2026-08-18 | Broadcom | VMware vCenter | Broadcom VMware vCenter Path Traversal Vulnerability | 4 |
| CVE-2026-60004 | 2026-08-25 | Gitea | Gitea | Gitea Code Injection Vulnerability | 11 |
| CVE-2026-60137 | 2026-07-21 | WordPress | Core | WordPress Core SQL Injection Vulnerability | 7 |
| CVE-2026-63030 | 2026-07-21 | WordPress | Core | WordPress Core Interpretation Conflict Vulnerability | 39 |
| CVE-2026-63077 | 2026-08-05 | JetBrains | TeamCity | JetBrains TeamCity Deserialization of Untrusted Data Vulnerability | 6 |
| CVE-2026-64849 | 2026-08-19 | MLflow | MLflow | MLflow Server-Side Request Forgery Vulnerability | 4 |
| CVE-2026-65400 | 2026-08-18 | Apple | macOS | Apple macOS Improper Authentication Vulnerability | 3 |
| CVE-2026-68820 | 2026-08-11 | Microsoft | Windows Ancillary Function Driver for WinSock  | Microsoft Windows Ancillary Function Driver for WinSock Use-After-Free Vulnerability | 3 |
| CVE-2026-71362 | 2026-09-24 | Adobe | Commerce and Magento  | Adobe Commerce and Magento Incorrect Authorization Vulnerability  | 1 |
| CVE-2026-7273 | 2026-09-21 | Zyxel | GS1900 Series Switches | Zyxel GS1900 Series Switches Stack-Based Buffer Overflow Vulnerability | 0 |
| CVE-2026-73570 | 2026-08-21 | Synacor | Zimbra Collaboration Suite (ZCS) | Zimbra Collaboration Suite (ZCS) OS Command Injection Vulnerability | 8 |
| CVE-2026-75650 | 2026-09-08 | Adobe | Commerce and Magento | Adobe Commerce and Magento Improper Neutralization of Special Elements Used in a Template Engine Vulnerability | 2 |
| CVE-2026-76460 | 2026-09-16 | Cisco | Identity Services Engine | Cisco Identity Services Engine Incorrect Use of Privileged APIs Vulnerability | 1 |
| CVE-2026-76461 | 2026-09-14 | Cisco | Secure Email Gateway | Cisco Secure Email Gateway SQL Injection Vulnerability | 4 |
| CVE-2026-8037 | 2026-08-07 | Progress | LoadMaster | Progress LoadMaster Command Injection Vulnerability | 2 |
| CVE-2026-81578 | 2026-08-31 | PaperCut | NG/MF | PaperCut NG/MF Missing Authentication for Critical Function Vulnerability | 1 |
| CVE-2026-81963 | 2026-09-08 | Microsoft | Windows | Microsoft Windows Link Following Vulnerability | 0 |
| CVE-2026-82078 | 2026-08-31 | PaperCut | NG/MF | PaperCut NG/MF Unsafe Reflection Vulnerability | 0 |
| CVE-2026-82329 | 2026-09-02 | JFrog | Artifactory | JFrog Artifactory Improper Authentication Vulnerability | 8 |
| CVE-2026-83548 | 2026-09-02 | SonicWall | SMA1000 Appliances | SonicWall SMA1000 Appliances Server-Side Request Forgery Vulnerability | 3 |
| CVE-2026-83549 | 2026-09-02 | SonicWall | SMA1000 Appliances | SonicWall SMA1000 Appliances OS Command Injection Vulnerability | 0 |
| CVE-2026-8452 | 2026-08-26 | Citrix | NetScaler ADC and NetScaler Gateway | Citrix NetScaler ADC and NetScaler Gateway Improper Restriction of Operations within the Bounds of a Memory Buffer Vulnerability | 4 |
| CVE-2026-85046 | 2026-09-04 | Google | Chromium V8 | Google Chromium V8 Type Confusion Vulnerability | 6 |
| CVE-2026-85706 | 2026-09-11 | GitLab | Community Edition and Enterprise Edition | GitLab Community Edition and Enterprise Edition Path Traversal Vulnerability | 15 |
| CVE-2026-85880 | 2026-09-08 | Microsoft | Windows | Microsoft Windows Heap-Based Buffer Overflow Vulnerability | 0 |
| CVE-2026-86218 | 2026-09-08 | N-able | N-central | N-able N-central Static Code Injection Vulnerability | 3 |
| CVE-2026-86950 | 2026-09-29 | Apple | Multiple Products | Apple Multiple Products Out-of-Bounds Write Vulnerability | 1 |
| CVE-2026-87491 | 2026-09-09 | Google | Chromium V8 | Google Chromium V8 Out of Bounds Write Vulnerability | 1 |
| CVE-2026-87886 | 2026-09-16 | Acronis | Backup | Acronis Backup Incorrect Default Permissions Vulnerability | 0 |
| CVE-2026-87902 | 2026-09-25 | WordPress | Core | WordPress Core Remote File Inclusion Vulnerability | 24 |
| CVE-2026-88771 | 2026-09-27 | Citrix | NetScaler | Citrix NetScaler Improper Input Validation Vulnerability | 5 |
| CVE-2026-88772 | 2026-09-27 | Citrix | NetScaler | Citrix NetScaler Improper Restriction of Operations within the Bounds of a Memory Buffer Vulnerability | 3 |
| CVE-2026-9198 | 2026-08-04 | IBM | Langflow | IBM Langflow Code Injection Vulnerability | 9 |
| CVE-2026-93616 | 2026-09-22 | Check Point | Multiple Products | Check Point Multiple Products Path Traversal Vulnerability | 2 |
| CVE-2026-93952 | 2026-09-22 | Arista | VeloCloud Orchestrator | Arista VeloCloud Orchestrator Improper Input Validation Vulnerability | 0 |
| CVE-2026-94127 | 2026-09-22 | F5 | BIG-IP APM | F5 BIG-IP APM Heap-based Buffer Overflow Vulnerability | 2 |
| CVE-2026-9586 | 2026-09-02 | Sangoma | Switchvox | Sangoma Switchvox SQL Injection Vulnerability | 1 |

---

## 5. 主要エンティティ

### 5.1 製品・ベンダー Top20

| 種⁠別 | 名⁠称 | 関⁠連⁠ト⁠ピ⁠ッ⁠ク⁠数 |
|---|---|---:|
| ベンダー | Microsoft | 87 |
| ベンダー | Google | 43 |
| ベンダー | Cisco | 37 |
| ベンダー | Anthropic | 30 |
| ベンダー | OpenAI | 21 |
| ベンダー | Rapid7 | 20 |
| ベンダー | Adobe | 19 |
| ベンダー | Citrix | 18 |
| ベンダー | SonicWall | 15 |
| ベンダー | DeepSeek | 13 |
| ベンダー | Apple | 12 |
| ベンダー | Cloudflare | 12 |
| ベンダー | Check Point | 11 |
| ベンダー | Oracle | 10 |
| ベンダー | Zimbra | 10 |
| ベンダー | CrowdStrike | 9 |
| ベンダー | Fortinet | 9 |
| ベンダー | Mandiant | 9 |
| ベンダー | Qwen | 9 |
| ベンダー | Amazon Web Services | 8 |

### 5.2 技術・基盤 Top10

| 種⁠別 | 名⁠称 | 関⁠連⁠ト⁠ピ⁠ッ⁠ク⁠数 |
|---|---|---:|
| 技術・基盤 | Active Directory | 19 |

### 5.3 脅威アクター・ランサムウェア Top10

| 種⁠別 | 名⁠称 | 関⁠連⁠ト⁠ピ⁠ッ⁠ク⁠数 |
|---|---|---:|
| ランサムウェアグループ | Qilin | 7 |
| ランサムウェアグループ | Clop | 6 |
| ランサムウェア/マルウェア | Vidar | 6 |
| 脅威アクター | Lazarus Group | 4 |
| 脅威アクター | APT29 | 3 |
| ランサムウェア/マルウェア | AsyncRAT | 3 |
| 脅威アクター | BRONZE BUTLER | 3 |
| ランサムウェアグループ | INC Ransom | 3 |
| 攻撃/検証ツール | Impacket | 3 |
| ランサムウェア/マルウェア | Remcos | 3 |

### 5.4 AIモデル・AIプロジェクト Top10

| 種⁠別 | 名⁠称 | 関⁠連⁠ト⁠ピ⁠ッ⁠ク⁠数 |
|---|---|---:|
| AIモデル/プロジェクト | Anthropic | 22 |
| AIモデル/プロジェクト | Claude | 22 |
| AIモデル/プロジェクト | Gemini | 11 |
| AIモデル/プロジェクト | OpenAI | 9 |
| AIモデル/プロジェクト | ChatGPT | 8 |
| AIモデル/プロジェクト | DeepSeek | 8 |
| AIモデル/プロジェクト | Copilot | 4 |
| AIモデル/プロジェクト | Claude Mythos | 3 |
| AIモデル/プロジェクト | Google Gemini | 3 |
| AIモデル/プロジェクト | GPT-5 | 3 |

---

## 6. 重要トピック Top10

| 順⁠位 | 最⁠高⁠温⁠度 | 掲⁠載⁠回⁠数 | カ⁠テ⁠ゴ⁠リ | タ⁠イ⁠ト⁠ル | 関⁠連⁠C⁠V⁠E |
|---:|---:|---:|---|---|---|
| 1 | 72.0 | 4 | 脆弱性 | CVE-2026-41940: cPanel & WHM authentication bypass exploited in ransomware attacks | CVE-2026-40473, CVE-2026-41940, CVE-2026-42208, CVE-2026-76460 |
| 2 | 69.0 | 4 | 脆弱性 | Microsoft 2026年9月 Patch Tuesday 関連まとめ | - |
| 3 | 66.0 | 5 | 脆弱性 | Microsoft 2026年7月 Patch Tuesday 関連まとめ | 多数（634件、個別CVE統計から除外） |
| 4 | 63.0 | 1 | 脆弱性 | Google Pixel owners urged to patch actively exploited modem flaw | CVE-2026-58704 |
| 5 | 62.0 | 6 | 脆弱性 | SonicWall customers under threat as attackers exploit 2 zero-days | CVE-2026-15409, CVE-2026-15410 |
| 6 | 62.0 | 3 | 脆弱性 | Cisco Secure Email Gateway SQL Injection Vulnerability | CVE-2026-76461 |
| 7 | 62.0 | 3 | 脆弱性 | 2026-009: Critical Vulnerabilities in Microsoft SharePoint | CVE-2026-32201, CVE-2026-45659, CVE-2026-50522, CVE-2026-56164, CVE-2026-58644 |
| 8 | 60.0 | 3 | 脆弱性 | Feds get 3 days to patch N-able God mode flaw under active exploit | CVE-2026-18577 |
| 9 | 59.0 | 2 | 脆弱性 | Attackers exploit zero-days in consistently besieged SonicWall product | CVE-2026-82329, CVE-2026-83548, CVE-2026-83549 |
| 10 | 58.0 | 3 | 脆弱性 | CVE-2025-20333: Cisco ASA/FTD persistence mechanism update | CVE-2023-20198, CVE-2025-20333, CVE-2025-20362, CVE-2025-20393 |

---

## 7. 2026年度Q2総括

### 7.1 全体傾向

掲載は278件で、そのうち190件が公開済みでした。総トピック数は527件、掲載項目数は626件で、話題は広く分散しつつも、平均最大熱度は37.6度、最高は72.0度にとどまりました。熱度分布では「59度以下」が519件と大半を占め、「70〜79度」は1件、「80度以上」は0件でした。カテゴリ別では「脆弱性」が235件で最多、次いで「AI×Security」が178件、「ランサムウェア」が52件でした。観測範囲では、脆弱性関連の話題量が最も大きく、AI×Securityも脆弱性に次ぐ規模で継続的に目立っています。

### 7.2 CVEの傾向

CVE関連では、登場CVEが203件、KEV公式掲載CVEが116件、PoC/Exploit候補ありCVEが113件でした。KEV公式掲載CVEとPoC/Exploit候補ありCVEの重なりは93件で、両方の観点に関わるものが少なくありません。上位の登場CVEでは、CVE-2026-45659が関連トピック数6で最多、CVE-2026-50656、CVE-2026-56164、CVE-2026-50522、CVE-2026-73570、CVE-2026-15409などが複数回登場していました。PoC/Exploit候補ありCVE数ではCVE-2026-73570が8で最も多く、CVE-2026-15409が5、CVE-2026-45659、CVE-2026-50656、CVE-2026-50522が各4でした。登場回数の多いCVEが、PoC/Exploit候補としても繰り返し現れる傾向が見られます。

### 7.3 悪用・PoC・KEVの観測

悪用やPoCに関する観測では、CVE-2026-41940、CVE-2026-58704、CVE-2026-15409、CVE-2026-15410、CVE-2026-50522、CVE-2026-18577、CVE-2026-83548、CVE-2026-83549が関連トピックに含まれていました。CVE-2026-41940は関連トピック数6で最上位で、PoC/Exploit候補ありCVE数も4でした。CVE-2026-50522は、関連トピックにおいてPoC登場後の活発な言及があり、CVE-2026-15409は関連トピック数3でPoC/Exploit候補ありCVE数が5でした。CVE-2026-58704は関連トピック数1ながら、KEV公式掲載CVEとして扱われていました。観測上は、PoC/Exploit候補とKEV公式掲載が重なる話題が複数あり、公開済みの注目度が高いCVEが限られた数の上位トピックに集まっています。

### 7.4 脅威アクター・ランサムウェアの動向

脅威アクター・ランサムウェア関連では、Qilinが関連トピック数7で最多、ClopとVidarが各6、Lazarus Groupが4でした。次いでAPT29、AsyncRAT、BRONZE BUTLER、INC Ransom、Impacket、Remcosが各3でした。上位にはランサムウェアグループと脅威アクターに加え、攻撃/検証ツールやマルウェア系の名称も含まれており、関連話題が一種類に偏らず並行していることがうかがえます。ランサムウェア側ではQilinとClopが相対的に多く、脅威アクター側ではLazarus GroupやAPT29が上位に入りました。

### 7.5 AI×Securityの傾向

AI×Securityでは、AnthropicとClaudeが各22で最上位、Geminiが11、OpenAIが9、ChatGPTとDeepSeekが各8でした。続いてCopilotが4、Claude Mythos、Google Gemini、GPT-5が各3でした。上位10件のうち同一系列と見られる名称が複数含まれており、話題は少数の名称に集まりやすい構造です。関連トピック数の差も大きく、最上位の22件と下位の3〜4件の間で掲載密度に開きがあります。全体のカテゴリ件数でもAI×Securityは178件と大きく、脆弱性に次ぐ主要な観測領域になっています。

### 7.6 観測上の留意事項

ここでの数値は、定められた期間内にCyber Heat Radarで掲載された話題、掲載回数、関連CVE、カテゴリ分類に基づく集計です。温度分布は話題単位の件数であり、掲載項目数や生成レポート数とは一致しません。CVE、KEV公式掲載CVE、PoC/Exploit候補ありCVEの各件数は、観測期間中に掲載対象となった話題との関連に基づいています。PoC/Exploit候補件数は、公開候補として確認された情報の件数であり、URLそのものは掲載していません。
