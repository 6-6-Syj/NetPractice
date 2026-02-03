<p style="text-align:center;"><em>This project has been created as part of the 42 curriculum by jmagand</em></p>

<div align="center">
<h1> <strong>✨ NetPractice ✨</strong></h1>
</div>

### 🎯 **Project Overview**

This project is a **network configuration simulator** where you solve networking problems to make virtual networks function properly. <br> With **10 progressive levels**, you'll diagnose and fix misconfigured networks through a practical web interface.

## 📋 Table of Contents
- [🔍 Description](#-description)
- [📖 Instructions](#-instructions)
  - [🚀 Installation](#-installation)
  - [⚙️ How It Works](#️-how-it-works)
  - [📤 Submission Details](#-submission-details)
- [📚 Resources](#-resources)
  - [📘 IP Addressing & Subnetting](#-ip-addressing--subnetting)
  - [🔗 TCP/IP Protocols](#-tcpip-protocols)
  - [🖧 Default Gateways, Routers & Switches](#-default-gateways-routers--switches)
  - [📡 OSI Model Layers](#-osi-model-layers)
  - [🔗 Links to documentation](#-links-to-documentation)
  - [🤖 About AI](#-about-ai)

---

<details>
<summary><strong>🔍 Description</strong></summary>

This project involves solving networking problems to make a network function properly.

**Key Features:**

- **10 training levels** of increasing complexity
- **Visual network diagrams** with interactive configuration
- **Real-time feedback** through system logs
- **Configuration export** for assignment submission

**Example Level Preview:**
<p align="center">
<img src="img/lvl9.png" alt="Level 9 Network Diagram" width="50%"/>
<br><sub><em>Example of a network configuration challenge</em></sub>
</p>

For each level, you're presented with a **non-functioning network diagram** and must adjust configurations until all connections work correctly.

</details>

<br>

<details>
<summary><strong>📖 Instructions</strong></summary>
<br>
<details>
<summary><strong>🚀 Installation</strong></summary>

**Step-by-Step Setup:**

1. **Download** the file attached to the project's page
2. **Extract** the files into any folder of your choice
3. **Run** the `run.sh` file: ./run.sh


**Expected Result:**
<p align="center"> <img src="img/welcome.png" alt="NetPractice Welcome Screen" width="50%"/> <br><sub><em>Welcome interface after successful launch</em></sub> </p>

**Access Options:**

1. **Training Mode**: Enter your login to use personal configurations
2. **Evaluation Mode**: Generate random configurations suitable for evaluations

</details>

<details>
<summary><strong>⚙️ How It Works</strong></summary>

**Interface Layout:**
<p align="center"> <img src="img/quests.png" alt="Level Objectives Display" width="50%"/> <br><sub><em>Objectives displayed at the top of each level</em></sub> </p>

#### **Control Buttons**

<p align="center"> <img src="img/buttons.png" alt="Control Buttons" width="50%"/> <br><sub><em>Primary interface controls</em></sub> </p>

1. **Check again:** Validates your current configuration
2. **Get my config:** Downloads configuration file for submission
3. **Next level:** Advances to next challenge. Only appears after successful completion

#### **Diagnostic Tools**

<p align="center"> <img src="img/logs.png" alt="Configuration Logs" width="50%"/> <br><sub><em>Diagnostic logs helping identify configuration errors</em></sub> </p>

The bottom log panel provides real-time feedback about:

1. Missing gateways
2. Invalid IP addresses
3. Routing issues
4. Connectivity problems

#### **📜 Rules**

1. Examine the network diagram and objectives
2. Modify the editable (unshaded) configuration fields
3. Check your configuration using the validation button
4. Review logs to understand any failures
5. Repeat until all objectives are met
6. Export your configuration when successful

</details>

<details>
<summary><strong>📤 Submission Details</strong></summary>

**Important Submission Requirements:**

✅ Complete all 10 levels successfully<br>
⬆️ Export each level's configuration using the "Get my config" button<br>
💾 Save all configuration files (level1.txt through level10.txt) in your repository's root directory<br>

**Expected repository structure:**
<p align="center"> <img src="img/configurations.png" alt="Configuration Files Structure" width="50%"/> <br><sub><em>Required configuration files for submission</em></sub> </p>

</details>

</details>

<br>

<details>
<summary><strong>📚 Resources</strong></summary>

<details> <summary><strong>📘 IP Addressing & Subnetting</strong></summary>

### IP Address basics
Format: 4 octets (e.g., 192.168.1.1), 32 bits total.

#### Address Classes (Traditional):

• Class A: 1.0.0.0 to 126.255.255.255 (Large networks)<br>
• Class B: 128.0.0.0 to 191.255.255.255 (Medium networks)<br>
• Class C: 192.0.0.0 to 223.255.255.255 (Small networks)<br>
• Classes D/E: Multicast and experimental<br>

#### CIDR Notation:<br>
Modern method (e.g., 192.168.1.0/24). The /24 is the prefix length (network bits).

### Subnetting

Number of Subnets = 2^n (where n = borrowed host bits)<br>
Usable Hosts per Subnet = 2^(32 - prefix) - 2<br>
Block Size = 256 - subnet_mask_octet_value<br>

Example:<br>
<br>
Network: 192.168.1.0/24<br>
Need: 4 subnets → Borrow 2 bits (2² = 4)<br>
New Subnet Mask: /26 or 255.255.255.192<br>
Block Size: 256 - 192 = 64<br>
<br>
• Subnet Ranges:<br>

192.168.1.0 to 192.168.1.63 (Network: .0, Broadcast: .63)<br>
192.168.1.64 to 192.168.1.127 (Network: .64, Broadcast: .127)<br>
192.168.1.128 to 192.168.1.191<br>
192.168.1.192 to 192.168.1.255<br>

<p align="center"> <img src="img/array.png" alt="CIDR chart" width="50%"/> <br><sub><em>IPV4 CIDR Chart</em></sub> </p>

<br></details>

<details> <summary><strong>🔗 TCP/IP Protocols</strong></summary><br>
TCP (Transmission Control Protocol) is a protocol that allows devices to communicate reliably over a network.<br>
It ensures that data reaches the destination correctly and in the right order, even if parts of the network are slow or unreliable.<br><br>
• It works at the Transport Layer (Layer 4) of the OSI model and is an essential part of the TCP/IP protocol suite used for Internet communication.<br>
• TCP establishes a logical connection between the sender and receiver before data transmission begins.<br>
• It ensures that data is delivered accurately and in the same order in which it was sent using acknowledgements and sequence numbers.<br>
• TCP detects errors using checksums and retransmits lost or corrupted packets to maintain data integrity.<br>
• It controls the data transmission rate to avoid overwhelming the receiver and adapts to network congestion for efficient communication.<br>

### How TCP Works?<br>
1. Segmenting<br>
• When an application sends data (like an email or file), TCP breaks the data into smaller chunks called segments.<br>
• Each segment has a header containing information like sequence numbers, ports, and flags.<br>
• This makes it easier to send large amounts of data over the network reliably.<br>
<br>
2. Routing via IP<br>
• Once TCP creates segments, they are handed to IP (Internet Protocol).<br>
• IP is responsible for delivering the segments from the sender to the receiver, possibly through multiple routers.<br>
• TCP doesn’t care about the path—IP handles routing and addressing.<br>
<br>
3. Reassembly at Receiver<br>
• Segments may arrive out of order because they can take different paths through the network.<br>
• TCP at the receiver uses sequence numbers to reassemble the segments into the correct order to reconstruct the original message.<br>
<br>
4. Acknowledgments (ACKs)<br>
• The receiver sends an ACK for every segment (or group of segments) it receives correctly.<br>
• This tells the sender that the data has arrived safely.<br>
• If an ACK is not received, TCP assumes the segment was lost and triggers retransmission.<br>
<br>
5. Retransmission<br>
• If the sender does not receive an acknowledgment within a certain time, it resends the missing segment.<br>
• This ensures no data is lost, making TCP reliable.<br>
<br>
6. Flow & Error Control<br>
• Flow Control: TCP prevents the sender from sending too much data too quickly for the receiver to handle, using a sliding window mechanism.<br>
• Error Control: TCP checks for corrupted segments using checksums and requests retransmission if needed.<br>
• Together, these mechanisms ensure data is delivered reliably and efficiently, without overloading the network or the receiver.<br>

### Advantages of TCP<br>

• Error-Free Data Transfer: TCP detects errors during transmission and retransmits lost or corrupted data, ensuring accurate delivery.<br>
• Ordered Delivery: Data packets are received in the same sequence in which they were sent, maintaining data consistency.<br>
• Flow Control: Prevents the sender from overwhelming the receiver by controlling the rate of data transmission.<br>
• Congestion Control: Adjusts the sending speed based on network traffic conditions to reduce packet loss and congestion.<br>
• Reliable Communication: Ensures complete and dependable data transfer, making it suitable for critical applications.<br>
• Widely Supported and Standardized: TCP is a globally accepted protocol, supported by all major operating systems and network devices.<br>

<br></details>

<details> <summary><strong>🖧 Default Gateways, Routers & Switches</strong></summary>

### Defaut gateway
The router a device uses to send traffic destined for networks outside its own local subnet.

Critical Rules for NetPractice:<br>
1. MUST be on the same IP subnet as the host device.<br>
2. The router itself MUST have an interface configured in that subnet.<br>
3. Only needed for communication OUTSIDE the local subnet.<br>

Common Configuration Error:<br>
Host IP: 192.168.1.10/24<br>
Gateway: 192.168.2.1    ❌ FAILS (Different subnet)<br>
Gateway: 192.168.1.1    ✅ WORKS (Same subnet)<br>

### Switch vs Router

1. **Switch**<br>
Switch connects devices within the same network/subnet.<br>
Forwards frames based on MAC addresses.<br>
The connections between devices on a local network segment.<br>
• All ports are in the same broadcast domain<br>
• Learns MAC addresses automatically<br>
• Creates separate collision domains<br>

2. **Router**<br>
A router is a networking device that forwards data packets between different computer networks.<br>
It connects multiple packet-switched networks or subnetworks, managing traffic by directing packets to their intended IP addresses.<br>
Routers allow multiple devices to share an Internet connection efficiently.<br><br>
Forwards packets based on IP addresses.<br>
The "gateway" devices that interconnect the various subnets in your diagram.<br>
• Has multiple interfaces in different subnets<br>
• Makes decisions using routing tables<br>
• Creates broadcast domains<br>

**Routing Table**: <br>
A host or router uses a routing table to decide where to send packets.<br>

<p align="center"> <img src="img/routingtable.png" alt="Routing table" width="50%"/> <br><sub><em>Routing table interface in NetPractice</em></sub> </p>

On the left: Target network (destination)<br>
On the right: The next hop (0.0.0.0 means directly connected)
<br></details>

<details> <summary><strong>📡 OSI Model Layers</strong></summary><br>
The OSI (Open Systems Interconnection) Model is a set of rules that explains how different computer systems communicate over a network.<br>
OSI Model was developed by the International Organization for Standardization (ISO).<br>
The OSI Model consists of 7 layers and each layer has specific functions and responsibilities.<br>
This layered approach makes it easier for different devices and technologies to work together.<br><br>
<p align="center"> <img src="img/osi.png" alt="OSI Layers" width="50%"/> <br><sub><em>The 7 layers of OSI</em></sub> </p>

7. **Application**

Function: User interface and network services.<br>
Examples: Web browser, email client, NetPractice's web interface.<br>
NetPractice: Where you interact with the simulator.<br>

6. **Presentation**

Function: Data translation, encryption, compression.<br>
Examples: SSL/TLS, JPEG, MPEG, ASCII.<br>
NetPractice: Data formatting for display.<br>

5. **Session**

Function: Manages dialogues/connections between applications.<br>
Examples: Session establishment, management, and termination.<br>
NetPractice: Manages your login session.<br>

4. **Transport**

Function: End-to-end connection, reliability, and flow control.<br>
Key Protocols: TCP (connection-oriented, reliable), UDP (connectionless, fast).<br>
NetPractice: Underlying connection for the web interface.<br>

3. **Network**

Function: Logical addressing, routing, and path determination.<br>
Key Protocols: IP, ICMP, ARP.<br>
NetPractice: THE MOST IMPORTANT LAYER FOR THIS PROJECT. This is where IP addresses, subnet masks, and gateways operate.<br>
Devices: Routers.<br>

2. **Data Link**

Function: Node-to-node delivery, framing, error detection. Converts packets to frames.<br>
Sublayers: LLC (Logical Link Control), MAC (Media Access Control).<br>
Key Protocols: Ethernet, Wi-Fi (802.11), PPP.<br>
Devices: Switches, Network Interface Cards (NICs).<br>
Addressing: MAC Address (e.g., 00:1A:2B:3C:4D:5E).<br>

1. **Physical**

Function: Transmits raw bit streams over a physical medium.<br>
Examples: Cables (Cat5e, fiber), connectors, electrical/optical signals.<br>
NetPractice: Represented by the physical lines connecting devices in the diagram.<br>


</details>
<br>

<details> <summary><strong>🔗 Links to documentation</strong></summary><br>
https://isrdoc.wordpress.com/tag/cidr/<br>
https://fr.wikipedia.org/wiki/Adresse_IP<br>
https://www.geeksforgeeks.org/computer-networks/routing-tables-in-computer-network/<br>
https://www.geeksforgeeks.org/computer-networks/introduction-of-a-router/szitch<br>
https://www.it-connect.fr/adresses-ipv4-et-le-calcul-des-masques-de-sous-reseaux/<br>
https://www.geeksforgeeks.org/computer-networks/open-systems-interconnection-model-osi/<br>
https://www.geeksforgeeks.org/computer-networks/what-is-transmission-control-protocol-tcp/<br>
</details>
<br>

<details>
<summary><strong>🤖 About AI</strong></summary>

In this project, I used AI to:<br>
- **Get tips and guidance** on proper Markdown (.md) syntax and structure<br>
- **Correct and improve** my English writing for better clarity<br>
- **Format and style** the README for optimal presentation on GitHub<br>
- **Troubleshoot formatting issues** specific to GitHub's Markdown implementation<br>

The AI assisted with transforming raw content into a well-organized, visually appealing README while ensuring all technical information remained accurate and helpful for users.
</details>
<br>