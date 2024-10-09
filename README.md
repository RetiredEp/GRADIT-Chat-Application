
# GRADIT Chat Application

Welcome to the **GRADIT Chat Application**! This project is a real-time chat application designed for students to connect, communicate, and collaborate seamlessly. The application is structured with two primary components: a **client** built with React and a **server** built with Node.js and Express.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Directory Structure](#directory-structure)
- [Getting Started](#getting-started)
- [Client Overview](#client-overview)
- [Server Overview](#server-overview)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Overview

The **GRADIT Chat Application** enables users to join chat rooms and communicate in real-time. Students can interact with peers, exchange ideas, and work together in a dynamic environment. The application features a clean and intuitive user interface for easy navigation.

## Features

- **Real-Time Messaging**: Communicate instantly with other users in a chat room.
- **Multiple Chat Rooms**: Join different chat rooms based on interests or subjects.
- **User-Friendly Interface**: Simple and responsive design for a seamless experience.
- **Message History**: View past messages exchanged in the chat room.
- **Exit Room Option**: Easily leave the chat room when done.

## Tech Stack

- **Frontend**: 
  - **React**: A JavaScript library for building user interfaces.
  - **React Router**: For managing navigation and routing within the application.
  - **Socket.io**: For real-time communication between clients and server.

- **Backend**: 
  - **Node.js**: JavaScript runtime for building server-side applications.
  - **Express**: A web application framework for Node.js.
  - **Socket.io**: For enabling real-time, bi-directional communication between web clients and servers.

## Directory Structure

```
GRADIT-Chat-Application
├── client
│   ├── public
│   ├── src
│   │   ├── components
│   │   │   ├── ChatComponent.js
│   │   │   ├── InfoBar.js
│   │   │   ├── Input.js
│   │   │   └── Messages.js
│   │   ├── App.js
│   │   └── index.js
│   └── package.json
└── server
    ├── index.js
    └── router.js
```

## Getting Started

To get a local copy of the application up and running, follow these steps:

### Prerequisites

Make sure you have the following installed on your machine:

- [Node.js](https://nodejs.org/en/download/) (v14 or higher)
- [npm](https://www.npmjs.com/get-npm) (comes with Node.js)

### Clone the Repository

1. Clone the repository:

   ```bash
   git clone https://github.com/RetiredEp/GRADIT-Chat-Application.git
   cd GRADIT-Chat-Application
   ```

### Setup Client

1. Navigate to the client directory:

   ```bash
   cd client
   ```

2. Install the client dependencies:

   ```bash
   npm install
   ```

3. Start the client development server:

   ```bash
   npm start
   ```

   The client application will be running on [http://localhost:3000](http://localhost:3000).

### Setup Server

1. Open a new terminal and navigate to the server directory:

   ```bash
   cd server
   ```

2. Install the server dependencies:

   ```bash
   npm install
   ```

3. Start the server:

   ```bash
   npm start
   ```

   The server will be running on [http://localhost:5000](http://localhost:5000).

## Client Overview

The client-side of the application is structured as follows:

- **App.js**: The main application component that sets up routing.
- **components**: Contains reusable components:
  - **ChatComponent.js**: Displays the chat interface when the user navigates to the `/chat` endpoint.
  - **InfoBar.js**: Shows the current room name and provides an option to exit the room.
  - **Messages.js**: Renders the list of messages exchanged in the chat room.
  - **Input.js**: Contains the input field for entering messages and the send button.

## Server Overview

The server-side of the application is responsible for handling WebSocket connections and routing:

- **index.js**: The main server file that initializes the Express app and sets up Socket.io for real-time communication.
- **router.js**: Manages routing for API endpoints, allowing for organized request handling.

## API Endpoints

### WebSocket Endpoint

- **`/`**: The main WebSocket endpoint for real-time communication. Use Socket.io to connect from the client.

## Contributing

Contributions are welcome! To contribute to this project, follow these steps:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
