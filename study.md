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
1. In JS, the triple equals sign helps determine if two objects are the same exact object (having the same typeof and the same value). Ruby, on the other hand, uses double equals. JS has its own double equals, which determines if the values match.
2. Both Ruby and JS have arrays, but object array functions in JS and the class array methods in Ruby have different syntax. To find the index of an element in an array in JS you write arrayName.indexOf("element"), whereas you write array_name.index("element") in Ruby.
3. Another difference exists in falsey-ness of certain values in JS versus Ruby. Null (or nil in Ruby) and false will return false, but some truthy values in Ruby will return false in JS, like 0, empty strings (""), and undefined.

http://blog.flatironschool.com/javascript-vs-ruby/
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
[1] pry(main)> name = "Jason"
=> "Jason"
[2] pry(main)> age = 28
=> 28
[3] pry(main)> "#{name} is #{age} years old"
=> "Jason is 28 years old."
```

## Ruby vs. Javascript :: String Methods

1. Open pry in your terminal and input `str = "ylbmessa lareneg`
2. With what you now know about ruby methods, reverse the string so that the output reads `"general assembly"` change the string into an array of characters so that the ouput reads : `["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]`
3. Then change your new array back into a string with hyphens in between characters so that your result is `"g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"`.
4. Even better if you can do so while removing the two `- -`'s between `general` and `assembly`

```md
[1] pry(main)> str = "ylbmessa lareneg"
=> "ylbmessa lareneg"
[2] pry(main)>  str.reverse!.chars.to_a
=> ["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]
[3] pry(main)> str.gsub(/(.{1})/, '\1-')
=> "g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y-"


```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
1. == and === mean different things, with === as a 'strict equality' comparator and == as a 'loose equality' comparator in JS. == in Ruby is the convention for equality.
2. Names that begin with a capital letter are treated as constants, so local variables should begin with a lowercase letter.
3. The usual operators for conditional expressions, and and or, do not follow the normal rules of precedence: 'and' does not bind tighter than 'or'.
```
