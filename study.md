# Ruby versus Javascript Study

Use your favorite search engine and any other resources to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Use `grunt test` to test your code.


## Comparison


Describe three examples of differens between Ruby and Javasctipt?

```md
In Ruby there is no need for parentheses after methods are performed on various data types.
  for example you can do array.pop instead of array.pop()

There is no need for variable declaration.
  For example, in JS you need to use let or const whereas in ruby you can simply declare a variable. See below:
    let myArray = [1, 2, 3, 4, 5] vs my_array = [1, 2, 3, 4, 5]

Instead of curly braces to determine when a function is starting or ending, Ruby makes use of do, end, and implicit returns.
```

## Ruby Versus Javascript :: String Interpolation

What is another, perhaps more DRY-compliant way to write this in Ruby?

Experiment in pry and place your answer below.

```ruby
[1] pry(main)> name = "Jason"
=> "Jason"
[2] pry(main)> age = 28
=> 35
[3] pry(main)> name + " is " + age.to_s + " years old."
=> "Jason is 28 years old."
```

```md
person = {name: "Jason", age: 28}
person[:name] + " is " + person[:age] + " years old."

```

## Ruby vs. Javascript :: String Methods

1. Open pry in your terminal and input `str = "ylbmessa lareneg`
2. With what you now know about ruby methods, reverse the string so that the output reads `"general assembly"` change the string into an array of characters so that the ouput reads : `["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]`
3. Then change your new array back into a string with hyphens in between characters so that your result is `"g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"`.
4. Even better if you can do so while removing the two `- -`'s between `general` and `assembly`

```md
str = str.reverse.split("");
str = str.join("-").gsub(/[- -]/, ' ') #gets rid of all dashes, unsure of how to only get rid of some

```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
Implicit returns can cause you to forget to add an end in certain places

Typing puts will simply allow a phrase to print eliminating need for console.log

Object are similar, but accessing them is different, probably the only thing that is harder in Ruby than JS Not everything in Ruby is an object like it is in JS.


```
