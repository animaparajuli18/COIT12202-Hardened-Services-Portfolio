# Password Security and Hashing

## Overview
This activity investigated password security using different password hashing algorithms. I generated password hashes using MD5crypt, SHA512crypt and yescrypt, configured password quality controls using PAM, tested account lockout protection, and compared password cracking results using John the Ripper.

## Tasks Completed
- Generated password hashes using MD5crypt, SHA512crypt and yescrypt.
- Created test users with different password hashing algorithms.
- Examined password hash entries stored in `/etc/shadow`.
- Configured PAM password quality requirements.
- Tested rejection of weak passwords.
- Tested repeated failed login attempts and account lockout.
- Used John the Ripper to test the resistance of different password hashes.
- Compared the cracking results of MD5crypt, SHA512crypt and yescrypt.

## Evidence

### 1. Password Hash Generation
This screenshot shows password hashes being generated using MD5crypt, SHA512crypt and yescrypt. It demonstrates the different hash formats produced by each password hashing algorithm.
<img width="916" height="407" alt="Screenshot 2026-08-14 145941" src="https://github.com/user-attachments/assets/83fffe03-0dd1-4f9c-8c68-a3e76e779476" />


### 2. Password Hashes Stored in /etc/shadow
This screenshot shows the test accounts using MD5crypt, SHA512crypt and yescrypt hashes in `/etc/shadow`. The different prefixes demonstrate that different hashing methods were applied to the accounts.<img width="967" height="640" alt="Screenshot 2026-08-14 150049" src="https://github.com/user-attachments/assets/db9ab348-7876-4dcf-b3da-776b2ff0cc55" />


### 3. PAM Password Quality Enforcement
This screenshot demonstrates the password quality policy rejecting a weak password. The `BAD PASSWORD` messages show that the configured PAM controls detected that the password did not satisfy the required complexity rules.
<img width="985" height="487" alt="Screenshot 2026-08-14 150558" src="https://github.com/user-attachments/assets/2a7128ef-ba97-46be-a922-f57050336f70" />

### 4. Failed Login and Account Lockout Evidence
This screenshot shows repeated unsuccessful login attempts followed by the `faillock` output. The recorded failures demonstrate the account lockout protection used to respond to repeated authentication failures.<img width="888" height="455" alt="Screenshot 2026-08-14 151555" src="https://github.com/user-attachments/assets/30fadc38-c2bd-4357-8560-12896538ab37" />

### 5. MD5crypt Password Cracking
This screenshot shows John the Ripper successfully cracking the MD5crypt password hash using the RockYou wordlist. The recovered password demonstrates the weakness of a guessable password when combined with an older password hashing method.
 <img width="913" height="382" alt="Screenshot 2026-08-14 152311" src="https://github.com/user-attachments/assets/b3edc21c-b892-4517-be80-a50a8e7122bc" />


### 6. SHA512crypt Password Cracking
This screenshot shows John the Ripper successfully recovering the password protected with SHA512crypt and displays the cracking result and execution time.<img width="1066" height="332" alt="Screenshot 2026-08-14 152448" src="https://github.com/user-attachments/assets/d220dbc0-a128-45db-8380-d7ac9a4db205" />


### 7. Yescrypt Password Cracking
This screenshot shows John the Ripper successfully recovering the yescrypt password and the time required for the cracking process. This result can be compared with the other hashing algorithms to demonstrate differences in password-cracking performance.
<img width="915" height="290" alt="Screenshot 2026-08-14 152618" src="https://github.com/user-attachments/assets/b7c49972-d929-4c98-be73-2d0cd9fa1377" />

## Conclusion
This activity demonstrated how password hashing algorithms, password quality policies and account lockout controls contribute to password security. The cracking tests also showed that password strength and the choice of hashing algorithm both affect resistance to password-cracking attacks.
