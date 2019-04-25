Requirements:
1. Node Module with a `findServer()` function which should return a Promise that either:
a. Resolves with the online server that has the lowest priority number.
b. Rejects with an error, if no Servers are online.
2. HTTP GET requests should be used to determine if a server is online or offline additionally the
following is required:
a. All GET requests should be done simultaneously.
b. A GET request should timeout after 5 seconds.
c. A server should be considered online if it’s response status code is between 200 and
299.
3. Unit Tests are required to sufficiently test all components of your module. Additionally the
following is required for unit tests:
a. All server interaction should be mocked.

Example Server Array:
```json

[
	{
		"url": "http://doesNotExist.boldtech.co",
		"priority": 1
	},
	{
		"url": "http://boldtech.co",
		"priority": 7
	},
	{
		"url": "http://offline.boldtech.co",
		"priority": 2
	},
	{
		"url": "http://google.com",
		"priority": 4
	}
]

```


What is expected from you:
1. A working demo of the module, that meets the above requirements.
2. A working unit test suite for the module, that meets the above requirements.
3. Instructions on how to install and run the demo as well as the unit tests.
What we are looking for:
1. Clearly written comments.
2. Neatly formatted modular code and consistent styling.
3. Demonstration of knowledge on Nodejs.
4. Demonstration of experience in writing structured well organized code.
5. Demonstration of knowledge on Promises (ECMA2015 definition or your favorite Promise
library).
6. Demonstration of knowledge on Unit Testing including experience with mocking target server(s).
