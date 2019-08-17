## Map

Beside simple methods to iterate over objects, Ruby Enumerable provides a number of important higher order constructs that we shall explore in further challenges. One such important method is the collect method, also known as map.

map as the name may suggest, takes a function and maps (applies) it to a collection of values one by one and returns the collection of result.

In this challenge, your task is to write a method which takes an array of strings (containing secret enemy message bits!) and decodes its elements using ROT13 cipher system; returning an array containing the final messages.

## :gem:My Code
```ruby
def rot13(secret_messages)
  secret_messages.map{| x | x.tr"a-z","n-za-m" }
end
```
