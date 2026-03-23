# 🗂️ Customised Virtual File System (CVFS)

<div align="center">

### A Linux-like Virtual File System implemented in C

[![Language](https://img.shields.io/badge/Language-C-00599C?style=for-the-badge&logo=c&logoColor=white)](https://github.com/ketkipakhale)
[![OS](https://img.shields.io/badge/Concepts-Operating_Systems-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/ketkipakhale)
[![GitHub](https://img.shields.io/badge/GitHub-ketkipakhale-181717?style=for-the-badge&logo=github)](https://github.com/ketkipakhale)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-38bdf8?style=for-the-badge)](https://portfolio-phi-rosy-56.vercel.app)

</div>

---

## 📌 About The Project

**Customised Virtual File System (CVFS)** is a system-level project that simulates a **Linux-like file system** entirely in C. It replicates the core internal data structures of a real operating system's file management — allowing users to perform all standard Linux file operations on **any operating system platform**.

> 🎯 This project demonstrates deep understanding of **Operating System internals**, **system programming**, and **low-level data structure design**.

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 🗄️ **Inode Table** | Simulated Incore Inode Table for file metadata management |
| 📋 **File Table** | Global File Table tracking all open file instances |
| 👤 **UAREA** | User Area structure for per-process file management |
| 📁 **UFDT** | User File Descriptor Table for file descriptor mapping |
| 💻 **Custom Shell** | Interactive shell supporting all file operation commands |
| 🔄 **Cross-Platform** | Run Linux file system operations on any OS |

---

## 🛠️ Data Structures Implemented
```
📦 Virtual File System
│
├── 🔷 Incore Inode Table
│     ├── File name
│     ├── File size
│     ├── File type (Regular / Directory)
│     ├── Permission (Read / Write / Execute)
│     └── Reference count
│
├── 🔷 File Table
│     ├── Read/Write offset
│     ├── Count of file descriptors
│     └── Pointer to Inode
│
├── 🔷 UAREA (User Area)
│     └── Per-process information
│
└── 🔷 User File Descriptor Table (UFDT)
      └── Array of pointers to File Table entries
```

---

## 💻 Supported Commands
```bash
# File Operations
create  <filename> <permission>   # Create a new file
open    <filename> <mode>         # Open existing file
close   <filename>                # Close an opened file
read    <filename>                # Read data from file
write   <filename>                # Write data to file
delete  <filename>                # Delete a file

# File Information
ls                                # List all files
stat    <filename>                # Display file statistics
fstat   <filedescriptor>          # Display file info by FD
lseek   <filename> <offset>       # Move file pointer offset

# System
closeall                          # Close all open files
help                              # Display all commands
exit                              # Exit the file system
```

---

## 🚀 How To Run

### Prerequisites
```
✅ GCC Compiler installed
✅ Any OS (Windows / Linux / Mac)
```

### Steps
```bash
# 1. Clone the repository
git clone https://github.com/ketkipakhale/cvfs.git

# 2. Navigate to the folder
cd cvfs

# 3. Compile the program
gcc cvfs.cpp.cpp -o cvfs

# 4. Run the Virtual File System
./cvfs
```

---

## 📚 Concepts Covered
```
✅ Operating System File System Architecture
✅ Inode-based File Management
✅ File Descriptors & File Tables
✅ System Calls Simulation
✅ Memory Management in C
✅ Pointer & Structure manipulation
✅ Process-level File Management (UAREA)
✅ Custom Shell / CLI Development
✅ Cross-platform System Programming
```

---

## 🧰 Tech Stack

![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![OS Concepts](https://img.shields.io/badge/OS_Concepts-FCC624?style=flat-square&logo=linux&logoColor=black)
![Data Structures](https://img.shields.io/badge/Data_Structures-FF6B6B?style=flat-square)
![System Programming](https://img.shields.io/badge/System_Programming-4CAF50?style=flat-square)
![Memory Management](https://img.shields.io/badge/Memory_Management-9C27B0?style=flat-square)

---

## 🔗 Other Projects

| Project | Description | Link |
|---|---|---|
| 🧠 NeuroBridge | Full-Stack Adaptive Learning Platform | [View](https://github.com/ketkipakhale/Neurobridge) |
| 🔐 File Packer | File Archiving with Encryption | [View](https://github.com/ketkipakhale) |
| 💬 Chat Messenger | P2P Real-time Chat App | [View](https://github.com/ketkipakhale) |
| 🌐 Portfolio | Personal Portfolio Website | [Visit](https://portfolio-phi-rosy-56.vercel.app) |

---

## 👩‍💻 Author

**Ketaki Pakhale**
- 🌐 Portfolio: [portfolio-phi-rosy-56.vercel.app](https://portfolio-phi-rosy-56.vercel.app)
- 💼 LinkedIn: [linkedin.com/in/ketakipakhale](https://www.linkedin.com/in/ketakipakhale/)
- 🐙 GitHub: [github.com/ketkipakhale](https://github.com/ketkipakhale)
- 📧 Email: pakhaleketaki@gmail.com

---

<div align="center">

⭐ **Star this repo if you found it useful!**

**Built with ❤️ by Ketaki Pakhale © 2026**

</div>
```

---

```
docs: add README for Customised Virtual File System
