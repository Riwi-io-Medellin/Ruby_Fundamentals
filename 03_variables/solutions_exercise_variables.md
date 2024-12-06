### Solutions

Here are the answers for each exercise. Try not to peek unless you're stuck!

---

#### Solution 1: Local Variables
```ruby
# Define variables
price = 100
discount_percentage = 20

# Calculate the discount amount
discount = price * discount_percentage / 100

# Calculate the total price after discount
total_price = price - discount

# Output the result
puts "The total price after a #{discount_percentage}% discount is: #{total_price}"
```

---

#### Solution 2: Instance Variables
```ruby
class Person
  def initialize(name)
    @name = name
  end

  def introduce
    # Output a greeting with the name
    puts "Hi, my name is #{@name}!"
  end
end

# Create an instance and test the method
person = Person.new("Alice")
person.introduce
```

---

#### Solution 3: Class Variables
```ruby
class Person
  @@count = 0

  def initialize(name)
    @name = name
    # Increment the class variable
    @@count += 1
  end

  def self.count
    # Return the count of instances
    @@count
  end
end

# Create instances and display the count
person1 = Person.new("Alice")
person2 = Person.new("Bob")
puts "Number of people created: #{Person.count}"
```

---

#### Solution 4: Global Variables
```ruby
$method_calls = 0

def call_method
  # Increment the global variable
  $method_calls += 1
end

# Call the method multiple times
3.times { call_method }

# Output the number of method calls
puts "The method was called #{$method_calls} times."
```

---

#### Solution 5: Constants
```ruby
# Define the constant PI
PI = 3.14159

def calculate_area(radius)
  # Use the constant to calculate the area
  area = PI * radius ** 2
  puts "The area of a circle with radius #{radius} is: #{area}"
end

# Test the method
calculate_area(5)
```

---

With these exercises, you'll get hands-on experience with local variables, instance variables, class variables, global variables, and constants in Ruby. Practice until you feel confident!