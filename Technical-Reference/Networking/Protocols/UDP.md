[User Datagram Protocol - Wikipedia](https://en.wikipedia.org/wiki/User_Datagram_Protocol)

Where TCP establishes a connection with the 3-way handshake, UDP is more of a broadcast where the message is simply sent to the destination and forgotten. There is no effort to establish a session, provide error handling, or even know if the receiver received the message.

TCP == phone conversation
UDP == shouting through a megaphone

TCP is slower due to more setup and teardown. UDP is faster but less reliable.