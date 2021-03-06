# PennCloud
Demo and Description for PennCloud - CIS 505 Final Project

# Information

This repository only contains the screenshots of the actual application, in compliance with the course policies that prevent sharing and publishing code as per the academic integrity requirements.

The private repo, [PennCloud-Code](https://github.com/anantm95/PennCloud-Code) contains the entire code. Please [write to me](mailto:anantm95@gmail.com) if you'd like access to the code.

# Description

PennCloud is a distributed cloud platform with a highly scalable, fault-tolerant key-value datastore at the backend that supports strong consistency, efficient replication, checkpointing and recovery.

# Team Members
* [Anant Maheshwari](https://www.linkedin.com/in/anantm95)
* [Garvit Gupta](https://www.linkedin.com/in/garvitgupta)
* [Sahana Vijaya Prasad](https://www.linkedin.com/in/sahana-vijaya-prasad)
* [Shiva Suri](https://github.com/shivasuri)

# Screenshots

![Drive](https://github.com/anantm95/PennCloud/blob/master/Images/Screen%20Shot%202018-06-17%20at%204.38.26%20PM.png "Drive")
Users can upload files, create folders, rename, delete, or move the items to different directories. All the files are replicated on `W` quorum servers at the backend.

![Admin](https://github.com/anantm95/PennCloud/blob/master/Images/Screen%20Shot%202018-06-17%20at%204.34.34%20PM.png "Admin")
The admin console lists all the active and inactive back-end servers, with an option to start or stop them.

![Mail](https://github.com/anantm95/PennCloud/blob/master/Images/Screen%20Shot%202018-06-17%20at%204.35.09%20PM.png "Mail")
Users can receive emails and send emails to local (@PennCloud) users and external users, which are relayed to the appropriate servers by checking the DNS MX records. The email server follows the `SMTP` protocol.

![Game ID](https://github.com/anantm95/PennCloud/blob/master/Images/Screen%20Shot%202018-06-17%20at%204.35.22%20PM.png "Game ID")
Allows players to create tic-tac-toe game and share the unique generated ID with friends to join the game.

![Game Play](https://github.com/anantm95/PennCloud/blob/master/Images/Screen%20Shot%202018-06-17%20at%204.36.49%20PM.png "Game Play")
Supports multiple users to play concurrently with two people joining one game.

## Components and system design

* Load balancer
* Front-end Server: HTTP Server, Quorum Client
* SMTP Mail Server
* Master Node
* Quorum group constituting of Storage Nodes
* Heartbeat Server
* Admin Console

<p align="center">
  <img src="https://github.com/TheGarvitGupta/PennCloud/blob/master/Images/Untitled-1.png" alt="System Design"/>
  <p align="center">System Design</p>
</p>
