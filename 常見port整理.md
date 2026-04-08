## 常見 Port 表格

| 協定 / 服務            | Port | 傳輸層     | 用途                       | 常見考點 / 備註                |
| ------------------ | ---: | ------- | ------------------------ | ------------------------ |
| FTP                |   20 | TCP     | 資料傳輸                     | FTP Data                 |
| FTP                |   21 | TCP     | 控制連線                     | 明文傳輸，常考不安全               |
| SSH                |   22 | TCP     | 安全遠端登入                   | 可取代 Telnet、也可做 SCP/SFTP  |
| Telnet             |   23 | TCP     | 遠端登入                     | 明文，不安全                   |
| SMTP               |   25 | TCP     | 郵件傳送                     | Mail Server 間傳信常用        |
| DNS                |   53 | TCP/UDP | 網域名稱解析                   | UDP 常見查詢，TCP 常用區域傳送/大型回應 |
| DHCP Server        |   67 | UDP     | DHCP 伺服器端                | 常與 68 一起考                |
| DHCP Client        |   68 | UDP     | DHCP 用戶端                 | 取得 IP                    |
| TFTP               |   69 | UDP     | 簡易檔案傳輸                   | 無驗證，常考弱點                 |
| HTTP               |   80 | TCP     | 網頁服務                     | 明文                       |
| POP3               |  110 | TCP     | 收信                       | 將郵件抓到本地端                 |
| NTP                |  123 | UDP     | 網路校時                     | 時間同步                     |
| NetBIOS            |  137 | UDP     | 名稱服務                     | Windows 舊式網路服務           |
| NetBIOS            |  138 | UDP     | 資料報服務                    | Windows 舊式網路服務           |
| NetBIOS            |  139 | TCP     | Session Service          | 常與 SMB 一起考               |
| IMAP               |  143 | TCP     | 收信                       | 郵件保留在伺服器                 |
| SNMP               |  161 | UDP     | 網管監控                     | 常見設備管理                   |
| SNMP Trap          |  162 | UDP     | SNMP 通知                  | Trap 訊息                  |
| BGP                |  179 | TCP     | 路由交換                     | 大型網路、自治系統                |
| LDAP               |  389 | TCP/UDP | 目錄服務                     | AD 常見                    |
| HTTPS              |  443 | TCP     | 加密網頁服務                   | TLS/SSL                  |
| SMB / CIFS         |  445 | TCP     | 檔案分享                     | Windows 檔案共享，資安很常考       |
| Syslog             |  514 | UDP     | 系統日誌                     | 日誌集中管理                   |
| SMTPS              |  465 | TCP     | 加密 SMTP                  | 舊式加密 SMTP                |
| IPsec ISAKMP / IKE |  500 | UDP     | VPN 金鑰交換                 | VPN 常考                   |
| LDAPS              |  636 | TCP     | 加密 LDAP                  | LDAP over SSL/TLS        |
| FTPS               |  989 | TCP     | FTP Data over SSL/TLS    | 加密 FTP                   |
| FTPS               |  990 | TCP     | FTP Control over SSL/TLS | 加密 FTP                   |
| IMAPS              |  993 | TCP     | 加密 IMAP                  | 安全收信                     |
| POP3S              |  995 | TCP     | 加密 POP3                  | 安全收信                     |
| MS SQL Server      | 1433 | TCP     | Microsoft SQL 資料庫        | 常見 DB Port               |
| Oracle DB          | 1521 | TCP     | Oracle 資料庫               | 常考                       |
| MySQL              | 3306 | TCP     | MySQL 資料庫                | 常見 DB Port               |
| RDP                | 3389 | TCP     | Windows 遠端桌面             | 遠端控制                     |
| PostgreSQL         | 5432 | TCP     | PostgreSQL 資料庫           | 常見 DB Port               |
| VNC                | 5900 | TCP     | 遠端桌面控制                   | 圖形化遠端                    |
| SOCKS Proxy        | 1080 | TCP     | 代理服務                     | Proxy 題目常見               |
| PPTP               | 1723 | TCP     | VPN                      | 舊式 VPN                   |
| L2TP               | 1701 | UDP     | VPN                      | 常搭配 IPsec                |
| SIP                | 5060 | TCP/UDP | VoIP 訊號控制                | 網路電話                     |
| SIP-TLS            | 5061 | TCP     | 加密 VoIP 訊號               | SIP over TLS             |
| Kerberos           |   88 | TCP/UDP | 身分驗證                     | AD / 網域驗證常考              |
| RADIUS             | 1812 | UDP     | 驗證授權                     | AAA                      |
| RADIUS Accounting  | 1813 | UDP     | 計費記錄                     | AAA                      |
| NFS                | 2049 | TCP/UDP | 網路檔案系統                   | Linux/Unix 常見            |
| Elasticsearch      | 9200 | TCP     | 搜尋/分析引擎                  | 常見於日誌分析平台                |
| WinRM              | 5985 | TCP     | Windows 遠端管理             | HTTP                     |
| WinRM over HTTPS   | 5986 | TCP     | Windows 遠端管理             | HTTPS                    |

---

## 考試最常考的一小份

如果你時間不多，先背這些：

|      Port | 服務         |
| --------: | ---------- |
|   20 / 21 | FTP        |
|        22 | SSH        |
|        23 | Telnet     |
|        25 | SMTP       |
|        53 | DNS        |
|   67 / 68 | DHCP       |
|        69 | TFTP       |
|        80 | HTTP       |
|       110 | POP3       |
|       123 | NTP        |
|   137-139 | NetBIOS    |
|       143 | IMAP       |
| 161 / 162 | SNMP       |
|       389 | LDAP       |
|       443 | HTTPS      |
|       445 | SMB        |
|       993 | IMAPS      |
|       995 | POP3S      |
|      1433 | MSSQL      |
|      1521 | Oracle     |
|      3306 | MySQL      |
|      3389 | RDP        |
|      5432 | PostgreSQL |
|      5900 | VNC        |

---

## 背誦技巧

### 1. 先分成「遠端連線 / 網頁 / 郵件 / 網路服務 / 資料庫」

* 遠端：22 SSH、23 Telnet、3389 RDP、5900 VNC
* 網頁：80 HTTP、443 HTTPS
* 郵件：25 SMTP、110 POP3、143 IMAP、993/995 加密版
* 網路服務：53 DNS、67/68 DHCP、69 TFTP、123 NTP、161/162 SNMP
* 檔案共享：20/21 FTP、445 SMB、2049 NFS
* 資料庫：1433 MSSQL、1521 Oracle、3306 MySQL、5432 PostgreSQL

### 2. 記「明文 vs 加密」

* Telnet 23 → 明文
* SSH 22 → 加密
* HTTP 80 → 明文
* HTTPS 443 → 加密
* POP3 110 / IMAP 143 → 明文版
* POP3S 995 / IMAPS 993 → 加密版

### 3. 郵件協定常一起考

* SMTP 25：寄信
* POP3 110：收信下載
* IMAP 143：收信同步

---

## 資安角度常見考點

| Port | 重點                              |
| ---: | ------------------------------- |
|   21 | FTP 明文帳密，容易被攔截                  |
|   23 | Telnet 明文登入，非常危險                |
|   69 | TFTP 無驗證                        |
|   80 | HTTP 明文傳輸                       |
|  445 | SMB 常見橫向移動、勒索攻擊考點               |
| 3389 | RDP 常見暴力破解目標                    |
|  161 | SNMP 若使用預設 community string 風險高 |

---

## 一句話速記版

* **22 遠端安全登入**
* **23 遠端明文登入**
* **53 DNS**
* **80/443 網頁**
* **110/143/25 郵件**
* **161/162 SNMP**
* **445 SMB**
* **3306 MySQL**
* **3389 RDP**
