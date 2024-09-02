**eCommerce MERN App**
This eCommerce web application is built using the MERN (MongoDB, Express, React, Node.js) stack. The project includes backend and frontend development, user authentication, an admin panel, product management, filters, and a shopping cart.

**Features**
User Registration and Login with JWT Authentication
Admin and User Panels
Category and Product Management (CRUD)
Product Filters and Pagination
Shopping Cart and Checkout
Order Management (Admin and User)
Responsive Design

**Backend**
Server Setup
The server is built using Node.js and Express. It handles the API requests and interacts with the MongoDB database.

**Database Connection**
The MongoDB connection is established using Mongoose, and environment variables are managed using the dotenv package.

**User Authentication**
User registration, login, and JWT-based authentication have been implemented. The backend uses bcrypt for password hashing and protects certain routes with middleware.

**Category and Product Management**
The admin can create, update, and delete categories and products. Image uploads are handled as part of the product creation process.

**Frontend**
React Setup
The front end is built with React. It includes components for various pages and uses React Router to navigate between them.

**Admin Panel**
The admin panel includes features for managing categories, products, and orders. It provides CRUD operations for both categories and products.

**Shopping Cart**
The shopping cart allows users to add, update, and remove products. Users can view their order history, and admins can manage order statuses.
