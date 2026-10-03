# 💬 Socket Chat - Real-Time Chat with ARCore Devices

A real-time two-person chat application using **Node.js**, **Express**, and **Socket.IO**. Works on any device with a browser (phones, tablets, ARCore devices).

## How It Works 🔧

**Server** (`server.js`) runs on your PC and:
- Accepts users joining a room with a code
- Broadcasts messages between 2 people in the same room
- Shows typing indicators and online status
- Max 2 people per room

**Client** (`public/index.html`) runs in the browser and:
- Lets users enter a name and room code
- Sends/receives messages in real-time via WebSocket
- Shows typing indicator when other person is typing
- Displays join/leave notifications

**Socket.IO** connects them instantly over WebSocket.

---

## Quick Start 🚀

1. **Extract** `socket-chat.rar`
2. **Open terminal** and go to the folder:
   ```bash
   cd socket-chat
   npm start
   ```
3. **Server runs** at `http://localhost:3000`

4. **On Device 1** (phone/PC):
   - Go to `http://192.168.1.100:3000` (your PC's IP)
   - Enter name: "Alice"
   - Enter room: "test-room"
   - Join

5. **On Device 2** (another phone/PC):
   - Go to `http://192.168.1.100:3000`
   - Enter name: "Bob"
   - Enter room: "test-room" (SAME room)
   - Join

**Both devices can now chat! 💬**

---

## Features ✨

✅ Real-time messaging  
✅ Typing indicator  
✅ Online status (🟡 waiting / 🟢 2 online)  
✅ Max 2 people per room  
✅ Mobile responsive  
✅ Join/leave notifications  

---

## Find Your PC IP 🖥️

**Windows:**
```bash
ipconfig
```
Look for **IPv4 Address** (e.g., `192.168.x.x`)

**Mac/Linux:**
```bash
ifconfig
```

Then use `http://YOUR-IP:3000` on your device.

---

## Files 📂

- `server.js` — Backend logic (rooms, messages, connections)
- `public/index.html` — Chat UI
- `package.json` — Project config
- `node_modules/` — Dependencies (auto-generated)

---

## Tech Stack

- Node.js + Express.js (server)
- Socket.IO (real-time communication)
- HTML/CSS/JavaScript (frontend)

---


License

Free to use and modify! 📄
