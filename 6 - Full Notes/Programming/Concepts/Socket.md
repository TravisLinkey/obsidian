
Low-level endpoint for sending and receiving data between devices over a network.

A fundamental concept used in network programming, and can operate over various protocols.

### Types

- ***TCP Sockets*** - Provide a reliable, connection-oriented communication channel. Data sent through a TCP socket is guaranteed to arrive in order, without errors.

- ***UDP Sockets*** - Provide a connectionless, unreliable communication channel. Data sent through UDP socket might arrive out of order, be duplicated, or get lost without notification.

### Examples

- ***TCP Sockets*** - Applications like SSH, HTTP/HTTPS, where a reliable connection is required.

- ***UDP Sockets*** - Applications like DNS, VoIP, and online gaming, where speed is more critical than reliability.