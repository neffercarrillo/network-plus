# Notes on Dion Training's Network+ Udemy Course

## Section 1: Introduction

### Introduction

- this is a foundational course
- 5 domains 1 networking concepts. 2 network implementation. 3 network operations. 4 network security. 5 network troubleshooting (this is the largest domain).
- 90 minutes to answer up to 90 questions
- there will be multiple choice, multiple select and pbqs (simulations)
- passing score: 720/900 (75% of the questions right)
- buy vouchers for the exam from jasondion.com/vochers (10% discount)
- 4 tips 1 closed captions are available. 2 control speech speed. 3 download and print the study guide. 4 join fb group and/or discord server.

### Download your free study guide

- downloaded 3 files. 1 exam objectives. 2 study notes. 3 study plan.

### Exam Tips

- 1 there will be no trick questions
- 2 pay attention to bold, italics or all uppercase
- 3 answer the questions based on the CompTIA Network+ knowledge
- 4 try not to fight the exam or the test questions
- 5 do not memorize the terms
- 6 there are no fill in the blank questions
- 7 set target date to get certified

## Section 2: Network Fundamentals

### Network Fundamentals

- networks can be wired or wireless
- 99.999 allows for five minutes of downtime each year (it has 5 nines. think about the number of nines and determine the amount of minutes/year)
  
###  Network Components

- clients. devices.
- servers. provide resources to the network.
- hubs. connect other network devices together over a LAN. older. increased network errors.
- switches. smart hubs. provide security and bandwidth utilization.
- wireless access points (WAP/AP). allow wireless devices to connect to a wireless network.
- routers. used to connect different networks together.
- firewalls. security barrier between internal and external networks.
- load balancers. distribute traffic across servers.
- proxy. intermediary between a user's device and the internet.
- intrusion detection systems/introduction prevention systems. ids detects. ips takes action to prevent intrusion.
- controllers. software-defined networking. central units used to manage flow control to network devices.
- network attached storage (NAS).
- storage area network (SAN). provides access to to consolidated block-level data storage.
- media. physical materials used to transmit the data.
- wide area network (WAN). connect network over large geographical areas.

### Network Resources

- client/server model. uses a dedicated server to provide resources. admin and backup are easier.
- peer-to-peer model. peers or other machines can share resources directly. harder to backup because files exist in different places.

### Network Geography

- personal area network (PAN). smallest type of wired/wireless network. covers less than 10 ft/3m.
- local area network (LAN). covers bout 300 ft/100m. wifi. 802.11. ethernet 802.3.
- campus area network (CAN). building-centric lan. covers several miles and different building. college campuses, business parks and military bases.
- metropolitan area network (MAN). connects locations scattered across the entire city. covers up to 25 miles.
- wide area network (WAN). connects geographically disparate internal networks. lease lines. virtual private networks. the internet is a wan. wan does not always have to be public.

### Understanding Network Geography

- examples of pan, lan and wan using his car.

### Wired Network Topology

- topology. arrangement of elements.
- physical or logical.
- physical topology. show how things are physically connected.
- logical topology. how the traffic is going to flow through the network. does not show the location of the device on the real world.
- point-to-point. involves a direct connection between 2 devices.
- ring. each device is connected to two other devices forming a circular data path.
  - fiber distributed data interface (FDDI). used to conduct data transmission on fiber optic. operates on a dual ring structure.
- bus topology. network devices are connected back to a central cable known as the bus. older tech and not commonly used.
- star. common network layout. each nodes connects to a centralized connection point.
- hub-and-spoke. variation of the star. a hub is connected to spokes. devices need to send data to hubs because they cannot make a point to point connection.
- mesh. point to point connection between every single device on the network.
  - full. every node is connected to every other node in the network.
  - partial. some nodes are organized in a full mesh scheme, while others are connected to some other nodes.

### Wireless Network Topology

- infrastructure mode. most common mode. wireless access point as a centralized point.
- ad-hoc mode. decentralized. peer-to-peer. does not require a router or access point.
- wireless mesh. interconnection of different types of nodes, devices, and radios. combines multiple technologies.

### Datacenter Topology

- datacenter. facility to organize process store and disseminate large amounts of data.
- three-tiered hierarchy.
  - core layer. 2 routers. backbone of the network.
  - distribution/aggregation layer. provides boundary definition.
  - access/edge layer. used to connect endpoint devices. regular switches.
- collapsed core. the core and distribution layers are merged into a single layer. this yields 2 layers. seen in smaller/medium sized data centers. not suitable for larger/complex networks.
- spine and leaf arch. alternative type used for communication within the datacenter itself.
  - leaf. access switches.
  - spine. network core. connects switches in a full mesh topology.
  - "top of rack switching."
  - spine and leaf arch can be used in combination with the three-tiered arch
- traffic flows.
  - north-south. traffic enters and leaves the data center. north. leaving dc. south. entering dc.
  - east-west. refers to data flow within a datacenter. 

## Section 3: OSI Model

### OSI Model

- open systems interconnection (OSI) model. developed in 1977 by the international organization for standardization (ISO).
- osi stack = osi model = osi reference model.
- 7 layers
- reference model. used to categorize functions of a network.
- networks today operate under the tcp/ip model.
- please do not throw sausage pizza away. <- use this mnemonic to remember the order of the OSI model.
- data exists in level 5, 6 and 7.
- layer 4, segment
- layer 3, packet
- layer 2, frame
- layer 1, bits
- do some people fear birthdays? mnemonic to remember the name of "data" as it is going down the osi model.

### Layer 1 (Physical)

- bits are transmitted across the network. includes physical and electrical network characteristics.
- transition modulation. one level represents 1 and one level represents 0.
- cables are also part of the physical layer
- synchronizing comms.
  - asynchronous. uses start and stop bits to indicate when tx occurs from the sender to the receiver.
  - synchronous. uses a reference clock to coordinate the transmissions by both sender and receiver.
- broadband. divides bandwidth into separate channels.
- baseband. uses all available frequencies on the medium all the time. uses a reference clock.
- time-division multiplexing (TDM). each session takes a turn to use bandwidth.
- statistical time-division multiplexing (statTDM). takes turns based on necessity.
- frequency-division multiplexing (FDM). divides the medium into channels based on frequencies.
- multiplexing takes limited amount of resources for more efficient utilization.
- layer 1 devices. cables (fiber optic, coaxial, ethernet). bluetooth. wifi. hubs. access points. media converters.
- layer 1 devices are repeaters, passing along whatever is received.
- layer 1 devices view the network physically.

### Layer 2 (Data Link)

- package bits into frames.
- media access control (mac). physical addressing system of a device.
- 48-bit physical addressing system
- first 24 bits identify the vendor of the device.
- second 24 bits identify the machine it belongs to.
- layer 2 devices view networks logically.
- logical link control (LLC). basic form of flow control. 
- llc provides basic error control functions.
- synchronization
  - isochronous. uses a common ref clock source and create time slots for tx.
  - synchronous. network devices agree on clocking. can use control characters.
  - asynchronous. each network devices reference internal clocks and use start and stop bits for synchronization.
    
### Layer 3 (Network)

- routing = layer 3 switching.
- IP is a routing protocol.
- two types. IPv4 and IPv6.
- 3 ways to send data
  - packet switching. data is divided into packets and then forwarded. can take different paths to get to the end. does not store the data like message switching.
  - circuit switching. dedicated comm link between two devices.
  - message switching. data is divided into messages which may be stored and forwarded.
- route discovery and selection. manually configured as a static route or dynamically through a routing protocol.
- connection services. augment layer 2 connection services and improve reliability.
- internet control message protocol (ICMP). sends error messages and operational info to an IP address
- layer 3 things. routers. multilayer switches. IPv4. IPv6. ICMP.

### Layer 4 (Transport)

- dividing line of the higher levels and the lower layers of the OSI model
- data type = segments/datagrams.
- TCP/UDP protocols.
- transmission control protocol (TCP). connection oriented protocol. reliable. connectionful protocol.
- three-way handshake. syn -> syn-ack -> ack
- user datagram protocol (UDP). connectionless. unreliable. it has less overhead than tcp.
- tcp uses segments. udp uses datagrams.
- tcp is...
  - reliable
  - connection oriented
  - segment retransmission and flow control through windowing
  - segment sequencing
  - acknowledges segments
- udp is...
  - unreliable
  - connectionless
  - no windowing or retransmission
  - no sequencing
  - no acknowledgment
- windowing. allows the clients adjust data in each segment.
- buffering. occurs when devices allocate memory to store segments if bandwidth is not readily available.
- example devices. wan accelerators. load balancers and firewalls.
  
### Layer 5 (Session)

- keeps conversations separate to prevent intermingling of data
- set up session. check user credentials and assign a number to identify it.
- maintain session.
  - transfer data
  - reestablish connection
  - acknowledge receipt of data
- tear down session. ending session after the transfer is done or when the other party disconnects.
- examples. H.233. netbios.
- H.323. video calls.
  - real-time transport protocol (RTP). streaming audio/video
- netbios. used to share files over a network.

### Layer 6 (Presentation)

- formats data to be exchanged and secure the data with encryption.
- data formatting. data is formatted by the computer to have compatibility between different devices.
  - american standard code for information interchange (ASCII). text.
- encryption. scramble data in transit to keep it secure.
  - transport layer security (TLS)
- examples. scripting languages. standard text. pictures. movie files. encryption algos (TLS and SSL).

### Layer 7 (Application)

- provides application-level services where users communicate with the computer.
- file transfer/network transfer.
- application services. unites communicating components from more than one network application.
  - examples. pop3, imap, smtp.
- service advertisement. sending out announcements to other devices on the network to state the services they offer.
- examples. email apps (pop3, imap, smtp). web browsing apps (http, https). domain name service (dns). file transfer protocols (ftp, sftp). remote access (rdp). 

### Encapsulation and Decapsulation

- encapsulation. put headers and trailers around data.
- decapsulation. remove encapsulation.
- protocol data unit (PDU). single unit of information.
- example. L7 PDU = data.
- tcp header (20 bytes).
  - 10 mandatory fields.
  - ...
  - 6 control flags
    - syn. used to sync connection
    - ack. acknowledgment flag.
    - fin. tear down connection
    - rst. used when client or server receives a packet that it was not expecting during the current connection.
    - psh. ensure data is given priority. used by the sender.
    - urg. similar to push and identifies incoming data as urgent. sent to tell the recipient to prioritize.
- udp header (8 bytes)
  - 4 fields.
    - source port, destination port, length. checksum
- IP header
  - fields...
- Ethernet Header
  - destination mac address
  - source mac
  - ethertype. indicate which protocol is encapsulated.
  - vlan tag
- mac address. physical address used to identify a network card.
- maximum transmission unit (MTU).
- jumbo frame. frame > 1500 MTU
  
### Understanding the OSI Model

- wireshark. packet analyzer.

## Section 4: Ports and Protocols

### Ports and Protocols

- port. virtual entry/exit point for comms used by applications to exchange info
- protocol. set of rules for data exchange.

### Network Port Fundamentals

- port. logical opening that represents a service that is waiting for traffic.
- ports from 0 to 65,535
- 3 groups 1 well known 2 registered 3 ephemeral
- well known ports. 0 to 1,023.
- registered ports. 1,024 to 49,151
  - registered with internet assigned numbers authority (IANA)
- ephemeral ports. dynamic ports or private ports. 49,152 to 65,535.

### Transmission Control Protocol (TCP)

- is a fundamental protocol.
- acts on the transport layer
- ensure reliable tx of data
- 3-way handshake (syn syn-ack ack)
- uses sequence number and acknowledgment messages for assurance
- employs flow control using windowing
- windowing. receiver specifies amount of data it can receive.
- port. numerical identifier that helps distinguish between different services in the same endpoint.
- header is between 20 t0 60 bytes in size

### User Datagram Protocol (UDP)

- used for time-sensitive tx (examples: video or dns lookups.)
- packet loss is acceptable.
- low latency
- reduced processing overhead
- acts on the transport layer of the osi model
- no three-way handshake or windowing
- header is 8 bytes in size
- stateless. does not maintain the state of the connection.

### Internet Control Message Protocol (ICMP)

- not used to send data between systems
- used for diagnosing network comm issues
- acts on the network layer
- header.
  - type 1 byte
  - code 1 byte context
  - checksum 2 bytes error checking the message header and data
- icmp flood attack. overwhelm target with icmp packets (ping). creates a denial of service (DoS) condition.
- distributed denial of service (DDoS) attack. attacker uses a network of computers for the attack.
- ping of death. attacker sends malformed or oversized packets using the icmp protocol
  - maximum IP packet is 65,535. the attacker crafts a packet bigger than this.

### Web Ports and Protocols

- port 80. http. hypertext transfer protocol.
- port 443. https. hypertext transfer protocol secure.
- hypertext transfer protocol (http). application layer protocol that enables plain text comms between clients and servers.
- hypertext transfer protocol secure (HTTPS). encrypted http. uses ssl or tls.
- secure sockets layer (SSL).
- transport layer security (TLS). newer method.
- security and encryption. http is unencrypted. https is encrypted.
- default usage. 95% of web traffic is sent over 443.
- SEO and trust. most search engines prioritize https over http.

### Email Ports and Protocols

- simple mail transfer protocol (SMTP). only used for sending emails. port 25. data sent in plain text.
  - smtps is a secure variant of smtp. transports messages via an encrypted tunnel. ports 465 or 587.
- post office protocol version 3 (POP3). retrieve email. port 110. messages are only available on the machine you downloaded them. emails are transmitted in plain text.
  - pop3s (POP3 Secure). port 995.
- internet message access protocol (IMAP). port 143. manage emails directly on the server.
  - imaps (IMAP Secure). port 993.

### File Transfer Ports and Protocols

- file transfer protocol (ftp). ports 20 and 21.
  - port 20. data transfer
  - port 21. sending control command.
  - not encrypted.
- secure file transfer protocol (SFTP)
  - port 22
  - tunneling ftp protocol through an ssh connection.
- trivial file transfer protocol (TFTP). port 69.
  - designed for sending files when minimal security is sufficient
- server message block (SMB). port 445.
  - windows file sharing
  - windows computers communicate with each other
  - used inside local area networks. not used to send data across the internet.

### Remote Access Ports and Protocols

- manage systems and networks from across the internet
- secure shell (SSH). port 22.
- telnet. port 23. user on one computer login remotely to another computer. unencrypted.
- remote desktop protocol (RDP). proprietary protocol developed by MS. graphical user interface to connect to another computer. port 3389.
  - data encryption.
  - smart card auth.
  - bandwidth reduction mechanisms,

### Network Service Ports and Protocols

- domain name system (DNS). translate domain names to IP addresses. port 53. udp for small messages/ tcp for larger messages.
- dynamic host config protocol (DHCP). automate assignment of IP addresses. servers listen on port udp 67. clients will receive responses via port 68 udp.
- sql services. protocols ued by database servers. Microsoft sql port 1433. mysql port 3306.
- simple network management protocol (SNMP). collect info and configure network devices. port 161 (snmp managers) and 162 udp (used by agents).
- system logging (syslog). message logging to a centralized server. port 514 udp/tcp.

### Other Network Service Ports and Protocols

- network time protocol (NTP). used to synchronize the clocks of a computer over a given network. port 123 udp.
- session initiation protocol (SIP). voice, video and messaging. port 5060 udp/tcp and 5061 tcp (encrypted).
- lightweight directory access protocol (LDAP). protocol for accessing and maintaining distributed directory information. port 389 tcp/udp. unencrypted.
  - ldap over ssl (LDAPS). encrypted LDAP. port 636 tcp.

### Finding Open Ports

- nmap (network mapper)

## Section 5: Media and Cabling

### Media and Cabling Distributions

- media. physical material used to tx data. copper. fiber and radio freq.

### Copper Media

- default type of cable used in networks.
- ieee 802.3 standard. defines the physical layer and data link layer's media access control (MAC) for wired ethernet networks.
- twisted pair cable.
- twisted pair cable. wiring in which two conductors of a single circuit are twisted together.
  - preferred method for data and voice
  - unshielded twisted pair (UTP). composed of pairs of wires twisted together, w/o additional shielding being added to the cable.
    - lightweight.
    - flexible.
    - cost-effective.
  - shielded twisted pair (STP). designed with a layer of insulation or shielding.
    - more expensive.
    - bulkier
- cat 5. 100Mbps. 100 meters max. 100 MHz freq. 100 BASE-T (Fast Ethernet)
- cat 5e (category 5 enhanced). 1000 Mbps/1 Gbps. 100 meters max. 100 MHz freq. 1000 BASE-T (Gigabit Ethernet)
  - contains more twists as the cat 5.
- cat 6. 1 GBps. 100 meters max. 250 MHz freq.
  - 10 GBps. 55 meters or less. 10G BASE-T (10 Gigabit Ethernet)
  - 1 Gbps. 100 meters or less. 1000 BASE T (Gigabit Ethernet)
- cat 6a (category 6 augmented). 10 GBps. 100 meters max. 500 MHz freq. 10G BASE-T (10-Gigabit Ethernet)
- cat 7. 10 Gbps. 100 meters maximum. 600 MHz freq. 10G BASE-T (10-Gigabit Ethernet)
- cat 8. Up to 40 GBps. 30 meters maximum. 2000 MHz/2 GHz max.
- coaxial (coax) cable. single copper conductor with an insulating layer and a conductive shield wrapped around it.
  - rg-6. used to support faster internet speeds.
  - rg-59. older cables used in analog video and cctv installations.
  - can support speeds of 1 GBps up to 300 m
- direct attach copper (DAC). fixed assemply copper cabling used to connect switches to routers or servers.
  - active. 100 Gbps at 15 m or less.
  - passive. 10 Gbps at 7 meters or less.
- twinaxial cable. component of a DAC.
  - used for SFP+ and QSFP.
  - support 10 (100 m), 25, 40 or 100 GBps (7 m)
- plenum cables. designed with fire-retardant plastic jackets made from materials such as pvc or fep.
  - prevent flames from spreading.
  - reduces amount of smoke.
- non-plenum cables. not designed with fire-retardand properties.

### Copper Network Connections

- connectors vary depending on application
- registered jack (RJ-X). connecting voice and data equipment
  - RJ-11
  - RJ-45
- radio guide (RG-X). used w/ coaxial cables.
  - RG-6
  - RG-59
- rj-11. standard for telephone wiring.
  - 6-position 2-conductor (6P2C) configuration
  - ideal for telephone applications
  - not suitable fr high speed tx
- rj-45. connector for data networks that utilize copper cables to create ethernet network.
  - 8 position 8-conductor (8P8C) configuration
  - can support high speed tx
- f-type connector. standard for cable tv and sat connections.
  - screw on connector
  - rg-6. standard for coaxial cables
  - rg-59. older spec for coaxial cables that used to be common for tv and radio signal tx
- bayonet neill-concelman (BNC) connector. characterized by its secure bayonet locking mechanism.
  - push and twist connector
  - BNC also erroneously called british naval connector

### Building a Copper Cable

- straight through cable (patch cable). contains same pin outs on the other end of the cable.
- 568B. preferred for jacks inside buildings. straight through patch cables.
- data terminal equipment (DTE). endpoint devices. laptops. desktops, etc.
- data commuinications equipment (DCE). switch, modem, hub, etc.
- dte to dte/dce to dce use a crossover cable.
- crossover cable. swaps end and receive pins.
- a switch to a swtich connection requies a crossover cable.
- medium dependent interface crossover (MDIX). automated way to electronically simulate a crossover cable even if using a straigh-through patch cable
- assume a switch is an older device that does not support MDIX unless the exam question states otherwise
- <<need to know the pattern of colors to build out cables>>

### Fiber Media

- used to transmit data using light
- emi immunity
- extented data tx range
- higher data transfer speeds
- operates in 10 to 100 Gbps due to limitations of hardware (not the cable)
- cost and complexity are higher than copper
- single mode fiber (SMF). designed for long distance comms. 8.3 to 10 microns in diameter.
- multi mode fiber (MMF). short distances. larger core size. 50 to 100 microns in diameter.
  - cheaper to manufacture.
  - used in buildings, campuses, office parks.
- choose multi mode fiber for higher data rates over short distances, rather than using copper media
- smf has a yellow sheath.
- mmf has a aqua blue/orange sheath

### Fiber Network Connections

- single mode optical connector st type
- subscriber connector (SC) (stick and click connector). known for square shape and push pull design
- lucent connector (LC) (love connector). push pull mechanism similar to the SCE but in a much smaller form factor
- straight tip connector (ST) (stick and twist connector). round shapre and twick-lock
  - common used with multi-mode fiber optic cables and applications.
  - suitable for outside applications
  - easy installation
- mechanical transfer registered jack (MTRJ). small, rectangular design... dual fiber connection.
  - compact.
- multi fiber push on connector (MPO). multiple fibers in a single connector.
- physical contact (PC). slight curvature. lowe back reflection. digital and telephone services. least effective reduction in back reflection.
- ultra physical contact (UPC). dome shaped. updated and better version of PC.
- angled physical contact (APC). 8 degree angle. long haul fiber installations.

### Transceivers

- any device that can transmit and receive data
- protocol. set of rules and standards that govern how data is transmitted.
- ethernet. family of computer networking technologies.
- fibre channel (FC). high speed network tech used to connect computer data storage to servers in storage area networks
- transceiver can translate data between protocols/types of connections
- media converters and transceivers are considered layer 1 devices
  - copper to fiber
  - fiber to copper
  - etc.
- small form factor plugabble (SFP). 4.25 Gbps
- small form factor plugabble plus (sfp+) 16 Gbps
- quad small form factor pluggable (QSFP) 40 Gbps
- quad small form factor pluggable plus (QSFP+) 41.2 Gbps
- quad small form factor pluggable 28 (QSFP28) 100 Gbps
- quad small form factor pluggable 56 (QSFP56) 200 Gbps
- QSFP are faster than SFP modules

## Section 6: Distribution Systems

### Distribution Systems

- cable distribution system. structure layout and organization of cables.

### Cable Distribution System

- organized system to connect network backbones all the way to the user
- demarcation point. internet provider ends and network infra and cabling begin.
- main distribution frame (MDF). main starting point for all interior cabling.
- intermediate distribution frame (IDF). sits in between the mdf and the user
- backbone switch everything connects back into it.
- cable tray. rigid structural system to secure cables.
  - horizontal. drop ceiling/under a raised floor.
  - vertical. vertical cross-connect.
- rakcs. designed to hold various devices.
- 2 post rack. two vertical posts.
- 4 post rack. four vertical posts. heavier equipment.
- wall mounted rack. smaller network equipment. for limited floor space.
- full cabinet rack. rack enclosure. secure environment. includes a door.
- patch panel. used to keep data center/server room organized.
  - front side - network jacks
  - back side - 110 punchdown block
- 110 block - punchdown block for voice and data applications that depends on CAT5.
- always connect the wall jack's cable to a patch panel
- fibe distribution panel. uses fiber connectors. no punchdown in the back.
  - front and back have the same type of connection.
  - can server as converters from one type of fiber connector to another

### Wiring a Network

- <<demo on wiring>>
- from switch > patch panel > punchdown > keystone (rj45 connector)

### Testing a Network

- <<demo of a wire testing device>>
- fox and a hound. toner probe. this helps to find which ports are tied to a patch panel. identify and document the network.
  
### Power Distribution Systems

- ensure consistent and reliable power delivery for equipment
- uninterruptible power supply (UPS). provides emergency power when main power fails. also provides line conditioning. provides with clean and reliable power. short duration (15 - 30 mins).
- power distribution unit (PDU). distributes power to network components. advanced power strips. provide power protection from surges, spikes, etc. but does not provide emergency power like a UPS.
- generator. installed outside data centers. provide longer term power during an outage.
- managing power load. prevents ckt overload and ensures efficient power usage.
- voltage. electric potential difference.

### Heating, Ventilation, and Air Conditioning (HVAC)

- Heating, Ventilation, and Air Conditioning (HVAC). provides temp control, humdity control and ventilation.
- temperature control. keep steady temps 66-77 F (20-25 C).
- humidity. too much humidity can cause condensation. too little humidity can cause static electrical charges. (keep it between 40 to 60%)
- airflow management.
  - port-side exhaust and intake. method of air distribution in which server racks are positioned in alternating rows with a cold and hot air aisle.
    
### Fire Supression Systems

- Wet pipe systems. most basic type of fire supression. sprinklers. avoid using in/around data centers.
- pre-action systems. helps minimize risk of release when using a wet pipe system.
- special supression systems. utilizes a clean agent as part of its supression system. the clean agent removes the oxygen in the room and thus suffocates the fire.
  - equipped with an alarm
  - has supplemental oxygen available

## Section 7: Wireless Networks

### Wireless Networks

- summary of the section.

### Wireless Network Types

- ad hoc/independent basic service set (IBSS). devices connect directly to each other rather than through a cnetral access point. peer to peer network. quick and temp networks. does not provide internet access. use for file sharing.
- infrastructure. devices are connected to a network through a wireless AP.
  - basic service set identifier (BSSID). set to the mac address of the wireless access point.
  - service set identifier (SSID). alphanumeric network name.
  - extended service set (ESS). creates a larger network that shares the same SSID to allow for seamless connectivity across a building.
- point to point. connect two distinct locations over a long distance using a high-gain antenna.
  - highly efficient.
- mesh. each node connects to multiple other nodes in the network.
  - self healing
  - large scale deployments
  - 2 types of mesh networks
    - 1 use ESS config in a wireless network that operates in infra mode
    - 2 involves multiple different types of wireless networks all operating together to provide servies to end users.
- autonomous access point. standalone device that contains all of the intelligence to handle wireless networking functions independently. think about the router at home.
- lightweight access points. multiple access points connecting back to a centralized controller.

### Wireless Antennas

- wireless antenna. send and receive signals.
- omnidirectional. transmists and receives wireless signals in all directions equally. default types of antennas in wireless APs and others.
- unidirectional. focuses on a single direction. suitable for long and narrow coverage areas.
- yagi. directional antenna that can provide high signal gains and uses a narrow beamwidth.
  - long distance areas.
  - this is a type of unidirectional antenna.

### Understanding Antennas

- <<demo of antennas>>
- parabolic antenna. special type of unidirectional antenna. curved dish. used w/ microwave signals and satelitte tv signals.

### Wireless Frequencies

- wireless frequencies. freq bands that are used to transmit and receive the radio waves used by the wireless networks to send data.
- 2.4GHz Band. widely used freqs. has been in use since 1997. good penetration. 2.400 to 2.495 GHz.
  - channel 11, 13 or 14.
- channel. physical medium through which the wireless networks can send and receive data.
  - only channels that don't overlap: 1, 6 and 11
  - US and Canada: 1 - 11
  - Japan: 1 - 14
  - Rest of the world: 1 - 13
- 5 GHz Band. 5.725 GHz - 5.875 GHz
  - 24 non overlapping channels of 20 MHz per channel
  - channel bonding. creates wider channel by merging two or more neighboring channels.
- 6 GHz Band
  - offers more channels and bandwidth, etc.
  - 5.925 to 7.125 GHz
- 802.11h standard -> comply with european regulations
- dynamic frequency selection. requiresd devices to actively monitor the environm,ent for radar systems
- transmit power control. allows devices to adjust their tx power to the minimum required for mainting a good quality connection.
- band steering. optimize distribution the client devices across different...

### 802.11 Standards

- wireless lan
- wireless a 5 GHz 54 Mbps 35 meters. was expensive.
- wireless b 2.4 GHz 11 Mbps 140 meters. affordable. widespread adoption.
- wireless g 2.4 GHz 54 Mbps 140 meters.
- wireless n 5 GHz (WiFi 4) 600 Mbps 35 meters.
  - 2.4 GHz 300 Mbps 70 meters
  - mimo. multiple input multiple output.
    - hub
- wireless ac (WiFi 5) 5 GHz 6.9 Gbps
  - mu-mimo. multiple user mimo
    - multipat wireless comm tech
    - switch.
- wireless ax (WiFi 6 and WiFi 6e) 2.4, 5 and 6 GHz 9.6 Gbps

### Wireless Security

- pre shared key (PSK). password.
  - scalability becomes a problem.
- 802.1x. enterprise authentication method.
- wired equivalent privacy (WEP). original 802.11 wireless security standard. not secure. depends on RC4.
  - uses a 24-bit initialization vector (IV)
- wifi protected access (WPA). WEP replacement. uses TKIP.
  - TKIP is weak and be cracked.
  - relies on RC4
  - message integrity check (MIC). hash data before sent over the network.
  - enterprise mode
- wifi protected access 2 (WPA2). 802.11i. wireless g, wireless n, wireless a, wireless ac
  - relies on ccmp
  - relies on aes.
  - personal mode. pre shared key.
  - enterprise mode. centralized authentication.
- wifi protected access 3 (WPA3).
  - simultaneous authentication of equals (SAE). enhanced handhsake process used in wifi authentication.
  - offers forward secrecy. past comms are protected.
- wifi protected setup (WPS). net sec standard aimed at simplifying the setup of a secure wifi connection.
  - vulnerable to bruteforce attack
  - uses an 8 digit pin

### Undetrstanding Wireless Security

- <<demo of setting up a wireless router>>
- use wpa2 
- disable SSID broadcast
- enable wireless isolation
- enable mac filtering
- disable wps setting

### When Wireless Security Fails

- <<attack on a WEP-enabled access point>>

### Captive Portals

- captive portal. web pages to newly connected users to a wifi network. used heavily in public networks.
  - used for authentication, policy acceptance and data collection.
  
## Section 8: Ethernet Switching

### Ethernet Switching

- summary of the section.

### Ethernet Fundamentals

- 10Base2 - thin net (old. not relevant for the exam.)
- 10Base5 - thick net (old. not relevant for the exam.)
- 10Baste-T Ethernet - 10Mbps over CAT3. 100 meters.
- deterministic network - network access is organized
- contention based network - used to determine who gets to access and communicate. collisions can occur.
- ethernet is a contention-based networking protocol
- csma/cd - carrier sense multiple access with collision detection
- cs carrier sensing - listen to the network
- carrier. signal that carriers info or data
- multiple access ma - different devices that have access to the network at the same time
- collision detection cd
- random backoff timer. allows devices to retransmit again when a timer reaches zero.
- collision domain. area of the network that shares a single segment.
  - keep collision domains small insider networks.
- ethernet switch. increase scalability of network.
- use switches instead of hubs.
  - each port is its own collision domain.

### Network Devices

- hub. layer 1 device. connect multiple network devices together. square icon with arrow pointed bothways. multi port repeaters.
  - passive. repeat the signal w/ no amplification.
  - active. repeats signal with amplification. overcomes the limit of 100m ot eh twisted pair cables.
  - smart. active hub with features like snmp.
- collision domains. multiple network segments connected together by hubs.
- bridge. analyzes source mac addresses and forwards based on the destination mac on the frames
  - the bridge can go/goes in between the hubs.
- switch. multiport bridge. layer 2 device that connects multiple network segments together.
  - it like a hub with a bridge after every port.
- broadcast domain. "area" where an ARP request goes.
- router. layer 3 devices that connect multiple networks and makes forwarding decisions based on logical network info.
- routers can separate broadcast domains.
  - helps reduce traffic and noise.
- layer 3 switch. makes layer 3 routing decisions and interconnects entire networks. not just network segments.
  - each port is its own broadcast domain and its own collision domain.

### Understanding Network Devices

- <<demo of network devices>>

### Virtual Local Area Network (VLAN)

- vlan. logical sub division of a network segment.
- switch is configured to utilize a vlan
- enhanced security. isolate sensitive data.
- improved performance. reducing the size of a broadcast domain.
- increased management. easier to implement policy changes and troubleshoot issues.
- improved cost efficiency.
- switch virtual interface (SVI). allows switching to route traffic between different vlans w/o requiring a separate router.

### VLAN Configuration

- 802.1q tagging. ieee standard that facilitate the management of multiple vlans in a single network.
- trunking. transmission of traffic from different vlans across the same physical network infrastructure, while keeping traffic from each vlan separate and secure.
- native (default) vlan. the one vlan on a trunk port that does not get tagged with a vlan identifier when frames are passed over a trunk link.
  - rename the default vlan to something other than vlan 1
- voice vlan. vlan dedicared to voip traffic.
- link aggregation. port channeling or bonding. method used in networks to combine multiple network connections into a single, logical link.
  - this aggregation adds bandwith availability. (i.e 4 x 1 Gbps ports = 4 Gbps)
- speed and duplex configurations. determine rate at which data can be transmitted.
- speed. rate of data transfer.
- duplex. how data is sent.
- half duplex - data tx and reception cannot occur at the same time.
- full duplex. data can be sent and received at the same time.
- auto negotiation.

### Understanding VLANs

- <<demo of how to configure a vlan using a unifi dream wall>>

### Spanning Tree Protocol (STP)

- spanning tree protocol (STP) (802.1d). permits redundant links between switches and prevents looping of network traffic.
- broadcast storm. multiple copies of frames being forwarded back and forth which then consumes the network.
- root bridge. switch with the lowest bridge id (BID).
  - BID is made up of a priority value and a mac address.
- non-root bridge. every other switch in the topology.
- root port. every non-root bridge has a single root port which is the closes to the root bridge in terms of cost.
  - faster cables have a lowe cost. slower cables have a higher cost.
- designated port. every network segment has a designated port which is the closest to the root bridge in terms of cost.
  - all ports on the root bridge are designated ports.
- non-designated port. ports that block traffic to create loop-free topoloigy.
  - receive bridge protocol data units (BPDUs).
- the switch goes thorugh four stages 1 blocking 2 listening 3 learning 4 forwarding
- blocking. bpdus are received but not forwarded.
- listening. populates the mac address table but does not forward frames.
- learning. process bdpus and this is where switch dtermines its role in the spanning tree.
- forwarding. forwards frames for operations.
- link cost. associated with the speed of the link - the lower the link's speed, the higher the cost.

### Network Access Control (NAC)

- network access control (NAC). inspect devices as they try to connect to a network.
- port security. securing physical network ports.
- mac filtering. controls access by device's mac address.
- 802.1x authentication. authentication framework for networks.
  - extensible authentication protocol (EAP).
  - supplicant
  - authenticator
  - authentication server. radius.
- time-based access control.
- location-based access control.
- role-based access control. enforces principle of least privilege.
- rule-based access control.

### Maximum Transmission Unit (MTU)

- mtu. largest size of a frame.
- measued in bytes.
- maximum load capacity of frames.
- mtu too high. packet loss.
- mtu too low. increased overhead.
- smaller mtu size is used in wireless networks than ethernet.
- vpn. smaller mtu size.
- pppoe. smaller mtu size.
- jumbo frames. any frame that exceeds the default of 1500 bytes.

## Section 9: IP Addressing

### IP Addressing

- internet protocol (IP) address. numerical label used to id internet communicating devices in a network.

### IPv4 Addressing

- internet protocol version 4.
- dotted-decimal notation.
- each section is an octet. (8 bits)
- 32 bits of addressable space
- network portion and host portion of the address.
- subnet mask. the ones define the network portion of the address and the zeros define the host portion of the address
- 5 classes - a,b,c,d,e
- a -> default subnet mask -> 255.0.0.0
- b -> default subnet mask -> 255.255.0.0
- c -> default subnet mask -> 255.255.255.0
- d -> no subnet mask assigned. reserved for multicast routing.
- multicast address. logical identifier for a group
- e -> no subnest mask assigned. reserved for experimental purposes.
- subnetting. taking a larger network portion and subdividing it.
- classful mask. default subnet mask. (ex. 255.255.255.0)
- classless mask. borrow some of the host bits from an ipv4 address. (ex. 255.255.255.192)
- cidr. classless inter-domain routing domain. 
- cidr notation. x.x.x.x/y (192.168.1.4/24)

### IPv4 Address Types

- public (routable). unique ip address that allows it to communicate with other devices on the internet.
- internet corp for assigned names and numbers (ICANN). manages and leases publicly routable ip addresses.
  - arin (north america)
  - lacnic (latin america)
  - afnic (africa)
  - apnic (asia pacific)
  - ripe (europe)
- private (non-routable). used within local networks for comms between devices within a network w/o using public ip address.
- private ip ranges.
- network address translation (NAT). method used in networking tha allows a single device to act as an agent between the internet and the private network.
- request for comments (RFC). publication from the (IETF)
  - RFC1918.
    - 10.0.0.0/24
    - 172.16.0.0 - 172.31.0.0
    - 192.168.0.0/16
- loopback address (localhost). specialized ip address assigned as 127.0.0.1
  - creates a loopback to the host
  - used for troubleshooting and testing network protocol software
- automatic private ip addresses (APIPA). addresses that are assigned by the os when the network's dhcp server is unavailable and an ip address has not been statically assigned by the system (169.254.0.0/16).
- dhcp process. DORA.
  - discover.
  - offer.
  - request.
  - acknowledge.

### IPv4 Data Flows

- unicast. single src to single dest.
- multicast. single src to multiple specific destinations.
- broadcast. single source to all dests.

### Assigning IPv4 Addresses

- static assignment. manually type ip address for the host, subnet, default gateway and dns(or wins).
- dynamic assignment. dynamic allocation of ip.
- domain name system (DNS). lookup ip address given a domain name.
- windows internet name service (WINS). identifies netbios systems on a tcp/ip net. its like dns but for a windows environment.
- bootstrap protocol (BOOTP). dynamically assigns ip and allows workstation to load a copy of the boot image.
- dynamic host control protocol (DHCP). assigns ip based on a scope.
- automatic private ip addressing (APIPA). used when a device does not have a static ip address or cannot reach a dhcp server. allows for a quick config of a network w/o a dhcp server. can't be routed outside of the local network.
- zero configuration (ZeroConf). based on apipa. resolves computer names w/o the need of dns using mdns. perform service discovery on a network.
  - apple bonjour
  - windows link local multicast name resolution (LLMNR)
  - linux SystemD

### Computer Mathematics

- 

### Subnetting

### Subnetting Practice

### Subnetting by Hand

### IPv6 Addressing

### IPv6 Data Flows

### IPv4 and IPv6 Compatibility Requirements

## Section 10:
## Section 11:
## Section 12:
## Section 13:
## Section 14:
## Section 15:
## Section 16:
## Section 17:
## Section 18:
## Section 19:
## Section 20:
## Section 21:
## Section 22:
## Section 23:
## Section 24:
## Section 25:
## Section 26:
## Section 27:
## Section 28:
## Section 29:

<!--  LocalWords:  pbqs balancers NAS ethernet centric lan FDDI OSI
<!--  LocalWords:  Datacenter datacenter osi tx baseband TDM statTDM
<!--  LocalWords:  FDM LLC llc isochronous IPv multilayer datagrams
<!--  LocalWords:  connectionful ack retransmission RTP american sftp
<!--  LocalWords:  Decapsulation decapsulation PDU rst psh urg DDoS
<!--  LocalWords:  ethertype wireshark lookups oversized unencrypted
<!--  LocalWords:  SEO DHCP ued mysql NTP unshielded UTP STP Mbps rg
<!--  LocalWords:  Gbps GBps
 -->
 -->
 -->
 -->
 -->
 -->
 -->
 -->
