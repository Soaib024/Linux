# 1. The Big Picture

## 1.1 Levels and Layers of Abstraction in a Linux System
- User Processes (GUI, Servers, Shell)
- Linux Kernel (System calls, Process management, Memory management, Device drivers)
- Hardware (CPU, Main memory, Disks, Networks ports)

Code running in kernel mode has unrestricted access to the processor and main memory.

## 1.2 Hardware: Understanding Main Memory

## 1.3 The Kernel

The kernel is in charge of managing tasks in four general system areas:
- Processes, Memory, Device drivers, System calls and support

One user process may not access the private memory of another process, 
User processes can share memory. A device is typically accessible only in kernel mode because improper access (such as a user process asking to turn off the power) could crash the machine. 

Other than init (see Chapter 6), all new user processes on a Linux system start as a result of fork(), and most of the time, you also run exec() to start a new program instead of running a copy of an existing process. 

## 1.4 User Space

## 1.5 Users

