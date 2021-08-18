# Authentication

- [Home](https://fadnesscharlie.github.io/reading-notes/301/)

- What is OAuth?
  - Open-standard authorization protocol or framework.
- Give an example of what using OAuth would look like.
  - A website that has multiple pages and while logging on to one page, will give access to other pages
- How does OAuth work? What are the steps that it takes to authenticate the user?
  - By generating tokens that then check with other sites to see if they match the corrisonding token to grant access.
- What is OpenID?
  - "OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans."


- What is the difference between authorization and authentication?
  - Authentication
    - Process of verifying who the user is
  - Authorization
    - Process of verifying what they have access to.
- What is Authorization Code Flow?
  - It is the flow of which the user and page gets authorization to access more information from the web page.
- What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
  - To have more access against more malicious attackers by adding another layer of security they have to go through.
- What is Implicit Flow with Form Post?
  - A way to grant access that your application does not need to keep secret key.
- What is Client Credentials Flow?
  - The application takes the user information they already entered and uses that to get access to other applications.
- What is Device Authorization Flow?
  - Uses a users device as a way of granting a access token for more proof.
- What is Resource Owner Password Flow?
  - When the application saves the username and password on the application itself.

## Resources

- [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)
- [Authorization and Authentication flows](https://auth0.com/docs/flows)

## BookMark/Skim

- [Auth0 for single page apps](https://auth0.com/docs/libraries/auth0-react) 

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
