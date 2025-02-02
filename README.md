# Product API

## Overview
This is a simple **RESTful API** built with **Node.js**, **Express.js**, and **MongoDB** for managing product data. It allows users to perform CRUD (Create, Read, Update, Delete) operations on products.

## Features
- **Create a product** (POST `/api/products`)
- **Retrieve all products** (GET `/api/products`)
- **Retrieve a single product by ID** (GET `/api/products/:id`)
- **Update a product** (PUT `/api/products/:id`)
- **Delete a product** (DELETE `/api/products/:id`)

## Technologies Used
- **Node.js** - JavaScript runtime environment
- **Express.js** - Backend framework for handling API requests
- **MongoDB** - NoSQL database for storing product information
- **Mongoose** - ODM for interacting with MongoDB

## Project Structure
```
├── models
│   ├── product.model.js       # Mongoose schema for products
├── controllers
│   ├── product.controller.js  # Business logic for handling API requests
├── routes
│   ├── product.route.js       # API route definitions
├── index.js                   # Main server file
```

## Installation & Setup
### Prerequisites
Ensure you have the following installed:
- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)

### Steps
1. **Clone the repository**
   ```sh
   git clone <repository-url>
   cd <repository-folder>
   ```
2. **Install dependencies**
   ```sh
   npm install
   ```
3. **Start the server**
   ```sh
   npm start
   ```
   The server will run on `http://localhost:3000`.

## API Endpoints
| Method  | Endpoint              | Description              |
|---------|----------------------|--------------------------|
| GET     | `/api/products`       | Retrieve all products   |
| GET     | `/api/products/:id`   | Retrieve a single product by ID |
| POST    | `/api/products`       | Create a new product   |
| PUT     | `/api/products/:id`   | Update an existing product |
| DELETE  | `/api/products/:id`   | Delete a product |

## Database Connection
The project connects to a MongoDB instance via Mongoose. Update the **MongoDB URI** in `index.js` if needed:
```js
mongoose.connect("your-mongodb-uri")
```

## License
This project is open-source and available under the **MIT License**.

