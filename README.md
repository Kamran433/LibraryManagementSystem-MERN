# Library Management System (MERN App)

Welcome to the Library Management System! This project is a complete MERN (MongoDB, Express.js, React.js, Node.js) stack application designed to handle library operations such as managing books, user authentication, and borrowing transactions.

## Features

- User Registration and Authentication
- CRUD Operations for Books
- Borrowing and Returning Books
- Admin Operations for Managing Users and Books
- JWT-based Authentication
- CORS Support
- Secure Password Hashing with bcrypt
- Middleware for Error Handling

## Getting Started

### Prerequisites

Ensure you have the following installed on your system:

- Node.js
- MongoDB

### Installation

1. **Clone the repository:**

```bash
git clone https://github.com/yourusername/library-management-system.git
cd library-management-system
```

2. **Install the dependencies:**

```bash
npm install
```

3. **Set up environment variables:**

Create a `.env` file in the root of your project and add the following:

```env
MONGO_URL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
FRONTEND=your_frontend_url
PORT=your_desired_port
```

### Running the Application

1. **Start the MongoDB server:**

Make sure your MongoDB server is running. If you have MongoDB installed locally, you can start it using:

```bash
mongod
```

2. **Start the application:**

```bash
npm start
```

Your server should now be running on the port specified in your `.env` file (default is 3000).

## API Endpoints

### User Authentication

- **Register a new user**

  ```http
  POST /api/register
  ```

- **Login**

  ```http
  POST /api/login
  ```

- **Get user data**

  ```http
  POST /api/userData
  ```

- **Get all users**

  ```http
  GET /api/getAllUser
  ```

### Book Management

- **Get all books**

  ```http
  GET /api/getAllBooks
  ```

- **Add a new book**

  ```http
  POST /api/add-book
  ```

- **Delete a book**

  ```http
  DELETE /api/delete-book/:id
  ```

- **Get a single book**

  ```http
  GET /api/get-singlebook/:id
  ```

- **Update a book**

  ```http
  PUT /api/updatebook/:id
  ```

### Borrowing Books

- **Borrow a book**

  ```http
  POST /api/add-borrowbook
  ```

- **Get all borrowed books**

  ```http
  GET /api/getAllBorrowedBooks
  ```

- **Delete a borrowed book**

  ```http
  DELETE /api/delete-borrowedbook/:id
  ```

- **Get a single borrowed book**

  ```http
  GET /api/get-singleborrowedbook/:id
  ```

- **Update a borrowed book**

  ```http
  PUT /api/updateborrowedbook/:id
  ```

### Testing API Joining

- **Add an author**

  ```http
  POST /api/author
  ```

- **Add a book with author**

  ```http
  POST /api/book
  ```

- **Populate author with books**

  ```http
  POST /api/authorbookpopulate
  ```

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

