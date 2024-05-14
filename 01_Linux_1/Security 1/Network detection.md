# Network Analysis Exercise

## Introduction
In this exercise, we explore network analysis using two popular tools: nmap and Wireshark. 

**Nmap** is a network scanning tool used to discover information about hosts and services on a network. It can provide details such as open ports on a host.

**Wireshark** is a protocol analyzer that captures and displays the data traveling back and forth on a network in real-time. It allows for in-depth analysis of network traffic, including packet inspection.

## Key Terms
- **nmap**: A network scanning tool used to discover hosts and services on a network.
- **Wireshark**: A protocol analyzer for network traffic analysis.
- **Open Ports**: Network ports that are actively accepting communications.
- **SSH**: Secure Shell, a cryptographic network protocol for operating network services securely over an unsecured network.

## Requirements
- Linux machine
- Wireshark

## Study

### Nmap Scan
- Executed the following command to scan the network of the Linux machine:  
  ```
  sudo nmap -sV -sT -Pn ipaddress -p port 
  ```
  ```
  sudo nmap -sV -sT -Pn ipaddress  
  ```
- Discovered that only the SSH port (52201/tcp) is open.
- Configured a firewall (ufw) to only allow specific ports.

### nmap output

PORT      STATE SERVICE VERSION
52201/tcp open  ssh     OpenSSH 8.2p1 Ubuntu 4ubuntu0.11 (Ubuntu Linux; protocol 2.0)
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

### Wireshark Analysis
- Opened Wireshark on a Linux machine.
- Analyzed network traffic while opening an internet browser.
- Noticed constant packets sent by Zoom and focused on packets sent by the browser.

## Used Sources
- [Nmap Official Documentation](https://nmap.org/)
- [Wireshark User Guide](https://www.wireshark.org/docs/)

## Experienced Issues
- Initially faced challenges configuring the firewall (ufw) to allow specific ports. Resolved by consulting the ufw documentation and adjusting the rules accordingly.

## Result
- Successfully analyzed the network using nmap, identifying only the SSH port as open.
- Analyzed network traffic with Wireshark, focusing on browser packets amidst Zoom traffic.

![nmap result](https://github.com/techgrounds/cloud-assignments-hollowearthyes/blob/e8b60d17c57b0bb5c010b94a7311224b7e1a5388/00_includes/Security1/Nmapscan.png)