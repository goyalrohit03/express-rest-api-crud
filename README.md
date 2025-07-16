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

### **1. Clone the repository**

```bash
git clone https://github.com/goyalrohit03/express-rest-api-crud.git
cd express-rest-api-crud

2. Install dependencies
bash
Copy
Edit
npm install
3. Add your Bearer Token
Open the index.js file and replace the placeholder with your actual token:

js
Copy
Edit
const yourBearerToken = "your-token-here";
👉 Don’t have a token yet? See how to get one

4. Run the development server
bash
Copy
Edit
node index.js
5. Open in your browser
Visit: http://localhost:3000

You will see a form with buttons for each REST operation: GET, POST, PUT, PATCH, DELETE.

🔑 How to Generate API Token
To access the Secrets API, you need a Bearer Token:

Go to https://secrets-api.appbrewery.com

Click on "Get your Bearer Token"

Sign in using your email

Copy the token provided

Paste it into your index.js:

js
Copy
Edit
const yourBearerToken = "paste-your-token-here";
📋 How to Use the App
Each button on the web form maps to a specific API operation. Here's how to use each:

GET Secret
Fill in the ID field

Click the GET button

Retrieves the secret with that ID

POST Secret
Fill in Secret, Score, and Route

Click the POST button

Adds a new secret to the database

PUT Secret
Fill in ID, Secret, Score, and Route

Click the PUT button

Completely replaces the existing secret with new data

PATCH Secret
Fill in ID and any fields you want to update

Click the PATCH button

Updates only specified fields of the secret

DELETE Secret
Fill in the ID field

Click the DELETE button

Deletes the secret with that ID

🗂️ Project Structure
bash
Copy
Edit
express-rest-api-crud/
├── index.js           # Main server file
├── package.json       # Project metadata and dependencies
├── views/
│   └── index.ejs      # HTML form rendered using EJS
├── .gitignore         # Excludes node_modules, env files, etc.
📌 Best Practices
Use a .gitignore file to exclude node_modules/ and any sensitive config like .env

Format API responses using JSON.stringify(result.data, null, 2) for better readability

Consider using dotenv for managing sensitive keys securely

