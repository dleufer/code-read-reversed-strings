# [String Reverser](https://www.codewars.com/kata/reversed-strings)

Write the purpose here:
* This code exists in order to reverse a string.
* It allows the user to input a string, and receive a reversed version of that string.

_function name_: solution
* Args: 1
  * It takes a string
* Return: a string
  * the returned string is a reverse of the original input string

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
* A string is passed as an argument to the function.
* The function reverses the order of the characters in the string.
* The function then returns the reversed string.

### Input Analysis

What characteristics of your inputs are important for your solution?
* It's a String.
* It's longer than 1 character.
* It doesn't contain integers or other non-string elements.
* It could be a problem if the string is an anagram: we won't know.
* Letters with accents could be an issue.
* Escape characters could cause problems.


What groupings will you have to consider when building your solution?
* What are groupings?

How did you use this information to select your test cases?
* We wrote a test case for each scenario that we considered important.

### Test Cases

```js
assert('dlrow' == solution('world'));
assert('g' == solution('g'));
assert(undefined == solution(1 'panda'));
assert('racecar' == solution('racecar'));
assert('navaN' == solution('Navan');
assert('énnod' == solution('donné');
assert('s\'ti' == solution('it\'s');
assert('gnaY\\gniY' == solution('Ying\\Yang');
```

[TOP](#index)

___

## Implementation

Give an overview of what is tricky about implementing this behavior.
* It's tricky to access the characters individually, because they come as a 'block' in the string input.
*

### Original Code

```js
function solution(s){
  var o = '';
  for (var i = s.length - 1; i >= 0; i--)
    o += s[i];
  return o;
}
```

_Strategy:_
* It is not heavy in language features (this is why we picked it).
* They declare a new variable, with a terrible name, o.
* o is set equal to an empty string.
* Then a for-loop is used.
* Statement 1 declares a variable, i, and sets it equal to the length of the string input minus 1. It is length minus 1 to deal with the zero indexing of the string.
* Statement 2 is the test condition. It checks if i is greater than or equal to zero. When i equals zero, the loop will stop.
* Statement 3 defines what happens at the end of one run of the loop. The value of i is reduced by 1. This allows the index to move backwards through the string.
* The first time the loop runs, i is set to correspond to the index value of the last character in the string.
* s[i] is used to access the last character in the string, and this is added to o.
* Statement 3 then runs, and the value of i is decremented by 1.
* Now statement 2 runs its test. If i is greater than -1, it passes, and the character from s[i] is added to o.
* Statement 3 runs again, decrementing i.
* This continues until i = -1, and then the return statement returns o.
* o now contains all the characters in the original string, but in reverse order.
* The for loop is now over.

_Language Features:_
* A for loop
* Variable declarations
* Strings
* .length property for Strings
* incrementation/decrementation

### Reconstruction

```js
function reverser(string){
  let reversedString = '';
  for (let i = string.length - 1; i >= 0; i--) {
    reversedString += string[i];
  }
  return reversedString;
}
```

_Strategy:_
* We used the same strategy, we just fixed bad variable and function names, and fixed unclear syntax (no curly braces).
* We also used let instead of var to declare our variables.

_Language Features:_
* We used the same language features.

_Comparison:_
* Our solution cleans things up a bit, and conforms more to best practice.


[TOP](#index)

___

## Notes

Things I learned studying this problem:
* How to use Python Tutor.
* That you should use good names for variables and functions.
* How a for loop works.
* Why you set i equal to string.length minus 1.


New vocabulary:
* let versus var.

Things I struggled with:
* How to for loop executes, especially the order of the 3 statements.

Lessons to apply for next time:
* Use good names.

[TOP](#index)


___
___
### <a href="http://elewa.education/blog" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/34921062-506450ae-f97d-11e7-875f-6feeb26ad72d.png" width="100" height="40"/></a>
