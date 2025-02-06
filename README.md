# E-Commerce Application

This repository contains both the **frontend** and **backend** for an e-commerce application built using **React.js**, **Node.js**, **Express.js**, and **MongoDB**.

## Cloning the Repository

To get started, clone this repository using:

```sh
git clone https://github.com/your-repo/e-commerce-app.git
cd e-commerce-app
```

## Features

- User authentication using JWT
- Product management (add, list, and remove products)
- File upload support using Multer
- Cross-Origin Resource Sharing (CORS) enabled
- Responsive UI with a navigation system

## Installation

### Backend Setup

1. Navigate to the backend directory:

   ```sh
   cd backend
   ```

2. Install dependencies:

   ```sh
   npm install
   ```

3. Set up environment variables:

   - Create a `.env` file in the backend directory and add:
     ```sh
     PORT=4000
     MONGO_URI=your_mongodb_connection_string
     JWT_SECRET=your_secret_key
     ```

4. Start the backend:
   ```sh
   npm start
   ```
   The backend will run on `http://localhost:4000/`.

### Frontend Setup

1. Navigate to the frontend directory:

   ```sh
   cd frontend
   ```

2. Install dependencies:

   ```sh
   npm install
   ```

3. Set up environment variables:

   - Create a `.env` file in the frontend directory and add:
     ```sh
     REACT_APP_BACKEND_URL=your_backend_url
     ```

4. Start the frontend:
   ```sh
   npm start
   ```
   The frontend will run on `http://localhost:3000/`.

## API Endpoints

### Authentication

- **POST** `/api/auth/register` - Register a new user
- **POST** `/api/auth/login` - Login and receive a JWT token

### Products

- **GET** `/api/products` - Fetch all products
- **POST** `/api/products` - Add a new product (Admin only)

### Orders

- **GET** `/api/orders` - Retrieve user orders
- **POST** `/api/orders` - Place a new order

## Frontend Components

### Navbar

- Located in `Navbar.jsx`, it contains the website logo and user profile section.

### Sidebar

- Located in `Sidebar.jsx`, it provides navigation to add products and list products.

### Add Product

- Located in `AddProduct.jsx`, allows users to upload product details and images.

### List Product

- Located in `ListProduct.jsx`, displays all available products with options to remove them.

### Footer

- Located in `Footer.jsx`, displays copyright information.

## Dependencies

### Backend

- **Express.js** - Web framework for Node.js
- **Mongoose** - MongoDB object modeling
- **jsonwebtoken** - Authentication using JWT
- **multer** - File upload handling
- **cors** - Cross-Origin Resource Sharing support

### Frontend

- **React.js** - Frontend library
- **React Router** - For navigation
- **CSS Modules** - Styling components

## Contributing

Feel free to submit issues and pull requests.
