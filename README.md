# 🔐 Express REST API Client – Secrets API Integration

This project is a **Node.js + Express.js** web application that interacts with the [Secrets API](https://secrets-api.appbrewery.com) using RESTful methods (`GET`, `POST`, `PUT`, `PATCH`, and `DELETE`). It features a clean frontend built with **EJS templating** and styled HTML forms, allowing users to perform and visualize API actions from a browser.

---

## ⚙️ Tech Stack

- **Node.js**
- **Express.js**
- **Axios**
- **EJS**
- **body-parser**

---

## 🚀 How to Run the App Locally

Follow these steps to get the application up and running on your local machine:

### 1. Clone the repository

git clone https://github.com/goyalrohit03/express-rest-api-crud.git
cd express-rest-api-crud

### **2. Install dependencies**
npm install

### **3. Add your Bearer Token**
Open the index.js file and replace the placeholder with your actual token:
const yourBearerToken = "your-token-here";

### **4. Run the development server**
node index.js

### 5. Open in your browser
visit : http://localhost:3000

### **🔑 How to Generate API Token** 
To access the Secrets API, you need a Bearer Token: 
- Visit: https://secrets-api.appbrewery.com
- Click on **"Get your Bearer Token"** 
- Sign in using your email
- Copy the token provided
- Paste it into your `index.js` file like this: ```js const yourBearerToken = "your-token-here";

### **📋 How to Use the App** 
Each button on the form corresponds to a specific API operation. Here's how to use them: --- 
#### **GET Secret** 
- Fill in the **ID** field
- - Click the **GET** button
  - - Retrieves the secret with that ID ---
#### **POST Secret** 
- Fill in **Secret**, **Score**, and **Route**
- Click the **POST** button
- Adds a new secret to the database ---
#### **PUT Secret** 
- Fill in **ID**, **Secret**, **Score**, and **Route**
- Click the **PUT** button - Completely replaces the existing secret with new data ---
#### **PATCH Secret** 
- Fill in **ID** and any field(s) you want to update
- Click the **PATCH** button - Updates only the specified fields ---
#### **DELETE Secret** 
- Fill in the **ID** field
- Click the **DELETE** button - Deletes the secret with that ID 
