# Pull `collections`

### Using Postman

1. **Open Postman** and create a new request.
2. Set the request type to **GET**.
3. Enter the URL for your API endpoint that retrieves collections, for example:
```shell
https://yourapi.com/api/collections
```
4. Click on the **Send** button to execute the request.
5. You should see the response containing the list of collections in the response body.

### Using Curl

You can use the following curl command in your terminal or command prompt to make the same GET request:
```shell
bash
curl -X GET "https://yourapi.com/api/collections"
```
### Example Output

The expected JSON response for the collections might look like this:
```js
{
  "collections": [
    {
      "id": 101,
      "user_id": 1,
      "name": "Favorite Classics",
      "privacy": "private",
      "created_at": "2023-08-15",
      "books": [
        {
          "id": 1,
          "title": "Wuthering Heights",
          "author": "Emily Brontë",
          "isbn": "NA",
          "edition": "US First Edition",
          "year": "1848",
          "publisher": "Harper & Brothers",
          "cover type": "Cloth",
          "condition": "Good",
          "price": "$17,500",
          "seller": "Heritage Books Haven",
          "language": "English",
          "status": "Acquired"
        },
        {
          "id": 2,
          "title": "Dracula",
          "author": "Bram Stoker",
          "isbn": "NA",
          "edition": "First Edition",
          "year": "1897",
          "publisher": "Archibald Constable and Company",
          "cover type": "Hardcover",
          "condition": "Near Fine",
          "price": "$40,000",
          "seller": "The Raven's Claw Rare Books Emporium",
          "language": "English",
          "status": "Acquired"
        }
      ]
    },
    {
      "id": 201,
      "user_id": 2,
      "name": "The Tolkien Archives",
      "privacy": "public",
      "created_at": "2023-09-01",
      "books": [
        {
          "id": 1,
          "title": "History of Middle Earth Box Set 1",
          "author": "J.R.R. Tolkien",
          "isbn": "978-0-063-37984-8",
          "edition": "First Edition",
          "year": "2024",
          "publisher": "William Morrow",
          "cover type": "Hardcover",
          "condition": "New",
          "price": "$68.99",
          "seller": "Amazon",
          "language": "English",
          "status": "Acquisition Pending"
        },
        {
          "id": 2,
          "title": "The Silmarillion",
          "author": "J.R.R. Tolkien",
          "isbn": "978-0-063-339619-7",
          "edition": "First Edition",
          "year": "2024",
          "publisher": "William Morrow",
          "cover type": "Hardcover",
          "condition": "New",
          "price": "$24.50",
          "seller": "Amazon",
          "language": "English",
          "status": "Acquired"
        }
      ]
    }
    // Additional collections here
  ]
}
```