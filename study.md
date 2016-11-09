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
1. When defining variables in Javascript, we always began by declaring a variable with "let", "var", or "const". In Ruby, variables can be defined without previsouly being declared. define variables without having to simple just start typing the name of the variable without having to preemptively use a keyword.

2. How "==" and "===" are used in each. In Js, '===' is known as a 'strict equality comparer' and '==' is a 'loose equality comparer'. In addition, we almost never use '==' in JS. In Ruby, we use '==' to test for equality, NOT '==='. As with the '==' in JS, we rarely use '===' in Ruby.

3. Incrementing. In JS, we were able to use '++' or '--' to increment. An example of this would be:
  var z = 1;
  z++;

 In Ruby, we would use the folloing to increment:
  x += 1
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
[1] pry(main)> name = "Jason"
=> "Jason" [2] pry(main)> age = 28
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
[1] pry(main)> str = "ylbmessa lareneg"
=> "ylbmessa lareneg"
[2] pry(main)> str.reverse!
=> "general assembly"
[3] pry(main)> split_arr = str.split(%r{\s*})
=> ["g", "e", "n", "e", "r", "a", "l", "a", "s", "s", "e", "m", "b", "l", "y"]
[4] pry(main)> joined_arr = split_arr.join("-")
=> "g-e-n-e-r-a-l-a-s-s-e-m-b-l-y"
[5] pry(main)> joined_arr.insert(13, "-")
=> "g-e-n-e-r-a-l--a-s-s-e-m-b-l-y"
[6] pry(main)> joined_arr.insert(14, " ")
=> "g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"


```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
1. How Booleans are handled in each language. In Ruby, only 'false' and 'nil' are considered falsey. In Javascript 'false', '0', "", '', 'null', 'undefined', and 'Nan' are all considered falsey. I found this strange because I thought that rules such as these would be more similar than other rules (such as syntax) across the board because 'true' & 'false' have very universal meanings.
2. Ruby has implicit returns. While very convenient, I thought it was strange that such a new language had this feature. I figured that the idea of returns would almost be standard in all languages. I guess the big difference in my understanding stems from the fact that we learned JS before Ruby.
3. Commenting out code. In Ruby, the comment character is '#' and it is used to comment out a full line.
4. Ruby's lack of an implicit number to string conversion. Again, I thought that this is strange because of our prior exposure to JS. Although, I guess it does make sense to not have implicit conversions when we have methods that are specifically made to convert data types, such as: '.to_s' and '.to_i'
```
