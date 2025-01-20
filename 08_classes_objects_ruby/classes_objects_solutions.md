### Solutions: Classes and Objects in Ruby

Below are the solutions to the exercises on classes and objects. Review these to compare with your implementations.

---

#### **Solution 1: Defining a Class**

```ruby
class Car
  def initialize(make, model, year)
    @make = make
    @model = model
    @year = year
  end

  def info
    "#{@year} #{@make} #{@model}"
  end
end

# Example
car = Car.new("Toyota", "Corolla", 2021)
puts car.info # Output: "2021 Toyota Corolla"
```

---

#### **Solution 2: Instance Methods**

```ruby
class Car
  def start
    puts "The car is starting!"
  end
end

# Example
car = Car.new("Toyota", "Corolla", 2021)
car.start # Output: "The car is starting!"
```

---

#### **Solution 3: Class Methods**

```ruby
class Car
  def self.vehicle_type
    "Automobile"
  end
end

# Example
puts Car.vehicle_type # Output: "Automobile"
```

---

#### **Solution 4: Inheritance**

```ruby
class ElectricCar < Car
  attr_accessor :battery_capacity

  def initialize(make, model, year, battery_capacity)
    super(make, model, year)
    @battery_capacity = battery_capacity
  end

  def charge
    puts "Charging the battery!"
  end
end

# Example
electric_car = ElectricCar.new("Tesla", "Model S", 2022, "100 kWh")
electric_car.charge # Output: "Charging the battery!"
```

---

#### **Solution 5: Using Modules**

```ruby
module Drivable
  def drive
    puts "Driving on the road!"
  end
end

class Car
  include Drivable
end

# Example
car = Car.new("Toyota", "Corolla", 2021)
car.drive # Output: "Driving on the road!"
```

---

#### **Solution 6: Combining Everything**

```ruby
# Create instance of ElectricCar
electric_car = ElectricCar.new("Tesla", "Model S", 2022, "100 kWh")

# Call all methods
puts electric_car.info        # Output: "2022 Tesla Model S"
electric_car.start            # Output: "The car is starting!"
electric_car.drive            # Output: "Driving on the road!"
electric_car.charge           # Output: "Charging the battery!"
```

---

By reviewing these solutions, you can better understand Ruby's classes, objects, inheritance, and mixins. Practice modifying these examples to deepen your skills.