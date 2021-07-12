# Message Queues

## Review, Research, and Discussion

1- **What does it mean that web sockets are bidirectional? Why is this useful?**

  Bidirectional means that it works both ways, meaning that both parties can send and receive at the same time.

2- **Does socket.io use HTTP? Why?**

  Yes , to allow HTTP and websocket servers to co-exist on the same TCP port.

3- **What happens when a client emits an event?**

  Execuiting the event handler.

4- **What happens when a server emits an event?**

  All listening clients will execute the handler for that event.

5- **What happens if a client “misses” an event?**

  The handler woudln’t be executed.

6- **How can we mitigate this?**

  Using messaging queueing.

## Document the following Vocabulary Terms

- **Socket** is a software structure within a network node of a computer network that serves as an endpoint for sending and receiving data across the network.

- **Web Socket** is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

- **Socket.io** is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers. It has two parts: a client-side library that runs in the browser, and a server-side library for Node.js. Both components have a nearly identical API.

- **Client** is a piece of computer hardware or software that accesses a service made available by a server as part of the client–server model of computer networks. The server is often (but not always) on another computer system, in which case the client accesses the service by way of a network.

- **Server** is a piece of computer hardware or software that provides functionality for other programs or devices, called “clients”.

- **OSI Model** is a conceptual model that characterises and standardises the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology.

- **TCP Model** is the conceptual model and set of communications protocols used in the Internet and similar computer networks. It is commonly known as TCP/IP because the foundational protocols in the suite are the Transmission Control Protocol and the Internet Protocol.

- **TCP** is one of the main protocols of the Internet protocol suite. It originated in the initial network implementation in which it complemented the Internet Protocol.

- **UDP** is one of the core members of the Internet protocol suite. With UDP, computer applications can send messages, in this case referred to as datagrams, to other hosts on an Internet Protocol network.

- **Packets** is a formatted unit of data carried by a packet-switched network. A packet consists of control information and user data; the latter is also known as the payload.

### Socket.io Chat Example

  Writing a chat application with popular web applications stacks like LAMP (PHP) has normally been very hard. It involves polling the server for changes, keeping track of timestamps, and it’s a lot slower than it should be.

  Sockets have traditionally been the solution around which most real-time chat systems are architected, providing a bi-directional communication channel between a client and a server.

  This means that the server can push messages to clients. Whenever you write a chat message, the idea is that the server will get it and push it to all other connected clients.

### Rooms and Namespaces

  Rooms are subdivisions of namespaces that can be created by the server. This allows you to broadcast data to a subset of related sockets. Two useful methods are provided for joining and leaving rooms, .join(room, callback) and .leave(room, callback) respectively. Both take two parameters, the room name and a callback.

  A namespace is basically a route defined on your API (/games) and upon connection, the request has to be sent to the specific namespace route let’s say the server is running on our localhost and we want to join the games namespace so we simply request a socket io connection to (http://localhost:3000/games) and thus all the connected sockets to one namespace would can reach sockets on the same namespace but can’t talk with other namespace’s socket..

### Emit cheatsheet

  Cheatsheet.
