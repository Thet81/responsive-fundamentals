<!-- readme.md -->

# Transitions in CSS

- We can control four aspects of an element's transition 
	- Which CSS properties transition
	- How long a transition lasts
	- How much time there is before a transition begins
	- How a transition accelerates

## Duration

- To create a simple transition in CSS, we must specify two of the four aspects : 
 1. The property that we want to transition.
 2. The duration of the transition.

 ```css
 	transition-property: color;
 	transition-duration: 1s;
 ```
## Timing function

	- The timing function describes the pace of the transition.
	- The default value is `ease`, which starts the transition slowly, speeds up in the middle, and slows down again at the end.
```css
	transition-timing-function: ease-out;
```

## Delay
 - Much like duration, the delay's value is an amount of time.
 - It specifies the time to *wait* before starting the transition.
 - We can use the `transition-delay` property like so:
 ```css
 	transition-delay : 200ms;
 ```

 ## Shorthand
 - We can use a shorthand version of these four property as follow.
 
 ```css
 	transition : color 1.5s linear 0.5s;
 ```

 - The properties are specified in this order : 
 	`transition-property`, `transition-duration`, `transition-timing-function`, `transition-delay`