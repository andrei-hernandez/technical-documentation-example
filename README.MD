# Product Management Service

## Introduction
The Product Management Service is a TypeScript-based service that provides endpoints for creating, updating, deleting, and retrieving products. It is designed to be easy to integrate into existing applications and provides a simple yet powerful interface for managing product data.

## Features
- Create new products
- Update existing products
- Delete products
- Retrieve product information

## Installation
To install the Product Management Service, follow these steps:
1. Clone the repository: `git clone <repository-url>`
2. Install dependencies: `npm install`
3. Build the project: `npm run build`

## Usage
Once the service is installed, you can start it by running `npm start`. By default, the service will listen on port 3000.

### Endpoints

#### Create a Product
```
POST /products
Body:
{
  "name": "Product Name",
  "price": 19.99,
  "description": "Product Description"
}
```

#### Update a Product
```
PUT /products/:id
Body:
{
  "name": "New Product Name",
  "price": 29.99,
  "description": "New Product Description"
}
```

#### Delete a Product
```
DELETE /products/:id
```

#### Get a Product
```
GET /products/:id
```

#### Get All Products
```
GET /products
```

## Dependencies
- Express.js
- TypeScript
- Mongoose (for database interaction)

## Configuration
The service can be configured using environment variables. Available configurations include:
- `PORT`: The port on which the service should listen (default: 3000)
- `MONGODB_URI`: The URI of the MongoDB database (required for database interaction)

## Contributing
Contributions to the Product Management Service are welcome! To contribute, fork the repository, make your changes, and submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
