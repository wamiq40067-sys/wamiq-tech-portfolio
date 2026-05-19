# Key Notes: All About Linux

## Introduction to Linux
- :contentReference[oaicite:0]{index=0} is an open-source operating system widely used in cybersecurity, cloud computing, servers, and software development.
- Linux is known for its:
  - Stability
  - Security
  - Flexibility
  - Multi-user support
- Being open-source means its source code is publicly available and can be modified by anyone.

## Components of Linux
### User
- The user interacts with the computer system and performs tasks.

### Applications
- Applications are programs designed to complete specific tasks.
- Linux applications are commonly installed using package managers.

### Shell
- The shell acts as the command-line interpreter between the user and the operating system.
- It converts user commands into instructions for the system.

### Kernel
- The kernel is the core component of Linux.
- It manages:
  - Processes
  - Memory
  - Hardware communication
  - Resource allocation

### Filesystem Hierarchy Standard (FHS)
- FHS defines how files and directories are organized in Linux.
- Directories help store and organize files systematically.

## Hardware in Linux Systems
### Internal Hardware
- Essential components required for system operation:
  - CPU
  - RAM
  - Hard Drive
  - Motherboard

### Peripheral Devices
- External devices connected to the computer:
  - Keyboard
  - Mouse
  - Monitor
  - Printer

## Important Hardware Components
### CPU
- Executes program instructions and handles processing tasks.

### RAM
- Temporary memory used while programs are running.
- Data is lost when the system powers off.

### Hard Drive
- Long-term storage device for files, applications, and operating system data.

---

# Key Notes: Linux Distributions

## What are Linux Distributions?
- Linux distributions (distros) are different versions of Linux built for specific purposes.
- Distributions combine:
  - Linux kernel
  - Applications
  - Package managers
  - User interfaces

## Common Linux Distributions

### Kali Linux
- :contentReference[oaicite:1]{index=1} is widely used in cybersecurity.
- Includes pre-installed tools for:
  - Penetration testing
  - Ethical hacking
  - Digital forensics

### Ubuntu
- :contentReference[oaicite:2]{index=2} is beginner-friendly and widely used.
- Supports both GUI and CLI environments.
- Popular in:
  - Cloud computing
  - Servers
  - Cybersecurity

### Parrot OS
- :contentReference[oaicite:3]{index=3} is designed for privacy and security tasks.
- Includes built-in security and forensic tools.

### Red Hat Enterprise Linux (RHEL)
- :contentReference[oaicite:4]{index=4} is a commercial Linux distribution for enterprise use.
- Known for:
  - Stability
  - Security
  - Professional support

### AlmaLinux
- :contentReference[oaicite:5]{index=5} is a community-supported replacement for CentOS.
- Maintains compatibility with Red Hat-based systems.

## Package Managers
- Package managers help install, update, and remove software packages.
- Debian-based systems commonly use:
  - `dpkg`
  - `APT`
- Red Hat-based systems commonly use:
  - `RPM`
  - `YUM`

---

# Key Notes: The Shell

## What is a Shell?
- The shell is a command-line interface used to interact with the operating system.
- It acts as a bridge between the user and the kernel.

## Functions of the Shell
- Accepts user commands
- Interprets instructions
- Sends commands to the kernel
- Displays results and error messages

## Common Linux Shells
### Bash
- :contentReference[oaicite:6]{index=6} is the default shell in most Linux systems.
- Popular because it is:
  - User-friendly
  - Powerful
  - Scriptable

### Other Linux Shells
- C Shell (`csh`)
- Korn Shell (`ksh`)
- Enhanced C Shell (`tcsh`)
- Z Shell (`zsh`)

## Shell Prompts
- Different shells use different prompt symbols:
  - `bash` and `ksh` commonly use `$`
  - `zsh` often uses `%`

## Standard Streams
### Standard Input (stdin)
- Data entered into the system through the command line.

### Standard Output (stdout)
- Normal output returned by the operating system.

### Standard Error (stderr)
- Error messages returned by the system.

## Importance of Bash in Cybersecurity
- Bash is widely used in:
  - System administration
  - Security operations
  - Automation
  - Scripting
- Cybersecurity professionals frequently use bash for managing Linux systems and running security tools.