# Network case study

Designing a network architecture for a setup that includes a web server for a webshop, a database with user login credentials, workstations for office workers, a printer, an Active Directory (AD) server, and a file server involves several considerations to ensure security, efficiency, and scalability. Here's a proposed architecture and the rationale behind the design decisions:

### 1. Network Segmentation

**Proposed Design**:
- **Public Segment**: This segment includes the web server. It should be placed in a Demilitarized Zone (DMZ) to ensure that it is separated from the internal network. This is critical for security purposes.
- **Private Segment**: This segment includes the database server, AD server, file server, workstations, and printer. These components should be on a separate network segment from the web server to enhance security and reduce the risk of external attacks reaching the internal network.

**Rationale**: Segregating the network into public and private segments ensures that external access is limited to the web server in the DMZ, protecting the internal network components from direct access from the internet. The database, although related to the web server, should not be directly accessible from the public internet for security reasons.

### 2. Network Devices and Infrastructure

- **Firewall**: A firewall should be configured between the internet and the DMZ, and between the DMZ and the private network. The firewall will manage and monitor traffic, allowing only specific types of traffic to pass through to the internal network based on predefined security rules.
- **Switches**: Managed switches should be used within the private network to connect workstations, the printer, the AD server, and the file server. This allows for better control and segmentation within the internal network.
- **Router**: A router should be used to connect the internal network with the external internet, providing NAT (Network Address Translation) services for internal devices.

**Rationale**: These devices are essential for managing traffic flow, enhancing security, and providing connectivity within the network and to the internet. The firewall is particularly critical for protecting the network from unauthorized access and attacks.

### 3. Security Measures

- **VPN Access**: For remote access to the private network, a VPN (Virtual Private Network) should be set up. This allows office workers to securely connect to the internal network from remote locations.
- **Antivirus and Anti-Malware**: All workstations and servers should have antivirus and anti-malware software installed to protect against threats.
- **Regular Backups**: Regular backups of the database and file server should be conducted to prevent data loss in case of a hardware failure or cyber attack.

**Rationale**: Security measures are essential to protect sensitive data, especially user login credentials and internal documents. VPN access ensures secure remote connections, while antivirus and anti-malware software help protect against software threats.

### 4. Network Services

- **Active Directory (AD) Server**: The AD server manages user identities and access controls within the network, facilitating authentication and authorization for users accessing network resources.
- **File Server**: The file server hosts internal documents and should have access controls configured to ensure that only authorized users can access sensitive information.

**Rationale**: These services are crucial for managing access to network resources and ensuring that only authorized personnel have access to sensitive information.

### Conclusion

To visualize the network architecture described earlier, we can create a flowchart that outlines the main components and their interconnections. Here's an overview of what the flowchart will include:

1. **Internet Connection** as the entry point.
2. **Firewall** separating the internet from the DMZ and the private network.
3. **DMZ (Demilitarized Zone)** containing:
   - Web Server for the webshop.
4. **Private Network** segment, further divided into:
   - Database Server for user login credentials, not directly accessible from the DMZ but can communicate with the web server.
   - Active Directory (AD) Server for managing user identities and access controls.
   - File Server for hosting internal documents with access controls.
   - Workstations for office workers.
   - Printer accessible within the private network.
5. **Security Measures** such as VPN access, antivirus, and backup solutions are indicated as overarching layers or services affecting multiple components.

Let's generate a flowchart based on this structure.

The flowchart for the described network architecture is ready. This diagram visualizes the main components of the network and their connections, emphasizing the separation between the DMZ and the private network, as well as highlighting the security measures that apply across the network.

![Network Architecture Flowchart](https://github.com/techgrounds/cloud-assignments-hollowearthyes/blob/094d7095f319c3d6b51ad1c55b0cbc5d92e86522/00_includes/Networking/networkcasestudy.png)