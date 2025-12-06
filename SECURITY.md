# Security Scanning

## Overview
This repository uses three types of security scanning:

### SAST (Static Analysis with CodeQL)
- Scans source code for vulnerabilities
- Runs on push to main branch
- Checks for: [Logic issues, unsafe code, dangerous api usage, other misconfigurations]
- Artifacts: See GitHub Security tab

### SCA (Dependency Check)
- Scans Python packages for known CVEs
- Runs on push to main branch
- Checks for: [Outdated package version, known CVEs in dependencies, retired libraries, CVSS Severity scoring]
- Artifacts: sca-reports

### DAST (Live Application with ZAP)
- Tests running application for vulnerabilities
- Runs on push to main branch
- Checks for: [Missing security headers, runtime configuration issues, sercer information leakage, bad endpoint behavior]
- Artifacts: zap-baseline-reports, zap-fullscan-reports

## Understanding Results
[Link to Part 10 in README]

## Reporting Vulnerabilities
Please email security@example.com