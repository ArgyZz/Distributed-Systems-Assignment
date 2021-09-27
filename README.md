# Distributed-Systems-Assignment
A recreation of the backend of a Tik-Tok Clone

A recreation of Tik-Toks backend in Java.
A 3 leveled program which allows sending data from one class to the other through a middle class that works as a server.
The program uses multithreading to ensure that a lot of clients can connect to one or more servers.
(The program is not great and is missing a lot of key features)

So to begin we have
1) The broker opperates as a server in our case 
2) The Publisher is the "person" that can post videos
3) The Cosnumer is the "person" who can see videos posted but the publishers
4) Publisher and Consumer could be the same person but they are not in our case.
5) We can create up to 3 brokers.
6) we can create as many publishers or consumers that we want


To Run:
1) We first initializing the Server (Broker) with port of 1234 or 5678 or 9101
2) Then we initialize the AppNode: 1 for publisher 0 for consumer
3) We initialize first for publisher. The publisher will automaticaly find the broker that it should connect to.
4) We select the Channel name(Check in the folder PublishersVideo for the names of the channels) You can create a new channel from inside the program.
5) We initialize the AppNode as a Consumer and we select the channel that we want to check 
6) Lists of videos appears
7) Type the name of the video that you want.
8) Data is sent localy from the Publisher to the Consumer through the broker
9) New Video is not playable because there are no metadata.
