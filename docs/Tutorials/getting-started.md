# Getting Started with the Archivist Database JSON

Before you start using the `the-archivist-db-source.json` file to complete tasks using cURL and Postman, it's essential to first set up your development environment, get your API server running, and ensure you can successfully retrieve data from your endpoints. This guide outlines how to do all of this so you can run the API service smoothly!

## Prerequisites

1. **Basic Knowledge**:
   - Familiarity with RESTful APIs and how they function.
   - Basic understanding of JSON format.

2. **Software Requirements**:
   - **Node.js**: Ensure you have Node.js installed on your machine. You can download it from [nodejs.org](https://nodejs.org/).
   - **cURL**: This command-line tool is used for transferring data with URLs. Most operating systems have it pre-installed. You can check by running `curl --version` in your command line.
   - **Postman**: Download and install Postman from [postman.com](https://www.postman.com/downloads/) for a user-friendly interface to test API endpoints.

3. **Project Setup**:
   - Create a project folder where you will store your JSON file and any related scripts.
   - Place the `the-archivist-db-source.json` file in your project directory.

---

## Let's get started!
   
### Step 1: Create an API Server


To interact with the JSON data, you need to create a simple API server. This can be done using Node.js and Express, as shown in the previous guides. Follow these steps:

1. **Initialize a New Node.js Project**:
   Open your command line and navigate to your project directory. Run the following command:

   ``` shell
   npm init -y
   ```

2. **Install Express**:
Install Express and body-parser by running:

   ``` shell
   npm install express body-parser
   ```

3. **Create a Server File**:
   Create a file named `server.js` and set up a simple Express server to read from your JSON file. You can refer to the code provided in previous steps to set up your server and endpoints.


### Step 2: Start the API Server


1. **Run the Server**:
   In your command line, execute the following command in your project directory:

   ``` shell
   node server.js
   ```

2. **Verify the Server is Running**:
   You should see an output message confirming that the server is running at a specified URL (e.g., `http://localhost:3000`).


### Step 3: Testing Your Development System


Now that your API server is running, it’s time to test your setup using cURL and Postman.

#### Testing with cURL

1. **Open Command Line**:
   Open a new terminal window.

2. **Test Users Endpoint**:
   Run the following command to fetch the users:

   ``` shell
   curl http://localhost:3000/users
   ```

3. **Test Collections Endpoint**:
   Run this command to fetch collections:

   ``` shell
   curl http://localhost:3000/collections
   ```

4. **Check Responses**:
   You should see JSON responses for both commands if everything is set up correctly.

#### Testing with Postman

1. **Open Postman**:
   Launch the Postman application.

2. **Create a New Request**:
   - Click on the "+" button to create a new tab.
   - Select `GET` as the request type.

3. **Test Users Endpoint**:
   - Enter the URL: `http://localhost:3000/users`
   - Click the "Send" button.
   - You should see the list of users in the response area.

4. **Test Collections Endpoint**:
   - Create another request with the URL: `http://localhost:3000/collections`
   - Click "Send" and check for the collections data in the response.
  
