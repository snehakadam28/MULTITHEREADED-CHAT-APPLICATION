# MULTITHEREADED-CHAT-APPLICATION

**COMPANY**: CODTECH IT SOLUTIONS

**NAME**: SNEHA VIJAY KADAM

**INTERN ID**: CT08JHS

**DOMAIN**: JAVA PROGRAMMING

**BATCH DURATION**: JANUARY 20TH, 2025 TO FEBRUARY 20TH, 2025

**MENTOR NAME**: NEELA SANTHOSH KUMAR

**Description of the code**:

1. Chat Server 

Overview

The ChatServer acts as the central hub that listens for incoming client connections and facilitates message broadcasting among connected clients.

Key Features

Listens on a fixed port (12345) for client connections.

Manages multiple clients using threads.

Broadcasts messages received from one client to all other connected clients.

Handles client disconnections gracefully by removing inactive clients from the list.


Code Breakdown

1. ServerSocket Initialization

The server starts by opening a ServerSocket on a specific port.

It continuously listens for incoming client connections.

When a client connects, it creates a ClientHandler thread for it.

2. Handling Multiple Clients (ClientHandler Class)

Each client is assigned a separate thread to handle communication.

The client sends messages via BufferedReader, which are then broadcasted to all other clients except the sender.

If a client disconnects, it is removed from the active clients list.

3. Broadcasting Messages (broadcastMessage Method)

The server keeps track of all connected clients.

Messages received from a client are forwarded to all other connected clients.



2. Chat Client (ChatClient.java)

Overview

Each ChatClient connects to the server and can send/receive messages in real-time.

Key Features

Connects to the server running at localhost on port 12345.

Handles incoming messages using a separate thread to ensure smooth UI/console operation.

Sends messages typed by the user to the server.


Code Breakdown

1. Connecting to the Server

A Socket is created using the server's IP (localhost) and port (12345).

The client opens input and output streams to communicate with the server.

2. Receiving Messages (Thread for Listening)

A separate thread continuously listens for messages from the server.

Incoming messages are displayed in the console.

3. Sending Messages (User Input)

The client reads user input from the console and sends it to the server.

4. Client Disconnection Handling

If the server closes or the user terminates the client, the connection shuts down gracefully.


Application

Multi-client Chat System: Enables multiple users to communicate in real time over a network.

Learning Socket Programming: Demonstrates fundamental concepts of Java sockets, threading, and networking.

Basic Networking Projects: Can be extended to include features like user authentication, message encryption, or a graphical user interface (GUI).


**OUTPUT**:
https://github.com/user-attachments/assets/1294db5c-ebc3-4d2d-8d98-fbba565a3c14
https://github.com/user-attachments/assets/cf5b539b-7143-4590-9fc9-8c1b6a698b67
