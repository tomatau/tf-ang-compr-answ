## Comprehension Check

1.  What's the purpose of a module?
	- Encapsulation, a form of namespacing for the components that it will container
	- Make a 'wrapper' or 'group up' components such as services, filters, templates, controllers, directives, etc...
	- Also to inject providers/external directives into the module that components may wish to use such as ngRoute, ngAnimation, etc...


2.  What's the syntax for defining a module?
	- <code>angular.module('moduleName', [ 'dependencyN' ]);</code>
	- this will return the module and make it available via <code>angular.module('moduleName'</code>


3.  How do you link a module with an HTML template?
	- include the script that contains the module
	- you can then specify the scope of that module using the ngApp directive as an attribute with a value equalling the name of the desired module. 


4.  Explain the concept of scope. Make sure you can describe what is meant by "parent" and "child" scope.
	- $scope in angular is a key:value storage object that is available within a defined context.
	- $rootScope is available in all contexts as it is the patent.  modules and controllers can also define child scope.
	- $scope also provides a few utility methods for managing events and bindings such as $watch, $on, $broadcast, $apply, etc…


5.  What is a controller?
	- A scope within your application for managing a view
	- it will initialise the state of the view and add some behaviours through dependency injection, declaring functions, etc...
	- Also thought of as a VM or presenter


6.  What's the syntax for defining a controller?

		angular.controller('MyControllerName',
		function(dependencies…, $scope){
			// do stuff
		});


7.  Explain what you do with `$scope` and `$rootScope` in Angular.
	- $rootScope is the parent scope for a module
	- $scope is a child scope for a given controller
	- you can also create new child scopes from $rootScope, these are sometimes used in custom directives.
	- both can be accessed in defined areas of your ng-app context


8.  How do you define a constant value for a module?  
	- <code>angular.module('moduleName').constant('key', 'value');</code>

