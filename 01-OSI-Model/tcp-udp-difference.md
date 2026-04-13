# 🌐 TCP vs UDP (Complete Guide)

---

## 🎯 Overview

TCP (Transmission Control Protocol) and UDP (User Datagram Protocol) are transport layer protocols used for communication between systems.

They define **how data is sent over the network**.

---

## 🧠 Key Difference

- **TCP** → Reliable, connection-oriented  
- **UDP** → Fast, connectionless  

---

## 📚 Comparison Table

| Feature | TCP | UDP |
|--------|-----|-----|
| Type | Connection-oriented | Connectionless |
| Reliability | High | Low |
| Speed | Slower | Faster |
| Error Checking | Yes | Minimal |
| Retransmission | Yes | No |
| Order Guarantee | Yes | No |
| Overhead | High | Low |
| Use Case | Critical data | Real-time data |

---

## 🔗 TCP (Transmission Control Protocol)

### 📌 What is TCP?

TCP ensures **reliable and ordered delivery of data**.

---

### 📌 Key Features

- Connection-oriented (3-way handshake)  
- Reliable delivery  
- Error detection and correction  
- Flow control  
- Congestion control  
- Data arrives in order  

---

### 📌 TCP Workflow

1. Connection established  
2. Data sent in segments  
3. Receiver sends acknowledgment (ACK)  
4. Lost data is retransmitted  

---

### 📌 TCP 3-Way Handshake

```text
Client → SYN → Server
Client ← SYN-ACK ← Server
Client → ACK → Server
```

Connection established ✅

---

### 📌 TCP Header Fields

- Source Port  
- Destination Port  
- Sequence Number  
- Acknowledgment Number  
- Flags (SYN, ACK, FIN)  

---

### 📌 TCP Use Cases

- Web browsing (HTTP/HTTPS)  
- File transfer (FTP)  
- Email (SMTP)  
- Banking applications  

---

## ⚡ UDP (User Datagram Protocol)

### 📌 What is UDP?

UDP sends data **without establishing a connection**.

---

### 📌 Key Features

- Connectionless  
- No acknowledgment  
- No retransmission  
- Faster transmission  
- Low overhead  

---

### 📌 UDP Workflow

1. Data is sent directly  
2. No confirmation  
3. No guarantee of delivery  

---

### 📌 UDP Header Fields

- Source Port  
- Destination Port  
- Length  
- Checksum  

---

### 📌 UDP Use Cases

- Video streaming  
- Online gaming  
- VoIP (voice calls)  
- DNS queries  

---

## ⚖️ TCP vs UDP (Deep Comparison)

### 🔹 Reliability

- TCP → Guaranteed delivery  
- UDP → No guarantee  

---

### 🔹 Speed

- TCP → Slower (checks, retries)  
- UDP → Faster (no checks)  

---

### 🔹 Ordering

- TCP → Maintains order  
- UDP → No ordering  

---

### 🔹 Overhead

- TCP → High overhead  
- UDP → Low overhead  

---

## 📦 Data Transmission Example

### TCP

```text
Send → ACK → Send → ACK → Resend if lost
```

---

### UDP

```text
Send → Send → Send (No confirmation)
```

---

## 🧠 When to Use What?

### ✅ Use TCP When:

- Data must be accurate  
- No data loss allowed  
- Order matters  

Examples:
- Banking  
- File downloads  
- APIs  

---

### ⚡ Use UDP When:

- Speed is critical  
- Some data loss is acceptable  

Examples:
- Live streaming  
- Gaming  
- Voice calls  

---

## 🔑 Key Concepts

### 🔹 Reliability vs Speed Tradeoff

- TCP → Reliability > Speed  
- UDP → Speed > Reliability  

---

### 🔹 Ports

Both TCP and UDP use **port numbers** to identify applications.

Example:
- HTTP → Port 80 (TCP)  
- DNS → Port 53 (UDP)  

---

## 🔍 Troubleshooting

| Issue | Protocol |
|------|---------|
| Packet loss | UDP |
| Slow connection | TCP |
| Out-of-order data | UDP |
| Connection failure | TCP |

---

## 🧠 Memory Trick

- TCP → **Safe & Reliable**  
- UDP → **Fast & Lightweight**  

---

## 🎯 One-Line Summary

👉 TCP ensures reliable communication  
👉 UDP provides fast communication  

---