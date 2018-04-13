## NodeJS Architecture

### Which of below is not part of NodeJS Architecture

	a. In built JS Modules
	b. Chrome V8 JS Engine
	*c. Express.js Framework
	d. OpenSSL Library
	e. None of the Above

### Which is not true about "Single threaded model" in NodeJS

	a. Irrespective of incoming request, there will be only one main thread to accept the request and return response
	b. All computing expressions are executed or processed by only one main thread
	c. Only one thread which executes instructions from the call stack
  *d. Due to single thread, only one request is processed at a time, hence it will block concurrent requests
  e. NodeJS process has only one thread running in it

### Which of below method is helpful to execute code explicitly on event loop

	a. setImmediate
	b. setInterval
	c. setTimeout
	d. process.nextTick
	*e. All of the Above

### Which of below is not true regarding I/O calls

	a. Slow due to device clock speed
	*b. Non-blocking due to CPU
	c. I/O calls are always blocking call, unless a library abstracts it to be asynchronous
	d. Traditionally, I/O calls are handled synchronously
	e. None of the Above

### Which of below are not true in NodeJS

	a. Blocking I/O calls are a problem, Asynchronous handling is a correct way to do it
	b. Is designed to handle large concurrent requests
	c. Uses only one CPU core, hence having multiple core is not natively effective
	d. Provides efficient Javascript compilation and execution
	*e. None of the Above

### Which of below is responsible for efficient execution of JavaScript code in NodeJS

	a. Event Loop
	b. Worker Threads
	c. NodeJS Bindings
	*d. Chrome v8 JS engine
	e. All of the above

### Which of below is not correct in case of handling Asynchronous execution

	a. Try/Catch is not effective
	b. Callbacks with out error first argument is not useful
	c. Callbacks with the error first argument is not useful
	d. Try/Catch in callback is not effective

### Made a asynchronous I/O call, which never returned, which of below helps handle it

	a. Wrap the I/O call with try/catch block
	b. Use callback with error as first argument
	c. Use callback with error as last  argument
	d. Throw error from callback method passed to asynchronous method
	*e. None of the above

### Identify the Computation expression from below

	a. const fs = require('fs');
	b. if(fs === undefined) { console.log('Oops.!'); }
	c. while(fs.read()) { console.log('Reading..!'); }
	*d. (a, b) => math.pow(a, b)
	e. None of the above

### Which of below is not useful in handling Asynchronous method calls

	a. Promise
	b. callback
	d. async
	e. await
	*f. None of the above
