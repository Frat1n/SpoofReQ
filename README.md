# 🛡️ SpoofReQ

**SpoofReQ** is a precompiled `.exe` penetration testing and HTTP spoofing tool written in **GoLang**. It allows ethical hackers and security researchers to craft custom HTTP requests, spoof headers, test for SQL injection, scan IPs and ports, analyze DNS records, and more — all from a simple command-line interface.

There are two versions of SpoofReQ:

- **Free Version** – Offers essential spoofing and scanning features.
- **Paid Version** – Unlocks advanced features like multithreaded scanning, full port sweeps, banner grabbing, stealth scans, DNS tools, and a more powerful Super Scan engine.

> ✅ No installation or Go setup is required. SpoofReQ is distributed as a precompiled `.exe` file. Just download and run it.

---

## 🆓 Free Version – Commands

```
set url <url>                   - Set the target URL
set headers <k:v,...>           - Set custom headers (comma-separated)
set method <GET|POST|PUT|DELETE>- Set HTTP method
set data <body>                 - Set POST/PUT data body
set timeout <seconds>           - Set request timeout (default 10s)
set followredirects <on|off>    - Follow HTTP redirects toggle
set ratelimit <ms>              - Delay between requests in milliseconds
set repeat <count>              - Repeat the request multiple times
rotate user-agent               - Randomly change User-Agent header
spoof ip                        - Randomize X-Forwarded-For header with fake IP
sqli test                       - Append common SQLi payloads to URL or data and run
super scan                      - Perform a deep, in-depth HTTP scan (limited in free version)
run                             - Execute the request(s)
show response                   - Show last response body
show headers                    - Show last response headers
show status                     - Show last response status code only
save <filename>                 - Save last response to file
clear                           - Clear all settings
help                            - Show this help
```

> ⚠️ **Note:** In the Free Version, `super scan` provides only basic vulnerability checks and does not include path brute-forcing, threaded analysis, or fingerprinting.

---

## 💼 Paid Version – Commands

### 🔧 Core Commands

```
set url <url>                   - Set the target URL
set headers <k:v,...>           - Set custom headers (comma-separated)
set method <GET|POST|PUT|DELETE>- Set HTTP method
set data <body>                 - Set POST/PUT data body
set timeout <seconds>           - Set request timeout (default 10s)
set followredirects <on|off>    - Follow HTTP redirects toggle
set ratelimit <ms>              - Delay between requests in milliseconds
set repeat <count>              - Repeat the request multiple times
set threads <count>             - Set scan thread count (default 100)
rotate user-agent               - Randomly change User-Agent header
spoof ip                        - Randomize X-Forwarded-For header with fake IP
run                             - Execute the request(s)
show response                   - Show last response body
show headers                    - Show last response headers
show status                     - Show last response status code only
save <filename>                 - Save last response to file
clear                           - Clear all settings
help                            - Show this help
exit                            - Exit the tool
```

### 🛰️ IP & Port Scanning

```
ipscan ports <ip>               - Scan top ports
ipscan full <ip>                - Scan full TCP range (1-65535)
ipscan banner <ip> <port>       - Grab service banner
ipscan detect <ip>              - Basic OS fingerprinting
ipscan open <ip>                - List only open ports
ipscan services <ip>            - Identify services
ipscan stealth <ip>             - Stealth scan
```

### 🌐 HTTP/Web App Scanning

```
ipscan http-check <ip>          - Probe HTTP/HTTPS
ipscan paths <ip>               - Check common paths
ipscan tls <ip>                 - Check TLS certificate
```

### 📡 DNS Analysis

```
ipscan dns <domain>             - DNS records lookup
ipscan reverse <ip>             - Reverse DNS lookup
```

### 🔐 Security Testing

```
sqli test                       - Test SQL injection
super scan                      - Comprehensive scan with full engine
```

---

## ⚖️ Feature Comparison

| Feature                        | Free Version ✅ | Paid Version 🔥 |
|-------------------------------|----------------|-----------------|
| Custom HTTP Requests          | ✅             | ✅              |
| IP & Header Spoofing          | ✅             | ✅              |
| SQL Injection Test            | ✅             | ✅              |
| Super Scan                    | Basic          | Full Power 💥   |
| Threaded Requests             | ❌             | ✅              |
| IP/Port Scanning              | ❌             | ✅              |
| DNS Tools                     | ❌             | ✅              |
| Stealth Scans & OS Detection  | ❌             | ✅              |
| TLS Certificate Scanning      | ❌             | ✅              |

---

## 📂 Usage

Just run the precompiled `.exe` file in your terminal, command prompt or simply start it by double clicking it on the desktop or any other file explorer:

```
SpoofReQ.exe
```

Type `help` inside the tool to view available commands.

---

## 🛑 Disclaimer

SpoofReQ is intended **only for educational and authorized penetration testing** purposes. Do **not** use this tool against systems or networks you do not own or have permission to test. Unauthorized use is illegal. The creator assumes no responsibility for misuse or damage caused by this software.

---

## 🗒️ Legal Notice

By purchasing the **paid version** of SpoofReQ, you acknowledge and agree to the following terms:

- You **may not** distribute, share, or provide the paid version of SpoofReQ to any third parties, including friends, colleagues, or acquaintances, without explicit written permission from the author.
- You **may not** claim ownership of the tool, resell, sublicense, or otherwise commercialize the software or its features.
- Unauthorized redistribution or sharing of the paid version is a violation of the license agreement and may result in immediate termination of your access, revocation of updates, and potential legal action.
- If you obtained SpoofReQ from an unauthorized third party, you are advised to seek a refund as the software must be purchased directly through official channels to ensure support and updates.
- This agreement is binding and intended to protect the intellectual property rights of the author and ensure fair use of the software.

Failure to comply with these terms will be treated seriously and may result in legal consequences. Please use SpoofReQ responsibly and ethically.

---

## 🧠 Credits
- Made by Evelitions
- Developed in GoLang
- Designed for speed, stealth, and portability
- Inspired by tools like Metasploit, Nmap, and sqlmap

For issues, feature requests, or paid version access, contact: `zzqxyz19@gmail.com`
