# Delete a `user`

Learn how to delete a `user` in your API using Postman and cURL!

### Deleting a User in Postman

1. **Open Postman** and create a new request.
2. Set the request type to **DELETE**.
3. Enter the URL for your API endpoint that deletes a user, including the user ID. For example:

  ```shell
  http://localhost:3000/users/1
  ```

(Replace `1` with the actual ID of the user you wish to delete.)
4. Click on the **Send** button to execute the request.
5. You should see a response indicating that the user has been successfully deleted.

### Example Response

The expected response after successfully deleting the user might look like this:
```js
{
  "message": "User deleted successfully"
}
```

---

### Deleting a User Using Curl

You can use the following curl command in your terminal or command prompt to make the same DELETE request:
```shell
curl -X DELETE "http://localhost:3000/users/1"
```

### Example Response

The expected response from the curl command after successfully deleting the user might look like this:
```js
{
  "message": "User deleted successfully"
}
```
---

### Note:
- Make sure the user ID specified in the URL exists in your database.
- Ensure your API server is running and accessible when you execute these requests.
- Deleting a user may also require certain permissions or authentication, so ensure you handle any authentication tokens as needed.

---

### Navigation

* Go to the [user resource](https://cnjoyce1225.github.io/the-archivist/Resources/user.html)

* Go to the [homepage](https://cnjoyce1225.github.io/the-archivist/)

