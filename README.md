
# Express.js Server Side Framework Assignment

This project is a simple Express.js server application designed for learning and practicing server-side development using Node.js and Express. It demonstrates RESTful API design, middleware usage, error handling, and basic CRUD operations for a products resource.

## Features
- Express.js server setup
- Products API with CRUD operations
- Modular route handling
- Custom error handling middleware
- Authentication and validation middleware
- MongoDB integration for data persistence

## Project Structure
```
├── server.js                # Main server entry point
├── package.json             # Project dependencies and scripts
├── config/
│   └── db.js                # Database connection setup
├── errors/
│   ├── NotFoundErrors.js    # Custom 404 error class
│   └── ValidationErrors.js  # Custom validation error class
├── midddleware/
│   ├── auth.js              # Authentication middleware
│   ├── ErrorHandler.js      # Error handling middleware
│   ├── logger.js            # Request logging middleware
│   └── validation.js        # Request validation middleware
├── models/
│   └── products.js          # Mongoose product model
├── routes/
│   └── productsRoutes.js    # Product routes
├── README.md                # Project documentation
└── Week2-Assignment.md      # Assignment instructions
```

## Getting Started

### Prerequisites
- Node.js (v14 or higher recommended)
- npm
- MongoDB (local or cloud instance)

### Installation
1. Clone the repository:
   ```powershell
   git clone <repo-url>
   cd express-js-server-side-framework-Aso-Uduma
   ```
2. Install dependencies:
   ```powershell
   npm install
   ```
3. Configure MongoDB connection in `config/db.js` if needed.

### Running the Server
```powershell
npm start
```
The server will start on the port specified in your environment or default to 3000.

## API Endpoints
- `GET /api/products` - List all products
- `GET /api/products/:id` - Get a product by ID
- `POST /api/products` - Create a new product
- `PUT /api/products/:id` - Update a product
- `DELETE /api/products/:id` - Delete a product

## Middleware
- **auth.js**: Protects routes with authentication logic
- **validation.js**: Validates incoming requests
- **ErrorHandler.js**: Handles errors and sends appropriate responses
- **logger.js**: Logs incoming requests

## Error Handling
Custom error classes and middleware are used to handle validation and not found errors, providing clear responses to the client.

## License
This project is for educational purposes.

## Author
Aso Uduma