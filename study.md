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
1. In Javascript, === means strict equality. Eg, 5 === 5 returns true
   In Ruby, "==" is used for strict equality.
2. In Javascript, incrementing or decrementing uses ++ or --.
   In Ruby, we use += or -=
3. Function syntaxes are different in Javascript and Ruby
4. Ruby:
   def hello_world
    puts "hello world"
   end
   Javascript:
   function hello_World() {
    console.log("Hello World");
   }
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
age = "28"
"#{name} is #{age} years old"
```

## Ruby vs. Javascript :: String Methods

1. Open pry in your terminal and input `str = "ylbmessa lareneg`
2. With what you now know about ruby methods, reverse the string so that the output reads `"general assembly"` change the string into an array of characters so that the ouput reads : `["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]`
3. Then change your new array back into a string with hyphens in between characters so that your result is `"g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"`.
4. Even better if you can do so while removing the two `- -`'s between `general` and `assembly`

```md
str = "ylbmessa lareneg"
str.reverse!
arr = []
0.upto(str.length - 1) do |i|
  arr << str[i]
end
len = (str.length - 1) * 2
0.upto(len) do |i|
  arr << arr[i]
  arr << "-"
end
```

## What are three common "gotchas" in Ruby after learning Javscript.

```md
"===" and "==" mean two different things in Javascript and Ruby.
Parantheses are not required to invoke a method in Ruby.
Ruby's convention is to use the snake_case in naming variables and functions.
```
