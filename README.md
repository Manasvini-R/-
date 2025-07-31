
# 🛡️ Hands-on Deployment of Honeypots Using Pentbox

This project demonstrates the deployment and testing of a **honeypot** using **Pentbox on Kali Linux**, simulating real-world attack scenarios for cybersecurity awareness and defense practice.

## 📌 Project Objective

The aim of this project is to understand and implement basic deception technology using **Pentbox**, a security suite, and simulate attacks to observe how honeypots behave when targeted. This helps build foundational knowledge for intrusion detection and network defense.

---

## 🧰 Tools & Technologies

- **OS:** Kali Linux
- **Tool:** Pentbox v1.8
- **Environment:** Simulated network setup (localhost)
- **Protocol Simulated:** SSH (Port 22), HTTP Access via IP

---

## ⚙️ Setup & Configuration

### 1. Launch Pentbox
```bash
ruby pentbox.rb
````

If you face permission issues, try:

```bash
sudo ruby pentbox.rb
```

### 2. Select Honeypot Option

From the Pentbox menu:

```
1. Network Tools
   └── 3. Honeypot
```

### 3. Configuration Options

#### a. **Fast Auto Configuration**

* Pentbox selects a random open port and starts listening.
* Simulate a basic attack by copying the local IP and entering it in a web browser.
* Results in an *Access Denied* message, proving honeypot detection.

#### b. **Manual Configuration**

* Enter port manually (e.g., Port 22 for SSH).
* Pentbox monitors the specified port for connections.
* Simulate an SSH scan using tools like `nmap`:

  ```bash
  nmap -p 22 <your_local_ip>
  ```

---

## 🔬 Attack Simulation

### Fast Auto Config Mode:

* Accessed honeypot IP via browser.
* Received an **Access Denied** page, confirming the honeypot trapped the request.

### Manual Port Config (SSH Port 22):

* Performed port scan using `nmap`.
* Honeypot logged and flagged incoming connections.

---

## 📄 Report

A detailed report of this project including screenshots, analysis, and results is available here:
[📎 Download Report](https://drive.google.com/file/d/13RNYIBjq0bzUwtMBbdfODlpGipyOe63h/view?usp=sharing)

---

## 📈 Key Learnings

* How to set up and configure a honeypot using Pentbox
* How to simulate attacks using basic tools
* How honeypots can detect and log unauthorized access attempts
* Practical experience in proactive cyber defense mechanisms

---

## 🔐 Future Enhancements

* Deploy Pentbox on a live network (not just localhost)
* Integrate with logging and alerting systems
* Extend to other honeypot solutions like Cowrie or Honeyd
* Analyze logs and correlate with SIEM tools

---

## 🧠 Author

**Manasvini R**
Cybersecurity Engineering

---

## 🏷️ Tags

`#CyberSecurity` `#Honeypot` `#Pentbox` `#KaliLinux` `#ThreatDetection` `#NetworkSecurity` `#DeceptionTechnology` `#InfoSec`

```

---

Let me know if you want a shorter version or if you want it to include code blocks, commands, or GitHub badges.
```
