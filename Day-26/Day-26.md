## 📘 Day 26 – Introduction to VLANs & Trunking

### 🧩 1. What is a VLAN?

**VLAN (Virtual Local Area Network)** is a logical segmentation of a physical LAN into **multiple broadcast domains**.

- Improves network security and performance  
- Reduces unnecessary broadcast traffic  
- Allows grouping of devices regardless of physical location  

Example:
- Separate VLANs for HR, Finance, and IT departments in the same office  

---

### 🔢 2. Types of VLANs

| Type | Description |
|------|-------------|
| Default VLAN | All switch ports belong by default (usually VLAN 1) |
| Data VLAN | Carries user-generated traffic |
| Voice VLAN | Dedicated for VoIP traffic |
| Management VLAN | For switch management access |
| Native VLAN | Used for untagged traffic on a trunk port |

---

### 🔁 3. What is Trunking?

**Trunking** allows a **single switch port to carry traffic for multiple VLANs**.

- Uses VLAN tagging (IEEE 802.1Q standard)  
- Essential for inter-switch communication  
- Preserves VLAN identity across switches  

Example:
- Switch1 VLAN 10, VLAN 20 → trunk link → Switch2 receives both VLANs  

---

### ⚙️ 4. Basic Configuration Concepts

- Assign VLAN to access ports:  
interface fastEthernet0/1
switchport mode access
switchport access vlan 10

css
Copy code

- Configure a trunk port:  
interface gig0/1
switchport mode trunk
switchport trunk allowed vlan 10,20

diff
Copy code

- Verify configuration:  
show vlan brief
show interfaces trunk

yaml
Copy code

---

### 🗂️ 5. Practical / Lab Practice

- Create multiple VLANs on a managed switch  
- Assign access ports to specific VLANs  
- Configure trunk links between switches  
- Test connectivity within VLANs and across VLANs using a router (inter-VLAN routing)  
- Observe VLAN tagging on trunk ports  

---

### 🧠 6. Key Terms

- **Access Port:** Switch port assigned to a single VLAN  
- **Trunk Port:** Port carrying multiple VLANs  
- **VLAN Tagging:** Adding VLAN ID to frames for identification  
- **Native VLAN:** Default VLAN for untagged traffic  
- **Inter-VLAN Routing:** Communication between VLANs via a router or Layer 3 switch  

---

### 📘 Day 26 Summary

✅ Learned what VLANs are and why they are used  
✅ Explored VLAN types and purposes  
✅ Understood trunking and VLAN tagging  
✅ Practiced configuring VLANs and trunk ports  
