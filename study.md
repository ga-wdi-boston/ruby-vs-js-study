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
The firstn difference is how to increment (or increase) variables. For example,
say we want to increase i by 1.
JS: i+
Ruby: i += 1

The second difference is when we want to do an absolute comparison of objects,
meaning we want to see if they are the exact same object.
JS: 3 === 3
Ruby: 3 == 3

A third difference is the syntax of methods. JS requires parens and
curly brackets that are not needed in Ruby.

JS:
function hello() {
  console.log("hello");
}

Ruby:
def hello
  puts "hello"
end

Source: http://blog.flatironschool.com/javascript-vs-ruby/
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
name = "Jason"
age = 28
"#{name} is #{age} years old."
```

## Ruby vs. Javascript :: String Methods

1. Open pry in your terminal and input `str = "ylbmessa lareneg`
2. With what you now know about ruby methods, reverse the string so that the output reads `"general assembly"` change the string into an array of characters so that the ouput reads : `["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]`
3. Then change your new array back into a string with hyphens in between characters so that your result is `"g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"`.
4. Even better if you can do so while removing the two `- -`'s between `general` and `assembly`

```md
1. => "ylbmessa lareneg"
2. str.reverse().chars()
3. str.reverse().chars().join("-")
4. str.reverse().chars().join("-").gsub('- -', ' ')
```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
1. Ruby doesn't implicitly convert numbers to strings like JavaScript.
2. Ruby's convention is to use underscores between words in names (a.k.a. 'snake_case'). Constants start with a capital letter.
3. The Ruby comment character is #. Everything following a # on a line is ignored by the interpreter.
```
