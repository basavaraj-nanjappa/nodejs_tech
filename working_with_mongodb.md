# Working with Data

### Core topics
- Distributed databases & CAP theorem
- NoSQL thinking
- Data modeling with MongoDB (Document databases)
- Working with MongoDB in NodeJS

### CAP theorem
[CAP Theorem](https://en.wikipedia.org/wiki/CAP_theorem)

![CAP](./images/good_cheap_fast.jpeg "CAP Theorem")

- **Consistency** : All participating/processing nodes have same version of data always
- **Availability** : Failure of a participating/processing nodes must not prevent the application from functioning as expected, the healthier nodes should continue processing
- **Partition Tolerance** : Tolerance against network outage/slow/fast, message loss/duplicate/

### NoSQL thinking
Why no SQL, [read here](https://martinfowler.com/articles/nosqlKeyPoints.html)
- No explicit schema definition, it is flexible & implicit (dynamic)
- No relational constraints (why?)
- No stored procedures
- No normalization, mostly flat, redundant (duplicated) data
- No atomic transactions (Atomic, Consistent, Isolated, Durable - ACID), only eventual consistency (Basic Availability, Soft-state, Eventual consistency - BASE)
	- Atomicity of write operation is only to a individual document level, not across documents, collections
	- Redundant data has to be updated by application code
- Horizontal scaling (Replication, Partitioning)

## Data modeling with MongoDB
- Model based on how often your read or write
- De-normalize data model
- Relating documents is not inbuilt, it has to be modeled and handled in Application level
- Use `references` and `embedded documents` to relate the document
- The growth of the relationships determine where to store the reference
- References
	- Referencing relation is recommended for many-to-one relation
	- Link or reference are stored by storing the unique identifier of the referenced documents
		- Eg:
				Collection: user
					{
						name: '',
						email: '',
						status: '',
						friends: [
							{
								email: ''
							},
							{
								email: ''
							},
							{
								email: ''
							},
						]
					}
	- Referenced relation, normalizes the data model hence more DB round trips are needed from application code
- Embed documents
	- related documents by flattening (denormalized) the document
	- This helps query and manipulate the related data in a single Database operation (Atomicity)
	- Query support selecting specific fields only, hence can either omit or select only the embedded document in queries
	- If embedded document constantly grows, then it may be good idea to give it a separate collection
	- Eg: Facebook posts are not good to keep directly under user collection
					Collection: user
					{
						name: '',
						email: '',
						status: '',
						posts: [
							{},
							{},
							{},
							{},
							{},
							{},
						]
					}
	- Redundancy is allowed, apply eventual consistency

### NodeJS & MongoDB
- Connection
	- error handling
	- reconnection

- Query
	- Simple queries
	- Query nested documents
	- Dot notation to access nested documents & elements
		- `<array>.<index>`
		- `<embedded document>.<field>`
	- [Query Documents](https://docs.mongodb.com/manual/tutorial/query-documents/)
	- [Query Embedded/Nested Documents](https://docs.mongodb.com/manual/tutorial/query-embedded-documents/)
	- [Query Array](https://docs.mongodb.com/manual/tutorial/query-arrays/)
	- [Query Array of Embedded Documents](https://docs.mongodb.com/manual/tutorial/query-array-of-documents/)
- Aggregation framework
	- Aggregation [pipeline](https://docs.mongodb.com/manual/reference/operator/aggregation-pipeline/)
	- Wind, Unwind
- Some sample queries
	- `db.products.insertMany([{name: 'iPhone', vendor: 'Apple'}, {name: 'Motog', vendor: 'Motorola'}, {name: "nokia", vendor: "nokia"}, {name: "samsung", vendor: "Samsung"}])`
	- `db.products.updateMany({}, { $set: { spec: { type: 'smartphone' } } } )`
	- `db.products.find({tags: { $all : ['smartphone']}})`
	- `db.products.find({'tags.0':'smartphone'}).pretty()`
	- `db.products.find({code: 'iphone'}).pretty()`
	- `db.products.find({reviews: { $elemMatch: {reviewer: "basav"}}}).pretty()`
	- `db.products.find({"spec.weight": 100}).pretty()`
	- `db.products.find({"spec.weight": { $gt: 100}}).pretty()`
	- `db.products.aggregate([{ $match: { 'spec.weight': { $gt: 100} } }, { $group: { _id: "$code", count: { $sum: 1 } } } ]).pretty()`
	- `db.products.aggregate([{ $match: { 'spec.weight': { $gt: 100} } }, { $group: { _id: "$code", maxPrice: { $max: "$price" } } } ]).pretty()`


- Mongoose
	- Schema definition, indexes
	- Virtual columns
	- Static & Instance methods
	- Validation
	- Query, pagination, sort, embedded documents (array, array of documents)
	- Update One, Update many, Updated embedded document
	- Delete
- Aggregation in code, using async

### References

- [Data Architecture - definition at Wikipedia](https://en.wikipedia.org/wiki/Data_architecture)
- [Database engines ranking and comparison](https://db-engines.com/en/ranking_categories)
- [Conceptual model - is relevant](http://www.vertabelo.com/blog/technical-articles/what-a-concept-is-logical-data-modeling-obsolete)
- [Achieving Usability Through Software Architecture](https://resources.sei.cmu.edu/library/asset-view.cfm?assetID=5605)
- [Database theory](https://databasetheory.org/)
- [CAP theorem in system design](https://medium.com/@noobj/how-we-used-cap-theorem-in-our-system-design-6f2ea82bd229)
- [Agile data modeling](http://agiledata.org/essays/agileDataModeling.html)
- Why [data flow](http://www.dataversity.net/get-value-data-organizations-also-focus-data-flow/) needs focus
- [What is data-flow](https://medium.com/digital-anatomy/what-is-data-flow-5a277d990f48)
- [Don't be data driven](https://medium.com/microsoft-design/if-you-want-to-be-creative-dont-be-data-driven-55db74078eda)
- [Sharded instance deployment](https://dzone.com/articles/composing-a-sharded-mongodb-on-docker)
