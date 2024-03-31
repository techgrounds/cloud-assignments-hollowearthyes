# Network Protocols and Wireshark Analysis

## Description
This document explores network protocols across different layers of the OSI model and introduces Wireshark, a powerful tool for network analysis. It covers the basics of various protocols, their OSI layer, and provides an exercise on capturing and analyzing network data using Wireshark.

### Key Terms
- OSI Model: Open Systems Interconnection model, a conceptual framework that standardizes the functions of a telecommunication or computing system into seven abstraction layers.
- TCP: Transmission Control Protocol, a connection-oriented protocol that provides reliable, ordered, and error-checked delivery of data.
- UDP: User Datagram Protocol, a connectionless protocol that provides a faster but less reliable service compared to TCP.
- HTTPS: Hypertext Transfer Protocol Secure, an extension of HTTP for secure communication over a computer network, widely used on the Internet.
- SSH: Secure Shell, a cryptographic network protocol for operating network services securely over an unsecured network.
- Wireshark: A popular network protocol analyzer used for troubleshooting, analysis, development, and education.

## Exercise
### Identify Protocols and OSI Layers
- **Layer 1 (Physical)**: Ethernet - responsible for the physical connection between devices.
- **Layer 2 (Data Link)**: MAC (Media Access Control) - controls how data is placed and received from the physical layer.
- **Layer 3 (Network)**: IP (Internet Protocol) - responsible for routing packets across networks.
- **Layer 5 (Session)**: NetBIOS (Network Basic Input/Output System) - manages sessions between computers.
- **Layer 6 (Presentation)**: SSL/TLS (Secure Sockets Layer/Transport Layer Security) - handles the presentation of data in a secure manner.
- **Layer 7 (Application)**: HTTP (Hypertext Transfer Protocol) - facilitates communication between web browsers and servers.

### Introduction of New Protocol
- The introduction of a new protocol involves defining its specifications, including its purpose, message format, and behavior.
- Standards organizations like the IETF (Internet Engineering Task Force) or IEEE (Institute of Electrical and Electronics Engineers) typically determine protocols.
- To introduce a new protocol, one needs to adhere to the standards set by these organizations, ensure compatibility with existing systems, and possibly gain acceptance through community review and adoption.

### Wireshark Analysis
- Install Wireshark from the official website: [Wireshark Download](https://www.wireshark.org/download.html)
- Capture network traffic using Wireshark.
- Filter captured packets by a specific protocol, e.g., HTTP or TCP.
- Analyze packet details, including headers, payloads, and source/destination addresses.

## Used Sources
- "Computer Networking: Principles, Protocols and Practice" by Olivier Bonaventure
- Wireshark Documentation and Tutorials

## Experienced Problems
No significant problems were encountered during the completion of this exercise. 

## Result
The exercise was successful. Screenshots of Wireshark capturing network data and analyzing a specific protocol (e.g., HTTP) were obtained. The understanding of network protocols and Wireshark functionalities was enhanced through practical application. 

![ERROR](https://www.google.com/url?sa=i&url=https%3A%2F%2Fmedium.com%2F%40kumarishefu.4507%2Ftry-hack-me-wireshark-traffic-analysis-write-up-part-2-11d299b504f3&psig=AOvVaw0feFZpmTAWNfFu16isnbiA&ust=1711968699019000&source=images&cd=vfe&opi=89978449&ved=0CBIQjRxqFwoTCLDjk8SqnoUDFQAAAAAdAAAAABAD)

