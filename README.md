# ToolShop-Postman-Project-API
This repository contains a Postman collection with automated API tests targeting the https://practicesoftwaretesting.com/ Tool Shop API. It includes requests and validations for Product Search and Add to Cart functionalities.

# Postman API Test Automation Example
This repository contains a Postman collection demonstrating automated API testing skills using the public Practice Software Testing Tool Shop API (https://practicesoftwaretesting.com).

## Purpose
This collection serves as a portfolio example showcasing the ability to:
  1. Identify and structure API requests for key e-commerce functionalities (Product Search, Add to Cart).
  2. Utilize Postman variables (via Pre-request Scripts) for parameterization and maintainability.
  3. Implement automated tests within Postman using JavaScript to validate:
  4. HTTP Status Codes (e.g., 200 OK, 201 Created).
  5. JSON Response Body structure (e.g., checking for arrays, object properties).
  6. Specific data values returned by the API.

## Collection File
ToolShop API Tests.postman_collection.json

## How to Use
  1. Download: Download the ToolShop API Tests.postman_collection.json file.
  2. Import to Postman:
       2.1. Open Postman.
       2.2. Click "Import".
       2.3. Upload the downloaded .json file.

## Run: 
Execute individual requests or the entire collection/folders to see the tests run and their results in the "Test Results" tab.

## Requests Included
The collection is organized into folders:

📁 Products: 

  [GET] List the product by name: Searches for products using a parameterized query (q). Includes tests validating status code, response structure (non-empty data array), and key product details (id, name, description, price).
  
📁 Cart: 

  [POST] Add a product to the cart by id: Adds a product to the cart using a parameterized product ID in the request body. Includes a test validating the 201 Created status code, confirming successful addition. Note: Based on analysis, this endpoint on the practice site doesn't require authentication headers.

## Variables
Request-specific parameters (_productName, _productId) are managed using Postman variables set in the Pre-request Script tab of each request.
