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

















































