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

TCP packets were analyzed using the Wireshark display filter.

The following observations were made:

- Captured TCP packets between different devices.
- Observed source and destination IP addresses.
- Observed source and destination port numbers.
- Observed reliable communication between devices.
### UDP Analysis

Filter Used

```text
udp
```

UDP packets were analyzed using the Wireshark display filter.

The following observations were made:

- Captured UDP packets between different devices.
- Observed source and destination IP addresses.
- Observed source and destination port numbers.
- Observed communication without establishing a connection.
### DNS Analysis

Filter Used

```text
dns
```

DNS packets were analyzed using the Wireshark display filter.

The following observations were made:

- Captured DNS query and response packets.
- Observed domain name requests.
- Identified communication between the client and DNS server.
