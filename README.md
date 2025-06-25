# DNS Troubleshooting Lab – Windows Server 2019 & Windows 10

This self-directed lab simulates a DNS resolution failure in a small enterprise IT environment using **Windows Server 2019** as a DNS server and **Windows 10** as a client. The goal is to identify, troubleshoot, and resolve a common DNS issue encountered in real-world IT support scenarios.

---

## Lab Objective

- Simulate a DNS resolution failure on a client machine
- Diagnose the issue using built-in Windows tools (`ping`, `nslookup`, `ipconfig`)
- Configure and test a Windows DNS Server with internal zones
- Set up forwarders to allow public DNS resolution
- Create both **Forward** and **Reverse Lookup Zones**
- Verify name-to-IP and IP-to-name resolution

---

## Lab Environment

| Component      | Configuration            |
|----------------|--------------------------|
| Host Machine   | Ubuntu (VirtualBox Host) |
| VM 1           | Windows Server 2019 (DC01) – DNS + AD DS |
| VM 2           | Windows 10 (Client01)     |
| Network Type   | Host-only + NAT (Dual Adapter) |

---

## Simulated Issue

The client was configured with an incorrect DNS server (`8.8.9.9`) and failed to resolve domain names.  
The DNS server itself was initially unable to reach external DNS servers due to lack of internet access.

---

## Solution Steps

1. **Configure static IP and DNS on Client01**
2. **Install and configure DNS Server role on DC01**
3. **Set up DNS forwarders to Google DNS (`8.8.8.8`, `1.1.1.1`)**
4. **Reconfigure networking to allow NAT (internet access)**
5. **Create internal DNS Forward and Reverse Lookup Zones**
6. **Add A and PTR records for `dc01.lab.local`**
7. **Verify resolution using `ping`, `nslookup`, and `ipconfig`**

---

## Screenshots
Will update soon

- DNS misconfiguration
- `nslookup` failures
- Server role setup
- DNS zone creation
- Successful lookups after fixing

---

## Skills Practiced

- DNS Server installation and configuration
- Forwarders and internal DNS zone management
- Reverse DNS (PTR record) setup
- Real-world network troubleshooting
- Windows Server & Client environment management

---


