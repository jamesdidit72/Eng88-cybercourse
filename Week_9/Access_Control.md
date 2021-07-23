# Access Control
## Models
- Discretionary AC (DAC)
  - Some OS uses  DAC
- Mandatory AC (MAC)
  - strict AC, protect important assets
  - the security clearance thing
- Role-based AC (RBAC) 
  - based on the individuals role (security privilege)
- Attribute-based AC (ABAC)
  - allows access based on the attributes of the object
- Rule-based AC (RBAC)
  - specifys a set of rules associated to a system (allowed/denied access protocols)
- Time-based AC (TBAC)
  - allows access depending on time (no access on weekends)
- The principle of least privilege
  - Giving someone more access than they need, which is bad practice
    
## AAA Framework
- Authentication
  - Users and admins must prove that they are who they say they are
- Authorisation
  - Authorisation services determine which resources the user can access and which operations the user is allowed to perform
- Accounting
  - Accounting records what the user does, including what is accessed, the amount of time the resource is accessed and any changes that were made

## AAA Architecture    
- Local AAA Authentication
  - sometimes known as self-contained authentication because it authenticates users against locally stored usernames and passwords
- Server-based AAA Authentication
  - This method authenticates against a central AAA server that contains the usernames and passwords for all users
    
## AAA Protocols
- RADIUS
  - Remote authentication dial-in user service (RADIUS)
  - a protocol that supports centralised authentication, authorisation and accounting management  for clients that establish connection with a network and intend to use any of the provided services 
- TACACs
  - Terminal Access Controller Access Control System
  - an old authentication protocol that was used on UNIX networks to allow a remote server to forward login requests to authentication servers for access control purposes  
- TACACS+
  - released by Cisco as a response to RADIUS
  - Cisco believed that RADIUS could use some design alterations  