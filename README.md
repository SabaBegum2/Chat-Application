# Multi-Threaded Chat Application

## Overview  
This project implements a **multi-threaded chat server and client system** in Java, enabling real-time communication between multiple users. The project focuses on efficient server performance, secure user management, and robust message broadcasting, designed with modular code for scalability and maintainability.  

## File Descriptions  
- **ChatServer.java**  
  The main server application that handles incoming client connections, manages active user sessions, and facilitates message broadcasting.  

- **ChatClient.java**  
  The client-side application allowing users to connect to the chat server, send messages, and receive updates in real-time.  

- **ReadThread.java**  
  A thread running on the client side to listen for and display incoming messages from the server.  

- **WriteThread.java**  
  A thread running on the client side to capture and send user messages to the server.  

- **UserThread.java**  
  A server-side thread assigned to each connected client, managing individual user interactions and communication with the server.  

## Features  
- **Server Performance**  
  - Multi-threaded architecture to handle concurrent users efficiently.  
  - Uses data structures for fast message delivery.  

- **User Management**  
  - Tracks active and inactive users.  
  - Stores and validates user credentials securely.  
  - Ensures data persistence across server restarts.  

- **Real-Time Communication**  
  - Message broadcasting to all connected clients.  
  - Entry notifications for newly joined users.  

- **Logging and Notifications**  
  - Automatic session logging with chat history.  
  - Notification system for user join events.  

## Setup  

1. **Clone the Repository**  
   ```bash  
   git clone https://github.com/SabaBegum2/chat-application.git  
   cd chat-application  
2. **Run the Server**
   Start the server to handle incoming client connections. In your terminal, run:
   ```bash
   java ChatServer
3. **Run the Client**
   To connect  to the server, run the client program. Open a new terminal window and run:
   ```bash
   java ChatClient
  You can run multiple instances of ChatClient in different terminal windows or on different devices to simulate multiple users.

## Usage
### Start the ChatServer
Begin by running the server to accept incoming client connections.

### Run ChatClient
Open multiple terminals or run the client on different devices to simulate multiple users. Each client can send and receive messages in real-time through the chat interface.

### Send and Receive Messages
Messages are broadcast to all connected clients. Users will receive notifications when a new user joins the chat, and detailed session logs are automatically recorded.

## Future Enhancement
- Private Messaging: Implement functionality for private one-on-one messaging between users.
- File Transfer Capabilities: Add the ability to send and receive files in real-time during chats.
- Message Encryption: Improve security by adding encryption to protect messages exchanged between clients and the server.
