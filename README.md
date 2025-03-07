# RestAPI-Doc

## API Endpoints

### GET /api/items
- Description: Retrieve a list of items
- Example Request:
  ```
  GET /api/items
  ```
- Example Response:
  ```json
  [
    {
      "id": 1,
      "name": "Item 1",
      "description": "Description of Item 1"
    },
    {
      "id": 2,
      "name": "Item 2",
      "description": "Description of Item 2"
    }
  ]
  ```

### POST /api/items
- Description: Create a new item
- Example Request:
  ```
  POST /api/items
  Content-Type: application/json

  {
    "name": "New Item",
    "description": "Description of the new item"
  }
  ```
- Example Response:
  ```json
  {
    "id": 3,
    "name": "New Item",
    "description": "Description of the new item"
  }
  ```

### PUT /api/items/{id}
- Description: Update an existing item
- Example Request:
  ```
  PUT /api/items/1
  Content-Type: application/json

  {
    "name": "Updated Item",
    "description": "Updated description of the item"
  }
  ```
- Example Response:
  ```json
  {
    "id": 1,
    "name": "Updated Item",
    "description": "Updated description of the item"
  }
  ```

### DELETE /api/items/{id}
- Description: Delete an item
- Example Request:
  ```
  DELETE /api/items/1
  ```
- Example Response:
  ```json
  {
    "message": "Item deleted successfully"
  }
  ```

## Setup and Usage Instructions

### Prerequisites
- Node.js (version 12 or higher)
- npm (Node Package Manager)

### Setup
1. Clone the repository:
   ```
   git clone https://github.com/UdayDamerla5/RestAPI-Doc.git
   ```
2. Navigate to the project directory:
   ```
   cd RestAPI-Doc
   ```
3. Install the dependencies:
   ```
   npm install
   ```

### Running the API Server
1. Start the server:
   ```
   npm start
   ```
2. The API server will be running at `http://localhost:3000`

### Dependencies
- Express (version 4.17.1 or higher)
- Body-parser (version 1.19.0 or higher)

## Sample Code

For sample code demonstrating how to use the API, please refer to the `sample_code.md` file.
