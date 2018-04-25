### Which of below characters should NoSQL databases fulfill

	a. No relational constraints
	b. Support partitioning, replication or Distributed database management
	c. Fit into CAP Theorem
	*d. All of the above
	e. None of the above

### Which of below is false about Relational databases

	a. Support relational constraints
	b. No easy support for partitioning, replication or Distributed database management
	c. Cannot fit into CAP Theorem
	*d. Consistency is not guaranteed
	e. None of the above

### Which of below feature is not provided by MongoDB

	a. In-memory storage model
	b. Timed expiration of data (Time To Live or T.T.L)
	b. Sharding of data
	c. Composite indexes
	*d. decentralized database

### Which of below is true about `Scheamless` character of NoSQL databases

	a. Very less schema is used
	b. Data is unstructured
	*c. Data structure is dynamic
	d. Schema is undefined
	e. All of the above

### What type of NoSQL database is MongoDb ?

	a. Key-Value pair
	b. Columnar family
	*c. Document oriented
	d. Graph database
	e. None of the Above

### Which of below key is valid in MongoDB

	a. Primary Key
	*b. Unique Key
	c. Foreign Key
	d. All of the above
	e. None of the above

### Which of the below statement(s) is TRUE about CAP theorem

	a. In case of a network partition, consistency can't be guaranteed but availability can.
	b. Consistency is always maintained regardless of a network partition.
	c. Availability takes precedence over consistency in case of a network partition.
	*d. Ony one out of the two, consistency or availability, can be guaranteed in case of network partition
	e. None of the above

### Who gets to decide which parameter, either consistency or availability, should be given more precedence over the other?

    a. Database Administrators
    b. Developers
    *c. Business requirement
    d. All of the above
    e. None of the above

### Mark the statement(s) which is closest to being TRUE.

	a. Relational databases will be completely replaced by NoSQL databases in the future.
	b. NoSQL databases can't offer us ACID, hence not good for transaction based apps.
	c. Polyglot databases are the future of app development.
	d. All the statements are true.
	*e. Only b & c

### In which of below use case, you'd choose a NoSQL database like MongoDb

	a. You want a rapid time to market.
	b. Your app is data heavy (large size of data)
	c. You want a quick prototype, poc.
	*d. All of the above

### Which of below does not belong to MongoDB

	a. Collection
	b. Document
	c. Field
	d. Index
	e. All of the Above
	*f. None of the Above

### Which of below is a valid reason to create a separate collection for the sub-document instead of flattening in the document

	a. Sub-document will be used very rarely
	b. Number of fields in Sub-document is more
	*c. Embedded sub-document size or growth is larger than, document size or growth
	d. Sub-document has a required field
	e. None of the Above

### Which of below method is invalid regarding insert

	a. db.exampleCollection.insertOne
	b. db.exampleCollection.insertMany
	*c. db.exampleCollection.insertAll
	d. db.exampleCollection.insert
	e. None of the above

### Which of below method is invalid regarding update

	a. db.exampleCollection.updateOne
	b. db.exampleCollection.updateMany
	*c. db.exampleCollection.update
	d. db.exampleCollection.fineOneAndUpdate
	*e. None of the above

### Which of below is valid about terminal command can be used for backup related tasks in MongoDB

	a. mongodump
	b. mongoimport
	c. mongoexport
	d. mongorestore
	*e. All of the above

### Which of below is considered bad practice regarding securing mongodb

	a. Not setting up Authentication
	b. Running mongodb with default port
	c. Exposing mongodb to Internet
	d. Not backing up database
	*e. All of the above

### Which of below helps paginate the results from mongodb

	a. db.exampleCollection.find().return(`<number of records to return>`)
	b. db.exampleCollection.find().limit(`<number of records to return>`)
	*c. db.exampleCollection.find().skip(`<number of records to skip>`).limit(`<number of records to return>`)
	d. db.exampleCollection.find().page(`<number of records to skip>`, `<number of records to return>`)
	e. Pagination is not supported in MongoDB

### Which is TRUE about Data modeling in MongoDb?

	a. De-normalization is preferred over normalization
	b. Data modeling is done based on use case and nature of queries
	c. Referencing data is preferred if a field or sub document has higher cardinality
	*d. All of the Above
	e. None of the Above

### Which of below is TRUE regarding MongoDB

	a. Storing petabytes of data on a single machine is recommended for faster reads
	b. USe stored procedures for better query performance in MonoDB
	*c. MongoDB guarantees consistency at a specific document level
	d. None of the above

### Which of below Transaction model is usually adopted in NoSQL database based systems

	a. ACID
	b. SALT
	*c. BASE
	d. All of the Above
	e. None of the Above
