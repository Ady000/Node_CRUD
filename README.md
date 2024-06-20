# Node_CRUD
Basic CRUD Operation in Node.js


# Node.js CRUD Application

This is a basic CRUD (Create, Read, Update, Delete) application built with Node.js, Express, and MongoDB. The application allows you to create, read, update, and delete items.

## Project Structure

```
node-crud/
│
├── models/
│   └── Item.js
│
├── routes/
│   └── items.js
│
├── config/
│   └── database.js
│
├── server.js
├── package.json
└── .gitignore
```

## Prerequisites

- Node.js and npm installed on your machine.
- MongoDB installed and running.

## Getting Started

1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/node-crud.git
   cd node-crud
   ```

2. **Install the dependencies:**
   ```sh
   npm install
   ```

3. **Set up environment variables:**
   Create a `.env` file in the root directory and add the following:
   ```env
   MONGO_URI=mongodb://localhost:27017/crudDB
   PORT=3000
   ```

4. **Run the server:**
   ```sh
   node server.js
   ```

5. **Use a tool like Postman to test the API endpoints:**
   - **Create**: `POST http://localhost:3000/items`
     ```json
     {
       "name": "Sample Item",
       "quantity": 10,
       "description": "This is a sample item."
     }
     ```
   - **Read all items**: `GET http://localhost:3000/items`
   - **Read a single item**: `GET http://localhost:3000/items/:id`
   - **Update**: `PUT http://localhost:3000/items/:id`
     ```json
     {
       "name": "Updated Item",
       "quantity": 5,
       "description": "This is an updated item."
     }
     ```
   - **Delete**: `DELETE http://localhost:3000/items/:id`

## Project Structure Details

- **`models/Item.js`**: Contains the Mongoose schema and model for items.
- **`routes/items.js`**: Defines the CRUD routes for the items.
- **`config/database.js`**: Handles the MongoDB connection.
- **`server.js`**: Sets up the Express server and uses the defined routes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request.

## Acknowledgements

- [Express](https://expressjs.com/)
- [Mongoose](https://mongoosejs.com/)
- [MongoDB](https://www.mongodb.com/)
- [dotenv](https://www.npmjs.com/package/dotenv)

```

Make sure to replace `https://github.com/your-username/node-crud.git` with the actual URL of your repository. This `README.md` file provides a clear and comprehensive guide for setting up and using your Node.js CRUD application.
