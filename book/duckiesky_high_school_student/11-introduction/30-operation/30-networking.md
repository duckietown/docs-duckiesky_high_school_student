#Networking{Introduction-to-networking status = ready}

# Network Layers

Using the Drone and ROS you will be introducted to networking topics -LANs,IP, and TCP.Together with the application layer form the "four-layer model" for networks.The LAN layer is in charge of actual delivery of packets,The IP layer is in charge of connecting multiple LANS providing the IP address and the TCP extends the IP address features dealing with connections and trasnport.

# Defintion

Local Area Networks, or LANs - the “physical” networks that provide the connection between machines.

LANs are, as the name says, “local”; it is the IP, or Internet
Protocol, 

TCP - deals with transport and connections and actually sending user data.

# Transport

The Transport layer is the Transmission Control Protocol, or TCP. TCP extends IP with the following features:

### reliability:
TCP numbers each packet, and keeps track of which are lost and recycles them after a time out or buffer. It buffers early-arriving and out of order packers for delivery at the right time.All the data packets are then recognized by the reciever and timed.

### connection-orientation:
 When a TCP connection is made, an application sends data by writing to that connection. 
### stream-orientation:
 An application using TCP can write 1 byte at a time, or 100 kB at a time; TCP
will buffer and/or divide up the data into appropriate sized packets.



## Example:
To ship data your drone with ROS will use TCP protocols, Which in turn calls the IP layer and then the LAN layer to delivery
the data. An application will not interact directly with IP and Lan layers at ALL. 
### How does the drone and basestation communicate?

All machines with the same network address can communicate with one Another.

Testing this, you can use "ping IP Address", to see if there is a connectibity between the drone and your Base Station when connecting to your drones network.

## Example:
### Ping 192.168.42.1
Output:
### 64 bytes from 192.168.42.1: icmp_seq=166 ttl=64 time=15.7 ms


## Example:

 
**Useful Resources and References**

[How Application Layer Services Work](https://www.youtube.com/watch?v=mGRClHHgNdk)

[TCP/IP Model Explained ](https://www.youtube.com/watch?v=PpsEaqJV_A0)

