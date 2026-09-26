# Local Process Chat System

A local chat system that enables communication between processes running on the same machine using **shared memory**.

The project uses **semaphores** to synchronize access to shared resources and prevent processes from accessing the shared memory in an unsafe manner.

A graphical user interface (GUI) is included to provide an interactive way for users to send and receive messages.

## Project Overview

The purpose of this project is to demonstrate **Inter-Process Communication (IPC)** and process synchronization.

Multiple processes communicate through a shared memory region, while semaphores coordinate access to the shared resource.

## Key Features

- 💬 Local communication between processes
- 🧠 Shared memory for inter-process communication
- 🔐 Semaphore-based synchronization
- 🖥️ Graphical User Interface
- 📩 Sending and receiving messages
- ⚙️ Demonstration of concurrent processes
- 🔄 Synchronized access to shared resources

## How It Works

The system uses shared memory as a communication area between processes.

The general workflow is:

```text
Process 1
    │
    │ Write Message
    ↓
┌─────────────────┐
│  Shared Memory  │
└─────────────────┘
    │
    │ Read Message
    ↓
Process 2
