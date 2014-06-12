### Comprehension Questions: 

Comprehension Questions

1. What is CORS?
	- Cross origin resource sharing? Cross Site HTTP Request
	
1. What are the three phases of an HTTP session?
	- handshake (open connection)
	- send request
	- received response

1. What are the three components of an HTTP request?
	- http version, method, path( absolute url but no domain)
	- headers on subsequent lines end with empty line
	- optional data block (for post usually)

1. What is an HTTP status code?
	- the status of the server performing the request e.g. errors, success

1. What is the schema for an HTTP response object?
	- http version (confirmation), status
	- response headers
	- response body

1. What are the different HTTP methods?
	- GET, HEAD, POST, DELETE, PUT, PATCH, OPTIONS(* cors), TRACE, PROPFIND, CONNECT

1. What is an idempotent method? Which HTTP methods are idempotent?
	- always has same side-effects: HEAD, GET, PUT, DELETE. (PUT creates and replaces if exists, DELETE removes)

1. What are headers?
	- options specifying data information, caching, cookie data, types, etc...
	- additional information
		- general, request, response, entity, end-to-end, hop-by-hop







1. What is an XHR object?
	- represents an AJAX connection request
	- XmlHttpRequest, an API

1. Is XHR only for getting XML data?
	- No, almost anything: mainly JSON, XML, HTML.
	- also can be HTTPS, FILE, FTP, etc…








1. What does REST stand for and mean?
	- representational state transfer

1. What are the six constraints for REST resources?
	- client server
		- uniform interface links them
	- stateless
		- server contains no client state, it's on client
		- self descriptive messages
		- OAuth2 isn't stateless but RESTful
	- cacheable
	- layered system
		- client can't assume
		- intermediaries between client and server
		- more scalable
	- code on demand (optional)
		- transfer logic to client
		- server can extend client by sending logic
	- uniform interface
		- HTTP verbs, URIs, HTTP Response

1. Give an example of a "sensible" resource name.
	- gentlemen

1. How do the GET, POST, PUT, and DELETE HTTP methods relate to REST resources?
	- CRUD
	- Create = POST
	- Read = GET
	- Update = PUT
	- Delete
