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

