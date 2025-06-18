# Multi-Thread Chat Application 💬🔗

A lightweight, real-time chat system built from scratch using Python sockets, threading, and PyQt5.  
This client-server project supports multiple users, public and private messaging, and a dynamic GUI.

---

## 🚀 Features

- **User Registration**: Connect with a unique username.  
- **Public Chat**: Broadcast messages to all connected users.  
- **Private Messaging**: Send direct messages to specific participants.  
- **Active User List**: View real-time list of online users.  
- **Emoji Support**: Quick-send emoji buttons in the chat client.  
- **Graceful Disconnection**: Properly handle users leaving the chat.

---

## 🏗️ Architecture

- **Server (server.py)**  
  - Built with Python’s `socket` and `threading` libraries.  
  - Listens for clients, spawns a dedicated thread per connection.  
  - Handles registration (`{REGISTER}`), broadcasting (`{ALL}`), private messaging, client listing (`{CLIENTS}`), and disconnection (`{QUIT}`).

- **Client (gui.py)**  
  - GUI implemented using **PyQt5**.  
  - Separate tabs for connection setup and chat room.  
  - Background thread listens for server messages to keep the UI responsive.  
  - Supports emojis, message history scroll, and dynamic recipient selection.

---

## 💻 Requirements

- Python 3.7 or higher  
- PyQt5  

Install PyQt5 via pip:

```bash
pip install PyQt5
```

---

## 🛠 Installation & Usage

1. **Clone the repository**  
   ```bash
   git clone https://github.com/yourusername/multithread-chat-app.git
   cd multithread-chat-app
   ```

2. **Start the server**  
   ```bash
   python server.py --host 127.0.0.1 --port 33002
   ```
   ![Image](https://github.com/user-attachments/assets/f74a3eca-a386-43c6-b6d3-0f65439f627a)

   ⚠️running ```GUI``` without ```srver``` occurs ```Status:Refused```

   ![Image](https://github.com/user-attachments/assets/64b358f9-1030-4360-b5ff-078135a27e0f)

   ⚠️Enter your name

   ![Image](https://github.com/user-attachments/assets/9f51f1fa-f1d5-4017-8f3c-fc37b0d40200)



4. **Launch the client**  
   ```bash
   python gui.py
   ```
   ![Image](https://github.com/user-attachments/assets/6071998d-6231-40a1-ade2-90854a470768)
   

5. **Connect**  
   - Enter server IP, port, and your username.  
   - Click **Connect** to join the chat room.

   ![Image](https://github.com/user-attachments/assets/6127d7b6-ff31-4f9b-b268-06c60844ed64)

   - Chat Room
     
   ![Image](https://github.com/user-attachments/assets/05982962-779f-4326-99ed-5dadb006e720)

    
   - Run-Time Chat

   ![Image](https://github.com/user-attachments/assets/06422673-6d63-4b76-a674-2e46aa4cdd9d)
    
---
## 📂 Project Structure

```
multithread-chat-app/
├── server.py            # Chat server implementation
├── gui.py               # PyQt5-based chat client GUI
└── README.md            # Project documentation
```

---

## 👥 Team Members

- Sheghaf Faraj Mohamed     
- Omar Ahmed Elragaby  
- Aya Ahmed Mohamed 
- AbdulRahman Essam Shoukry (me)
- Ahmed Mesbah Ahmed 

---

## 📜 License

This project is licensed under the **MIT License**.  
Feel free to use, modify, and distribute with attribution.
