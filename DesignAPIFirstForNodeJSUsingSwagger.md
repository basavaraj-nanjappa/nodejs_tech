# Design APIs first using Swagger
Think APIs first, design micro-services better

APIs enable interoperability, which is a key ask in modern cloud ecosystems. Though we will discuss with example in Node.js, this is easily applicable to other tech stacks

### Why is it important to think API first
- Shifts think about design of backend as a participating service in the ecosystem, instead of monolith
- Encourages `Design by Contract` and helps parallel development cycles
- Effective to understand, communicate, review with your stake holders
- Directs towards, thinking about experience of user
- Testable APIs from the beginning

### Ho to do it
Follow these steps

1. **Design APIs**

	- Semantically define `URI` signature (`HTTP Method`, `Path`, `Path variables`)
	- Identify `query parameters`, `request body structure`
	- Identify expected `Response` (`success`, `business exceptions`, `errors`)

2. **Test APIs with Mock data**

	- Generate test cases for APIs
	- Try out APIs with Mock or sample data
	- Identify different possible sample data

3. **Review with stake holder by publishing API Document**

	- Publish documented APIs to stake holders, along with mock data or sample data
	- Give your stake holder a playground to try out APIs
	- From here, you can iterate `Step #1` through 3, if you have not yet got them correct

4. **Implement APIs**

	- Use MVC architecture and implement the APIs
	- Continuously test APIs using the same test cases generated during `step #2`
	- Deploy them for your stake holders to try, use and provide feedback
	- From here, you can iterate `Step #1` through 4, if you have not yet got them correct

