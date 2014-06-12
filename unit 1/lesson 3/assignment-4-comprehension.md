## Comprehension Check

1. Explain $attrs and initial-attr-values. How would you use this in a controller and template, and what's the advantage? 	
	- $attrs is a map to any scoped attributes set on the assigned controller element
	- initial-attr-values are the values you set on the assigned controller element


2. How can you share state across controllers in Angular?
 	- you can make use of the $rootScope to global state
	- you can emit up to parent controllers or broadcast down to child controllers
	- you can make use of both to have the rootScope broadcast to all other e.g. siblings
	- you can also share state via services, constants and values if appropriate


3. Explain the difference between emitting and broadcasting an event in Angular.

	- see above: emitting goes up, broadcasting goes down.