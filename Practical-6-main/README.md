
## Installation

### 1. Clone the Repository

```
git clone https://github.com/yourusername/ecommerce-app.git
cd ecommerce-app
```

---

### 2. Install Dependencies

```
npm install
```

---

### 3. Configure Environment Variables

Create a `.env` file in the root directory.

Example:

```
MONGO_URI=mongodb://localhost:27017/ecommerce
PORT=5000
```

---

### 4. Start MongoDB Server

Make sure MongoDB is running.

If using local MongoDB:

```
mongod
```

Or ensure the **MongoDB service** is running in your system.

---

### 5. Run the Application

Start the server:

```
node server.js
```

or using nodemon:

```
npx nodemon server.js
```

Server will start on:

```
http://localhost:5000
```

---

## API Endpoints

### Product Routes

Create Product

```
POST /api/products
```

Get All Products

```
GET /api/products
```

Update Product

```
PUT /api/products/:id
```

Delete Product

```
DELETE /api/products/:id
```

---

### Example Request (Create Product)

POST `/api/products`

Body (JSON):

```
{
  "name": "Laptop",
  "price": 80000,
  "description": "Gaming Laptop",
  "stock": 10
}
```

---

### Example Update Request

PUT `/api/products/:id`

```
{
  "price": 75000,
  "stock": 15
}
```

---

## Testing the API

You can test the endpoints using:

* Postman
* curl
* Thunder Client (VS Code)

---

---
