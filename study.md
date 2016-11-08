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
One big difference is that semicolons are not used in Ruby whereas they're used
frequently in JS.

Objects in JS are hashes in Ruby.

To access the value of a key in Ruby, you use [] whereas in JS you can use "."
You can't use "." in Ruby.
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
"#{name} is #{age} years old"  (When I tried to include the "." at the end of
the sentence I got a "\n" after it, and I'm not sure how to fix that.)
```

## Ruby vs. Javascript :: String Methods

1. Open pry in your terminal and input `str = "ylbmessa lareneg`
2. With what you now know about ruby methods, reverse the string so that the output reads `"general assembly"` change the string into an array of characters so that the ouput reads : `["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]`
3. Then change your new array back into a string with hyphens in between characters so that your result is `"g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"`.
4. Even better if you can do so while removing the two `- -`'s between `general` and `assembly`

```md
I'm not entirely sure what I am supposed to be writing here.
  For 1) I did str.reverse
  For 2) I did newArray = str.split(//)
  For 3) newArray.to_s  ...can't figure out how to put hyphens in between though
```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
In Ruby, we us == to test equality rather than ===, which we used in JS.
We don't need to use parentheses in Ruby when calling a function. In JS, we
did have to use parentheses.
Only "false" and "nil" are falsey in Ruby.
```
