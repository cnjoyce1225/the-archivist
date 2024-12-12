# Create `user`

### Using Postman

1. **Open Postman** and create a new request.
2. Set the request type to **POST**.
3. Enter the URL for your API endpoint that adds a user, for example:
```shell
http://localhost:3000/users
```
4. In the **Body** tab, select **raw** and set the type to **JSON**.
5. Add the JSON payload for the new user. For example:

  ```shell
  {
    "first_name": "John",
    "last_name": "Doe",
    "email": "john.doe@example.com",
    "privacy": "public"
  }
  ```

6. Click on the **Send** button to execute the request.
7. You should see the response indicating that the user has been added.

### Using Curl

You can use the following curl command in your terminal or command prompt to make the same POST request:

  ```shell
  curl -X POST "http://localhost:3000/users" \
  -H "Content-Type: application/json" \
  -d '{
    "first_name": "John",
    "last_name": "Doe",
    "email": "john.doe@example.com",
    "privacy": "public"
  }'
  ```

### Example Response

The expected JSON response after successfully adding the user might look like this:
  ```js
{
  "id": 5,
  "first_name": "John",
  "last_name": "Doe",
  "email": "john.doe@example.com",
  "privacy": "public"
}
  ```

### Note:
- Ensure that the email is unique and does not already exist in the database.
- Ensure your API server is running and accessible when you execute these requests.

---

### Navigation

* Go to the [user resource](https://cnjoyce1225.github.io/the-archivist/Resources/user.html)

* Go to the [homepage](https://cnjoyce1225.github.io/the-archivist/)
