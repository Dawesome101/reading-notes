# CRUD

## Index

[Home](../README.md)  
[Status Codes Based on REST Methods](#status-codes-based-on-rest-methods)  
[Build a REST API with Node.js, Express, and mongoDB](build-a-rest-api-with-node-js--express--and-mongodb)

## [Status Codes Based on REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

1. In your own words, describe what each group of status code represents:  
100’s = Reads the header and tells the client its request has been received.  
200’s = Success!
300’s = Redirects.  Data has moved or isn't present anymore.
400’s = Client errors. Mainly invalid requests
500’s = Server erros. Either too many requests or unreachable proxy.
2. What is a status code 202?
   - Accepted - If the deletion is asynchronous and takes some time, which is the case in distributed systems, it can be appropriate to return this code with some information or URL to tell the client when it will be deleted.
3. What is a status code 308?
   - Permanent Redirect - This is the right code if the resource will now be available at a new URL and the client should directly access it via the new URL in the future. The current endpoint can’t control the clients’ behavior after the request and a subsequent redirect if the resource URL changes again have to be issued from the new URL.
4. What code would you use if an update didn’t return data to a client?
   - 204 No Content - A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.
5. What code would you use if a resource used to exist but no longer does?
   - 410 Gone - This is like 404 but we know that the resource existed in the past, but it got deleted or somehow moved, and we don’t know where.
6. What is the ‘Forbidden’ status code?
   - 403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

## [Build a REST API with Node.js, Express, and mongoDB](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
   - Eventually the server will need to be run on something that is not localhost.  
2. What is middleware?
   - Code that run but before a request gets passed to your route
3. What does `app.use(express.json())` do?
   - Lets our server accept json as a body inside of an element.
4. What does the `/:id` mean in a route?
   - Provides access to whatever is typed in after the first slash (/).
5. What is the difference between `PUT` and `PATCH`?
   - `Put` updates all of the information for the subscriber at once.
   - `Patch` only updates what the user passes.
6. How do you make a default value in a schema?

   ```js
   const subscriberSchema = new mongoose.Schema({
      name: {
         type: String,
         required: true
      }
      subscriberToChannel {
         type: String,
         required: true
      }
      subscribeDate: {
         type: Date,
         required: true,
         default: Date.now
      }
   })
   ```

7. What does a `500` error status code mean?
   - There is an error on the server.
8. What is the difference between a status `200` and a status `201`?
   - `200` means everything was successful.
   - `201` means successfully created an object.

[Back To Top](#index)
