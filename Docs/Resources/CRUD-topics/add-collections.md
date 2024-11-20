# Add `collections`

### Using Postman

1. **Open Postman** and create a new request.
2. Set the request type to **POST**.
3. Enter the URL for your API endpoint that adds a collection, for example:
```shell
https://yourapi.com/api/collections
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
bash
curl -X POST "https://yourapi.com/api/collections" \
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
