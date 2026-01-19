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

Hubs and Switches:
-All work at Layer 2 of the OSI reference model

-Hubs forward frames out of every port except the port on which the frame was received, like a broadcast frame. Frames can collide on the media, causing problems in transmission. Requires half-duplex, send or receive, not both.
-
Switches use a MAC address table to track which MAC address is attached to which switchport, which means that each frame can be forwarded to the specific device to which it is destined instead of flooded out every port. Can operate in full-duplex, send and receive.

A collision domain is a media segment where collisions can occur. A hub forwards all traffic out of every port, all media segments are considered as part of the same collision domain. A switch breaks up collision domains, because frames are sent only to the port where the MAC address is attatched. This makes a switch more efffective and efficient .It cuts down on collisions making re-transmission of frames less frequent. 

A switch learns which MAC address is connected to each port by reading the source MAC address from incoming frames on the port. This MAC address/port combination gets added to the MAC address table and refreshed over time to ensure that information in the MAC address table is accurate. 
The switch then uses the MAC address table to compare destination addresses to determine which switchport to forward them out of.
*Some switches have a type of memory called ‘Content Addressable Memory, so the MAC address table may also be called the CAM table.*































