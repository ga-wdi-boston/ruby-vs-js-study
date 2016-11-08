# Ruby versus Javascript Study

Use your favorite search engine and any other resources to research and respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your search. We ask you to write responses in your own words in order to see how you process what you've read. Please do not respond with direct quotes from source material. Instead, digest what you've read and repeat it in your own voice.

Use `grunt test` to test your code.

## Comparison

Describe three examples of differens between Ruby and Javasctipt?

```markdown
1. The use of semi-colons. 2. "Puts" as a return statment of sorts
3. Loop syntax ie:
i=0
loop do
  i+=1
end
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

```markdown
Person = {}
[:name]="Jason"
```

## Ruby vs. Javascript :: String Methods

1. Open pry in your terminal and input `str = "ylbmessa lareneg`
2. With what you now know about ruby methods, reverse the string so that the output reads `"general assembly"` change the string into an array of characters so that the ouput reads : `["g", "e", "n", "e", "r", "a", "l", " ", "a", "s", "s", "e", "m", "b", "l", "y"]`
3. Then change your new array back into a string with hyphens in between characters so that your result is `"g-e-n-e-r-a-l- -a-s-s-e-m-b-l-y"`.
4. Even better if you can do so while removing the two `- -`'s between `general` and `assembly`

```markdown
str.reverse.split("").to_s.delete('\\" ')```

## What are three common "gotchas" in Ruby after learning Javscript.

```markdown
Boolean comparions do not behave the same ie: === and ==. Variables with capitol letters are defined as constant. Negative index calls that exceed the amount of indecies for an array will return the last value and not undefined.  
```
