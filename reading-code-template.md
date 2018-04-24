# [Title](and link to original code)

Write the purpose here:
* Why does this code exist? 
* What does it allow a user to do?
* This will look something like: A user can ...
* This shouldn't be very long

_function name_: Function
* Args: (how many args does this function take?)
  * (List each arg, it's type, and it's purpose)
* Return: (what type does this function return?)
  * (Describe the return value in nested detail)

or if it's an object

_object name_: Object
* Properties: number of them
  * _name of property_: type
    * Initial Value: what's written in the source code
    * Purpose: What it does in the object
* Methods: number of them
  * _name of method_: 
    * Args: (how many args does this function take?)
      * (List each arg, it's type, and it's purpose)
    * Return: (what type does this function return?)
      * (Describe the return value in nested detail)
    * Behavior: what does this method do?
    * Purpose: why does this method exist in the object?

### Index:
* [Behavior](#behavior)
  * [Input Analysis](#input-analysis)
  * [Test Cases](#test-cases)
* [Implementation](#implementation)
  * [Original Code](#original-code)
  * [Reconstruction](#reconstruction)
* [Notes](#notes)

___

## Behavior

Describe the behavior of this code, behavior is very closely tied to test cases.  The behavior of code has to do with the external effects of this code: what it's arguments are, what it's return value is, and anything else in the program that it modifies.  If you find yourself describing what's written between the opening and closing curly braces of a function, you're probably doing this wrong.

Another nice way to think about this is by asking yourself:
* "When this code has _finished_ running, what will have changed?"


### Input Analysis

What characteristics of your inputs are important for your solution? 

What groupings will you have to consider when building your solution? 

How did you use this information to select your test cases?

### Test Cases

```js
assert(5 == add(2, 3));
assert(1 == add(-2, 3));
assert(-1 == add(2, -3));
assert(-5 == add(-2, -3));
```

[TOP](#index)

___

## Implementation 

Give an overview of what is tricky about implementing this behavior.
* Anything unexpected challenges?
* Did trying to code it change your understanding of the behavior?

### Original Code

```js
// the original code you studied
```

_Strategy:_
Explain the strategy they used.  Was it heavy in logic or languge features? What strategies did they use?  How is it like and unlike others?


_Language Features:_
What language features did they use, and how much does their solution rely on them?

### Reconstruction

```js
// your reconstruction here
// same specs, same behavior, different implementation
```

_Strategy:_
Explain the strategy you used.  Was it heavy in logic or languge features? What strategies did they use?  How is it like and unlike others?

_Language Features:_
What language features did you use, and how much does your solution rely on them?

_Comparison:_
How does your solution compare to theirs?  How would you make yours more like theirs? What suggestions would you have for them?


[TOP](#index)

___

## Notes

Things I learned studying this problem:


New vocabulary:


Things I struggled with:


Lessons to apply for next time:


[TOP](#index)


___
___
### <a href="http://elewa.education/blog" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/34921062-506450ae-f97d-11e7-875f-6feeb26ad72d.png" width="100" height="40"/></a>