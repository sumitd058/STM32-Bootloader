# Embedded Bootloader and Secure Firmware Update
A secure bootloader for embedded systems (ARM Cortex-M STM32F4 and RH850) supporting secure firmware updates, memory management, version control, and error handling.

# Overview
This project focuses on secure firmware management for embedded systems. Key features include setting defined memory regions for bootloader and application, implementing a secure firmware update protocol, and error handling.

# Features
Memory Layout: Separates memory for bootloader and application code.
Update Mechanism: Uses cryptographic verification for secure updates.
Memory Access: Provides secure read/write access.
Version Control: Tracks bootloader and application versions.
Error Handling: Manages memory and version errors.
Getting Started

# Prerequisites
ARM Toolchain for cross-compilation
STM32 Cube IDE or Renesas Flash Programmer for flashing
