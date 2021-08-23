# CRUD

- [Home](https://fadnesscharlie.github.io/reading-notes/301/)

## Status Codes Based On REST Methods
1. In your own words, describe what each group of status code represents:
   1. 100’s = Request fails before the page will take in their information
   2. 200’s = Things are working fine
   3. 300’s = When something is not directing them the right way
   4. 400’s = Error from the user
     1. 404 =  Could not find something
   5. 500’s = Error from our side
2. What is a status code 202?
   1. Accepted
3. What is a status code 308?
   1. Redirecting the URL to correct site
4. What code would you use if an update didn’t return data to a client?
   1. a 204 code
5. What code would you use if a resource used to exist but no longer does?
   1. 404
6. What is the ‘Forbidden’ status code?
   1. 403

## Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
   1. We want it to be different because it links to our local host.
2. What is middleware?
   1. Code that runs when the server get a request but before it gets past to your routes.
3. What does app.use(express.json()) do?
   1. Lets the server accept JSON as a body inside of a post or get element
4. What does the /:id mean in a route?
   1. Route with a parameter
5. What is the difference beween PUT and PATCH?
   1. Patch will update whatever information is passed, but put will update everything along with whatever information is passed.
6. How do you make a defalut value in a schema?
   1. Create a JSON formattted with new mongoose.Schema({})
7. What does a 500 error status code mean?
   1. Error on our side
8. What is the difference between a status 200 and a status 201?
   1. 200 means everything worked, and 201 means we successfully updated something

## Resources

- [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)
- [Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

## Things I want to know more about

- 

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
