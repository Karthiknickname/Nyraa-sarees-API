Nyraa Sarees – Backend

The backend service for the Nyraa Sarees Project, built with Node.js, Express.js, and PostgreSQL.
It provides a robust REST API to manage products, categories, subcategories, product variants, stock mangement, order management with secure, scalable, and maintainable architecture.

🚀 Features

• 🛍️ Product Management – CRUD APIs for products

• 📂 Category & Subcategory Management – Organize and fetch hierarchical data

• 🎨 Variant Management – Add and manage product variants (size, color, etc.)

• 🖼️ Image Upload Support – Product Variant & banner uploads

• 🔐 Authentication & Authorization JWT based 

• 📊 Scalable PostgreSQL Database with Sequelize

• ⚡ Error Handling & Validations with middleware

🛠️ Tech Stack

Runtime: Node.js

Framework: Express.js

Database: PostgreSQL

Client: Sequelize

Auth: JWT & Bcrypt 

File Uploads: Multer 

📂 Folder Structure
NYRAA_API/
│── src/
│   ├── config/          
│   ├── controllers/  
│   ├── middlewares/    
│   ├── models/         
│   ├── routes/
│   ├── uploads/                  
│   ├── utils/          
│   └── app.js        
│
├── .env                  
├── package.json
└── README.md

⚡ Getting Started 

1️⃣ Install Dependencies

npm install

2️Setup Environment Variables

Create a .env file in the root directory:

DB_NAME = Name of your DB
DB_DIALECT=postgres
DB_PORT= 5432/5433
BASE_URL=https://localhost:5000
JWT_SECRET=your_jwt_secret_key

ADMIN_USERNAME = admin username
ADMIN_PASSWORD = admin password
JWT_SECRET

MAIL_USER=your-email@gmail.com
MAIL_PASS=your-app-password

3️⃣ Database Setup

Run migrations or sync models:

# If using Prisma
npx prisma migrate dev

# If using Sequelize
npx sequelize-cli db:migrate

4️⃣ Run Development Server
npm run dev


Server runs on:

http://localhost:5000

📊 API Endpoints
🔑 Auth (optional)

POST /api/auth/register – Register a new user

POST /api/auth/login – Login and get JWT

🛍️ Products

GET /api/products – Get all products

POST /api/products – Create a new product

GET /api/products/:id – Get product by ID

PUT /api/products/:id – Update product

DELETE /api/products/:id – Delete product

📂 Categories

GET /api/categories 

POST /api/categories

GET /api/categories/{id}

PUT  /api/categories/{id}

DELETE /api/categories

📂 Subcategories

GET /api/subcategories

POST /api/subcategories

GET api/subcategories/{id}

PUT api/subcategories/{id}

DELETE api/subcategories/{id}

🎨 Product Variants

GET /api/variants

POST /api/variants

GET /api/product-variants/{id}

PUT /api/product-variants/{id}

DELETE /api/product-variants

