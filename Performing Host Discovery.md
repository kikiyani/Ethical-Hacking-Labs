                                                             Task l: Perform Host Discovery using Nmap

Performing the ARP ping scan we get host is up which means that we can send ARP requests to the host:

<img width="605" height="127" alt="image" src="https://github.com/user-attachments/assets/4ebba851-7e49-4bd7-86c0-bf6df6e8b19a" />

Next, we do UDP ping scan which shows host is up as well, which means our UDP packets can reach the host

<img width="570" height="126" alt="image" src="https://github.com/user-attachments/assets/52d81732-5506-4d7b-91c7-20f563083a47" />

ICMP ping scan sends ICMP echo packets to our target host and if the host gets them and is up the following results are shown:

<img width="556" height="132" alt="image" src="https://github.com/user-attachments/assets/9f6fb31c-3838-491b-8ab1-b8d1b0815755" />

The ICMP ECHO ping sweep is used to determine the live hosts from a range of IP addresses by sending ICMP ECHO requests to multiple hosts.

<img width="624" height="135" alt="image" src="https://github.com/user-attachments/assets/ccbabad1-1ef5-4b91-a95a-c322c25f5bc9" />

ICMP timestamp ping, here the attackers query a timestamp message to acquire the information related to the current time from the target host machine.

<img width="624" height="173" alt="image" src="https://github.com/user-attachments/assets/02ef3b17-8396-4cd3-808c-fec47233081d" />

ICMP Address Mask Ping Scan, alternative for ICMP echo ping, used when the administrators block the normal PING:

<img width="624" height="169" alt="image" src="https://github.com/user-attachments/assets/da08642b-f319-473e-aeba-f4e7ec1ecc56" />

TCP SYN Ping Scan: This technique sends empty TCP SYN packets to the target host, ACK response means that the host is active:

<img width="624" height="140" alt="image" src="https://github.com/user-attachments/assets/b219cabb-9e9d-48b0-8c6b-73bc1dc5f05e" />

TCP ACK Ping Scan: This technique sends empty TCP ACK packets to the target host; an RST response means that the host is active:

<img width="624" height="169" alt="image" src="https://github.com/user-attachments/assets/dadfd04e-d8de-4b35-a182-88756fbbb197" />

IP Protocol Ping Scan: This technique sends different probe packets of different IP protocols to the target host, any response from any probe indicates that a host is active:
<img width="624" height="120" alt="image" src="https://github.com/user-attachments/assets/13b6fbbb-c41f-49b2-bef5-eb70488ccfaf" />

                                                           
                                                             
