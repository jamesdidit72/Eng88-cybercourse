# Penetration Testing

## Defintion:
- **Is:** A method for gaining assurance in the security of an IT system
- **By:** Attempting to breach some or all of that system's security
- **Using:** the same tools and techniques
- **As:** An adversary might

## Cyber Security Colours 
### Teams
- Blue Team:
  - Defenders: Responsible for implementing defensive security, damage control and incident response
- Red Team:
  - Breakers/ Attackers: a team commissioned to perform "ethical hacking" on a organisation, including: 
    - compliance testing
    - black box testing
- white Team:
  - Admins: responsible for refereeing an engagement between a red team of mock attackers and a blue team of actual defenders
- Yellow Team:
  - Builders: Responsible for developing the security system of an organisation
    
### Hackers
- Black hat: Attackers (extensive knowledge of systems, develop malicious software)(motivations: personal, financial, political, etc (refer to threat actors))
- White hat: Extensive knowledge, use it for good (pen testing, ethical hacking) Requires permission from the target
- Grey hat: They look for vulnerabilities in systems without permission, then report any issues (may ask for a fee for finding the fault)
### Testing
- Whitebox Testing: Full knowledge of the system being tested
- Blackbox Testing: No info about the internal system, from an external hacker perspective
- Greybox Testing: the attacker has partial knowledge of the system

## Pentesting Characteristics
### Pen Testers
- Pentesters can be internal employees or a 3rd party pen testers
- 3rd party tests should be performed by qualified and experienced staff only
- tests cannot be procedural, quality of the
- NCSC recommends that HMG orgs use testers which are part of the CHECK scheme
### Pentesting Objectives
- Vulnerability identification in bespoke or niche software (web applications)
- Scenario driven testing aimed at identifying vulnerabilities (see if an employee loses their laptop, can this laptop be used maliciously?)
- Scenario driven testing of detection and response capability

### Pentesting Scope
- A well-scoped pen test cab give confidence:
    - that the products and security controls tested have been configured
### Pen testing Results
- used to identify the level of technical risk of the soft and hardware vulnerabilities
- what is used, targets allowed, knowledge of the system given beforehand
- can only validate that the IT system are not vulnerable to any known issue on the day of the test
### PenTesting Expiry
- uncommon for a year or more to pass between pen test
- test can be valid for a year or a day, depending when a vulnerability occurs in the system
### pentesting start point
- external network pen test:
    - what most people think when we talk about pen testing
- internal network pen test:
    - simulates the actions a hacker might take once access has been gained to a network (could be a hacker, malicious actor or a disgruntled employee)

### Pen testing methods/ targets    
- physical pen testing (gaining access to a building)
- social engineering pen testing (target human factors/ manipulating people)
- web app pen testing (lost of sensitive data online)
- client side pen testing (a software in the clients system (vulnerability in the browser you're using))
- cloud pen testing ()

### pentesting blindness level
- targeted (blindless) pen test (working as a group)
- blind pen testing (alone, no help)
- double blind pen testing (both have no info about the other, can test the defence against any potential breach)

## Pentesting Phases
- 1st phase:
    - Pre-Engagement interactions
        - outline the logistics, the goals, legal restrictions (outline all parameters of the test)
- 2nd phase:
    - Reconnaissance
        - gather information about the target
- 3rd phase:
    - Scanning/ Inspection
        - come into contact with the target (open ports, ip addresses etc)
- 4th phase:
    - threat modelling
        - pen tester will try to exploit the vulnerability found in the previous steps
- 5th phase:
    - Exploitation
        - more technical than threat modelling
- 6th phase:
    - Foothold installation
        - once you have compromised the system, you try to elevate your privileges
- 7th phase:
    - analysis and reporting
        - carefully report step by step
- 8th phase:
    - cleanup and remediation
        - fix what they broke, removed, opened etc
        - put it back to what the system was before the test began