# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-18) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-26)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. What does it mean that web sockets are bidirectional? Why is this useful?
Have two directions for dataflow. which means it can send and receive data. this will also help with the tcp handshake to make sure data reaches the desired destination
2. Does socket.io use HTTP? Why?
it can be used since it was based on HTTP but usually TCP is used with socket.io
3. What happens when a client emits an event?
client asks the server for a tcp connection using web sockets. Once the client is connected to the server through websockets, socket.io can send events to the send through the connection.
4. What happens when a server emits an event?
5. What happens if a client “misses” an event?
ignored
6. How can we mitigate this?

## terms

Web Socket: computer communications protocol, providing full-duplex communication channels over a single TCP connection.
Socket.io: a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers.
Client: a piece of computer hardware or software that accesses a service made available by a server
Server:a piece of computer hardware or software that provides functionality for other programs or devices.
