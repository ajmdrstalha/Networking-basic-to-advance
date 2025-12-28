## 📘 Day 8 – VLANs & Trunking

### 🧩 1. What is a VLAN?

A **VLAN (Virtual Local Area Network)** is a **logical segmentation of a network** within the same physical network.

- Groups devices based on function, department, or project  
- Reduces broadcast traffic  
- Improves network security and management  

Example:
- VLAN 10 → HR Department  
- VLAN 20 → IT Department  

---

### 🔢 2. VLAN Types

| Type | Description |
|------|-------------|
| Default VLAN | Default on all switches, usually VLAN 1 |
| Data VLAN | Carries user-generated data |
| Voice VLAN | Dedicated for VoIP traffic |
| Management VLAN | Used for managing network devices |

---

### 🔁 3. What is Trunking?

**Trunking** allows multiple VLANs to pass through a **single physical link** between switches.

- Uses **tagging** (802.1Q) to identify VLANs  
- Enables VLAN communication across switches  
- Reduces cabling complexity  

Example:
Switch1 (VLAN 10,20) → Trunk → Switch2 (VLAN 10,20)

yaml
Copy code

---

### ⚙️ 4. VLAN Tagging (802.1Q)

- Adds a **VLAN ID** to Ethernet frames  
- Ensures frames reach the correct VLAN on the receiving switch  
- Untagged frames are usually assigned to the **native VLAN**  

---

### 🗂️ 5. Practical / Lab Practice

- Create VLANs on a managed switch:  
vlan 10
name HR
vlan 20
name IT

yaml
Copy code
- Assign switch ports to VLANs  
- Configure a trunk port between two switches  
- Test connectivity within same VLAN and across VLANs  

---

### 🧠 6. Key Terms

- **VLAN:** Logical network segment  
- **Trunk:** Link carrying multiple VLANs  
- **Access Port:** Port assigned to a single VLAN  
- **Native VLAN:** Untagged VLAN on a trunk  

---

### 📘 Day 8 Summary

✅ Learned what VLANs are and their benefits  
✅ Explored VLAN types and configurations  
✅ Understood trunking and 802.1Q tagging  
✅ Practiced VLAN and trunk configurations  
