# Project1

Blogifier 
Blogifier is travel blog app that makes it easy to discover new travel destinations with travel stories submitted by people who have been there. The user can read the blog posts submitted by other users or my create their own posts. If the user chooses to create a post, they are required to register as a user. Users also may search the existing posts by location or author.

-----------------------------------------------------

This project was created as a group assignment for the Coding Bootcamp at U of MN.

Its contributors include:

Nick Arnold
Drew Brooksbank
Dave Farnick
Jon Hernandez
Bowie Sessions
Tasha Shrader

-----------------------------------------------------

Technologies Used:
HTML
CSS
Sequelize
MySQL
MySQL2
Passport.js
Express
Axios
bcrypt-nodejs
JavaScript
Heroku

-----------------------------------------------------

See the deployed app at:
https://blogifier.herokuapp.com/

-----------------------------------------------------

DOCUMENTATION for Passport.js

Passport is authentication middleware for Node.js. It can be unobtrusively dropped in to any Express-based web applicationIt results in authentication using a username and password.

Despite the complexities involved in authentication, code does not have to be complicated.

app.post('/login', passport.authenticate('local', { successRedirect: '/',
                                                    failureRedirect: '/login' }));
Install
$ npm install passport
Authenticate
Authenticating requests is as simple as calling passport.authenticate() and specifying which strategy to employ. authenticate()'s function signature is standard Connect middleware, which makes it convenient to use as route middleware in Express applications.

app.post('/login',
  passport.authenticate('local'),
  function(req, res) {
    // If this function gets called, authentication was successful.
    // `req.user` contains the authenticated user.
    res.redirect('/users/' + req.user.username);
  });
By default, if authentication fails, Passport will respond with a 401 Unauthorized status, and any additional route handlers will not be invoked. If authentication succeeds, the next handler will be invoked and the req.user property will be set to the authenticated user.
-----------------------------------------------------

![screen shot 2019-02-14 at 12 36 52 pm](https://user-images.githubusercontent.com/46514256/52810195-a335a280-3057-11e9-9a29-f1168def1dd6.png)
![screen shot 2019-02-14 at 12 37 10 pm](https://user-images.githubusercontent.com/46514256/52810196-a335a280-3057-11e9-898d-856e930f875b.png)
![screen shot 2019-02-14 at 12 38 06 pm](https://user-images.githubusercontent.com/46514256/52810197-a335a280-3057-11e9-9671-f5bc59b7f885.png)

