# 🔍 CTF Notes: Reverse Engineering & InfoSec Concepts

## 🧠 CTF Spotlight Concepts

### 🔄 About Reverse Engineering

**Reverse engineering (RE)** involves analyzing a binary to determine its functionality (e.g., to find a flag).

- It is the process of dissecting and understanding the internal mechanisms, architecture, and behavior of hardware, software, or systems.
- RE can expose design concepts, source code, or vulnerabilities.  
- Common use case: **vulnerability research**.

> 💡 **Example:** A reverse engineer will take the final product and pull it apart to figure out what parts were used to make the final product.

This process is usually involved in malware analysis — like a digital autopsy:  
**"To see for one's self."**

---

### ⚠️ Obstacles in RE

- **Packing:** Malware may be compressed or packed so disassemblers won't work. Code must often be decompressed first.  
  Malware authors often use multiple packers to hide/encrypt code.
  
- **Obfuscation:** Code might be encrypted, layered, or encoded in a way that makes reverse engineering difficult.  

> 🧩 *Reverse engineering doesn't always reveal what the malware does. It's like solving an enigma with a missing key.*

---

## 🧰 Reverse Engineering Tools and Techniques

### 🛠 Common Tools

- IDA Pro
- Ghidra
- OllyDbg
- Radare2
- Wireshark

These are **five** key tool categories used in RE:

---

### 🔧 Disassemblers

Software like **IDA Pro**, **Ghidra**, and **Radare2** disassemble code into assembly language.  
This helps analyze the low-level workings of a program.  
Disassemblers help expose logic and control flow.

---

### 🐞 Debuggers

**OllyDbg** and **x64dbg** are examples of dynamic analysis tools.  
They let you step through code, inspect memory, and modify runtime behavior.

---

### 🧬 Hex Editors

Tools like **Hex Workshop** and **Hex Fiend** enable you to open and analyze raw binary data.  
Useful for binary-level data inspection and modification.

---

### 📦 Decompilers

Examples include:

- **JEB Decompiler**
- **JADX** (for Android)
- **Static Binary Analysis Tool**

These allow you to recover high-level source code (to a degree) and understand structure without needing to fully reverse binary logic.

---

### 🌐 Network Analyzers

Tools like **Wireshark** capture and inspect network packets.  
Essential for dynamic analysis of networked applications or malware with command & control (C2) behavior.

🔗 More info: [What is Reverse Engineering in Cybersecurity? – GeeksforGeeks](https://www.geeksforgeeks.org/computer-networks/what-is-reverse-engineering-technique-in-cybersecurity/)

---

## 📁 CTF Category Index

| Category       | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| **Pwn**        | Exploiting binaries to gain shell or escalate privileges                    |
| **Crypto**     | Challenges involving cryptographic algorithms (e.g., RSA, AES, XOR)         |
| **Web**        | Attacks against web apps (XSS, SQLi, SSRF, etc.)                            |
| **Forensics**  | File analysis, memory dumps, and steganography                              |
| **Other**      | Miscellaneous challenges (OSINT, Trivia, Blockchain, etc.)                  |

---

## ✅ Tips from Cyber Camp

- Analyze packed binaries using a debugger + hex editor combo.
- Always test suspicious binaries in isolated VMs.
- Don't trust strings output alone—use `ltrace`, `strace`, or dynamic debugging.
- Use `tcpdump` or Wireshark to monitor malware network activity.


### 📚 References

[CTF Beginner's Guide](https://jaimelightfoot.com/blog/so-you-want-to-ctf-a-beginners-guide/) <br>
[Static vs Dynamic Analysis](https://rahulsinghinfosec.github.io/hackme/reverse-engineering/static-vs-dynamic-analysis.html) <br>
[What is Reverse Engineering in Cybersecurity? – GeeksforGeeks](https://www.geeksforgeeks.org/computer-networks/what-is-reverse-engineering-technique-in-cybersecurity/)