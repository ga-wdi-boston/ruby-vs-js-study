# Ruby versus Javascript Study

Use your favorite search engine and any other resources to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Use `grunt test` to test your code.


## Comparison


Describe three examples of differences between Ruby and Javascript?

```md
1. Variables
In Javascript you need to declare variables by prefacing them with something like const, let or var.
Example: let myArray = [1, 2, 3, 4, 5];
In Ruby, you don't need to preface the variable with anything.
Example: myArray = [1, 2, 3, 4, 5]

2. Semicolons
In JavaScript, most often you need a semicolon after a statement whereas, you don't in Ruby.

3. Equivalency
In JavaScript, you use === to determine whether two things are the same object.  In Ruby, you use ==.

Resources:
http://blog.flatironschool.com/javascript-vs-ruby/
https://medium.com/learning-to-code/ruby-vs-javascript-a-quick-comparison-ebd3b63ebc49#.x7mn6bu1t
```

## Ruby Versus Javascript :: String Interpolation

What is another, perhaps more DRY-compliant way to write this in Ruby?

Experiment in pry and place your answer below.

```ruby
[1] pry(main)> name = "Jason"
=> "Jason"
[2] pry(main)> age = 28
=> 28
[3] pry(main)> name + " is " + age.to_s + " years old."
=> "Jason is 28 years old."
```

```md
person = { name: jason, age: 28 }
"#{person[:name]} is #{person[:age]} years old."
```

## Ruby vs. Javascript :: String Methods

1. Open pry in your terminal and input `str = "ylbmessa lareneg`
2. With what you now know about ruby methods, reverse the string so that the output reads `"general assembly"` change the string into an array of characters so that the ouput reads : `["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]`
3. Then change your new array back into a string with hyphens in between characters so that your result is `"g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"`.
4. Even better if you can do so while removing the two `- -`'s between `general` and `assembly`

```md
str.reverse.chars.join('-').gsub(/- -/, ' ')
```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
1. Remembering to end loops with 'end'
2. Methods that don't take arguments don't need parenthesis (like in the last exercise).
3. Hashes in Ruby are similar, but not the same thing as Objects in JavaScript.
```
