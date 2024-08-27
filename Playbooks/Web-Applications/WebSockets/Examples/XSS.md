This example comes from PortSwigger Academy.

[Lab: Manipulating WebSocket messages to exploit vulnerabilities | Web Security Academy (portswigger.net)](https://portswigger.net/web-security/websockets/lab-manipulating-messages-to-exploit-vulnerabilities)

![](../../../../_attachments/screenshot_20240401155155.png)

There's a live chat feature which appears to be fairly interactive. This is a common use case for web sockets due to the ability to poll, etc.

![](../../../../_attachments/screenshot_20240401160058.png)

In fact, we can see the connection playing "ping pong":

![](../../../../_attachments/screenshot_20240401160229.png)

We can see the user message being submitted.

![](../../../../_attachments/screenshot_20240401170534.png)

If the other side of the chat is also being rendered in a browser, then it may be possible to submit an XSS attack if the input is not properly sanitized.

The objective is to cause an alert():

![](../../../../_attachments/screenshot_20240401170705.png)

We can see that the payload is replayed back to the client, causing an alert().


Here is the official solution which took a slightly different route:

![](../../../../_attachments/screenshot_20240401170824.png)

[Manipulating WebSocket messages to exploit vulnerabilities (Video solution) (youtube.com)](https://www.youtube.com/watch?v=63jRvCUkTEc)
