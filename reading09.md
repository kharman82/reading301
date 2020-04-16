[README.MD](README.md)  
[medium.com](Functional Programming)  


**Functional Programming**  
- Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.  
_Pure Functions_  
- returns the same result if given the same argument aka . (deterministic)  
- using a global object that isn't passed as a parameter to the function is impure.  
- Any function that relies on a random number generator can't be pure either.  
_observable side effects_  
- modifying a global object or a parameter passed by reference.  
_Pure functions benefits_  
- Given a parameter A → expect the function to return value B  
- Given a parameter C → expect the function to return value D  
_example_ :a function to receive a collection of numbers and expect it to increment each element of this collection.  

**Immutability**  
- When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.  
**slugify**  
- method to transform the string input into a url slug.  
- toLowerCase: converts the string to all lower case  
- trim: removes whitespace from both ends of a string  
- split and join: replaces all instances of match with replacement in a given string  
- We combine all these 4 functions and we can "slugify" our string.  

**Functions as first-class entities**  
- The idea of functions as first-class entities is that functions are also treated as values and used as data.  
    - refer to it from constants and variables.  
    - pass it as a parameter to other functions  
    - return it as a result from other functions.  
_The idea is to treat functions as values and pass functions like data. This way we can combine different functions to create new functions with new behavior._  
**Higher-order functions**  
_function that takes one or more functions as arguments, or returns a function as its result_  

- The filter function expects a true or false value to determine if the element should or should not be included in the result collection.  
- We can also use the filter higher order function to receive the even function, and return a list of even numbers.  
**Map**  
_The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values._  

**Reduce**  
- The idea of reduce is to receive a function and a collection, and return a value created by combining the items.  


