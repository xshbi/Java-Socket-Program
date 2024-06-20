# Java-Socket-Program
This is a basic program to show to connect the socket.



### Java Socket Programming Process

Java socket programming allows for the communication between two applications running on different Java Runtime Environments (JRE). This typically involves a client-server communication model where a server socket listens for incoming client connections and responds accordingly.

#### Key Components:
1. **Socket**: An endpoint of a two-way communication link between two programs running on the network [citation:2][citation:6].
2. **ServerSocket**: This class is used to create a server socket that waits for client requests and establishes a connection [citation:5][citation:8].

#### Connection-Oriented Socket Programming:
1. The **ServerSocket** listens on a specified port and waits for client connections using the `accept()` method.
2. The **Socket** object represents the client's endpoint and is created by the client program to connect to the server [citation:3][citation:7].

#### Communication Steps:
1. **Server Side**:
   - Create a **ServerSocket** and wait for connections.
   - Upon accepting a connection, a **Socket** object is created to handle communication with the client.
   - Use input and output streams to read and write data.
   - Close the socket once the communication is complete.
   
2. **Client Side**:
   - Create a **Socket** to connect to the server.
   - Use input and output streams to read and write data.
   - Close the socket once the communication is complete [citation:9][citation:10].

### Diagram

#### Server-Client Communication Flow:
```
Client       Server
  |             |
  |   Socket    |
  |------------>|
  |             |
  |   .accept() |
  |<------------|
  |             |
  | Input/Output |
  |------------->|
  |<-------------|
  |             |
  |  .close()   |
  |------------>|
```



