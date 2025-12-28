## 📘 Day 3 – Subnetting | Subnet Mask, CIDR, and Calculations

---

### 🧩 1. What is Subnetting?

Subnetting is the process of dividing a large network into smaller logical networks called **subnets**.

- Reduces network congestion  
- Improves security  
- Efficient use of IP addresses  
- Easier network management  

Example:
```

192.168.1.0/24
↓
192.168.1.0/26

```

---

### 🧮 2. Subnet Mask Explained

A subnet mask separates the **network portion** and **host portion** of an IP address.

Example:
```

IP Address : 192.168.1.10
Subnet Mask: 255.255.255.0

```

Binary format:
```

11111111.11111111.11111111.00000000

```

- `1` → Network bits  
- `0` → Host bits  

---

### 📐 3. CIDR Notation

CIDR stands for **Classless Inter-Domain Routing**.

Format:
```

IP / Number_of_Network_Bits

```

Examples:

| CIDR | Subnet Mask |
|-----|-------------|
| /8  | 255.0.0.0 |
| /16 | 255.255.0.0 |
| /24 | 255.255.255.0 |
| /26 | 255.255.255.192 |

---

### 🧱 4. Network, Host, and Broadcast Address

Example:
```

192.168.1.0/24

```

| Type | Address |
|------|---------|
| Network Address | 192.168.1.0 |
| First Host | 192.168.1.1 |
| Last Host | 192.168.1.254 |
| Broadcast Address | 192.168.1.255 |

---

### 🔢 5. Subnet and Host Calculation

Formulas:
```

Number of Subnets = 2^n
Number of Hosts   = 2^h − 2

```

Where:
- `n` = borrowed bits  
- `h` = host bits  

Example:
```

/26 → Host bits = 6
Hosts = 2⁶ − 2 = 62

```

---

### 🧠 6. Subnetting Example

Given:
```

192.168.10.0/26

```

Subnet size:
```

256 − 192 = 64

```

| Subnet | Network | Host Range | Broadcast |
|--------|---------|------------|-----------|
| 1 | 192.168.10.0 | .1 – .62 | .63 |
| 2 | 192.168.10.64 | .65 – .126 | .127 |
| 3 | 192.168.10.128 | .129 – .190 | .191 |
| 4 | 192.168.10.192 | .193 – .254 | .255 |

---

### ⚠️ 7. Common Subnetting Mistakes

- Using network address as host IP  
- Using broadcast address as host IP  
- Wrong subnet mask selection  
- Forgetting to subtract 2 hosts  

---

### 🧪 8. Practical / Lab Practice

Calculate subnet details for:
```

10.0.0.0/24
172.16.5.0/27
192.168.100.0/26

```

Verify using:
- Online subnet calculator  
- `ipconfig` (Windows)  
- `ip addr` (Linux)  

---

### 🧠 9. Key Terms

- **Subnet:** Smaller logical network  
- **CIDR:** Flexible IP addressing  
- **Broadcast:** Message sent to all devices  
- **Host Range:** Valid usable IP addresses  

---

### 📘 Day 3 Summary

✅ Learned subnetting basics  
✅ Understood subnet masks and CIDR  
✅ Calculated hosts and subnets  
✅ Practiced real subnetting examples  
```

