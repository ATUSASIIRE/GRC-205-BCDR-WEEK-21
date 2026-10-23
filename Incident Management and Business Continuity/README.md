# Northbridge Skills Institute BCDR Project

## Overview
This repository contains a completed Business Continuity and Disaster Recovery (BCDR) analysis developed for the GRC205 course at the International Cybersecurity and Digital Forensics Academy (ICDFA).

The project evaluates a flooding and power outage scenario affecting Northbridge Skills Institute and provides a comprehensive continuity and recovery strategy covering:

- Business Impact Analysis (BIA)
- Recovery Time Objectives (RTOs)
- Recovery Point Objectives (RPOs)
- Backup and Restore Design
- Disaster Recovery Strategy Evaluation
- Business Continuity Planning
- Incident Management Coordination
- Recovery Scheduling and Testing
- Governance, Metrics, and Continuous Improvement

## Project Information
- Student: Atusasiire Daren Cared
- Student ID: 2025/GRC/12793
- Course: GRC205 – Business Continuity and Disaster Recovery
- Module: Week 21 – Incident Management and Business Continuity
- Instructor: Mr. Aminu Idris

## Scenario Summary
Northbridge Skills Institute experiences severe flooding and a power failure that renders the primary site inaccessible.

Available:
- Microsoft 365 Identity Services
- Email Services

Unavailable:
- AUTH01
- DB01
- LMS01 and dependent applications
- On-premises infrastructure

The exercise focuses on maintaining business operations, protecting critical services, recovering systems, and minimizing disruption to examinations, finance, admissions, payroll, and records management.

## Key Deliverables
### 1. Business Impact Analysis
Identified and prioritized five critical business functions:
1. Teaching and Assessment
2. Finance and Fee Processing
3. Admissions and Registration
4. Payroll Services
5. Records and Certificates

### 2. Recovery Objectives
Defined:
- RTO
- RPO
- Maximum Tolerable Downtime (MTD)

Mapped recovery targets to business requirements and service acceptance criteria.

### 3. Backup Strategy
Implemented recommendations based on:
- 3-2-1 Backup Rule
- Offsite Protection
- Immutable Backups
- Recovery Validation Testing
- Incremental and Full Backup Scheduling

### 4. Recovery Strategy Evaluation
Compared:
- Cold Site
- Warm Site
- Hot Site

Recommended a Warm Site strategy with protected backups and regular testing as the most cost-effective option within budget.

### 5. Business Continuity Plan
Developed:
- Incident activation criteria
- Recovery runbook
- Communication plan
- RACI matrix
- Temporary operating procedures
- Service restoration workflow

### 6. Governance and Compliance
Aligned recommendations with:
- NIST SP 800-34 Rev.1
- ISO 22301:2019
- ISO 22301:2019 Amendment 1 (Climate Action)

## Recovery Highlights
- Critical path recovery completed in approximately 4.5 hours.
- LMS restoration projected at 11:45, missing the scheduled 11:00 examination.
- Continuity workarounds required to preserve assessment operations.
- Major improvement areas identified around backup independence, identity recovery, and recovery validation.

## Skills Demonstrated
- Governance, Risk & Compliance (GRC)
- Business Impact Analysis (BIA)
- Disaster Recovery Planning
- Business Continuity Management
- Risk Assessment
- Incident Response Coordination
- Recovery Testing and Validation
- ISO 22301 Alignment
- NIST Framework Application
- Operational Resilience Planning

## Repository Contents
README.txt                 - Project summary
GRC205_BCDR_Week21_Atusasiire_Daren_Cared.doc  - Full assignment report

## Key Outcome
The project concludes that business continuity success depends not only on restoring systems but also on validating data integrity, maintaining governance controls, executing tested recovery procedures, and ensuring business acceptance before service restoration is declared complete.

## Disclaimer
This work was produced for academic learning purposes as part of the ICDFA GRC205 curriculum and reflects the scenario assumptions provided in the assignment brief.
