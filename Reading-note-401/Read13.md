# Message Queues

### Review, Research, and Discussion

1. What does it mean that web sockets are bidirectional? Why is this useful?
- means you can send and recieve data from client to server and from server to the client.
2. Does socket.io use HTTP? Why?
- yes 
3. What happens when a client emits an event?
- will run the event in server that was listinig for this event.
4. What happens when a server emits an event?
- will run the event in the client that was listinig for this event.
5. What happens if a client “misses” an event?
- he will not see any thing 
6. How can we mitigate this?
- using queues 



### Document the following Vocabulary Terms

**Socket**
-  allow communication between two different processes on the same or different machines

**Web Socket**
- Web Socket is a protocol that provides full-duplex(multiway) communication i.e allows communication in both directions simultaneously

**Socket.io**
- Socket.IO is a library that enables real-time, bidirectional and event-based communication between the browser and the server
![](https://socket.io/images/bidirectional-communication.png)

**Client**
- its the browser or any one req data from server 

**Server**
- the one how reseve the req from client and response for this req 

**OSI Model**
- The open systems interconnection OSI provides a standard for different computer systems to be able to communicate with each other.

**TCP Model**
-  TCP stands for Transmission Control Protocol a communications standard that enables application programs and computing devices to exchange messages over a network.

**TCP**
- TCP/IP stands for Transmission Control Protocol/Internet Protocol. TCP/IP is a set of standardized rules that allow computers to communicate on a network such as the internet.

**UDP**
- User Datagram Protocol (UDP) a communications protocol that facilitates the exchange of messages between computing devices in a network. It’s an alternative to the transmission control protocol (TCP). In a network that uses the Internet Protocol (IP), it is sometimes referred to as UDP/IP.

**Packets**
- They are the basic units of information transfer over a network, as each information being sent off by a sender is broken down into small structures to enable easy and quick transmission over network links. Without these fragmentations, it will be a lot harder to move big chunks of information across a network.