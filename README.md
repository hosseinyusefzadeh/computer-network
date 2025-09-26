# Computer Networks

In this repository, we aim at reviewing and learning computer networks concepts.

## What are computer networks? Why?

A computer network is simply a group of computers or devices that are connected together so they can share information and resources. These connections can be through wires, like Ethernet cables, or wireless, like Wi-Fi.

But why were networks created in the first place?
The main reason was communication and sharing. In the early days of computing, each computer worked alone, and if you wanted to send data to someone far away, you had to copy it onto a tape or disk and physically deliver it. Networks solved this problem by letting computers exchange information instantly. Scientists and engineers could share research results, programs, and even computing power without leaving their offices.

Today, networks are so important that we barely notice them — but we couldn’t live our daily lives without them. When you send a message to a friend, stream a video, play an online game, buy something from a shop on the other side of the world, or even just search for information, you are using computer networks. Banks, hospitals, airplanes, factories — almost everything depends on networks to keep working smoothly.

In short, computer networks were invented to help computers talk to each other and share resources, and now they connect the entire world.



## History
In the 1960s, scientists funded by ARPA (the Advanced Research Projects Agency in the U.S.) had a big idea: connect research computers across the country so they could share data and resources. They also wanted the system to survive failures — even if one computer or connection was shut down, the others should still work.

In 1969, their project, called ARPANET, came to life. At first, only four computers were connected — at UCLA, Stanford, UC Santa Barbara, and the University of Utah — but it was enough to show that the idea worked.

By 1973, ARPANET was using packet switching, a clever way of breaking data into small pieces and sending them through many possible routes. That same year, it even made its first international connections to Norway and London, proving this technology could go worldwide.

A big milestone came in 1983, when ARPANET switched to the TCP/IP protocol. This was like teaching all computers a common language, and it is still the language of the Internet today. Many people call this the real "birth of the Internet."

Finally, in 1990, ARPANET was retired — but by then, its ideas had spread everywhere. The Internet was growing fast. Just one year later, in 1991, Tim Berners-Lee introduced the World Wide Web, which gave us websites, browsers, and clickable links. This made the Internet easy to use and opened the door to the connected world we have today.


## Computer networks layers
The goal of these models are to break down complex network communication into smaller, manageable parts.




### The OSI model (7 layers)

#### Physical Layer
The lowest layer of the OSI reference model is the Physical Layer. It is responsible for the actual physical connection between the devices. The physical layer contains information in the form of bits.

Physical Layer is responsible for transmitting individual bits from one node to the next.

When receiving data, this layer will get the signal received and convert it into 0s and 1s and send them to the Data Link layer, which will put the frame back together.

Common physical layer devices are Hub, Repeater, Modem, and Cables.
##### Functions of Physical Layer
Bit Synchronization: The physical layer provides the synchronization of the bits by providing a clock. This clock controls both sender and receiver thus providing synchronization at the bit level.

Bit Rate Control: The Physical layer also defines the transmission rate i.e. the number of bits sent per second.

Physical Topologies: Physical layer specifies how the different, devices/nodes are arranged in a network i.e. bus topology, star topology, or mesh topology.

Transmission Mode: Physical layer also defines how the data flows between the two connected devices. The various transmission modes possible are Simplex, half-duplex and full duplex.

#### Data Link Layer
The data link layer is responsible for the node-to-node delivery of the message. The main function of this layer is to make sure data transfer is error-free from one node to another, over the physical layer.

When a packet arrives in a network, it is the responsibility of the DLL to transmit it to the Host using its MAC address.

Packet in the Data Link layer is referred to as Frame. Switches and Bridges are common Data Link Layer devices.

The packet received from the Network layer is further divided into frames depending on the frame size of the NIC (Network Interface Card). DLL also encapsulates Sender and Receiver’s MAC address in the header.

The Receiver’s MAC address is obtained by placing an ARP (Address Resolution Protocol) request onto the wire asking, "Who has that IP address?" and the destination host will reply with its MAC address.

##### Functions of Data link Layer
Framing: Framing is a function of the data link layer. It provides a way for a sender to transmit a set of bits that are meaningful to the receiver. This can be accomplished by attaching special bit patterns to the beginning and end of the frame.

Physical Addressing: After creating frames, the Data link layer adds physical addresses (MAC addresses) of the sender and/or receiver in the header of each frame.

Error Control: The data link layer provides the mechanism of error control in which it detects and retransmits damaged or lost frames.

Flow Control: The data rate must be constant on both sides else the data may get corrupted thus, flow control coordinates the amount of data that can be sent before receiving an acknowledgment.

Access Control: When a single communication channel is shared by multiple devices, the MAC sub-layer of the data link layer helps to determine which device has control over the channel at a given time.

#### Network Layer
The Network Layer is the 5th Layer from the top and the 3rd layer from the Bottom of the OSI Model. It is one of the most important layers which plays a key role in data transmission. The main job of this layer is to maintain the quality of the data and pass and transmit it from its source to its destination. It also handles routing, which means that it chooses the best path to transmit the data from the source to its destination, not just transmitting the packet. There are several important protocols that work in this layer.
<img width="1012" height="1013" alt="osi-model-network-layer-3_1" src="https://github.com/user-attachments/assets/0b06d161-e32d-4559-bba5-442a9b9a2479" />

##### functions of Network layer
Some of the most important functions of the network layer are given below :
1-Assigning Logical Address: It provides unique IP addresses to devices for identification and communication across networks.
2-Packetizing: It encapsulates data into packets for efficient transmission.
3-Host-to-Host Delivery: It ensures data is delivered from the sender to the intended receiver across networks.
4-Forwarding: It is the process of moving packets from the input to the appropriate output interface in a router, based on the destination address
5-Fragmentation and Reassembly: It splits large packets into smaller fragments for transmission and reassembles them at the destination.
6-Logical Subnetting: It divides larger networks into smaller subnetworks for better management and routing efficiency.
7-Network Address Translation (NAT): Maps private IP addresses to a public IP for internet access, conserving IPs and adding security.
8-Routing: It determines the best path for packets to travel to their destination across multiple networks.

##### How does the Network layer works?
This entire process ensures reliable, step-by-step delivery of data across complex interconnected networks.
*Every device gets a unique address (IP address) to identify it on the network.
*Data is packaged into small packets, with labels showing where it’s coming from and where it’s going.
*Routers figure out the best path to send the packets to their destination.
*Packets travel step by step through different routers until they reach the right device.
*If a packet is too big, it gets broken into smaller pieces to fit through the network.
*At the destination, the pieces are put back together into the original data.
*If something goes wrong, like the destination can’t be reached, an error message is sent back.

#### Transport Layer


#### Session Layer


#### Presentation Layer


#### Application Layer




### The TCP/IP model (4 layers)
#### Network Access/Link Layer
#### Internet Layer
#### Transport Layer
#### Application Layer
