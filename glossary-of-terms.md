# Glossary of Terms

#### Argument

An input to a [method](#method):

```ruby
"well, hello!".gsub("ll", "✌️") # => "we✌️, he✌️o!"
```

In the example above, the strings `"ll"` and `"✌️"` are both arguments to the method `gsub`.

The syntax for giving a method its arguments is to put them within parentheses immediately following the method's name; and if there are multiple arguments, then they are separated by commas.

While Ruby is pretty flexible about whitespace most of the time, remember: **don't put a space between the method's name and the parentheses that contain its arguments!**

Ruby does allow you to, optionally, omit the parentheses; and some Rubyists do prefer that style. So when you are reading Ruby around the internet, you will encounter things like this:

```ruby
"well, hello!".gsub "ll", "✌️"
```

It's just a matter of taste which style you use, but definitely don't use both parentheses _and_ a space, like this

```ruby
"well, hello!".gsub ("ll", "✌️") # wrong!
```

Personally, I prefer using the parentheses around arguments to keep it clear what goes with what. Otherwise I get confused, especially when there's more than one method on the same line.


#### Array

One of the built-in Ruby [classes](#class). It is one of the two primary classes we use to represent **lists of things**. (The other one is [`Hash`](#hash).)

Ruby represents the list within square brackets, with each element separated by a comma:

```ruby
["doug", "alice", "carol", "bob"]
```

Each element of an `Array` can be any Ruby object — even another `Array`.

A blank instance of `Array` can be created like any Ruby object, by calling `.new` on the class:

```ruby
a = Array.new
```

or by using the square bracket shorthand:

```ruby
a = []
```

You can add elements to an array with the `.push()` method, which takes one argument; the object you want to add to the end of array:

```ruby
a.push("doug")
a.push("alice")
a.push("carol")
a.push("bob")
```

There is also a shorthand for adding elements to an array with the `<<` ("**shovel**") operator:

```ruby
a << "doug"
a << "alice"
a << "carol"
a << "bob"
```

You can also pre-populate the array _in one fell swoop_ when you create it:

```ruby
a = ["doug", "alice", "carol", "bob"]
```

You can then access elements in the array by position number with the `.at()` method:

```ruby
a.at(1) # => "alice"
```

Notice that position numbers begin at `0`, not `1` as you might expect.

There is also a square bracket shorthand for accessing elements:

```ruby
a[1] # => "alice"
```

[Read more about arrays here.](https://guides.firstdraft.com/fundamental-classes.html#arrays)

#### Block

#### Box

#### Chain

#### Class

#### Def

#### Div

#### Do

#### Each

#### Element

#### Expression

#### Fixnum

One of the built-in Ruby [classes](#class).

#### Float

One of the built-in Ruby [classes](#class).

#### Gem

#### Hash

One of the built-in Ruby [classes](#class). It is one of the two primary classes we use to represent **lists of things**. (The other one is [`Array`](#array).)

Ruby represents the list within curly brackets, with each element separated by a comma:

```ruby
{ :first_name => "Raghu", :last_name => "Betina", :role => "Instructor" }
```

Each element in a `Hash` consists of a **key/value pair**. The key comes first and is separated from the value by a `=>`, which is called a **hash rocket**.

Technically, the key can be any Ruby object, but we almost always use [`Symbol`s](#symbol), if we have a choice in the matter.

The value can can be any Ruby object — even another `Hash`, or an [`Array`](#array).

A blank instance of `Hash` can be created like any Ruby object, by calling `.new` on the class:

```ruby
h = Hash.new
```

or by using the curly bracket shorthand:

```ruby
h = {}
```

You can add elements to a hash with the `.store()` method, which takes two arguments; the first is the key you want to store an object under, and the second is the object you want to store:

```ruby
h.store(:first_name, "Raghu")
h.store(:last_name, "Betina")
h.store(:role, "Instructor")
```

There is also a square bracket shorthand for storing elements in a hash:

```ruby
h[:first_name] = "Raghu"
h[:last_name] = "Betina"
h[:role] = "Instructor"
```

You can also pre-populate the hash _in one fell swoop_ when you create it:

```ruby
h = { :first_name => "Raghu", :last_name => "Betina", :role => "Instructor" }
```

You can then access elements in the hash by key number with the `.fetch()` method:

```ruby
h.fetch(:role) # => "Instructor"
```

There is also a square bracket shorthand for accessing elements:

```ruby
h[:role] # => "Instructor"
```

[Read more about hashes here.](https://guides.firstdraft.com/ruby-hashes.html)

#### Instance Variable

#### Key

#### Label

#### Loop

#### Method

#### Object

#### Operator

#### Render

#### Scrape

#### Source

#### String

One of the built-in Ruby [classes](#class).

#### Symbol

One of the built-in Ruby [classes](#class).

#### Table

#### Value

#### Variable