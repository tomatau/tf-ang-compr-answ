## Comprehension Questions:

1. What is binding?
	- syncing state of data between the view and model in angular
	- this is using observable patterns to notify and update on changes

	
2. What is the purpose of the {{ }} braces in Angular templates?
	- display values of variables
	- more generally speaking it is to wrap an expression than can be evaluated inside the view when not a part of an existing directive's instance configuration.

	
3. Give some examples of expressions that can be evaluated in an Angular template.
	- someValue === 'example'
	- 42 - 41
	- 'Alf has ' + item
	- someArray[0]

	
4. The video recommends that you not put much logic in your Angular templates. Why do you think this is?
	- clutters view to make it less readable
	- we want domain logic in one place for clarity and reuse
	- logic is not the responsibility of a view/template as we may end up having to repeat it elsewhere and avoid maintaining it in multiple locations
	- e.g. we may want the same logic inside a different view
	

5. How can you use data binding in Angular to set a CSS class?
	- using an expression with the ng-class directive (without {{}})
	- 	{someClass: expression, anotherClass: expression}
	- using a normal class attribute and adding an expression that returns the desired class names