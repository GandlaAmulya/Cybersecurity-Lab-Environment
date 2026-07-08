# ApexPlanet Cybersecurity Lab

## Project Overview

This project demonstrates the setup of a cybersecurity testing environment using Kali Linux and Metasploitable2 in Oracle VirtualBox. The lab environment was used to perform network communication testing, packet capture, port scanning, and cryptographic operations using industry-standard cybersecurity tools.

---

## Tools Used

* Oracle VirtualBox
* Kali Linux
* Metasploitable2
* Wireshark
* Nmap
* OpenSSL

---

## Lab Environment

### Kali Linux

* Operating System used for security testing and analysis.

### Metasploitable2

* Intentionally vulnerable machine used for cybersecurity practice.

### Network Configuration

* Adapter Type: Host-Only Adapter
* Kali Linux IP: 192.168.56.101
* Metasploitable2 IP: 192.168.56.102

---

## Tasks Performed

### 1. Connectivity Testing

A ping test was performed to verify communication between Kali Linux and Metasploitable2.

Command:

```bash
ping 192.168.56.102
```

Result:

* Successful communication established between both virtual machines.

---

### 2. Packet Capture Using Wireshark

Wireshark was used to capture and analyze network packets.

Activities:

* Started packet capture on the active network interface.
* Generated traffic using the ping command.
* Observed captured packets and protocol information.

Result:

* Network traffic successfully captured and analyzed.

---

### 3. Port Scanning Using Nmap

Nmap was used to identify open ports and active services running on Metasploitable2.

Command:

```bash
nmap 192.168.56.102
```

Sample Open Services:

* FTP (21)
* SSH (22)
* Telnet (23)
* HTTP (80)

Result:

* Multiple open ports and services identified successfully.

---

### 4. OpenSSL Encryption and Decryption

A file was encrypted and decrypted using AES-256-CBC encryption.

Commands:

```bash
echo "Hello ApexPlanet" > message.txt

openssl enc -aes-256-cbc -salt -in message.txt -out message.enc

openssl enc -d -aes-256-cbc -in message.enc -out decrypted.txt

cat decrypted.txt
```

Output:

```text
Hello ApexPlanet
```

Result:

* File encryption and decryption completed successfully.

---

## Learning Outcomes

Through this project, the following concepts were learned:

* Virtual machine setup and management
* Host-only network configuration
* Linux command-line operations
* Network connectivity testing
* Packet capture and analysis
* Port scanning and service discovery
* Basic cryptography using OpenSSL
* Cybersecurity lab deployment

---

## Conclusion

The cybersecurity lab environment was successfully configured using Kali Linux and Metasploitable2. The project demonstrated practical usage of Wireshark, Nmap, and OpenSSL for cybersecurity-related tasks. This lab provided hands-on experience with essential security tools and networking concepts used in real-world environments.
