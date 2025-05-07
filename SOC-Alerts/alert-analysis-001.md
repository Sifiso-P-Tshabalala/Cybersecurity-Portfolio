# 🚨 Alert Analysis Report – 001

**Analyst:** Sifiso P. Tshabalala  
**Date:** 2025-05-07  
**Alert ID:** SOC-ALERT-001  
**Severity:** High  
**Status:** Resolved  

---

## 🛑 Alert Summary

- **Alert Type:** Brute Force Login Attempt
- **Source:** Microsoft Defender for Endpoint
- **Detection Time:** 02:43 AM (UTC+2)
- **Affected Host:** HR-Laptop-12
- **Username Targeted:** katlego@udtrucks.co.za

---

## 🔍 Analysis Details

A high number of failed login attempts were detected within a short time frame from an external IP address (45.67.89.22). The system flagged this as a potential brute force attack targeting a domain user account.

The login attempts originated from a non-whitelisted IP located in **Nigeria** and were directed at the organization's VPN gateway.

---

## 🛡️ Response Actions

- Blocked source IP via firewall rules
- Forced password reset for the affected user
- Temporarily disabled the account to prevent lockout risk
- Conducted system-wide credential exposure review
- Updated SIEM rules to escalate similar attempts in future

---

## ✅ Lessons & Recommendations

- Implement MFA on VPN and O365 logins
- Enforce IP allow-listing for remote access services
- Review and lower lockout threshold for critical accounts

---

## 📎 Artifacts

- SIEM Screenshot (saved separately)
- Firewall log extract
- User activity timeline

---

> _This report is a fictional sample created to showcase analytical thinking and incident response process for entry-level cybersecurity roles._
