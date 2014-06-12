### Comprehension Questions: 

1.  What is a controller?
	- component involved with decision making
	- in the past it was where you compose models with views and events with use cases
	- in angular it is the 'VM'
	- it's main responsibility in angular is to initialise state and add behaviour to a view

2.  How do you link to a controller in your HTML file?
	- write JavaScript containing a function and include the script in the html file.  You should use the ngController directive inside the view to set the scope of the desired controller.

3.  How do you link a controller to a DOM element?
	- ng-controller attribute with a value of the controller function declaration to create a controller scope inside the element


4.  What's the syntax for declaring a controller?
	- <code>< element ng-controller="MyControllerName" /></code>

	where function MyControllerName(){} is a controller inside JavaScript that most likely has $scope injected into it.