

````md
# WebSockets – Introduction (Pure WS) 🔌

## 📌 Overview
This project is a **basic introduction to WebSockets** using the **`ws` library** in Node.js with **TypeScript**.  
It demonstrates how real-time, two-way communication works between a client and a server **without using Express or HTTP servers**.

The project focuses on the **pure WebSocket approach**, making it easier to understand core WebSocket concepts.

---

## ✨ Features
- WebSocket server running on port **8080**
- Handles client connection events
- Listens for incoming messages from clients
- Implements a simple **Ping–Pong mechanism**
- Uses **TypeScript** for better type safety

---

## 🛠️ Tech Stack
- **Node.js**
- **WebSocket (`ws`)**
- **TypeScript**
- **Postman (for WebSocket testing)**

---

## 🧠 What I Learned
- What WebSockets are and **why they are different from HTTP**
- How WebSockets maintain a **persistent connection**
- Setting up a **pure WebSocket server** without Express
- Handling:
  - Client connections
  - Incoming messages
  - Server responses
- How real-time communication works (Ping → Pong)

---

## ⚙️ How It Works
1. A WebSocket server is created using `WebSocketServer`.
2. The server listens on **port 8080**.
3. When a client connects:
   - A connection event is triggered.
4. The server listens for messages from the client.
5. If the server receives `"ping"`:
   - It responds with `"pong"`.

This mimics real-time communication used in chats, live tracking, and multiplayer apps.

---

## 🚀 How to Run the Project

### 1️⃣ Install Dependencies
```bash
npm install
````

### 2️⃣ Start the Server

```bash
npm run dev
```

### 3️⃣ Test Using Postman

* Open **Postman**
* Click **New → WebSocket**
* Connect to:

  ```
  ws://localhost:8080
  ```
* Send:

  ```
  ping
  ```
* Server will respond with:

  ```
  pong
  ```

---

## 📂 Project Structure

```
websockets-01-intro/
│
├── src/
│   └── index.ts        # WebSocket server logic
│
├── dist/               # Compiled output
├── package.json
├── tsconfig.json
└── .gitignore
```

---

## 🔍 Key Notes

* This project does **not use Express**
* WebSocket types are installed separately:

  ```bash
  npm install ws @types/ws
  ```
* Demonstrates one of the **three WebSocket approaches**:

  1. HTTP-based
  2. Express-based
  3. **Pure WebSocket (used here)**

---

## 🚀 Future Improvements

* Broadcast messages to multiple clients
* Add client-side WebSocket implementation
* Implement rooms or channels
* Add authentication over WebSockets

---

## 📚 Ideal For

* Beginners learning WebSockets
* Understanding real-time communication basics
* Preparing for chat apps, live updates, or multiplayer systems

```


