# Quickstart guide

This guide will help you get up and running quickly with the API using the provided JSON file containing user and collection data. Follow these steps to start making API requests and accessing data.

## Step 1: Understanding the Data Structure
The API deals with two primary entities: **Users** and **Collections**.

### Users
Each `user` has the following attributes:

* id: Unique identifier for the user
* first_name: The user's first name
* last_name: The user's last name
* email: The user's email address
* privacy: Privacy setting for the user (public/private)


### Collections
Each `collection` has the following attributes:

* id: Unique identifier for the collection
* user_id: The ID of the user who owns the collection
* name: The name of the collection
* privacy: Privacy setting for the collection (public/private)
* created_at: The date the collection was created
* books: An array of books included in the collection with attributes such as title, author, ISBN, etc.

## Step 2: Setting Up Your Environment
Choose Your Tool:

* Use cURL for command-line interactions.
  * [Click here](./Tutorials/curl-setup.md) for next steps in cURL!
* Use Postman for a graphical interface to make API requests.
  * [Click here](./Tutorials/postman-setup.md) for next steps in Postman!
