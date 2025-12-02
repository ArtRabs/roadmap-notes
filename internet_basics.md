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

## What does the Internet Represent

There are many routers in internet.

LAN 1 <-> Internet <-> LAN 2

Connecting to to internet can stand for conneccting to the another computer in anywhere in the world.

Internet is the strucutre that connect all LANs all over the world.

In internet there are many routers.

LAN 1 <-> Router 1 - Router 2 - Router 3 - ... <-> LAN 2

If there are millions of LANs in the world, then it is obvious to use many routers as well.

If there is no switch, how to LAN?

If there is no router, how to connect to internet?

Home router, it consist both switch and router capabilities.

But only use home router if you have few devices, enough for usual home.

If there is only one router to connect, let us say a giant router of some sort, then cool.

But what if, it broke?

All to lot and single point of failure.

If that router failed, everybody fails connecting to internet.

So just use many routers.

Remember how to connect to router normally?

PC 1 -> Switch -> Router -> Internet

Switch to router uses cable but router to internet does not

Imagine again the there is only one big router, then all cables all over the world is connected to that big router just to connect to internet.

Disadvantages were overloading, world wide long cables, single point of failure.

But who knows, somebody might use that kind of router and solved those disadvantages, or perhaps use that disadvantages as a exclusitivity.

Even pirates found and sold cables that very long, I mean there is nothing to stop them.

Another reason why use many routers instead. 

Also there are country wide cables, at least not world wide, distributed to whole world. (The stuff pirates sold off)

They all use fiber optics instead of copper.

Why?

Because it is fast and long lenght of it will perhaps not cause error in data transmission.

How packet moves in internet

LAN 1 -> LAN2

Inside the LAN 1
 PC1 -> Switch -> Router -> Internet
 Inside the internet
  Router 1 -> Router 2 -> Router 3 -> ...
  Router X -> LAN 2

Each router must have s specific table called Routing Table

Forwarding, after a router recieve a packet

Route Filtering, each router has a special processors

Packet must always be sent in the fastest way

There are many ways, many routers in internet, so the packet can be sent in many routers just to get from LAN 1 to LAN 2, but packet a special algorithm to go the fastest way.

Also it is miliseconds happening.

Remember that

> The internet is a **network of networks**.

We all have many kinds of devices like phone, tablet, computer, smart television, and so on.

So in our home is LAN 1, our friends is LAN 2, neighbor is LAN 3, and there are many more people in this world, so there is a lot of LAN

So every LAN connected to internet, is also the internet itself.

Combination of all these networks.


### Sources
- 📄 Article: [How does the internet work?](https://cs.fyi/guide/how-does-internet-work)
- 🎥 Video: [How does the internet work? (Full Course)](https://youtu.be/zN8YNNHcaZc?si=2XY2ikhJ3JSb81GR)
