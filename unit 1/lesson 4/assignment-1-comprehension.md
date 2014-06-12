### Comprehension Questions: 

1. What's the difference between CSS transitions and keyframe animations?
	- keyframes are named and self contained animations that can be reused
	- css transitions are a property for a single property that adds an easing, duration and other options for the animations of other properties on the same selection

2. What is the transition property shorthand for?
	- transition-property, transition-duration, transition-timing-function, transition-delay

3. What do the following transition parameters control? property, duration, timing-function, and delay.
	- property: the css property
	- duration: how long the animation will take to complete
	- timing-function: the curv used to complete the animation
	- delay: any time the animation will wait before starting

4. How can you detect when a transition has completed?
	- the animation complete event will be fired in JavaScript
		- transitionEnd / webkitTransitionEnd

5. How do you use @keyframes at rules?
	- to create a named keyframe but you must specify chrome vendor prefix as well as the non prefixed, then inside the named rule you specify the animations with percentages or to/from.

6. How do you make an animation loop?
	- using keyframes with a setting of infinite or forward and reverse using percentages but still a loop

7. How could you implement a loading image animation?
	- using keyframes to rotate a loading shape or image
	- making the loop infinite
	- using javascript to rotate an image or shape
	- animate it over time

8. What is GreenSock?
	- an animation library for javascript
	- an alternative to animation css library

9. How would you animate an element using jQuery?
	- using the animate function on a jQuery element object specifying properties, duration, easing and a callback on complete
	- You can also use addClass and css with duration properties.
	- Extra easing is available from the jQuery UI