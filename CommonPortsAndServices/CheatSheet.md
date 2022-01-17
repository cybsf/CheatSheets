
A list of common ports with their respective services, transport protocol and a brief description.


# Common Ports And Services

| Port Number | Service name 		| Transport protocol | Description																	|
| :---------: | :---------------------: | :----------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------	|
| 7 	      | Echo 	     		| TCP/UDP      	     | Server echo the host input. Can also be used for relaying ICMP datagrams										|
| 19	      | Chargen	     		| TCP/UDP	     | Source of byte-stream for debugging/ payload for bandwith measurement										|
| **20**      | **FTP-transfer**        | **TCP**            | **File Transfer Protocol: Used to tranfser files**      												|
| **21**      | **FTP-connection**      | **TCP**	     | **File Transfer Protocol: Used to establish connection before file transfer**									|
| **22**      | **SSH** 		| **TCP**	     | **Secure Shell: Secure way to access a computer over the network 										|
| 22  	      | SCP 		        | TCP    	     | Secure Copy Protocol: Secure way to transfer files between devices           	                                                                |
| **22**      | **SFTP**        	| **TCP**            | **SSH File Tranfser Protocol: Secure way to transfer files between devices**    	                                                                |
| **23**      | **Telnet**   		| **TCP**            | **Insecure way to access a computer over the network**												| 
| **25**      | **SMTP**     		| **TCP**	     | **Simple Mail Transfer Protocol: Send Mail To People**												|
| 42          | WINS Replication	| TCP	             | Windows Internet Naming Service: Used in mapping NetBIOS names to IP addresses  									|
| 43          | WHOIS        	        | TCP                | Port used by the command line program WHOIS to send queries 											|
| 49          | TACACS      		| TCP/UDP            | Terminal Access Controller Access-Control System: Family of protocols handling remote authentication and related services			|
| **53**      | **DNS**       		| **TCP/UDP**        | **Domain Name System: IP mapping to domain names. UDP mostly for queries and TCP mostly for zone tranfsers**					|
| **67-68**   | **DHCP**		| **UDP**	     | **Domain Host Configuration Protocol: Dynamic network configuration for devices inside a LAN**							|
| 67-68       | BOOTP      	        | TCP                | Bootstrap Protocol: Provides devices with an IP from a configuration server                                                                      |
| **69**      | **TFTP**      		| **UDP**  	     | **Trivial File Transfer Protocol: Used for transferring files inside a LAN instead of the internet**						|
| 70          | Gopher        		| TCP                | Designed for distributing, searching and retrieving documents in IP networks (biggest rival of HTTP in the early years)				|
| 79          | Finger        		| TCP                | Designed for exchanging human-oriented status and user information (status updates from users in a LAN						|
| **80**      | **HTTP**       	        | **TCP/UDP**        | **Hypertext Transfer Protocol: application layer protocol in the IP suite model for distributed, collaborative, hypermedia information systems	|
| 88          | Kerberos                | UDP                | Kerberos is a protocol designed for authentication and security for client/server applications							|
| 102         | MS Exchange             | TCP                | Port used by Microsoft Exchange to communicate with other Message Transfer Agent									|
| **110**     | **POP3**                | **TCP**            | **Post Office Protocol: Used to retrieve mails from a mailserver**										|
| 113         | Ident                   | TCP                | Used for user authentication ex. when you try to use a mailserver, the mailserver will first authenticate through port 113 Identd service	|
| 119         | NNTP	                | TCP                | News Network Transfer Protocol: Used for transporting usenet news articles between news server							|
| **123**     | **NTP**                 | **UDP**            | Network Time Protocol: Used for clock synchronization between computers 										|
| 135         | Microsoft RPC           | UDP                | Microsoft Remote Prodecure Call:	Service that allows other systems to discover what servics are advertised on a machine and on which port	|
| 137	      | NetBIOS Name Service    | UDP                | Network Basic Input/Output System: Name registration and resolution                                                                              |
| 138	      | NetBIOS Datagram Service| UDP 	             | Network Basic Input/Output System: Destribution service for connectionless communications                                                        |
| 139	      | NetBIOS Session Service | TCP                | Network Basic Input/Output System: Session service for connection-oriented communications							|
| **143**     | **IMAP4**               |                    |																			|
| **161-162** | **SNMP**                |                    |																			|
| 177         | XDMCP	                |                    |																			|
| 179         | BGP	                |                    |																			|
| 201         | AppleTalk               |                    |																			|
| 264         | BGMP	                |                    |																			|
| 318         | TSP	                |                    |																			|
| 381-383     | HP Openview             |                    |																			|
| **389**     | **LDAP**                |                    |																			|
| **411-412** | **Direct Connect**      |                    |																			|
| **443**     | **HTTPS**	        |                    |																			|
| 445         | Microsft DS             |                    |																			|
| 464         | Kerberos                |                    |																			|
| **465**     | **SMTPS**               |                    |																			|
| 497         | Retrospect              |                    |																			|
| **500**     | **ISAKMP**              |                    |																			|
| 512         | rexec  	                |                    |																			|
| 514         | syslog	                |                    |																			|
| 515         | LPD/LPR	                |                    |																			|
| 520         | RIP	                |                    |																			|
| 521         | RIPng (IPv6)            |                    |																			|
| 540         | UUCP                    |                    |																			|
