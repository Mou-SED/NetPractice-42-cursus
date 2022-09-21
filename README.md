<div align="center">
<img width=1000 hiegth=400 src="doc/Group%205.png">
</div>

<div align="center">
NetPractice is a general practical exercise to let you discover networking specifically on Subnetting.
</div>

## What is  an IP address
An IP address is simply an identifier for each device in a network, it is through it that the device can communicate with other devices, there are two different types.
- IPv4: Example of IPv4 -> 66.94.29.13
  - has a 32-bit address length.
  - It Supports Manual and DHCP address configuration.
  - In IPv4 end to end, connection integrity is Unachievable.
  - It can generate 4.29×109 address space.
  - The Security feature is dependent on application.
  - Address representation of IPv4 is in decimal.
  - Fragmentation performed by Sender and forwarding routers.
  - In IPv4 Packet flow identification is not available.
  - In IPv4 checksum field is available.
  - It has broadcast Message Transmission Scheme.
  - In IPv4 Encryption and Authentication facility not provided.
  - IPv4 has a header of 20-60 bytes.
  - IPv4 consist of 4 fields which are separated by dot (.) -> (---.---.---.---).
  - IPv4’s  IP addresses are divided into five different classes. Class A , Class B, Class C , Class D , Class E.
  - IPv4 supports VLSM(Variable Length subnet mask).
- IPv6: Example of IPv6 -> 2001:0000:3238:DFE1:0063:0000:0000:FEFB
  - IPv6 has a 128-bit address length.
  - It supports Auto and renumbering address configuration.
  - In IPv6 end to end, connection integrity is Achievable.
  - Address space of IPv6 is quite large it can produce 3.4×1038 address space.
  - IPSEC is an inbuilt security feature in the IPv6 protocol.
  - Address Representation of IPv6 is in hexadecimal.
  - In IPv6 fragmentation performed only by the sender.
  - In IPv6 packet flow identification are Available and uses the flow label field in the header.
  - In IPv6 checksum field is not available.
  - In IPv6 multicast and anycast message transmission scheme is available.
  - In IPv6 Encryption and Authentication are provided.
  - IPv6 has header of 40 bytes fixed.
  - IPv6 consist of 8 fields, which are separated by colon -> (---:---:---:---:---:---:---:---).
  - IPv6 does not have any classes of IP address.
  - IPv6 does not support VLSM.

In our NetPractice project, we will use IPv4.
<hr/>
Before starting the problem to be solved in the project (Subnetting), we start with the TCP protocol that allowed application programs and devices to exchange messages.

## TCP: Transport Layer

<div align="center">
<img width=200 hiegth=200 src="doc/tcp.png">
</div>

TCP is the abbreviation for Transmission Control Protocol. It is a communication standard that allows application programs and devices to exchange messages over a network. It is used to send packets over the Internet.

TCP ensures the integrity of data communicated over a network. Before transmitting data, TCP establishes a connection between a source and its destination, which remains active until the communication begins. It then breaks large amounts of data into smaller packets, while ensuring end-to-end delivery without data loss.

The IP protocol is part of a suite of Internet protocols, which also includes the Transmission Control Protocol. Together, these two protocols are known as TCP/IP. The Internet protocol suite manages the rules for packetizing, addressing, transmitting, routing and receiving data on networks.

## Public Address and Private Address

In the world of IPv4, we will use different types of IP addresses to complete the largest number of device available in the world, the two different types being the public IP address and the private IP address.

A public IP address is an IP address that can be accessed directly through the Internet and is assigned to your network router by your Internet Service Provider (ISP). A public (or external) IP address helps you connect to the Internet from inside your network, to outside your network.

A private IP address is the address your network router assigns to your device. Each device on the same network is assigned a unique private IP address (sometimes called a private network address) - this is how devices on the same internal network talk to each other.

When a network is connected to the Internet, it cannot use any of the reserved private IP addresses. The following ranges are reserved for private IP addresses:

```
192.168.0.0 – 192.168.255.255 (65,536 IP addresses)
172.16.0.0 – 172.31.255.255   (1,048,576 IP addresses)
10.0.0.0 – 10.255.255.255     (16,777,216 IP addresses)
```

## Subnet Mask

The principal factor in solving the subnetting problem is the subnet mask, which has the same form as the IP address (---.---.---.---), which is the address used to separate a network address from a host address in the IP address. It defines the range of IP addresses that can be used in a network or subnet.
