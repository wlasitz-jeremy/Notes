The data link layer defines the rules for sending and recieving data between two different network nodes. Frame encoding and error checking is done at this level. 

It is split into two sublayers: 

-LLC: Logical Link Control communicates the networking software at higher layers and device hhardware. It also deals with deals with addressing, multiplexing and acknoladgement messages.

-MAC: Media Access Control is responsible for data encapsulation and de-encapsulization as well as access to the physical media. It controls the interaction between devices and provides frame synchronization. 

There are several protocols that can be used at layer 2 to direct traffic inside of a network:
-Virtual LAN
-PPP (Point-To-Point Protocol)
-WAN
-Ethernet
-Frame Relay
-High-Level Data Link Control (HDLC)
-Multi-Protocol Label Switching (MPLS)
and others
-Ethernet is the default Protocol at Layer 2. Any other protocol would be specified.

Every layer has their own header they create when sending  and they are stripped when the data is unpacked. 

The frame structure of headers has a frame header on one side with a payload in the middle and a frame trailer on the other side. Within the header the FRAME START designates the start of the frame. The ADDRESSING is the source and destination of the MAC addresses. The TYPE indicates the protocol used at layer 3. The CONTROL shows the flow control services.

The frame structure of the trailer has two parts within it. The ERROR DETECTION is used to determine errors while in transit. The FRAME STOP indicates the end of the frame.

Media Access Control – Every Network Interface Card (NIC) has a unique 48-bit MAC address in hexadecimal. These addresses are also called physical addresses; they are burned into the hardware.

Each MAC address is broken into 2 sections:
-OUI – Organizationally Unique Identifier: 24 bits assigned to a specific manufacturer/model by the IEEE
-Vendor Assigned ID: 24 bits unique to the specific interface

A Unicast addresses points to a single NIC. A Broadcast addresses make sure all the hosts on the network recieve the frame. A Multicast addresses frames within a multicast MAC address will be recieved by interfaces that are configured as a group. 

Common Topologies:

-Bus: Each network node connect to a common media. Wireless works as a bus topology in some respects.
-Ring: Each node has 2 connections, one to each of 2 neighbours. Traffic moves from source to destination in one direction through each of the intervening nodes.
-Star: Each node connects to a common central point, typically a switch. The most common small network topology.
-Mesh: Full: Each node is connected to every other node using a point-to-point connection. Partial: Some nodes are connected to every other node, other are connected to select other nodes



































