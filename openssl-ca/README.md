# OpenSSL Certificate Authority and HTTPS

## Overview
This activity focused on creating a Certificate Authority (CA), generating and signing certificates, configuring an HTTPS server, and verifying secure TLS communication in GNS3.

## Tasks Completed
- Created an Intermediate Certificate Authority.
- Generated a server private key and Certificate Signing Request (CSR).
- Signed the server certificate using the Intermediate CA.
- Created the CA certificate chain.
- Installed the server certificate and private key.
- Configured Nginx to use HTTPS.
- Verified that Nginx was listening on port 443.
- Tested TLS certificate verification.
- Successfully accessed the HTTPS server using the trusted Root CA.

## Evidence

### Intermediate CA Certificate Created
Created and signed the Intermediate CA certificate using the Root CA.

## Evidence

### Intermediate CA Certificate Created
Created and signed the Intermediate CA certificate using the Root CA.

<img width="922" height="307" alt="Screenshot 2026-08-14 141956" src="https://github.com/user-attachments/assets/99183dd7-29b5-4598-a769-8eb89002fe9f" />
 

### Server Certificate Signed by Intermediate CA
Generated the server CSR and successfully signed the server certificate for www.12311345.lab.
<img width="755" height="147" alt="Screenshot 2026-08-14 140901" src="https://github.com/user-attachments/assets/7f1094a8-f3a2-4821-9259-4c753407f3a4" />

### Server Certificate and CA Chain Created
Created the CA certificate chain and confirmed that the server certificate and CA chain files were generated.
<img width="1002" height="227" alt="Screenshot 2026-08-14 142503" src="https://github.com/user-attachments/assets/75c7c243-aa38-42f5-8250-4231ff7f0b75" />


### Server Private Key Installed
Transferred and installed the server private key in /etc/ssl/private/server.key.
 <img width="1357" height="321" alt="Screenshot 2026-08-14 142830" src="https://github.com/user-attachments/assets/4f956403-4eb4-4208-8d35-e6a2376a8bda" />

 
### Nginx HTTPS Configuration Verified
Tested the Nginx configuration successfully and confirmed that the HTTPS service was listening on port 443.
<img width="1412" height="956" alt="Screenshot 2026-08-14 142917" src="https://github.com/user-attachments/assets/5d72d62a-4e26-4bed-89c3-ed5d3b9627f6" />


### TLS Certificate Verification Successful
Verified the TLS connection successfully. The connection used TLSv1.3 and returned "Verify return code: 0 (ok)".
<img width="800" height="332" alt="Screenshot 2026-08-14 143016" src="https://github.com/user-attachments/assets/0f428bd3-7a35-4896-94bb-75a156080b7c" />



### HTTPS Server Successfully Accessed
Successfully accessed https://www.12311345.lab/ using the trusted Root CA certificate. The server returned "HTTPS Server 12311345".
 <img width="735" height="180" alt="Screenshot 2026-08-14 143206" src="https://github.com/user-attachments/assets/727e6227-2317-401f-a513-db8ddb3c0efc" />

