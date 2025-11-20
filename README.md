#  Task 5 **Capture and Analyze Network Traffic Using Wireshark**

This repository contains the deliverables for **Task 5** of the Elevate Labs Cyber Security Internship.  
The objective of this task is to capture network packets using Wireshark, analyze common protocols,  
and export the capture as a `.pcap` file.

---

## 🛠 **Tools Used**
- **Wireshark** (Windows)
- Browser (Chrome/Edge)
- Windows Command Prompt (for ping tests)

---

## 📡 **Steps Performed**

### **1️⃣ Installed & Opened Wireshark**
Downloaded Wireshark and selected my active **Wi-Fi interface** for live capture.

### **2️⃣ Started Live Packet Capture**
Clicked the Wi-Fi interface → began capturing incoming and outgoing packets.

### **3️⃣ Generated Network Traffic**
To produce analyzable packets, I performed:
- Browsing websites (Google, YouTube, etc.)
- Running ping commands:
  ```
  ping google.com
  ```

### **4️⃣ Stopped Capture After ~1 Minute**
Used the **red stop button** to freeze the capture.

### **5️⃣ Analyzed Packets By Applying Filters**
I applied the following Wireshark filters to inspect different protocols:

| Protocol | Filter Used |
|---------|-------------|
| DNS | `dns` |
| TCP | `tcp` |
| UDP | `udp` |
| TLS/HTTPS | `tls` |
| HTTP (if any) | `http` |

Screenshots for each filter are added inside the `/screenshots` folder.

### **6️⃣ Exported Packet Capture**
Saved the capture file as:
```
capture.pcapng
```
This file is included in this repository.

---

## 🌐 **Protocols Identified & Explanation**

### **🟦 1. DNS (Domain Name System)**
Used for converting domain names (google.com) into IP addresses.  
Common packet types:
- Standard query
- Standard query response

### **🟥 2. TCP (Transmission Control Protocol)**
A connection-oriented and reliable protocol — ensures data packets arrive in order.

### **🟨 3. UDP (User Datagram Protocol)**
A fast, connectionless protocol used in streaming, gaming, and VoIP.

### **🟩 4. TLS/HTTPS (Encrypted Web Traffic)**
TLS encrypts HTTP traffic.  
Since most websites use HTTPS, the majority of captured traffic shows up as TLS.

---

## 📁 **Repository Structure**
```
task-5-wireshark/
│── README.md
│── capture.pcapng
├── dns_filter.png
├── tcp_filter.png
├── tls_filter.png
```

---


