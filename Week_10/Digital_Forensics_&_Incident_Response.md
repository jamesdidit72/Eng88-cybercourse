# Digital Forensics & Incident Response
## Incident Response
- **Incident response** (IR)
    - Is a structured methodology for handling security incidents, breaches and cyber threats
- **Incident Response Plan** (IRP)      
    - A well-defined incident response plan allows you to effectively identify, minimise the damage and reduce the cost of a cyber attack while finding and fixing the cause to prevent future attacks
### Incident Categorisation
| category | Description |  
|:---------: |:----------------------------:|
| Malicious Code |  |  
| DoS |  |  
| Phishing |  |  
| Unauthorised Access |  |  
| Insider |  |  
| Data Breach |  |  
| Targeted attack |  |

#### Severity Matrix
- Critical
  - over 80% of staff unable to work
  - critical systems offline with no resolution
  - high risk to / definite breach of sensitive client or personal data  
  - Financial impact
  - severe reputational damage - long term effects 
- High
  - 50% of staff unable to work
  -   
- Medium
- Low
#### Steps of IR
**What you should ask yourself in each stage**
- Preparation
  - has everyone been trained on security policies
  - has the training been approved by appropriate management
  - Does the IRT know their roles and the required notifications to make
  - has the team participated in mock drills
- Identification
  - When did the event happen
  - how was it discovered
  - Have any other areas been impacted
  - what is the scope of the compromise
  - does it affect operations
  - has the source (point of entry) of the event been discovered
- Containment
  - Whats been done to contain the breach short term
  - and long term
  - has any discovered malware been quarantined from the rest of the environment
  - what sorts of backups are in place
  -
  -
  -
- Eradication
  - have you securely removed any malware/artifacts from the attacker
  - has the system been hardened, patched and updates applied
  - can the system be re-imaged
- Recovery
  - what can systems be returned to production
  - have systems been patched, hardened and tested
  - can the system be restored from a trusted back up
  - how long will the affected systems be monitored and what will you look for when monitoring
  - what tools will ensure similar attacks will not reoccur
- Post-Incident Activity (lessons learned)
  - what changes needs to be made to the security
  - how should employees be trained differently
  - what weakness did the breach exploit
  - how will you ensure a similar breach doesnt happen again
  
- emergency contact/ communications list
- at least one conference number
- escalation criteria
- system back up and recovery processes list
- Forensics analysis list
- jumpbag list
  - list of overall actions the employee has to take straight away
- security policy review list
#### playbooks
- A playbook (or runbook) is a detailed response plan, usually focused on a specific incident type


## digital Forensics (DF)
Digital forensic science is a branch of forensic science that focuses on the recovery and investigation of material found in digital devices related to cybercrime
#### Computer forensics
- originally, DF was used as the synonym for computer forensics
- now it is limited to analysising and collecting evidence from:
  - computer systems
  - embedded systems
  - any static memory (usbs)
#### Mobile Device Forensics
- collect data from mobile devices
- different from computers as they have inbuilt communication systems such as GSM
- the data retrieved from mobile devices, includes
  - short message services
  - emails
  - data regarding the location of the user
  - call log
  - user dictionary content
  - data from installed apps
  - system files
  - usage logs
  - other deleted data
#### Network forensics
- capturing and analysing network traffic and netowkr packets over local and wide area networks (or internet)
- the analysis also covers intrusion detection
- often considered as a proactive investigation element: uses two systems to collect data:
  - catch it as you can
  - stop look and listen
#### Database Forensics
- study of databases and its metadata fall under this
- database forensic investigator analyses:
  - database content
  - log files
  - in-RAM data
  
#### Forensic data analysis
- it covers the investigation of financial crimes associated with structured data
- the prim,ary motice of forensic data analysis is to find a pattern behind fraudulent activities
#### email forensics
- email header analysis
- email server investigation
- investigation of network devices
- sender mail fingerprints
- software embedded identifiers
- bait tactics
#### Cloud forensics
- the app of digital forensics in cloud computing as a subset of network forensics to gather and preserve evidence in a way that is suitable for presentation in a court of law
- is the amalgamation of all the different forensics
- involves interactions among various cloud actors:
  - provider
  - consumer
  - broker
  - carrier
  - auditors
- legally it is multi-jurisdictional and multi-tenant situations  
### DF Phases
- Phase 1 
  - First response
- Phase 2 
  - Search and Seizure
- Phase 3 
  - Collect the evidence
- Phase 4 
  - Secure the evidence
- Phase 5
  - Data Acquisition
- Phase 6 
  - Data Analysis
- Phase 7
  - Evidence Assessment
- Phase 8 
  - Documentation and Reporting
- Phase 9
  - Testify as an Expert witness