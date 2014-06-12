### Comprehension Questions: 

Comprehension Questions

1. What is the purpose of the $http service?
	- provides get, post, delete, put requests for cross domain etc.
	- returns a promise

2. What must you include in your query parameters if you want to make a JSONP request using Angular?
	- JSON_CALLBACK as a callback param, some servers have a custom method name e.g. jsonp
	- method is JSONP for the requst

3. If you want to make CORS requests, what do you need to do?
	- set the Xdomain flag
	- remove any custom headers e.g. "X-"