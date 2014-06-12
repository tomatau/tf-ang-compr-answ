1. What is client side routing?
	- use of the push state and browser url history
	- also using hash symbols in urls to change pages, angular uses /#!/ as it is a convention for SEO

1. Why do Angular apps typically listen to URLs prefixed routes are prefixed with a hash (#) or hash bang (#!)?
	- so that the page doesn't refresh and when push state isn't supported by all potential customers

1. What do you need to do to include ngRoute in your application?
	- as routing is no longer provided by default so it must be injected
	- to gain access to the $routeProvider, $routeParams and $route

1. What is the syntax for defining a route?

```javascript
$routeProvider
.when('/some-route/:param', {
	template: 'Stuff',
	controller: 'BobCtrl as bob',
	resolve: function(){
		return 'Need this string!';	}})
```

1. What's the difference between the template and templateUrl properties in the route config object?
	- templateURL specifies the address the template file
	- template specifies the template string to display at the said URL

1. How do you detect variables in URLs in Angular?
	- :var[?]
	- prefix with : to denote a named param
	- suffix with ? to denote optional

1. What is the purpose of the resolve property in the route config object?
	- to force dependencies to resolve before the route is displayed
	- these resolve properties can then be injected into the controller

1. What does the $location service let you do?
	- modify the (#) location of the url (the route)
	- by use of the path function

1. What is the purpose of the .otherwise() method on the $routeProvider service?
	- a fallback method to catch any routes that haven't been specified

1. How can you alias your controllers using ControllerAs syntax?
	- ng-controller="Controller as c" inside a template
	- controller: 'Ctrl as c' inside route config

1. What is $templateCache?
	- a storage for the templates that have been loaded already so we can refetch them quickly