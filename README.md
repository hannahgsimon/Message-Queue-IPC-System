# Message Queue IPC System

This project demonstrates **interprocess communication (IPC)** using **System V message queues** in C/C++. It focuses on safe and structured message passing between processes, illustrating how operating systems support asynchronous communication without shared memory.

## ✨ Features
- IPC using System V message queues
- Structured message definitions
- Explicit send/receive logic
- Clear separation of interface and implementation
- Error-aware message handling

## 🛠️ Technologies Used
- C / C++
- Linux System V IPC
  - Message queues
- GCC / G++

## 📁 Project Structure
```bash
.
├── Message_que.h            # Message queue interface and structures
├── Message_que.cpp          # Message queue implementation
└── Message_que_demo.cpp     # Driver / test program
```

## ⚙️ How It Works
- A message queue is created using a unique key.
- Messages are packaged into structured formats.
- Sending processes enqueue messages into the system queue.
- Receiving processes dequeue messages based on type.
- The OS ensures ordered, safe delivery without shared memory.
- This approach avoids race conditions common in shared-memory designs and highlights OS-managed synchronization.

## 🧪 Build & Run
Compile using G++:
```bash
g++ message_queue_demo.cpp Message_que.cpp -o Message_queue_demo
```

Run:
```bash
./message_queue_demo
```
⚠️ This program is intended to be run on a Linux-based system with System V IPC support.

---

## 📜 License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## 📬 Contact
For questions or feedback, please contact Hannah G. Simon at hgsimon2@gmail.com.
