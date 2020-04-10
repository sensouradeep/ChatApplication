# ChatApplication
Making a Chat Application using Java
1. How to Run the Chat Server
You need to specify the port number when running the server program from the command line. For example:
>>java ChatServer 8989
This starts the server listening on the port number 8989, and you see the following output in the server once it started:
>>Chat Server is listening on port 8989
The server is waiting for new clients forever, so you have to press Ctrl + C to terminate it.
 
2. How to Run a Chat Client
To run the client, you need to specify the server’s hostname/IP address and port number in the command line. For example:
>>java ChatClient localhost 8989
This tells the client to connect to the server at localhost on port 8989. Then you see the following message in the server’s console:
>>New user connected
And in the client’s console:
>>Connected to chat server
>>No other users connected
You see, the server tells the client how many users are connected, but there’s no user at this time. Then the program asks for the username:
>>Enter your name:_
>>Enter a username, say John, and then you can start chatting:
>>Enter your name: John
>>[John]:_
>>Now, let’s start the second client with username is Peter. At this time, you see the server tells that there’s one online user is John:
>>Connected users: [John]
>>The user John is notified about new user Peter:
>>New user connected: Peter
>>Type some messages from John and Peter and you see each user sees other’s messages, just like talking in a chat room.
>>Now, John wants to quit so he types ‘bye’- the client program terminates, and you see the following output in the server’s console:
>>The user John quitted
Peter also gets a message from the server:
>>John has quitted.



That’s basically how the chat application is running. You can test it with more clients and the application is still running smoothly.
