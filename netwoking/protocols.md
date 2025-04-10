# 📖 DevOps Protocols & Ports Cheat Sheet

As I’ve been growing in my DevOps journey, understanding **network protocols** and their port numbers has helped me troubleshoot smarter and build more reliable systems.

Here’s a quick reference I put together based on real-world use cases 👇

---

## 🔐 Common Protocols & Ports

| Protocol | Port | Use Case in DevOps |
|---------|------|---------------------|
| **SSH** | 22   | secure shell access to remote servers and vms |
| **HTTP** | 80   | serving apps, webhooks, monitoring, api testing |
| **HTTPS** | 443 | secure version of http, used in production environments |
| **FTP** | 21   | file transfers, sometimes seen in legacy systems |
| **SMTP** | 25   | sending emails – used for alerts, logs, monitoring notifications |
| **DNS** | 53   | resolving domain names – crucial in cloud and kubernetes networking |
| **TCP** | varies | reliable transport, used by ssh, http, https |
| **UDP** | varies | faster transport, used in dns, streaming, some logs |
| **IP** | - | foundation of all network traffic, vital for routing and vpc configuration |

---

## 🧠 Why This Matters

- 📡 helps debug connectivity issues quickly  
- 🔄 improves understanding of infrastructure components  
- 🛠️ essential when working with cloud, ci/cd, container orchestration  
- 📈 boosts overall system design and reliability  

---

## 📎 Quick Tips

- always check firewall rules and security groups – most issues come from blocked ports  
- tools like `telnet`, `netcat (nc)`, or `curl` can help test port connectivity  
- document as you go — having a personal reference saves time later  

---

## 🔗 Useful Commands

```bash
# check if a port is open
nc -zv your-server-ip 22

# test http/https
curl -I http://your-app-url.com
