# Message Queues

- [Home](https://fadnesscharlie.github.io/reading-notes/401/)

## Review, Research, and Discussion

1. What does it mean that web sockets are bidirectional? Why is this useful?
   - This means that when one party is making a request, it does not need the other party to pair it with another request, making it accept or recieve request whenever it is needed without a response
2. Does socket.io use HTTP? Why?
   - Yes because it depends on HTTP to its initial connection
3. What happens when a client emits an event?
   - The emitted event will trigger the events connected to it whether it be in the back end or front end
4. What happens when a server emits an event?
   - The emitted event will trigger the events connected to it whether it be in the back end or front end
5. What happens if a client “misses” an event?
   - It will ignore it
6. How can we mitigate this?
   - Adding in a try catch or error handling

## Document the following Vocabulary Terms

- Socket
  - An event that works with socket.io to create listeners
- Web Socket
  - A communication protocol which provides a full-duplex and low-latency channel between the server and the browser.
- Socket.io
  - A library that enables real-time, bidirectional and event-based communication between the browser and the server.
- Client
  - Loads the browser side of socket.io-client
- Server
  - Integrates with the Node.JS HTTP Server Socket.io
- OSI Model
  - Open Systems Interconnection Model is a reference model that describes how information from a software application in one computer moves through a physical medium to the software application in another computer [ref](https://www.javatpoint.com/osi-model)
- TCP Model
  - it is a communication standard that exchanges messages over a network and will ensure delivery
- TCP
  - Transfer Control Protocol
- UDP
  - User Datagram Protocol
    - a communication standard that exchanges data by sending data faster as they do not need confirmation of the packets being sent
- Packets
  - Smaller forms of data that has been split from a bigger chunk

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   - TCP
   - Sockets
   - Server/client
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   - Error handling in event transmission
   - More on TCP and UDP
   - More use case for sockets
3. What are you most excited about trying to implement or see how it works?
   - Sockets

## Resources

- [Socket.io Chat Example](https://socket.io/get-started/chat/)
- [Rooms and Namespaces](https://socket.io/docs/rooms-and-namespaces/)
- [Socket.io Emit Cheatsheet](https://socket.io/docs/emit-cheatsheet/)

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
