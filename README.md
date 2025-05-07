# Capstone-Project-Step-2 🧁🍩🍰🥐
Full Bakery Website

1. Tech Stack
   
   * Frontend:
     * React – JavaScript library for building UIs
     * React Router – Handles navigation between pages
     * CSS – CSS framework for responsive, modern styling
     * Axios – For communicating with the backend API

   * Backend:
     * Node.js + Express.js – To build APIs and manage server side logic
   
   * Database:
     * MongoDB – NoSQL database for storing users, products, and orders

   * Content Management:
     * Adding/editing products
     * Viewing orders
     * Managing inventory

   * Hosting:
     * Netlify – Frontend deployment
     * Render – Backend deployment


2. Focus of the Project
   * This will be an full-stack website.
     * The goal is to create a fully functional e-commerce platform where both frontend and backend logic work to deliver a seamless experience for customers and admins.


3. Project Type
   * This project will be a responsive website for both desktop and mobile users.

4. Project Goal
   * The project is designed to work for a online bakery.
   Customers would be able to:
     * Browse bakery products like cakes, pastries, and bread
     * View item details such as: ingredients, price, availability
     * Add items to a cart and proceed to checkout
   
  * This website will offer a realistic e-commerce experience that mirrors the workflow of a small business bakery.


5. User Demographic
    * This website targets two main user groups:
     
     * Bakery Customers:
         * Bakery lovers who value convenience and artisanal products
         * Shoppers who support local or small businesses

     * Admin Users:
        * Bakery owners or staff who manage stock, products, and orders
        * Individuals responsible for product inventory, pricing, and orders


6. Data and API
    * The app will use a custom-built API that supports:
      * Products such as: name, image, description, price, category, tags, stock.
      * Users
      * Order: cart items, user info, payment status.
        
   * All data will be stored in MongoDB


7. Project Approach
   * Database Schema:
     * Users: id, name, email, password, role - 2 roles, admin role and costumer role
     * Products: id, name, description, price, stock, image
     * Orders: id, userId, items, totalPrice, pickupInfo, status
   
   * Development Plan:
     * Setup backend API (Node.js + MongoDB)
     * Database Setup: MongoDB for storing products, users, and orders.
     * Build product routes (GET, POST, PUT, DELETE)
     * Implement authentication and admin dashboard routes
     * Develop frontend with pages: Home, Shop, Product Detail, Cart, Checkout, Admin
     * Connect frontend to backend via Axios
     * Deploy frontend and backend separately

    * Potential API Issues:
       * Concurrency Issues: Ensuring stock is properly updated when two users attempt to buy the same product at the same time.
       * Error Handling: Returning appropriate error messages for common issues, such as invalid input or failed database operations.
       * Data Validation: Ensuring input data like product details is validated.
       * Scaling: As the user base and data grow, the application may require optimizations for speed and efficiency.

    * Sensitive Information:
       * User Authentication: Passwords must be hashed before storage using a library like bcrypt.
       * User Data: Email addresses, order history are sensitive and must be protected against unauthorized access.
       * Payment Information: Payment information must be processed securely through third-party services.
   
    * Functionality:
      * User Authentication:
        * Users can sign up, log in, and securely access their accounts.
        * Admins have specific routes for managing products and orders.
        
     * Product Management:
        * Users can browse products, view details, and add items to their cart.
        * Admin users can add, update, or delete products.
         
     * Shopping Cart & Checkout:
        * Users can view their cart, modify quantities, or remove items.
        * During checkout, users provide pickup details and confirm their order.
        
     * Order Management:
        * Admin users can view and update orders, changing their status.
        
     * Admin Dashboard:
        * Admin users can see an overview of orders and manage product inventory.

8. User Flow
   * Customer Flow:
     * Home Page: Customers land on the homepage and browse products.
     * Shop: Navigate to the shop page to view all products.
     * Product Detail: Click on a product to see its detailed description and add it to the cart.
     * Cart: Go to the cart page to review products and quantities.
     * Checkout: Enter pickup details and proceed to payment.
     * Order Confirmation: After checkout, the customer receives a summary of their order.
   
   * Admin Flow:
     * Admin Login: Admin logs into the admin dashboard.
     * Dashboard: View a list of orders and products, manage the store.
     * Product Management: Add, update, or delete products.
     * Order Management: View and update the status of customer orders.

    
         
