#### Which of below is true about Monoliths

	a. Monoliths have multiple services (process), independent of each other
	b. Have separate individual databases specific to service
	*c. Are regid and slow for making new changes
	d. Fully automated testing
	e. Often developed by smaller teams
	
#### Which of below will solve problems posed by the Monoliths

	a. Part & Whole (separation of concerns)
	b. Single Responsibility Principle
	c. Decoupled & Distributed systems
	d. Design by contract
	*e. All of the Above

#### Which of below concepts are applied in design & implementation of Microservices

	a. Separation of Concerns
	b. Single Responsibility Principle
	c. Service Oriented Architecture
	d. Design by contrast
	*e. All of the Above

#### Identify most important benefit of Microservices way of implementing

	a. Independent, Isolated & Automated testing of componentized services
	b. Can release each services independently
	*c. Independently evolve the service
	d. Can be managed by smaller team
	e. None of the Above

#### Which of below will not qualify to be a Microservice

	a. Distributed services (multiple service, which can run independently as different process)
	b. Share common database for greater denormalization and lower data redundancy
	c. Lower cohessions among services
	d. Share similar philosophy of "single responsibility" principle
	e. None of the Above

#### Which of the below ways can be used for Communication

	a. Event Driven
	b. Message Driven
	c. API
	d. Orchestrated
	e. All of the Above
	f. None of the Above
	
#### Which of below will constraint a service to independently evolve

	a. Shares same data model with other services
	b. Directly access databaes of other services
	c. Maintains replica data of specific entities and synchronizes whever same is modified in other services
	d. Has its own user authentication
	*e. All of the Above
	f. None of the Above
	
#### Which of below will liberate a service to independently evolve

	a. Identifying a well defined bounded context
	b. Gathering the responsibilities or business capability, which change for same reason
	c. Allowing redundant metadata, which otherwise need to cross bounded ccontext 
	d. Separating out other concerns and carefully controlling/reviewing scope creep
	*e. All of the Above
	f. None of the Above
	
#### Which of below are benefits of Microservices

	a. Manageable by smaller team
	b. Can replace easily & completely
	c. Polyglot tech stack
	d. Extensible by adding new services
	e. Can scale only those which have higher load
	f. All of the Above
	
#### Which of below are overheads of Microservices

	a, Polyglot tech stack (Programming languages, Technologies, Databases)
	b. Need to automate Build, Test & Deployment
	c. Need to design for tolerating failure of service
	d. Need to monitor services for failures, zombie services
	*e. All of the Above
	f. None of the Above

#### Which of below is true regarding Bounded Context

	a. Is a logical runtime boundary for the service
	b. Is a tangible or physical implementation boundary
	c. Manifests Database schema/structure, code base or code repository to create a boundary
	d. Avoids confusion among team members by clearly defining applicability of domain model to the service
	*e. All of the Above
	f. None of the Above
	
#### Which of below refer to “micro” in Microervices

	a. Independent system of smaller complexity
	b. Two pizzas are enough to feed the team
	c. Can release(deploy, distribute) Independently
	d. Another service cannot write or read data of another service
	e. All of the Above
	f. None of the Above

#### Considering a eCommerce system, which of below is not a Microservice

	a. Product catalog & Shopping cart
	b. Orders & Shipping
	c. Customer & Subscriptions
	d. All of the Above
	e. None of the Above
	
#### When you should avoid Microservice

	a. Technology diversity has to be avoided
	b. The system is lot more simpler to implement & understand as monolithic
	c. The system has to be deployed on a limited infra as a single unit
	d. Eventual consistency is not acceptable (CAP Theorem is not applicable)
	e. Not enough independent responsibilities
	f. All of the Above

#### Which of below refers to or is true regarding "Stateless Microservice"

	a. Which is not a "Stateful Microservice"
	b. Which has no persistence layer
	c. Does not share database with other service
	d. All of the Above
	e. None of the Above
