# Network Packet Analysis using Wireshark

## Overview
This project demonstrates network traffic analysis using Wireshark.  
The goal was to capture ICMP packets, analyze packet behavior, and observe abnormal traffic patterns such as high-frequency ping activity.

## Tools Used
- Wireshark
- Kali Linux
- VirtualBox
- ICMP (Internet Control Message Protocol)

## Environment
- Kali Linux running on VirtualBox
- Network Adapter: Bridged Mode
- Packet capture interface: eth0

## Steps Performed

1. Started Wireshark packet capture on `eth0`
2. Generated ICMP traffic using ping commands
3. Captured ICMP Echo Request and Echo Reply packets
4. Analyzed packet details such as:
   - Source IP
   - Destination IP
   - TTL
   - ICMP Type and Code
5. Used Wireshark **Conversations** feature to observe packet flow
6. Generated high-frequency ICMP traffic to simulate abnormal behavior
7. Visualized packet spikes using **Wireshark I/O Graph**

## Key Observations

- ICMP Type 8 represents Echo Request packets
- ICMP Type 0 represents Echo Reply packets
- High frequency ICMP traffic can indicate:
  - Network scanning
  - Early stages of DoS behavior
  - Network troubleshooting activity

## Screenshots

### Wireshark Interface
![interface](images/wireshark-interface.png)

### ICMP Packet Capture
![icmp](images/icmp_packet_capture.png)

### Packet Details
![details](images/icmp_packet_details.png)

### ICMP Conversations
![conversation](images/icmp_conversation_sorted.png)

### High Frequency ICMP Traffic
![ping](images/icmp_high_frequency_ping.png)

### I/O Graph Analysis
![graph](images/icmp_io_graph.png)

## Files Included

| File | Description |
|----|----|
network_traffic_icmp.pcap | Packet capture file |
ICMP_Network_Packet_Analysis_Report.pdf | Detailed analysis report |
images/ | Wireshark screenshots |

## Learning Outcome

This project helped develop understanding of:

- Packet level network analysis
- ICMP protocol behavior
- Traffic pattern analysis
- Wireshark packet inspection
- Detecting abnormal network activity

## Author

Mohammed Amaan
