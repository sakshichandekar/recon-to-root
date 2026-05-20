# Kioptrix Walkthrough

## Overview

This walkthrough documents the exploitation of the Kioptrix vulnerable machine in a controlled lab environment.

The assessment included:
- reconnaissance
- service enumeration
- SMB enumeration
- vulnerability exploitation
- root access

---

## Attack Path Summary

1. Performed network scanning and identified exposed services
2. Enumerated SMB, RPC, and web services
3. Identified outdated Samba version
4. Exploited vulnerable Samba service
5. Gained remote root access on the target machine

---

## Key Findings

- Multiple outdated services exposed
- Null SMB sessions enabled
- Weak SMB configuration observed
- Vulnerable Samba version identified
- Successful remote code execution achieved through Samba exploitation

---

## Report

Detailed findings and screenshots are available in:

- [`Kioptrix VAPT Report`](./Kioptrix.pdf)

---
