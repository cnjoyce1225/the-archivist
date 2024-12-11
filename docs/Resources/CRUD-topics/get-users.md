# Get `users`

### Using Postman

1. **Open Postman** and create a new request.
2. Set the request type to **GET**.
3. Enter the URL for your API endpoint that retrieves users, for example:
```shell
http://localhost:3000/users
```
4. Click on the **Send** button to execute the request.
5. You should see the response with the list of users in the response body.
(insert sample here)

### Using Curl
You can use the following curl command in your terminal or command prompt to make the same GET request:
```shell
curl -X GET "http://localhost:3000/users"
```
### Example Output

The expected JSON response for the users might look like this:
```js
[
    {
  "users": [
    {
      "id": 1,
      "first_name": "Liam",
      "last_name": "Carter",
      "email": "liam.carter@example.com",
      "privacy": "public"
    },
    {
      "id": 2,
      "first_name": "Sophia",
      "last_name": "Nguyen",
      "email": "sophia.nguyen@example.com",
      "privacy": "public"
    },
    {
      "id": 3,
      "first_name": "Ethan",
      "last_name": "Ramirez",
      "email": "ethan.ramirez@example.com",
      "privacy": "private"
    },
    {
      "id": 4,
      "first_name": "Olivia",
      "last_name": "Patel",
      "email": "olivia.patel@example.com",
      "privacy": "private"
    }
  ]
}
]
```

---

### Note:
- Make sure your API server is running and accessible when you execute these requests.

---

### Navigation

* Go to the [user resource](https://cnjoyce1225.github.io/the-archivist/Resources/user.html)

* Go to the [homepage](https://cnjoyce1225.github.io/the-archivist/)

