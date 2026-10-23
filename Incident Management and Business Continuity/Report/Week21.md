# Incident Management and Business Continuity Report
 ## Project Overview

This repository contains a completed Business Continuity and Disaster Recovery (BCDR) 
assessment prepared as part of the GRC205 Business Continuity and Disaster Recovery
course at the International Cybersecurity and Digital Forensics Academy (ICDFA).

The project analyzes a severe flooding and power outage scenario affecting
Northbridge Skills Institute**, evaluates business impacts, defines recovery objectives,
designs backup and recovery strategies, develops a coordinated business continuity 
plan,and assesses organizational resilience against established industry frameworks.

 ## Scenario Summary

At 08:00 WAT on Day 0, Northbridge Skills Institute experiences:

- Severe flooding
- Power failure
- Loss of access to the primary site

### Available Services
 - Microsoft 365 Identity Services
 - Microsoft 365 Email

### Unavailable Services
 - AUTH01
 - DB01
 - LMS01
 - On-premises applications
 - Local infrastructure

The primary business concern is maintaining critical operations while protecting an examination scheduled for 11:00 WAT

### Project Objectives

The assignment addresses:

- Business Impact Analysis (BIA)
- Recovery Time Objectives (RTO)
- Recovery Point Objectives (RPO)
- Maximum Tolerable Downtime (MTD)
- Backup and Recovery Design
- Disaster Recovery Strategy Selection
- Business Continuity Planning
- Recovery Scheduling
- Governance and Compliance
- BC/DR Performance Measurement

### Key Findings

- Teaching and Assessment is the highest-priority service.
- LMS dependency creates a significant recovery bottleneck.
- AUTH01 and DB01 represent critical shared dependencies.
- A single failure can affect multiple business functions simultaneously.


### Estimated Losses

Outage Duration and Estimated Impact
- 8 Hours  NGN 1,200,000 
- 24 Hours NGN 3,360,000 

### Additional examination rescheduling cost:

- NGN 120,000 one-time penalty

### Key Observation

Current recovery capability does not fully satisfy the proposed objectives because:

- LMS01 misses the examination deadline.
- AUTH01 recovery points are too old.
- Backup independence controls require validation.

 ### Backup and Recovery Architecture

 Backup Design

 #### DB01

- Daily Full Backup
- Hourly Incremental Backups
- 35-Day Daily Retention
- 12-Week Weekly Retention
- 12-Month Monthly Retention

#### AUTH01

- Configuration Backup Every 4 Hours
- System State Protection
- Secure Recovery Credential Storage

#### FS01

- Incremental Backup Every 4 Hours
- Daily Full Backup
- Metadata Preservation
- ACL Preservation



### 3-2-1 Backup Strategy

The design follows:

- 3 Copies of Data
- 2 Different Storage Media
- 1 Offsite Copy

### Additional controls:

- Immutable Backups
- Multi-Factor Authentication
- Least Privilege Access
- Encryption at Rest
- Encryption in Transit
- Dual Approval for Deletion

### Disaster Recovery Strategy Evaluation
Options Compared
Cold Site is 1,200,000 for 24–48 Hours
Warm Site is 2,100,000 for 3–5 Hours
Hot Site is 3,000,000 Approximately 1 Hour

### Recommended Option
Warm Site + Protected Backups

### Reasons
- Meets budget constraints
- Improves recoverability significantly
- Provides balanced cost-to-benefit ratio
- Supports critical operational restoration

### Limitations
- Examination deadline still missed
- Authentication recovery gap remains
- Requires regular testing and validation


 ### Business Continuity Plan (BCP)
Activation Criteria
BC/DR procedures are activated when:
- Critical services fail for over 30 minutes
- Site safety is compromised
- Recovery objectives are threatened
- MTD thresholds may be exceeded

 ### Command Structure
 Key Roles
- Institute Director
- BC/DR Coordinator
- DR Lead
- Facilities Lead
- Business Owners
- Incident Response Lead

### Communication Channels
Primary:
- Microsoft 365 Email
- Approved Messaging Platforms

### Fallback:
- Phone Trees
- SMS Notifications

 ### Recovery Runbook
Recovery Sequence
1. Incident Declaration
2. Site Safety Validation
3. Recovery Network Restoration
4. AUTH01 Recovery
5. Backup Integrity Validation
6. DB01 Recovery
7. FS01 Recovery
8. Application Restoration
9. Business Acceptance Testing
10. Return-to-Service Approval

### Recovery Testing Results
Baseline Recovery Timeline
Service with Recovery Time 
  - Recovery Network 08:30 
  - AUTH01  09:00 
  - Security Validation  09:30 
  - FS01  10:30 
  - DB01  11:00 
  - LMS01  11:45 
  - FIN01  11:30 
  - REG01  12:00 
  - HR01  12:30 


 ### Results Summary
Successful Objectives
- Finance RTO Achieved
- Admissions RTO Achieved
- Payroll RTO Achieved
- Records RTO Achieved


### Failed Objective
-Teaching & Assessment RTO Missed

#### Reason:
- LMS restoration completed at 11:45
- Examination deadline was 11:00

 ### Corrective Action Plan
Priority 1 Actions
- Separate Production and Backup Administrators
- Enforce MFA Everywhere
- Document Provider Independence
- Implement Immutable Backup Validation
- Reduce AUTH01 Recovery Point Age
- Validate Exam Continuity Procedures

 ### Priority 2 Actions
- Test Finance Reconciliation Processes
- Conduct Full End-to-End Recovery Testing
- Train Coordinators on Manual Procedures

 ### Governance Alignment
NIST SP 800-34 Rev.1
Mapped areas include:
1. Planning Authority
2. Business Impact Analysis
3. Preventive Controls
4. Recovery Strategy
5. Plan Development
6. Testing & Exercises
7. Maintenance & Improvement

### ISO 22301 Alignment
The project addresses:
- Organizational Context
- Leadership
- Planning
- Support
- Operations
- Performance Evaluation
- Continual Improvement

Climate resilience considerations were also incorporated through reference to the ISO 22301:2019 Climate Action Amendment.
 Maturity Assessment
 Current State
 Level 2 – Developing (Repeatable)

### Characteristics:
- Basic continuity plans exist
- Recovery process is repeatable
- Testing is inconsistent
- Recovery success varies


 ### Target State
Level 3 – Defined (Standardized)
Desired improvements:
- Formal governance structure
- Standardized procedures
- Regular testing program
- Measured recovery performance
- Evidenced corrective actions

 ### Key Lessons Learned
- Business continuity is more than restoring technology.
- Technical recovery must support business recovery.
- Examination continuity requires pre-approved alternatives.
- Backup availability does not guarantee recoverability.
- Continuous testing is essential for resilience.

 ### Conclusion
The analysis demonstrates that Northbridge Skills Institute can recover critical
operations using a warm-site strategy supported by protected backups and governance controls.
However, recovery capabilities must be strengthened through improved identity recovery, backup independence,
validation testing, and continuity planning for examination services.
Successful resilience depends on tested recovery procedures, business-owner acceptance,
measurable performance metrics and continuous improvement rather than recovery technology alone

### References
- NIST SP 800-34 Rev.1: Contingency Planning Guide for Federal Information Systems
- ISO 22301:2019 Business Continuity Management Systems
- ISO 22301:2019/Amd 1:2024 Climate Action Amendment
- ICDFA GRC205 Week 21 Learning Materials


Atusasiire Daren Cared  
ICDFA Student Batch B2025  
Governance, Risk & Compliance Engineering(GRCE)

