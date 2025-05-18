# Wifi_Lock

**Wifi_Lock** is a collection of network programming examples and tools developed as part of the ECE369 course. It encompasses various client-server models using TCP and UDP protocols, implemented in Python, MATLAB, and Arduino. The repository serves as a practical resource for understanding and experimenting with network communication concepts.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Description](#Project-Description)
- [MATLAB Communication](#MATLAB-Communication)
- [Python Socket Programming Examples](#Python-Socket-Programming-Examples)
- [File Structure](#file-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [License](#license)

---

## Overview

This repository includes a variety of scripts and programs that demonstrate:

- TCP and UDP client-server communication
- Multithreaded server implementations
- Peer-to-peer networking
- GUI-based client interfaces
- Integration with Arduino for hardware communication

These examples are designed to provide hands-on experience with socket programming and network communication protocols.

---

## Features

- **Multilingual Implementations**: Examples in Python, MATLAB, and Arduino
- **Comprehensive Coverage**: Includes echo servers, peer-to-peer clients, GUI-based clients, and multithreaded servers
- **Educational Focus**: Great for learning and experimenting with networking concepts

---

## Project Description

This project was originally developed as part of our Junior Design (ECE 388) course and centers around a custom-built Wi-Fi-enabled door lock system. The system uses an **Arduino Uno R4 WiFi** board to control a physical lock mechanism, allowing remote operation over a wireless network.

The Python-based **GUI Client** in this repository communicates with the Arduino over Wi-Fi, sending commands to **lock** or **unlock** the door in real time. The Arduino receives these commands via a simple socket server implementation and actuates the lock accordingly.

This setup simulates a smart home security device and demonstrates integration between hardware (Arduino and servo lock) and software (Python socket programming and GUI). The project highlights concepts in IoT, embedded systems, and network programming.

---

## MATLAB Communication

As part of our exploration of network protocols, we implemented client-server communication in **MATLAB** to send and receive data packets between two computers on the same network. These scripts demonstrate the core principles of socket-based communication in a high-level computing environment.

The implementation includes:

- `TCPClient.m` and `TCPServer.m`: Scripts that establish a TCP connection where the client sends messages to the server and receives acknowledgments.
- `UDPClient.m` and `UDPServer.m`: Scripts that demonstrate connectionless communication using UDP, suitable for lightweight or real-time data transmission.
- `UDPClientTimer.m`: A modified UDP client that includes timestamping to measure **round-trip time (RTT)** and evaluate performance under various network conditions.

This MATLAB-based approach enabled us to visualize and test real-time data transmission, latency, and socket reliability in a controlled setting, helping bridge the gap between theory and hands-on implementation of networking protocols.

---

## Python Socket Programming Examples

This repository includes a variety of Python scripts designed to demonstrate fundamental and advanced concepts in socket programming. These examples were created to progressively build an understanding of how devices communicate over networks using TCP and UDP protocols.

### TCP Examples

- **`TCPEchoClient.py` / `TCPEchoServer.py`**  
  Demonstrates a basic client-server model using TCP sockets. The client sends a message, and the server echoes it back. This teaches the core concepts of connection-oriented communication, handshaking, and stream-based data transfer.

- **`MultithreadedServer.py`**  
  Enhances the TCP server by allowing it to handle multiple clients simultaneously using Python’s threading module. This example introduces concurrency in networking, which is critical for building scalable applications.

- **`TCPpeeroneother.py` / `TCPpeertopeer.py`**  
  Simulates peer-to-peer communication where both ends act as both client and server. This model is useful for decentralized systems and teaches the concept of bidirectional communication.

### UDP Examples

- **`UDPEchoClient.py` / `UDPEchoserver.py`**  
  A basic example of connectionless communication using UDP. These scripts show how to send and receive messages without establishing a persistent connection, which is useful in low-latency or lossy environments.

- **`UDPTimerClient.py` / `UDPTimerServer.py`**  
  These add timing logic to measure round-trip delay or assess network performance, illustrating how UDP can be used in time-sensitive applications like gaming or real-time telemetry.

- **`UDPpeeroneother.py` / `UDPpeertopeer.py`**  
  Similar to the TCP peer scripts, but using UDP. This teaches how to build decentralized communication systems using connectionless protocols.

---

These Python scripts collectively introduce key socket programming concepts:
- Sockets and ports
- TCP vs. UDP behavior
- Client-server architecture
- Peer-to-peer models
- Multithreading and concurrency
- Real-time communication and timing analysis
- Hardware integration via network

Together, they offer a well-rounded foundation for understanding how data flows between devices on a network and how different protocols are suited to different applications.


---

## File Structure

Some key files in this repository include:

- `ArduinoServer.c`: C script for Arduino communication over network
- `GuiClient.py`: Python-based graphical user interface client

- `MultithreadedServer.py`: TCP server using multithreading to handle multiple clients using TCP Echo Client
- `TCPEchoClient.py` / `TCPEchoServer.py`: Basic TCP echo model
- `TCPpeeroneother.py` / `TCPpeertopeer.py`: Peer-to-peer TCP communication
- `UDPEchoClient.py` / `UDPEchoserver.py`: Basic UDP echo model in Python
- `UDPpeeroneother.py` / `UDPpeertopeer.py`: Peer-to-peer UDP communication
- `UDPTimerClient.py` / `UDPTimerServer.py`: Timed UDP communication

- `TCPClinet.m` / `TCPServer.m` : MATLAB TCP client and Server
- `UDPClinet.m` / `UDPClinetTimer.m`: MATLAB UDP clients with timing features
  
- `ECE369-main.zip`: ZIP archive of the project contents

---

## Getting Started

To explore and run the examples:

### 1. Clone the repository

```bash
git clone https://github.com/brandall03/Wifi_Lock.git
cd Wifi_Lock

