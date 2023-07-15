# Realtime-Canvas

## Canvas Drawing App with Socket.io
This project is a simple canvas drawing application built using React for the frontend and Express.js with Socket.io for the backend. It allows users to draw on a canvas and share their drawings with other users in real-time using WebSockets.

## Features
Real-time drawing: Multiple users can draw on the canvas simultaneously, and their changes will be instantly visible to all other connected users.

Brush customization: Users can change the brush color and size to create different types of drawings.

Eraser: Users can switch to an eraser mode to remove any parts of their drawing.

Clear canvas: Users can clear the entire canvas to start fresh.

Save canvas data: The app stores the canvas data on the server and broadcasts it to all connected clients, so that when a new user joins, they can see the existing drawings.

## Installation
To run the application, follow these steps:

1.Clone the repository:
git clone https://github.com/yourusername/canvas-drawing-app.git

2.Install the dependencies for both the frontend and backend:
cd canvas-drawing-app
cd client
npm install
cd ../server
npm install

3.Run the server and client in separate terminal windows:
* In the server directory
npm start

* In the client directory
npm start
The application should now be accessible at http://localhost:3000.

## Server (Backend)
The backend of the application is built using Express.js and Socket.io. It sets up a WebSocket server using the socket.io library to handle real-time communication between clients. When a user draws on the canvas, the server receives the drawing data and broadcasts it to all other connected clients.

## Client (Frontend)
The frontend is built using React and renders the canvas where users can draw. It also provides buttons to customize the brush, switch to eraser mode, and clear the canvas. The frontend establishes a WebSocket connection with the server to receive updates about other users' drawings.

## Dependencies

## Backend (server)

Express.js: Web framework for the backend.

Socket.io: Library for real-time WebSocket communication.

## Frontend (client)

React: JavaScript library for building user interfaces.

Socket.io-client: Library to connect to the WebSocket server on the backend.


## Improvements
This is a basic implementation of a real-time canvas drawing app. To make it more robust and feature-rich, you can consider the following improvements:

User authentication: Implement user authentication to allow only registered users to draw and share their drawings.

Persistent drawings: Store the drawings in a database so that they are not lost when the server restarts.

Drawing tools: Add more drawing tools, such as shapes, text, and an undo/redo feature.

Share drawings: Allow users to share their drawings through a unique URL or by saving them as images.

