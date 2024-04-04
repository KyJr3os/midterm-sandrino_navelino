**Midterm-Sandrino_Navelino**
# **Kali Linux Tools** 

Kali Linux is a widely used Linux distribution specifically designed for digital forensics and penetration testing. It comes pre-installed with numerous tools categorized into various domains such as information gathering, vulnerability analysis, exploitation, wireless attacks, reverse engineering, and more. Here's a brief overview of some of the categories and tools available in Kali Linux:

<details>
<summary><h2>Information Gathering</h2></summary>

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

</details>
