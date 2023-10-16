# Writing Good Documentation

## Step 1 - Using Codeblocks.

Codeblocks in markdown make it *very easy* for tech people to **copy, paste, share** code.
A good **Cloud Engineer** uses Codeblocks whenever possible.

Because it allows others to copy and paste their code to replicate or research issues.

- In order to ceate codeblocks in makdown you need to use three backticks (`)
- Not to be confused with single quotation `'`


```
class Person
  attr_accessor :name, :age

  # Constructor method
  def initialize(name, age)
    @name = name
    @age = age
  end

  # Instance method to introduce the person
  def introduce
    puts "Hello, my name is #{@name} and I am #{@age} years old."
  end

  # Instance method to check if person is an adult
  def adult?
    @age >= 18
  end
end

# Create a new person instance
john = Person.new("John", 25)

# Introduce the person
john.introduce

# Check if the person is an adult
if john.adult?
  puts "#{john.name} is an adult."
else
  puts "#{john.name} is not an adult."
end
```

- When you can you should attempt to apply syntax higlighting to your codeblocks

```ruby
class Person
  attr_accessor :name, :age

  # Constructor method
  def initialize(name, age)
    @name = name
    @age = age
  end

  # Instance method to introduce the person
  def introduce
    puts "Hello, my name is #{@name} and I am #{@age} years old."
  end

  # Instance method to check if person is an adult
  def adult?
    @age >= 18
  end
end

# Create a new person instance
john = Person.new("John", 25)

# Introduce the person
john.introduce

# Check if the person is an adult
if john.adult?
  puts "#{john.name} is an adult."
else
  puts "#{john.name} is not an adult."
end
```

Just a random downsized picture of showing an image of an Octocat smiling and raising a tentacle

<img width="200px" src="https://myoctocat.com/assets/images/base-octocat.svg" />

Good Cloud Engineers use codeblocks for both Code and Errors that appear in the console.

```bash
Traceback (most recent call list):
  2: from /us/bin/irb:23:in `<main>'
  1: from (irb):1
RunetimeError: This is a custom error message
```
> Here is ab example of using a codeblock for an error that appears in bash.


## Step 3 - Use gitHub Flavoured  Markdown Task Lists

GitHub extends Markdown to have a list where you can check of items. [<sup>[1]</sup>](#external-references)

- [ ] Finish Step 1
- [ ] Finish Step 2
- [ ] Finish Step 3

## Step 4 - Use Emojis (optional)

GitHub Flavored Markdown (GFM) supports emoji shortcodes.
Here are some examples:

| Name | Shortcode | Emoji | 
| --- | --- | --- |
| Cloud | `:cloud:` | :cloud: |
| Cloud | `:cloud_with_lightning:` | :cloud_with_lightning: |

## Step 5 - How to create a table

You can use the following markdown foirmat to create tables:

```md
| Name | Shortcode | Emoji | 
| --- | --- | --- |
| Cloud | `:cloud:` | :cloud: |
| Cloud | `:cloud_with_lightning:` | :cloud_with_lightning: |
```

GFM extends the functionality of markdown tables to provide more alignment an tabel cell formatinng options. [<sup>[2]</sup>](#external-references)

## External References

- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/). 
- [Basic writing and formatting syntax (Github Flavored Markdown)](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#images).
- [GFM - Task Lists]([<sub>[1]</sub>z](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists)https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists). <sup>[1]</sup>
- [GFM - Emoji Cheatsheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#emoji-cheat-sheet).
- [GFM - Tables (with extensions)](https://github.github.com/gfm/#tables-extension-). <sup>[2]</sup>
