# OSI & TCP/IP

# OSI Model (Open systems interconnection)

1. **Application**
- Most users interact with this, applications
- Protocols work with the data the person is using
- Supplies to and receives data from layer 6

1. **Presentation**
- Converts data from one format to another (like encryption & decryption)
- Translates the data from the top layer back and vice versa
- Transfers to session layer (when)

1. **Session**
- Starts & stops connections between devices
- Starts & stops connections when interrupted

1. **Transport**
- Transmission of data over networks (speed, where is goes etc.)
- TCP & UDP usually
- Once completed passed to or  received from the network layer

1.  **Network**
- Routing of data
- Sends data to the correct location
- IP part
- Manages IP and MAC addresses
- For IP it uses ARP

1. **Data link**
- Most complex
- Packages the data packets
- MAC Media access control
- LLC Logical Link control
- Data passes to or from the physical layer

1. **Physical**
- Electrical/Physical label (Cables, PINOUTS, light, voltage etc.)
- Is the device plugged in? Y/N
- 5V or 0V for cables

7 → 4 are host layers, all other are media layers

**All**

**People**

**Seem**

**To**

**Need**

**Data**

**Processing**

# TCP/IP

1. Application
    
    Combines functions of the application, presentation and session layers from the OSI model.
    
    The layer is similar to the transport layer of the OSI model and is responsible fro end to end communication, and error free delivery of data, shielding the upper layer applications from the complexities of data
    
2. Transport layer
    
    Exchange data receipt acknowledgements and retransmit missing packet, ensuring that packets arrive in order and without error
    
    Protocols:
    
    - TCP → Applications interact together using TCP as they were physically connected, it transmits data in a way resembling character by character transmission rather than separate packets. A starting point that establishes the connection, the transmission in byte order and the ending point that closes the connection to make up the transmission
    - UDP → Datagram delivery service is provided by UDP. Connections between receiving and sending hosts are not verified by UDP, commonly used by applications that transport small amounts of data, as it eliminates then process of establishing and validating connections
3. Network layer
    
    Parallel to the OSI network layer
    
    Defines the protocols which are responsible for logical transmission of data over a network.
    
    Main protocols:
    
    - IP → Internet Protocol, Responsible for delivering packets from source host to destination host by looking at the IP addresses in packet headers
    - ICMP → Internet Control Message Protocol, in IP diagrams and responsible for providing hosts with information about network problems
    - ARP → Address Resolution Protocol, Finds the hardware address of a host from a known IP address. It has various types: Reverse ARP, Proxy ARP, Gracious ARP and Inverse ARP)
4. Network access layer
    
    A collection of applications that require network communication.
    
    Layer is responsible for generating data and initialising connection requests, and manages data transmission, and receiving data. 
    
    The packets network protocol type (TCP/IP) is identified by the layer
    
    Error prevention and framing are provided (PPP Framing and IEEE 802.2 framing are two examples)
    

# TCP/IP VS The OSI model

TCP/IP is the physical way that computer processes data, whereas the OSI model is the theoretical model