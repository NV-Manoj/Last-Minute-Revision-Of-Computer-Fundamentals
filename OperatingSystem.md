**Operating Systems (OS)**
# Last-Minute Revision Notes for Operating Systems

## Table of Contents
1. [Basic Concepts](#basic-concepts)
2. [Process Management](#process-management)
3. [Threads](#threads)
4. [Memory Management](#memory-management)
5. [File Systems](#file-systems)
6. [Deadlocks](#deadlocks)
7. [Scheduling Algorithms](#scheduling-algorithms)
8. [Concurrency](#concurrency)
9. [Inter-Process Communication (IPC)](#inter-process-communication-ipc)
10. [Virtual Memory](#virtual-memory)
11. [Device Management](#device-management)
12. [Security and Protection](#security-and-protection)
13. [Important Commands (Linux)](#important-commands-linux)
14. [Common OS Concepts](#common-os-concepts)

---

## 1. Basic Concepts

- **Operating System (OS)**: Software that manages hardware and software resources and provides services for computer programs.
- **Kernel**: Core component of the OS that manages system resources and facilitates communication between hardware and software.
- **Shell**: Interface that allows users to interact with the OS, either through command-line (CLI) or graphical (GUI).

## 2. Process Management

- **Process**: A program in execution, containing the program code and its current activity.
- **State of a Process**:
  - **New**: Process is being created.
  - **Ready**: Process is waiting to be assigned to a processor.
  - **Running**: Instructions are being executed.
  - **Waiting**: Process is waiting for an event to occur.
  - **Terminated**: Process has finished execution.

## 3. Threads

- **Thread**: The smallest unit of processing that can be scheduled by the OS.
- **Advantages of Threads**:
  - Less resource-intensive than processes.
  - Easier to share data between threads.
  - More responsive to user interactions.

## 4. Memory Management

- **Memory Management**: Process of coordinating computer memory, allocating space to processes and ensuring efficient memory usage.
- **Paging**: Memory management scheme that eliminates the need for contiguous allocation of physical memory, dividing memory into fixed-size pages.
- **Segmentation**: Divides memory into segments based on logical divisions.

## 5. File Systems

- **File System**: Manages how data is stored and retrieved on disk drives.
- **Types of File Systems**:
  - **FAT (File Allocation Table)**: Simple file system, widely used.
  - **NTFS (New Technology File System)**: Advanced file system for Windows with security features.
  - **ext4 (Fourth Extended Filesystem)**: Common file system for Linux.

## 6. Deadlocks

- **Deadlock**: A situation where two or more processes are unable to proceed because each is waiting for the other to release resources.
- **Conditions for Deadlock**:
  - Mutual Exclusion
  - Hold and Wait
  - No Preemption
  - Circular Wait
- **Strategies to Handle Deadlocks**:
  - Prevention
  - Avoidance (e.g., Banker's Algorithm)
  - Detection and Recovery

## 7. Scheduling Algorithms

- **Scheduling**: Method for determining which process runs at a given time.
- **Types of Scheduling Algorithms**:
  - **FCFS (First-Come, First-Served)**: Processes are executed in the order they arrive.
  - **SJF (Shortest Job First)**: Executes the process with the shortest execution time.
  - **Round Robin**: Each process gets a small time slice in a cyclic order.
  - **Priority Scheduling**: Processes are scheduled based on priority.

## 8. Concurrency

- **Concurrency**: Ability of the OS to handle multiple tasks at the same time.
- **Race Condition**: A situation where two or more processes access shared data and try to change it simultaneously, leading to inconsistent results.

## 9. Inter-Process Communication (IPC)

- **IPC**: Mechanisms that allow processes to communicate and synchronize their actions.
- **Methods of IPC**:
  - **Pipes**: Unidirectional communication channel.
  - **Message Queues**: Messages are stored in a queue until they are read.
  - **Shared Memory**: Processes can access a common memory space.
  - **Semaphores**: Used for signaling between processes.

## 10. Virtual Memory

- **Virtual Memory**: Allows the execution of processes that may not be completely in memory by using disk space as an extension of RAM.
- **Benefits**:
  - Increases the apparent amount of memory.
  - Provides process isolation.
  - Simplifies memory management.

## 11. Device Management

- **Device Management**: Controls hardware devices through drivers and ensures communication between the OS and peripherals.
- **Types of I/O Devices**:
  - **Block Devices**: Access data in blocks (e.g., hard drives).
  - **Character Devices**: Access data as a stream (e.g., keyboard).

## 12. Security and Protection

- **Security**: Measures taken to protect data from unauthorized access.
- **Protection**: Mechanisms to control access to resources within the system.
- **Common Security Measures**:
  - User authentication
  - Access control lists (ACLs)
  - Encryption

## 13. Important Commands (Linux)

1. **List Files**:
   ```bash
   ls -l
   ```

2. **Change Directory**:
   ```bash
   cd directory_name
   ```

3. **Copy Files**:
   ```bash
   cp source destination
   ```

4. **Move/Rename Files**:
   ```bash
   mv source destination
   ```

5. **Remove Files**:
   ```bash
   rm filename
   ```

6. **Display File Content**:
   ```bash
   cat filename
   ```

7. **Show Running Processes**:
   ```bash
   ps aux
   ```

8. **Kill a Process**:
   ```bash
   kill process_id
   ```

## 14. Common OS Concepts

- **Boot Process**: Sequence of events from powering on the computer to loading the OS.
- **Kernel Mode vs. User Mode**:
  - **Kernel Mode**: Full access to hardware and system resources.
  - **User Mode**: Restricted access for running user applications.
- **Multitasking**: Ability of the OS to execute multiple processes simultaneously.

---

### **Pro-Tip**:
- Understand the differences between **monolithic kernels** and **microkernels**.
- Be familiar with system calls and their role in OS.
- Study the impacts of **context switching** on system performance.

---

Good luck with your interview preparation! 🚀

---
