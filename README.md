# Network-Traffic-Analysis-Using-Wireshark on Windows
Capturing and analyzing network traffic using Wireshark on Windows.
## Prerequisites

Before capturing network traffic, ensure the following requirements are met:

- Windows 10 or Windows 11
- Wireshark installed
- Administrator privileges
- Active network connection (Wi-Fi or Ethernet)
- Basic understanding of networking concepts
## Installing Wireshark

1. Download Wireshark from the official website:

   https://www.wireshark.org/

2. Run the installer and follow the default installation steps.

3. During installation, ensure **Npcap** is selected, as it is required for packet capturing.

4. After installation, launch Wireshark as **Administrator**.

## Capturing Traffic with Wireshark

### Launch Wireshark

Open Wireshark by running it as **Administrator**.

### Select Network Interface

Choose the active network interface (Wi-Fi or Ethernet) that is connected to the Internet.

### Start Packet Capture

Click the **blue shark fin** icon to begin capturing network traffic.

### Generate Network Traffic

Generate different types of network traffic by performing the following actions:

- Browse websites such as Google, GitHub, and YouTube.
- Run the following command to generate ICMP traffic:

```cmd
ping google.com
```

- Run the following command to generate DNS traffic:

```cmd
nslookup google.com
```

### Stop Packet Capture

Click the **red stop** button after capturing sufficient packets.

### Save Packet Capture

Go to **File → Save As** and save the captured packets as:

```
capture.pcapng
```

Store the file inside the **captures** folder for future analysis.
## Packet Analysis

The captured network traffic was analyzed using Wireshark display filters to observe different protocols and their communication patterns.
### TCP Analysis

Filter Used

```text
tcp
```

TCP packets were analyzed to observe reliable, connection-oriented communication between hosts.

The following details were observed:

- Source and destination IP addresses
- Source and destination port numbers
- TCP flags (SYN, ACK, FIN)
- Sequence and acknowledgement numbers
- Packet length
- IPv4 and IPv6 communication
