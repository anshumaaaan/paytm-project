# Digital Wallet and Peer-to-Peer Payment Application

## Introduction

This is a comprehensive, full-stack digital wallet application, inspired by popular peer-to-peer payment platforms. Built entirely on the **MERN stack (MongoDB, Express, React, Node.js)**, the project is engineered to handle secure user authentication and ensure reliable, atomic financial transactions. The primary goal was to architect a robust system that delivers a smooth user experience while upholding strict standards for data integrity and security across the entire application lifecycle.

-----

## Key Features

The application is designed around core financial service functionalities, prioritizing security and user experience:

  * **Secure User Authentication:** Implemented using **JSON Web Tokens (JWT)** for secure, stateless session management, protecting sensitive application endpoints.

  * **Atomic Transaction Processing:** Leverages **Mongoose Sessions** on the backend to guarantee that all fund transfer operations are atomic. This ensures transactions either complete successfully or fail completely, rigorously adhering to ACID properties (Atomicity, Consistency, Isolation, Durability).

  * **Real-Time Balance Updates:** Utilizes efficient **React state management** to provide immediate, real-time feedback and balance updates to the user following any action or transaction.

  * **Modern and Responsive UI:** The frontend, developed with React and styled using **Tailwind CSS**, offers a utility-first, modern, and highly responsive interface optimized for all device sizes.

  * **Data Validation:** Integrates **Zod** for robust schema validation, securing data integrity for all inputs processed between the frontend and backend.

-----

## Technologies Used

This project utilizes a modern MERN stack architecture, detailed below:

### Frontend

| Technology | Purpose |
| :--- | :--- |
| **React.js (with Vite)** | Core library for building the dynamic user interface. Vite is used for an optimized development environment and fast build times. |
| **Tailwind CSS** | A utility-first CSS framework for rapid UI development and ensuring responsive design. |
| **Axios** | A promise-based HTTP client used for making clean, reliable API requests to the Express server. |

### Backend

| Technology | Purpose |
| :--- | :--- |
| **Node.js & Express.js** | Forms the server backbone, providing a scalable and robust framework for API development. |
| **MongoDB (with Mongoose)** | NoSQL database used for flexible data storage, with Mongoose providing structured schema modeling and interaction. |
| **JWT (JSON Web Tokens)** | Standard mechanism for securing API routes and managing authorized user sessions. |
| **Zod** | Essential library for input and output schema validation, enhancing API security and type safety. |

-----

## Screenshots

| Authentication Pages | Application Dashboard |
| :---: | :---: |
| \![Sign up and Sign in pages] | \![Dashboard and Send money page] |

-----

## Getting Started

To set up and run the digital wallet application locally, follow the instructions below.

### Prerequisites

Ensure the following software is installed on your system:

  * **Node.js** (v14 or higher)
  * **MongoDB** (Local instance or cloud connection details)

### Clone the Repository

Clone the project repository to your local machine:

```bash
git clone [https://github.com/syedahmedullah14/PayTM-Project.git](https://github.com/syedahmedullah14/PayTM-Project.git)
cd PayTM-Project
```

### Backend Setup

1.  Navigate to the backend directory:

    ```bash
    cd backend
    ```

2.  Install required Node dependencies:

    ```bash
    npm install
    ```

3.  Configure Environment Variables: Create a **`.env`** file in the `backend` directory and add the following required variables:

    ```env
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_secure_authentication_secret
    ```

4.  Start the server:

    ```bash
    npm start
    ```

The backend API will now be running.

### Frontend Setup

1.  Navigate to the frontend directory:

    ```bash
    cd ../frontend
    ```

2.  Install required React dependencies:

    ```bash
    npm install
    ```

3.  Start the development server using Vite:

    ```bash
    npm run dev
    ```

The application will typically be accessible in your browser at `http://localhost:5173`.
