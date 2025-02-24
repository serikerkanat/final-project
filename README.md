# Blue Giants

## Project Name
Blue Giants

## Project Description
Blue Giants is an educational platform designed to provide information about whales, the largest and most majestic creatures of the ocean. This project features a backend system that stores whale data in MongoDB and a frontend interface where users can explore and interact with this information.

## Purpose
The project aims to raise awareness about whales, their characteristics, and their importance in marine ecosystems.

## What It Does
- **Add Whale Information:** Allows users to add information about different whale species, such as their name and description.
- **Display Whales:** Displays a list of stored whales in an interactive and visually appealing table on the website.
- **User-Friendly Interface:** Provides a simple and intuitive interface to explore whale-related information.

## Target Audience
- Marine life enthusiasts and conservationists.
- Students and educators seeking resources on marine biology.
- Developers looking to understand full-stack development with Node.js and MongoDB.

## Team Members
- Amir Zhunussov

## Screenshot
**Blue Giants Preview**

## Getting Started

### Prerequisites
- **Node.js:** Install Node.js (version 16 or higher). [Download here](https://nodejs.org/)
- **MongoDB:** Install MongoDB Community Edition or use MongoDB Atlas for cloud hosting. [Download here](https://www.mongodb.com/try/download/community)
- **Postman:** For testing API endpoints. [Download here](https://www.postman.com/downloads/)

### Installation Steps

#### Backend Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/blue-giants.git
   cd blue-giants
   ```
2. **Install dependencies:**
   ```bash
   npm install
   ```
3. **Create a `.env` file** in the root directory and add your environment variables:
   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   PORT=3000
   ```
4. **Run the backend server:**
   ```bash
   npm start
   ```
   Ensure the server is running on the specified port (default: 3000).

#### Frontend Setup
1. **Navigate to the frontend folder:**
   ```bash
   cd frontend
   ```
2. **Open the `index.html` file** in your browser or use a local server (e.g., Live Server in VS Code).

## Tools and Resources
- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Compass for local testing, Atlas for cloud hosting)
- **Frontend:** HTML, CSS, JavaScript
- **API Testing:** Postman
- **Code Editor:** Visual Studio Code

## API Documentation

### Endpoints

#### 1. Get All Whales
- **Method:** GET
- **URL:** `/api/whales`
- **Description:** Retrieve a list of all whales.
- **Response:**
  ```json
  [
    {
      "_id": "64f1b2c7e4b0d8a9c8f1b2c7",
      "name": "Blue Whale",
      "description": "The largest animal on Earth."
    }
  ]
  ```

#### 2. Add a New Whale
- **Method:** POST
- **URL:** `/api/whales`
- **Description:** Add a new whale to the database.
- **Request Body:**
  ```json
  {
    "name": "Humpback Whale",
    "description": "Known for their complex songs."
  }
  ```
- **Response:**
  ```json
  {
    "_id": "64f1b2c7e4b0d8a9c8f1b2c8",
    "name": "Humpback Whale",
    "description": "Known for their complex songs."
  }
  ```

#### 3. Get a Single Whale
- **Method:** GET
- **URL:** `/api/whales/:id`
- **Description:** Retrieve details of a specific whale by ID.
- **Response:**
  ```json
  {
    "_id": "64f1b2c7e4b0d8a9c8f1b2c7",
    "name": "Blue Whale",
    "description": "The largest animal on Earth."
  }
  ```

#### 4. Update a Whale
- **Method:** PUT
- **URL:** `/api/whales/:id`
- **Description:** Update details of a specific whale by ID.
- **Request Body:**
  ```json
  {
    "name": "Blue Whale",
    "description": "The largest animal on Earth, found in all oceans."
  }
  ```
- **Response:**
  ```json
  {
    "_id": "64f1b2c7e4b0d8a9c8f1b2c7",
    "name": "Blue Whale",
    "description": "The largest animal on Earth, found in all oceans."
  }
  ```

#### 5. Delete a Whale
- **Method:** DELETE
- **URL:** `/api/whales/:id`
- **Description:** Delete a specific whale by ID.
- **Response:**
  ```json
  {
    "message": "Whale deleted successfully."
  }
  ```

## Dependencies
- **express:** Fast, unopinionated, minimalist web framework for Node.js.
- **mongoose:** MongoDB object modeling for Node.js.
- **dotenv:** Loads environment variables from a `.env` file.
- **bcryptjs:** For hashing passwords.
- **jsonwebtoken:** For generating and verifying JSON Web Tokens (JWT).
- **cors:** Middleware for enabling CORS.
- **joi:** Schema description language and data validator for JavaScript.
- **cookie-parser:** Parse Cookie header and populate `req.cookies`.
```
