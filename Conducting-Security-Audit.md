# Conducting A Security Audit

## TABLE OF CONTENTS
1. Introduction
2. Scenario
3. Scope of Audit
4. Goals of Audit
5. Controls Assessments Checklist
6. Payment Card Industry Data Security Standard (PCI DSS) Checklist
7. General Data Protection Regulation (GDPR) Checklist
8. System and Organizations Controls (SOC type 1, SOC type 2)  Checklist
9. Recommendations
10. Conclusion

<br>

## 1. Introduction

In this activity, I will conduct a security audit for a fictional company, Botium Toys, a manufacturer and retailer of children's toys. 
With Botium’s expanding online presence, the IT department faces increasing pressure to safeguard the company's digital assets. To address these concerns, a comprehensive IT security audit has been commissioned.
This report will feature important aspects of the audit, including the scope and goals of the audit, and the results of the assessment.


<br><br>
## 2. Scenario

Here are some important facts about Botium Toys' security posture:
- Currently, all Botium Toys employees have access to internally stored data and may be able to access cardholder data and customers’ PII/SPII.
- Encryption is not currently used to ensure confidentiality of customers’ credit card information that is accepted, processed, transmitted, and stored locally in the company’s internal database. 
- Access controls pertaining to least privilege and separation of duties have not been implemented.
- The IT department has ensured availability and integrated controls to ensure data integrity.
- The IT department has a firewall that blocks traffic based on an appropriately defined set of security rules.
- Antivirus software is installed and monitored regularly by the IT department. 
- The IT department has not installed an intrusion detection system (IDS).
- There are no disaster recovery plans currently in place, and the company does not have backups of critical data. 
- The IT department has established a plan to notify E.U. customers within 72 hours if there is a security breach. Additionally, privacy policies, procedures, and processes have been developed and are enforced among IT department members/other employees, to properly document and maintain data.
- Although a password policy exists, its requirements are nominal and not in line with current minimum password complexity requirements (e.g., at least eight characters, a combination of letters and at least one number; special characters). 
- There is no centralized password management system that enforces the password policy’s minimum requirements, which sometimes affects productivity when employees/vendors submit a ticket to the IT department to recover or reset a password.
- While legacy systems are monitored and maintained, there is no regular schedule in place for these tasks and intervention methods are unclear.
- The store’s physical location, which includes Botium Toys’ main offices, store front, and warehouse of products, has sufficient locks, up-to-date closed-circuit television (CCTV) surveillance, as well as functioning fire detection and prevention systems.


 <br><br>
## 3. Scope of Audit
To assess all assets alongside internal processes and procedures related to the implementation of controls and compliance best practices.


<br><br>
## 4. Goals of Audit
- Implement the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF)
- List assets currently managed by the IT department
- Provide an overview of the risks and/or fines that the company might experience due to the current state of their security posture.
- Use a controls and compliance checklist to determine which controls and compliance best practices need to be implemented.


<br><br>
## 5. Controls Assessment

### Current Assets:
* On-premises equipment for in-office business needs
* Employee equipment: end-user devices (desktops/laptops, smartphones), remote workstations, headsets, cables, keyboards, mice, docking stations, surveillance cameras, etc.
* Storefront products available for retail sale on site and online; stored in the company’s adjoining warehouse
* Management of systems, software, and services: accounting, telecommunication, database, security, ecommerce, and inventory management
* Internet access
* Internal network
* Data retention and storage
* Legacy system maintenance: end-of-life systems that require human monitoring 
<br>

### Administrative Controls

|Control Name|Control Type|Explanation|Needs Implementation (X)|
|------------|------------|-----------|-------------------------|
|Least Privilege|Preventative|Users have the least amount of access required to perform their everyday tasks; Currently all employees have access to internatlly stored data|X|
|Disaster Recovery Plans|Corrective|Focuses on how an organizations recover from interruptions with minimal impact on operations; Botium toys has no disaster recovery plans in place|X|
|Password Policies|Preventative|Prevents unauthorized access; Botium has a password policy but passwords not in line with complexity requirements|X|
|Access Control Policies|Preventative|Policies dictating who can access what resources, under what conditions, and at what time; Access controls at Botium have not been implemented|X|
|Account Management Policies|Preventative|Defines how user accounts are created, managed, monitored, and deactivated to protect systems. Reduces attack surface and limits  overall impact from disgruntled/former employees|X|
|Separation of Duties|Preventative|Refers to the dividing of responsibilities among multiple people so that no one person has full control over all aspects of a critical task or system|X|
<br>

### Technical Controls
|Control Name|Control Type|Explanation|Needs Implementation(X)|
|------------|------------|-----------|-----------------------|
|Firewall|Preventative|Filters unwanted or malicious traffic from entering network; Botium Toys already has Firewalls installed| 
|Intrusion Detection Systems|Detective|Detects and prevents anomalous traffic; Botium has no IDS installed|X|
|Encryption|Deterrent|Conversion of readable data into an unreadable format; Encryption is currently not used at Botium|X|
|Backups|Corrective|Backups are copies of data stored in a separate location to protect against data loss; the company does not have backups of critical data|X|
|Password Management|Preventative|Refers to the strategies, tools, and best practices used to create, store, protect, reset, and use passwords securely; Botium has no centralized password management system that enforces the password policy’s minimum requirement|X|
|Antivirus Software|Preventative|A program designed to detect, prevent, and remove malware; Botium has an antivirus installed and regularly monitored| |
|Manual Monitoring, Maintenance, and Intervention|Preventative|Refers to the human hands-on work needed to keep systems secure, functioning, and up to date; Legacy systems are monitored and maintained| |
<br>

### Physical Controls
|Control Name|Control Type|Explanation|Needs Implementation(X)|
|------------|------------|-----------|-----------------------|
|Time-Controlled safe|Deterrent|Security device that only allows access during specific times or after a set delay; Botium's physical location has sufficient locks| |
|Closed Circuit Television (CCTV)|Preventative/Detective|Video surveillance system used to monitor and record activity in a specific area; Botium Toys has CCTV installed| |
|Locks|Preventative/Deterrent|Prevent unauthorized personnel from physically accessing/modifying network infrastructure; Store has sufficient locks| |
|Locking Cabinets (for network gear)|Preventative|Prevent unauthorized personnel from physically accessing/modifying network infrastructure; Store has sufficient locks but could make use of locking cabinets|X|
|Signage indicating alarm service provider|Deterrent|Deter certain types of threats by making the likelihood of a successful attack seem low|X|
|Fire detection and prevention|Detective/Preventative|Detect fire in physical location and prevent damage to physical assets; Botium Toys has functioning fire detection and prevention systems| |

<br><br>

|Control|Yes/No|Explanation|
|-------|------|-----------|
|Least Privilege|No|All Botium Toys employees have access to internally stored data and may be able to access cardholder data and customers’ PII/SPII; Access controls pertaining to least privilege and separation of duties have not been implemented|
|Disaster Recovery Plans|No|No disaster recovery plans currently in place|
|Password Policies|No|Password policy exists but its requirements are not in line with current minimum password complexity requirements|
|Separation of Duties|No|Access controls pertaining to least privilege and separation of duties have not been implemented|
|Firewall|Yes|The IT department has a firewall installed|
|IDS|No|The IT department has not installed an intrusion detection system (IDS)|
|Backups|No|No disaster recovery plans currently in place, and the company does not have backups of critical data|
|Antivirus Software|Yes|Antivirus software is installed and monitored regularly by the IT department|
|Manual monitoring, maintenance, and intervention for legacy systems|No|Legacy systems are monitored and maintained, there is no regular schedule in place for these tasks and intervention methods are unclear|
|Encryption|No|Encryption is not currently used to ensure confidentiality of customers’ credit card information|
|Password Management System|No|No centralized password management system that enforces the password policy’s minimum requirements|
|Locks (offices, storefront, warehouse)|Yes|The store’s physical location, which includes Botium Toys’ main offices, store front, and warehouse of products, has sufficient locks|
|Closed-circuit television (CCTV) surveillance|Yes|The store’s physical location, which includes Botium Toys’ main offices, store front, and warehouse of products, has up-to-date closed-circuit television (CCTV) surveillance|
|Fire Detection/Prevention|Yes|The store’s physical location, which includes Botium Toys’ main offices, store front, and warehouse of products, has functioning fire detection and prevention systems|


<br><br>
## 6. Payment Card Industry Data Security Standard (PCI DSS) Checklist

|Best Practice|Yes/No|Explanation|
|-------------|------|-----------|
|Only authorized users have access to customers’ credit card information|No|All Botium Toys employees have access to internally stored data and may be able to access cardholder data and customers’ PII/SPII|
|Credit card information is stored, accepted, processed, and transmitted internally, in a secure environment|No|Encryption is not currently used to ensure confidentiality of customers’ credit card information|
|Implement data encryption procedures to better secure credit card transaction touchpoints and data|No|Data needs to be encrypted to ensure confidentiality of customer information|
|Adopt secure password management policies|No|Botium Toys has not adoped secure password management policies;Password policies are nominal and no password management system is currently in place|



<br><br>
## 7. General Data Protection Regulation (GDPR) Checklist

|Best Practice|Yes/No|Explanation|
|-------------|------|-----------|
|E.U. customers’ data is kept private/secured|No|The company does not encrypt their customers data|
|There is a plan in place to notify E.U. customers within 72 hours if their data is compromised/there is a breach|Yes|The IT department has established a plan to notify E.U. customers within 72 hours if there is a security breach|
|Ensure data is properly classified and inventoried|No|Data has not been classified|
|Enforce privacy policies, procedures, and processes to properly document and maintain data|Yes|Privacy policies, procedures, and processes have been developed and enforced to properly document and maintain data|


<br><br>
## 8. System and Organizations Controls (SOC type 1, SOC type 2)  Checklist
|Best Practice|Yes/No|Explanation|
|-------------|------|-----------|
|User access policies are established|No|Access controls pertaining to least privilege and separation of duties have not been implemented|
|Sensitive data (PII/SPII) is confidential/private|No|All Botium Toys employees have access to internally stored data and may be able to access cardholder data and customers’ PII/SPII; Customer data not encrypted|
|Enforce privacy policies, procedures, and processes to properly document and maintain data|Yes|The IT department has ensured availability and integrated controls to ensure data integrity|
|Data is available to individuals authorized to access it|No|Sensitive data accessible to ALL employees|

<br><br>
## 9. Recommendations






