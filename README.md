# Lab 02: Threat Modelling - Group X (University Digital Library)

## Group Members
* **M Hammad (051)** - Group Lead / GitHub Maintainer
* **Ali Hamza (027)** - Asset and Boundary Analyst
* **Saim Ali Shahid (020)** - Threat Analyst

## Scenario Description
The University Digital Library is a web application where students and teachers search and download digital books and papers. Librarians manage the content, while administrators control accounts and permissions. The system uses a cloud database and requires login for all users. The primary security goal is to ensure secure, role-based access with no unauthorized access, tampering, or service disruption.

## Project Metrics
* **Total Assets identified:** 10
* **Total Threats identified:** 12 (Covering all 6 STRIDE categories)
* **Total Risks registered:** 12

## Repository Files
* `Lab02_GroupX_LibrarySystem.json` - The OWASP Threat Dragon model file containing the DFD and threats.
* `Lab02_ThreatReport.pdf` - The automatically generated Threat Dragon PDF report.
* `Lab02_Final_Report.pdf` - The final comprehensive lab report containing the Risk Register, SDLC mapping, and practice questions.

## Top 3 Risks & Mitigations
1. **R12: SQL Injection in Search Query (Score: 25 - Critical)** 
   * *Mitigation:* Implement parameterized queries and strict input validation.
2. **R1: Password Guessing on Login (Score: 20 - Critical)**
   * *Mitigation:* Lockout after 5 failed attempts, rate limiting, and MFA.
3. **R6: Student Gains Admin Rights (Score: 20 - Critical)**
   * *Mitigation:* Strict server-side Role-Based Access Control (RBAC) checks.
