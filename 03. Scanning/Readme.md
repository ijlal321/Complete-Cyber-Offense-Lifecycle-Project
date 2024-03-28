
# Scanning

## Table Of Content

1. [Introduction](#introduction)
2. [Theory Behind Scanning](#theory-behind-scanning)
3. [Tools and Techniques Used](#tools-and-techniques-used)
   - [TCP & UDP](#tcp--udp)
   - [Netdiscover](#netdiscover)
   - [Performing Nmap Scan](#performing-nmap-scan)
   - [Different Nmap Scan Types](#different-nmap-scan-types)
   - [Discovering Target Operating System](#discovering-target-operating-system)
   - [Detecting Version Of Service Running On An Open Port](#detecting-version-of-service-running-on-an-open-port)
4. [Conclusion](#conclusion)


## Introduction

The "Scanning" project focuses on exploring scanning techniques in cybersecurity. Scanning plays a crucial role in identifying open ports, services running on those ports, and potential vulnerabilities within a target system or network.

### Theory Behind Scanning

Scanning is a phase in cybersecurity assessments that involves probing target systems or networks to gather information about their infrastructure, services, and potential vulnerabilities. It helps in understanding the attack surface and forms the basis for further analysis and security testing.

## Tools and Techniques Used

### **TCP & UDP**

   - TCP (Transmission Control Protocol) and UDP (User Datagram Protocol) are fundamental protocols used in networking.
   - TCP is connection-oriented and ensures reliable data delivery, while UDP is connectionless and prioritizes speed.
   - Understanding the differences between TCP and UDP is essential for effective scanning and communication with target systems.

### **Netdiscover**

   - Netdiscover is a network scanning tool used for discovering active hosts on a network.
   - To perform a Netdiscover scan, use the following command:

     ```
     netdiscover -i eth0
     ```

   - Replace "eth0" with your network interface. Netdiscover will display a list of active hosts along with their MAC addresses and IP addresses.
  
     ![image](https://github.com/ijlal321/Complete-Cyber-Offense-Lifecycle-Project/assets/103317626/a260b7e9-5452-4e17-9df8-24a9be90e83c)

### **Performing Nmap Scan**

   - Nmap (Network Mapper) is a versatile and powerful scanning tool used for network discovery and security auditing.
   - To perform a basic Nmap scan, use the following command:

     ```
     nmap target_ip_address
     ```

   - Replace "target_ip_address" with the IP address of the target system or network. Nmap will scan for open ports and services on the target.

![image](https://github.com/ijlal321/Complete-Cyber-Offense-Lifecycle-Project/assets/103317626/d1dabc2d-d8eb-4a97-8ddc-f8eba672590a)


### **Different Nmap Scan Types**

   - Nmap offers various scan types, including:
     - SYN Scan: Stealthy scan using TCP SYN packets.
     - UDP Scan: Scan for open UDP ports.
     - Full TCP Connect Scan: Completes the TCP three-way handshake.
     - Intense Scan: Comprehensive scan with default scripts and thorough checks.
     - Stealth Scan: SYN scan with additional evasion techniques.
     - OS Detection Scan: Identifies the target's operating system.

### **Discovering Target Operating System**

   - Nmap can detect the operating system (OS) running on the target system using OS detection techniques.
   - To perform an OS detection scan with Nmap, use the following command:

     ```
     nmap -O target_ip_address
     ```

   - Nmap will analyze responses from the target and provide information about the probable OS running on the target system.

![image](https://github.com/ijlal321/Complete-Cyber-Offense-Lifecycle-Project/assets/103317626/cd9c7a60-962e-4456-a4da-019c08e7a591)


### **Detecting Version Of Service Running On An Open Port**

   - Nmap can also detect the version of services running on open ports using version detection techniques.
   - To perform a version detection scan with Nmap, use the following command:

     ```
     nmap -sV target_ip_address
     ```

   - Nmap will probe open ports and attempt to identify the specific versions of services running on those ports.

![image](https://github.com/ijlal321/Complete-Cyber-Offense-Lifecycle-Project/assets/103317626/2340bed1-3103-4340-b568-58b406496850)


## Conclusion

The "Scanning" project has explored essential scanning techniques and tools used in cybersecurity assessments. Scanning plays a vital role in identifying potential vulnerabilities, understanding target systems, and planning effective security strategies. By mastering scanning techniques, cybersecurity professionals can enhance their ability to assess and secure systems and networks effectively.
