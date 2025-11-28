# 🌐 Internet

As a developer, it is important to have a solid understanding of what the internet is and how it works.

## Table of Contents
- [Introduction to the Internet](#introduction-to-the-internet)
- [How the Internet Works: An Overview](#how-the-internet-works-an-overview)

---

## Introduction to the Internet

**Network** — A group of computers or other devices connected to each other.

**Example:** Computers, phones, and other devices can connect together through the internet to share information or play games.

> The internet is a **network of networks**.

The internet was **developed in the late 1960s** by the United States Department of Defense.  
It was designed as a **decentralized communication network** that could withstand a nuclear attack.

---

## How the Internet Works: An Overview

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

**Source:** [How does the internet work?](https://cs.fyi/guide/how-does-internet-work)