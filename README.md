# RESTful Inventory Management API

A production-ready backend API demonstrating mastery of modern Node.js development, NoSQL database design, and RESTful architecture patterns.

## 💼 Skills Demonstrated

This project showcases how i worked with **Node.js and Express.js** backend development, where I built a scalable HTTP server with sophisticated routing and middleware management. The API implements full RESTful architecture with complete CRUD operations following industry best practices. A custom logging system demonstrates expertise in error handling and production-level debugging, while the modular codebase i made sure to make separate of concerns through organized models, routes, and controllers.

The data layer reflects database design skills using **MongoDB and Mongoose**, including efficient schema design with proper validation and type safety. The project demonstrates practical experience with NoSQL data modeling, handling multiple field types and relationships, with optimized queries for data retrieval and manipulation at scale.

Beyond core development, this project incorporates standard practices including API testing with Insomnia, version control with Git and GitHub, Docker containerization for deployment, and structured monitoring systems.

## 🏗️ Architecture Overview

**Stack:** Node.js | Express.js | MongoDB | Mongoose

**Key Features:**

- Full CRUD API endpoints for inventory management
- Input validation and error handling
- Structured logging for monitoring
- Docker containerization for deployment
- RESTful conventions and HTTP status codes

## 🚀 API Endpoints

| Method | Endpoint     | Description             |
| ------ | ------------ | ----------------------- |
| GET    | `/items`     | Retrieve all items      |
| POST   | `/items`     | Create a new item       |
| PUT    | `/items/:id` | Update an existing item |
| DELETE | `/items/:id` | Delete an item          |

## 📊 Data Model

**Collection:** `items`

```
{
  _id: ObjectId,
  name: String,           // Item name/title
  category: String,       // Product category (Fruit, Dairy, Bakery, etc.)
  price: Number,          // Item price
  quantity: Number        // Current stock quantity
}
```

## 🚀 Getting Started

### Prerequisites

- Node.js v14+
- MongoDB running locally or via Docker
- npm or yarn package manager

### Installation & Setup

```bash
# Clone the repository
git clone <repository-url>
cd mongo-express

# Install dependencies
npm install

# Start MongoDB (if not running)
# Via Docker: docker-compose up -d

# Start the server
node index.js

# API available at: http://localhost:3000
```

## 📖 Documentation & Testing

**API Testing:** Use Insomnia, Postman, or curl to test endpoints

- All endpoints return JSON responses
- Proper HTTP status codes (200, 201, 400, 404, 500)
- Request/response examples available in screenshots

## 🔧 Technical Highlights

- **Custom Logger**: Implemented structured logging for debugging and monitoring
- **Mongoose Validation**: Schema validation ensures data integrity
- **Docker Support**: Application containerized for consistent deployment
- **Production Ready**: Error handling, status codes, and best practices implemented

---

### MongoDB Database Setup

![MongoDB Compass showing database and collection](4.png)
_MongoDB Compass showing the `myfirstdatabase` with `items` collection and sample grocery data_

### API Testing - CRUD Operations

#### GET Request - Fetch All Items

![GET request showing all items](0.png)
_GET request to `/items` endpoint showing all grocery items in the database_

#### POST Request - Create New Item

![POST request creating new item](1.png)
_POST request to `/items` endpoint creating a new "Oranges" item_

#### PUT Request - Update Item

![PUT request updating item](2.png)
_PUT request to `/items/:id` endpoint updating Apples quantity to 30_

#### DELETE Request - Remove Item

![DELETE request removing item](3.png)
_DELETE request to `/items/:id` endpoint successfully removing an item_

---

_This project was created as part of a backend development course to learn fundamental concepts of API development and database integration._
