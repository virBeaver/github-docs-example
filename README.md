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
> Here is an example of using a codeblock for an error that appears in bash.

## Step 2 - How to take screenshots

A screenshot is when you capture a part of your screen from your laptop, desktop or phone.

> This is **not** to be confused with take a photo with your phone.

To take screenshots both on macOS and Windows, you can use the following hotkeys:

**On macOS (formerly Mac OS X):**

1. **Entire Screen:**
   - Command (⌘) + Shift + 3

2. **Selected Portion:**
   - Command (⌘) + Shift + 4, then drag to select the area you want to capture.

3. **Window:**
   - Command (⌘) + Shift + 4, then press Spacebar. Click the window you want to capture.

4. **Entire Screen and save to clipboard (instead of saving to a file):**
   - Command (⌘) + Control + Shift + 3

5. **Selected Portion and save to clipboard:**
   - Command (⌘) + Control + Shift + 4, then drag to select the area.

By default, screenshots on macOS are saved to the desktop with a name like "Screen Shot YYYY-MM-DD at HH.MM.SS AM/PM."

**On Windows:**

1. **Entire Screen:**
   - Print Screen (often labeled as PrtScn)

2. **Active Window:**
   - Alt + Print Screen

3. **Selected Portion (Windows 10 and later):**
   - Windows + Shift + S (This will open up a snipping tool interface allowing you to select a portion of the screen. The screenshot will be saved to your clipboard.)

4. **Using Snipping Tool:**
   - This isn't a hotkey per se, but Windows has a built-in app called Snipping Tool which allows for various screenshot options. You can search for it in the Start menu.

5. **Save the Entire Screen directly as a file (Windows 8 and later):**
   - Windows + Print Screen (The screenshot will be saved in the "Screenshots" folder inside the "Pictures" library.)

Remember, after taking a screenshot, you can paste it directly into most applications (like Paint or Word) using the paste function (Command/Control + V).


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

[Secret Window Hidden Garden]()

## External References

- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/). 
- [Basic writing and formatting syntax (Github Flavored Markdown)](https://docs.github.com/de/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#images).
- [GFM - Task Lists]([<sub>[1]</sub>z](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists)https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists). <sup>[1]</sup>
- [GFM - Emoji Cheatsheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md#emoji-cheat-sheet).
- [GFM - Tables (with extensions)](https://github.github.com/gfm/#tables-extension-). <sup>[2]</sup>
