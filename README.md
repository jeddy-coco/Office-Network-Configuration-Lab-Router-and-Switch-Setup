# Office Network Configuration Lab – Router & Switch Setup

A simple office network simulation built-in **Cisco Packet Tracer**, where I configured **switch management, VLAN interfaces, and IP routing** between PCs and routers. This lab is a foundational setup for understanding end-device communication, switch setup, and router integration.

---

## 💡 What This Lab Demonstrates

- ✅ Basic switch management configuration  
- ✅ VLAN 1 interface setup on a switch  
- ✅ Assigning an IP address to the switch for remote management  
- ✅ Bringing up interfaces with `no shutdown`  
- ✅ Connecting PCs to switches and switches to a router  
- ✅ Preparing for inter-VLAN routing and further expansion

---

## 🖥️ Devices in the Topology

- **3 Switches** (Switch-PT)
- **1 Router** (2901)
- **6 PCs** (labeled PC0 to PC5)
- Interconnected via Ethernet with appropriate cable types

---

## 🔧 Configuration Steps Taken

On the **switch (Switch 4)**:
```bash
enable
configure terminal
interface vlan 1
ip address 192.168.1.1 255.255.255.0
no shutdown
exit
This:

Enables VLAN 1 interface

Assigns it an IP address for management (192.168.1.1/24)

Brings the interface up

All PCs are connected to switches, and switches are connected in a way to ensure communication reaches the router.

🧪 Purpose of the Lab
Practice basic Layer 2 and Layer 3 configurations

Set the stage for inter-VLAN routing, DHCP, port security, and remote management via Telnet/SSH

Understand the importance of VLAN interfaces and switch IP assignment for network management

📌 Next Steps
 Configure the router interface with a matching subnet

 Test PC-to-PC and PC-to-router communication using ping

 Enable Telnet or SSH access to switches

 Implement VLANs for better segmentation

💭 Notes
Don't forget: switches don't route, but they do need an IP for you to manage them!
Also, remember to no shutdown — or your interfaces will just sit there looking pretty but doing nothing. 😄

🧾 License
Feel free to use or remix this lab setup for your personal learning, classroom demos, or late-night troubleshooting marathons.
