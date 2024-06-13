In computer networking, localhost is a hostname that refers to the current computer used to access it. The name localhost is reserved for loopback purposes.
The Internet Protocol Version 4 address 0.0.0.0 can have multiple uses. 
The hosts file is a plain text file that all operating systems use to translate hostnames (also known as web addresses or URLs) into IP addresses. When you type in a hostname, such as wikipedia.org, your system will look into the hosts file to get the IP address needed to connect to the appropriate server. 
Netcat or nc is a networking utility for debugging and investigating the network.

This utility can be used for creating TCP/UDP connections and investigating them. The biggest use of this utility is in the scripts where we need to deal with TCP/UDP sockets.

In this article we will learn about the netcat command by some practical examples.
1. Netcat in a Server-Client Architecture

The netcat utility can be run in the server mode on a specified port listening for incoming connections.

$ nc -l 2389

Also, it can be used in client mode trying to connect on the port(2389) just opened
$ nc localhost 2389

Now, if we write some text at the client side, it reaches the server side. Here is the proof :

$ nc localhost 2389
HI, server
