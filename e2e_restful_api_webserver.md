## RESTful API Development

#### Which of below can be used to for implementing Grocery ordering system using "Alexa" from Amazon?

	a. By making a telephone call to Alexa
	b. Automating sending email to Alexa
	*c. Developing & Integrating using REST style APIs
	d. By accessing Alexa Database
	e. By linking Grocery system database with Alexa database

#### What we can do with APIs?

	a. Two systems can talk to one another
	b. Two bots can talk to one another
	c. A System and bot can talk to one another
	d. We can enable interoperability with a system
	e. Systems can be extended to interact more with user
	*f. All of the Above

#### Without standardized APIs, what issues we may have to counter?

	a. Integration becomes tightly coupled
	b. Time to integration takes long time
	c. Different code bases to communicate with different clients for same server or visa verse
	*d. All of the Above
	e. None of the Above

#### Which is true about HATEOS in below?

	a. HATEOS is a constraint on REST to enable navigation in client interaction
	b. Uses Hypermedia As The Engine Of Application State
	c. HATEOS makes client have no prior knowledge about REST APIs for interaction
	d. Server can evolve its APIs without informing clients
	*e. All of the above

#### Which of below you will follow in designing APIs for given problem

	a. Analyze and define a Domain Entity Model
	b. Identify all domain entities, including process entities
	c. Try listing all possible type of API requests or Queries to data
	d. Define the correct URI semantics for the identified APIs
	e. Define Input & Response data structure, format
	*f. All of the above

#### Which of below is not an alternatives to REST

	a. RPC, RMI
	b. SOAP
	c. WebSockets
	d. GraphQL
	*e. TCP/IP
	f. All of the Above

#### Which of below is incorrect semantic for Uniform Resource Identifier

	a. GET https://example.com/products/
	b. GET https://example.com/products/:productId/reviews
	c. GET https://example.com/products/:productId/ratings
	d. GET https://example.com/products/:productId/orders
	*e. GET https://example.com/products/:productId/getRatings

#### Which of below is incorrect semantic for Uniform Resource Identifier

	a. GET https://example.com/products/
	*b. GET https://example.com/findProducts
	c. POST https://example.com/products/
	d. PATCH https://example.com/products/:productId
	e. DEL https://example.com/products

#### Which of below are REST principles

	a. Uniform interface for Resources
	b. System follows Client - Server architecture, i.e., server has business logic, client interfaces only and can evolve independently
	c. Server is Stateless, will not store anything about client requests or past requests on server
	d. Resources are Cacheable, either on client side or in the network
	e. Layered system
	f. All of above
	
## Project Structuring

#### Pragmatic project structuring is essential because

	a. Need to breakdown the system into easily manageable components of lesser complexity
	b. Need to minimize coupling & cohesion among components
	c. Many developers have to work together for a complex and/or large systems
	d. Modularity, Consistency and testability reduces learning curve for a new developer of the team
	e. Reduces time to troubleshoot, debug
	*f. All of the Above

#### Organizing your project to proper folder structure should be done when?

	a. During Testing phase
	b. During beta release
	*c. First day of the project and constantly review
	d. Any time of the project
	e. Should not be, as it will become opinionated and against Agile methodology
	f. None of the Above

#### Which of below are characters of Vertical slicing?

	a. Easy for continuous integration and testing
	b. One developer can completely own one module or a component
	c. Can evolve a module or a component independently
	d. All code of a component/module is in one place
	e. None of the Above

#### Separation of concern refers to which of below

	a. Separate request recognizing (matching), parsing from handling of request
	b. Separate business logic steps from orchestration steps
	c. Separate database interaction from business logic
	*d. All of the above
	e. None of the above

## Logging

#### Which one of these libraries is not suitable for handling ERROR logs?

	a. winston
	b. log4js
	c. bunyan
	*d. morgan
	e. None of the above

#### Which of below is a valid reason to use a library for logging?

	a. Using console.log will spam application logs and not useful to diagnose
	b. Logging must be controllable as a config, without any code change
	c. Errors should be logged all the time
	d. Desirable to configure Logging format, file size, rotation of files and name of log files
	e. All of the above

### Which of below is a valid Logging level

	a. TRACE
	b. ERROR
	c. INFO
	d. DEBUG
	e. WARNING
	*f. All of the above

## Application Configurations

#### What is the correct way to set the mongodb url in your application config?
	a. `const MONGO_URL = "mongodb://localhost:27017";`
	b. `const MONGO_URL = (process.env.MONGO_URL || "mongodb://localhost:27017";`
	c. `const MONGO_URL = process.env.MONGO_URL`
	d. All of the above
	e. None of the above

#### Which of below is invalid values conventionally set for `NODE_ENV`

	a. "production"
	b. "development"
	c. "test"
	*d. "local"
	e. None of the above

#### Which of below is a valid about application configuration

	a. All configuration should be in one central place
	b. Application behavior should change according to deployment environment without code change
	c. Hard coded values are recipe for disastrous quality of application
	d. All of the above
	e. None of the above
