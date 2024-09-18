#checklist 

In no particular order:

##### 1. Network Scanning and Enumeration
- Host Discovery:
  - **Tools:**
    - **Nmap**: Network discovery and host enumeration (`nmap -sn <target>`).
    - **Masscan**: Fast network port scanner.
    - **Ping** / **hping3**: ICMP and TCP-based host discovery.
- Port Scanning:
  - **Tools:**
    - **Nmap**: Comprehensive port scanning (`nmap -p- <target>`).
    - **Unicornscan**: High-speed port scanning.
    - **RustScan**: Fast, modern port scanner.
- Service Version Detection:
  - **Tools:**
    - **Nmap**: Service and version detection (`nmap -sV <target>`).
    - **Ncat** / **Netcat**: Banner grabbing to identify services manually.
- OS Fingerprinting:
  - **Tools:**
    - **Nmap**: OS detection (`nmap -O <target>`).
    - **Xprobe2**: Remote OS fingerprinting.
    - **p0f**: Passive OS fingerprinting (can be used actively for banner grabbing).
##### 2. Vulnerability Scanning
- Network Vulnerability Scanning:
  - **Tools:**
    - **Nessus**: Comprehensive network vulnerability scanner.
    - **OpenVAS**: Open-source vulnerability scanner.
    - **Nmap NSE**: Nmap scripting engine for vulnerability detection (`nmap --script vuln <target>`).
- Web Application Vulnerability Scanning:
  - **Tools:**
    - **OWASP ZAP**: Web application scanner.
    - **Nikto**: Web server scanner.
    - **Burp Suite**: Active scanning for web vulnerabilities.
- Specialized Scanning:
  - **Tools:**
    - **Wpscan**: WordPress vulnerability scanner.
    - **JoomScan**: Joomla vulnerability scanner.
    - **CMSmap**: Scan CMS for known vulnerabilities.
##### 3. Network and Service Enumeration
- SMB/Windows Enumeration:
  - **Tools:**
    - **Enum4linux**: Enumerate Windows and Samba systems.
    - **smbclient**: Access and enumerate SMB shares.
    - **rpcclient**: Interact with Windows RPC services.
- SNMP Enumeration:
  - **Tools:**
    - **snmpwalk**: Enumerate SNMP data (`snmpwalk -v2c -c public <target>`).
    - **onesixtyone**: SNMP enumeration and brute-forcing.
- LDAP Enumeration:
  - **Tools:**
    - **ldapsearch**: Query LDAP directories.
    - **ADExplorer**: GUI tool for exploring Active Directory.
- SSH Enumeration:
  - **Tools:**
    - **Nmap NSE**: SSH enumeration scripts (`nmap --script ssh* <target>`).
    - **ssh-audit**: SSH server auditing.
- HTTP Enumeration:
  - **Tools:**
    - **Gobuster** / **Dirbuster**: Directory and file brute-forcing.
    - **Nmap NSE**: HTTP enumeration scripts (`nmap --script http-* <target>`).
    - **whatweb**: Identify web technologies.
##### 4. Web Application Enumeration
- Directory and File Brute-Forcing:
  - **Tools:**
    - **Gobuster**: Directory and file brute-forcing (`gobuster dir -u <target> -w <wordlist>`).
    - **dirsearch**: Fast web path scanner.
- Subdomain Enumeration:
  - **Tools:**
    - **SubBrute**: DNS subdomain brute-forcing.
    - **Amass**: In-depth subdomain enumeration.
- Web Parameter Fuzzing:
  - **Tools:**
    - **Burp Suite**: Fuzz parameters with Intruder.
    - **ffuf**: Fuzz web applications (`ffuf -w <wordlist> -u <target>?param=FUZZ`).
##### 5. Credential and Password Attacks
- Password Brute-Forcing:
  - **Tools:**
    - **Hydra**: Network login brute-forcing (`hydra -L <userlist> -P <passlist> <target>`).
    - **Medusa**: Fast network logon cracker.
    - **Ncrack**: Network authentication cracker.
- Password Spraying:
  - **Tools:**
    - **CrackMapExec**: Perform password spraying on SMB.
    - **Metasploit**: Password spraying modules.
- Credential Dumping:
  - **Tools:**
    - **Mimikatz**: Extract passwords from memory (post-exploitation).
    - **SecretsDump**: Dump hashes from Windows machines.
##### 6. Wireless Network Enumeration
- Wireless Network Scanning:
  - **Tools:**
    - **Kismet**: Wireless network detection and intrusion detection.
    - **airodump-ng**: Capture wireless traffic and identify networks.
- Wireless Network Attacks:
  - **Tools:**
    - **aircrack-ng**: Crack WEP/WPA-PSK keys.
    - **Wifite**: Automated wireless attack tool.
##### 7. VoIP and Telephony Enumeration
- SIP and VoIP Enumeration:
  - **Tools:**
    - **Sipvicious**: Scan and enumerate SIP devices.
    - **Svmap**: Scan for SIP devices on a network.
- PBX/Voicemail Enumeration:
  - **Tools:**
    - **Amap**: Application identification scanner.
    - **VoIPong**: VoIP traffic sniffer.
##### 8. Database Enumeration
- Database Service Enumeration:
  - **Tools:**
    - **Nmap NSE**: Database enumeration scripts (`nmap --script=oracle-*`).
    - **Metasploit**: Database modules for MySQL, MSSQL, Oracle, etc.
- Database Brute-Forcing:
  - **Tools:**
    - **Hydra**: Brute-force login credentials (`hydra -l <username> -P <passwordlist> mysql://<target>`).
    - **SQLMap**: Automated SQL injection and database takeover.
##### 9. Active Directory Enumeration
- AD Enumeration:
  - **Tools:**
    - **BloodHound**: Visualize Active Directory relationships.
    - **ldapdomaindump**: Dump Active Directory information via LDAP.
    - **CrackMapExec**: Enumerate AD information.
- Kerberos Enumeration:
  - **Tools:**
    - **Kerbrute**: Enumerate users via Kerberos.
    - **GetUserSPNs**: Identify user accounts with SPNs (Service Principal Names).
##### 10. Cloud Service Enumeration
- AWS Enumeration:
  - **Tools:**
    - **AWS CLI**: Interact with AWS services.
    - **CloudMapper**: Visualize AWS infrastructure.
    - **ScoutSuite**: Security auditing tool for cloud services.
- Azure and GCP Enumeration:
  - **Tools:**
    - **Azucar**: Enumerate Azure services.
    - **GCPBucketBrute**: Brute-force Google Cloud Storage buckets.
##### 11. Physical Security Testing (If permitted)
- Physical Network Access:
  - **Tools:**
    - **Packet Capture**: Wireshark for network traffic analysis.
    - **USB Rubber Ducky**: Keystroke injection tool.
- RFID and NFC:
  - **Tools:**
    - **Proxmark3**: RFID card cloning and manipulation.
    - **ACR122U**: NFC reader for reading and emulating cards.