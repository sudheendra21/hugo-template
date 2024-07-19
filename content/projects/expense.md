---
title: "Expense Tracker Web App"
date: 2023-07-19
draft: false
tags: ["web development", "react", "node.js", "mongodb"]
categories: ["projects"]
---

# Expense Tracker Web App

![Expense Tracker App Screenshot](/images/expense-tracker-screenshot.png)

## Overview
The Expense Tracker Web App is a full-stack application designed to help users track and manage their personal expenses. It provides an intuitive interface for recording expenses, categorizing them, and visualizing spending patterns through charts and graphs.

## Features
- User authentication and authorization
- Add, edit, and delete expense entries
- Categorize expenses into predefined categories
- View expenses by date range and category
- Interactive data visualization using charts and graphs
- Responsive design for seamless use across devices

## Technologies Used
- Front-end:
  - React: JavaScript library for building user interfaces
  - Redux: State management library for predictable state handling
  - Axios: Promise-based HTTP client for making API requests
  - Chart.js: JavaScript charting library for data visualization
- Back-end:
  - Node.js: JavaScript runtime for server-side development
  - Express: Web application framework for building RESTful APIs
  - MongoDB: NoSQL database for storing expense data
  - Mongoose: Object Data Modeling (ODM) library for MongoDB and Node.js
- Authentication:
  - JSON Web Tokens (JWT): Secure authentication mechanism for stateless communication
  - bcrypt: Library for hashing passwords before storing them in the database

## Project Structure
- `client`: Contains the front-end React application
  - `src/components`: Reusable UI components
  - `src/pages`: Individual pages of the application
  - `src/services`: API service for making HTTP requests to the back-end
  - `src/reducers`: Redux reducers for managing application state
- `server`: Contains the back-end Node.js application
  - `config`: Configuration files for the server
  - `controllers`: Request handlers for different API endpoints
  - `models`: Mongoose models for interacting with the database
  - `routes`: API routes for handling HTTP requests
- `database`: Contains scripts for initializing and seeding the MongoDB database

## Installation and Setup
1. Clone the repository:
   ```
   git clone https://github.com/johndoe/expense-tracker.git
   ```
2. Navigate to the project directory:
   ```
   cd expense-tracker
   ```
3. Install dependencies for the server:
   ```
   cd server
   npm install
   ```
4. Install dependencies for the client:
   ```
   cd ../client
   npm install
   ```
5. Set up the MongoDB database:
   - Install MongoDB on your system or use a cloud-based service like MongoDB Atlas
   - Update the database connection URL in `server/config/db.js`
6. Start the development server:
   ```
   cd ../server
   npm run dev
   ```
7. Start the client application:
   ```
   cd ../client
   npm start
   ```
8. Open your browser and visit `http://localhost:3000` to access the Expense Tracker Web App.

## Future Enhancements
- Implement data export functionality to download expense data as CSV or PDF
- Add support for multiple currencies and currency conversion
- Integrate with a receipt scanning API to automatically extract expense details from receipts
- Implement a budgeting feature to set monthly spending limits and track progress
- Enhance the data visualization with more advanced charts and insights

## Contributing
Contributions to the Expense Tracker Web App are welcome! If you find any bugs or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/johndoe/expense-tracker). If you'd like to contribute code, please fork the repository and submit a pull request with your changes.

## License
This project is licensed under the MIT License. See the [LICENSE](https://github.com/johndoe/expense-tracker/blob/main/LICENSE) file for more information.

## Contact
If you have any questions or inquiries about the Expense Tracker Web App, feel free to reach out:
- Email: john.doe@example.com
- LinkedIn: [linkedin.com/in/johndoe](https://www.linkedin.com/in/johndoe)
- GitHub: [github.com/johndoe](https://github.com/johndoe)