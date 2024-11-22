# Pull `users`

### Using Postman

1. **Open Postman** and create a new request.
2. Set the request type to **GET**.
3. Enter the URL for your API endpoint that retrieves users, for example:
```shell
https://yourapi.com/api/users
```
4. Click on the **Send** button to execute the request.
5. You should see the response with the list of users in the response body.
(insert sample here)

### Using Curl
You can use the following curl command in your terminal or command prompt to make the same GET request:
```shell
bash
curl -X GET "https://yourapi.com/api/users"
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
- Replace `https://yourapi.com/api/users` with the actual endpoint of your API that returns the list of users.
- Make sure your API server is running and accessible when you execute these requests.