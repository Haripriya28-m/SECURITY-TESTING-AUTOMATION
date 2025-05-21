# OWASP ZAP Security Scan Report – Juice Shop

## 🛠 Tool Used
- **OWASP ZAP** (Zed Attack Proxy) – Version 2.16.1

## 🧪 Target Application
- **URL Scanned**: [https://juice-shop.herokuapp.com](https://juice-shop.herokuapp.com)
- **Application Type**: Intentionally vulnerable web application (used for educational and testing purposes)

## ⚡ Scan Method
- Automated scan using:
  - Traditional Spider
  - AJAX Spider
  - Active Scan
- Browser proxy: Firefox

## 🔍 Summary of Alerts Detected

| # | Alert Name                              | Risk Level | Instances |
|---|------------------------------------------|------------|-----------|
| 1 | Content Security Policy (CSP) Not Set    | Medium     | 56        |
| 2 | Cross-Domain Misconfiguration            | Medium     | 72        |
| 3 | Hidden Files Found                       | Medium     | 4         |
| 4 | JavaScript Source File Inclusion         | Medium     | 96        |
| 5 | Timestamp Disclosure - Unix              | Low        | 228       |
| 6 | X-Frame-Options Header Not Set           | Low        | 1         |
| 7 | Strict-Transport-Security Header Missing | High       | 1         |
| 8 | Server Leaks Version Information         | Medium     | 3         |

## 🔧 Suggested Remediation Steps

Here are some general remediation recommendations for common issues:

- **CSP Header Not Set**  
  _Add a strong `Content-Security-Policy` header to prevent cross-site scripting (XSS)._

- **Strict-Transport-Security Not Set**  
  _Use the `Strict-Transport-Security` header to enforce HTTPS connections._

- **Cross-Domain Misconfiguration**  
  _Limit cross-origin requests using CORS headers to trusted domains only._

- **X-Frame-Options Not Set**  
  _Set the `X-Frame-Options` header to `DENY` or `SAMEORIGIN` to protect against clickjacking._

- **Hidden Files**  
  _Remove or restrict access to sensitive files or directories such as `.git`, `.env`, or backups._

---

## 📸 Screenshot

Below is a screenshot of the scan result from OWASP ZAP:

![Image](https://github.com/user-attachments/assets/6b8753cb-254e-438a-a1ab-f4aa0a64a67e)

## 📝 Conclusion

This scan demonstrates the ability to automate web application security testing using OWASP ZAP. All identified vulnerabilities were part of a deliberately insecure web application for testing purposes. This task successfully fulfills the requirement of performing and documenting automated security testing.

