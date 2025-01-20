### Data Types and Collections in Ruby

Ruby is a flexible and dynamic programming language, offering a rich set of data types and collections. Understanding these is key to writing efficient and effective Ruby code. This chapter introduces Ruby's fundamental data types, collections, and their uses.

---

## **1. Fundamental Data Types**

### **Strings**
Strings represent sequences of characters. They can be enclosed in single (`'`) or double (`"`) quotes.

#### Key Points:
- Double-quoted strings allow interpolation and escape sequences.
- Single-quoted strings are more literal.

```ruby
# Examples of Strings
greeting = "Hello, Ruby!"
single_quote_example = 'This is a string.'
```

### **Numbers**
Ruby supports integers and floating-point numbers.

#### Key Points:
- Integers (`Fixnum` and `Bignum`) are used for whole numbers.
- Floats represent decimal numbers.

```ruby
# Examples of Numbers
integer_example = 42
float_example = 3.14
```

### **Booleans**
Booleans represent true or false values.

```ruby
# Examples of Booleans
is_ruby_fun = true
is_python_better = false
```

---

## **2. Collections**

### **Arrays**
Arrays store ordered lists of elements.

#### Key Points:
- Elements can be of any type.
- Access elements using their index (starting at 0).

```ruby
# Example of Array
colors = ["red", "green", "blue"]
puts colors[0] # Output: "red"
```

### **Hashes**
Hashes store key-value pairs, similar to dictionaries in other languages.

#### Key Points:
- Keys can be symbols, strings, or any other object.
- Values can be of any type.

```ruby
# Example of Hash
person = { name: "Alice", age: 25, city: "New York" }
puts person[:name] # Output: "Alice"
```

### **Ranges**
Ranges represent sequences with a start and an end.

#### Key Points:
- Defined using `..` (inclusive) or `...` (exclusive).

```ruby
# Example of Range
range = (1..5)
puts range.to_a # Output: [1, 2, 3, 4, 5]
```

---

## **3. Symbols**
Symbols are immutable, reusable constants often used as identifiers or keys.

```ruby
# Example of Symbols
status = :active
```

---

For practical exercises and challenges, refer to:

- [Go to exercises: Data Types and Collections](./exercise_data_types.md)