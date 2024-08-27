[https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers](https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers)

| Service                       | Transport Protocol                      | Port                                                    | Notes                                     |
| ----------------------------- | --------------------------------------- | ------------------------------------------------------- | ----------------------------------------- |
| [FTP](Protocols/FTP.md)       | TCP                                     | 21 (control) <br><br>20 (data)                          |                                           |
| SSH                           | TCP                                     | 22                                                      |                                           |
| [Telnet](Protocols/Telnet.md) | TCP                                     | 23                                                      |                                           |
| [SMTP](Protocols/SMTP.md)     | TCP                                     | 25 (relay) <br><br>587 (submission)                     |                                           |
| [WHOIS](Protocols/WHOIS.md)   | TCP                                     | 43                                                      |                                           |
| TACACS                        | TCP <br><br>UDP                         | 49 <br><br>49                                           | TCP or UDP                                |
| DNS                           | TCP <br><br>UDP                         | 53 <br><br>53                                           | TCP or UDP (see protocol for details)     |
| DHCP                          | UDP                                     | 67, 68                                                  |                                           |
| TFTP                          | UDP                                     | 69                                                      |                                           |
| [HTTP](Protocols/HTTP.md)     | TCP <br><br>TCP                         | 80 <br><br>443 (over TLS)                               |                                           |
| Kerberos                      | TCP                                     | 88                                                      |                                           |
| POP3                          | TCP                                     | 110 <br><br>995 (over TLS)                              | POP3S is POP over TLS ==> port 995        |
| RPC                           | TCP <br><br>UDP                         | 111 <br><br>111                                         |                                           |
| NTP                           | UDP                                     | 123                                                     |                                           |
| Microsoft RPC                 | TCP                                     | 135                                                     |                                           |
| NetBIOS                       | UDP <br><br>UDP <br><br>TCP             | 137 <br><br>138 <br><br>139                             |                                           |
| SMB                           | TCP                                     | 445                                                     | UDP when AD is in use?                    |
| IMAP                          | TCP                                     | 143                                                     |                                           |
| SNMP                          | UDP                                     | 161                                                     |                                           |
| BGP                           | TCP                                     | 179                                                     |                                           |
| AppleTalk                     | TCP                                     | 201                                                     |                                           |
| LDAP                          | TCP                                     | 389                                                     |                                           |
| ISAKMP                        | UDP                                     | 500                                                     |                                           |
| R-Services                    |                                         | 512,513,514                                             | TCP and UDP?                              |
| Syslog                        | UDP                                     | 514                                                     |                                           |
| RIP                           | UDP                                     | 520                                                     |                                           |
| DHCPv6                        | UDP                                     | 546 (client) <br><br>547 (server)                       |                                           |
| IPMI                          | UDP                                     | 623                                                     | Intelligent Platform Management Interface |
| Rsync                         | TCP                                     | 873                                                     | Management                                |
| VMWare ESXi                   | TCP <br><br>UDP                         | 902 <br><br>902                                         | TCP and UDP                               |
| SOCKS Proxy                   | TCP <br><br>UDP                         | 1080 <br><br>1080                                       | TCP and UDP                               |
| OpenVPN                       | TCP <br><br>UDP                         | 1194 <br><br>1194                                       | TCP and UDP                               |
| MSSQL                         | TCP <br><br>UDP <br><br>TCP             | 1433  <br><br>1434  <br><br>1434                        | TCP and UDP; see Microsoft docs           |
| Oracle DB                     | TCP                                     | 1521                                                    | Oracle TNS                                |
| NFS                           | TCP                                     | 2049                                                    |                                           |
| Squid Proxy                   | TCP                                     | 3128                                                    |                                           |
| MySQL                         | TCP                                     | 3306                                                    |                                           |
| RDP                           | TCP                                     | 3389                                                    |                                           |
| SIP                           | TCP <br><br>UDP <br><br>TCP <br><br>UDP | 5060 <br><br>5060 <br><br>5061 (TLS) <br><br>5061 (TLS) | TCP or UDP                                |
| XMPP                          | TCP                                     | 5222                                                    | Jabber                                    |
| PostgreSQL                    | TCP                                     | 5432                                                    |                                           |
| Nagios                        | TCP                                     | 5666 (NRPE)                                             |                                           |
| VNC                           | TCP                                     | 5900                                                    |                                           |
| WinRM                         | TCP                                     | 5985,5986                                               |                                           |
| X11                           | TCP                                     | 6000-63                                                 |                                           |
| IRC                           | TCP                                     | 6665-6669                                               | 6667 is common                            |
| Tor                           | TCP                                     | 9001                                                    |                                           |
| HSQL/HSQLDB                   | TCP                                     | 9001                                                    |                                           |
| Openfire                      | TCP                                     | 9090 (HTTP) <br><br>9091 (HTTPS)                        |                                           |
| JetDirect                     | TCP                                     | 9100                                                    |                                           |