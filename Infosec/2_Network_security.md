## Protocol
### 3 Elements
- Syntax
	- the format and structure
- Semantics
	- pre-defined rules for the data (format)
- Timing
	- what after what

### Functions
- Addressing
- Sequence control
	- Only for connection-oriented protocols. (e.g. TCP)
- Fragmentation & Reassembly
	- For big file transfer.
- Encapsulation
- Connection control
	- Connecting and Disconnecting
- Flow control
- Error control
	- Finding SDU, PCI error
- Synchronization
- Multiplexing
- 전송 서비스


## OSI Layer
Check Obsidian_Vault

### Layer 1
- Hardwares
	- Repeater
		- hardware to amplify signals.
		- Now, all network hardware includes it as a function.
	- (dummy) Hub
		- Old form of the Switch
		- Copy and send a packet to every clients
		- Modern Hub is called **Switching Hub**
		- (Switch sends a packet only to the destination client.)

### Layer 2
- MAC address
- Protocols
	- ethernet
	- X.25
	- frame relay
	- ATM
- Hardwares
	- Bridge
		- Early days device to connect LAN and LAN
	- Switch
		-  How it works
			- Cut-through vs Store & forward
			- Intelligent switching
				- Cut-through until error occurs and Store & forward activates.
			- Uses Switch table that stores MAC address and corresponding ports.

### Layer 3
- Network address + Host address (32-bit)
- IPv6 (128-bit)
- Protocols
	- ARP
		- Ask MAC address to certain IP address
	- RARP
	- IP
	- ICMP
		- ping
	- IGMP
		- multicast
- Hardwares
	- Router (gateway)
		- Routing table 
			- Stores the location of routers based on their IP addresses.
			- Used to find best route for a packet.
			- Columns
				- Network Destination
				- Netmask
				- Gateway
					- Next hop
					- next IP address to which the packet is forwarded
				- Interface
					- Outgoing interface that connect to the destination(Gateway)
				- Metric
					- Assigned value to choose optimal routes.
					- Number of hops to be crossed to get to the destinastion network.
			- `route PRINT`
			- `tracert [ip_address]`
				- Send ICMP packet
		- Routing Types
			- Static
			- Dynamic

### Layer 4
- Uses **Port**
- Protocols
	- TCP
	- UDP

### Layer 7
- Protocols
	- FTP
	- Telnet
	- SMTP
	- DNS
	- TFTP
	- HTTP
	- ...