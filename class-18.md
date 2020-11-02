# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-17) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-19)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

What is the benefit of transforming data into packets?
Data packets are able to find the destination without the use of a dedicated channel.
2. UDP is often refereed to as a connectionless protocol. Why is this?
there is no handshaking between sending and receiving segments.
3. Can a socket server application have multiple socket connections?
yes
4. Can a socket connection application be connected to multiple socket servers?
no, if a client needs to connect to multiple servers multiple socket instances should be created for each server.
5. Can an application be both a socket server and a socket connection?
yes

## Term

OSI Model: is a conceptual framework used to describe the functions of a networking system. consists of 7 layers (Layer 7 - Application.
Layer 6 - Presentation.
Layer 5 - Session.
Layer 4 – Transport.
Layer 3 - Network.
Layer 2 – Data Link.
Layer 1 - Physical.)  
TCP Model: is a concise version of the OSI model.consists of 4 layers corresponding to(Application, Transport, Network and Data link)  
TCP: (Transmission Control Protocol) is a standard that defines how to establish and maintain a network conversation through which application programs can exchange data  
UDP: (User Datagram Protocol) is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet.  
Packets: small segments of a larger message
Socket: one endpoint of a two-way communication link between two programs running on the network  

## Socket.io

Socket.IO is a library which enables real-time and full duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts, both WebSocket vs Socket.io are event-driven libraries
