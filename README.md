# CRUD Application using Spring Boot and Elasticsearch

![image](https://github.com/lucasruviaro/spring-elasticsearch-crud/assets/103154696/c8110897-a002-4563-ba72-b79f2cc2e4f6)


This repository contains a basic CRUD (Create, Read, Update, Delete) application built with Spring Boot and Elasticsearch. The application provides API endpoints for managing products.

## Endpoints

1. **Fetch All Products**

   - **Endpoint:**
     ```http
     GET /api/findAll
     ```

   - **Description:**
     Fetches all saved products.

2. **Insert a New Product**

   - **Endpoint:**
     ```http
     POST /api/insert
     ```

   - **Request Body:**
     ```json
     {
       "name": "table",
       "description": "table 50x50in",
       "quantity": 100,
       "price": 349.99
     }
     ```

   - **Description:**
     Saves a new product with the specified details.

3. **Update an Existing Product**

   - **Endpoint:**
     ```http
     PUT /api/update/{id}
     ```

   - **Request Body:**
     ```json
     {
       "name": "table",
       "description": "table 50x50in",
       "quantity": 100,
       "price": 349.99
     }
     ```

   - **Description:**
     Updates an already saved product identified by its unique ID.

4. **Delete a Product**

   - **Endpoint:**
     ```http
     DELETE /api/delete/{id}
     ```

   - **Description:**
     Deletes a product with the specified ID.
