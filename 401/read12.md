# Socket.io

## Review, Research, and Discussion

1. **What is the benefit of transforming data into packets?**

    Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data, sending smaller packets helps ensure each section is transmitted successfully. If a packet is not received or is “dropped,” only the dropped packet needs to be reset.

2. **UDP is often refereed to as a connectionless protocol. Why is this?**

    UDP does not have a mechanism to make sure that the payload is not corrupted. As a result, the application must take care of data integrity all by itself. source (Links to an external site.). UDP is commonly used for applications that are lossy (can handle some packet loss), such as streaming audio and video. It is also used for query-response applications, such as DNS queries.

3. **Can a socket server application have multiple socket connections?**

    The server can handle 65,536 sockets per single IP address. So the quantity can be easily extended by adding additional network interfaces to a server. Meanwhile, it’s extremely important to track how many connections present on a server.

4. **Can a socket connection application be connected to multiple socket servers?**

    Yes, each listening (bound) port is serviced by a separate socket (as are all the connections made from each listening port)

5. **Can an application be both a socket server and a socket connection?**

    Yes, it can.

## Document the following Vocabulary Terms

- **Observer Pattern** is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.

- **Listener** is a function in a computer program that waits for an event to occur.

- **Event Handler** scripts that are automatically executed when an event occurs.

- **Event Driven Programming** is when a program is designed to respond to user engagement in various forms. It is known as a programming paradigm in which the flow of program execution is determined by “events.” Events are any user interaction, such as a click or key press, in response to prompt from the system.

- **Event Loop** is a construct that allows JavaScript and Node.js to perform non-blocking operations, it handles the synchronous script on a single thread, while leaving async code to be handled separately off the single thread, then adds it back to the call stack once it returns giving the impression of a multi-threaded language. Or, async code can be awaited, giving it the impression of synchronous code.

- **Event Queue** is a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system.

- **Call Stack** is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function.

- **Emit/Raise/Trigger** is firing the event.

- **Subscribe** is enrolling in a service or agreeing to receive continuous info from a publisher, the user should input their emails or some credentials to become subscribed.

- **database** is an organized collection of data, generally stored and accessed electronically from a computer system.

## Preparation Materials

### OSI Model Explained

Learn computer network layers or OSI layers in a computer network, OSI Model, OSI reference model or open system interconnection model or networking model including Application Layer, Presentation Layer, Session Layer, Transport Layer, Network Layer, Data Link Layer and Physical layer. Definition, Function, and use of the OSI network model. Protocols in computer network layers of OSI model.

OSI Model defines and is used to understand – How data is transferred from one computer to another in a computer network?

In the most basic form, two computers (end-points) connected to each other with LAN Cable (Network Media) and connectors (RJ45) sharing data with the help of NICs forms a network.

But if one computer is based on Microsoft Windows and the other one has MAC OS installed, then how these two computers are going to communicate with each other?

In order to accomplish successful communication b/w computers or networks of different architectures, 7-layered OSI Model or Open System Interconnection Model was introduced by the International Organization for Standardization in 1984.

### TCP - Three-way handshake in details

TCP stands for transmission control protocol. TCP is a reliable and connection-oriented transport protocol. With TCP, data can be delivered successfully and accurately.

Many applications, such as web,  email, and FTP, use TCP. Before TCP transmits data, it will use three-way handshake to establish a connection.

### WebSocket

**WebSocket** is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C.

WebSocket is distinct from HTTP. Both protocols are located at layer 7 in the OSI model and depend on TCP at layer 4. Although they are different, RFC 6455 states that WebSocket "is designed to work over HTTP ports 443 and 80 as well as to support HTTP proxies and intermediaries," thus making it compatible with HTTP. To achieve compatibility, the WebSocket handshake uses the HTTP Upgrade header to change from the HTTP protocol to the WebSocket protocol.

The WebSocket protocol enables interaction between a web browser (or other client application) and a web server with lower overhead than half-duplex alternatives such as HTTP polling, facilitating real-time data transfer from and to the server. This is made possible by providing a standardized way for the server to send content to the client without being first requested by the client, and allowing messages to be passed back and forth while keeping the connection open. In this way, a two-way ongoing conversation can take place between the client and the server. The communications are usually done over TCP port number 443 (or 80 in the case of unsecured connections), which is beneficial for environments that block non-web Internet connections using a firewall. Similar two-way browser-server communications have been achieved in non-standardized ways using stopgap technologies such as Comet.

### WebSocket vs Socket.io

**WebSocket** is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

**Socket.IO** is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.
