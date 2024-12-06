### Logical and Comparison Operators in Ruby

Ruby provides a rich set of operators to perform logical and comparison operations. These operators are used to evaluate conditions, perform logical tests, and control the flow of your programs. Below is a detailed explanation of these operators along with examples.

---

## **Logical Operators**

Logical operators are used to combine multiple conditions or invert their outcomes. Ruby provides three main logical operators:

1. **AND (`&&` and `and`)**
   - Returns `true` if both operands are `true`.
   - `&&` has a higher precedence than `and`.
   - Example:
     ```ruby
     puts true && true  # Output: true
     puts true && false # Output: false
     puts true and false # Output: false
     ```

2. **OR (`||` and `or`)**
   - Returns `true` if at least one operand is `true`.
   - `||` has a higher precedence than `or`.
   - Example:
     ```ruby
     puts true || false  # Output: true
     puts false || false # Output: false
     puts true or false  # Output: true
     ```

3. **NOT (`!` and `not`)**
   - Reverses the logical state of its operand.
   - Example:
     ```ruby
     puts !true  # Output: false
     puts !false # Output: true
     puts not true  # Output: false
     ```

---

## **Comparison Operators**

Comparison operators are used to compare two values. They return `true` or `false` based on the result of the comparison.

1. **Equality (`==` and `===`)**
   - `==`: Checks if two values are equal.
   - `===`: Used in case statements and pattern matching.
   - Example:
     ```ruby
     puts 5 == 5  # Output: true
     puts 5 == 3  # Output: false
     puts (1..10) === 5 # Output: true
     ```

2. **Inequality (`!=`)**
   - Checks if two values are not equal.
   - Example:
     ```ruby
     puts 5 != 3  # Output: true
     puts 5 != 5  # Output: false
     ```

3. **Greater Than and Less Than (`>`, `<`, `>=`, `<=`)**
   - `>`: Checks if the left operand is greater than the right.
   - `<`: Checks if the left operand is less than the right.
   - `>=`: Checks if the left operand is greater than or equal to the right.
   - `<=`: Checks if the left operand is less than or equal to the right.
   - Example:
     ```ruby
     puts 10 > 5   # Output: true
     puts 10 < 5   # Output: false
     puts 10 >= 10 # Output: true
     puts 10 <= 9  # Output: false
     ```

4. **Spaceship Operator (`<=>`)**
   - Returns:
     - `-1` if the left operand is less than the right.
     - `0` if the two operands are equal.
     - `1` if the left operand is greater than the right.
   - Example:
     ```ruby
     puts 5 <=> 10  # Output: -1
     puts 10 <=> 10 # Output: 0
     puts 15 <=> 10 # Output: 1
     ```

5. **Equality by Type and Value (`eql?`)**
   - Returns `true` if two values are of the same type and value.
   - Example:
     ```ruby
     puts 5.eql?(5)       # Output: true
     puts 5.eql?(5.0)     # Output: false
     ```

6. **Object Identity (`equal?`)**
   - Returns `true` if two objects have the same object ID.
   - Example:
     ```ruby
     a = "hello"
     b = "hello"
     puts a.equal?(b)  # Output: false
     c = a
     puts a.equal?(c)  # Output: true
     ```

---

## **Examples Combining Logical and Comparison Operators**

1. Checking multiple conditions:
   ```ruby
   age = 25
   puts age > 18 && age < 30  # Output: true
   ```

2. Nested conditions:
   ```ruby
   temperature = 75
   weather = "sunny"
   puts temperature > 70 && weather == "sunny"  # Output: true
   ```

3. Combining NOT and OR:
   ```ruby
   logged_in = false
   admin = false
   puts !(logged_in || admin)  # Output: true
   ```

---

## **Best Practices**

- Use `&&` and `||` for most logical operations because they have higher precedence and are generally more predictable.
- Use parentheses to make complex conditions easier to read:
  ```ruby
  puts (5 > 3) && (10 < 20)
  ```
- Avoid mixing `and`/`or` with `&&`/`||` to prevent confusion due to precedence differences.

---

With logical and comparison operators, you can build powerful conditional statements and control flows in your Ruby programs. Practice combining these operators to solidify your understanding!


### [Go to practice exercise](./exercise_logical_operatos.md)
These exercises provide hands-on practice with logical and comparison operators. After completing them, check your answers in the solutions file.