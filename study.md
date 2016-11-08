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
Javascript does not have implicit returns, they must be specified inside functions or they will return nothing.

Ruby allows variables to be declared without a declaration like "let" or "const"

iteration in JS requires a for loop (usually). Ruby has many methods to avoid this, such as .each, which accomplished the same thing with less code.
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
str.reverse
str.reverse.split("")
str.reverse.split("").join("-")
str.reverse.gsub(/\s+/, "").split("").join("-")
```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
1. only nil and false are falsey in Ruby. "" and 0, for example, are truthy.
2. == is equal value in Ruby, in JS it's ===
3. Ruby uses floor division for integers, so 4/3 => 1, not 1.33333333 as in JS
```
