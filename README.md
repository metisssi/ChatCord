# ChatCord - Real-time Chat Application

ChatCord is a real-time chat application built with Node.js, Express, and Socket.io that allows users to join different chat rooms and communicate in real-time.

## Features

- 🚀 Real-time messaging using WebSockets
- 🏠 Multiple chat rooms (JavaScript, Python, PHP, C#, Ruby, Java)
- 👥 User management with join/leave notifications
- 📱 Responsive design for mobile and desktop
- ⏰ Message timestamps
- 🎨 Modern UI with Font Awesome icons

## Tech Stack

- **Backend**: Node.js, Express.js, Socket.io
- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Dependencies**: moment.js for time formatting, qs for URL parsing

## How It Works

### 1. Initial Setup
- First, you need to enter your username and select a group
<img width="1919" height="1033" alt="Group selection" src="https://github.com/user-attachments/assets/4a767700-6f3b-4da5-8294-f534bd753a28" />

- After clicking "Join Chat", the chat interface opens
<img width="1919" height="944" alt="Chat interface" src="https://github.com/user-attachments/assets/785287a1-cb1d-452d-b360-97139704e402" />

- ChatCord Bot welcomes you with "Welcome to ChatRooms" and shows the current group and users

### 2. Multi-Client Support
- When opening a new browser window (new client) and joining the same group
<img width="1905" height="1018" alt="New client joining" src="https://github.com/user-attachments/assets/061a5987-0fd8-44ad-9705-c1995269993a" />

- User1 can see messages from test2 and test2's name appears in the USERS list
<img width="1914" height="1006" alt="image" src="https://github.com/user-attachments/assets/823d8fed-0d8a-429d-a3bf-3fa2aa56885b" />


### 3. Leave Room Functionality
- When clicking "Leave Room", you return to the main screen
<img width="149" height="37" alt="Leave room button" src="https://github.com/user-attachments/assets/6af7c031-6713-4548-bf85-d96d53f49382" />

- The first user receives a notification that the second user has left the chat
<img width="1387" height="613" alt="User left notification" src="https://github.com/user-attachments/assets/c732ba2f-192c-4ab6-8f30-be732c679605" />

- If you choose another chat room (for example, Rubo room), you will not see the previous users from the other room



 

## Project Structure

```
chat-rooms/
├── public/
│   ├── css/
│   │   └── style.css          # Application styles
│   ├── js/
│   │   └── main.js           # Client-side JavaScript
│   ├── index.html            # Landing/join page
│   └── chat.html             # Chat room interface
├── utils/
│   ├── messages.js           # Message formatting utilities
│   └── user.js               # User management functions
├── server.js                 # Main server file
└── package.json              # Project dependencies
```

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd chat-rooms
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

Or start the production server:
```bash
npm start
```

4. Open your browser and navigate to `http://localhost:3000`

## Usage

1. **Join a Room**: 
   - Enter your username on the landing page
   - Select a programming language room from the dropdown
   - Click "Join Chat"

2. **Chat**:
   - Type your message in the input field
   - Press Enter or click Send to send messages
   - View real-time messages from other users
   - See who's currently in the room in the sidebar

3. **Leave Room**:
   - Click the "Leave Room" button in the header
   - Or simply close the browser tab

## Available Chat Rooms

- JavaScript
- Python
- PHP
- C#
- Ruby
- Java

## API/Socket Events

### Client to Server Events
- `joinRoom`: Join a specific chat room with username and room name
- `chatMessage`: Send a message to the current room
- `disconnect`: Leave the current room

### Server to Client Events
- `message`: Receive a chat message
- `roomUsers`: Get updated list of users in the room

## Scripts

- `npm start`: Start the production server
- `npm run dev`: Start the development server with nodemon for auto-restart

## Dependencies

### Production Dependencies
- `express`: Web framework for Node.js
- `socket.io`: Real-time bidirectional event-based communication
- `moment`: Date and time formatting library

### Development Dependencies
- `nodemon`: Automatically restart the server during development

## Browser Compatibility

The application works in all modern browsers that support:
- WebSockets
- ES6+ JavaScript features
- CSS Grid and Flexbox



## Author

Andriy Simchera



## Future Enhancements

- [ ] User authentication
- [ ] Private messaging
- [ ] Message history persistence
- [ ] File sharing capabilities
- [ ] Custom room creation
- [ ] User profiles and avatars
- [ ] Message reactions/emojis
- [ ] Dark/light theme toggle
