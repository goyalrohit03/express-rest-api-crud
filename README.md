project:
  name: Express REST API Client – Secrets API Integration
  description: |
    A Node.js + Express web app that interacts with the Secrets API using REST operations (GET, POST, PUT, PATCH, DELETE).
    The project includes a styled EJS form to interact with API endpoints using Axios.

tech_stack:
  - Node.js
  - Express.js
  - Axios
  - EJS
  - body-parser

setup:
  step_1:
    title: Clone the repository
    command: |
      git clone https://github.com/goyalrohit03/express-rest-api-crud.git
      cd express-rest-api-crud
  step_2:
    title: Install dependencies
    command: npm install
  step_3:
    title: Add your Bearer Token
    file: index.js
    instruction: |
      Replace the placeholder with your real token:
      const yourBearerToken = "your-token-here";
  step_4:
    title: Start the server
    command: node index.js
  step_5:
    title: Open in browser
    url: http://localhost:3000

api_token:
  how_to_generate:
    step_1: Visit https://secrets-api.appbrewery.com/
    step_2: Click "Get your Bearer Token"
    step_3: Sign in with your email
    step_4: Copy the token provided
    step_5: Paste the token into index.js as the value for yourBearerToken

usage:
  GET_secret:
    endpoint: /secrets/:id
    form_fields: [id]
    action: Click "GET"
    result: Fetches a secret by ID
  POST_secret:
    endpoint: /secrets
    form_fields: [secret, score, route]
    action: Click "POST"
    result: Creates a new secret
  PUT_secret:
    endpoint: /secrets/:id
    form_fields: [id, secret, score, route]
    action: Click "PUT"
    result: Replaces a secret completely
  PATCH_secret:
    endpoint: /secrets/:id
    form_fields: [id, secret (optional), score (optional), route (optional)]
    action: Click "PATCH"
    result: Updates specific fields of a secret
  DELETE_secret:
    endpoint: /secrets/:id
    form_fields: [id]
    action: Click "DELETE"
    result: Deletes the secret by ID

project_structure:
  - index.js
  - package.json
  - views/
    - index.ejs
  - .gitignore

notes:
  - Add `.gitignore` and exclude `node_modules/` and `.env`
  - Format API responses using `JSON.stringify(result.data, null, 2)` for better readability
  - Consider using `dotenv` to manage sensitive tokens

contact:
  github: https://github.com/goyalrohit03
  support: Raise an issue on the GitHub repository

