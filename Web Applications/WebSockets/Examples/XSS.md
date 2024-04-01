This example comes from PortSwigger Academy.

[Lab: Manipulating WebSocket messages to exploit vulnerabilities | Web Security Academy (portswigger.net)](https://portswigger.net/web-security/websockets/lab-manipulating-messages-to-exploit-vulnerabilities)

![](attachments/Pasted%20image%2020240401155155.png)

There's a live chat feature which appears to be fairly interactive. This is a common use case for web sockets due to the ability to poll, etc.

![](attachments/Pasted%20image%2020240401160058.png)

In fact, we can see the connection playing "ping pong":

![](attachments/Pasted%20image%2020240401160229.png)

We can see the user message being submitted.

![](attachments/Pasted%20image%2020240401170534.png)

If the other side of the chat is also being rendered in a browser, then it may be possible to submit an XSS attack if the input is not properly sanitized.

The objective is to cause an alert():

![](attachments/Pasted%20image%2020240401170705.png)

We can see that the payload is replayed back to the client, causing an alert().


Here is the official solution which took a slightly different route:

![](attachments/Pasted%20image%2020240401170824.png)

[Manipulating WebSocket messages to exploit vulnerabilities (Video solution) (youtube.com)](https://www.youtube.com/watch?v=63jRvCUkTEc)
