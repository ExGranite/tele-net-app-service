# TELE NET APP SERVICE

This is a project done in completion to the Computer Networks course.

Software Used for Simulation: [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer)

### Topology:

<p><img src="https://github.com/ExGranite/tele-net-app-service/blob/main/Topology.png"></p>

### Number of Hosts:

- DHAKA - 1000
- KHULNA - 480
- CHITTAGONG - 230
- RANGPUR - 55
- RAJSHAHI - 330
- SYLHET - 175

The number of hosts for each branch can be doubled. Hence extra room for extra IP addresses were left.

### Features:

- Separate network for each branch
- Khulna-Chittagong and Chittagong-Rangpur connected with each other more securely than other networks
- Rajshahi and Chittagong connected without human intervention
- Dhaka works as the connector between the two groups
- Dhaka works as a receiver of packets delivered to unknown ip addresses
- Rajshahi and Khulna have a connection between them but it wont activate until the network from Dhaka routers stop working, else packets will travel from Rajshahi to Khulna traveling via Dhaka
- Dhaka network will have the host devices dynamically get their IP addresses generated from a server inside the network named “IP generator”
- There are two branches with their own corporate office : DHAKA and CHITTAGONG - each have their own web server named in the order : “Tele Net Dhaka” and “Tele Net CTG” which will be connected to Dhaka and Chittagong server accordingly and entering the websites it will show message: “Welcome to the TeleNet World, people of DHAKA/CTG!!” (depending on the web server area)

### Assumptions:

o Network Address considered 192.168.0.0/19
o All routers secured with password
o Sylhet connected to main branch Dhaka
o Static routing for Chittagong - Rangpur, Chittagong - Khulna for more secure
o Floating static routing for Rajshahi – Khulna
o Administrative distance for floating route considered 10
o RIP routing for remaining
o 100 IPs excluded for DHCP
o Dhaka as a way point between Chittagong and Rajshahi without human intervention

### License

Please use for education purposes only. It is alright to take inspirations, but please do not use the exact software for your projects/assignments. <br> <br> © Copyright Ahmad Al Asad
