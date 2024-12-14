
# Apni Dukaan

This is a full-fledged E-commerce website built using the MERN (MongoDB, Express.js, React, and Node.js) stack. The purpose of this project is to create an efficient and user-friendly web application that enables customers to browse, search, and purchase products. It also provides sellers with the ability to list their products, manage inventory, and process orders. The application integrates both frontend and backend features into a cohesive platform.

## Table of Contents

- [Project Overview](#project-overview)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Configuration](#configuration)
- [API Documentation](#api-documentation)
  - [API Endpoints](#api-endpoints)
- [Technologies](#technologies)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Project Overview

**Key Features:**

1. **User Authentication:** 
   - Users can create accounts, log in, and maintain personalized profiles.
   - Supports Google SignUp/In for easy authentication.
   - Users can track their order history, view, and update their profiles.

2. **Product Catalog:**
   - Comprehensive product catalog organized into categories and subcategories.
   - Users can browse items, apply filters (e.g., price range), and sort with pagination support.
   - Detailed product descriptions and photos.

3. **Shopping Cart:**
   - Add products to a shopping cart, view contents, adjust quantities, and proceed to checkout.

4. **Secure Payment Processing:**
   - Integration with secure payment gateways, such as Braintree, for seamless transactions.
   - Payment options include credit/debit cards, digital wallets, and cash-on-delivery.

5. **Search Functionality:**
   - Advanced search with filters and sorting for accurate results.

6. **Admin Dashboard:**
   - Tools for managing products, inventory, user accounts, and order processing.
   - Insights through analytics and sales reports.

7. **Order Tracking:**
   - Customers can track the status of their orders, view shipping details, and receive notifications.

8. **Responsive Design:**
   - Fully responsive UI accessible on desktops, tablets, and smartphones.

## Prerequisites

Ensure the following dependencies and tools are installed:

- **Frontend Prerequisites:**
  - React.js
  - Google OAuth

- **Backend Prerequisites:**
  - Node.js
  - npm or yarn
  - MongoDB
  - Cloudinary
  - Braintree

## Getting Started

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/Apni-Dukaan
   cd Apni-Dukaan
   ```

2. Install dependencies for both frontend and backend:
   ```bash
   cd frontend
   npm install
   cd ../backend
   npm install
   ```

### Configuration

1. Create an `.env` file in both the frontend and backend directories and configure the required environment variables.

   **Frontend:**
   ```env
   PORT=3000
   Google_Client_ID=************
   Base_Url=**********
   ```

   **Backend:**
   ```env
   PORT=8000
   MONGO_URL=************
   JWT_SECRET=************
   CLOUD_NAME=************
   API_KEY=************
   API_SECRET=************
   MERCHANT_ID=************
   PUBLIC_KEY=************
   PRIVATE_KEY=************
   ```

2. Start the backend server:
   ```bash
   cd backend
   nodemon index.js
   ```

3. Start the frontend application:
   ```bash
   cd frontend
   npm start
   ```

## API Documentation

### API Endpoints

#### **Auth**
- **POST /auth/login** - Log in using username and password.
- **POST /auth/register** - Register a new user.
- **POST /auth/forgot-password** - Reset password.
- **GET /auth/user-auth** - Verify user authentication.
- **GET /auth/admin-auth** - Verify admin authentication.

#### **Category**
- **POST /category/create-category** - Create a new category.
- **PUT /category/update-category/:id** - Update an existing category.
- **GET /category/get-category** - Fetch all categories.
- **DELETE /category/delete-category/:id** - Delete a category.

#### **Product**
- **POST /product/create-product** - Add a new product.
- **GET /product/get-category** - Fetch all products.
- **POST /product/filter-product** - Filter products based on criteria.
- **GET /product/category-product/:slug** - Fetch products by category.

## Technologies

- **React.js** (Frontend)
- **Node.js**, **Express.js**, **MongoDB** (Backend)
- **Google OAuth** (Authentication)
- **Cloudinary** (Image storage)
- **Braintree** (Payment processing)

## Contributing

You can contribute by adding new features, such as a ratings and reviews section.

## License

This project is licensed under the **MIT License**.

## Contact

Feel free to reach out via LinkedIn: [Rajesh Jha](https://www.linkedin.com/in/rajesh-jha-0aa47a205/).
