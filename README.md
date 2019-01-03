## Quiz

- The purpose of this homework is to test your understanding of both the Ruby Language
  and the Rails web development framework. Please do leverage the resources that
  appear within the references section of this document.

## Software requirements

- Ruby 2.3.1 or higher

## Clone this repository
```
git clone git@github.com:clarkngo/fh-homework-08.git
```

## Navigate to the Rails application

```
$ cd fh-homework-08
```

## License

fh-homework-08 is released under the [MIT license](https://mit-license.org).

## Copyright

copyright:: (c) Copyright 2018 Clark Jason Ngo. All Rights Reserved.

## Quiz

### 1. What is an Object? Please write your answer below.

In Computer Science an object can be a variable, a data structure, a function, or a method, and as such, a value in memory referenced by an identifier.
In OOP, Object refers to a particular instance of class.
In Ruby, everything is an object.

### 2. What is a Class? Please write your answer below.
In object-oriented programming, a class is an extensible program-code-template for creating objects, providing initial values for state (member variables) and implementations of behavior (member functions or methods).

### 3. What's the difference between a class and module?
Class can be instantiated and a Module cannot.

Ruby Modules are similar to classes in that they hold a collection of methods, constants, and other module and class definitions. Modules are defined much like classes are, but the module keyword is used in place of the class keyword.

### 4. What does the self mean in the Ruby language? Please write your answer below.
Self in Ruby. The keyword self in Ruby gives you access to the current object – the object that is receiving the current message.

Source: https://www.jimmycuadra.com/posts/self-in-ruby/

### 5. What is a block as defined in the Ruby language?
Ruby Code blocks (called closures in other languages) are chunks of code between braces or between do..end that you can associate with method invocations, almost as if they were parameters. A Ruby block is a way of grouping statements, and may appear only in the source adjacent to a method call; the block is written starting on the same line as the method call's last parameter (or the closing parenthesis of the parameter list). The code in the block is not executed at the time it is encountered. Instead, Ruby remembers the context in which the block appears (the local variables, the current object, and so on) and then enters the method.

Source: http://rubylearning.com/satishtalim/ruby_blocks.html

Given the following:
hash = { a: 1, b: 2, c: 3, e: 4, f: 5, g: 6, h: 7, i: 8, j: 9, k: 0 }
Please answer the following questions:
### 6. How would I get the value of 'f'? Please write your answer below.

5

### 7. How would I add the key, 'l', with a value of 11 to the 'hash'? Please write your answer below.

8. Write a method, sum_hash_values, which takes all the values of a hash produces a total. Please write your answer below.
```
def sum_hash_values( some_hash )
# write your answer here
end
```
9. Write a method, sum_hash_odd_values, which takes all of the odd values of a hash produces a total. Please write your answer below.
```
def sum_hash_odd_values( some_hash )
# write your answer here
end
```
Note: Please don't use any Ruby Standard library methods.
10. What's the difference between a Hash vs Array in the Ruby language? Write your answer below.

11. Write a method to determine whether not a string is a palindrome using
recursion?
```
def palindrome?( some_string )
_palindrome?( some_string, 0, some_string.length - 1 )
end
def _palindrome?( some_string, head_index, tail_index )
# define your method here
end
```
> is_palindrome( "bob" )
> => true
> is_palindrome( "frank" )
> => false
> is_palindrome( "pop" )
> => true
> is_palindrome( "xxxx yyyy xxxx" )
> => true
Note: Your solution should not use map, each, for, while, and so on.
12. Given an array write a method to compute the length of an array
using recursion.
def length( array )
# define your method here
end
Note: Your solution should not use a Ruby Standard Library method which
implements the same functionality. Also, your solution
should not be using map, each, for, while, and so on.
13. Given an array write a method to compute the length of an array
using iteration.
```
def length( array )
# define your method here
end
```
Note: Your solution should not use a Ruby Standard Library method which
implements the same functionality.
14. computes the power of number with a given exponent using recursion
```
power(number, exponent) where number is an integer and exponent >= 0
def power(number, exponent)
# write your code here
end
```
Note: Your solution should not use a Ruby Standard Library method which
implements the same functionality. Also, your solution
should not be using map, each, for, while, and so on.
15. Consider the following two methods:
```
def times_four(arg1);
puts arg1 * 4;
end
```
```
def multiply(arg1, arg2);
puts arg1 * arg2;
end
```
What will be the result of each of the following lines of code:
times_four 5 => please write your answer here
times_four(5) => please write your answer here
times_four (5) => please write your answer here
multiply 1, 2 => please write your answer here
multiply(1, 2) => please write your answer here
multiply (1, 2) => please write your answer here
16. What is the convention for methods which end with a question mark ? e.g. #all?, #kind_of?, directory?
a) They should always require arguments.
b) They should always return a boolean value.
c) They should always report a value of the object they're being called on.
17. For the string class, what's the difference between "#slice" and "#slice!"?
a) None, "#slice" is just an alias for "@slice!".
b) There is no "#slice!" method in Ruby on Rails.
c) "#slice" returns a new object, "#slice!" destructively updates - mutates - the object's value.
18. Given the Ruby expression `a, b = b, a` where a = 5 and b = 6\. What's the value of 'a' and 'b' after the expression is executed?
a) a = 5, b = 6
b) a = 6, b = 5
c) a = 6, b = 6
Git Core
19. What are the steps (i.e. commands) to initialize a local Git repository? Please write your answer below.
20. What's the command to stage a file using Git? Please write your answer below.
21. What are the necessary commands to setup a local repository so that one can push to Github.com? Please write your answer below.
22. What does `git checkout branch-name` do? Please write your answer below.
23. What does `git checkout -b branch-name` do? Please write your answer below.
24. What does `git branch -D branch-name` do? Please write your answer below.
25. What does `git merge branch-name` do where `branch-name` is a sub branch of `master`? Please explain your answer below.
RSpec Core
26. What is TDD?
27. What is RSpec? Please write your answer below?
28. Given the following Spec
```
describe Person do
it 'should not be valid' do
person = Person.new( 'John', 'Doe')
expect( person ).to_not be_nil
end
end
```
Write the implementation below which will make this test pass.
Note: It may be better to run locally on your system for correctness?
29. Continuing with the previous spec write an example for testing a method `full_name`.
```
describe Person do
it '.full_name' do
# add your code here
end
end
```
Note: If you created a person with the first name of `John` and the last name of
`Doe`, then the `full_name` should generate `John Doe`.
30. Write the implementation code which passes the example we created in (29). Please write your answer below.
```
Note: If you created a person with the first name of `John` and the last name of
`Doe`, then the `full_name` should generate `John Doe`.
```
31. Continuing with the previous spec write an example for testing a method `reversed_full_name`.
```
describe Person do
it '.reversed_full_name' do
# add your code here
end
end
```
Note: If you created a person with the first name of `John` and the last name of
`Doe`, then the `reversed_full_name` should generate `Doe, John`.
32. Write the implementation code which passes the example we created in (31). Please write your answer below.
Note: If you created a person with the first name of `John` and the last name of `Doe`, then the `reversed_full_name` should generate `Doe, John`.
33. Write the example and implementation code which passes the following examples.
```
describe Person do
it '#first_name' do
person = Person.new( 'John', 'Doe')
# add you code here
end
it '#last_name' do
person = Person.new( 'John', 'Doe')
# add your code here
end
end
class Person
# add your code here
end
```
34. Add a `middle_name` method to our `Person` class. Rewrite all the examples using the information from the above.
```
describe Person do
it '#initialize' do
# add your code here
expect( person ).to_not be_nil
end
it '#full_name' do
# add your code here
end
it '#reversed_full_name' do
# add your code here
end
it '#first_name' do
# add you code here
end
it '#last_name' do
# add your code here
end
it '#middle_name' do
# add your code here
end
end
```
Rails Core
35. Please explain M in model view controller (MVC) within the Ruby on Rails
Framework? For example, what's the role of the model. Write your answer below in your own words.
36. Please explain V in model view controller (MVC) within the Ruby on Rails
Framework? For example, what's the role of the view. Write your answer below in your own words.
37. Please explain C in model view controller (MVC) within the Ruby on Rails
Framework? For example, what's the role of the controller. Write your answer below in your own words.
38. Use the Rails generator to produce a model called Actor which has the
following fields:
- first_name - string
- middle_name - string
- last_name - string
Please write the command below.
39. Implement the Actor class using Ruby. Write your answer below.
40. Use the Rails generator to produce a model called Movie which has the
following fields:
- actor_id - integer
- name - string
- release_on - date
Please write the command below.
41. Implement the Movie class using Ruby. Write your answer below.
42. Use the Rails generator to produce a model called Filmography which has the following fields:
- actor_id - integer
- movie_id - integer
Note: This is our join model which we'll be able to associate a
given actor to a movie.
43. Implement the Filmography class using Ruby. Write your answer below.
44. Update the Actor model with the proper associations for accessing its'
filmographies and movies. Write the updated model below.
45. Update the Movie model with the proper associations for accessing its'
filmographies and actors. Write the updated model below.
46. Using the information from (43) - (45), write a Rails query which
would give one all the movies for a given Actor. Please write
your answer below.
47. Using the information from (43) - (45), write a Rails query which
would give one all the actors which starred in a given Movie. Please
write your answer below.