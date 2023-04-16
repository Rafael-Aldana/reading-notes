# Socket.io

## Web Sockets

What is a Web Socket?

A webSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

Describe the Web Socket request/response handshake and what happens once the connection is established.

WebSockets are a bi-directional, full-duplex communication protocol that allow real-time, low-latency communication between a web browser and a server. The WebSockets protocol is built on top of HTTP and uses a WebSocket handshake to establish a connection between the client and the server.

Here is an overview of the WebSocket handshake process:

The client sends an HTTP request to the server with an "Upgrade" header field and a "Connection" header field with the value "Upgrade", indicating that it wants to upgrade the connection to a WebSocket connection.
The client includes a "Sec-WebSocket-Key" header field with a random string that is used in the response to prevent certain types of attacks.
The server responds with an HTTP response with a "101 Switching Protocols" status code and the "Upgrade" and "Connection" headers set to "WebSocket".
The server includes a "Sec-WebSocket-Accept" header field with a value that is computed from the client's "Sec-WebSocket-Key" header and a predefined string. This helps verify that the handshake was not tampered with.
Once the handshake is complete, the connection is upgraded to a WebSocket connection and both the client and server can send messages to each other at any time.
Once the WebSocket connection is established, the client and server can send messages to each other in real-time without the overhead of HTTP requests and responses. Both the client and server can initiate messages, and the messages are sent as frames over the WebSocket connection. The frames can be either binary or text data and can be fragmented across multiple frames if necessary.

WebSocket connections are especially useful for real-time applications such as chat applications, online gaming, or any application where real-time updates are important. The WebSocket protocol is supported by most modern browsers and can be used with any server-side technology that supports WebSockets, such as Node.js.

Web Sockets provide a standardized way for the server to send content to a client without first receiving a ____ from that client.

The WebSocket protocol enables interaction between a web browser (or other client application) and a web server with lower overhead than half-duplex alternatives such as HTTP polling, facilitating real-time data transfer from and to the server. This is made possible by providing a standardized way for the server to send content to the client without being first requested by the client, and allowing messages to be passed back and forth while keeping the connection open. In this way, a two-way ongoing conversation can take place between the client and the server. The communications are usually done over TCP port number 443 (or 80 in the case of unsecured connections), which is beneficial for environments that block non-web Internet connections using a firewall. Similar two-way browser–server communications have been achieved in non-standardized ways using stopgap technologies such as Comet or Adobe Flash Player.

## Socket.io Tutorial

What does the event handler io.on() do?

io.on() is an event listener that enables the server to handle incoming events from clients in Socket.IO.

Describe some possible proof of life or proof that the code works as expected

In the context of Socket.IO, a "proof of life" can refer to a way to verify that a client is still connected to the server and sending/receiving data. One way to achieve this is to use the socket.io-client library on the client-side to periodically send a "heartbeat" message to the server, which the server can then use to confirm that the client is still connected and responsive.

What does socket.emit() do?

socket.emit() is a method that is used to emit an event to the client or clients that are connected to the server. When you call socket.emit(), you specify the name of the event as the first argument, and any data you want to send as the second argument.

## Socket.io vs Web Sockets

What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).

WebSocket is a protocol for low-latency, bidirectional communication between a client and server, while Socket.IO is a library that builds on top of WebSocket (and other transports) to provide real-time, event-based communication with additional features. It's similar to the relationship between Git and GitHub, where Git is a version control system and GitHub is a platform for hosting Git repositories and providing additional features.

When would you use Socket.IO?

Socket.IO is a great choice when you need to build real-time, event-based applications that require bi-directional communication between a client and a server. It's particularly useful when you need to build chat applications, multiplayer games, collaborative document editing tools, or any other application that requires real-time updates.

Some specific use cases for Socket.IO include:

Real-time messaging applications: Socket.IO makes it easy to build chat applications that allow users to send and receive messages in real-time.

Multiplayer games: Socket.IO provides a way to build real-time multiplayer games that allow players to interact with each other in real-time.

Collaborative editing tools: Socket.IO can be used to build collaborative editing tools that allow multiple users to edit a document or file in real-time.

Real-time analytics: Socket.IO can be used to build real-time analytics tools that allow you to track user behavior on your website or application in real-time.

In general, Socket.IO is a good choice when you need to build applications that require real-time updates and bidirectional communication between a client and server.

When would you use WebSockets?

WebSockets are a good choice when you need to build real-time, event-driven applications that require low latency and high performance. They are particularly useful when you need to build applications that require bi-directional communication between a client and a server, but don't require the additional features and complexity of Socket.IO.

Some specific use cases for WebSockets include:

Real-time stock market updates: WebSockets can be used to provide real-time stock market updates to traders and investors.

Real-time sports scores: WebSockets can be used to provide real-time scores and updates for sports games.

Real-time collaboration tools: WebSockets can be used to build real-time collaboration tools, such as whiteboards or project management tools.

Real-time monitoring and dashboards: WebSockets can be used to build real-time monitoring and dashboards, such as server monitoring tools or website analytics dashboards.

In general, WebSockets are a good choice when you need to build real-time applications that require low latency and high performance, and don't require the additional features and complexity of Socket.IO.

## OSI Model Explained

What are a couple of key takeaways from this video?

The OSI Model (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.
Other key take aways from this video are that the OSI model is divided into seven layers and they are:

  1. Physical Layer
  2. Data Link Layer
  3. Network Layer
  4. Transport Layer
  5. Session Layer
  6. Presentation Layer
  7. Application Layer

## TCP Handshakes Explained

Translate the gist of this video to a non-technical friend

TCP uses a three-way handshake to establish a reliable connection. The connection is full duplex, and both sides synchronize (SYN) and acknowledge (ACK) each other. The exchange of these four flags is performed in three steps—SYN, SYN-ACK, and ACK

[link-to-reading-notes](https://en.wikipedia.org/wiki/WebSocket).
[link-to-reading-notes](https://www.tutorialspoint.com/socket.io/).
[link-to-reading-notes](https://www.educba.com/websocket-vs-socket-io/).
[link-to-reading-notes](https://www.youtube.com/watch?v=vv4y_uOneC0).
[link-to-reading-notes](https://www.youtube.com/watch?v=xMtP5ZB3wSk).

## Bookmark and Review

[link-to-reading-notes](https://socket.io/docs/).
[link-to-reading-notes](https://socket.io/docs/server-api).
[link-to-reading-notes](https://socket.io/docs/client-api).
[link-to-reading-notes](https://amritb.github.io/socketio-client-tool/).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?