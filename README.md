# SECURITY-TESTING-AUTOMATION

# Security Testing Project – OWASP Juice Shop

## 🔐 Tool Used
- **OWASP ZAP** (v2.16.1)

## 🧪 Target Web Application
- [OWASP Juice Shop](https://juice-shop.herokuapp.com/)

## 🛠️ Scan Type
- Automated Scan using Traditional and AJAX Spider

## ⚠️ Key Findings
- CSP Header Not Set (56 occurrences)
- Cross-Domain Misconfiguration (72)
- Hidden Files Found (4)
- JavaScript Source File Inclusion (96)
- Timestamp Disclosure - Unix (228)
- and others...

## 📸 Screenshot
![Scan Screenshot](screenshot.png)

## 📂 Report
Detailed findings can be found in the [zap-scan-report.md](zap-scan-report.md) file.

> **Disclaimer**: This scan was performed on a publicly available test site for educational purposes.
