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
A lot of syntax for methods varies from Ruby to JS (e.g. array.index(x) v.s. array.indexOf(x), array.any?{|x| x > 2} v.s. array.some(functions(n){ return x > 2}), etc)
You do not need to use "()" when passing variables to a function in Ruby.
You do not need to end statemends with ";"
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

```ruby

def intro(name, age)
  puts "#{name} is #{age} years old."
end

```

## Ruby vs. Javascript :: String Methods

1. Open pry in your terminal and input `str = "ylbmessa lareneg`
2. With what you now know about ruby methods, reverse the string so that the output reads `"general assembly"` change the string into an array of characters so that the ouput reads : `["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]`
3. Then change your new array back into a string with hyphens in between characters so that your result is `"g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"`.
4. Even better if you can do so while removing the two `- -`'s between `general` and `assembly`

```ruby
str = "ylbmessa lareneg"

puts str.reverse().split(/\B/).join("-")

```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
1) Using the wrong syntax
2) === !== ==
3) only false and nil are falsey
4) '#' for commenting
```
