### Exercises: Methods in Ruby

These exercises are designed to help you practice creating and using methods in Ruby, covering parameters, return values, default arguments, and blocks, procs, and lambdas. Attempt each exercise before checking the solutions.

---

#### **Exercise 1: Basic Method**
Create a method `greet` that takes no arguments and prints "Hello, Ruby!".

```ruby
# Define the method greet
def greet
  # Your code here
end

# Call the method
greet
```

---

#### **Exercise 2: Method with Parameters**
Write a method `add` that takes two numbers as parameters and returns their sum.

```ruby
# Define the method add
def add(a, b)
  # Your code here
end

# Call the method and print the result
puts add(5, 10)
```

---

#### **Exercise 3: Method with Default Arguments**
Create a method `greet_user` that takes one parameter `name` and prints "Hello, [name]!". If no name is provided, it should default to "Guest".

```ruby
# Define the method greet_user
def greet_user(name = "Guest")
  # Your code here
end

# Call the method with and without arguments
greet_user("Alice")
greet_user
```

---

#### **Exercise 4: Method with Explicit Return**
Write a method `multiply` that takes two numbers as parameters and explicitly returns their product.

```ruby
# Define the method multiply
def multiply(a, b)
  # Your code here
end

# Call the method and print the result
puts multiply(3, 4)
```

---

#### **Exercise 5: Using Blocks**
Create a method `perform_task` that takes a block. The method should print "Starting task..." before executing the block and "Task completed!" afterward.

```ruby
# Define the method perform_task
def perform_task
  # Your code here
end

# Call the method with a block
perform_task do
  puts "This is the task being performed."
end
```

---

#### **Exercise 6: Using Procs**
Write a method `apply_proc` that takes a proc and a number as arguments, then calls the proc with the number.

```ruby
# Define the method apply_proc
def apply_proc(proc, num)
  # Your code here
end

# Create a proc and test the method
my_proc = Proc.new { |x| x * 2 }
puts apply_proc(my_proc, 5)
```

---

#### **Exercise 7: Using Lambdas**
Write a method `apply_lambda` that takes a lambda and a string as arguments, then calls the lambda with the string.

```ruby
# Define the method apply_lambda
def apply_lambda(lambda_func, str)
  # Your code here
end

# Create a lambda and test the method
my_lambda = ->(name) { "Hello, #{name}!" }
puts apply_lambda(my_lambda, "Ruby")
```

---

#### **Exercise 8: Combining Methods and Blocks**
Write a method `repeat_task` that takes a block and a number `n`, and executes the block `n` times.

```ruby
# Define the method repeat_task
def repeat_task(n)
  # Your code here
end

# Call the method with a block
repeat_task(3) do
  puts "Repeating task..."
end
```

---

#### **Exercise 9: Method with Variable Parameters**
Create a method `sum_all` that takes a variable number of arguments and returns their sum.

```ruby
# Define the method sum_all
def sum_all(*numbers)
  # Your code here
end

# Test the method
puts sum_all(1, 2, 3, 4, 5)
```

---

### [Go to Solutions](./methods_solutions.md)
These exercises are designed to help you master Ruby methods and their various features. Once you've completed them, check your answers in the solutions file.
