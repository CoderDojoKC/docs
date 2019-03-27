# Loops and Repeating Things

2015 had 12 months: January, February, March, April, May, June, July, August, September, October, November, December

2016 had 12 months: January, February, March, April, May, June, July, August, September, October, November, December

2017 had 12 months: January, February, March, April, May, June, July, August, September, October, November, December

2018 had 4 months: January, February, March, April, … which months are next?

* * *

Spin around and count each spin until you are dizzy. How many times could you spin around?

* * *

These are examples of loops. What are we doing with a loop? We are repeating things over and over again.

* * *

Your day could be condensed to “Wake up, do stuff, go to bed.”

```javascript
while (alive) {
    me.wakeUp();
    me.doStuff();
    me.goToBed();
}
```

In Scratch, this could look like:

```javascript
// Scratch
(repeat until (not alive)
    (wakeUp)
    (doStuff)
    (goToBed)
)
```

You’ll notice that even though these loops appear to go on forever, they have a conditional for when they can exit the loop. You want to have an “exit condition” to ensure that you don’t have an endless loop in your program.

In JavaScript, the school year could be written as:

```javascript
for (i = 0; i < 40; i++) {
    console.log("Let's go to school this week!");
}
// Let's go to school this week!
// Let's go to school this week!
// Let's go to school this week!
// Let's go to school this week!
// Let's go to school this week!
// ...
```

Here, the exit condition is that it has looped 40 times. It cannot loop 41 times.

You can also do something with the variables that are part of that loop.

```javascript
var weekdays = ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"];

for (i = 0; i < weekdays.length; i++ ) {
    console.log(weekdays[i]);
}

// Sunday
// Monday
// Tuesday
// Wednesday
// Thursday
// Friday
// Saturday
// Sunday
```

This could be rewritten using a special type of array loop called a `foreach`:

```javascript
weekdays.forEach(function(day) {
    console.log(day);
});
```

What are some things that you can loop over? You can loop over items in a list, like repeating back the list of items you are supposed to get at the store.

You can also use a loop to repeat an action. For instance, what if I want to have a character walk across the screen? I could say:

```javascript
// Scratch
(move(10))
(useNextCostume)
(wait(1))

(move(10))
(useNextCostume)
(wait(1))

(move(10))
(useNextCostume)
(wait(1))

(move(10))
(useNextCostume)
(wait(1))

(move(10))
(useNextCostume)
(wait(1))
```

Or, I could put those actions in a loop:

```javascript
// Scratch
(repeat(5)
    (move(10))
    (useNextCostume)
    (wait(1))
)
```

## Example Projects

* Scratch: [Loop Through Names](https://scratch.mit.edu/projects/216162307)
  <iframe src="https://scratch.mit.edu/projects/embed/216162307/?autostart=false" width="485" height="402" frameborder="0" allowfullscreen="allowfullscreen"></iframe>
* Scratch: Ethan G. [Cup Game](https://scratch.mit.edu/projects/149735896/)
  <iframe src="https://scratch.mit.edu/projects/embed/149735896/?autostart=false" width="485" height="402" frameborder="0" allowfullscreen="allowfullscreen"></iframe>
* Scratch: [Random Number Generator](https://scratch.mit.edu/projects/219375454)
  <iframe src="https://scratch.mit.edu/projects/embed/219375454/?autostart=false" width="485" height="402" frameborder="0" allowfullscreen="allowfullscreen"></iframe>
* Scratch: [Summer Plan: Go hiking!](https://scratch.mit.edu/projects/115901669) -- forever-loops used for animation
  <iframe src="https://scratch.mit.edu/projects/embed/115901669/?autostart=false" width="485" height="402" frameborder="0" allowfullscreen="allowfullscreen"></iframe>

## Project Ideas

* Reduce repeated steps to show a character walking across the screen
* Read names in a list that start with the letter "R"
