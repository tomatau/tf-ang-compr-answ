### Comprehension Questions: 

1. What file do you need to inlcude in a script tag in your templates to use ngAnimate?
	- angular-animate.js

	
2. What are the 'ng-' prefixed CSS classes you write rules for to achieve animations?
	- enter, leave, move, x-active, ng-hide, ng-hide-add/remove (for transitions)
	- keyframes/transitions in the above class' for 'animations'

	
3. How could you animate an ng-hide call?
	- add classes to ng-hide, ng-hide-add and ng-hide-remove that contain the animations or 
	- use beforeAddClass and, addClass and the same for removeClass
	

4. How do you attach multiple animation events to a CSS class using JavaScipt animations?
	- add animations for the available keys in the animate configuration such ass addClass / enter / move / etc...
	

5. How do you include ngAnimate as a dependency for your module?
	- [ 'ngAnimate' ] as a module dependency, the dependency array is set after the module name for the angular.module function
	

6. Give the starting and ending CSS classes for each of the following events: enter, leave, move.
	- ng-enter -> ng-enter-active
	- ng-leave -> ng-leave-active
	- ng-move -> ng-move-active
	

7. How do animations work with ng-repeat?
	- enter when they appear (after initial state is loaded for the scope), move when they sort or shuffle, leave when removed (filtered)
	

8. What is a staggered animation?
	- a queue of animations with a delay between the start of each animation so they are introduced one by one (ie. not all at precisely the same time)
	

9. Give a code example that uses staggered animation

e.g.
	
	.ng-enter-stagger {
		-webkit-transition-delay: 0.2s;
		transition-delay: 0.2s;
	}
	// rest as usual for ng-enter / enter-active
	

	
