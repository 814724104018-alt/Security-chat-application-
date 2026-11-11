SECURE CHAT APPLICATION (JAVA)

Aim:
To create a simple client-server chat application using Java TCP sockets
and AES-GCM encryption for message confidentiality and integrity.

Requirements:
- JDK 8 or later
- Two terminal windows on the same computer

How to run:
1. Open this folder in a terminal.
2. Compile:
   javac ChatCrypto.java Server.java Client.java
3. In Terminal 1, start the server:
   java Server
4. In Terminal 2, start the client:
   java Client
5. Type messages in either terminal. Type exit to stop that side.

Sample output:
SERVER:
Secure Chat Server started...
Waiting for client...
Client connected.
Type messages (type exit to stop).
You: Hello
Client: Hi, secure chat!
You: exit

CLIENT:
Connected to Secure Chat Server.
Type messages (type exit to stop).
You: Hi, secure chat!
Server: Hello
You: exit

Notes:
- The chat encrypts each message using AES-GCM before sending it over TCP.
- Both demo programs use the same sample key so they can communicate.
- This is an educational lab demonstration, not production-ready security.
  A real application needs authenticated key exchange, secure key storage,
  user authentication, certificate validation, and additional protections.
