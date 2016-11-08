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
Well, the differences are within the language.  1: (ruby)== vs (js)===  equal signs,
though === and = can be used both, == and === are the most common
2: declaring methods and functions, again, language.  JS delcares by function() and Runy declares by
def
3:falsey values.  Ruby has two, JS has more.

citing: http://blog.flatironschool.com/javascript-vs-ruby/
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
Quick question here:  why do I get no spaces between my words in terminal when it
displays?

I'm not sure how you would make this any simpler.  I'm guessing that you want a way, since it's on the homeowork....You're not really repeating yourself, your naming two properties and putting them in a string...
What do you mean?!
```

## Ruby vs. Javascript :: String Methods

1. Open pry in your terminal and input `str = "ylbmessa lareneg`
2. With what you now know about ruby methods, reverse the string so that the output reads `"general assembly"`
 change the string into an array of characters so that the ouput reads : `["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]`
3. Then change your new array back into a string with hyphens in between characters so that your result is `"g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"`.
4. Even better if you can do so while removing the two `- -`'s between `general` and `assembly`

```md
str.reverse
str.reverse.chars
str.reverse.gsub(/\s*/, '-').gsub(/^-+|-+$|\s/, "").split   (this is ugly, but it's the only way I could figure out how to do it)
str.reverse.gsub(/\s*/, '-').gsub(/^-+|-+$|\s/, "").split

AHH!  I almost have it.  I can't quite remove the --.  Crap.


```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
cited: from wikipedia
Names which begin with a capital letter are treated as constants, so local variables should begin with a lowercase letter.
only nil and false evaluate to false.
a === b : used in case statements (read as "a matches b").



```
