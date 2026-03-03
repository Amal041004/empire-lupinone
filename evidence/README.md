Evidence – Empire: LupinOne Penetration Test

This folder contains structured screenshot evidence captured during the full penetration testing lifecycle of the Empire: LupinOne virtual machine.

All activities were conducted in a controlled lab environment for academic and learning purposes.

---

1. Reconnaissance Phase

| Step | Description | Screenshot |
|------|------------|------------|
| 01 | Network verification using ifconfig | 01-network-verification-ifconfig.png |
| 02 | Host discovery using Nmap sweep | 02-host-discovery-nmap-sweep.png |
| 03 | Service enumeration (-sC -sV scan) | 03-service-enumeration-nmap-sCv.png |

---

2. Web Enumeration Phase

| Step | Description | Screenshot |
|------|------------|------------|
| 04 | Initial web homepage | 04-web-homepage.png |
| 05 | robots.txt analysis | 05-robots-txt-analysis.png |
| 06 | Attempted hidden directory access | 06-hidden-directory-access.png |
| 07 | FFUF installation | 07-ffuf-installation.png |
| 08 | Discovery of secret directory | 08-ffuf-secret-directory-discovery.png |
| 09 | Accessing secret directory | 09-secret-directory-content.png |
| 10 | Discovery of mysecret.txt | 10-ffuf-mysecret-discovery.png |

---

3. Key Extraction & Cracking

| Step | Description | Screenshot |
|------|------------|------------|
| 11 | Encoded SSH key content | 11-mysecret-encoded-content.png |
| 12 | Base58 decoding in CyberChef | 12-base58-decoding-cyberchef.png |
| 13 | Saving SSH private key locally | 13-ssh-key-saved.png |
| 14 | SSH hash generation using ssh2john | 14-ssh2john-hash-generation.png |
| 15 | Password cracked using John | 15-john-password-cracked.png |

---

4. Initial Access

| Step | Description | Screenshot |
|------|------------|------------|
| 16 | Successful SSH login | 16-ssh-login-success & user-directory-listing.png |
| 17 | User flag retrieved | 17-user-flag.png |

---

5. Privilege Escalation (Horizontal)

| Step | Description | Screenshot |
|------|------------|------------|
| 18 | Sudo enumeration (icex64) | 18-sudo-enumeration-icex64.png |
| 19 | LinPEAS download | 19-linpeas-download.png |
| 20 | LinPEAS execution results | 20-linpeas-execution.png |


---

6. Privilege Escalation (Root)

| Step | Description | Screenshot |
|------|------------|------------|
| 21 | Root shell obtained | 21-root-shell-obtained.png |
| 22 | Root flag retrieved | 22-root-flag.png |

---

Final Status

User access achieved  
Horizontal privilege escalation successful   
Vertical privilege escalation successful  
Root flag captured  

---

**Author:** Amal Reji  
**Project:** Empire: LupinOne VulnHub Penetration Test  
**Environment:** Controlled Virtual Lab
