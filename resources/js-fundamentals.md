# JS Fundamentals

## What is an analogy to describe Javascript and its relationship to HTML and CSS

Think of a car fresh from the factory floor:
- HTML is parts of the car like doors, seats, engine, etc
- CSS is the styling of those parts ie paint job, interior trim, decals, etc
- Javascript is like being the owner of the car where you can decide if you want to change anything in the car like the parts or add Playboy seat covers.

## Explain `control flow` and `loops` using an example process from everyday life, for example 'waking up' or 'brushing your teeth' (but not those)

In programming, this refers to the order in which instructions are executed. The structures in place to direct this flow are sequential, selection, and iteration. Sequential runs in as a series of instructions. Selection gives choice based off certain conditions met (or not). Iteration or Loops involve performing actions either knowing how many times or not. This is much akin to adjusting your sweet, ergonomic, office chair until you reach your desired height or reading a book ie repeat reading a page until you want to take a break.

## Describe what the DOM is and an example of how you might interact with it

The DOM or Document Object Model is a data representation of all the properties, methods and events that comprise of the structure and content of a web document. So for an HTML document, it is the elements, and its attributes, and the content inside each of those elements. 

The browser creates the DOM and you would use Javascript to connect to it and then manipulate those **nodes**, as they are called, in real-time. One way of interacting with the DOM is by utilising the Dev Tools built into most modern browsers and running Javascript code directly:

![dev tools](/images/js-in-devtools.png)

*Javascript is run in the Console inside of DevTools*

Another way is to create a script in Javascript and have your website run that script to interact that way:

![javascript script](/images/js-script.png)

You can have many scripts run in your website you just have to reference them inside your HTML document.

## Explain the difference between accessing data from arrays and objects

Arrays are a collection of data where each piece of data has a number signisying where it is in a sequence:

`arrayPets = ['cat', 'dog', 'fish']`

This shows `cat` in the first position, `dog` in the second, etc. The data is accessed in an array by its position. This is known as its `index`. So `arrayPets[0]` would be the value `cat` at `index` of `0` and `arrayPets[2]` would be the value `fish` with an `index` of `2`. You may be confused with why it starts at `0` but this is a programming norm and the way I see it is how many positions is that data away from the initial position.

Objects stores its data in a pairing of a name for that data and the data itself. The name is called the `key` and the data is the `value`. This is known as a `key-value` pair and is fundamental in how you access its data:

```
const person = {
  "First Name": 'John',
  surname: 'Doe',
  gender: 'male',
  age: '30'
}  
```

In the above example, `firstName` is a key and `John` is the value for that key. You can access data in an object with one of two ways:
- Dot Notation - for when you directly give the name of a key `person.surname`
- Bracket Notation - for an indirect use such as in a variable or is a string `person["First Name"]`

There are some nuances to using these notations but we'll leave it at that for now.

## Explain what functions are and why they are helpful

Functions is a way for programmers to reuse a bunch of code over and over again. You can give a relatable name to a function and insert that in your code. This saves on time and makes it easier to maintain should you need to make changes to the function instead of the places you would have used that code.

Functions can be created to take input and make use of it to give a customised result. It can be as simple as taking two numbers, adding them together and then allow us to use that result in a way we see fit.

You can even use other functions inside other functions putting reusability at its core as you can piece together a function from lots of smaller functions to make something more complex.