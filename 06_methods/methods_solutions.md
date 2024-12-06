### Solutions: Methods in Ruby

Here are the solutions for the exercises on methods in Ruby. Review these solutions to enhance your understanding and compare them with your implementations.

---

#### **Solution 1: Basic Method**

```ruby
# Define the method greet
def greet
  puts "Hello, Ruby!"
end

# Call the method
greet
```

---

#### **Solution 2: Method with Parameters**

```ruby
# Define the method add
def add(a, b)
  a + b
end

# Call the method and print the result
puts add(5, 10)  # Output: 15
```

---

#### **Solution 3: Method with Default Arguments**

```ruby
# Define the method greet_user
def greet_user(name = "Guest")
  puts "Hello, #{name}!"
end

# Call the method with and without arguments
greet_user("Alice")  # Output: Hello, Alice!
greet_user           # Output: Hello, Guest!
```

---

#### **Solution 4: Method with Explicit Return**

```ruby
# Define the method multiply
def multiply(a, b)
  return a * b
end

# Call the method and print the result
puts multiply(3, 4)  # Output: 12
```

---

#### **Solution 5: Using Blocks**

```ruby
# Define the method perform_task
def perform_task
  puts "Starting task..."
  yield if block_given?
  puts "Task completed!"
end

# Call the method with a block
perform_task do
  puts "This is the task being performed."
end

# Output:
# Starting task...
# This is the task being performed.
# Task completed!
```

---

#### **Solution 6: Using Procs**

```ruby
# Define the method apply_proc
def apply_proc(proc, num)
  proc.call(num)
end

# Create a proc and test the method
my_proc = Proc.new { |x| x * 2 }
puts apply_proc(my_proc, 5)  # Output: 10
```

---

#### **Solution 7: Using Lambdas**

```ruby
# Define the method apply_lambda
def apply_lambda(lambda_func, str)
  lambda_func.call(str)
end

# Create a lambda and test the method
my_lambda = ->(name) { "Hello, #{name}!" }
puts apply_lambda(my_lambda, "Ruby")  # Output: Hello, Ruby!
```

---

#### **Solution 8: Combining Methods and Blocks**

```ruby
# Define the method repeat_task
def repeat_task(n)
  n.times { yield if block_given? }
end

# Call the method with a block
repeat_task(3) do
  puts "Repeating task..."
end

# Output:
# Repeating task...
# Repeating task...
# Repeating task...
```

---

#### **Solution 9: Method with Variable Parameters**

```ruby
# Define the method sum_all
def sum_all(*numbers)
  numbers.sum
end

# Test the method
puts sum_all(1, 2, 3, 4, 5)  # Output: 15
```

---
These solutions demonstrate how to effectively use methods in Ruby. Review them carefully, experiment with modifications, and try creating similar exercises to further enhance your skills.

### [Back to menu](../README.md)


