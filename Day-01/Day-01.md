## 📘 **Day 1 – What is Networking? | LAN, WAN, Internet, Topologies & Devices**

### 🧩 **1. What is Networking?**

* **Definition:** Connecting two or more devices to share data and resources.
* **Purpose:** File sharing, communication (email, chat), internet access, centralized management.
* **Example:** Your phone connecting to Wi‑Fi to reach a web server.
* **Real‑life analogy:** Roads (network), vehicles (data), and destinations (devices).

---

### 🏠 **2. Types of Networks**

| Type                                | Description                      | Example                           |
| ----------------------------------- | -------------------------------- | --------------------------------- |
| **LAN** (Local Area Network)        | Connects devices in a small area | Office, school lab                |
| **MAN** (Metropolitan Area Network) | Covers a city or campus          | University network                |
| **WAN** (Wide Area Network)         | Connects multiple LANs           | Internet, corporate branch links  |
| **PAN** (Personal Area Network)     | Very small range                 | Bluetooth between phone & headset |

---

### 🌍 **3. The Internet**

* The world’s largest WAN interconnecting billions of devices.
* Uses public IPs and routing protocols (BGP).
* ISPs provide the link between your LAN and the global internet.
* Key components: DNS, IP addressing, routing, switching.

---

### 🔗 **4. Network Devices – Introduction**

| Device              | Function                                          | Example                      |
| ------------------- | ------------------------------------------------- | ---------------------------- |
| **Computer / Host** | Generates or receives data                        | PC, laptop, server           |
| **Switch**          | Connects devices within a LAN using MAC addresses | Cisco 2960, TP‑Link          |
| **Router**          | Connects different networks & directs data via IP | Home Wi‑Fi router            |
| **Hub**             | Broadcasts data to all ports (outdated)           | Old network hub              |
| **Access Point**    | Provides wireless connection to LAN               | Wi‑Fi AP                     |
| **Modem**           | Converts ISP signal (fiber/DSL) into digital data | ISP‑provided device          |
| **Firewall**        | Protects network by controlling traffic           | Hardware / software firewall |

> 💡 *

---

### 🗺️ **5. Network Topologies**

| Topology   | Description                             | Pros                  | Cons                 |
| ---------- | --------------------------------------- | --------------------- | -------------------- |
| **Bus**    | All devices share one backbone cable    | Simple, cheap         | Collision risk       |
| **Star**   | All devices connect to a central switch | Easy to manage        | Single point failure |
| **Ring**   | Devices form a circle                   | Predictable data path | Failure breaks loop  |
| **Mesh**   | Each device connects to many others     | High reliability      | Expensive            |
| **Hybrid** | Combination of topologies               | Flexible              | Complex setup        |

---

### ⚙️ **6. How Data Travels**

* Data is broken into **packets**.
* Packets contain source IP, destination IP, and payload.
* Switches forward data inside a LAN.
* Routers forward data between different networks.
* DNS converts domain names into IP addresses.

---

### 🧠 **7. Key Terms**

* **Node:** Any device connected to a network.
* **Bandwidth:** Maximum data transfer rate of a link.
* **Latency:** Time taken for data to travel from source to destination.
* **Protocol:** A set of rules for communication (e.g., TCP/IP).

---

### 🧪 **8. Practical / Lab Idea**

* Draw a simple **home network diagram**:

  `Modem → Router → Switch → PCs + Wi‑Fi Devices`

* Check IP configuration:

  * **Windows:** `ipconfig`
  * **Linux:** `ifconfig` or `ip addr`

---

### 📘 **Day 1 Summary**

✅ Defined what networking is
✅ Learned LAN, MAN, WAN, and the Internet
✅ Introduced core network devices
✅ Understood network topologies and packet flow

