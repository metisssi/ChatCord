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

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Author

Andriy Simchera

## License

This project is licensed under the ISC License.

## Future Enhancements

- [ ] User authentication
- [ ] Private messaging
- [ ] Message history persistence
- [ ] File sharing capabilities
- [ ] Custom room creation
- [ ] User profiles and avatars
- [ ] Message reactions/emojis
- [ ] Dark/light theme toggle
