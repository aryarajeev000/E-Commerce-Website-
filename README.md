# E-Commerce Website
## Overview

This repository contains the source code for an E-Commerce website built with Node.js, Express, and MongoDB. The application allows users to browse products, place orders, and manage their profiles. Admins can manage products, categories, and order statuses. It includes a secure authentication system and a payment gateway integration.

Project Structure

### client/: Frontend code (not covered here).

### config/: Configuration files (e.g., database connection, environment variables).

### controllers/: Logic for handling requests and interacting with models.

### helpers/: Utility functions used throughout the app.

### middlewares/: Custom middleware (e.g., authentication, authorization).

### models/: MongoDB models defining the data structure.

### routes/: Express route definitions.

### server.js: Entry point for the application.

# Routes
## 1. Authentication Routes (authRoute.js)

This file contains routes for user authentication.

### POST /register: Registers a new user.

### POST /login: Logs in an existing user.

### POST /forgot-password: Initiates password recovery.

### GET /profile: Gets the current user's profile.

### GET /orders: Gets all orders placed by the logged-in user.

### GET /order/:id: Gets a single order by ID.

### PUT /update-profile: Updates the user's profile.

# 2. Category Routes (categoryRoutes.js)

This file contains routes for managing product categories.

### POST /create-category: Creates a new category (admin only).

### PUT /update-category/:id: Updates an existing category (admin only).

### DELETE /delete-category/:id: Deletes a category (admin only).

### GET /category/:slug: Fetches a category by its slug.

### GET /categories: Fetches all categories.

# 3. Product Routes (productRoutes.js)

This file contains routes for managing products.

### POST /create-product: Creates a new product (admin only).

### PUT /update-product/:id: Updates an existing product (admin only).

### DELETE /delete-product/:id: Deletes a product (admin only).

### GET /product/:slug: Fetches a product by its slug.

### GET /products: Fetches all products.

### GET /products/filters: Filters products based on criteria like category, price, etc.

Route and Model Relationship Diagram
          +------------+         +-------------+
          |  Category  |<------->|   Product   |
          +------------+         +-------------+
                ^                     ^
                |                     |
                +----------+  +-----------------+
                           |  |     Order       |
                +--------+ |  +-----------------+
                |  User   |<------------------+
                +--------+ |
                           |
                  +--------+----+
                  |   Auth Route |
                  +-------------+

## Middleware

requireSignIn: Ensures that the user is authenticated.

isAdmin: Ensures that the user has admin privileges.

## Setup and Installation

## Clone the repository:

git clone https://github.com/yourusername/e-commerce-website.git
cd e-commerce-website


Install dependencies:

### npm install


## Set up environment variables in a .env file (refer to .env.example for a template).

## Start the server:

## npm start


The application will be running on the specified port (usually localhost:5000).


## npm start


The application will be running on the specified port (usually localhost:5000).
