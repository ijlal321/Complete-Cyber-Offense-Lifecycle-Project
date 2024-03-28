
# Reconnaissance & Information Gathering

## Introduction

The "Reconnaissance & Information Gathering" project focuses on understanding and utilizing key tools and techniques for gathering critical data in cybersecurity assessments.

## Table Of Content

1. [Introduction](#introduction)
2. [What is Information Gathering?](#what-is-information-gathering)
3. [Tools and Techniques Used](#tools-and-techniques-used)
   - [Obtaining IP Address, Physical Address Using Whois Tool](#obtaining-ip-address-physical-address-using-whois-tool)
   - [Whatweb Stealthy Scan](#whatweb-stealthy-scan)
   - [Whatweb Aggressive Scan](#whatweb-aggressive-scan)
   - [Gathering Emails Using theHarvester & Hunter.io](#gathering-emails-using-theharvester--hunterio)
   - [Finding Usernames With Sherlock](#finding-usernames-with-sherlock)
4. [Conclusion](#conclusion)


### What is Information Gathering?

Information gathering, also known as reconnaissance, is the process of collecting strategic data about target systems or networks. This phase is crucial for identifying potential vulnerabilities, understanding the target environment, and planning effective security strategies.

## Tools and Techniques Used

###  **Obtaining IP Address, Physical Address Using Whois Tool**

   The Whois tool is a domain lookup service that provides information about domain registrations. For example, to obtain information about a domain like "example.com," you can use the following command in a terminal:

   ```
   whois example.com
   ```

   This command will return details such as the registrar, registration date, expiration date, domain owner contact information, and sometimes even the physical address associated with the domain registration.

![image](https://github.com/ijlal321/Complete-Cyber-Offense-Lifecycle-Project/assets/103317626/694d92aa-fe9c-4356-af66-2523d6746436)


### **Whatweb Stealthy Scan**

   Whatweb is a web scanning tool that analyzes websites and provides insights into their technologies. To perform a stealthy scan using Whatweb, you can use the following command:

   ```
   whatweb --stealthy example.com
   ```

   This command will scan the target website ("example.com") in a less intrusive manner, gathering information about the web server type, CMS (Content Management System), web framework, and other technologies without triggering alarms or alerts.

![image](https://github.com/ijlal321/Complete-Cyber-Offense-Lifecycle-Project/assets/103317626/72691d68-6741-4441-ad9c-6769f9fb4f3d)

### **Whatweb Aggressive Scan**

   The aggressive scan mode in Whatweb provides a more detailed analysis of the target website. You can perform an aggressive scan using the following command:

   ```
   whatweb --aggressive example.com
   ```

   This command will conduct a thorough scan, revealing specific versions of software, plugin configurations, potentially vulnerable areas, and more detailed insights into the target's web environment.

![image](https://github.com/ijlal321/Complete-Cyber-Offense-Lifecycle-Project/assets/103317626/391b91ee-60a6-4f85-bf28-4f355e920fa3)


### **Gathering Emails Using theHarvester & Hunter.io**

   TheHarvester is a reconnaissance tool that collects email addresses, subdomains, and other data related to a target domain. For example, to gather email addresses associated with the domain "example.com," you can use the following command:

   ```
   theharvester -d example.com -l 100 -b all
   ```

   This command will search various sources for email addresses related to "example.com" and output the results. Similarly, Hunter.io can be used to extract email addresses from websites by entering the domain name in the Hunter.io search bar.

![image](https://github.com/ijlal321/Complete-Cyber-Offense-Lifecycle-Project/assets/103317626/b2c77405-5575-4f86-832d-aa10974c5b16)


### **Finding Usernames With Sherlock**

   Sherlock is a tool for username enumeration across multiple online platforms. To search for usernames associated with a target, you can use the following command:

   ```
   python3 sherlock.py target_username
   ```

   Replace "target_username" with the specific username you want to search for. Sherlock will scan various platforms and social media networks to identify accounts associated with the provided username.


![image](https://github.com/ijlal321/Complete-Cyber-Offense-Lifecycle-Project/assets/103317626/7c7a37a0-063c-41fe-9d3c-626a39422183)

## Conclusion

The "Reconnaissance & Information Gathering" project has demonstrated practical examples of using essential tools and techniques in cybersecurity assessments. Information gathering plays a pivotal role in understanding target environments, identifying potential vulnerabilities, and formulating effective security strategies. By mastering these reconnaissance techniques, cybersecurity professionals can enhance their ability to assess and secure systems and networks effectively.

