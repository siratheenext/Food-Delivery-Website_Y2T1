[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/OspoeYOK)

# Food Delivery Website: ChickNext's Ken

This repository contains a full-stack web application for "ChickNext's Ken," a conceptual Korean fried chicken restaurant. This project was developed as part of the **ITDS242: Web Technologies Lab** course at Mahidol University.

The application provides a user-facing website for browsing the menu and an admin dashboard for managing products and users, secured with Google reCAPTCHA.

---

## Key Features

### Customer-Facing
* **Home Page:** Features a promotional carousel and highlights key menu items.
* **Menu & Categories:** Browse all products, filterable by categories (Chicken, Snacks, Drinks, Toppings).
* **Search:** A dedicated search page with advanced filters for price, promotion status, and type.
* **Product Details:** View detailed information for each menu item.
* **About Us:** A team page listing the project members and contact information.

### Admin Dashboard
* **Secure Login:** Admin login page is protected by Google reCAPTCHA and requires admin credentials.
* **Session Management:** Uses cookies to maintain admin login sessions.
* **Product Management (CRUD):** Full capabilities to add, view, update, and delete menu items (products).
* **Admin Management (CRUD):** Full capabilities to add, view, update, and delete admin accounts.

---

## Technologies Used

* **Frontend:** HTML, CSS, JavaScript
* **Backend:** Node.js, Express.js
* **Database:** MySQL
* **Node.js Libraries:**
    * `express`
    * `mysql2`
    * `body-parser`
    * `cookie-parser`
    * `cors`
    * `dotenv`
    * `fs`
    * `multer` (for image uploads)
    * `nodemon` (for development)
* **Web Services:** Google reCAPTCHA v2

---

## Setup and Installation

To run this project locally, please follow these steps.

### 1. Folder Structure

Ensure the project directory is organized as follows:

### 2. Database Setup (MySQL)

1.  Import the `sec2_gr8_database.sql` file into your MySQL server. This will create the `chicknext` database and populate initial data.
2.  Create a new user account in MySQL with the following credentials:
    * **Username:** `itds242`
    * **Host:** `localhost`
    * **Password:** `ict555!!!`
3.  Grant privileges to this new user:
    * Go to **User and Privileges**.
    * Select the `itds242` user.
    * Go to the **Schema Privileges** tab.
    * Click **Add Entry**.
    * Select **Selected schema** and choose `chicknext`.
    * Grant all **Object Rights** (SELECT, INSERT, UPDATE, DELETE, etc.).

### 3. Backend (API) Setup

1.  Navigate to the backend directory:
    ```bash
    cd Project_Sec2_gr8/Sec2_gr8_ws_src/back
    ```
2.  Initialize the project and install dependencies:
    ```bash
    npm init
    # When prompted, set the entry point to: back.js
    npm install body-parser cookie-parser cors dotenv express fs multer mysql2 nodemon
    ```
3.  Open the `package.json` file and in the `scripts` section, add:
    ```json
    "scripts": {
      "start": "nodemon back.js"
    }
    ```
4.  Start the backend server (leave this terminal running):
    ```bash
    npm start
    ```

### 4. Frontend (Client) Setup

1.  Open a **new terminal** and navigate to the frontend directory:
    ```bash
    cd Project_Sec2_gr8/Sec2_gr8_ws_src/front
    ```
2.  Initialize the project and install dependencies (same as backend):
    ```bash
    npm init
    # When prompted, set the entry point to: front.js
    npm install body-parser cookie-parser cors dotenv express fs multer mysql2 nodemon
    ```
3.  Open the `package.json` file and in the `scripts` section, add:
    ```json
    "scripts": {
      "start": "nodemon front.js"
    }
    ```
4.  Start the frontend server (leave this terminal running):
    ```bash
    npm start
    ```

### 5. Access the Application

Once both servers are running, you can access the website at:
**[http://localhost:3030](http://localhost:3030)**

---

## Team Members

* **Thanyarat Wuthiroongreungsakul**
* **Kemisara Anankamongkol**
* **Chawanwit Khuanphatkul**
* **Sirathee Klinbua**

