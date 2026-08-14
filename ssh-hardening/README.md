# SSH Hardening

## Overview
This activity focused on configuring and hardening an SSH service in GNS3. I configured SSH authentication, strengthened the SSH server configuration, tested account lockout protection using fail2ban, and tested secure SSH tunnelling.

## Tasks Completed
- Configured Ed25519 SSH keys.
- Configured SSH authentication.
- Hardened the SSH server configuration.
- Disabled root SSH login.
- Disabled password authentication.
- Restricted SSH access to the authorised user.
- Configured fail2ban protection.
- Tested failed SSH login attempts and confirmed blocking.
- Tested SSH tunnelling to an internal web server.

## Evidence
The screenshots in this folder show the configuration and testing completed during the SSH hardening activity.

### SSH tunnel success (Internal Server 12311345
<img width="1213" height="492" alt="Screenshot 2026-08-14 160506" src="https://github.com/user-attachments/assets/ed5b34da-1c38-4611-bf29-2376203bb8e6" />


### Fail2ban successfully banned 10.10.1.20
<img width="777" height="302" alt="Screenshot 2026-08-14 155837" src="https://github.com/user-attachments/assets/3dbe6373-147e-4580-a6e4-44c4dc41d5ed" />

### Student login works + root login denied
<img width="1103" height="686" alt="Screenshot 2026-08-14 155741" src="https://github.com/user-attachments/assets/f95a605f-3cfd-47f0-9114-b42aec416d40" />

### SSH CONFIGURATION
<img width="881" height="307" alt="Screenshot 2026-08-14 155423" src="https://github.com/user-attachments/assets/8350118c-63b4-4d0c-b172-ea4cb73cd9e5" />

### SSH KEY ADDED

<img width="975" height="275" alt="Screenshot 2026-08-14 154913" src="https://github.com/user-attachments/assets/f2632fe6-0bc8-41e5-abc5-4b5e5aa3c419" />
