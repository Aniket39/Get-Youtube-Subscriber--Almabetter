<img src="https://cdn-icons-png.flaticon.com/512/1384/1384060.png" alt="Alt text" width="700" title="Optional title">

# Get YouTube Subscribers
The YouTube Subscribers is a simple backend project that provides a RESTful API for retrieving data about subscribers to YouTube channels. The project is built using Node.js and Express, and uses MongoDB as the database to store the subscriber data.

The API provides several endpoints that allow users to retrieve data in JSON format, including an endpoint to get all subscribers, an endpoint to get all subscribers' names and subscribed channels, and an endpoint to get details about a particular subscriber based on their ID. The project also handles error cases, such as when an incorrect subscriber ID is provided or when a user accesses an unknown endpoint.

The main purpose of this project is to provide a starting point for building a larger application that deals with YouTube data. The project can be used as a basis for building a more complex API that includes additional functionality, such as adding or deleting subscribers, searching for subscribers based on specific criteria, or integrating with the YouTube API to access data about channels and videos.

 
## Table of Contents
- [Get YouTube Subscribers](#get-youtube-subscribers)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
  - [Features](#features)
  - [Dependencies](#dependencies)
  - [Documentation](#documentation)
  - [API Endpoints](#api-endpoints)
  - [Demo](#demo)
  - [Badges](#badges)

## Installation
To get started with the Project, you'll need to have Node.js and MongoDB installed on your machine. Once you have those installed, follow these steps:

```bash
Clone this repository to your local machine.
Install the required dependencies by running npm install in the project directory.
Start the server by running npm start. The server will be available at http://localhost:3000.
```
## Features
The following features are available in the API:
- Get an array of all subscribers in JSON format.
- Get an array of all subscribers' names and subscribed channels in JSON format.
- Get details about a particular subscriber based on their ID, including their name, subscribed channel, and subscribed date.
- Handle error cases, such as when an incorrect subscriber ID is provided or when a user accesses an unknown endpoint.

## Dependencies
The following dependencies are required to run the Get YouTube Subscribers :
```bash
NodeJs
ExpressJs
Mongoose
nodemon
```


**Note**: Please ensure that your code adheres to the existing style and passes the unit tests before submitting a pull request.

## Documentation
- [NodeJs](https://nodejs.org/)
- [Express](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Mongoose](https://mongoosejs.com/)

## API Endpoints
1. GET http://localhost:3000/ → The client will see the “Hello User!” message which is used to verify that application is working properly.

2. GET http://localhost:3000/subscribers → When the user hit this, **endpoint /subscribers**, the client will **get an array of all subscribers in JSON format** from the database where the data is stored in local MongoDB database.

3. GET http://localhost:3000/subscribers/names →When the user hit this, endpoint **/subscribers/names** the client will to get an array of all subscribers in JSON format with **only name and subscribed Channel fields** from the database, where the data is stored in local MongoDB database.

4. GET http://localhost:3000/subscribers/:id → When the user hit this, endpoint **/subscribers/:id** in ID, the user needs to enter the USER’S ID which is stored in the database to get a particular **user’s details like name, subscribed Channel and subscribed Date** from the database, where the data is stored in local MongoDB database.

5. GET http://localhost:3000/subscribers/:id → When the client gives **incorrect USER’S ID instead of correct USER’S ID** (where the ID does not match) which is stored in database, the **Client will get an Error message like“ Subscriber doesn't exist with the given _id: sdijvrbv” in JSON format with 400 error status code.**

6. GET http://localhost:3000/something → when the user hit the unwanted route which is not mentioned above (which is used to handle all other requests), they will get an error message like Route not found in JSON format with an 404 error status code.



## Demo
[Click here to Visit Site](https://get-you-tube-subscribers-alma-better-hd4c-iamnaveensingh.vercel.app/).


## Badges

[![Node.js](https://img.shields.io/badge/Node.js-v16.9.1-green.svg)](https://nodejs.org/)

[![Express](https://img.shields.io/badge/Express-v4.17.1-blue.svg)](https://expressjs.com/)

[![MongoDB](https://img.shields.io/badge/MongoDB-v5.1.1-green.svg)](https://www.mongodb.com/)

[![Mongoose](https://img.shields.io/badge/Mongoose-v6.0.9-blue.svg)](https://mongoosejs.com/)

