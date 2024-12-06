### Control Structures in Ruby

Control structures are essential in programming as they allow you to control the flow of your program based on conditions, loops, or cases. Ruby provides a variety of control structures to handle decision-making and iteration. This document focuses on the theoretical understanding of these control structures.

---

## **1. Conditional Statements**

Conditional statements are used to execute specific blocks of code based on whether a condition evaluates to `true` or `false`.

### **`if` Statement**

- The `if` statement is used to check a condition and execute code if the condition is `true`.
- Syntax:
  ```ruby
  if condition
    # code to execute if condition is true
  end
  ```

### **`else` Statement**

- Used to specify code that runs when the `if` condition is `false`.
- Syntax:
  ```ruby
  if condition
    # code if condition is true
  else
    # code if condition is false
  end
  ```

### **`elsif` Statement**

- Adds additional conditions to an `if-else` structure.
- Syntax:
  ```ruby
  if condition1
    # code if condition1 is true
  elsif condition2
    # code if condition2 is true
  else
    # code if none of the conditions are true
  end
  ```

### **`unless` Statement**

- Executes code if the condition is `false`.
- Syntax:
  ```ruby
  unless condition
    # code to execute if condition is false
  end
  ```

---

## **2. Loops**

Loops are used to repeat a block of code multiple times. Ruby offers several looping constructs to suit different needs.

### **`while` Loop**

- Repeats the block of code as long as the condition is `true`.
- Syntax:
  ```ruby
  while condition
    # code to execute while condition is true
  end
  ```

### **`until` Loop**

- Repeats the block of code until the condition becomes `true`.
- Syntax:
  ```ruby
  until condition
    # code to execute until condition is true
  end
  ```

### **`for` Loop**

- Iterates over a range or collection.
- Syntax:
  ```ruby
  for variable in collection
    # code to execute for each element in collection
  end
  ```

### **`each` Loop**

- A common way to iterate over collections such as arrays or hashes.
- Syntax:
  ```ruby
  collection.each do |element|
    # code to execute for each element
  end
  ```

---

## **3. `case` Statement**

The `case` statement in Ruby is a powerful control structure for selecting one of many blocks of code to execute based on a specific value.

- Syntax:
  ```ruby
  case variable
  when value1
    # code to execute if variable equals value1
  when value2
    # code to execute if variable equals value2
  else
    # code to execute if no conditions match
  end
  ```

- Key Features:
  - The `case` statement is more readable than a long chain of `if-elsif` statements.
  - It uses the `===` operator for comparison, making it flexible for pattern matching.

---

## **Key Points to Remember**

1. **Condition Evaluation**:
   - Ruby evaluates conditions based on truthy and falsy values.
   - `nil` and `false` are the only falsy values; everything else is truthy, including `0` and empty strings.

2. **Modifiers**:
   - Ruby allows conditional and loop constructs to be written in a single line as modifiers:
     ```ruby
     puts "Condition met!" if condition
     puts "Looping..." while condition
     ```

3. **Break and Next**:
   - `break`: Exits a loop immediately.
   - `next`: Skips the current iteration and moves to the next one.

4. **Iterators**:
   - Use iterators like `each` for readability and flexibility.
   - Iterators are preferable to `for` loops in most cases.

5. **Indentation**:
   - Ruby relies on proper indentation and clean syntax to improve readability. Always use consistent formatting for better code maintainability.

---

This theoretical overview provides a foundation for understanding Ruby’s control structures. For practical applications and examples, refer to the exercises and solutions in their respective files:

- [Exercises: Control Structures](./exercise_control_structures.md)