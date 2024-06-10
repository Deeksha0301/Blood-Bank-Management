# Blood Bank Management Sysytem

---

## Introduction

Welcome to the Blood Bank Management System project repository! This project aims to provide a comprehensive solution for managing blood donations, inventory, and donor records. It facilitates seamless interaction between donors, hospitals, and organizations involved in blood donation activities.

---


## Features

### User Management
- **User Authentication:** Secure user registration and login using JWT tokens.
- **Role-based Access Control:** Different access levels for admin, organization, donor, and hospital users.

### Inventory Management
- **Blood Inventory:** Track blood units by type (O+, O-, AB+, AB-, etc.), manage incoming and outgoing transactions.
- **Real-time Updates:** Monitor available blood quantities and generate reports.

### Donor and Hospital Management
- **Donor Records:** Maintain donor profiles, track donation history.
- **Hospital Records:** Manage hospital information and blood requests.

### Analytics and Reporting
- **Blood Group Analytics:** Calculate and display statistics on blood group availability.
- **Transaction Logs:** Audit logs for inventory transactions and user activities.

### Frontend Interface
- **Dashboard:** Interactive dashboard for visualizing inventory status and donor/hospital information.
- **Forms and Validation:** User-friendly forms with validation for data entry and updates.

---

## Objective
The primary objective of this project is to enhance the blood donation process by providing a seamless user experience and efficient blood inventory management for blood banks and donors. 






---

## Technologies Used

### Backend
- **Node.js:** Server-side runtime environment.
- **Express.js:** Web application framework for Node.js.
- **MongoDB:** NoSQL database for storing application data.
- **Mongoose:** MongoDB object modeling tool.
- **JWT (JSON Web Tokens):** For secure authentication and authorization.
- **bcrypt.js:** Library for hashing passwords securely.
- **Morgan:** HTTP request logger middleware.
- **Cors:** Cross-Origin Resource Sharing middleware.

### Frontend
- **React:** JavaScript library for building user interfaces.
- **Redux:** State management for React applications.
- **React Router:** Declarative routing for React applications.
- **Axios:** Promise-based HTTP client for making API requests.
- **Material-UI:** React UI framework for faster and easier web development.
- **Chart.js:** Simple yet flexible JavaScript charting library.

### Development Tools
- **Visual Studio Code:** Integrated development environment (IDE).
- **Postman:** API development and testing tool.
- **Git:** Version control system for tracking changes in the codebase.
- **GitHub:** Hosting platform for software development and version control.

---

## Setup Instructions

### Prerequisites
- Node.js installed on your local machine.
- MongoDB installed and running locally or a cloud MongoDB instance.
- Environment variables for JWT secret and MongoDB connection string.

### Backend Setup
1. Clone the repository:
   ```
   git clone https://github.com/Deeksha0301/Blood-Bank-Management.git
   ```
2. Navigate to the backend directory:
   ```
   cd blood-bank-management-system/server
   ```
 
3. Install dependencies:
   ```
   npm install
   ```
4. Set up environment variables:
   - Create a `.env` file in the `backend` directory.
   - Define variables:
     ```
     PORT=8080
     JWT_SECRET=your_jwt_secret
     MONGODB_URI=your_mongodb_connection_string
     ```
5. Run the backend server:
   ```
   npm start
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```
   cd ../client
   ```
2. Install dependencies:
   ```
   npm install
   ```
3. Start the React development server:
   ```
   npm start
   ```

4. Access the application in your browser at `http://localhost:3000`.

---

## Backend Details

The backend is built using Node.js and Express.js, providing RESTful APIs for managing users, blood inventory, donors, hospitals, and organizations. MongoDB is used as the database with Mongoose as the ODM (Object Data Modeling).

### Folder Structure
- **`/controllers`**: Contains controller functions for handling business logic.
- **`/middlewares`**: Custom middleware functions for authentication and authorization.
- **`/models`**: Mongoose schemas defining database models.
- **`/routes`**: Express router definitions for different API endpoints.
- **`/utils`**: Utility functions and helper modules.

### API Endpoints
- `/api/auth`: User authentication and registration.
- `/api/inventory`: Blood inventory management (CRUD operations).
- `/api/analytics`: Endpoint for generating blood group analytics.
- `/api/admin`: Admin-only endpoints for managing users and system data.

---

## Frontend Details

The frontend is developed using React, Redux for state management, and Material-UI for UI components. It provides an intuitive user interface for interacting with the backend APIs.

### Folder Structure
- **`/src/components`**: Reusable React components.
- **`/src/pages`**: Individual pages/components for different sections of the application.
- **`/src/redux`**: Redux store configuration, actions, and reducers.
- **`/src/services`**: Axios service for API requests.
- **`/src/utils`**: Utility functions and helper modules.

### Components
- **Dashboard**: Main dashboard displaying blood inventory statistics and analytics.
- **Forms**: Forms for user authentication, blood donation entries, and hospital requests.
- **Charts**: Interactive charts for visualizing blood group data and transaction logs.

---

## API Documentation

For detailed API documentation, including endpoint descriptions, request/response formats, and usage examples, refer to the [API Documentation](./API_DOCUMENTATION.md) file.

---

## Screenshots

![Dashboard](./screenshots/dashboard.png)
*Dashboard displaying blood inventory and analytics.*

![Login Page](./screenshots/login.png)
*Login page with user authentication.*

---

## Live Link
https://blood-bank-management-8rfk.vercel.app/login

---

## Future Improvements

- Implement email notifications for donor alerts and critical inventory levels.
- Enhance frontend with additional data visualizations and responsive design.
- Integrate automated testing for backend APIs using Jest or Mocha.




