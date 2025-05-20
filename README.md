Food Order Application
This is a food ordering application with a React frontend and Node.js backend.
Setup Instructions
Backend Setup

Navigate to the backend directory:
cd backend

Install dependencies:
npm i

Configure your database:

Open database/db.js file
Modify the database connection settings:

javascriptfoodOrderDB = await mysql.createConnection({
  host: "localhost",
  user: "root",
  password: <your root password>,  // Change this to your MySQL root password
  database: <your database name>,  // Change this to your database name
});

Start the backend server:
npm run dev
The backend will start running on http://localhost:3000

Frontend Setup

Navigate to the frontend directory:
cd frontend

Install dependencies:
npm i

Create a .env file in the frontend root directory with the following content:
VITE_BASE_URL="http://localhost:3000/api"

Start the frontend development server:
npm run dev
The frontend application will be available at http://localhost:5173 (or another port if 5173 is already in use)

Running the Application

Make sure the backend server is running first
Then start the frontend server
Access the application through your browser at the URL displayed after starting the frontend

Features

Browse available food shops
View food items for each shop
Add items to cart
Place orders

Technologies Used

Frontend: React, TanStack Query, React Router
Backend: Node.js, Express
Database: MySQL
