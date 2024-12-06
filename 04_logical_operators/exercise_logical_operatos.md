### Exercises: Logical and Comparison Operators in Ruby

These exercises will help you practice and solidify your understanding of logical and comparison operators in Ruby. Try to complete each one and test your code to ensure it behaves as expected. Solutions will be available for reference.

---

#### **Exercise 1: Logical AND and OR**
Write a program that checks if a number is within the range 1 to 100, inclusive, and prints a message indicating whether it is valid or not.

```ruby
# Define a variable
number = 50

# Check if the number is within the range
if ___________
  puts "The number #{number} is within the range."
else
  puts "The number #{number} is out of range."
end
```

---

#### **Exercise 2: Combining NOT with Logical Operators**
Write a program that checks if a user is either logged in or an admin and prints a message if access is denied.

```ruby
# Define variables
logged_in = false
admin = false   

# Check if access is denied
if ___________
  puts "Access denied."
else
  puts "Access granted."
end
```

---

#### **Exercise 3: Comparison Operators**
Write a program that compares two numbers and prints which one is greater, or if they are equal.

```ruby
# Define two numbers
num1 = 10
num2 = 20

# Compare the numbers
if ___________
  puts "#{num1} is greater than #{num2}."
elsif ___________
  puts "#{num2} is greater than #{num1}."
else
  puts "#{num1} and #{num2} are equal."
end
```

---

#### **Exercise 4: Spaceship Operator**
Use the spaceship operator to sort an array of numbers in ascending order.

```ruby
# Define an array of numbers
numbers = [5, 2, 9, 1, 3]

# Sort the array using the spaceship operator
sorted_numbers = numbers.sort { |a, b| ___________ }

# Print the sorted array
puts "Sorted numbers: #{sorted_numbers}"
```

---

#### **Exercise 5: Complex Conditions**
Write a program that checks if a person is eligible to vote. The conditions are:
- The person must be at least 18 years old.
- The person must be a citizen.

```ruby
# Define variables
age = 20
citizen = true

# Check eligibility
if ___________
  puts "You are eligible to vote."
else
  puts "You are not eligible to vote."
end
```

---

#### **Exercise 6: Equality and Identity**
Write a program to check if two strings are equal in value and if they refer to the same object in memory.

```ruby
# Define two strings
string1 = "hello"
string2 = "hello"

# Check equality
if ___________
  puts "The strings are equal in value."
else
  puts "The strings are not equal in value."
end

# Check object identity
if ___________
  puts "The strings are the same object."
else
  puts "The strings are different objects."
end
```

---

### [Go to Solutions](./operators_solutions.md)

These exercises provide hands-on practice with logical and comparison operators. After completing them, check your answers in the solutions file.