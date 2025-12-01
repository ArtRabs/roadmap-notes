# 🌐 Internet Basics

As a developer, it is important to have a solid understanding of what the internet is and how it works.

## 📚 Table of Contents
- [Introduction](#introduction)
- [How the Internet Works](#how-the-internet-works)
- [Switch](#-switch)
- [Router](#-router)

---

## Introduction

**Network** — A group of computers or other devices connected to each other.

**Example:** Computers, phones, and other devices can connect together through the internet to share information or play games.

> The internet is a **network of networks**.

The internet was **developed in the late 1960s** by the United States Department of Defense.  
It was designed as a **decentralized communication network** that could withstand a nuclear attack.

---

## How the Internet Works

At a high level, the internet works by connecting devices and computer systems together using a set of standardized protocols.

These protocols define how information is exchanged between devices and ensure that data is transmitted reliably and securely.

The core of the internet is a global network of interconnected **routers**, which are responsible for directing traffic between different devices and systems.



```
[Your Device]
      |
      |  sends data (packets)
      v
+-------------+
|   Router 1  |
+-------------+
      |
      |  forwards packet
      v
+-------------+
|   Router 2  |
+-------------+
      |
      |  forwards packet
      v
+-------------+
|   Router 3  |
+-------------+
      |
      |  continues until destination
      v
[Destination Device / Server]
```

- Your device breaks data into **packets**.
- Each router examines the **packet header** and decides the next hop.
- The packet travels router by router until it reaches the final destination.
- This process is repeated for every packet, which is why the internet is often called a **network of networks**.

## 🔌 Switch

- A **switch** connects multiple PCs together in a **Local Area Network (LAN)**.
- Example: PC1, PC2, … PC7 all connect to the switch using cables.
- **Cables used:**
  - `CAT-5` and `CAT-6` (Category cables; CAT-6 is faster).
  - Fiber optic cables are faster than copper cables.
- **Limitations:**
  - Switches only work with cables (no wireless).
- **Alternative:**
  - An **Access Point (AP)** provides wireless connectivity instead of cables.
- **Communication:**
  - PCs can only communicate if they are in the same network (LAN).
  - Example packet flow:
    ```text
    PC1 → Switch → PC6
    ```
    If this happens, PC1 and PC6 are on the same network and can communicate.
- **Ports:**
  - Switch has LAN ports.
  - PCs have LAN ports.

⚠️ At this stage: PCs are connected in a LAN, but **no internet yet**.

### Diagram: LAN with Switch
```text
   [PC1]   [PC2]   [PC3]   [PC4]   [PC5]   [PC6]   [PC7]
      |      |      |       |       |       |       |
      +------+------+-------+-------+-------+-------+
                             |
                          [Switch]
```

---

## 🌐 Router

- A **router** connects the LAN (via the switch) to the **Internet**.
- **ISP (Internet Service Provider)** provides the cable for internet access.
- **Roles:**
  - Switch handles LAN communication (PC1 ↔ PC5).
  - Router does not manage LAN communication directly.
  - Router enables PCs to send packets to the internet.
- **Packet flow:**
  ```text
  PC1 → Switch → Router → Internet
  ```
  ```text

     [PC1]   [PC2]   [PC3]   [PC4]   [PC5]   [PC6]   [PC7]
      |      |      |       |       |       |       |
      +------+------+-------+-------+-------+-------+
                             |
                          [Switch]
                             |
                          [Router]
                             |
                          [Internet]

  ```
  
### Sources
- 📄 Article: [How does the internet work?](https://cs.fyi/guide/how-does-internet-work)
- 🎥 Video: [How does the internet work? (Full Course)](https://youtu.be/zN8YNNHcaZc?si=2XY2ikhJ3JSb81GR)
