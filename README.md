
# Foundations of Python Network Programming

Welcome!

This GitHub repository offers all of the example Python code from the
Third Edition of *Foundations of Python Network Programming* as revised by
[Brandon Rhodes](http://rhodesmill.org/brandon/) for Python 3:

Each chapter’s source code lives in its own directory:

*   [Chapter 1: Introduction to Client-Server Networking](py3/chapter01#readme)
*   [Chapter 2: UDP](py3/chapter02#readme)
*   [Chapter 3: TCP](py3/chapter03#readme)
*   [Chapter 4: Socket Names and DNS](py3/chapter04#readme)
*   [Chapter 5: Network Data and Network Errors](py3/chapter05#readme)
*   [Chapter 6: TLS/SSL](py3/chapter06#readme)
*   [Chapter 7: Server Architecture](py3/chapter07#readme)
*   [Chapter 8: Caches and Message Queues](py3/chapter08#readme)
*   [Chapter 9: HTTP Clients](py3/chapter09#readme)
*   [Chapter 10: HTTP Servers](py3/chapter10#readme)
*   [Chapter 11: The World Wide Web](py3/chapter11#readme)
*   [Chapter 12: Building and Parsing E-Mail](py3/chapter12#readme)
*   [Chapter 13: SMTP](py3/chapter13#readme)
*   [Chapter 14: POP](py3/chapter14#readme)
*   [Chapter 15: IMAP](py3/chapter15#readme)
*   [Chapter 16: Telnet and SSH](py3/chapter16#readme)
*   [Chapter 17: FTP](py3/chapter17#readme)
*   [Chapter 18: RPC](py3/chapter18#readme)

## The Network Playground

Many novice network programmers do not have interesting networks to
explore — many homes have only a laptop plus a broadband modem to which
the homeowner does not have access.

To remedy this situation, I have developed an entire [Network
Playground](playground) consisting of more than a half dozen hosts
providing services from SSH and Telnet to a web server and FTP.  The
“hosts” are built using Docker, and I hope soon to package the whole
thing up as a virtual machine that users can download.

The result will be that the user can get a prompt from which they can
connect out to the `example.com` server farm and talk to all kinds of
network services.  And just as in a real network, they will find that
these machines are several hops away — hops that can be inspected by
normal networking tools like `traceroute`:

```
$ ssh h1

# traceroute www.example.com
traceroute to www.example.com (10.130.1.4), 30 hops max, 60 byte packets
 1  192.168.1.1 (192.168.1.1)  0.513 ms  0.208 ms  0.265 ms
 2  isp (10.25.1.1)  0.544 ms  0.220 ms  0.115 ms
 3  backbone (10.1.1.1)  0.364 ms  0.227 ms  0.252 ms
 4  example.com (10.130.1.1)  0.617 ms  0.355 ms  0.407 ms
 5  www.example.com (10.130.1.4)  1.301 ms  0.415 ms  0.522 ms
```

You can find the instructions here: [The Network Playground](playground).

## The Python Base

This folder contains some exercises for me to learn the basic syntax of Python.









