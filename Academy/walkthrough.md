# Academy Walkthrough

## Overview

This walkthrough documents the penetration testing process performed on the Academy vulnerable machine in a controlled lab environment.

The assessment focused on:
- reconnaissance
- FTP enumeration
- credential discovery
- web exploitation
- reverse shell access
- privilege escalation

---

## Attack Path Summary

1. Identified exposed FTP, SSH, and HTTP services on the target machine
2. Discovered anonymous FTP access
3. Retrieved sensitive credentials from an exposed file
4. Cracked MD5 password hash and accessed the web application
5. Uploaded a PHP reverse shell through insecure file upload functionality
6. Gained shell access as `www-data`
7. Performed local enumeration using LinPEAS
8. Retrieved credentials from `config.php`
9. Logged in through SSH as user `grimmie`
10. Exploited writable scheduled task script to gain root access

---

## Key Findings

- Anonymous FTP login enabled
- Sensitive credentials exposed through accessible files
- Weak MD5 password hashing used
- Insecure file upload functionality allowed remote code execution
- Hardcoded credentials stored in configuration files
- Writable scheduled task enabled privilege escalation

---

## Report

Detailed findings and screenshots are available in:

- [`Academy VAPT Report`](./Academy.pdf)

---
