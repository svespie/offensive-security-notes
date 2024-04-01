Tools like Burp Suite can capture and intercept WebSocket traffic. The proxy tool includes a WebSockets tab.

![](attachments/Pasted%20image%2020240401151632.png)

The WebSocket proxy settings:

![](attachments/Pasted%20image%2020240401151540.png)

Once intercepted, it is possible to manipulate and replay WebSocket traffic in the same way as HTTP traffic (depending on the data format in the intercepted messages).

Messages can be manipulated to conceivably execute traditional web application attacks such as XSS, SQL injection, command injection, etc.

XSS example:

![](attachments/Pasted%20image%2020240401154225.png)

[Working with WebSocket messages in Burp Repeater - PortSwigger](https://portswigger.net/burp/documentation/desktop/tools/repeater/websocket-messages)
