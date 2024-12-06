### Solutions: Logical and Comparison Operators in Ruby

Here are the solutions for the exercises on logical and comparison operators. Compare these answers with your code to understand the concepts better.

---

#### **Solution 1: Logical AND and OR**

```ruby
# Define a variable
number = 50

# Check if the number is within the range
if number >= 1 && number <= 100
  puts "The number #{number} is within the range."
else
  puts "The number #{number} is out of range."
end
```

---

#### **Solution 2: Combining NOT with Logical Operators**

```ruby
# Define variables
logged_in = false
admin = false

# Check if access is denied
if !(logged_in || admin)
  puts "Access denied."
else
  puts "Access granted."
end
```

---

#### **Solution 3: Comparison Operators**

```ruby
# Define two numbers
num1 = 10
num2 = 20

# Compare the numbers
if num1 > num2
  puts "#{num1} is greater than #{num2}."
elsif num1 < num2
  puts "#{num2} is greater than #{num1}."
else
  puts "#{num1} and #{num2} are equal."
end
```

---

#### **Solution 4: Spaceship Operator**

```ruby
# Define an array of numbers
numbers = [5, 2, 9, 1, 3]

# Sort the array using the spaceship operator
sorted_numbers = numbers.sort { |a, b| a <=> b }

# Print the sorted array
puts "Sorted numbers: #{sorted_numbers}"
```

---

#### **Solution 5: Complex Conditions**

```ruby
# Define variables
age = 20
citizen = true

# Check eligibility
if age >= 18 && citizen
  puts "You are eligible to vote."
else
  puts "You are not eligible to vote."
end
```

---

#### **Solution 6: Equality and Identity**

```ruby
# Define two strings
string1 = "hello"
string2 = "hello"

# Check equality
if string1 == string2
  puts "The strings are equal in value."
else
  puts "The strings are not equal in value."
end

# Check object identity
if string1.equal?(string2)
  puts "The strings are the same object."
else
  puts "The strings are different objects."
end
```

### [Back to menu](../README.md)
