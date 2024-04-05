**Midterm-Sandrino_Navelino**
# **Kali Linux Tools** 

Kali Linux is a widely used Linux distribution specifically designed for digital forensics and penetration testing. It comes pre-installed with numerous tools categorized into various domains such as information gathering, vulnerability analysis, exploitation, wireless attacks, reverse engineering, and more. Here's a brief overview of some of the categories and tools available in Kali Linux:

<details>
<summary><h2>Information Gathering</h2><br>
  
Information gathering is the initial phase of a security assessment where various tools and techniques are employed to gather intelligence about a target system, network, or organization. This phase aims to collect as much relevant information as possible to better understand the target's infrastructure, potential vulnerabilities, and attack surface. Information gathering techniques may include network scanning, reconnaissance, enumeration, and open-source intelligence (OSINT) gathering. These techniques help security professionals identify potential entry points, weaknesses, and avenues for further exploitation during the assessment process.

</summary>

  <summary><h3>Information Gathering Techniques</h3></summary>
 
1. **DNS Analysis**: Examining Domain Name System (DNS) records to gather information about domain names, such as IP addresses, mail servers, and name servers associated with a particular domain.

2. **IDS/IPS Identification**: Detection and identification of Intrusion Detection Systems (IDS) and Intrusion Prevention Systems (IPS) on a network to understand security mechanisms in place.

3. **Live Host Identification**: Determining which hosts on a network are currently active and reachable, usually accomplished through techniques such as ping sweeps or ARP scans.

4. **Network Port Scanner**: Using tools like Nmap to scan a network and identify open ports on target systems, providing insights into running services and potential vulnerabilities.

5. **OSINT Analysis (Open-Source Intelligence)**: Gathering information from publicly available sources like websites, social media, and public databases to gather intelligence about targets.

6. **Route Analysis**: Analyzing routing information on a network to understand how data packets are routed between hosts and networks, helping in mapping network topology and identifying attack paths.

7. **SMB Analysis (Server Message Block)**: Analyzing the SMB protocol, commonly used for sharing files, printers, and resources on a network, to gather information about shared resources and potential security vulnerabilities.

8. **SMTP Analysis (Simple Mail Transfer Protocol)**: Analyzing the SMTP protocol used for sending and receiving email messages, providing insights into email server configurations and potential security issues.

9. **SNMP Analysis (Simple Network Management Protocol)**: Analyzing the SNMP protocol used for managing and monitoring network devices, revealing information about device configurations and potential security weaknesses.

10. **SSL Analysis (Secure Sockets Layer)**: Analyzing SSL/TLS certificates and encryption configurations used to secure communications over the network, identifying cryptographic protocols and potential security vulnerabilities.

<summary><h3>Information Gathering Tools</h3></summary>
  Tools in this category are used to gather information about targets, including hosts, networks, and services.<br>
  Examples of this are below:

## 1. Nmap

Nmap (Network Mapper) is a powerful open-source network scanning tool used for discovering hosts and services on a computer network, thus creating a "map" of the network.

- YouTube Video: [Introduction to Nmap - Network Scanning Basics](https://www.youtube.com/watch?v=6-Uemw0aYXM)
  - Command: `nmap <target>`
    <details>
    <summary>Copy Command</summary>
    
    ```
    nmap <target>
    ```
    </details>

## 2. theHarvester

theHarvester is a tool for gathering email accounts, subdomains, virtual hosts, and open ports from public sources like search engines and PGP key servers.

- YouTube Video: [theHarvester - Information Gathering Tool](https://www.youtube.com/watch?v=t-cjcJJa0fQ)
  - Command: `theharvester -d <target> -l <limit>`
    <details>
    <summary>Copy Command</summary>
    
    ```
    theharvester -d <target> -l <limit>
    ```
    </details>

## 3. Recon-ng

Recon-ng is a full-featured web reconnaissance framework written in Python. It provides a powerful environment for conducting reconnaissance and open-source intelligence gathering on a target.

- YouTube Video: [Recon-ng - Open Source Intelligence Framework](https://www.youtube.com/watch?v=ybA2SoO97bA)
  - Command: `recon-ng`
    <details>
    <summary>Copy Command</summary>
    
    ```
    recon-ng
    ```
    </details>

## 4. Maltego

Maltego is a data visualization tool used for open-source intelligence and forensics investigations. It allows users to visualize complex relationships among entities gathered from various sources.

- YouTube Video: [Maltego CE Tutorial](https://www.youtube.com/watch?v=mv-vtcvt1l8)
  - Additional Information: Maltego offers Community Edition (CE) for free, with limited functionalities compared to the commercial version.
    ```
    Maltego offers Community Edition (CE) for free, with limited functionalities compared to the commercial version.
    ```

## 5. SpiderFoot

SpiderFoot is an open-source intelligence automation tool that enables users to gather information from various sources, including search engines, social media platforms, and public databases.

- YouTube Video: [SpiderFoot - Open Source Intelligence Automation Tool](https://www.youtube.com/watch?v=Lwe5amqP5kc)
  - Additional Information: SpiderFoot provides a user-friendly web interface for configuring and running scans.
    ```
    SpiderFoot provides a user-friendly web interface for configuring and running scans.
    ```
## 6. Amass

Amass is a tool used for network mapping, it discovers and enumerates subdomains through various techniques.
- YouTube Video: [Amass - Network Mapping Tool](https://www.youtube.com/watch?v=YTzZ5IVmmRM)
  - Command: `amass enum -d example.com`
    ```
    amass enum -d example.com
    ```

## 7. Dmitry

Dmitry is an information gathering tool used for gathering intelligence about a target by performing a variety of tasks such as subdomain enumeration, port scanning, and more.
- YouTube Video: [Dmitry - Information Gathering Tool](https://www.youtube.com/watch?v=6Gd9GXbhjWc)
  - Command: `dmitry -winsepo example.txt example.com`
    ```
    dmitry -winsepo example.txt example.com
    ```

## 8. Ike-scan

Ike-scan is a command-line tool used for discovering, fingerprinting, and testing IPsec VPN systems.
- YouTube Video: [Ike-scan - IPsec VPN Testing Tool](https://www.youtube.com/watch?v=YYZZma27S-A)
  - Command: `ike-scan <target>`
    ```
    ike-scan <target>
    ```

## 9. Legion (Root)

Legion (Root) is a multi-purpose security auditing and penetration testing framework which provides an easy-to-use interface along with an efficient and effective scanning engine.
- YouTube Video: [Legion (Root) - Security Auditing and Penetration Testing Framework](https://www.youtube.com/watch?v=2_rT5CJZ5iU)
  - Command: `legion`
    ```
    legion
    ```

## 10. Netdiscover

Netdiscover is an active/passive ARP reconnaissance tool, it discovers hosts on a network by actively sending ARP requests and analyzing responses.
- YouTube Video: [Netdiscover - ARP Reconnaissance Tool](https://www.youtube.com/watch?v=ISqCkfQK1QA)
  - Command: `netdiscover -i eth0`
    ```
    netdiscover -i eth0
    ```
<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>
</details>

<details>
<summary><h2>Vulnerability Analysis</h2><br>
  
Vulnerability analysis involves the systematic identification, assessment, and exploitation of weaknesses in computer systems, networks, and applications. This process aims to discover and mitigate security vulnerabilities that could be exploited by attackers to compromise the confidentiality, integrity, or availability of information assets. Vulnerability analysis techniques may include vulnerability scanning, penetration testing, fuzzing, and code review. By identifying and addressing vulnerabilities proactively, organizations can reduce the risk of security breaches and protect their assets from exploitation by malicious actors.

</summary>

### Vulnerability Analysis Techniques

Vulnerability analysis techniques involve methods for identifying and exploiting vulnerabilities within computer systems, networks, and applications.

#### 1. Fuzzing Tools

Fuzzing is a technique used to discover vulnerabilities in software by sending random, invalid, or unexpected data inputs to target applications or systems. Fuzzing tools automate this process, generating and sending test cases to identify potential vulnerabilities such as buffer overflows, injection flaws, and other security weaknesses.

#### 2. VoIP Tools

Voice over Internet Protocol (VoIP) tools are specialized tools designed to assess the security of VoIP systems and protocols. These tools analyze VoIP traffic, protocols, and configurations to identify vulnerabilities such as unauthorized access, eavesdropping, spoofing, and denial-of-service (DoS) attacks.

### Vulnerability Analysis Tools

Vulnerability analysis tools are software applications designed to assist security professionals in identifying, assessing, and exploiting vulnerabilities in computer systems, networks, and applications.

#### 1. legion (root)

Legion (Root) is a multi-purpose security auditing and penetration testing framework which provides an easy-to-use interface along with an efficient and effective scanning engine.

- YouTube Video: [Legion (Root) - Security Auditing and Penetration Testing Framework](https://www.youtube.com/watch?v=2_rT5CJZ5iU)
  - Command: `legion`
    ```
    legion
    ```

#### 2. Nikto

Nikto is a web server vulnerability scanner that checks for various known vulnerabilities and misconfigurations in web servers.

- YouTube Video: [Nikto - Web Server Vulnerability Scanner](https://www.youtube.com/watch?v=kAzJOXrEJQY)
  - Command: `nikto -h <target>`
    ```
    nikto -h <target>
    ```

#### 3. Nmap

Nmap (Network Mapper) is a powerful open-source network scanning tool used for discovering hosts and services on a computer network, thus creating a "map" of the network.

- YouTube Video: [Introduction to Nmap - Network Scanning Basics](https://www.youtube.com/watch?v=6-Uemw0aYXM)
  - Command: `nmap <target>`
    ```
    nmap <target>
    ```

#### 4. Unix-Privesc-Check

Unix-Privesc-Check is a script to check for simple privilege escalation vectors on Unix systems. It identifies misconfigurations that could allow unprivileged users to escalate their privileges to root.

- YouTube Video: [Unix-Privesc-Check - Checking for Privilege Escalation Vectors](https://www.youtube.com/watch?v=Kt2b5e9rZYY)
  - Command: `unix-privesc-check`
    ```
    unix-privesc-check
    ```
<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>
</details>

<details>
<summary><h2>Web Application Analysis</h2><br>

Web Application Analysis involves assessing the security posture of web applications to identify and mitigate vulnerabilities that could be exploited by attackers. This process aims to ensure the confidentiality, integrity, and availability of web application data and resources.
</summary>

### Techniques

#### 1. CMS & Framework Identification
CMS & Framework Identification involves identifying the content management systems (CMS) and web application frameworks used by a target web application. This information helps in understanding the underlying technologies and potential vulnerabilities associated with them.

#### 2. Web Application Proxies
Web Application Proxies are tools used to intercept, inspect, and modify HTTP/HTTPS traffic between a web browser and a web server. They aid in analyzing and manipulating web application requests and responses for security testing purposes.

#### 3. Web Crawlers & Directory Bruteforce
Web Crawlers and Directory Bruteforce tools are used to systematically explore and map the structure of a web application by discovering hidden or unlinked pages, directories, and resources. This technique helps in identifying potential attack surfaces and hidden vulnerabilities.

#### 4. Web Vulnerability Scanner
Web Vulnerability Scanners are automated tools designed to identify security vulnerabilities in web applications by scanning for common issues such as SQL injection, cross-site scripting (XSS), and insecure configuration settings. They help in detecting and prioritizing vulnerabilities for further investigation and remediation.

### Tools

#### 1. Burp Suite
Burp Suite is a powerful web application security testing toolkit that includes various tools for web vulnerability scanning, manual testing, and exploitation. It provides a comprehensive platform for assessing the security of web applications during development and deployment.
- YouTube Video: [Burp Suite Tutorial](https://www.youtube.com/watch?v=1XL4OoJnKtI)
  - Command: `burpsuite`

#### 2. Commix
Commix is an automated command injection tool specifically designed for web applications. It allows security testers to identify and exploit command injection vulnerabilities in web applications by automating the process of payload generation and injection.
- YouTube Video: [Commix - Command Injection Tool](https://www.youtube.com/watch?v=YkMJo_7tiIc)
  - Command: `commix`

#### 3. Skipfish
Skipfish is a web application security scanner developed by Google that performs comprehensive security assessments of web applications. It is known for its speed and efficiency in identifying vulnerabilities such as SQL injection, cross-site scripting (XSS), and directory traversal.
- YouTube Video: [Skipfish - Web Application Security Scanner](https://www.youtube.com/watch?v=tbAxjM8sQQ8)
  - Command: `skipfish`

#### 4. SQLMap
SQLMap is a powerful open-source tool used for automated SQL injection and database takeover attacks against web applications. It helps security testers identify and exploit SQL injection vulnerabilities by automatically detecting and exploiting them to retrieve database contents.
- YouTube Video: [SQLMap - SQL Injection Tool](https://www.youtube.com/watch?v=CvIhJfmZw0s)
  - Command: `sqlmap`

#### 5. WebShells
WebShells are malicious scripts or programs that attackers upload to compromised web servers to gain remote access and control over the server. They can be used to execute arbitrary commands, upload/download files, and perform various other malicious activities on the server.

#### 6. WPScan
WPScan is a WordPress vulnerability scanner that identifies security vulnerabilities and misconfigurations in WordPress websites. It specifically targets WordPress installations and plugins, providing security testers with valuable insights into potential weaknesses that could be exploited by attackers.
- YouTube Video: [WPScan - WordPress Vulnerability Scanner](https://www.youtube.com/watch?v=M1mSQ2Ngt3A)
  - Command: `wpscan`

<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>
</details>

<details>
<summary> 
<h2>Database Assessment</h2><br>

Database Assessment involves evaluating the security of databases to identify vulnerabilities and weaknesses that could compromise the confidentiality, integrity, and availability of data stored within them.
</summary>

 <summary><h3>Database Assessment Tools</h3></summary>

#### 1. SQLite Database Browser:
 SQLite Database Browser is a graphical tool used for browsing, analyzing, and managing SQLite database files. It provides a user-friendly interface for viewing table structures, executing SQL queries, and exporting data.
Command: N/A

#### 2.SQLMap:
 SQLMap is a powerful open-source tool used for automated SQL injection and database takeover attacks against web applications. It helps security testers identify and exploit SQL injection vulnerabilities by automatically detecting and exploiting them to retrieve database contents.
Command: sqlmap -u <URL>

<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>
</details>

<details>
<summary><h2>Password Attacks</h2><br>Password attacks involve methods used to gain unauthorized access to systems or accounts by guessing or cracking passwords.</summary>

### Password Attacks Techniques

Password attacks are methods used to gain unauthorized access to systems or accounts by guessing or cracking passwords.

#### 1. Offline Attacks

Offline attacks involve attempting to crack password hashes obtained from a system or database.

#### 2. Online Attacks

Online attacks involve attempting to log in to a system or service using a list of possible passwords, often through automated means.

#### 3. Passing the Hash Tools

Passing the hash is a technique used to authenticate to a system using the hashed password instead of the actual plaintext password.

#### 4. Password Profiling & Wordlists

Password profiling involves gathering information about a target user to create custom wordlists tailored to their likely passwords.

### Password Attacks Tools

Password attacks tools are software applications designed to facilitate the process of cracking passwords.

#### 1. crewl

crew is a password list generation tool that creates custom wordlists based on various criteria such as word length, character sets, and patterns.

- YouTube Video: [crew - Password List Generation Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `crew <options>`
    ```
    crew <options>
    ```

#### 2. crunch

crunch is a wordlist generator that allows users to create custom wordlists of a specified length and character set.

- YouTube Video: [crunch - Wordlist Generation Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `crunch <options>`
    ```
    crunch <options>
    ```

#### 3. hashcat

hashcat is a password recovery tool that supports various hashing algorithms and attack modes for cracking password hashes.

- YouTube Video: [hashcat - Password Recovery Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `hashcat <options>`
    ```
    hashcat <options>
    ```

#### 4. hydra

hydra is a network logon cracker that supports multiple protocols for brute-forcing passwords, including HTTP, FTP, SSH, Telnet, and more.

- YouTube Video: [hydra - Network Logon Cracker](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `hydra <options>`
    ```
    hydra <options>
    ```

#### 5. john

john, also known as John the Ripper, is a fast password cracker that supports various cracking modes and hash types.

- YouTube Video: [john - Password Cracker](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `john <options>`
    ```
    john <options>
    ```

#### 6. medusa

medusa is a command-line tool for network authentication brute-forcing, supporting various protocols and services.

- YouTube Video: [medusa - Network Authentication Brute-Forcer](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `medusa <options>`
    ```
    medusa <options>
    ```

#### 7. ncrack

ncrack is a high-speed network authentication cracking tool that supports multiple protocols and services, designed for efficiency and reliability.

- YouTube Video: [ncrack - Network Authentication Cracker](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `ncrack <options>`
    ```
    ncrack <options>
    ```

#### 8. ophcrack

ophcrack is a Windows password cracker based on rainbow tables. It can recover passwords from hashes using precomputed tables.

- YouTube Video: [ophcrack - Windows Password Cracker](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `ophcrack <options>`
    ```
    ophcrack <options>
    ```

#### 9. wordlists

Wordlists are collections of words, phrases, or character combinations used in password attacks to guess or crack passwords.

- YouTube Video: [Wordlists - Password Attack Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `wordlists <options>`
    ```
    wordlists <options>
    ```
<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>

</details>

<details>
<summary><h2>Wireless Attacks</h2><br>Wireless attacks involve techniques and tools used to exploit vulnerabilities in wireless networks and devices.</summary>

### Wireless Attacks Techniques

Wireless attacks techniques involve methods used to exploit vulnerabilities in wireless networks and devices.

#### 1. 802.11 Wireless Tools

802.11 wireless tools are a set of utilities used for monitoring, analyzing, and attacking Wi-Fi networks. These tools enable users to capture packets, crack encryption keys, and perform various attacks against wireless networks.

#### 2. Bluetooth Tools

Bluetooth tools are specialized utilities designed for analyzing and attacking Bluetooth-enabled devices and networks. These tools allow users to sniff Bluetooth traffic, perform device fingerprinting, and exploit vulnerabilities in Bluetooth implementations.

### Wireless Attacks Tools

Wireless attacks tools are software applications specifically developed for conducting attacks against wireless networks and devices.

#### 1. aircrack-ng

Aircrack-ng is a suite of tools used for assessing Wi-Fi network security. It includes tools for capturing packets, analyzing wireless traffic, and performing attacks such as brute-force cracking of WEP and WPA/WPA2 encryption keys.

- YouTube Video: [Aircrack-ng - Wi-Fi Network Security Assessment](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `aircrack-ng <options>`
    ```
    aircrack-ng <options>
    ```

#### 2. fern wifi cracker (root)

Fern Wifi Cracker is a wireless security auditing and attack tool written in Python. It provides a graphical user interface (GUI) for performing various Wi-Fi attacks, including WEP and WPA/WPA2 key cracking.

- YouTube Video: [Fern Wifi Cracker - Wireless Security Auditing Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `fern-wifi-cracker`
    ```
    fern-wifi-cracker
    ```

#### 3. kismet

Kismet is a wireless network detector, sniffer, and intrusion detection system. It can detect and analyze Wi-Fi networks, Bluetooth devices, and other wireless communications, providing detailed information about nearby wireless activity.

- YouTube Video: [Kismet - Wireless Network Detector and IDS](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `kismet`
    ```
    kismet
    ```

#### 4. pixiewps

Pixiewps is a tool for exploiting the WPS (Wi-Fi Protected Setup) vulnerability to recover WPA/WPA2 passphrases. It performs offline brute-force attacks against the WPS PIN, allowing attackers to retrieve the Wi-Fi password.

- YouTube Video: [Pixiewps - WPS PIN Recovery Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `pixiewps <options>`
    ```
    pixiewps <options>
    ```

#### 5. reaver

Reaver is a popular tool for exploiting the WPS vulnerability to crack WPA/WPA2-PSK passwords. It performs brute-force attacks against the WPS PIN, attempting to recover the Wi-Fi passphrase through automated PIN guessing.

- YouTube Video: [Reaver - WPS PIN Attack Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `reaver <options>`
    ```
    reaver <options>
    ```

#### 6. wifite

Wifite is a wireless auditing tool that automates the process of testing and securing Wi-Fi networks. It combines various wireless attack tools such as Aircrack-ng, Wifite, and Reaver into a single script, simplifying the process of capturing handshakes and cracking passwords.

- YouTube Video: [Wifite - Automated Wireless Attack Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `wifite <options>`
    ```
    wifite <options>
    ```

</details>


<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>
