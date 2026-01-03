# OS Intro — Foundations

> *Phase 0.0.0 · kernel-er*


## What is an Operating System?

An **Operating System (OS)** is a collection of **system-level software programs** that acts as a **vital interface between computer hardware and the end user**.

In simple terms, the OS:

* Sits between **hardware** and **applications**
* Controls and coordinates the **entire computer system**
* Manages physical resources such as:

  * **CPU (processor)**
  * **Main memory (RAM)**
  * **Secondary storage (disk space)**

Without an OS, application software would need to directly deal with hardware complexity—which is inefficient, error-prone, and unrealistic.


## Primary Goals of an Operating System

The core purposes of an OS are:

1. **Ease of Use**
   Make the computer system simple and convenient for users and programmers.

2. **Efficiency**
   Use hardware resources effectively to maximize performance.

3. **Problem Solving**
   Provide abstractions and services that allow programs to be written and executed easily.

An OS is not just about control—it is about **making powerful hardware usable**.


## The Most Important Concept: Virtualization

At the heart of modern operating systems lies the concept of **virtualization**.

**Virtualization** means:

> The OS takes **physical hardware resources** and transforms them into **virtual, easier-to-use abstractions**.

Instead of forcing programs to deal with raw hardware, the OS presents a **clean, powerful illusion** of resources.


## Types of Virtualization

### 1. CPU Virtualization

* A computer may have **one physical CPU**, but the OS creates the *illusion* of **multiple virtual CPUs**.
* This allows the system to run **multiple programs at the same time**.
* The OS rapidly switches the CPU between tasks, making them appear to execute simultaneously.

 Result: **Concurrency on a single processor**.


### 2. Memory Virtualization

* **Physical memory model**: a simple array of bytes in RAM.
* **Virtualization effect**:

  * Each process is given its **own private virtual address space**.
  * Processes are isolated from one another.

This ensures:

* Safety (one process cannot corrupt another)
* Simplicity (programs can assume contiguous memory)
* Efficient memory management

 Result: **Illusion of private memory for every process**.


### 3. System Calls and APIs

Applications do **not** directly access hardware.

Instead:

* Programs use **Application Programming Interfaces (APIs)**
* APIs internally invoke **system calls**

System calls allow programs to:

* Create and execute processes
* Access files and devices
* Request memory
* Communicate with the OS kernel

 Result: Applications remain **hardware-independent**, while the OS handles low-level details.


## OS as a Layered System

The OS acts as a **layer**:

```
Applications
────────────
Operating System
────────────
Hardware
```

It manages this relationship using several architectural features:

### Key Architectural Components

1. **Kernel**
   The core of the OS that runs in privileged mode and controls system resources.

2. **Dual Mode Operation**

   * User Mode: limited access
   * Kernel Mode: full hardware access

3. **Traps and System Calls**
   Controlled entry points from user mode to kernel mode.

4. **Device Drivers and Controllers**
   Software components that manage hardware devices.

5. **Interrupts**
   Mechanism for hardware and software to signal the CPU for immediate attention.



An Operating System is not just software—it is a **resource manager, illusion maker, and protector** of the system.

---

**Created:** Jan-03-2026 /
**Updated:** Jan-03-2026
