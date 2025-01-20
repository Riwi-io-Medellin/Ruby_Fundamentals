### Solutions: Creating Your Own Gem

Below are the solutions for the exercise on creating a gem. Compare these with your implementation to ensure accuracy.

---

#### **Solution: Creating the `string_tools` Gem**

1. **Set Up the Directory Structure**:

```bash
mkdir string_tools
cd string_tools
```

Directory structure:

```bash
string_tools/
├── lib/
│   └── string_tools.rb
├── string_tools.gemspec
```

---

2. **Write the Code**:
In `lib/string_tools.rb`:

```ruby
module StringTools
  def self.reverse_words(sentence)
    sentence.split.reverse.join(" ")
  end
end
```

---

3. **Define the Gemspec File**:

In `string_tools.gemspec`:

```ruby
Gem::Specification.new do |spec|
  spec.name        = "string_tools"
  spec.version     = "0.1.0"
  spec.summary     = "A gem to reverse words in a sentence."
  spec.files       = ["lib/string_tools.rb"]
  spec.authors     = ["Your Name"]
  spec.email       = ["youremail@example.com"]
  spec.homepage    = "https://rubygems.org/gems/string_tools"
end
```

---

4. **Build and Install the Gem**:

```bash
gem build string_tools.gemspec
gem install string_tools-0.1.0.gem
```

---

5. **Test the Gem**:
Create a Ruby script `test_string_tools.rb`:

```ruby
require 'string_tools'

sentence = "Hello Ruby World"
reversed = StringTools.reverse_words(sentence)
puts reversed # Output: "World Ruby Hello"
```

Run the script:

```bash
ruby test_string_tools.rb
```

---

By following these steps, you should have successfully created and tested the `string_tools` gem. Gems like this can be expanded with more functionality and distributed for others to use.
