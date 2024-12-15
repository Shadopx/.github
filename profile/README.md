# **WIP: Shadopx**  
**Dynamic Proxy and VPN Management for Secure, Anonymous Connections.**

> **Note**: Shadopx is currently under **active development** and nearing its release. Testing and refining are our top priorities at this stage.  
>   
> **Please use Shadopx ethically** and responsibly to ensure it aligns with legal and ethical practices.

---

## **What is Shadopx?**  

Shadopx is an advanced, **TypeScript-based library** built for dynamic **proxy rotation** and **VPN management**. It is designed to protect applications running on servers, ensuring privacy, anonymity, and stability without requiring any changes to the application code.

Whether you're running a BitTorrent client like **Deluge** or another service, Shadopx seamlessly routes its traffic through **rotating proxies** or **VPN connections**, shielding your **real IP address** from being exposed.

Shadopx combines **stealth**, **precision**, and **control** to offer a robust solution for network anonymity and proxy management.

---

## **Features**

- **Dynamic Proxy Rotation**  
   Rotate proxies intelligently using:  
   - Round-robin  
   - Random selection  
   - Every-other-request strategies  

- **VPN Integration**  
   Seamlessly integrate **OpenVPN** or premium VPN providers for server-level anonymity.  

- **Kill Switch (Strict Mode)**  
   Prevent real IP leaks by blocking traffic when no proxies or VPNs are healthy.  

- **Health Checks**  
   Proxies and VPN servers are dynamically validated to ensure reliability.  

- **Extensible Configuration**  
   Easy-to-edit **JSON** or **YAML** configuration files for user-friendly setup.  

- **Application-Agnostic**  
   Works with any application, like **Deluge**, without modifying its source code.  

- **Concurrency Optimisation**  
   Efficient task queue ensures smooth proxy rotation for concurrent requests.  

---

## **Why Use Shadopx?**

Shadopx is designed to **"just work"** with minimal setup. By focusing on clean abstraction and robust performance, Shadopx:  
- Protects your applications from exposing their real IP addresses.  
- Dynamically switches proxies or VPN servers to maintain uptime and anonymity.  
- Scales seamlessly for both simple and advanced use cases.  

---

## **Supported VPN Providers**  

For a VPN provider to be compatible with Shadopx, it must meet the following requirements:

| **Requirement**              | **Description**                                                    |
|-------------------------------|--------------------------------------------------------------------|
| **Custom Config Support**     | Allows OpenVPN `.ovpn` files or API-based server switching.       |
| **CLI/Programmatic Access**   | Ability to start, stop, or rotate VPN connections programmatically.|
| **Server List Access**        | Provides server lists (static or API-driven) for rotation.         |
| **Username/Password Auth**    | Supports authentication via credentials.                          |
| **Interval Rotation Support** | Ability to switch servers at specified intervals.                 |

---

### **VPN Compatibility Table**  

| **VPN Provider**         | Custom Config | CLI Access | Server List | Auth Support | Interval Rotation | Custom DNS |
|---------------------------|---------------|------------|-------------|--------------|-------------------|------------|
| **NordVPN**              | ✅ Yes        | ✅ Yes     | ✅ Yes      | ✅ Yes       | ✅ Yes            | ✅ Yes     |
| **Surfshark**            | ✅ Yes        | ✅ Yes     | ✅ Yes      | ✅ Yes       | ✅ Yes            | ✅ Yes     |
| **Private Internet Access (PIA)** | ✅ Yes | ✅ Yes     | ✅ Yes      | ✅ Yes       | ✅ Yes            | ✅ Yes     |
| **ProtonVPN**            | ✅ Yes        | ✅ Yes     | ✅ Yes      | ✅ Yes       | ✅ Yes            | ✅ Yes     |
| **CyberGhost**           | ✅ Yes        | ✅ Limited | ✅ Yes      | ✅ Yes       | ✅ Yes            | ✅ Yes     |
| **ExpressVPN**           | ❌ No         | ❌ Limited | ❌ No       | ✅ Yes       | ❌ No             | ❌ No      |
| **Hotspot Shield**       | ❌ No         | ❌ No      | ❌ No       | ❌ No        | ❌ No             | ❌ No      |

---

## **How Does It Work?**

Shadopx operates as an intermediary proxy or VPN layer:  
1. **Proxy Rotation**: Proxies are dynamically fetched, validated, and rotated based on user-defined strategies.  
2. **VPN Integration**: Connects to OpenVPN servers or premium VPN providers for interval-based server switching.  
3. **Kill Switch**: When strict mode is enabled, Shadopx blocks traffic if proxies or VPN servers fail, preventing real IP exposure.  

You can easily point any application (e.g., Deluge, web scrapers, or APIs) to Shadopx as a proxy server, and it will automatically protect and anonymise all traffic.

---

## **Getting Started**

To see Shadopx in action, check out our main repository:  
🔗 **[Shadopx Repository](https://github.com/shadopx/shadopx)**  

The repository README provides:  
- Step-by-step installation instructions  
- Configuration examples (JSON/YAML)  
- Use case guides (e.g., protecting Deluge BitTorrent client)  

---

## **Ethical Use**

We ask all users to use Shadopx responsibly and **ethically**. This tool is designed to protect privacy, improve uptime, and ensure secure connections for legitimate use cases. Misusing Shadopx for unlawful activities may result in serious consequences.  

---

## **Contributing**

Shadopx is an evolving project, and contributions are welcome! Feel free to fork, submit PRs, or discuss new ideas.  

---

Thank you for checking out **Shadopx**! We’re excited to bring you a powerful and reliable solution for proxy rotation and VPN integration.  

🚀 **Stealth. Precision. Protection.** 🚀  

---
