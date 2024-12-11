# Get collections by user

The most common use case for getting collections is to get all collections for a user. This tutorial will guide you through doing that!

## Before we start

Let's go over how the API endpoints will work for this tutorial.  

You will use this endpoint structure to retrieve collections:

``` shell
GET /api/collections?first_name={first_name}&last_name={last_name}
```

## Using Postman to get the collection

1. Open Postman

* Launch Postman on your computer.

2. Create a New Request

* Click on the New button or the + tab to create a new request.
* Select HTTP Request.

3. Set Up the Request

* Set the request method to GET.
* Enter the API endpoint URL:

``` shell
https://yourapi.com/api/collections?first_name=Liam&last_name=Carter
```

4. Send the Request
* Click the Send button.

# Expected Output
* Postman will display the response in the lower section, showing the collections associated with the specified user, similar to the output from cURL.
* If this dosn't work, after Step 3, you should set headers. You can do this by going to the `Headers` tab and adding a new header with the qualities:
  * Key: `Content-Type`
  * Value: `application/json`
