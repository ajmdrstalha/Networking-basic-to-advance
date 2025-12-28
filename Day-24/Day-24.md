## 📘 Day 24 – Introduction to IPv6

### 🧩 1. What is IPv6?

**IPv6 (Internet Protocol version 6)** is the **next-generation IP protocol** designed to replace IPv4.

- Uses **128-bit addresses** (compared to IPv4’s 32-bit)  
- Provides a vastly larger address space  
- Simplifies routing and improves security  

Example:
2001:0db8:85a3:0000:0000:8a2e:0370:7334

yaml
Copy code

---

### 🔢 2. IPv6 Address Types

| Type | Description |
|------|-------------|
| Unicast | Single interface on a host; one-to-one communication |
| Multicast | One-to-many communication within a group |
| Anycast | One-to-nearest communication; one-to-one-of-many |
| Link-local | Used for communication within a single network segment |

---

### 🔁 3. IPv6 Address Structure

- 128 bits divided into **8 groups of 16 bits**  
- Hexadecimal format separated by colons  
- Leading zeros can be omitted  
- Consecutive zero groups can be shortened using `::`  

Example:
Full: 2001:0db8:0000:0000:0000:ff00:0042:8329
Short: 2001:db8::ff00:42:8329

yaml
Copy code

---

### ⚙️ 4. Benefits of IPv6

- Vast address space  
- Simplified header for faster processing  
- Built-in IPSec support  
- No need for NAT in most cases  
- Auto-configuration (stateless or DHCPv6)  

---

### 🗂️ 5. Practical / Lab Practice

- Assign IPv6 addresses to devices on a test network  
- Test connectivity using `ping6` or `ping -6`  
- Configure a static IPv6 route on a router  
- Explore IPv6 autoconfiguration on Linux and Windows  
- Compare IPv4 vs IPv6 connectivity and addressing  

---

### 🧠 6. Key Terms

- **Unicast:** One-to-one communication  
- **Multicast:** One-to-many communication  
- **Anycast:** One-to-nearest-of-many communication  
- **Link-local:** Address valid only on the local segment  
- **Autoconfiguration:** Automatic IPv6 assignment without DHCP  

---

### 📘 Day 24 Summary

✅ Learned what IPv6 is and why it’s needed  
✅ Explored IPv6 address types and structure  
✅ Understood benefits of IPv6  
✅ Practiced configuring and testing IPv6 addresses  
