iChat Chat Application
Introduction
iChat is a simple real-time chat application built using Socket.io, Node.js, and HTML/CSS/JavaScript. This project demonstrates basic real-time communication between multiple clients through a web socket server.
Features
- Real-time Messaging: Users can send and receive messages instantly.
- Join/Leave Notifications: Users are notified when someone joins or leaves the chat.
- Client-Side Audio Notification: A sound is played when a new message is received.
- Username Prompt: Users are prompted to enter their name before joining the chat.
Prerequisites
Before you begin, ensure you have met the following requirements:
- Node.js and npm installed on your machine.
Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ichat.git
   ```

2. Navigate to the project directory:
   ```bash
   cd ichat
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Start the server:
   ```bash
   node index.js
   ```

5. Open the application in your browser:
   Visit `http://localhost:8000` in your web browser.
Project Structure
```
.
├── css/
│   └── style.css        # Custom styles for the chat interface
├── js/
│   └── client.js        # Client-side JavaScript for managing chat functionalities
├── index.js             # Server-side script using Socket.io
├── iChat.html           # HTML file for the chat interface
├── iphone_ding.mp3      # Notification sound
└── README.md            # Project documentation
```
How It Works
- **Server-Side:** The `index.js` file initializes a Socket.io server on port 8000 and listens for events such as `new-user-joined`, `send`, and `disconnect`. It broadcasts messages to all connected clients except the one that sent the message.

- **Client-Side:** The client connects to the Socket.io server, sends and receives messages, and updates the DOM accordingly. The user is prompted to enter their name before joining the chat.
Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to create a pull request or open an issue.


