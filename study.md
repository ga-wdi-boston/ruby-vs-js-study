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
In Ruby you can use spaces in the place of parenthesis to enclose arguments
passed to functions and parameters; in Javascript parenthesis are required.

Ruby has more robust/elegant array manipulation then Javascript does. E.g. in
Ruby you can use negative indexes to get a value of from the end of an array
while in Javascript you cannot.

In Ruby the case of a character means something when naming variables, such as
StartingWithACapitalLetter meaning the variable is a constant, while in Javascript
you have to declare the variable using 'const'
```

## Ruby Versus Javascript :: String Interpolation

What is another, perhaps more DRY-compliant way to write this in Ruby?

Experiment in pry and place your answer below.

```ruby
[1] pry(main)> name = "Jason"
=> "Jason" [2] pry(main)> age = 28
=> 35
[3] pry(main)> name + " is " + age.to_s + " years old."
=> "Jason is 28 years old."
```

```md
[1] pry(main)> name = "Jason"
=> "Jason"
[2] pry(main)> age = 28
=> 35
[3] pry(main)> "#{name} is #{age} years old."
=> "Jason is 28 years old."
```

## Ruby vs. Javascript :: String Methods

1. Open pry in your terminal and input `str = "ylbmessa lareneg`
2. With what you now know about ruby methods, reverse the string so that the output reads `"general assembly"` change the string into an array of characters so that the ouput reads : `["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]`
3. Then change your new array back into a string with hyphens in between characters so that your result is `"g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"`.
4. Even better if you can do so while removing the two `- -`'s between `general` and `assembly`

```md
str.reverse.split('').join(',').gsub(',', '-').gsub('- -', ' ')
```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
You cannot 'use' negative indexes in Javascript! It will simply return undefined.
In Ruby, however, a negative index will return the value from the end of an array.

Ruby has different syntax for enclosing things like loops and if statements than
in Javascript (Ruby 'do/end' vs Javascript '{/}')

Comparisons in Ruby and Javascript behave differently then each other. So == in
Ruby is not the same as == in Javascript, likewise with === in Ruby and === in Javascript.
```
