### 3. Variable Types in Ruby

Variables are fundamental in Ruby programming. They allow you to store, manipulate, and retrieve data during the execution of a program. Ruby variables are dynamically typed, meaning you don't need to declare their type explicitly. Here's everything you need to know about variables in Ruby.

---

#### What Are Variables?

Variables in Ruby are containers for storing values. These values can be of different types, such as numbers, strings, or objects. Ruby uses variable names as identifiers to access these stored values.

---

### Types of Variables in Ruby

Ruby has four main types of variables, each serving a distinct purpose and scope:

1. **Local Variables**
   - Local variables are declared with lowercase letters or underscores (`_`) at the beginning of their names.
   - They are only accessible within the block, method, or class where they are defined.
   - Example:
     ```ruby
     name = "Alice"
     age = 25
     puts "Name: #{name}, Age: #{age}"
     ```

2. **Instance Variables**
   - Instance variables begin with an `@` symbol and are specific to an object instance.
   - They are used to store data that belongs to an instance of a class.
   - They are accessible throughout the object but are not shared across instances.
   - Example:
     ```ruby
     class Person
       def initialize(name, age)
         @name = name
         @age = age
       end

       def details
         "Name: #{@name}, Age: #{@age}"
       end
     end

     person = Person.new("Alice", 25)
     puts person.details
     ```

3. **Class Variables**
   - Class variables begin with `@@` and are shared among all instances of a class.
   - They store values that are relevant to the entire class, not individual instances.
   - Example:
     ```ruby
     class Person
       @@population = 0

       def initialize(name)
         @name = name
         @@population += 1
       end

       def self.population
         @@population
       end
     end

     Person.new("Alice")
     Person.new("Bob")
     puts "Population: #{Person.population}"
     ```

4. **Global Variables**
   - Global variables begin with a `$` symbol and are accessible throughout the program, across all classes and methods.
   - They should be used sparingly as they can make code harder to debug and maintain.
   - Example:
     ```ruby
     $global_var = "I am global!"

     def show_global
       puts $global_var
     end

     show_global
     ```

---

### Dynamic Typing in Ruby

In Ruby, variables are dynamically typed, meaning their type is determined at runtime based on the value assigned. For example:

```ruby
value = 42       # value is an Integer
value = "Hello"  # value is now a String
```

This flexibility allows developers to write concise and adaptable code.

---

### Constants

- Constants in Ruby are variables that should not change once assigned. They are declared with an uppercase letter at the beginning of their name.
- Although Ruby allows reassigning constants, it will display a warning.
- Example:
  ```ruby
  PI = 3.14159
  puts PI
  ```

---

### Special Variables in Ruby

Ruby provides several built-in special variables for various purposes. Some of the most commonly used ones include:

- `$0`: The name of the current file.
- `$_`: The last string read by the `gets` method.
- `$?`: The exit status of the last executed child process.
- `$$`: The process ID of the current Ruby program.

Example:
```ruby
puts "This program is running with PID: #{$$}"
```

---

### Variable Scope

The scope of a variable defines where it can be accessed or modified. In Ruby:

- **Local variables** are scoped to the block, method, or class where they are defined.
- **Instance variables** are scoped to the object instance.
- **Class variables** are shared across all instances of the class.
- **Global variables** are accessible anywhere in the program.

---

### Best Practices for Using Variables

1. Use descriptive names for variables to improve code readability:
   ```ruby
   first_name = "Alice"
   ```
2. Avoid using global variables unless absolutely necessary.
3. Use constants for values that should not change.
4. Follow Ruby's naming conventions:
   - Local variables: snake_case
   - Constants: SCREAMING_SNAKE_CASE
   - Instance variables: `@variable`
   - Class variables: `@@variable`

---

### Example Code with All Variable Types

```ruby
class Example
  @@class_count = 0  # Class variable

  def initialize(name)
    @name = name     # Instance variable
    @@class_count += 1
  end

  def self.class_count
    @@class_count
  end

  def show_details
    local_var = "Local variable"  # Local variable
    puts "Name: #{@name}"
    puts local_var
  end
end

$global_var = "Global variable"  # Global variable

example1 = Example.new("Object 1")
example2 = Example.new("Object 2")

example1.show_details
puts "Class count: #{Example.class_count}"
puts "Global: #{$global_var}"
```

---

By mastering Ruby variables and their scopes, you'll be able to write more effective and structured code. Ruby’s flexibility and simplicity make it a powerful tool for managing data within your programs.

Practice the theory with the following exercises.
### . [Variables practice exercise](./exercise_variables.md)
