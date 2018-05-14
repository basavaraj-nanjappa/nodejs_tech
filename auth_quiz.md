Authentication & Authorization

### Which of below, we don't have to deal in building applications for users

    a. Identification
    b. Authentication
    c. Authorization
    *d. All of the Above
    e. None of the Above

### Authentication is what ?

	a. Match password of the user
	*b. Verify and confirm the identity of the identify claim
	c. Algorithm to decrypt and match password
	d. None of the Above

### Which of below is not a `type` of `Authentication`

	a. Single factor authentication
	b. Two factor authentication
	c. Multi factor authentication
	d. Single Sign-on
	*e. One time password OTP

### Which of below is not used for integrating Identification process

	a. OpenID
	b. OAuth
	c. SAML
	d. Auth0
	*e. Username & Password

### Which of below types of authorization can be set using `Authorization` header

	a. Basic
	b. Bearer
	c. Digest
	*d. All of the Above
	e. None of the Above

### Which of below are part of JWT Token

	a. Header
	b. Payload
	c. Signature
	*b. All of the Above
	c. None of the Above
	
### Why is it useful to use of Token based authentication

	a. Compact
	b. Self-contained
	c. Authentication process can be stateless
	d. Fits both user based and system based authentication scenarios
	*e. All of the above
	

### What is PassportJS in the context of NodeJS

	a. Library for flexible authentication mechanism
	b. Authentication middleware
	c. Extensible to various authentication types & ways
	*d. All of the above
	e. None of the above
	
### Which of below are alternatives to PassportJS

	a. Custom developed authentication mechanism
	b. Auth0
	c. Using the `jswonwebtoken' module or library
	d. All of the Above
	e. None of the Above

### Which of below can be set on JWT Token

	a. A private key or secret
	b. expiration time
	c. Issuer address
	d. Issued time
	e. All of the above

### Which of below is not a valid strategy in PassportJS

	a. Passport-local
	b. Passport-OAuth2
	c. Passport-custom
	d. Passport-github
	*e. Passport-basic
	
### Which of below headers should be disabled or controlled

	a. X-XSS-Protection
	b. X-Powered-By
	c. Referrer-Header
	d. Strict-Transport-Security
	*e. All of the Above
	f. None of the Above
	
### Which of below status codes are used for Authentication status of API

	a. 401
	b. 403
	c. 407
	*d. All of the Above
	e. None of the Above

### Which of below refers to Authorization

	a. Controlling of the access to resources
	b. Role based access control
	c. Checking the grants of the access on a resources
	d. All of the Above
	e. None of the Above


### Which of below is correct way to chain the PassportJS middleware for authentication

	a. Simply by adding middleware before the handler method

```javascript
app.post('/login', passport.authenticate('local'), (req, res) => res.send('Successfully authenticated'));
```

	b. By registering a custom callback for the strategy
```javascript
app.post('/login', function(req, res, next) {
  passport.authenticate('local', function(err, user, info) {
    if (err) { return res.send('Error in authentication') }
    if (!user) { return res.send('User does not exists'); }
    return res.send('Successfully authenticated');
  })(req, res, next);
});
```

	b. Simply specify the routes to redirect to after the authentication
```javascript
app.post('/login', passport.authenticate('local', { successRedirect: '/', failureRedirect: '/login' }));
```

	*c. All of the Above
	d. None of the Above
