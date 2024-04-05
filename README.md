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
<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>

</details>

<details>
<summary><h2>Reverse Engineering</h2><br>Reverse engineering is the process of analyzing and understanding the structure and behavior of software systems, hardware components, or other artifacts to extract design information, discover vulnerabilities, or replicate functionality without access to the original source code or documentation.</summary>

### Reverse Engineering Tools

Reverse engineering tools are software applications used to analyze, disassemble, decompile, debug, and manipulate binaries, executables, and other artifacts.

#### 1. NASM Shell

NASM Shell is an interactive shell for the Netwide Assembler (NASM), a popular assembler used for creating assembly language programs. It provides a command-line interface for assembling and debugging x86 assembly code.

- YouTube Video: [NASM Shell - Interactive Assembly Language Programming](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `nasm -f elf32 -o output.o input.asm`
    ```
    nasm -f elf32 -o output.o input.asm
    ```

#### 2. clang

Clang is a C language family frontend for LLVM, providing support for compiling C, C++, and Objective-C programs. It offers a modern compiler infrastructure with features such as static analysis, code generation, and optimization.

- YouTube Video: [Clang - C Language Frontend for LLVM](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `clang -o output input.c`
    ```
    clang -o output input.c
    ```

#### 3. clang++

Clang++ is the C++ language frontend for LLVM, extending the capabilities of Clang to support compiling C++ programs. It offers compatibility with modern C++ standards and features for static analysis, code generation, and optimization.

- YouTube Video: [Clang++ - C++ Language Frontend for LLVM](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `clang++ -o output input.cpp`
    ```
    clang++ -o output input.cpp
    ```

#### 4. radare2

Radare2 is a powerful command-line framework for reverse engineering and analyzing binaries. It provides a wide range of features, including disassembly, debugging, patching, scripting, and binary analysis, making it a versatile tool for reverse engineering tasks.

- YouTube Video: [Radare2 - Command-Line Reverse Engineering Framework](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `radare2 <binary>`
    ```
    radare2 <binary>
    ```

</details>

<details>
<summary><h2>Exploitation Tools</h2><br>Exploitation tools are software applications used by security professionals and penetration testers to exploit vulnerabilities in target systems, applications, or networks. These tools often automate the process of identifying, exploiting, and gaining unauthorized access to vulnerable systems, allowing testers to assess the security posture of their targets and remediate vulnerabilities.</summary>

### Exploitation Tools

Exploitation tools encompass a variety of software applications designed to identify, exploit, and gain unauthorized access to vulnerable systems, applications, or networks.

#### 1. crackmapexec

CrackMapExec is a post-exploitation tool that can be used to assess and exploit Windows-based systems. It provides features for gathering information, executing commands, and exploiting vulnerabilities in Windows environments.

- YouTube Video: [CrackMapExec - Post-Exploitation Tool for Windows Systems](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `crackmapexec <options>`
    ```
    crackmapexec <options>
    ```

#### 2. Metasploit Framework

Metasploit Framework is a penetration testing platform that enables security researchers and penetration testers to exploit vulnerabilities, create payloads, and conduct post-exploitation activities. It provides a wide range of modules and payloads for various exploitation scenarios.

- YouTube Video: [Metasploit Framework - Penetration Testing](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `msfconsole`
    ```
    msfconsole
    ```

#### 3. MSF Payload Creator

MSF Payload Creator is a tool used for generating various payloads compatible with the Metasploit Framework. It allows users to create custom payloads tailored to their specific exploitation needs, including reverse shells, bind shells, and meterpreter sessions.

- YouTube Video: [MSF Payload Creator - Payload Generation Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `msfvenom <options>`
    ```
    msfvenom <options>
    ```

#### 4. SearchSploit

SearchSploit is a command-line utility for searching and displaying information about exploits and vulnerabilities from the Exploit Database. It allows users to quickly find relevant exploit scripts and details about vulnerabilities that can be exploited in target systems.

- YouTube Video: [SearchSploit - Exploit Database Search Utility](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `searchsploit <search_query>`
    ```
    searchsploit <search_query>
    ```

#### 5. Social Engineering Toolkit (SET)

The Social Engineering Toolkit (SET) is a versatile toolkit for performing social engineering attacks, including phishing campaigns, credential harvesting, and exploitation of human vulnerabilities. It provides a range of attack vectors and modules for crafting convincing social engineering scenarios.

- YouTube Video: [Social Engineering Toolkit (SET) - Exploiting Human Vulnerabilities](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `setoolkit`
    ```
    setoolkit
    ```

#### 6. SQLMap

SQLMap is a popular open-source penetration testing tool used for detecting and exploiting SQL injection vulnerabilities in web applications and databases. It automates the process of identifying SQL injection flaws and extracting sensitive data from vulnerable systems.

- YouTube Video: [SQLMap - Automated SQL Injection Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `sqlmap <options>`
    ```
    sqlmap <options>
    ```

<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>
</details>

<details>
<summary><h2>Sniffling & Spoofing</h2><br>Sniffling & Spoofing techniques and tools are commonly used in network security testing and ethical hacking to intercept network traffic, analyze it for vulnerabilities, and spoof or manipulate network packets for various purposes.</summary>

### Sniffling & Spoofing Techniques

Sniffling & Spoofing techniques involve methods for intercepting and manipulating network traffic to achieve different objectives.

#### 1. Network Sniffers

Network sniffers are tools used to capture and analyze network traffic passing through a network interface. They enable security professionals to inspect packets, extract information, and identify potential security vulnerabilities, such as unencrypted data transmission or insecure protocols.

#### 2. Spoofing & MTM (Man-in-the-Middle)

Spoofing and Man-in-the-Middle (MITM) attacks involve intercepting communication between two parties and manipulating the traffic, often without their knowledge. These attacks can be used to eavesdrop on sensitive information, tamper with data, or impersonate legitimate entities.

### Sniffling & Spoofing Tools

Sniffling & Spoofing tools are software applications used to perform network sniffing, packet manipulation, and spoofing attacks in network security assessments and penetration testing.

#### 1. Ettercap Graphical

Ettercap Graphical is a comprehensive network sniffing and spoofing tool that supports various attack techniques, including ARP poisoning, DNS spoofing, and packet filtering. It provides a user-friendly graphical interface for performing Man-in-the-Middle (MITM) attacks and analyzing intercepted traffic.

- YouTube Video: [Ettercap - Network Sniffing and Spoofing Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `ettercap -G`
    ```
    ettercap -G
    ```

#### 2. Macchanger

Macchanger is a utility for changing the Media Access Control (MAC) address of network interfaces on a system. It allows users to spoof their MAC address to bypass MAC-based access controls or to conduct anonymous network activities.

- YouTube Video: [Macchanger - MAC Address Spoofing Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `macchanger -r <interface>`
    ```
    macchanger -r <interface>
    ```

#### 3. Minicom

Minicom is a terminal emulation program that allows users to interact with remote systems through serial communication. While not specifically designed for sniffing or spoofing, it can be used in conjunction with other tools for debugging and monitoring serial connections.

#### 4. mitmproxy

Mitmproxy is an interactive TLS-capable intercepting proxy for HTTP and HTTPS with a console interface. It allows for HTTP traffic inspection, modification, and replaying, making it useful for debugging, testing, and security assessment of web applications.

- YouTube Video: [Mitmproxy - Intercepting Proxy for HTTP/HTTPS](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `mitmproxy`
    ```
    mitmproxy
    ```

#### 5. Netsniff-ng

Netsniff-ng is a high-performance Linux network sniffer that provides tools for packet capture, analysis, and generation. It offers features for capturing packets at high speeds, filtering traffic based on specific criteria, and performing advanced protocol analysis.

#### 6. Responder

Responder is a tool for performing LLMNR, NBT-NS, and MDNS poisoning attacks to capture user credentials transmitted over the network. It listens for specific network traffic and responds with fake authentication requests to trick users into disclosing their credentials.

#### 7. Scapy

Scapy is a powerful interactive packet manipulation program and library for Python. It allows users to forge or decode packets, send them on the wire, capture them, match requests and replies, and more. Scapy can be used for network analysis, testing, and troubleshooting.

- YouTube Video: [Scapy - Packet Manipulation with Python](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `scapy`
    ```
    scapy
    ```

#### 8. Tcpdump

Tcpdump is a command-line packet analyzer that allows users to capture and display TCP/IP packets transmitted or received over a network interface. It provides extensive filtering options and can save captured packets to a file for later analysis.

- YouTube Video: [Tcpdump - Packet Capture and Analysis](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `tcpdump <options>`
    ```
    tcpdump <options>
    ```

#### 9. Wireshark

Wireshark is a widely-used network protocol analyzer that allows users to capture and interactively browse the traffic running on a computer network. It provides a rich set of features for deep inspection of hundreds of protocols, live capture, offline analysis, and packet editing.

- YouTube Video: [Wireshark - Network Protocol Analyzer](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `wireshark`
    ```
    wireshark
    ```

<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>
</details>

<details>
<summary><h2>Post Exploitation</h2><br>Post Exploitation techniques and tools are utilized by attackers after gaining unauthorized access to a system or network to maintain control, extract sensitive information, or perform further malicious activities.</summary>

### Post Exploitation Techniques

Post Exploitation techniques involve methods used by attackers to maintain access, exfiltrate data, or establish persistence after compromising a system or network.

#### 1. OS Backdoors

OS Backdoors are stealthy mechanisms installed on compromised systems to provide attackers with persistent access and control. These backdoors often include remote access tools or hidden user accounts that allow attackers to maintain control over the compromised system.

#### 2. Tunneling & Exfiltration

Tunneling & Exfiltration techniques involve establishing covert communication channels between the attacker's system and the compromised network to bypass security controls and exfiltrate sensitive data. Attackers may use techniques such as encrypted tunnels, covert channels, or data compression to transfer stolen information without detection.

#### 3. Web Backdoors

Web Backdoors are malicious scripts or applications installed on web servers to provide unauthorized access and control to attackers. These backdoors often exploit vulnerabilities in web applications or server configurations to upload and execute malicious code, allowing attackers to maintain persistence and perform further actions.

### Post Exploitation Tools

Post Exploitation tools are software applications used by attackers to maintain control, exfiltrate data, or perform malicious activities on compromised systems or networks.

#### 1. evil-winrm

Evil-WinRM is a Windows Remote Management tool that allows attackers to execute commands remotely on compromised Windows systems. It provides a command-line interface similar to Windows PowerShell, allowing attackers to interact with compromised systems and execute arbitrary commands.

- YouTube Video: [Evil-WinRM - Windows Remote Management Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `evil-winrm -i <target> -u <username> -p <password>`
    ```
    evil-winrm -i <target> -u <username> -p <password>
    ```

#### 2. exe2hex

Exe2Hex is a tool used to convert executable files (EXE) into hexadecimal format. This can be useful for bypassing security controls or antivirus detection by embedding the executable within other files or disguising it as harmless data.

#### 3. Impacket

Impacket is a collection of Python scripts for working with network protocols. It includes tools for creating and manipulating network packets, performing password attacks, and exploiting vulnerabilities in Windows systems. Impacket is widely used by penetration testers and red teamers for post-exploitation activities.

- YouTube Video: [Impacket - Python Network Protocol Library](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `impacket <options>`
    ```
    impacket <options>
    ```

#### 4. Mimikatz

Mimikatz is a powerful post-exploitation tool that allows attackers to extract plaintext passwords, hashes, and other credentials from memory, registry hives, and other sensitive areas of Windows operating systems. It can also perform pass-the-hash attacks and escalate privileges on compromised systems.

- YouTube Video: [Mimikatz - Credential Dumping Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `mimikatz <options>`
    ```
    mimikatz <options>
    ```

#### 5. Netcat

Netcat (nc) is a versatile networking utility that can be used for reading and writing data across network connections. It is commonly used by attackers for creating reverse shells, transferring files, port scanning, and other post-exploitation tasks.

- YouTube Video: [Netcat - Networking Utility](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `nc <options>`
    ```
    nc <options>
    ```

#### 6. PowerShell Empire

PowerShell Empire is a post-exploitation framework that allows attackers to maintain control over compromised Windows systems using a variety of modules and agents. It provides a powerful command-and-control (C2) infrastructure for managing compromised hosts and executing post-exploitation tasks.

- YouTube Video: [PowerShell Empire - Post-Exploitation Framework](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `empire`
    ```
    empire
    ```

#### 7. PowerSploit

PowerSploit is a collection of PowerShell scripts that can be used for offensive security purposes, including post-exploitation activities. It includes modules for persistence, privilege escalation, credential theft, and lateral movement on Windows systems.

- YouTube Video: [PowerSploit - Offensive PowerShell Toolkit](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `powersploit <options>`
    ```
    powersploit <options>
    ```

#### 8. Proxychains4

Proxychains is a tool for routing TCP and DNS network traffic through proxy servers. It can be used by attackers to anonymize their network activities, bypass firewalls, and pivot through compromised systems during post-exploitation operations.

- YouTube Video: [Proxychains - Proxy Routing Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `proxychains4 <options>`
    ```
    proxychains4 <options>
    ```

#### 9. Starkiller

Starkiller is a cross-platform GUI for Empire, a post-exploitation framework for Windows. It provides a user-friendly interface for managing agents, modules, listeners, and other components of the Empire C2 infrastructure.

#### 10. Weevely

Weevely is a stealthy web shell that allows attackers to execute remote commands on compromised web servers. It provides a command-line interface for interacting with the target system, uploading and downloading files, and performing various post-exploitation tasks.

<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>
</details>

<details>
<summary><h2>Forensic</h2><br>Forensic techniques and tools are used in digital forensics investigations to collect, preserve, and analyze evidence from digital devices and systems. This process involves identifying and recovering digital artifacts, analyzing data structures, and reconstructing events to support legal proceedings or incident response activities.</summary>

### Forensic Techniques

Forensic techniques encompass various methods and procedures used in digital forensics investigations to collect, analyze, and interpret digital evidence.

#### 1. Forensic Carving Tools

Forensic Carving Tools are software applications used to recover deleted or damaged files from storage devices by searching for file signatures or specific patterns in raw data. These tools can reconstruct fragmented files and extract valuable evidence even from corrupted or partially overwritten storage media.

#### 2. Forensic Imaging Tools

Forensic Imaging Tools are used to create forensic images or exact copies of storage devices, including hard drives, USB drives, and memory cards. These tools ensure the preservation of digital evidence by capturing every bit of data stored on the original device, allowing forensic analysts to perform thorough investigations without altering the original evidence.

#### 3. PDF Forensics Tools

PDF Forensics Tools are specialized software applications used to analyze PDF (Portable Document Format) files for forensic purposes. These tools extract metadata, analyze document structure, and identify hidden content or malicious code embedded within PDF files, providing valuable insights for digital forensic investigations involving PDF documents.

#### 4. Sleuth Kit Suite

The Sleuth Kit (TSK) Suite is an open-source collection of forensic analysis tools designed to analyze disk images and perform file system analysis on various operating systems. It includes tools for file system examination, timeline analysis, keyword search, and metadata extraction, making it a valuable resource for digital forensic investigations.

### Forensic Tools

Forensic tools are software applications specifically designed for digital forensics investigations, providing capabilities for evidence collection, analysis, and reporting.

#### 1. autopsy (root)

Autopsy is a digital forensics platform that provides a graphical interface for analyzing disk images and performing file system analysis. It includes features for recovering deleted files, extracting artifacts, and generating detailed forensic reports, making it suitable for both novice and experienced forensic examiners.

- YouTube Video: [Autopsy - Digital Forensics Platform](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `autopsy`
    ```
    autopsy
    ```

#### 2. binwalk

Binwalk is a firmware analysis tool used for extracting embedded files and data from firmware images. It can identify file signatures, analyze compression algorithms, and extract filesystems or executable code from firmware images, making it valuable for analyzing IoT devices, embedded systems, and firmware-based attacks.

- YouTube Video: [Binwalk - Firmware Analysis Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `binwalk <options>`
    ```
    binwalk <options>
    ```

#### 3. bulk_extractor

Bulk Extractor is a digital forensics tool used for extracting information such as email addresses, credit card numbers, and other sensitive data from disk images or raw data files. It employs various scanning algorithms and regular expressions to identify and extract relevant information, making it useful for analyzing large datasets and identifying potential evidence.

- YouTube Video: [Bulk Extractor - Digital Forensics Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `bulk_extractor <options>`
    ```
    bulk_extractor <options>
    ```

#### 4. hasdeep

Hasdeep is a hash-based deduplication tool used to identify duplicate files within large datasets or disk images. It calculates cryptographic hashes (e.g., MD5, SHA-1) of files and compares them to identify duplicate content, allowing forensic examiners to reduce storage requirements and focus on unique or relevant data during investigations.

<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>
</details>

<details>
<summary><h2>Reporting Tools</h2><br>Reporting tools are essential components in cybersecurity to document and communicate findings, assessments, and recommendations effectively. These tools enable security professionals to generate comprehensive reports that summarize analysis results, vulnerabilities, incidents, and remediation actions for stakeholders, including clients, management, and regulatory bodies.</summary>

### Reporting Tools

Reporting tools facilitate the creation of detailed and visually appealing reports to convey cybersecurity findings and insights to various stakeholders.

#### 1. Cherry Tree

Cherry Tree is a hierarchical note-taking application with rich text formatting capabilities, making it suitable for organizing and documenting cybersecurity findings, notes, and observations. It supports the creation of structured documents with nested folders, checkboxes, hyperlinks, images, and more, allowing users to create comprehensive and well-organized reports.

- YouTube Video: [Cherry Tree - Note-Taking Application](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `cherrytree`
    ```
    cherrytree
    ```

#### 2. Cutycapt

Cutycapt is a command-line utility that captures screenshots of web pages, enabling security professionals to include visual representations of web-based findings in their reports. It supports various output formats, including PNG, JPEG, and PDF, and can render web pages with JavaScript, making it suitable for capturing dynamic web content for documentation purposes.

- YouTube Video: [Cutycapt - Web Page Screenshot Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `cutycapt --url=<URL> --out=<output_file>`
    ```
    cutycapt --url=<URL> --out=<output_file>
    ```

#### 3. Faraday Start

Faraday Start is a command-line tool for initiating the Faraday Collaborative Penetration Test and Vulnerability Management Platform. It allows users to launch the Faraday server and client applications, providing a centralized environment for conducting penetration tests, managing vulnerabilities, and generating comprehensive reports.

- YouTube Video: [Faraday - Collaborative Penetration Testing Platform](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `faraday`
    ```
    faraday
    ```

#### 4. Maltego (Installer)

Maltego is a data visualization tool used for open-source intelligence and forensics investigations. While the installer version facilitates the installation process, Maltego itself provides capabilities for generating graphical representations of complex relationships among entities gathered from various sources.

- YouTube Video: [Maltego CE Tutorial](https://www.youtube.com/watch?v=EXAMPLE)
  - Additional Information: Maltego offers Community Edition (CE) for free, with limited functionalities compared to the commercial version.
    ```
    Maltego offers Community Edition (CE) for free, with limited functionalities compared to the commercial version.
    ```

#### 5. Pipal

Pipal is a forensic tool used for analyzing password statistics and trends within a dataset, enabling security professionals to identify common passwords, password patterns, and password complexity levels. It generates statistical reports and visualizations to help assess the strength of password policies and identify potential weaknesses in authentication mechanisms.

- YouTube Video: [Pipal - Password Analysis Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `pipal <options>`
    ```
    pipal <options>
    ```

#### 6. RecordMyDesktop

RecordMyDesktop is a screen recording tool that captures desktop activities and interactions, allowing security professionals to create video demonstrations or tutorials for inclusion in cybersecurity reports. It supports various output formats and recording settings, making it suitable for documenting processes, procedures, and findings in a visually engaging format.

- YouTube Video: [RecordMyDesktop - Screen Recording Tool](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `recordmydesktop --output=<output_file>`
    ```
    recordmydesktop --output=<output_file>
    ```
    
<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>
</details>

<details>
<summary><h2>Social Engineering Tools</h2><br>Social engineering tools are designed to manipulate human behavior to obtain sensitive information, access, or privileges through deception and psychological manipulation. These tools simulate various social engineering attacks, such as phishing, pretexting, and baiting, to assess the security awareness and resilience of individuals and organizations.</summary>

### Social Engineering Tools

Social engineering tools enable security professionals to conduct simulated attacks to assess the susceptibility of individuals and organizations to social engineering tactics.

#### 1. Maltego (Installer)

Maltego is a data visualization tool used for open-source intelligence and forensics investigations. While the installer version facilitates the installation process, Maltego itself provides capabilities for generating graphical representations of complex relationships among entities gathered from various sources.

- YouTube Video: [Maltego CE Tutorial](https://www.youtube.com/watch?v=EXAMPLE)
  - Additional Information: Maltego offers Community Edition (CE) for free, with limited functionalities compared to the commercial version.
    ```
    Maltego offers Community Edition (CE) for free, with limited functionalities compared to the commercial version.
    ```

#### 2. MSF Payload Creator

MSF Payload Creator is a tool integrated into the Metasploit Framework for generating custom payloads for use in social engineering attacks. It allows security professionals to create tailored payloads with specific characteristics and functionalities to bypass security defenses and exploit vulnerabilities in target systems.

- YouTube Video: [MSF Payload Creator - Custom Payload Generation](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `msfvenom -p <payload> <options>`
    ```
    msfvenom -p <payload> <options>
    ```

#### 3. Social Engineering Toolkit (Root)

The Social Engineering Toolkit (SET) is a powerful framework for conducting social engineering attacks, including phishing, credential harvesting, and payload delivery. It provides a wide range of attack vectors and features, allowing security professionals to simulate real-world social engineering scenarios and assess the security posture of organizations.

- YouTube Video: [Social Engineering Toolkit (SET) - Overview and Usage](https://www.youtube.com/watch?v=EXAMPLE)
  - Command: `setoolkit`
    ```
    setoolkit
    ```
    
</details>


<a href="#top" style="position: fixed; bottom: 20px; right: 20px; padding: 10px 20px; background-color: #007bff; color: white; text-decoration: none;">Back to Top</a>
