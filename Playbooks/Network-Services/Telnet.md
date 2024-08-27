[Telnet Reference](../../Technical-Reference/Networking/Protocols/Telnet.md)

https://book.hacktricks.xyz/network-services-pentesting/pentesting-telnet

### Discovery
Commonly discovered on a port scan:

`$ sudo nmap -n -p 23 -sTV <ip_address>`

![Pasted image 20240327152146](../../_attachments/telnet_nmap.png)

Wireshark packet captures might also reveal telnet communication. Wireshark filter:

`tcp.port == 23`

### Enumeration
Commonly connected to with the telnet, netcat, ncat and other capable clients.

Banner grab with netcat:

`$ nc -nv <ip_address> 23`

![Pasted image 20240327152508](../../_attachments/ncat.png)

Additional enumeration can be performed by nmap:

`$ sudo nmap -n -p -sTV --script "*telnet* and safe" <ip_address>`

![Pasted image 20240327153104](../../_attachments/telnet_nmap2.png)

Metasploit also has some modules for telnet enumeration:

![Pasted image 20240327154131|1000](../../_attachments/metasploit_telnet_aux.png)

Example:

`msf> use auxiliary/scanner/telnet/telnet_version`
`msf> set RHOST <ip_address>`
`msf> run`

![Pasted image 20240327154337](../../_attachments/metasploit_telnet_version.png)

### Exploitation
- Sniff plaintext credentials or data over network traffic
- Weak credentials / credential guessing
- Credential brute force