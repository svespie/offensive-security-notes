[Internet protocol suite - Wikipedia](https://en.wikipedia.org/wiki/Internet_protocol_suite)

[Internet - Wikipedia](https://en.wikipedia.org/wiki/Internet)

A simpler model for modern network communication compared to the OSI Model. However, it is still just a model.

4 layers:


| Layer | Name              | Description                                                                                                                                                                                   |
| ----- | ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 4     | Application Layer | Incorporates layers 5,6,7 of OSI collectively as the stuff that happens once the data is received. Gives meaning to the transmitted/received data.<br><br>Examples: FTP, HTTP, SMTP           |
| 3     | Transport Layer   | Defines rules for communicating with other machines, regardless of what network they are on. The concept of a port and how to interact with ports are defined here.<br><br>Examples: TCP, UDP |
| 2     | Internet Layer    | Defines how communication is routed from network to network. Forms the backbone of the Internet. Introduces the idea of an IP address.<br><br>Examples: IP, IPsec, ICMP                       |
| 1     | Link Layer        | Defines how to communicate to the local network. Physical connections implementation is excluded, assuming agnostic implementations of various media.<br><br>Examples: ARP                    |

[Address Resolution Protocol - Wikipedia](https://en.wikipedia.org/wiki/Address_Resolution_Protocol)

