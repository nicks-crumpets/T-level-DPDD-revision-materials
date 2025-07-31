# Wired & Wireless networks

# Types of wireless Networks

- WLAN - Allows all users in a small area, such as a home or a library
- WPANS - IR and Bluetooth (IEE 802.155) can be used to share connections in a PAN (Dist. 30ft)
- WMANS - Connection of multiple networks in a MAN, alternative to cabling
- WWANS - Can be maintained over cities or countries, such as 2G

### Wireless standards

The IEE Defines the mechanical process of how WLANS are implemented the 802.11 standards to keep products compatible 

Wi-Fi alliance - certifies companies by ensuring their products follow 802.11 standard.

This makes sure all types of wireless networks will (mostly) work seamlessly together without issue.

WLAN Standards

![image.png](Wired%20&%20Wireless%20networks%201115301291278014a095cd98c9227745/image.png)

# Signal distortion

- Absorption objects - Absorb RF webs killing the Wi-Fi signal
- Scattering objects - Dispersing RF waves by carpet, plasterboard etc.
- Reflection objects -  Reflecting waves in another direction (Glass, mirrors)

# Transmission methods

### **Direct sequence Spread Spectrum**

One channel to send data across all frequencies in the channel

### **Orthogonal Frequency Division Multiplexing (OFDM)**

Uses a spread spectrum to increase data rates 

### **MIMO Multiple input Multiple output**

Uses DSS and/or ODFM by spreading across 14 overlapping channels at 5MhZ

# 802.11 Access modes

- Ad hoc mode - Based on the independent basic service set (IBSS) Setting connections directly to other clients
- Infrastructure mode - Designed to deal with security and scalability issues. Wireless clients can communicate with each other via an Access Point, the two implementations currently in use are:
    - Basic service set (BSS)
        
        Clients connect to an AP, allowing communication or LAN-based resources. The WLAN is identified by a single SSID, with each AP having a unique ID, a Basic Service Set Identifier (BSSID), the MAC address of the AP’s wireless card. Often used for non roaming clients
        
    - Extended service set (ESS)
        
        Two or more BSS’s are interconnected to allow larger roaming distance, the AP’s also share a single SSID,  but have a unique BSSID
        

# Encryption & Security

### Wired Equivalent Privacy

First security solution for WLAN’s that used encryption. Uses a static- 64-bit key, where the key is 40 bits long and a 24-bit initialisation vector (IV) is used, sent in clear text.

Because WEP uses RC4 as an encryption algorithm and the IV is sent in plain text, it can be broken, therefore, the key was extended to 104 bits with the IV value. Either variation can easily be broken on modern technology now

## 802.1x EAP | Extensible Authentication protocol (EAP)

A layer 2 process that allows a wireless client to authenticate to the network, the two varieties, one being for wireless connections, and one for LAN connections, known as EAP over LAN (EAPoL)

One of the issues in wireless is allowing a WLAN client to communicate to devices behind an AP. There are 3 standards for this process:

- EAP
- 802.1x
- Remote Authentication Dial In User Services (RADIUS)

EAP defines a standard way of encapsulating authentication information, such as a username and password, or a digital certificate that the AP can use to authenticate the user.

802.1x and RADIUS define how to packetize the EAP information to move it across a network

### Wi-Fi Protected Access (WPA)

Can operate in two modes, personal and enterprise mode

Personal mode was designed for home & SOHO usage, a pre-shared key is used for authentication, requiring the configuration of the same key on the client and the AP

Enterprise mode is meant for large companies where authentication servers will centralise the authentication credentials of the clients

### WPA 2

Instead of using WEP, which uses the weaker RC4 encryption algorithm, the much more secure Advanced Encryption Standard (AES) counter mode CBC-MAC Protocol (CCMP) algorithm

### WPA 3

Safer with more features, passwords are harder to crack, old data is safer, 

## Advantages of wireless networks

- Highly mobile, just need to be within a range
- Much lower cost to set up a wireless network, fewer resources
- BYOD is easy to implement, as the policy can be just for a wireless network

- Makes the area look much ✨prettier✨
- Simple to install & maintain

  

## Disadvantages of wireless networks

- Security can be a concern, as the media to connect is available (WPA2, WP3)
- Slower and somewhat unreliable data transfer speed (interference, number of users)
- It  can be unreliable and interference is a massive issue

## Advantages of wired networks

- Stable & reliable
- No interference from other networks
- Much faster
- Invisible if you don’t know it exists
- Easier to instal

- Limited set of users, speed stays consistent
- Own separate feed (The cable you connect with)
- Better security, as the network is all closely monitored
- Cheaper to set up than wired

## Disadvantages of wired networks

- Inflexible and stuck in one place
- Can’t easily run cables
- May require more time to install

- Need to have skills to set up and install a wired network
- Maintenance is essential, staff may be needed
- Cables get messy very quickly & can get disconnected mistakenly (oh no)

# What’s best?

Depends on what you want. 

Security? Wired. 

Portability? Wireless. 

Both? Hybrid

MAC - Media Access Control (Address)