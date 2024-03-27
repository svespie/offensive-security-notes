[Reference](obsidian://open?vault=notes-offensive-security&file=Reference%2FNetworking%2FProtocols%2FTelnet)

https://book.hacktricks.xyz/network-services-pentesting/pentesting-telnet


#### Discovery
Commonly discovered on a port scan:

`$ sudo nmap -n -p 23 -sTV <ip_address>`

![[Pasted image 20240327152146.png]]


Wireshark packet captures might also reveal telnet communication. Wireshark filter:

`tcp.port == 23`

#### Enumeration
Commonly connected to with the telnet, netcat, ncat and other capable clients.

Banner grab with netcat:

`$ nc -nv <ip_address> 23`

![[Pasted image 20240327152508.png]]


Additional enumeration can be performed by nmap:

`$ sudo nmap -n -p -sTV --script "*telnet* and safe" <ip_address>`

![[Pasted image 20240327153104.png]]



Metasploit also has some modules for telnet enumeration:

![[Pasted image 20240327154131.png]]

Example:

`msf> use auxiliary/scanner/telnet/telnet_version`
`msf> set RHOST <ip_address>`
`msf> run`

![[Pasted image 20240327154337.png]]


#### Exploitation
- Sniff plaintext credentials or data over network traffic
- Weak credentials / credential guessing
- Credential brute force