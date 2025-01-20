### Classes and Objects in Ruby

In Ruby, classes and objects are the building blocks of object-oriented programming. They allow you to model real-world entities, encapsulate data, and define behavior through methods.

---

## **1. Defining Classes**

A class in Ruby is defined using the `class` keyword. Inside the class, you can define methods and attributes to represent its behavior and data.

### Syntax:

```ruby
class ClassName
  # Attributes and methods go here
end
```

### Example:

```ruby
class Person
  def initialize(name, age)
    @name = name
    @age = age
  end

  def introduce
    "Hi, my name is #{@name} and I am #{@age} years old."
  end
end

person = Person.new("Alice", 30)
puts person.introduce # Output: Hi, my name is Alice and I am 30 years old.
```

---

## **2. Instance and Class Methods**

### Instance Methods
Instance methods operate on an instance of the class. They are defined using the `def` keyword and can access instance variables using `@`.

```ruby
class Calculator
  def add(a, b)
    a + b
  end
end

calc = Calculator.new
puts calc.add(2, 3) # Output: 5
```

### Class Methods
Class methods operate on the class itself and are defined using `self` or prefixed with `self.`.

```ruby
class MathUtils
  def self.square(number)
    number * number
  end
end

puts MathUtils.square(4) # Output: 16
```

---

## **3. Inheritance and Mixins**

### Inheritance
Inheritance allows a class to inherit behavior and attributes from another class. Use the `<` symbol to specify a parent class.

```ruby
class Animal
  def speak
    "I am an animal."
  end
end

class Dog < Animal
  def speak
    "Woof!"
  end
end

dog = Dog.new
puts dog.speak # Output: Woof!
```

### Mixins with Modules
Modules provide a way to share reusable code across multiple classes. They are included using the `include` keyword.

```ruby
module Swimmable
  def swim
    "I can swim!"
  end
end

class Fish
  include Swimmable
end

fish = Fish.new
puts fish.swim # Output: I can swim!
```

---

For practical exercises and challenges, refer to:

- [Go to exercises: Classes and Objects](./exercise_classes_objects.md)
