 Wireshark Network Capture Report
________________________________________
1. Installation
Tool Used: Wireshark
Platform: Linux
Wireshark was installed and configured successfully. The user was granted the necessary permissions to capture packets without requiring root access.
________________________________________
2. Capture Setup
•	Interface Used: wlan0
•	Capture Duration: Approximately 1 minute
•	Tool: Wireshark GUI
________________________________________
3. Traffic Generation
To generate traffic during the capture:
•	Opened a web browser and visited: https://www.example.com
•	Executed a ping command to simulate ICMP traffic:
ping -c 5 google.com
________________________________________
4. Capture Termination
The capture was stopped manually after about 1 minute using the stop button in Wireshark.
Approximate Packet Count: [e.g., 2,000 – fill in based on your actual result]
________________________________________
5. Protocol Filtering
Protocol-specific filters were applied using Wireshark's filter bar to analyze various types of traffic:
•	DNS – to observe name resolution
•	TCP – to inspect connection setup and data exchange
•	ICMP – to analyze ping-related traffic
•	(Optionally: http, tls, or arp if present)
________________________________________
6. Identified Protocols
The following network protocols were observed:
Protocol	Description
DNS	Used for resolving domain names (e.g., www.google.com)
TCP	Handles reliable data transmission and session setup
ICMP	Used by ping for network diagnostics
________________________________________
7. Analysis Summary
Example Packet Details
Packet #1 – DNS Request
•	Source: 10.0.2.15
•	Destination: 172.217.174.78
•	Info: Standard query A www.google.com
•	Protocol: DNS
________________________________________
Packet #2 – TCP Handshake
•	Source: 10.0.2.15
•	Destination: 172.217.174.78
•	Info: SYN → SYN-ACK → ACK
•	Protocol: TCP
________________________________________
Packet #3 – ICMP Echo Request
•	Source: 10.0.2.15
•	Destination: 172.217.174.78
•	Info: Echo (ping) request
•	Protocol: ICMP
________________________________________
Conclusion
Wireshark successfully captured and analyzed real-time traffic during a live browsing and ping session. The capture revealed a variety of network protocols and demonstrated the tool’s ability to dissect packet-level details effectively.
________________________________________
