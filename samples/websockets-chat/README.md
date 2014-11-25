ESP WebSockets Chat Sample
===

This sample shows how to create a chat server using WebSockets and ESP. This 
application echos incoming packets back to all clients. The application source 
is in chat.c. This is a simple ESP controler with one action that is run in 
response to the URI: 

    /ws/test/chat

The HTML page web/index.html is served to the client browser to issue a web socket
request.

The server is configured to keep the web socket open for 10 minutes of inactivity and
then close the connection.

Requirements
---

* [Appweb](https://embedthis.com/appweb/download.html)
* [MakeMe Build Tool](https://embedthis.com/me/download.html)

To build:
---
    me 

To run:
---
    me run

The server listens on port 8080. Browse to: 
 
     http://localhost:8080/

This opens a web socket and sends any messages entered into the text field to all clients.

Code:
---
* [cache](cache) - Directory for compiled ESP modules
* [appweb.conf](appweb.conf) - Appweb server configuration file
* [chat.c](chat.c) - WebSockets chat server code
* [start.me](start.me) - MakeMe build instructions
* [web](web) - Directory containing the index.html web page

Documentation:
---
* [Appweb Documentation](https://embedthis.com/appweb/doc/index.html)
* [ESP Directives](https://embedthis.com/appweb/doc/users/dir/esp.html)
* [ESP Tour](https://embedthis.com/esp/doc/start/tour.html)
* [ESP Controllers](https://embedthis.com/esp/doc/users/controllers.html)
* [ESP APIs](https://embedthis.com/esp/doc/ref/native.html)
* [ESP Guide](https://embedthis.com/esp/doc/users/index.html)
* [ESP Overview](https://embedthis.com/esp/doc/index.html)

See Also:
---
* [esp-angular-mvc - ESP Angular MVC Application](../esp-angular-mvc/README.md)
* [esp-controller - Serving ESP controllers](../esp-controller/README.md)
* [esp-html-mvc - ESP MVC Application](../esp-html-mvc/README.md)
* [esp-page - Serving ESP pages](../esp-page/README.md)
* [secure-server - Secure server](../secure-server/README.md)
* [simple-server - Simple server and embedding API](../simple-server/README.md)
* [typical-server - Fully featured server and embedding API](../typical-server/README.md)
* [websockets-echo - WebSockets echo server](../websockets-echo/README.md)