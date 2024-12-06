### Exercises: Control Structures in Ruby

These exercises are designed to help you practice and understand Ruby's control structures. Each exercise focuses on a specific concept covered in the theory. Try to complete them before checking the solutions file.

---

#### **Exercise 1: Basic `if` and `else`**

Write a program that takes a number as input and checks if it is positive, negative, or zero. Print the result.

```ruby
# Input a number
number = gets.to_i

# Check if the number is positive, negative, or zero
if ___________
  puts "The number is positive."
elsif ___________
  puts "The number is negative."
else
  puts "The number is zero."
end
```

---

#### **Exercise 2: `unless` Statement**

Write a program that checks if a user-provided number is not divisible by 5 and prints a message if it is not.

```ruby
# Input a number
number = gets.to_i

# Check if the number is not divisible by 5
unless ___________
  puts "The number is not divisible by 5."
end
```

---

#### **Exercise 3: `while` Loop**

Write a program that prints all numbers from 1 to 10 using a `while` loop.

```ruby
# Initialize a counter
counter = 1

# Print numbers from 1 to 10
while ___________
  puts counter
  counter += 1
end
```

---

#### **Exercise 4: `until` Loop**

Write a program that prints numbers from 10 down to 1 using an `until` loop.

```ruby
# Initialize a counter
counter = 10

# Print numbers from 10 to 1
until ___________
  puts counter
  counter -= 1
end
```

---

#### **Exercise 5: `for` Loop**

Write a program that calculates the sum of numbers from 1 to 100 using a `for` loop.

```ruby
# Initialize the sum
sum = 0

# Calculate the sum using a for loop
for ___________
  sum += number
end

puts "The sum of numbers from 1 to 100 is: #{sum}"
```

---

#### **Exercise 6: `each` Loop**

Write a program that iterates through an array of names and prints a personalized greeting for each name.

```ruby
# Define an array of names
names = ["Alice", "Bob", "Charlie"]

# Print a personalized greeting for each name
names.each do |name|
  puts "Hello, ___________!"
end
```

---

#### **Exercise 7: `case` Statement**

Write a program that takes a grade (A, B, C, D, F) as input and prints the corresponding description:

- A: "Excellent"
- B: "Good"
- C: "Average"
- D: "Below Average"
- F: "Fail"

```ruby
# Input a grade
grade = gets.chomp.upcase

# Print the corresponding description
case ___________
when "A"
  puts "Excellent"
when "B"
  puts "Good"
when "C"
  puts "Average"
when "D"
  puts "Below Average"
when "F"
  puts "Fail"
else
  puts "Invalid grade."
end
```

---

#### **Exercise 8: Combining Loops and Conditional Statements**

Write a program that prints all even numbers from 1 to 20 using a loop and a conditional statement.

```ruby
# Loop through numbers from 1 to 20
for ___________
  # Print only even numbers
  if ___________
    puts number
  end
end
```

---

### [Go to Solutions](./control_structures_solutions.md)

These exercises will strengthen your understanding of control structures in Ruby. Once you’ve completed them, check your answers in the solutions file.