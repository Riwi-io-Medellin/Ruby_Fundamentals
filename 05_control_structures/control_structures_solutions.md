### Solutions: Control Structures in Ruby

Here are the solutions to the exercises on control structures in Ruby. Compare your answers to these solutions to enhance your understanding.

---

#### **Solution 1: Basic `if` and `else`**

```ruby
# Input a number
number = gets.to_i

# Check if the number is positive, negative, or zero
if number > 0
  puts "The number is positive."
elsif number < 0
  puts "The number is negative."
else
  puts "The number is zero."
end
```

---

#### **Solution 2: `unless` Statement**

```ruby
# Input a number
number = gets.to_i

# Check if the number is not divisible by 5
unless number % 5 == 0
  puts "The number is not divisible by 5."
end
```

---

#### **Solution 3: `while` Loop**

```ruby
# Initialize a counter
counter = 1

# Print numbers from 1 to 10
while counter <= 10
  puts counter
  counter += 1
end
```

---

#### **Solution 4: `until` Loop**

```ruby
# Initialize a counter
counter = 10

# Print numbers from 10 to 1
until counter < 1
  puts counter
  counter -= 1
end
```

---

#### **Solution 5: `for` Loop**

```ruby
# Initialize the sum
sum = 0

# Calculate the sum using a for loop
for number in 1..100
  sum += number
end

puts "The sum of numbers from 1 to 100 is: #{sum}"
```

---

#### **Solution 6: `each` Loop**

```ruby
# Define an array of names
names = ["Alice", "Bob", "Charlie"]

# Print a personalized greeting for each name
names.each do |name|
  puts "Hello, #{name}!"
end
```

---

#### **Solution 7: `case` Statement**

```ruby
# Input a grade
grade = gets.chomp.upcase

# Print the corresponding description
case grade
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

#### **Solution 8: Combining Loops and Conditional Statements**

```ruby
# Loop through numbers from 1 to 20
for number in 1..20
  # Print only even numbers
  if number % 2 == 0
    puts number
  end
end
```

---

By reviewing these solutions, you can solidify your understanding of Ruby’s control structures. Experiment with these solutions to explore alternative approaches or variations to deepen your knowledge.

### [Back to menu](../README.md)