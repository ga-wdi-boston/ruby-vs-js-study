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
Ruby you just write the name of variable JS you have to declare it.
you say *end* at the end of function in ruby instead of with closing bracket }.
in ruby methods do not require () parenthesis, in js parenthesis are required even if it's empty

https://medium.com/learning-to-code/ruby-vs-javascript-a-quick-comparison-ebd3b63ebc49#.hd2r8r7a8
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
"Jason is twenty-eight years old."
```

## Ruby vs. Javascript :: String Methods

1. Open pry in your terminal and input `str = "ylbmessa lareneg`
2. With what you now know about ruby methods, reverse the string so that the output reads `"general assembly"` change the string into an array of characters so that the ouput reads : `["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]`
3. Then change your new array back into a string with hyphens in between characters so that your result is `"g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"`.
4. Even better if you can do so while removing the two `- -`'s between `general` and `assembly`

```md
str.reverse

for 3 and 4 I looked at the documetnation https://ruby-doc.org/core-2.2.0/String.html#method-i-slice-21
for awhile could not find the right method.
```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
Not using == in Ruby instead using === from js.
ruby doesn't convert numbers to strings automatically as JS does.
you don't use let or const to declare a variable in ruby, as in JS.
```
