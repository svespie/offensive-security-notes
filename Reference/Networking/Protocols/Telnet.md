[Telnet - Wikipedia](https://en.wikipedia.org/wiki/Telnet)

https://datatracker.ietf.org/doc/html/rfc854

"teletype network"

Default Port: TCP 23

Provides a command line interface to a remote host. Connects via plaintext but otherwise similar to SSH, which replaced it.

Common config files:

/etc/inetd.conf
/etc/xinetd.d/telnet
/etc/xinetd.d/stelnet

There is also a telnet client. Basic syntax:

`$ telnet <ip> <optional:port>`

![Pasted image 20240327151515](../../../_attachments/Pasted%20image%2020240327151515.png)