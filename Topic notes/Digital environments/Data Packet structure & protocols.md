# Data Packet structure & protocols

# Protocols

*“Network protocols are a set of rules, conventions, and data structures that dictate how devices exchange data across networks. In other words, network protocols can be equated to languages that two devices must understand for seamless communication of information, regardless of their infrastructure and design differences”*

**Simple explanation:** A set of rules devices follow to connect over a network, so they can communicate (”talk”)

## Transmission types

![image.png](Data%20Packet%20structure%20&%20protocols%201185301291278036a11ac85153e9eee0/image.png)

# Data packet anatomy

In networking, data is bundled into packets of data. They travel around an area, and are unpacked by another node/computer on the network.

Administrators and engineers who troubleshoot & analyse networks sometimes use protocol analysers to open packets giving an insight on what’s happening on then network.

Examples of various common data packet anatomies:

## UDP

A connectionless protocol containing no reliability (Best effort, no guarantee, like the postal system)

←———————————  32 Bits  —————————————>

| Source port | Destination Port |
| --- | --- |
| Length | Checksum |

## TCP

Every single packet gets delivered (A guaranteed delivery service)

A connection-oriented Layer 4 protocol that provides full-duplex, acknowledged, and flow-controlled service

TCP always operates in full-duplex mode (two independent byte streams travelling in opposite directions) Only during the start and end of a connection will data be transferred in one direction and not the other  

![DataPacketStructures.drawio.png](Data%20Packet%20structure%20&%20protocols%201185301291278036a11ac85153e9eee0/DataPacketStructures.drawio.png)

- **Source Port** and **Destination Port** fields (16 bits each) identify the end points of the connection
- **Sequence Number** field (32 bits) specifies the number assigned to the first byte of data in the current message
- **Acknowledgement Number** field (32 bits) contains the value of the next sequence number that the sender of the segment is expecting to receive, if the ACK control bit is set
- **Data Offset** (a.k.a. Header Length) field (variable length) tells how many 32-bit words are contained in the TCP header
- **Reserved field** (6 bits) must be zero. This is for future use
- **Flags field** (6 bits) contains the various flags:
    - **URG** → Indicates that some urgent data has been placed
    - **ACK** → Indicates that acknowledgement number is valid
    - **PSH** → Indicates that data should be passed to the application as soon as possible.
    - **RST** → Resets the connection
    - **SYN** → Synchronizes sequence numbers to initiate a connection
    - **FIN** → Means that the sender of the flag has finished sending data
- Window field (16 bits) specifies the size of the sender's receive window (that is, buffer space available for incoming data).
Checksum field (16 bits) indicates whether the header was damaged in transit.
Urgent pointer field (16 bits) points to the first urgent data byte in the packet.
Options field (variable length) specifies various TCP options.
Data field (variable length) contains upper-layer information.

# Circuit switching and packet switching

What is packet switching?

Grouping data into packets that are transmitted over a network, Data in the header is used by networking hardware to direct the packet to its destination

What is circuit switching?

*A dedicated route that data must transmit over*

Implementing a telecommunications network where two network nodes establish a dedicated communications channel, known as a circuit, through the network before the nodes can communicate

This allows full bandwidth to be used and the nodes are connected for the entire communication duration

 There are 2 types of packet switching:

- Datagram (The internet)
- Virtual circuit (Frame relay, ATM)

### Simple switching network

![image.png](Data%20Packet%20structure%20&%20protocols%201185301291278036a11ac85153e9eee0/image%201.png)

Packet switching examples

- Designed for voice services
- Resources dedicated to a particular call
- In data transmission, lots of the time is idle (e.g. web browsing)
- Fixed data rate

## Basic operation

Data is transmitted in short packets

Typically in the order of 1000 bytes, with longer messages being split into multiple packets, containing a portion of user data & control info.

Control info must have:

- Routing info, to be routed to the correct destination
- Recall the content of an IP header

## Advantages of packet switching

- Line efficiency
- Data rate conversion
- Priorities can be used

## Datagram

![image.png](Data%20Packet%20structure%20&%20protocols%201185301291278036a11ac85153e9eee0/image%202.png)

## Virtual Circuit

A pre-planned route is established before any packets are sent, then all packets take the same route. (Usually used for networks with very heavy traffic)

Each packet contains a virtual circuit identifier as opposed to  a destination address. Each node on the route knows where to forward the packets, it doesn’t need to make a decision.

![image.png](Data%20Packet%20structure%20&%20protocols%201185301291278036a11ac85153e9eee0/image%203.png)

# Comparison of communication switching techniques

![image.png](Data%20Packet%20structure%20&%20protocols%201185301291278036a11ac85153e9eee0/image%204.png)