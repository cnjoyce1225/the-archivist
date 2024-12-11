# Get collections by user

The most common use case for getting collections is to get all collections for a user. This tutorial will guide you through doing that!

## Before we start

Let's go over how the API endpoints will work for this tutorial.  

You will use this endpoint structure to retrieve collections:

``` shell
GET /collections?first_name={first_name}&last_name={last_name}
```

## Using Postman to get the collection

We will use the user `Liam Carter` as an example!

1. **Open Postman** and create a new request.
2. Set the request type to **GET**.
3. Enter the URL for your API endpoint that retrieves collections for `Liam Carter`:

``` shell
http://localhost:3000/collections?first_name=Liam&last_name=Carter
```

4. Click the Send button to execute the request.

You should see the response containing the list of collections for that user in the response body.

* If this dosn't work, after Step 3, you should set headers. You can do this by going to the `Headers` tab and adding a new header with the qualities:
  * Key: `Content-Type`
  * Value: `application/json`
 
 ---

 ## Using cURL to get the collection

We will use the user `Liam Carter` as an example!

1. You can use the following curl command in your terminal or command prompt to make the same GET request:

``` shell
curl -X GET "http://localhost:3000/collections?first_name=Liam&last_name=Carter" \
     -H "Content-Type: application/json"
```

### Example Output

The API should return a response containing the collections associated with the specified user. For example:

``` js
{
  "collections": [
    {
      "id": 101,
      "user_id": 1,
      "name": "Favorite Classics",
      "privacy": "private"
    }
  ]
}
```
