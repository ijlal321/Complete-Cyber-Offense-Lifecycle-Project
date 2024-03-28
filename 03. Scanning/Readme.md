Here is the documentation for the "03. Scanning" project:

---

# 03. Scanning

## Introduction

The "Scanning" project focuses on exploring scanning techniques in cybersecurity. Scanning plays a crucial role in identifying open ports, services running on those ports, and potential vulnerabilities within a target system or network.

### Theory Behind Scanning

Scanning is a phase in cybersecurity assessments that involves probing target systems or networks to gather information about their infrastructure, services, and potential vulnerabilities. It helps in understanding the attack surface and forms the basis for further analysis and security testing.

## Tools and Techniques Used

1. **TCP & UDP**

   - TCP (Transmission Control Protocol) and UDP (User Datagram Protocol) are fundamental protocols used in networking.
   - TCP is connection-oriented and ensures reliable data delivery, while UDP is connectionless and prioritizes speed.
   - Understanding the differences between TCP and UDP is essential for effective scanning and communication with target systems.

2. **Netdiscover**

   - Netdiscover is a network scanning tool used for discovering active hosts on a network.
   - To perform a Netdiscover scan, use the following command:

     ```
     netdiscover -i eth0
     ```

   - Replace "eth0" with your network interface. Netdiscover will display a list of active hosts along with their MAC addresses and IP addresses.

3. **Performing Nmap Scan**

   - Nmap (Network Mapper) is a versatile and powerful scanning tool used for network discovery and security auditing.
   - To perform a basic Nmap scan, use the following command:

     ```
     nmap target_ip_address
     ```

   - Replace "target_ip_address" with the IP address of the target system or network. Nmap will scan for open ports and services on the target.

4. **Different Nmap Scan Types**

   - Nmap offers various scan types, including:
     - SYN Scan: Stealthy scan using TCP SYN packets.
     - UDP Scan: Scan for open UDP ports.
     - Full TCP Connect Scan: Completes the TCP three-way handshake.
     - Intense Scan: Comprehensive scan with default scripts and thorough checks.
     - Stealth Scan: SYN scan with additional evasion techniques.
     - OS Detection Scan: Identifies the target's operating system.

5. **Discovering Target Operating System**

   - Nmap can detect the operating system (OS) running on the target system using OS detection techniques.
   - To perform an OS detection scan with Nmap, use the following command:

     ```
     nmap -O target_ip_address
     ```

   - Nmap will analyze responses from the target and provide information about the probable OS running on the target system.

6. **Detecting Version Of Service Running On An Open Port**

   - Nmap can also detect the version of services running on open ports using version detection techniques.
   - To perform a version detection scan with Nmap, use the following command:

     ```
     nmap -sV target_ip_address
     ```

   - Nmap will probe open ports and attempt to identify the specific versions of services running on those ports.

## Conclusion

The "Scanning" project has explored essential scanning techniques and tools used in cybersecurity assessments. Scanning plays a vital role in identifying potential vulnerabilities, understanding target systems, and planning effective security strategies. By mastering scanning techniques, cybersecurity professionals can enhance their ability to assess and secure systems and networks effectively.

---

This documentation provides an overview of scanning theory, tools used, and techniques such as Netdiscover and Nmap scans, along with examples of their usage and their significance in cybersecurity assessments.