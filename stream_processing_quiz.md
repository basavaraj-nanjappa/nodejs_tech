## Stream Processing

#### Which of below are benefits we get using Stream processing

	a. Low memory footprint by the application
	b. Consistent way for Asynch & Synch processing
	c. Faster processing of the data
	d. Can handle large amount of data with ease
	*e. All of the Above

#### Which type of stream is not supported in NodeJS

	a. Readable Stream
	b. Writable Stream
	c. Duplex Stream
	d. Transform Stream
	*e. None of the Above

#### In NodeJS Streams are implemented using which of below

	a. Memory Buffers
	b. Event Loop
	*c. EventEmitters
	d. Promises
	e. Callbacks

#### Which of below scenario is not suitable for use of Stream processing

	a. Identifying anomaly in IoT device data
	b. Real time forex spread calculation
	c. ETL of huge data from file storage to Database
	*d. All of the Above
	e. None of the Above

#### Which below statement best defines Streams

	a. Stream is a buffer of contentious flow of Data
	b. Data distributed over memory space
	*c. Data distributed over time
	d. All of the Above
	e. None of the Above

#### Which of below statement is true about `HighWaterMark` in the context of Streams in NodeJS

	a. The amount of data potentially buffered by stream depends on the `HighWaterMark`
	b. `HighWaterMark` can be set by passing as option to streams constructor method
	c. For streams in Object Mode `HighWaterMark` is the number of Objects to buffer
	d. For normal streams `HighWaterMark` is the number of bytes to buffer
	*e. All of the Above

#### Which of below scenarios is possible using Streams

	a. Read from file as stream and pipe to another file
	b. Read incoming API request as stream and return response as Stream
	c. Read data from Databases as stream
	d. Add processing pipes to data stream in extensible way
	*e. All of the Above

#### Which of below statement is false about Duplex and Transform streams

	a. Has a separate buffer for reading data
	b. Has a separate buffer for writing data
	*c. Has only one buffer for reading and writing data
	d. None of the Above

#### Which of below event is not supported by Writable Streams in NodeJS

	*a. Event `data`
	b. Event `drain
	c. Event `pipe`
	d. Event `unpipe`
	e. Event `finish`

#### Which of below event is not supported by Readable Streams in NodeJS

	a. Event `data`
	b. Event `end`
	c. Event `error`
	*d. Event `cork`
	e. Event `redable`

#### Which of below event is not supported by Duplex Streams in NodeJS

	a. Event `data`
	b. Event `drain`
	c. Event `error`
	*d. Event `destroy`
	e. Event `unpipe`

#### Which of below statement is false about Streams

	a. Reads data as chunks
	b. Handles back pressure
	c. Can pause and resume stream operation
	d. Only Asynchronous operations can be performed
	e. Streams can be on Object mode
