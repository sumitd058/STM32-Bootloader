Embedded Bootloader and Secure Firmware Update
This project implements a secure bootloader for embedded systems with functionalities for firmware updates, secure memory management, version control, and error handling. Designed to ensure secure and reliable firmware management, this bootloader runs on ARM Cortex-M (STM32F4) and RH850 microcontrollers.

Table of Contents
Overview
Features
Memory Layout
Update Mechanism
Memory Access
Version Control
Error Handling
Getting Started
Dependencies
Build and Deployment
License
Overview
This project is focused on developing a secure bootloader for embedded systems with specific emphasis on secure firmware updates, memory integrity, and system reliability. Key functions include setting memory regions for bootloader and application code, implementing a secure update protocol, memory access, and error handling.

Features
Memory Layout Configuration: Define specific memory regions for bootloader and application code.
Secure Update Mechanism: Robust protocol for secure firmware updates.
Secure Memory Access: Implements secure memory read/write functions.
Version Control: Structuring for version tracking of bootloader and application.
Comprehensive Error Handling: Detect and handle errors for memory and version mismatches.
Memory Layout
The project defines specific memory regions to separate bootloader and application code for enhanced security and modularity. This helps in:

Protecting bootloader code from unauthorized access or modification.
Enabling secure handoff to application code post-verification.
Update Mechanism
The bootloader implements a secure protocol for firmware updates:

Authentication: Uses cryptographic verification to ensure the integrity of firmware updates.
Rollback Protection: Prevents downgrades by verifying firmware versioning.
Secure Transfer: Encrypts firmware data during updates for confidentiality.
Memory Access
Provides secure read and write access to protected memory regions.
Protects sensitive data using cryptographic methods and permission-based access.
Version Control
Version information structures are defined for both bootloader and application code:

Ensures compatibility between bootloader and application versions.
Prevents execution of incompatible firmware versions.
Error Handling
Comprehensive error handling is implemented to:

Detect and respond to memory access errors.
Handle version mismatches or corrupt firmware files.
Log and report errors for troubleshooting and diagnostics.
Getting Started
Prerequisites
To build and deploy the bootloader, you will need:

ARM Toolchain for cross-compilation
STM32 Cube IDE or Renesas Flash Programmer for deployment
Debugger compatible with target microcontroller
