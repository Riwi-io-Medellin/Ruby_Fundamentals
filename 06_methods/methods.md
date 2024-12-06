### Methods in Ruby

Methods are one of the fundamental building blocks of Ruby programming. They allow you to encapsulate reusable logic, improve code readability, and reduce repetition. Ruby provides a flexible way to create and use methods with features like parameters, return values, default arguments, and advanced constructs such as blocks, procs, and lambdas.

---

## **1. Creating and Using Methods**

A method in Ruby is defined using the `def` keyword, followed by the method name. The method body contains the logic to execute, and it ends with the `end` keyword.

### Key Points:
- **Method names** should follow Ruby's naming conventions (snake_case).
- Methods can be called by their name after definition.
- Methods can accept arguments, return values, or perform specific tasks without returning anything.

### Syntax:
```ruby
def method_name(parameters)
  # logic here
end
```

Example (Minimal Explanation):  
```ruby
def greet
  puts "Hello, world!"
end
```

---

## **2. Parameters and Return Values**

Methods in Ruby can take **parameters**, which are placeholders for values passed to the method during its call.

### Parameters:
- Specified in parentheses after the method name.
- Used within the method body to work with the input.

### Return Values:
- Ruby methods return the value of the last evaluated expression by default.
- You can also explicitly return a value using the `return` keyword.

### Syntax:
```ruby
def add(a, b)
  a + b  # Implicit return
end

def multiply(a, b)
  return a * b  # Explicit return
end
```

---

## **3. Default Arguments**

Ruby allows methods to have **default arguments**. These arguments take a default value if no value is provided during the method call.

### Key Points:
- Default values are specified when defining the method.
- If an argument is passed during the method call, it overrides the default.

### Syntax:
```ruby
def greet(name = "Guest")
  puts "Hello, #{name}!"
end
```

Example (Minimal Explanation):  
Calling `greet` with no arguments will use the default value "Guest".

---

## **4. Blocks**

Blocks are anonymous pieces of code passed to methods. They are enclosed in `{}` for single-line blocks or `do...end` for multi-line blocks.

### Key Points:
- Blocks are commonly used with iterators like `each`.
- A method can execute the block using the `yield` keyword.

### Syntax:
```ruby
def perform_task
  puts "Starting task..."
  yield if block_given?  # Execute the block if provided
  puts "Task finished!"
end
```

---

## **5. Procs**

A **proc** (short for procedure) is an object that encapsulates a block of code. Unlike blocks, procs can be assigned to variables and reused.

### Key Points:
- Created using `Proc.new` or `proc`.
- Called using the `call` method.

### Syntax:
```ruby
my_proc = Proc.new { |x| puts "The number is #{x}" }
my_proc.call(5)
```

---

## **6. Lambdas**

A **lambda** is similar to a proc but has stricter rules:
- It checks the number of arguments passed during a call.
- Returning from a lambda exits only the lambda, not the enclosing method.

### Key Points:
- Created using the `lambda` keyword or the `->` syntax.
- Called using the `call` method.

### Syntax:
```ruby
my_lambda = lambda { |x| puts "Hello, #{x}" }
my_lambda.call("Ruby")
```

---

## **7. Differences Between Blocks, Procs, and Lambdas**

| Feature                | Blocks                     | Procs                      | Lambdas                    |
|------------------------|----------------------------|----------------------------|----------------------------|
| **Syntax**             | `{}` or `do...end`         | `Proc.new` or `proc`       | `lambda` or `->`           |
| **Argument Checking**  | No                         | No                         | Yes                        |
| **Return Behavior**    | Exits from method          | Exits from method          | Exits from lambda only     |
| **Reuse**              | No                         | Yes                        | Yes                        |

---
### Predefined Methods in Ruby

Ruby comes with a rich set of predefined methods that are part of its core library. These methods are available across different classes and modules, providing a wide range of functionality without requiring additional installation or definition. Here’s a categorized list of commonly used predefined methods in Ruby:

---

## **1. String Methods**

Strings in Ruby have numerous built-in methods to manipulate text:

- **Length and Case**
  - `length` / `size`: Returns the number of characters.
  - `upcase` / `downcase`: Converts all characters to uppercase/lowercase.
  - `capitalize`: Capitalizes the first character.
  - `swapcase`: Switches the case of each character.

- **Manipulation**
  - `concat`: Concatenates strings.
  - `strip`: Removes leading and trailing whitespace.
  - `chomp`: Removes the trailing newline character.
  - `gsub`: Replaces substrings based on a pattern.

- **Query**
  - `include?`: Checks if a substring is present.
  - `start_with?` / `end_with?`: Checks if the string starts/ends with a substring.

---

## **2. Array Methods**

Arrays have built-in methods for working with collections:

- **Access and Query**
  - `first` / `last`: Returns the first/last element.
  - `length` / `size`: Returns the number of elements.
  - `empty?`: Checks if the array is empty.
  - `include?`: Checks if an element exists.

- **Transformation**
  - `map`: Applies a block to each element, returning a new array.
  - `flatten`: Converts nested arrays into a single-level array.
  - `reverse`: Reverses the order of elements.

- **Addition and Removal**
  - `push` / `<<`: Adds an element to the end.
  - `pop`: Removes and returns the last element.
  - `shift` / `unshift`: Removes/adds elements from/to the start.

---

## **3. Hash Methods**

Hashes store key-value pairs and provide powerful methods:

- **Access and Query**
  - `keys`: Returns an array of all keys.
  - `values`: Returns an array of all values.
  - `has_key?` / `has_value?`: Checks for a specific key/value.

- **Manipulation**
  - `merge`: Combines two hashes into one.
  - `delete`: Removes a key-value pair by key.
  - `invert`: Swaps keys and values.

---

## **4. Enumerable Methods**

The `Enumerable` module provides methods for collections like arrays and hashes:

- `each`: Iterates over each element.
- `select` / `reject`: Returns elements that match/do not match a condition.
- `find`: Returns the first element that matches a condition.
- `reduce` / `inject`: Combines elements to produce a single value.
- `sort` / `sort_by`: Sorts elements based on criteria.

---

## **5. Numeric Methods**

Numeric methods provide utilities for integers and floats:

- **Basic Math**
  - `abs`: Returns the absolute value.
  - `ceil` / `floor`: Rounds up/down to the nearest integer.
  - `round`: Rounds to the nearest integer or specified decimal places.

- **Comparison**
  - `even?` / `odd?`: Checks if a number is even/odd.
  - `positive?` / `negative?`: Checks the sign of a number.

---

## **6. Time Methods**

Ruby’s `Time` class provides methods for working with dates and times:

- **Current Time**
  - `now`: Returns the current time.
  - `today`: Returns the current date.

- **Formatting**
  - `strftime`: Formats the time based on a specified pattern.

- **Manipulation**
  - `+` / `-`: Adds or subtracts seconds to/from a time object.

---

## **7. File Methods**

The `File` class provides methods for handling files:

- **File Information**
  - `exist?`: Checks if a file exists.
  - `size`: Returns the size of the file.
  - `directory?`: Checks if a path is a directory.

- **Reading and Writing**
  - `read`: Reads the contents of a file.
  - `write`: Writes data to a file.
  - `open`: Opens a file for reading or writing.

---

## **8. Kernel Methods**

The `Kernel` module provides globally available methods:

- `puts`: Prints output with a newline.
- `print`: Prints output without a newline.
- `gets`: Reads user input from the console.
- `sleep`: Pauses the program for a specified number of seconds.

---

## **How to Explore More**

You can explore Ruby’s predefined methods further by using the `ri` (Ruby Interactive) tool or the official Ruby documentation:

- **Check methods for a class**:
  ```bash
  ri String
  ```

- **Check details for a method**:
  ```bash
  ri Array#map
  ```

For a comprehensive list of predefined methods, visit the [Ruby Documentation](https://ruby-doc.org/).

## **Best Practices**

1. **Use Methods to Encapsulate Logic**:
   - Methods should perform a single, well-defined task.
   - Avoid overly long methods to keep code maintainable.

2. **Use Default Arguments for Flexibility**:
   - Default arguments make your methods more versatile and reduce the need for method overloading.

3. **Prefer Lambdas for Argument Checking**:
   - Use lambdas when you need stricter control over the number of arguments passed.

4. **Leverage Blocks for Iteration**:
   - Blocks are great for methods that iterate over collections or perform temporary actions.

5. **Use Procs for Reusable Code**:
   - Procs are ideal for scenarios where the same block of code needs to be reused multiple times.

---



For practical exercises and challenges, refer to:

- [Go to exercises: Control Structures](./exercise_methods.md)