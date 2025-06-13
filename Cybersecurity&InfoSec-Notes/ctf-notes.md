# CTF Spotlight concepts

## About Reverse Engineering

**Reverse engineering (RE)**: involve taking a binary and reverse engineering it to determine its functionality (finding a flag)
> process of dissecting and comprehending the internal mechanisms, architecture, and operation of hardware, software, or systems to expose their design concepts, source code, or architecture. Also used for vulnerability research<br>
> Example: A reverse engineer will take the final product and pull it apart to figure out what parts were used to make the final product.
> This process is usually used in malware analysis, like an autopsy or **autopsia**, "To see for one's self"

**packing**: malware is compressed & disassembly won't work. Code must be decompressed b4 analysis, some **malware authors** may use multiple packing programs to hide their code/encrypt code itself.<br>
**code becomes a riddle wrapped in a mystery inside an enigma, and we might not have the key to solve it**
Reverse engineering something also doesn't mean we can reveal **what that malware does**.
<br>

### Reverse Engineering Tools and Techniques

IDA, Pro, Ghidra, OllyDbg, Radare2, Wireshark <br>

Here are ***five*** key tools and techniques used in reverse engineering:

**Disassemblers**: Software such as IDA Pro, ghdl, and radare2 disassembles a code into assembly language, which helps in the analysis of the higher workings of a program. Here, the role of software documentation is that it contains information about the construction and work of programs.

**Debuggers**: That is why there are OllyDbg and x64dbg, which work mainly for dynamic analysis, as they let you step through the code and setup how the execution is going to go, and they let you inspect and change certain elements located in the memory. This aids in describing the running behavior of a program at runtime.

**Hex Editors**: Both Hex Workshop and Hex Fiend resources enable the user to open and view raw binary data in a file. This is good for studying and/or altering the data at the most basic level.

**Decompilers**: Some of the most popular approaches include the Static Binary Analysis Tool, the use of JEB Decompiler for source code decompiling, and JADX. This enables one to know the outlines of the arrangement of the software without having to tackle assembly language.

**Network Analyzers**: Examples of the SNM tools include Wireshark, which captures and analyzes network traffic. They are used to capture protocols used by networks and the information passed in between applications, which proves useful in reverse engineering applications that are networked. <br>
More info @[What is Reverse Engineering Technique in Cybersecurity?](https://www.geeksforgeeks.org/computer-networks/what-is-reverse-engineering-technique-in-cybersecurity/)

Pwn: successfully compromise or gain control over a system, application, or network
Crypto
Web
Forensics/Stego
Other





#### References

[CTF Beginner's Guide](https://jaimelightfoot.com/blog/so-you-want-to-ctf-a-beginners-guide/) <br>
[Static vs Dynamic Analysis](https://rahulsinghinfosec.github.io/hackme/reverse-engineering/static-vs-dynamic-analysis.html)