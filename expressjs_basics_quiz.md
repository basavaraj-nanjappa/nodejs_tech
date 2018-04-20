## Building Webserver using express

### The ________ object has properties that are local variables within the application.

    a. app.use
    b. app.store
    *c. app.locals
    d .app.storage

### app.all() is like the standard app.METHOD() methods, except it matches all HTTP Get requests.

    *a. false
    b. true

### Which of below will parse and return route parameters?

    a. req.query.params
    b. req.query
    *c. req.params
    d. req.body
    e. None of the Above

### Select correct route parameter formats?

    *a. users/:userId/address/:addressId
    b. users/%!@userId/
    c. users/?*!userId
    d. all Of above

### How many number of callback functions can be assigned to handle a request in the route?

    a. one
    b. four
    *c. Unlimited
    d. two

### How can we create chainable route handlers for a route path in ExpressJS?

    a. app.router()
    *b. app.route()
    c. app.routing()
    d. Non of the Above

### Which one is correct for routing in express?

    a. It refers to functions that have access to the request object.
    b. It refers to all callback functions those are executed on a particular request.
    *c. It refers to determining how an application responds to a client request to a particular endpoint
    d. None of above

### Which task performed by Middleware functions?

    a. Execute any code.
    b. Make changes to the request and the response objects.
    c. End the request-response cycle.
    d. Call the next middleware function in the stack.
    *e. All of Above


### Which one is correct implementation of error handler in expressjs?

    *a.
```javascript
function errorHandler (err, req, res, next) {
  if (res.headersSent) {
    return next(err)
  }
  res.status(500)
  res.render('error', { error: err })
}
```

    b.
```javascript
function errorHandler (req, res, err) {
  if (res.headersSent) {
    return next(err)
  }
  res.status(500)
  res.render('error', { error: err })
}
```

    c.
```javascript
function errorHandler (err) {
  if (res.headersSent) {
    return next(err)
  }
  res.status(500)
  res.render('error', { error: err })
}
```
    d. None of the Above

### To serve static files such as images, CSS files, and JavaScript files, Which one will be used in Express.

    a. static.express()
    b. path.join()
    *c. express.static()
    d. All of them
    e. None of above

### Route handlers can be in the form of a function, an array of functions, or combinations of both

    *a. true
    b. false
    c. It depends

### __________ Use the  class to create modular, mountable route handlers.

    a. app.route()
    b. express.route()
    *c. express.Router()
    d. router()

### Which one is the built in middleware in expressjs?

    a. express.router()
    b. router.route()
    c. router.use()
    *d. express.urlencoded()
    e. All of the above

### The _______ function is a top-level function exported by the express module.

    a. Router()
    *b. express()
    c. both
    d. None of above
    e. All of them

### Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.

    *a. true
    b. false

