<div align="center">

# 👻 GHOST-TALK
### **Secure. Ephemeral. Encrypted.**
*A Billionaire-Tier LAN Messaging Terminal for the Modern Age.*

[![C++](https://img.shields.io/badge/Language-C++17-00599C?style=for-the-badge&logo=c%2B%2B)](https://en.cppreference.com/w/cpp/17)
[![Raylib](https://img.shields.io/badge/GUI-Raylib_5.0-white?style=for-the-badge)](https://www.raylib.com/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Windows_%7C_macOS-lightgrey?style=for-the-badge)](https://github.com/CodeHashiraX/Ghost-Talk)

</div>

---

## 📜 **Mission Brief**
**Ghost-Talk** is not just a chat app; it is a **cyber-security statement**. 

Built from the ground up in C++ without relying on heavy frameworks, it offers a raw, high-performance communication channel for local networks. It bypasses the internet entirely, ensuring your data never touches a cloud server. 

With its custom **"Neural Float"** physics engine and **Matrix-style decryption visuals**, Ghost-Talk turns simple text messaging into a cinematic experience.

---

## ✨ **Key Capabilities**

### 🛡️ **The Ghost Protocol (Core Engine)**
* **Zero-Trace Architecture:** Messages exist only in RAM. Closing the app triggers an immediate memory wipe.
* **XOR Encryption:** All packets are scrambled before leaving your machine, rendering them unreadable to packet sniffers.
* **LAN Auto-Discovery:** Instantly detects your local IP address for seamless Host/Join setups.

### ⚛️ **Physics-Enabled UI**
* **Neural Float:** Messages don't sit still. They bob gently in a zero-gravity simulation (`sin(time)`), connected by dynamic neural links.
* **Projectile Data Flow:** Visualize network traffic as glowing "Data Orbs" fly physically from sender to receiver.
* **Matrix Decrypt:** Incoming messages appear as raw binary garbage (`#@!%`) before mathematically resolving into readable text.

### 🧨 **Self-Destruct Mode (Red Alert)**
* **Ephemeral Nodes:** Activate the **[!]** toggle to send "Burn After Reading" messages.
* **Dynamic Memory Management:** Nodes physically delete themselves from the Linked List after 10 seconds, freeing memory in real-time.
* **Visual Warning:** Red-pulsing bubbles alert the recipient of the message's volatile nature.

---

## 🛠️ **Installation & Compilation**

### **Prerequisites**
* **C++ Compiler** (Clang, GCC, or MSVC)
* **Raylib 5.0** Library

### **⚡ Quick Start (macOS)**
1.  **Clone the Repo:**
    ```bash
    git clone [https://github.com/CodeHashiraX/Ghost-Talk.git](https://github.com/CodeHashiraX/Ghost-Talk.git)
    cd Ghost-Talk
    ```
2.  **Compile (M-Series Optimized):**
    ```bash
    clang++ src/main.cpp -o GhostTalk -std=c++17 -I/opt/homebrew/include -L/opt/homebrew/lib -lraylib -framework IOKit -framework Cocoa -framework OpenGL
    ```
3.  **Execute:**
    ```bash
    ./GhostTalk
    ```

### **⚡ Quick Start (Windows)**
1.  Open the project in **Visual Studio**.
2.  Link `raylib.lib` and `ws2_32.lib` in Project Properties.
3.  Build & Run `Release` mode.

---

## 🎮 **Operational Manual**

### **Phase 1: Initialization**
1.  **Identity:** Enter your Alias (e.g., `Master AK`).
2.  **Mode Selection:**
    * **HOST:** Creates a server on Port 9999.
    * **JOIN:** Connects to a Host IP.
    * **SANDBOX:** Offline testing mode.

### **Phase 2: Secure Communication**
* **Type & Send:** Messages flow instantly with projectile visuals.
* **Scroll:** Use `Mouse Wheel` or `Up/Down` keys to traverse history.
* **Self-Destruct:** Toggle the **[!]** button (Top Right). Messages sent now will vanish in 10s.

---

## 🧠 **Under The Hood (For Engineers)**

| Component | Implementation Detail |
| :--- | :--- |
| **Data Structure** | Custom Doubly Linked List (`struct MessageNode`) |
| **Networking** | Asynchronous Non-Blocking Sockets (`<sys/socket.h>` / `Winsock2`) |
| **Encryption** | Custom XOR Cipher per packet |
| **Rendering** | Immediate Mode GUI (Raylib) with Scissor Clipping |
| **Physics** | Sine-wave floating offsets + Lerp interpolation |

---

## 👥 **Credits**
* **Architect:** [Master AK](https://github.com/CodeHashiraX)
* **Engine:** Raylib 5.0

---
<div align="center">

*"Privacy is not an option. It is the default."*

</div>
