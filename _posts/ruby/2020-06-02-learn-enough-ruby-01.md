---
layout: post
title: Learn Enough Ruby - Chapters 1 - 4
date: 2020-06-02 13:06:57 -7000
tags: ruby
categories: learn-enough
---

## Regex

[rubular](https://rubular.com/)
[regex101](https://regex101.com/)

## Hashes

- Hashes are like key/value pairs. Hash is also called an associative array.

`user["first_name"] = "myFirstName"`
`user["last_name"] = "myLastName"`

- Keys and values can be defined with `=>` , called a “hashrocket” to set more than one set at a time.

`user = {"first_name" => "Buzz", "last_name" => "Aldrin"}`

## Symbols

- Hash keys should be defined as symbols these days, they are like strings but with less baggage.

`user = {:firstname => "Buzz", :lastname => "Aldrin"}`

`user[:firstname]`

- The second syntax that can be used replaces the symbol/hashrocket combination with the name of the key followed by a colon and a value:

`{ name: "Michael Hartl", email: "michael@example.com" }`

## Hash iteration

```
flash = {success: "It worked", danger: "It failed"}

# inspect method, which returns a string with a literal representation of the object it’s called on
flash.each do |key, value|
  puts "key #{key.inspect} has value #{value.inspect}"
end
```

### inspect

- `inspect` is a useful method that returns the literal representation of the object its called on.

`puts (1..5).to_a`
1
2
3
4
5

`puts (1..5).to_a.inspect`
[1, 2, 3, 4, 5]

- You can also call it using `p` instead of `puts`

`p (1..5).to_a`
[1, 2, 3, 4, 5]

## VS code open a file from terminal

[How to open vs code from terminal](https://stackoverflow.com/questions/29971053/how-to-open-visual-studio-code-from-the-command-line-on-osx)

- Then use the command `code hello.rb` or other file to launch it in vs code

## Debugging tips

- chapter 5 section 2 in Hartl book
