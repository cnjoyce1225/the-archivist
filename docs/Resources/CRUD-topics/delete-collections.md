# Deleting `collections`

In this reference, you'll learn how to delete a collection from your API using Postman and curl. Deleting a collection typically requires the use of the DELETE HTTP method.

### Deleting a Collection in Postman

1. **Open Postman** and create a new request.
2. Set the request type to **DELETE**.
3. Enter the URL for your API endpoint that deletes a collection, including the collection ID. For example:

```shell
https://yourapi.com/api/collections/101
```

(Replace `101` with the actual ID of the collection you wish to delete.)
4. Click on the **Send** button to execute the request.
5. You should see a response indicating that the collection has been successfully deleted.

### Example Response

The expected response after successfully deleting the collection might look like this:

```js
{
  "message": "Collection deleted successfully"
}
```

---

### Deleting a Collection Using Curl

You can use the following curl command in your terminal or command prompt to make the same DELETE request:

```shell
curl -X DELETE "https://yourapi.com/api/collections/101"
```

### Example Response

The expected response from the curl command after successfully deleting the collection might look like this:

```js
{
  "message": "Collection deleted successfully"
}
```

---

### Note:
- Replace `https://yourapi.com/api/collections/101` with the actual endpoint of your API that deletes a collection.
- Make sure the collection ID specified in the URL exists in your database.
- Ensure your API server is running and accessible when you execute these requests.
- Deleting a collection may also require certain permissions or authentication, so ensure you handle any authentication tokens as needed.