# 🔐 DNS Security Audit Tool

A DNS Security Audit Tool that checks a DNS server for potential security vulnerabilities. This tool helps identify misconfigurations and flaws in DNS infrastructure, ensuring better protection and network stability.

---

## 🧪 What It Does

This tool performs **8 essential security checks** on a provided DNS server IP:

1. **DNSSEC Check**  
   - Verifies if DNS responses are cryptographically signed.
   - ❌ If disabled, responses can be spoofed.

2. **Cache Snooping Check**  
   - Checks if an outsider can query the DNS cache.
   - ❌ Vulnerable servers may leak internal DNS activity.

3. **DNS Rebinding Check**  
   - Tests for DNS rebinding vulnerability.
   - ✅ Safe servers block such behavior.

4. **DNS Amplification Check**  
   - Measures the amplification factor of DNS responses.
   - ⚠️ High amplification can be abused for DDoS attacks.

5. **Wildcard Injection Check**  
   - Detects if DNS resolves non-existent subdomains.
   - ✅ Safe servers don’t return wildcard entries.

6. **NXDOMAIN Attack Check**  
   - Checks for denial-of-service risk due to non-existent domain flooding.
   - ✅ Secure servers handle invalid queries properly.

7. **DNS Reflection Check**  
   - Tests if the server can be used in reflective DDoS attacks.
   - ❌ Vulnerable if large responses go to spoofed IPs.

8. **Open Recursion Check**  
   - Verifies if the server allows public recursive queries.
   - ✅ Safe servers restrict recursion to trusted users.

---

## 🧑‍🏫 Academic Info

- **Instructor:** Asst. Prof. Engr. Abdul Rahman  
- **Student:** Muhammad Ali

---

## ▶️ How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/dns-security-audit-tool.git
cd dns-security-audit-tool
