Streamify 🌊
Streamify is a full-stack MERN application designed to connect language learners from around the world. It's more than just a chat app; it's a dedicated platform for users to find native speakers, make friends, and practice their skills through real-time text chat and video calls.

This project was built from scratch and features a secure, cookie-based authentication system, a real-time backend, and a modern, responsive React frontend.

📸 Key Features
Secure User Authentication: Full signup, login, and logout flow using JWT (JSON Web Tokens) stored in secure HttpOnly cookies.

Real-Time Chat: Instantly message other users (powered by Socket.IO).

Live Video Calls: Start 1-on-1 video calls with friends (powered by WebRTC).

User Discovery: Find new language partners and manage a friends list.

Notifications: Receive real-time notifications for messages and requests.

User Onboarding: A multi-step process for new users to set up their profiles, native language, and learning goals.

Modern UI: A clean, responsive user interface built with Tailwind CSS.

Client-Side State Management: Uses React Query (@tanstack/react-query) to efficiently manage server state, cache data, and provide a smooth UX.

🛠️ Tech Stack
This project is a full-stack MERN application with a few modern tools.

Frontend
React: A JavaScript library for building user interfaces.

React Router: For client-side routing and navigation.

React Query: For server state management, caching, and data fetching.

Tailwind CSS: A utility-first CSS framework for rapid UI development.

Axios: For making HTTP requests to the backend API.

Socket.IO Client: For real-time communication with the server.

Lucide Icons: For clean, beautiful icons.

Backend
Node.js: A JavaScript runtime for the server.

Express.js: A minimal and flexible Node.js web application framework.

MongoDB: A NoSQL database for storing user data, messages, and more.

Mongoose: An elegant MongoDB object modeling tool for Node.js.

JSON Web Tokens (JWT): For creating secure access tokens.

Bcrypt.js: For hashing user passwords securely.

Socket.IO: For enabling real-time, bidirectional communication.

🚀 Getting Started
To run this project on your local machine, follow these steps.

Prerequisites
Node.js (v18 or later recommended)


**1. Clone the Repository**
git clone [https://github.com/your-username/streamify.git](https://github.com/your-username/streamify.git)
cd streamify
2. Backend Setup
The backend server handles all API logic, database operations, and real-time connections.

# Navigate to the backend folder
cd backend

# Install all required dependencies
npm install

# Create a .env file in the /backend folder
# and add your environment variables:
touch .env

Your backend/.env file must contain the following variables:

# Your MongoDB connection string
MONGO_URI=mongodb+srv://...

# A strong, random string for signing JWTs
JWT_SECRET=YOUR_SUPER_SECRET_KEY_HERE

# The port for the backend server to run on
PORT=5001

Once your .env file is ready, you can start the backend server:

# Start the server (using nodemon for development)
npm run dev

# Or just run the server
npm start

Your backend should now be running on http://localhost:5001.

3. Frontend Setup
The frontend is the React application that users interact with.

# Open a NEW terminal window
# Navigate to the frontend folder (if you have one)
# If your frontend is in the root, just run npm install from the root.
cd frontend

# Install all required dependencies
npm install

# Start the React development server
npm start

Your React app should now be running and accessible at http://localhost:3000. It is already configured to proxy API requests to your backend at http://localhost:5001.

NPM (comes with Node.js)

MongoDB Atlas account (or a local MongoDB instance)
