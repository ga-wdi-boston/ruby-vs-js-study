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
The use of == and ===.  In javascript we use === to compare two values.  In ruby we use ==.  Javascript also
utlizes == but it returns a boolean.

The syntaxt for functions is different.  If I wish to display 'Hello World' I would need to define the function
in Ruby and then use 'puts' to display.  In JS I would create the function and console.log for diaplay.

A more obvious difference is in how JS and Ruby are composed.  JS appears to be more complex at face value while
Ruby can almost be interpreted in plain english terms.
<!-- your answer here -->
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
man = {name: 'Jason', age: 28}
man[:name] + ' is ' + man[:age].to_s + ' years old.'


```

## Ruby vs. Javascript :: String Methods

1. Open pry in your terminal and input `str = "ylbmessa lareneg`
2. With what you now know about ruby methods, reverse the string so that the output reads `"general assembly"` change the string into an array of characters so that the ouput reads : `["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]`
3. Then change your new array back into a string with hyphens in between characters so that your result is `"g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"`.
4. Even better if you can do so while removing the two `- -`'s between `general` and `assembly`

```md
str = "ylbmessa lareneg"
str.reverse.chars.to_s.strip.gsub(' ', '-').gsub(/[^\w-]/, '').gsub(/--/,'-')
```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
1. Using variables and semicolons
2. Mistaking === for == and also == for =
3. Null is not the same as Nil
```
