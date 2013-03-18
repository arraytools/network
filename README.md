network
=======
network contains simple C codes for testing socket programming. 

## Source

The source code was originally from [linuxhowtos.org](http://www.linuxhowtos.org/C_C++/socket.htm).

The source code for server.c and server2.c is modified to avoid an error "ERROR on binding: Address already in use". See [here](http://www.yolinux.com/TUTORIALS/Sockets.html) for an explanation.

## Features

* The client and server does not have to be on the same machine.
* The client and server does not have to be on the same type of OS.
* How about the compiler?

## Getting Started

From a bash shell:

```c
gcc server.c -o server
gcc client.c -o client
```

To test the connection, from the server side
```bash
$ ./server 51717
```

From the client side,
```bash
$ ./client 192.168.1.10 51717
```

We will see server side shows up the message client side has entered.



