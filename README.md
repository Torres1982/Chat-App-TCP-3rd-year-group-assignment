# Chat-App-TCP-3rd-year-group-project

Technologies used: Java, TCP, UML.

The goal of the project was to create a messenger/chat application implementing a remote communication using 
java socket programming and multi-threading.

The chat application includes a Server and a Client program, and also a GUI interface that supports the Client’s terminal.
The GUI framework enables users to choose among several unique terminal skins, which differ in color from each other. 
A few sound effects applied to the “Send Message” button are also provided to the users, which can be used according to 
their preferences. The application allows clients to navigate through the “Menu Bar” or use the “Accelerator Keys” to
access some of the functionalities of the software application.

In order to maximize the efficiency of this system and how it operates, multi-threading has been be applied. 
The application can accommodate multiple hosts; in order to achieve this, threads are implemented. In the client a new thread 
is started, which uses an inner class as the runnable task for the thread. The thread can then read in from the server’s 
socket stream broadcasting all the messages to connected clients (the messages are displayed in the text area). On the server 
side the application uses threads to read the client messages and then broadcast the messages to all participating clients. 

This application uses java sockets which enables a connection from a process to another process. These socket objects created 
in java can then manage stream based connections. The essence of what this system does is to concurrently send and receive 
messages to the server, interacting with the GUI and simultaneously reading messages coming in from the server to the client. 
This task is completed through software constructs (sockets) on both the server application and the client where the 
server listens for requests from the clients on a designated port.
