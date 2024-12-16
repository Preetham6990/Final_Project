# Web-Project

## Setup
### Ensure Python 3 compatibility.
1. **Install Required Packages:**
   - pip install fastapi
   - pip install pydantic
   - pip install uvicorn

## Database Setup

2. **Initialize the database with:**
   - python init_db.py

## API Endpoints

### Customers
- **POST /customers:** Adds a new customer.
- **GET /customers/{id}:** Fetches details of a customer by ID.
- **DELETE /customers/{id}:** Removes a customer by ID.
- **PUT /customers/{id}:** Updates details of a customer by ID.

These endpoints manage customer records, allowing for addition, retrieval, modification, and deletion of data.

### Menu Items
- **POST /items:** Adds a new menu item.
- **GET /items/{id}:** Fetches details of a menu item by ID.
- **DELETE /items/{id}:** Removes a menu item by ID.
- **PUT /items/{id}:** Updates details of a menu item by ID.

These endpoints help in managing menu items, facilitating their addition, display, update, and deletion.

### Orders
- **POST /orders:** Places a new order.
- **GET /orders/{id}:** Fetches order details by ID.
- **DELETE /orders/{id}:** Cancels an order by ID.
- **PUT /orders/{id}:** Modifies details of an existing order.

These endpoints assist in order handling, enabling order placement, viewing, updating, and cancellation.

## Running the Server

Upon running the server, it will display a URL (http://127.0.0.1:8000).

### Note for POST Requests

When using POST to add new records, remove the automatically generated `"id": 0` from the FastAPI form and complete the remaining fields as needed.
