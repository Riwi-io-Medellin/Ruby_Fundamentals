### Solutions: Data Types and Collections in Ruby

Below are the solutions to the exercises on data types and collections. Compare these with your implementations to understand better.

---

#### **Solution 1: Strings**

```ruby
# Define the string variable
name = "Ruby"
# Use string interpolation
puts "Hello, #{name}!" # Output: "Hello, Ruby!"
```

---

#### **Solution 2: Numbers**

```ruby
# Define the square method
def square(number)
  number * number
end

# Example call
puts square(4) # Output: 16
```

---

#### **Solution 3: Arrays**

```ruby
# Define the array
colors = ["red", "blue", "green"]
# Add a new color
colors << "yellow"
# Print the length
puts colors.length # Output: 4
```

---

#### **Solution 4: Hashes**

```ruby
# Define the hash
book = { title: "To Kill a Mockingbird", author: "Harper Lee", year: 1960 }
# Access the title
puts book[:title] # Output: "To Kill a Mockingbird"
```

---

#### **Solution 5: Ranges**

```ruby
# Define the range
range = (1..10)
# Check if 7 is included
puts range.include?(7) # Output: true
```

---

#### **Solution 6: Booleans**

```ruby
# Define the is_even? method
def is_even?(number)
  number % 2 == 0
end

# Example call
puts is_even?(4) # Output: true
puts is_even?(5) # Output: false
```

---

#### **Solution 7: Symbols**

```ruby
# Define the hash
user_profile = { name: "Alice", age: 30, email: "alice@example.com" }
# Print the email
puts user_profile[:email] # Output: "alice@example.com"
```

---

By reviewing these solutions, you can solidify your understanding of Ruby's data types and collections. Practice modifying these examples to create your own implementations.