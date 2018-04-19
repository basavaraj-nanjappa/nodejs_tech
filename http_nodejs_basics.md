## Building Webserver using Nodejs

### Which of the following statement(s) are true about the C10M problem?

      I It can be solved using nodejs as a webserver.
     II App developer has to optimize the code and deployment, even if nodejs is used as a server.
    III Only one machine is enough to handle the request, we can scale it vertically.
     IV Multiple machines sitting behind a load balancer is required, we scale it horizontally.

    a. All the statements are true
    b. I, II
    *c. II, IV
    d. IV

### Which statement is true about a Web Server?

    a. It communicates over HTTP protocol.
    b. Nodejs alone can be used as a web server in production deployment.
    c. Web server is used to serve static resources (HTML, pdf, images)
    d. b and c are true
    *e. only b is false, rest are true

### A web page keeps on loading, without any end, then the request times out, what could be the reason. Assume, there is no network error.

    a. There is some internal server error.
    *b. Request - Response cycle in not ended. (res.end is not called explicitly)
    c. Database connection error.
    e. Its a invalid request
    d. None of the above

### What does the status code 500 signify?

    a. Route not found
    b. Network error
    *c. Internal server error
    d. Unauthorized access

### What is true about a Request Handler?

    a. It's a middleware function
    b. It bootstraps the server to listen on a particular port
    c. It has access to the request and the response objects
    *d. All of the Above
    e. Only a and c

### How to handle errors when starting a node server?

    a. Using try/catch blocks
    b. Using Error callbacks
    *c. By listening to 'error' event on server
    d. By listening to 'connection' event on server

### Which of below npm module can be used for testing URL end points in Nodejs?

    a. mocha
    b. superagent
    *c. supertest
    d. chai

### Given a url, `http://www.my-awesome-webapp/myfiles?name=abcd&city=xyz`, and nodejs url module, how'll you get hold of query strings, name and city?

    *a. url.parse(req.url, true).query
    b. url.parse(req.url, false).query
    c. url.parse(req.url, true).pathname
    d. url.parse(req.url, false).pathname

### Which of below is a invalid HTTP response code

    a. 404
    b. 304
    c. 204
    d. 104
    *e. 004

### Given a URL end point `http://example.com/employees/1092/certificates`, identify possible URL parameter in the end point

    a. employees
    b. 1092
    c. certificates
    *d. All of the Above
    e. None of the Above

### Which one of below listed module is useful in developing web services in NodeJS

    a. `url`
    b. `querystring`
    c. `http`
    d. 'https'
    *e. All of the Above

### Given below code, which URLs or the end points are matched, are sure to receive response with status code 200

```javascript
const http = require('http');
http.createServer((req, res) => res.end(' Thank you ')).listen(3000);
```

    a. curl -v -X GET http://localhost:3000/example/one
    b. curl -v -X POST "http://localhost:3000/example/two?un=john"
    c. curl -v -X PATCH "http://localhost:3000/example/three?un=john&pw=loginifucan"
    d. curl -v -X DELETE "http://localhost:3000/example/four?un=john&pw=loginifucant&tk=ADF72348aSDFAew9132sD492"
    e. curl -v -X PUT "http://localhost:3000/example//five?un=john&pw=loginifucant&tk=ADF72348aSDFAew9132sD492&q=_"
    *f. All of the Above

### What is the version of HTTP protocol in use today ?

    a. HTTP v1.0
    *b. HTTP v1.1
    c. HTTP v1.2
    d. HTTP v2.0
    e. HTTP has no version

### Which of below statement is true

    a. URL end points can be tested by checking status code
    b. URL end points are manually tested, not able to automate
    *c. Web services require extensive test automation, hence TDD is a best thing to follow
    d. Web services use HTTP protocol hence no need to test as response code are clear indication of status

### Which of below cannot be developed in NodeJS web server

    a. Image uploading
    b. Live streaming of videos
    c. Chat Bots / Voice Driven Bots
    d. Static web sites
    *e. Coffee vending machine

