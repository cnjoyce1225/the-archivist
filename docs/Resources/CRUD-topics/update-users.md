# Update `users`

In this reference, you'll learn how to update a user's information in your API using Postman and curl. Updating a user typically requires the use of the PUT or PATCH HTTP method.

### Updating a User in Postman

1. **Open Postman** and create a new request.
2. Set the request type to **PUT** or **PATCH** (PUT is generally used for full updates, while PATCH is used for partial updates).
3. Enter the URL for your API endpoint that updates a user, including the user ID. For example:

```shell
https://yourapi.com/api/users/1
```

(Replace `1` with the actual ID of the user you wish to update.)
4. In the **Body** tab, select **raw** and set the type to **JSON**.
5. Add the JSON payload with the updated user information. For example:

```js
{
  "first_name": "John",
  "last_name": "Doe",
  "email": "john.doe@example.com",
  "privacy": "private"
}
```

6. Click on the **Send** button to execute the request.
7. You should see a response indicating that the user has been successfully updated.

### Example Response

The expected response after successfully updating the user might look like this:

```js
{
  "message": "User updated successfully",
  "user": {
    "id": 1,
    "first_name": "John",
    "last_name": "Doe",
    "email": "john.doe@example.com",
    "privacy": "private"
  }
}
```

---

### Updating a User Using Curl

You can use the following curl command in your terminal or command prompt to make the same update request:

```shell
bash
curl -X PUT "https://yourapi.com/api/users/1" \
-H "Content-Type: application/json" \
-d '{
  "first_name": "John",
  "last_name": "Doe",
  "email": "john.doe@example.com",
  "privacy": "private"
}'
```

### Example Response

The expected response from the curl command after successfully updating the user might look like this:

```js

{
  "message": "User updated successfully",
  "user": {
    "id": 1,
    "first_name": "John",
    "last_name": "Doe",
    "email": "john.doe@example.com",
    "privacy": "private"
  }
}

```

---

### Note:
- Replace `https://yourapi.com/api/users/1` with the actual endpoint of your API that updates a user.
- Ensure that the user ID specified in the URL exists in your database.
- Ensure your API server is running and accessible when you execute these requests.
- Updating a user may also require certain permissions or authentication, so ensure you handle any authentication tokens as needed.