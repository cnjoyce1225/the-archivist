# Update a `collection`

Learn how to update a `collection` in your API using Postman and cURL!

### Updating a Collection in Postman

1. **Open Postman** and create a new request.
2. Set the request type to **PUT** or **PATCH** (PUT is generally used for full updates, while PATCH is used for partial updates).
3. Enter the URL for your API endpoint that updates a collection, including the collection ID. For example:

```shell
http://localhost:3000/collections/101
```

(Replace `101` with the actual ID of the collection you wish to update.)
4. In the **Body** tab, select **raw** and set the type to **JSON**.
5. Add the JSON payload with the updated collection information. For example:

```js
{
  "name": "Updated Collection Name",
  "privacy": "public",
  "created_at": "2023-10-01"
}
```

6. Click on the **Send** button to execute the request.
7. You should see a response indicating that the collection has been successfully updated.

### Example Response

The expected response after successfully updating the collection might look like this:

```js
{
  "message": "Collection updated successfully",
  "collection": {
    "id": 101,
    "user_id": 1,
    "name": "Updated Collection Name",
    "privacy": "public",
    "created_at": "2023-10-01"
  }
}
```

---

### Updating a Collection Using Curl

You can use the following curl command in your terminal or command prompt to make the same update request:

```shell
curl -X PUT "http://localhost:3000/collections/101" \
-H "Content-Type: application/json" \
-d '{
  "name": "Updated Collection Name",
  "privacy": "public",
  "created_at": "2023-10-01"
}'
```

### Example Response

The expected response from the curl command after successfully updating the collection might look like this:

  ```js
{
  "message": "Collection updated successfully",
  "collection": {
    "id": 101,
    "user_id": 1,
    "name": "Updated Collection Name",
    "privacy": "public",
    "created_at": "2023-10-01"
  }
}
  ```

---

### Note:
- Ensure that the collection ID specified in the URL exists in your database.
- Ensure your API server is running and accessible when you execute these requests.
- Updating a collection may also require certain permissions or authentication, so ensure you handle any authentication tokens as needed.

---

### Navigation

* Go to the [collection resource](https://cnjoyce1225.github.io/the-archivist/Resources/collections.html)

* Go to the [homepage](https://cnjoyce1225.github.io/the-archivist/)
