# Get collections by user

The most common use case for getting collections is to get all collections for a user. This tutorial will guide you through doing that!

## Before we start

Let's go over how the API endpoints will work for this tutorial.  

You will use this endpoint structure to retrieve collections:

``` shell
GET /api/collections?first_name={first_name}&last_name={last_name}
```

## Using Postman to get the collection

We will use the user `Liam Carter` as an example!

1. Launch Postman on your computer.

2. Create a New Request:

* Click on the New button or the + tab to create a new request.
* Select HTTP Request.

3. Set Up the Request:

* Set the request method to GET.
* Enter the API endpoint URL:

``` shell
https://yourapi.com/api/collections?first_name=Liam&last_name=Carter
```

4. Click the `Send` button

### Expected Output
* Postman will display the response in the lower section, showing the collections associated with the specified user, similar to the output from cURL.
* If this dosn't work, after Step 3, you should set headers. You can do this by going to the `Headers` tab and adding a new header with the qualities:
  * Key: `Content-Type`
  * Value: `application/json`
 
 ---

 ## Using cURL to get the collection

We will use the user `Liam Carter` as an example!

1. Use the following curl command in your terminal or command prompt to make this GET request:

``` shell
curl -X GET "https://yourapi.com/api/collections?first_name=Liam&last_name=Carter" \
     -H "Content-Type: application/json"
```

### Expected Output

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
