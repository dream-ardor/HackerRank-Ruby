A common scenario that arises when using a collection of any sort, is to get perform a single type of operation with all the elements and collect the result.

For example, a sum(array) function might wish to add all the elements passed as the array and return the result.

A generalized abstraction of same functionality is provided in Ruby in the name of reduce (inject is an alias). That is, these methods iterate over a collection and accumulate the value of an operation on elements in a base value using an operator and return that base value in the end.

Consider an arithmetico-geometric sequence where the  term of the sequence is denoted. In this challenge, your task is to complete the sum method which takes an integer n and returns the sum to the n terms of the series.

## :gem:My Code
```ruby
def sum_terms(n)
  (0..n).inject {|sum, i| sum + (i * i + 1)}
end
```
