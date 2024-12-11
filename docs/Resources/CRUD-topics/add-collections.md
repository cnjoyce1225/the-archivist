# Create `collections`

### Using Postman

1. **Open Postman** and create a new request.
2. Set the request type to **POST**.
3. Enter the URL for your API endpoint that adds a collection, for example:
```shell
http://localhost:3000/collections
```
4. In the **Body** tab, select **raw** and set the type to **JSON**.
5. Add the JSON payload for the new collection. For example:
  ```js
  {
    "user_id": 1,
    "name": "New Collection Name",
    "privacy": "private",
    "created_at": "2023-10-01",
    "books": []
  }
  ```
6. Click on the **Send** button to execute the request.
7. You should see the response indicating that the collection has been added.

### Using Curl

You can use the following curl command in your terminal or command prompt to make the same POST request:
```shell
curl -X POST "http://localhost:3000/collections" \
-H "Content-Type: application/json" \
-d '{
  "user_id": 1,
  "name": "New Collection Name",
  "privacy": "private",
  "created_at": "2023-10-01",
  "books": []
}'
```
### Example Response

The expected JSON response after successfully adding the collection might look like this:
  ```js
  {
  "id": 501,
  "user_id": 1,
  "name": "New Collection Name",
  "privacy": "private",
  "created_at": "2023-10-01",
  "books": []
  }
  ```

---

### Note:
- Ensure that the `user_id` corresponds to a valid user in your database.
- Ensure your API server is running and accessible when you execute these requests.

---

### Navigation

* Go to the [collection resource](https://cnjoyce1225.github.io/the-archivist/Resources/collections.html)

* Go to the [homepage](https://cnjoyce1225.github.io/the-archivist/)

