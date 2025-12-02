# 🌐 Internet Basics

As a developer, it is important to have a solid understanding of what the internet is and how it works.

## 📚 Table of Contents
- [Introduction](#introduction)
- [How the Internet Works](#how-the-internet-works)
- [Switch](#-switch)
- [Router](#-router)
- [What Does the Internet Represent](#-what-does-the-internet-represent)
- [Meaning of Connecting to the Internet](#-meaning-of-connecting-to-the-internet)
- [Wide Area Network](#-wide-area-network)
- [Router 2](#-router-2)
- [Internet Service Provider](#-internet-service-provider)

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

## 🌐 What Does the Internet Represent

The internet is the **structure that connects all LANs across the world**.  
It is made up of millions of routers working together to forward packets reliably.

Connecting to to internet can stand for conneccting to the another computer in anywhere in the world.

### Why Many Routers?

- LAN 1 ↔ Internet ↔ LAN 2
- If there were only one giant router:
  - ⚠️ Single point of failure — if it breaks, the whole internet fails.
  - Overloading and impractical worldwide cabling.
- Solution: distribute traffic across **many routers**.

### Home Routers

- A home router combines **switch + router** functions.
- Suitable for small networks with a few devices.

### Packet Movement

### Diagram: LANs Connected Through the Internet
```text
   [LAN 1]
   [PC1] -- [Switch] -- [Router] --+
                                    |
                                    v
                                [Router 1]
                                    |
                                    v
                                [Router 2]
                                    |
                                    v
                                [Router 3]
                                    |
                                    v
   [PC1] -- [Switch] -- [Router] --+
   [LAN 2]
```

- Each router uses a **routing table** to decide the next hop.

- Routers perform **forwarding** and **route filtering**.

- Packets are sent via the **fastest available path** using algorithms.

- This happens in **milliseconds**.

### Fiber Optics vs Copper

- Internet backbone cables use **fiber optics**:

  - Faster transmission.

  - Longer distances with fewer errors.

- Copper is common in LANs but not ideal for global infrastructure.

### 🌍 Big Picture: What the Internet Represents

> The internet is a **network of networks**.

- Every LAN (LAN 1: home, LAN 2: friends, LAN 3: workplace, etc.) is part of the internet.

```text
 [LAN 1]   [LAN 2]   [LAN 3]   [LAN 4]   ... millions more
     |        |        |        |
     +--------+--------+--------+
                  |
              [Internet]
```

- Billions of devices — phones, tablets, computers, smart TVs — connect through these LANs.
- The internet is the **combination of all these networks**.

## 🌐 Meaning of Connecting to the Internet

When connecting to the internet, we primarily use the **router feature**.  
A home router also works, since it includes router capabilities.

### Example: Accessing YouTube

- User clicks a video on **youtube.com**.

- The computer creates a **packet** (request message).

- Packet flow:

  ```text
  PC → Home Router → Internet → YouTube Server
  ```

- The YouTube server receives the packet, processes the request, and sends the video back.

- Since the video is delivered piece by piece, this process is called **streaming**.

### Packet Transmission

- Packet transmission is the basis of:

  - Connecting to the internet.

  - Communicating with computers anywhere in the world.

### Servers

- A server is a much more powerful computer than a normal PC.

- Servers must handle connections from many users simultaneously.

- Example: YouTube servers manage millions of video requests.

- There are many servers across the internet — this avoids a single point of failure.

## 🌐 Wide Area Network

A **WAN (Wide Area Network)** is a combination of multiple LANs connected together.

### LAN and WAN

- LAN 1 + LAN 2 = WAN

- LANs are **private networks**.

- WANs use the **internet** to connect LANs across different locations.

### Why Use WAN Instead of Just Internet?

- The internet is a **public network** — everyone uses it.

- Hackers and vulnerabilities exist everywhere.

- Sending private files directly over the internet exposes them.

- A WAN provides **privacy and security** between LANs.

### Setting Up a WAN

- Use a **VPN (Virtual Private Network)**.

- VPN provides secure communication between LAN 1 and LAN 2.

- Example packet flow:

  ```text
  PC1 → Home Router → VPN Tunnel → Home Router → PC2
  ```

### VPN Techniques

- **Site-to-Site VPN** connects entire LANs securely.

- **Encryption**: protects the data.

- **Encapsulation**: wrapping a packet inside another packet.

- **Tunneling**: a special encapsulation method.

- On the receiving side:

  - **Decapsulation** removes the wrapper.

  - **Decryption** restores the original packet.

- Then the packet is delivered to the destination computer.

### Security Notes

- There is no such thing as **100% security**.

- Every system has vulnerabilities.

- Still, VPNs and WAN setups are **better than nothing**.

> The *largest WAN* in the world is **internet**.

## 🔌 Router 2

### Connecting Switches

- A single LAN can be created by connecting **two switches** together.

- The distance between switches must be short.

- Example: **Campus Area Network (CAN)**.

### Security Comparison

- Which is more secure: **WAN with VPN** or **LAN**?

  - LAN is always more secure since packets do not leave the local network.

  - Both can be secure, but LAN avoids exposure to the internet.

### Router Tasks

- LANs use **switches**.

- WANs use **routers**.

- Main task of a router: connect **different types of networks**.

### Campus Area Network (CAN)

  ```text
          LAN 1                          LAN 2
   +----------------+             +----------------+
   |   [PC1] [PC2]  |             |   [PC3] [PC4]  |
   |       |        |             |       |        |
   |    [Switch 1]  |             |    [Switch 2]  |
   +--------+-------+             +--------+-------+
            |                              |
            +------------+-----------------+
                         |
                      [Router]
                         |
                     [Internet]
  ```

## 🌐 Internet Service Provider

Internet Service Providers or ISPs are companies that enable users to connect to the internet.

### Types of ISPs

- **Local ISP**: connects neighborhoods.

- **Regional ISP**: connects cities within a country.

- **Global ISP**: connects countries across the world.


### ISP Hierarchy

```text
LAN 1   LAN 2   LAN 3
  |       |       |
  +---+---+-------+
          |
     Local ISP 1
          |
     Regional ISP 1
          |
     Global ISP 1
          |
     Global ISP 2
          |
     Regional ISP 2
          |
     Local ISP 2
  +---+---+-------+
  |       |       |
LAN 4   LAN 5   LAN 6

```

- Local ISPs 1, 2, 3 can connect to the same Regional ISP.

- Local ISPs + Regional ISPs = **Network of a Country**.

- Some Local ISPs may connect directly to Global ISPs:

  - Faster

  - Suitable location

  - Requires expensive infrastructure

### Point of Presence (PoP)

- A PoP is a physical location where ISPs connect.

- Can include switches, routers, servers, and other networking equipment.

### LAN to ISP

- A LAN can connect directly to a Regional ISP.

- Communication involves:

  - Sending a **request message** to a server.

  - Receiving a **response message** from the server.

- Note: The **packet path** from user → server may differ from server → user.

### Peering

- **Peering** is a direct connection between an ISP and a service provider (Google, Netflix, Microsoft, etc.).

- Purpose: faster access to servers and content.

  ```text
  Local ISP → Google Server
  ```
- YouTube is owned by Google, so it benefits from direct peering.

### Global ISP Responsibilities

- Handles international communications.

- Maintains the Internet Backbone.

- Connects through Internet Exchange Points (IXPs).

### Sources
- 📄 Article: [How does the internet work?](https://cs.fyi/guide/how-does-internet-work)
- 🎥 Video: [How does the internet work? (Full Course)](https://youtu.be/zN8YNNHcaZc?si=2XY2ikhJ3JSb81GR)
