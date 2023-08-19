# File Metadata Microservice

Build a full stack JavaScript app that is functionally similar to this: https://file-metadata-microservice.freecodecamp.rocks.

This code sets up a Node.js application using the Express.js framework to handle file uploads and analysis. It utilizes the multer middleware to process file uploads. Here's a breakdown of the code:

Module Imports:

The express, cors, dotenv, and multer modules are imported.
The dotenv module is used to load environment variables from a .env file.
Express Application Initialization:

An instance of the Express application is created using express().
Middleware Setup:

CORS middleware is used to enable Cross-Origin Resource Sharing.
The application serves static files from the "public" directory using the /public route.
The /views directory is used to serve the "index.html" file.
File Upload and Analysis API Endpoint:

An API endpoint (/api/fileanalyse) is created to handle POST requests for file uploads and analysis.
The upload middleware from multer is used to process the uploaded file. It's configured to handle files uploaded with the field name 'upfile'.
In the callback function, the response is sent with JSON containing information about the uploaded file:
name: The original name of the uploaded file.
type: The MIME type of the uploaded file.
size: The size of the uploaded file in bytes.
Server Listening:

The server starts listening on the port specified in the process.env.PORT variable or on port 3000 if not provided.
A message is logged to indicate that the server is running and listening on the specified port.
In summary, this code creates a simple file upload and analysis service using Node.js, Express.js, and the multer middleware. Users can upload a file using the API endpoint, and the server responds with information about the uploaded file, including its name, type, and size.
  
# Solution Challenge
In this challenge I tried to get as close as possible to your solution:
- Live Site URL: [Replit](https://replit.com/@AndresF-Sanchez/boilerplate-project-filemetadata)

# Author

- Author - [@AndresF-SanchezG](https://github.com/AndresF-SanchezG)
- School - [Freecodecamp](https://www.freecodecamp.org/)
- Curse - [File Metadata Microservice](https://www.freecodecamp.org/learn/back-end-development-and-apis/back-end-development-and-apis-projects/file-metadata-microservice)






