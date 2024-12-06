### Exercise: Variables in Ruby

Below is a set of exercises designed to help you practice and understand the use of variables in Ruby. Each exercise includes a partially completed code snippet that you need to finish. The solutions are provided at the end for reference, but try to solve them on your own first!

---

#### **Exercise 1: Local Variables**
Complete the code to calculate and display the total price after applying a discount.

```ruby
# Define variables
price = 100
discount_percentage = 20

# Calculate the discount amount
discount = ___________

# Calculate the total price after discount
total_price = ___________

# Output the result
puts "The total price after a #{discount_percentage}% discount is: #{total_price}"
```

---

#### **Exercise 2: Instance Variables**
Define a class `Person` with an instance variable `@name`. Complete the method `introduce` to display the person's name.

```ruby
class Person
  def initialize(name)
    @name = ___________
  end

  def introduce
    # Output a greeting with the name
    puts "Hi, my name is ___________!"
  end
end

# Create an instance and test the method
person = Person.new("Alice")
person.introduce
```

---

#### **Exercise 3: Class Variables**
Complete the code to track the number of `Person` instances created using a class variable.

```ruby
class Person
  @@count = ___________

  def initialize(name)
    @name = name
    # Increment the class variable
    ___________
  end

  def self.count
    # Return the count of instances
    ___________
  end
end

# Create instances and display the count
person1 = Person.new("Alice")
person2 = Person.new("Bob")
puts "Number of people created: #{Person.count}"
```

---

#### **Exercise 4: Global Variables**
Fix the code to correctly use a global variable for counting the number of method calls.

```ruby
$method_calls = ___________

def call_method
  # Increment the global variable
  ___________
end

# Call the method multiple times
3.times { call_method }

# Output the number of method calls
puts "The method was called #{$method_calls} times."
```

---

#### **Exercise 5: Constants**
Define a constant `PI` and use it to calculate the area of a circle with a given radius.

```ruby
# Define the constant PI
PI = ___________

def calculate_area(radius)
  # Use the constant to calculate the area
  area = ___________
  puts "The area of a circle with radius #{radius} is: #{area}"
end

# Test the method
calculate_area(5)
```

---

With these exercises, you'll get hands-on experience with local variables, instance variables, class variables, global variables, and constants in Ruby. Practice until you feel confident!

### . [Exercise solutions](./solutions_exercise_variables.md)

Here you will find the solutions to the proposed exercises. If you don't try to do them on your own, you will never learn. Just use it as a comparison with your proposed solution.