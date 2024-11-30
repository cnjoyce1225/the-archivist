# Delete a book from `collections`

In this reference, you'll learn how to delete a book from a collection in your API using Postman and curl. Deleting a book typically requires the use of the DELETE HTTP method.

### Deleting a Book from a Collection in Postman

1. **Open Postman** and create a new request.
2. Set the request type to **DELETE**.
3. Enter the URL for your API endpoint that deletes a book from a specific collection, including the collection ID and the book ID. For example:

```shell
https://yourapi.com/api/collections/101/books/1
```

(Replace `101` with the actual ID of the collection and `1` with the actual ID of the book you wish to delete.)
4. Click on the **Send** button to execute the request.
5. You should see a response indicating that the book has been successfully deleted from the collection.

### Example Response

The expected response after successfully deleting the book might look like this:

```js
{
  "message": "Book deleted successfully from collection"
}
```

---

### Deleting a Book from a Collection Using Curl

You can use the following curl command in your terminal or command prompt to make the same DELETE request:

```shell
bash
curl -X DELETE "https://yourapi.com/api/collections/101/books/1"
```

### Example Response

The expected response from the curl command after successfully deleting the book might look like this:

```js
{
  "message": "Book deleted successfully from collection"
}
```

---

### Note:
- Replace `https://yourapi.com/api/collections/101/books/1` with the actual endpoint of your API that deletes a book from a collection.
- Make sure the collection ID and book ID specified in the URL exist in your database.
- Ensure your API server is running and accessible when you execute these requests.
- Deleting a book from a collection may also require certain permissions or authentication, so ensure you handle any authentication tokens as needed.