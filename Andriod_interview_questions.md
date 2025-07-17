# Android
# 📱 Android & Embedded Systems Q&A

## Android & Embedded System Basics

**Q1: What is an embedded system?**  
A: An embedded system is a combination of hardware and software designed to perform a specific task.

**Q2: Why are embedded systems used?**  
A: They are efficient, cost-effective, compact, and consume less power.

**Q3: Is a smartphone a complete embedded system?**  
A: No, it’s a complex system made up of multiple embedded systems like camera, display, and sensors.

**Q4: Give two examples of embedded systems in a phone.**  
A: Camera Module, Fingerprint Sensor.

---

## ⚠️ Embedded Systems Safety Classification

**Q5: What defines a safety-critical embedded system?**  
A: Failure may harm human life; it requires deterministic timing and uses simpler OS like FreeRTOS or Baremetal.

**Q6: What type of OS is used in non-safety-critical embedded systems?**  
A: Linux or Android.

**Q7: Which embedded system requires minimal user input?**  
A: Safety-critical systems.

---

## 🏗️ Embedded System OS Stack

**Q8: What is the purpose of the Application layer in embedded systems?**  
A: It provides the user interface and functionality.

**Q9: What does the driver layer do?**  
A: It interacts with hardware through the kernel space.

**Q10: What bridges user space and kernel space?**  
A: System Call Interface.

---

## 🔨 Build System & Firmware

**Q11: What is a build system?**  
A: A tool that automates the conversion of source code into executable files.

**Q12: What is a toolchain in embedded systems?**  
A: A set of tools (like `gcc`) used to compile and build software.

**Q13: Name 3 output files from an Android build system.**  
A: RootFS Image, Kernel Image, Bootloader Image.

---

## 📊 Android vs Linux

**Q14: Which C library does Android use?**  
A: Bionic C.

**Q15: What scheduling algorithm does Android use?**  
A: Completely Fair Scheduler (CFS) with red-black tree.

**Q16: What is Vruntime in CFS?**  
A: Virtual runtime = CPU Time × Weight, used to decide process priority.

**Q17: What is the role of the Low Memory Killer (LMK)?**  
A: It kills low-priority apps when RAM is low.

**Q18: How is logging different in Android vs Linux?**  
A: Android uses `logcat`, Linux uses `journalctl`.

---

## 😴 Power Management in Android

**Q19: What is a wakelock in Android?**  
A: A feature that prevents the device from sleeping during important tasks.

**Q20: What does the sleep-prone kernel do?**  
A: Allows the kernel to suspend the CPU during inactivity.

---

## 🔌 Interprocess Communication (IPC)

**Q21: What IPC mechanism does Android use?**  
A: Binder IPC.

**Q22: What IPC does Linux use?**  
A: System V IPC like pipes and message queues.

---

## 🔧 HAL and Drivers

**Q23: What does HAL stand for?**  
A: Hardware Abstraction Layer.

**Q24: What does HAL do in Android?**  
A: Acts as a bridge between hardware and Android Framework.

**Q25: What is the difference between AIDL and HIDL?**  
A: AIDL is Java-based and uses Binder IPC; HIDL is C++-based and supports both Binder IPC and direct calls.

---

## 🧠 Android Architecture

**Q26: What are the 3 types of Android apps?**  
A: System Apps, User Apps, Privileged Apps.

**Q27: What are Android APIs?**  
A: Predefined interfaces to interact with system features like camera, GPS.

**Q28: What is the Android Framework?**  
A: Java-based layer that manages system services like ActivityManager, NotificationManager.

---

## 🔁 Android Runtime & Zygote

**Q29: What replaced Dalvik VM in Android?**  
A: Android Runtime (ART) with AOT (Ahead of Time) compilation.

**Q30: What is the role of Zygote?**  
A: It preloads system resources and forks new processes for applications.

**Q31: What does `.dex` stand for?**  
A: Dalvik Executable — compressed bytecode optimized for Android.

**Q32: How is ART faster than Dalvik?**  
A: It uses AOT to compile code to native machine code before execution.

---

## 🔋 Boot Process

**Q33: What is BootROM?**  
A: The first code that runs, stored in read-only memory.

**Q34: What is the role of the Bootloader?**  
A: Loads the kernel and initializes hardware from flash memory.

---
