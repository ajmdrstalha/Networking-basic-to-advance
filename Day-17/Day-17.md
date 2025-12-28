## 📘 Day 17 – Switch Configuration Basics

### 🧩 1. What is a Switch?

A **switch** is a network device that **connects multiple devices within a LAN** and forwards data based on **MAC addresses**.

- Operates at **Layer 2 (Data Link Layer)**  
- Reduces network collisions compared to hubs  
- Can be managed or unmanaged  

Example:
- Connecting PCs, printers, and servers in an office network  

---

### 🔢 2. Types of Switches

| Type | Description |
|------|-------------|
| Unmanaged Switch | Simple plug-and-play switch with no configuration |
| Managed Switch | Configurable switch with VLANs, QoS, security features |
| Smart Switch | Limited management capabilities, cost-effective |
| PoE Switch | Provides Power over Ethernet for devices like IP cameras |

---

### 🔁 3. Basic Switch Operations

- Learning MAC addresses of connected devices  
- Forwarding frames to correct ports  
- Filtering unnecessary traffic  
- Supporting VLANs and trunking (if managed)  

---

### ⚙️ 4. Switch CLI Commands (Cisco Example)

- Access switch CLI via console or SSH  
- Common commands:

enable # Enter privileged mode
configure terminal # Enter global config mode
hostname Switch1 # Set switch name
interface fastEthernet0/1
switchport mode access # Configure port as access
switchport access vlan 10
show running-config # View current configuration
show vlan brief # View VLAN assignments

yaml
Copy code

---

### 🗂️ 5. Practical / Lab Practice

- Connect PCs to a switch and test connectivity  
- Assign ports to different VLANs  
- Configure trunk port between two switches  
- Verify MAC address table using `show mac address-table`  
- Observe frame forwarding in a simple LAN  

---

### 🧠 6. Key Terms

- **Switchport:** Physical interface on a switch  
- **Access Port:** Port assigned to a single VLAN  
- **Trunk Port:** Port carrying multiple VLANs  
- **MAC Table:** Stores MAC addresses and corresponding ports  
- **PoE:** Power over Ethernet for devices  

---

### 📘 Day 17 Summary

✅ Learned what a switch is and its purpose  
✅ Explored types of switches  
✅ Practiced basic switch configuration  
✅ Verified VLAN and MAC table functionality 
