## **Creating Your Own Gem**

Creating a gem allows you to share your code with others or use it across multiple projects. Gems are typically created to solve specific problems or provide reusable functionality.

---

### Steps to Create a Gem:

1. **Set Up the Directory Structure**:

```bash
mkdir my_gem
cd my_gem
```

Inside the directory:

```bash
my_gem/
├── lib/
│   └── my_gem.rb
├── my_gem.gemspec
```

2. **Write Your Code**:
In `lib/my_gem.rb`:

```ruby
module MyGem
  def self.greet(name)
    "Hello, #{name}!"
  end
end
```

3. **Define the Gemspec File**:

The `.gemspec` file includes metadata about your gem, such as its name, version, authors, and dependencies.

```ruby
# my_gem.gemspec
Gem::Specification.new do |spec|
  spec.name        = "my_gem"
  spec.version     = "0.1.0"
  spec.summary     = "A simple gem for greeting."
  spec.files       = ["lib/my_gem.rb"]
  spec.authors     = ["Your Name"]
  spec.email       = ["youremail@example.com"]
  spec.homepage    = "https://rubygems.org/gems/my_gem"
end
```

4. **Build and Install the Gem**:

```bash
gem build my_gem.gemspec
gem install my_gem-0.1.0.gem
```

5. **Use Your Gem**:

After installation, you can use your gem like any other:

```ruby
require 'my_gem'
puts MyGem.greet("World")
```

---

### Exercise: Creating a Gem

1. Create a gem named `string_tools`.
2. Add a method `reverse_words(sentence)` that reverses the words in a given sentence.
3. Define the gemspec file with appropriate metadata.
4. Build and install the gem.
5. Write a test script that uses the `string_tools` gem to reverse the words in a sentence and prints the result.

```ruby
# Your code here
```


### [Go to Solutions](./creating_gem_solutions.md)