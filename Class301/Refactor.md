## My summary of reading the functional programming article.
# What is functional programming:

![Functional programming](/images/fun.jpg)

It is a programming paradigm or more like a style of building the structure and elements of computer programs, that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

# Pure function:

So how do we know if a function is pure or not? Here is a very strict definition of purity:

1- It returns the same result if given the same arguments (it is also referred as deterministic).
2- It does not cause any observable side effects.
It returns the same result if given the same arguments

# Immutability:

When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.
In Javascript we commonly use the for loop. This next for statement has some mutable variables.


# Referential transparency:

Basically, if a function consistently yields the same result for the same input, it is referentially transparent.
pure functions + immutable data = referential transparency
With this concept, a cool thing we can do is to memoize the function. Imagine we have this function:

# Functions as first-class entities:

The idea of functions as first-class entities is that functions are also treated as values and used as data.
Functions as first-class entities can:
1- refer to it from constants and variables

2- pass it as a parameter to other functions

3- return it as result from other functions
The idea is to treat functions as values and pass functions like data. This way we can combine different functions to create new functions with new behavior.

# Filter:

Given a collection, we want to filter by an attribute. The filter function expects a true or false value to determine if the element should or should not be included in the result collection. Basically, if the callback expression is true, the filter function will include the element in the result collection. Otherwise, it will not.

# Map:

The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values.


# Reduce:

This is to reduce a function and a collection, and return a value created by combining the items.


# Refactor:

Refacoring is rewriting code for perfomance and readablility. Writing good code from the start is best practice, rather than having to rewrite code.

## To make my code more useable i will use REFACTOR:
Like giving spaces between every block of code to make it more tidy.

write one function that accepts a list of friendly things

separated some logic and reduced the number of lines of code

Using understandable variable names

adding comments so we can know this for what or what doing

***First Scenario***
We’re an URL-shortening website, like TinyURL. We accept a long URL and return a short URL that forwards visitors to the long URL. We have two functions.

***Second Scenario***
We’re a social media website where user URLs are generated randomly. Instead of random gibberish, we’re going to use the friendly-words package that the Glitch team works on. They use this to generate the random names for your recently created projects!

# When to use it:
A time to refactor your code is when you are working with something that you need to write over and over again. This isn’t the only time that you can refactor your code, however, it’s extremely common to run into things that are repetitive.

![Refactor](https://miro.medium.com/max/1838/1*EsrElEhlwbNxiCdpRmiubg.png)
# And that was it for this summary.