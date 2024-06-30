# E-commerce Inventory Management System

## Overview

This is a simple e-commerce inventory management system built with FastAPI. It provides endpoints to manage products in an inventory.

## Features

- **POST /products**: Create a new product.
- **GET /products**: Retrieve all products.
- **GET /products/{id}**: Retrieve a single product by ID.
- **PUT /products/{id}**: Update a product by ID.
- **DELETE /products/{id}**: Delete a product by ID.

## Setup and Installation

### Prerequisites

- Python 3.10 or higher
- Virtual environment tool (optional but recommended)
- VS Code or any code editor
- Command Line Interface (CLI)

### Steps

1. Clone the Repository:

   ```bash
   git clone <repository-url>
   cd "C:\Users\hp\VS Code Projects\E-commerce API development"

2. Create a Virtual Environment:

    ```bash
    command: python -m venv venv
    
3. Activate the Virtual Environment:

    On Windows:
    ```bash
    command: .\venv\Scripts\activate

4. Install Required Libraries:

    ```bash
    commands: pip install fastapi uvicorn sqlalchemy pydantic

5. Create the SQLite Database:

    ```bash
    python -c "from main import Base, engine; Base.metadata.create_all(bind=engine)"

6. Run the Application:

    ```bash
    command: uvicorn main:app --reload

The application will be available at http://127.0.0.1:8000.   


# API Documentation:

    Visit http://127.0.0.1:8000/docs for the interactive API documentation.

## Usage:

Create a Product

- **Endpoint: POST /products**

    Request Body: json

    {
    "name": "Product Name",
    "description": "Product Description",
    "price": 150
    }

Retrieve All Products:

- **Endpoint: GET /products**

Retrieve a Product by ID:

- **Endpoint: GET /products/{id}**

Update a Product:

- **Endpoint: PUT /products/{id}**

    Request Body: json

    {
    "name": "Updated Product Name",
    "description": "Updated Product Description",
    "price": 150
    }

Delete a Product:

- **Endpoint: DELETE /products/{id}**

License:
This project is licensed under the MIT License.

By following these steps, you'll have a complete FastAPI application that you can run and test locally. This includes setting up the project, running the application, and providing comprehensive documentation.