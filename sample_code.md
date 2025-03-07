# Sample Code

Below is a sample code demonstrating how to use the API.

## Sample Code for GET /api/items

```javascript
const axios = require('axios');

axios.get('http://localhost:3000/api/items')
  .then(response => {
    console.log(response.data);
  })
  .catch(error => {
    console.error('Error fetching items:', error);
  });
```

## Sample Code for POST /api/items

```javascript
const axios = require('axios');

const newItem = {
  name: 'New Item',
  description: 'Description of the new item'
};

axios.post('http://localhost:3000/api/items', newItem)
  .then(response => {
    console.log('Item created:', response.data);
  })
  .catch(error => {
    console.error('Error creating item:', error);
  });
```

## Sample Code for PUT /api/items/{id}

```javascript
const axios = require('axios');

const updatedItem = {
  name: 'Updated Item',
  description: 'Updated description of the item'
};

axios.put('http://localhost:3000/api/items/1', updatedItem)
  .then(response => {
    console.log('Item updated:', response.data);
  })
  .catch(error => {
    console.error('Error updating item:', error);
  });
```

## Sample Code for DELETE /api/items/{id}

```javascript
const axios = require('axios');

axios.delete('http://localhost:3000/api/items/1')
  .then(response => {
    console.log('Item deleted:', response.data);
  })
  .catch(error => {
    console.error('Error deleting item:', error);
  });
```
