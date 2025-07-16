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

<pre lang="markdown"> ### **2. Install dependencies** ```bash npm install ``` --- ### **3. Add your Bearer Token** Open the `index.js` file and replace the placeholder with your actual token: ```js const yourBearerToken = "your-token-here"; ``` 👉 Don’t have a token yet? [See how to get one](#-how-to-generate-api-token) --- ### **4. Run the development server** ```bash node index.js ``` --- ### **5. Open in your browser** Visit: ```url http://localhost:3000 ``` You will see a web form with buttons for each REST operation: **GET**, **POST**, **PUT**, **PATCH**, and **DELETE**. </pre>
