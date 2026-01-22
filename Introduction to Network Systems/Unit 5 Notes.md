The protocol at layer 3 uses IPv4 and Ipv6. IPv4 is connectionless, there is no cknowladgement the packet was recieved. The packet structure for the network layer has a packet header and encapsulates the 4th layer. It provides 3 layer addressing allowing packets to be transfered between remote networks. IPv6 is more simplified than IPv4. 

IPv4 Headers:
-Version: 4 decimal
-TOS: Type of service 
-TTL: Time to Live is how many network boundaries before it is discarded
-Protocol: What is the payload

Address Formatting:
-An IPv4 address is Binary and 32 bits long
    -Shown in “dotted-decimal” format
    -Easier for humans to read
    -Each decimal value represents an 8-bit binary number
    -8 bits is called an octet or a byte
        -10 . 1 . 2 . 3
        -00001010 . 00000001 . 00000010 . 00000011
        -Actual Address = 00001010000000010000001000000011 (What a computer sees)
    -Decimal values are from 0 to 255
    -Decimal 0 = Binary 00000000
    -Decimal 255 = Binary 11111111

-IPv6 address
    -Uses 128 bits to identify source and destination network and hosts.
    -2128 addresses = 340 Trillion Trillion Trillion (3.40*1038)
    -Latest version of the Internet Protocol, represented in Hexadecimal (Base-16)

A subnet mask indicates which bits of the IPv4 address belong to the network portion and which to the host. It uses binary ANDing process to determine whether an address is inside or outside a local network. It is expressed in dottted-decimal format. Binary ANDingis determining on or off wiht logic. 

IPv4 Class Addressing:
Based on first four bits of the IP address
Class A
0xxxxxxx = 00000000 to 01111111 = 0 to 127
Default mask = 255.0.0.0 = /8
Class B
10xxxxxx = 10000000 to 10111111 = 128 to 191
Default mask = 255.255.0.0 = /16
Class C
110xxxxx = 11000000 to 11011111 = 192 to 223
Default mask = 255.255.255.0 = /24
Class D (Multicast)
1110xxxx = 11100000 to 11101111 = 224 to 239
Class E (Experimental)
1111xxxx = 11110000 to 11111111 = 240 to 255

IPv4 Address Types: 

-Unicast (one host)
Host section cannot be all 0’s or all 1’s
-Network (also called Subnet)
Host section all 0’s
-Directed Broadcast
Host section all 1’s
-Broadcast
255.255.255.255 (all 1’s)
-Multicast
D Class
224.x.x.x are “well known”

IPv6 Address Types:

-Global Unicast – Unique address for use on public networks. Currently using addresses beginning with 2000::/3 (2000-3fff in first hextet)
-Unique Local – Address usable only in private network spaces. Addresses begin with FD00::/8
-Link Local – Unique addresses usable only inside the local network. Addresses begin with FE80::/10 
-Multicast – Group addresses that configured devices will receive packets on only if directed to do so. Addresses begin with FF00::/8

















































