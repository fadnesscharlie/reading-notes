# Bearer Authorization

- [Home](https://fadnesscharlie.github.io/reading-notes/401/)

## Review, Research, and Discussion

1. Write the following steps in the correct order:
   - Register your application to get a client_id and client_secret
   - Ask the client if they want to sign in via a third party
   - Make a request to a third-party API endpoint
   - Redirect to a third party authentication endpoint
   - Make a request to the access token endpoint
   - Receive authorization code
   - Receive access token
2. What can you do with an authorization code?
   - You can access data but only as a short-lived token
3. What can you do with an access token?
   - Access data, but on a much longer token, in duration of minutes or hours
4. What’s a benefit of using OAuth instead of your own basic authentication?
   - Being able to have more security and know whomever you gave the token to, is who they say they are.

## Document the following Vocabulary Terms

- Client ID
  - A unique means of identification. This can include password, PIN, personal identification or an electronic key.
- Client Secret
  - A secret that is only known to your application and the authorization server. This is to prevent client impersonation.
- Authentication Endpoint
  - Also known as device authentication, is another authentication at the end point, making sure the end point connecting device is verified as well, is also who you wanted to connect to, and acts like a two-part authentication
- Access Token Endpoint
  - Where the API creates a request, it verifies the endpoint with an access token
- API Endpoint
  - The end point of server or service
- Authorization Code
  - A code that lets you have access to certain data or services
- Access Token
  - Token-based authenication to allow an application to access an API

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   - Tokens
   - Authenication
   - Authorization
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   - Auth in general
   - Incorporating this with what we already have
   - How to make your applications more secure, and how it might not be secure
3. What are you most excited about trying to implement or see how it works?
   - Incorporating Auth into our application and differnet methods

## Resources

- [JWTs Explained](https://www.youtube.com/watch?v=926mknSW9Lo)
- [Intro to JWT](https://jwt.io/introduction/)
- [Are JWTs Secure?](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)

## BookMark/Skim

- [npm jsonwebtoken docs](https://www.npmjs.com/package/jsonwebtoken)

## Things I want to know more about

- Auth

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
