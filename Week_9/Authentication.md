# Authentication
## What is it?
A process or action of proving or showing something to be genuine or valid

## Fundamentals of Authentication
- something you know (password)
- something you have (usb)
- something you are (fingerprint)

- passwords (form of a string of letters, numbers and special characters)
    - most common form of authentication
    - not that good for todays (2021) security (not enough protection)
    - using anything bar a random password is weak    
        - **good traits:**
            - The longer the password, the more difficult it is to crack
            - variety
        - **bad traits:**
            - using a word from a dictionary
            - using personal information
            - using patterns/ variations of a password
            - using character substitutions
            - only putting numbers and special characters at the name
            - using common passwords
    - **Attacks**
        - brute force
        - dictionary attack
        - rainbow table attack (db thats used by tracking the password hash)
    - **Defences**
        - SALT techniques (adds random word to the end of the password (changes the hash))
        - Key stretching
      
## Token Authentication
- token can be hardware or software
- a material device that is used to access secure systems
- common forms include a dongle, card, RFID chip, USB
- a token makes it more difficult for a hacker to access an account since they must have long credentials and a tangible device itself, which is much harder for the hacker to obtain

## Biometric Authentication
- Key advantages:
    - Can be easily compared to authorised features saved in a database
    - Can control physical access when installed on entrances and doors
    - Can be added into multi-factor authentication process
- common methods:
    - Facial recognition
    - Fingerprint scanner
    - Voice identification
    - eye scanners
## Certificate-based Authentication
- Certificate-based authentication technologies identity users, machines or devices by using digital certificates
- A digital certificate is an electronic document based on the idea of a driver's license or a passport
- The certificate contains the digital identity of a user including a public key, and the digital signature of a certification authority
- Digital certificates prove the ownership of a public key and issued only by a certification authority
## Multi-factor Authentication
- multi-factor authentication (MFA) is an authentication method that requires two or more independent ways to identify a user
- example:
    - codes generated from a user's smartphone
    - captcha tests
    - fingerprints
    - facial recognition
- MFA methods and technologies increase the confidence of users by adding multiple layers of security
- MFA maybe a good defence against most account hacks, but it has its own pitfalls. People may lose their phones or SIM cards and not be able to generate an authentication code
## Authentication Protocols
- NTLM ()
- KERBEROS ()
- PAP (Password Authentication Protocol)
- CHAP (challenge handshake authentication protocol)
- SSL (Secure Socket Layer)/ TLS (Transport Layer Security)