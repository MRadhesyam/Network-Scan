# Network-Scan
Network scanning task using Nmap to identify open ports and services on local network, with analysis of security risks.

## Steps Performed:
1. Installed Nmap and Wireshark.
2. Found local IP range: 192.168.1.0/24
3. Ran TCP SYN scan using `nmap -sS 192.168.1.0/24`
4. Saved results to `scan_results.txt`
5. Identified open ports and services.

## Findings:
- Device 192.168.31.41: Open ports 62078 (TCP)
- Device 192.168.31.113: No open Ports
- Device 192.168.31.118: Open ports 80 and 135 (TCP)
- Device 192.168.31.142: Open ports 7000, 8001,8002, 8080 (TCP)
- Device 192.168.31.186: Open ports 135, 139, 445 (TCP)
- Device 192.168.1.15: Open ports 443 (HTTPS)

## Security Risks:
- SSH (22) → Brute force risk if weak credentials.
- HTTP (80) → Data not encrypted.
